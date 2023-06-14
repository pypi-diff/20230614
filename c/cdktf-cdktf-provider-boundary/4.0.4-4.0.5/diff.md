# Comparing `tmp/cdktf-cdktf-provider-boundary-4.0.4.tar.gz` & `tmp/cdktf-cdktf-provider-boundary-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-boundary-4.0.4.tar", last modified: Thu Jun  1 14:10:09 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-boundary-4.0.5.tar", last modified: Wed Jun 14 03:16:33 2023, max compression
```

## Comparing `cdktf-cdktf-provider-boundary-4.0.4.tar` & `cdktf-cdktf-provider-boundary-4.0.5.tar`

### file list

```diff
@@ -1,79 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.032792 cdktf-cdktf-provider-boundary-4.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.032792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130913 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@4.0.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account/
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    24539 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account_password/
--rw-r--r--   0 runner    (1001) docker     (123)    27172 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method/
--rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    67707 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method_password/
--rw-r--r--   0 runner    (1001) docker     (123)    27967 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_json/
--rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_library_vault/
--rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/
--rw-r--r--   0 runner    (1001) docker     (123)    28769 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_store_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20210 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_store_vault/
--rw-r--r--   0 runner    (1001) docker     (123)    45180 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_username_password/
--rw-r--r--   0 runner    (1001) docker     (123)    25695 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/group/
--rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host/
--rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    21880 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    45184 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set/
--rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    31425 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set_static/
--rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_static/
--rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/managed_group/
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    32610 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/role/
--rw-r--r--   0 runner    (1001) docker     (123)    27656 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/scope/
--rw-r--r--   0 runner    (1001) docker     (123)    31793 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/scope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/target/
--rw-r--r--   0 runner    (1001) docker     (123)    50852 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/target/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/user/
--rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.040792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/worker/
--rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-06-01 14:09:57.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:10:09.036792 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-01 14:10:08.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 14:10:09.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:10:08.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 14:10:08.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 14:10:08.000000 cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.337278 cdktf-cdktf-provider-boundary-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 03:16:33.337278 cdktf-cdktf-provider-boundary-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.317278 cdktf-cdktf-provider-boundary-4.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.325278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.325278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154991 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@4.0.5.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.325278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account/
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.325278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)    24618 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    24539 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    27416 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method/
+-rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)    93502 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    67707 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    27967 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_json/
+-rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_library_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/
+-rw-r--r--   0 runner    (1001) docker     (123)    28769 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_store_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20210 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_store_vault/
+-rw-r--r--   0 runner    (1001) docker     (123)    45180 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_username_password/
+-rw-r--r--   0 runner    (1001) docker     (123)    25695 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/group/
+-rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host/
+-rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.329278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    21880 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    45184 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set/
+-rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    31425 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    24894 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    24732 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/managed_group/
+-rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/managed_group_ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)    22663 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/managed_group_ldap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    38793 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/role/
+-rw-r--r--   0 runner    (1001) docker     (123)    27656 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)    31793 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/scope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/target/
+-rw-r--r--   0 runner    (1001) docker     (123)    53611 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/target/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.333278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-06-14 03:16:16.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:16:33.325278 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-14 03:16:33.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-14 03:16:33.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:16:33.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-14 03:16:33.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 03:16:33.000000 cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/LICENSE` & `cdktf-cdktf-provider-boundary-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/PKG-INFO` & `cdktf-cdktf-provider-boundary-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-boundary
-Version: 4.0.4
+Version: 4.0.5
 Summary: Prebuilt boundary Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-boundary.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-boundary.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/README.md` & `cdktf-cdktf-provider-boundary-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/setup.py` & `cdktf-cdktf-provider-boundary-4.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-boundary",
-    "version": "4.0.4",
+    "version": "4.0.5",
     "description": "Prebuilt boundary Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-boundary.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -20,17 +20,19 @@
     "package_dir": {
         "": "src"
     },
     "packages": [
         "cdktf_cdktf_provider_boundary",
         "cdktf_cdktf_provider_boundary._jsii",
         "cdktf_cdktf_provider_boundary.account",
+        "cdktf_cdktf_provider_boundary.account_ldap",
         "cdktf_cdktf_provider_boundary.account_oidc",
         "cdktf_cdktf_provider_boundary.account_password",
         "cdktf_cdktf_provider_boundary.auth_method",
+        "cdktf_cdktf_provider_boundary.auth_method_ldap",
         "cdktf_cdktf_provider_boundary.auth_method_oidc",
         "cdktf_cdktf_provider_boundary.auth_method_password",
         "cdktf_cdktf_provider_boundary.credential_json",
         "cdktf_cdktf_provider_boundary.credential_library_vault",
         "cdktf_cdktf_provider_boundary.credential_library_vault_ssh_certificate",
         "cdktf_cdktf_provider_boundary.credential_ssh_private_key",
         "cdktf_cdktf_provider_boundary.credential_store_static",
@@ -42,34 +44,35 @@
         "cdktf_cdktf_provider_boundary.host_catalog_plugin",
         "cdktf_cdktf_provider_boundary.host_catalog_static",
         "cdktf_cdktf_provider_boundary.host_set",
         "cdktf_cdktf_provider_boundary.host_set_plugin",
         "cdktf_cdktf_provider_boundary.host_set_static",
         "cdktf_cdktf_provider_boundary.host_static",
         "cdktf_cdktf_provider_boundary.managed_group",
+        "cdktf_cdktf_provider_boundary.managed_group_ldap",
         "cdktf_cdktf_provider_boundary.provider",
         "cdktf_cdktf_provider_boundary.role",
         "cdktf_cdktf_provider_boundary.scope",
         "cdktf_cdktf_provider_boundary.target",
         "cdktf_cdktf_provider_boundary.user",
         "cdktf_cdktf_provider_boundary.worker"
     ],
     "package_data": {
         "cdktf_cdktf_provider_boundary._jsii": [
-            "provider-boundary@4.0.4.jsii.tgz"
+            "provider-boundary@4.0.5.jsii.tgz"
         ],
         "cdktf_cdktf_provider_boundary": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.16.3, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.81.0, <2.0.0",
+        "jsii>=1.83.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,19 @@
 
 from typeguard import check_type
 
 from ._jsii import *
 
 __all__ = [
     "account",
+    "account_ldap",
     "account_oidc",
     "account_password",
     "auth_method",
+    "auth_method_ldap",
     "auth_method_oidc",
     "auth_method_password",
     "credential_json",
     "credential_library_vault",
     "credential_library_vault_ssh_certificate",
     "credential_ssh_private_key",
     "credential_store_static",
@@ -126,29 +128,32 @@
     "host_catalog_plugin",
     "host_catalog_static",
     "host_set",
     "host_set_plugin",
     "host_set_static",
     "host_static",
     "managed_group",
+    "managed_group_ldap",
     "provider",
     "role",
     "scope",
     "target",
     "user",
     "worker",
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
 from . import account
+from . import account_ldap
 from . import account_oidc
 from . import account_password
 from . import auth_method
+from . import auth_method_ldap
 from . import auth_method_oidc
 from . import auth_method_password
 from . import credential_json
 from . import credential_library_vault
 from . import credential_library_vault_ssh_certificate
 from . import credential_ssh_private_key
 from . import credential_store_static
@@ -160,13 +165,14 @@
 from . import host_catalog_plugin
 from . import host_catalog_static
 from . import host_set
 from . import host_set_plugin
 from . import host_set_static
 from . import host_static
 from . import managed_group
+from . import managed_group_ldap
 from . import provider
 from . import role
 from . import scope
 from . import target
 from . import user
 from . import worker
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_account`
 
-Refer to the Terraform Registory for docs: [`boundary_account`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account).
+Refer to the Terraform Registory for docs: [`boundary_account`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Account(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.account.Account",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account boundary_account}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account boundary_account}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account boundary_account} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account boundary_account} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#auth_method_id Account#auth_method_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#type Account#type}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#description Account#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#login_name Account#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#name Account#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#password Account#password}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#auth_method_id Account#auth_method_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#type Account#type}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#description Account#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#login_name Account#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#name Account#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#password Account#password}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -261,20 +261,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#auth_method_id Account#auth_method_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#type Account#type}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#description Account#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#login_name Account#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#name Account#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#password Account#password}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#auth_method_id Account#auth_method_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#type Account#type}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#description Account#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#login_name Account#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#name Account#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#password Account#password}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9f3a78290e59f53f12897f7e509e444fe46777e5e9e4d9f11c486df5264a6d41)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -380,62 +380,62 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#auth_method_id Account#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#auth_method_id Account#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#type Account#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#type Account#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#description Account#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#description Account#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def login_name(self) -> typing.Optional[builtins.str]:
         '''The login name for this account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#login_name Account#login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#login_name Account#login_name}
         '''
         result = self._values.get("login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#name Account#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#name Account#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''The account password. Only set on create, changes will not be reflected when updating account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account#password Account#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account#password Account#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_account_oidc`
 
-Refer to the Terraform Registory for docs: [`boundary_account_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc).
+Refer to the Terraform Registory for docs: [`boundary_account_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AccountOidc(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.accountOidc.AccountOidc",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc boundary_account_oidc}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc boundary_account_oidc}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc boundary_account_oidc} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc boundary_account_oidc} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#description AccountOidc#description}
-        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#issuer AccountOidc#issuer}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#name AccountOidc#name}
-        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#subject AccountOidc#subject}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#description AccountOidc#description}
+        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#issuer AccountOidc#issuer}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#name AccountOidc#name}
+        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#subject AccountOidc#subject}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -239,19 +239,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#description AccountOidc#description}
-        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#issuer AccountOidc#issuer}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#name AccountOidc#name}
-        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#subject AccountOidc#subject}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#description AccountOidc#description}
+        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#issuer AccountOidc#issuer}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#name AccountOidc#name}
+        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#subject AccountOidc#subject}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5a9f2ecb8fb73ab43552aa884097a49be5578a649f7b9437164ada5cd9d24ded)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -355,52 +355,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#description AccountOidc#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#description AccountOidc#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def issuer(self) -> typing.Optional[builtins.str]:
         '''The OIDC issuer.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#issuer AccountOidc#issuer}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#issuer AccountOidc#issuer}
         '''
         result = self._values.get("issuer")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#name AccountOidc#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#name AccountOidc#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def subject(self) -> typing.Optional[builtins.str]:
         '''The OIDC subject.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_oidc#subject AccountOidc#subject}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_oidc#subject AccountOidc#subject}
         '''
         result = self._values.get("subject")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/account_password/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/account_password/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_account_password`
 
-Refer to the Terraform Registory for docs: [`boundary_account_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password).
+Refer to the Terraform Registory for docs: [`boundary_account_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,64 +22,64 @@
 
 
 class AccountPassword(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.accountPassword.AccountPassword",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password boundary_account_password}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password boundary_account_password}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
-        type: builtins.str,
         description: typing.Optional[builtins.str] = None,
         login_name: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         password: typing.Optional[builtins.str] = None,
+        type: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password boundary_account_password} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password boundary_account_password} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#type AccountPassword#type}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#description AccountPassword#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#login_name AccountPassword#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#name AccountPassword#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#password AccountPassword#password}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#description AccountPassword#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#login_name AccountPassword#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#name AccountPassword#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#password AccountPassword#password}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#type AccountPassword#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__de5579060aaa808bca337fff86591ab9d221b8b3b2f5f5138c853d8101b24931)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = AccountPasswordConfig(
             auth_method_id=auth_method_id,
-            type=type,
             description=description,
             login_name=login_name,
             name=name,
             password=password,
+            type=type,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
@@ -99,14 +99,18 @@
     def reset_name(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetName", []))
 
     @jsii.member(jsii_name="resetPassword")
     def reset_password(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPassword", []))
 
+    @jsii.member(jsii_name="resetType")
+    def reset_type(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetType", []))
+
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
@@ -228,74 +232,73 @@
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "auth_method_id": "authMethodId",
-        "type": "type",
         "description": "description",
         "login_name": "loginName",
         "name": "name",
         "password": "password",
+        "type": "type",
     },
 )
 class AccountPasswordConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         auth_method_id: builtins.str,
-        type: builtins.str,
         description: typing.Optional[builtins.str] = None,
         login_name: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         password: typing.Optional[builtins.str] = None,
+        type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#type AccountPassword#type}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#description AccountPassword#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#login_name AccountPassword#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#name AccountPassword#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#password AccountPassword#password}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#description AccountPassword#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#login_name AccountPassword#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#name AccountPassword#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#password AccountPassword#password}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#type AccountPassword#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9b0bbd75ce8fded2755ce13d83166390b51916ecaf627f133149858f88c5f382)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument auth_method_id", value=auth_method_id, expected_type=type_hints["auth_method_id"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument login_name", value=login_name, expected_type=type_hints["login_name"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "auth_method_id": auth_method_id,
-            "type": type,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -311,14 +314,16 @@
             self._values["description"] = description
         if login_name is not None:
             self._values["login_name"] = login_name
         if name is not None:
             self._values["name"] = name
         if password is not None:
             self._values["password"] = password
+        if type is not None:
+            self._values["type"] = type
 
     @builtins.property
     def connection(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
         '''
         :stability: experimental
@@ -380,66 +385,65 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def type(self) -> builtins.str:
-        '''The resource type.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#type AccountPassword#type}
-        '''
-        result = self._values.get("type")
-        assert result is not None, "Required property 'type' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#description AccountPassword#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#description AccountPassword#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def login_name(self) -> typing.Optional[builtins.str]:
         '''The login name for this account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#login_name AccountPassword#login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#login_name AccountPassword#login_name}
         '''
         result = self._values.get("login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#name AccountPassword#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#name AccountPassword#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''The account password. Only set on create, changes will not be reflected when updating account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/account_password#password AccountPassword#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#password AccountPassword#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def type(self) -> typing.Optional[builtins.str]:
+        '''The resource type.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/account_password#type AccountPassword#type}
+        '''
+        result = self._values.get("type")
+        return typing.cast(typing.Optional[builtins.str], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -456,19 +460,19 @@
 publication.publish()
 
 def _typecheckingstub__de5579060aaa808bca337fff86591ab9d221b8b3b2f5f5138c853d8101b24931(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     auth_method_id: builtins.str,
-    type: builtins.str,
     description: typing.Optional[builtins.str] = None,
     login_name: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     password: typing.Optional[builtins.str] = None,
+    type: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
@@ -518,15 +522,15 @@
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     auth_method_id: builtins.str,
-    type: builtins.str,
     description: typing.Optional[builtins.str] = None,
     login_name: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     password: typing.Optional[builtins.str] = None,
+    type: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_auth_method`
 
-Refer to the Terraform Registory for docs: [`boundary_auth_method`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method).
+Refer to the Terraform Registory for docs: [`boundary_auth_method`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AuthMethod(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethod.AuthMethod",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method boundary_auth_method}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method boundary_auth_method}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method boundary_auth_method} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method boundary_auth_method} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#scope_id AuthMethod#scope_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#type AuthMethod#type}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#description AuthMethod#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#name AuthMethod#name}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#scope_id AuthMethod#scope_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#type AuthMethod#type}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#description AuthMethod#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#name AuthMethod#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -261,20 +261,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#scope_id AuthMethod#scope_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#type AuthMethod#type}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#description AuthMethod#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#name AuthMethod#name}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#scope_id AuthMethod#scope_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#type AuthMethod#type}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#description AuthMethod#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#name AuthMethod#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1dbc89045cef41c40c62b2ae4f0b26d37995a7c431554876680e5a3612faa380)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -380,62 +380,62 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#scope_id AuthMethod#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#scope_id AuthMethod#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#type AuthMethod#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#type AuthMethod#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#description AuthMethod#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#description AuthMethod#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def min_login_name_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum login name length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
         '''
         result = self._values.get("min_login_name_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def min_password_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum password length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
         '''
         result = self._values.get("min_password_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method#name AuthMethod#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method#name AuthMethod#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_auth_method_oidc`
 
-Refer to the Terraform Registory for docs: [`boundary_auth_method_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc).
+Refer to the Terraform Registory for docs: [`boundary_auth_method_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AuthMethodOidc(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethodOidc.AuthMethodOidc",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc boundary_auth_method_oidc}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc boundary_auth_method_oidc}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -56,37 +56,37 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc boundary_auth_method_oidc} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc boundary_auth_method_oidc} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
-        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
-        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
-        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
-        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
-        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
-        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
-        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
-        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
-        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
-        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
-        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
-        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
-        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
-        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
-        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
-        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
+        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
+        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
+        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
+        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
+        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
+        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
+        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
+        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
+        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
+        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
+        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
+        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
+        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
+        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
+        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
+        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -617,33 +617,33 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
-        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
-        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
-        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
-        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
-        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
-        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
-        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
-        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
-        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
-        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
-        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
-        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
-        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
-        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
-        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
-        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
+        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
+        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
+        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
+        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
+        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
+        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
+        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
+        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
+        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
+        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
+        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
+        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
+        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
+        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
+        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
+        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__109748e397e8bf3db45cc8c8ef5e0c5cd569f2720acf7de41e15cd8807f5d1a5)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -789,192 +789,192 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def account_claim_maps(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Account claim maps for the to_claim of sub.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
         '''
         result = self._values.get("account_claim_maps")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def allowed_audiences(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Audiences for which the provider responses will be allowed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
         '''
         result = self._values.get("allowed_audiences")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def api_url_prefix(self) -> typing.Optional[builtins.str]:
         '''The API prefix to use when generating callback URLs for the provider.
 
         Should be set to an address at which the provider can reach back to the controller.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
         '''
         result = self._values.get("api_url_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def callback_url(self) -> typing.Optional[builtins.str]:
         '''The URL that should be provided to the IdP for callbacks.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
         '''
         result = self._values.get("callback_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def claims_scopes(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Claims scopes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
         '''
         result = self._values.get("claims_scopes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def client_id(self) -> typing.Optional[builtins.str]:
         '''The client ID assigned to this auth method from the provider.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
         '''
         result = self._values.get("client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_secret(self) -> typing.Optional[builtins.str]:
         '''The secret key assigned to this auth method from the provider.
 
         Once set, only the hash will be kept and the original value can be removed from configuration.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
         '''
         result = self._values.get("client_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_secret_hmac(self) -> typing.Optional[builtins.str]:
         '''The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
         '''
         result = self._values.get("client_secret_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def disable_discovered_config_validation(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here.
 
         The validation is only performed at create or update time.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
         '''
         result = self._values.get("disable_discovered_config_validation")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def idp_ca_certs(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of CA certificates to trust when validating the IdP's token signatures.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
         '''
         result = self._values.get("idp_ca_certs")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def is_primary_for_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, makes this auth method the primary auth method for the scope in which it resides.
 
         The primary auth method for a scope means the user will be automatically created when they login using an OIDC account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
         '''
         result = self._values.get("is_primary_for_scope")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def issuer(self) -> typing.Optional[builtins.str]:
         '''The issuer corresponding to the provider, which must match the issuer field in generated tokens.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
         '''
         result = self._values.get("issuer")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_age(self) -> typing.Optional[jsii.Number]:
         '''The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again.
 
         A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
         '''
         result = self._values.get("max_age")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def signing_algorithms(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Allowed signing algorithms for the provider's issued tokens.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
         '''
         result = self._values.get("signing_algorithms")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def state(self) -> typing.Optional[builtins.str]:
         '''Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
         '''
         result = self._values.get("state")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of auth method; hardcoded.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_auth_method_password`
 
-Refer to the Terraform Registory for docs: [`boundary_auth_method_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password).
+Refer to the Terraform Registory for docs: [`boundary_auth_method_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class AuthMethodPassword(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethodPassword.AuthMethodPassword",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password boundary_auth_method_password}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password boundary_auth_method_password}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password boundary_auth_method_password} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password boundary_auth_method_password} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#description AuthMethodPassword#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#name AuthMethodPassword#name}
-        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#type AuthMethodPassword#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#description AuthMethodPassword#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#name AuthMethodPassword#name}
+        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#type AuthMethodPassword#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -265,20 +265,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#description AuthMethodPassword#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#name AuthMethodPassword#name}
-        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#type AuthMethodPassword#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#description AuthMethodPassword#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#name AuthMethodPassword#name}
+        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#type AuthMethodPassword#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__af88e38a2d8da29c1ca22bf38935f935319c8c7e54482070ed6059cf1b1914ae)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -385,61 +385,61 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#description AuthMethodPassword#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#description AuthMethodPassword#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def min_login_name_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum login name length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
         '''
         result = self._values.get("min_login_name_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def min_password_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum password length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
         '''
         result = self._values.get("min_password_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#name AuthMethodPassword#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#name AuthMethodPassword#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The resource type, hardcoded per resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/auth_method_password#type AuthMethodPassword#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/auth_method_password#type AuthMethodPassword#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_json`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_json`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json).
+Refer to the Terraform Registory for docs: [`boundary_credential_json`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialJson(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialJson.CredentialJson",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json boundary_credential_json}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json boundary_credential_json}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json boundary_credential_json} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json boundary_credential_json} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
-        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#object CredentialJson#object}
-        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#description CredentialJson#description}
-        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#name CredentialJson#name}
+        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
+        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#object CredentialJson#object}
+        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#description CredentialJson#description}
+        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#name CredentialJson#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -214,18 +214,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
-        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#object CredentialJson#object}
-        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#description CredentialJson#description}
-        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#name CredentialJson#name}
+        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
+        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#object CredentialJson#object}
+        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#description CredentialJson#description}
+        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#name CredentialJson#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__340d4278104f6afbd7bb239bf58cb0463b6ea62d015f46764886dc09702f25f7)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -325,46 +325,46 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The credential store in which to save this json credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def object(self) -> builtins.str:
         '''The object for the this json credential.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#object CredentialJson#object}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#object CredentialJson#object}
         '''
         result = self._values.get("object")
         assert result is not None, "Required property 'object' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of this json credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#description CredentialJson#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#description CredentialJson#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of this json credential. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_json#name CredentialJson#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_json#name CredentialJson#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_library_vault`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_library_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault).
+Refer to the Terraform Registory for docs: [`boundary_credential_library_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialLibraryVault(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialLibraryVault.CredentialLibraryVault",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault boundary_credential_library_vault}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault boundary_credential_library_vault}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault boundary_credential_library_vault} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault boundary_credential_library_vault} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
-        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
-        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
-        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
-        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
+        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
+        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
+        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
+        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -320,22 +320,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
-        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
-        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
-        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
-        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
+        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
+        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
+        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
+        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__91de0f894b7ba615dddb6aca0eb531c0b3eb874ab7cf11ccd93bc0005f9d79fb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -447,84 +447,84 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The ID of the credential store that this library belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def path(self) -> builtins.str:
         '''The path in Vault to request credentials from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
         '''
         result = self._values.get("path")
         assert result is not None, "Required property 'path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def credential_mapping_overrides(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''The credential mapping override.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
         '''
         result = self._values.get("credential_mapping_overrides")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def credential_type(self) -> typing.Optional[builtins.str]:
         '''The type of credential the library generates. Cannot be updated on an existing resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
         '''
         result = self._values.get("credential_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def http_method(self) -> typing.Optional[builtins.str]:
         '''The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
         '''
         result = self._values.get("http_method")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def http_request_body(self) -> typing.Optional[builtins.str]:
         '''The body of the HTTP request the library sends to Vault when requesting credentials.
 
         Only valid if ``http_method`` is set to ``POST``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
         '''
         result = self._values.get("http_request_body")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_library_vault_ssh_certificate`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_library_vault_ssh_certificate`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate).
+Refer to the Terraform Registory for docs: [`boundary_credential_library_vault_ssh_certificate`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialLibraryVaultSshCertificate(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialLibraryVaultSshCertificate.CredentialLibraryVaultSshCertificate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
-        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
-        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
-        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
-        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
-        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
-        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
-        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
+        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
+        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
+        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
+        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
+        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
+        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
+        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -396,25 +396,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
-        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
-        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
-        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
-        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
-        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
-        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
-        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
+        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
+        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
+        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
+        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
+        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
+        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
+        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07a8dcdd30946ca78931edfad9b73c37ebdc6bbf6b64db6c12efef586c5bdaeb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -534,110 +534,110 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The ID of the credential store that this library belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def path(self) -> builtins.str:
         '''The path in Vault to request credentials from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
         '''
         result = self._values.get("path")
         assert result is not None, "Required property 'path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username to use with the certificate returned by the library.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def critical_options(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Specifies a map of the critical options that the certificate should be signed for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
         '''
         result = self._values.get("critical_options")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def extensions(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Specifies a map of the extensions that the certificate should be signed for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
         '''
         result = self._values.get("extensions")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def key_bits(self) -> typing.Optional[jsii.Number]:
         '''Specifies the number of bits to use for the generated keys.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
         '''
         result = self._values.get("key_bits")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def key_id(self) -> typing.Optional[builtins.str]:
         '''Specifies the key id a certificate should have.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
         '''
         result = self._values.get("key_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def key_type(self) -> typing.Optional[builtins.str]:
         '''Specifies the desired key type; must be ed25519, ecdsa, or rsa.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
         '''
         result = self._values.get("key_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[builtins.str]:
         '''Specifies the requested time to live for a certificate returned from the library.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_ssh_private_key`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_ssh_private_key`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key).
+Refer to the Terraform Registory for docs: [`boundary_credential_ssh_private_key`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialSshPrivateKey(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialSshPrivateKey.CredentialSshPrivateKey",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
-        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
-        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
-        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
-        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
-        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
+        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
+        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
+        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
+        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
+        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
+        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -267,20 +267,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
-        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
-        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
-        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
-        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
-        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
+        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
+        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
+        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
+        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
+        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
+        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__30a5df1330fa363ae15ceeafc3730ab842c6721e89ade7fcc4b7d65e0db69db4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -385,63 +385,63 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''ID of the credential store this credential belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def private_key(self) -> builtins.str:
         '''The private key associated with the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
         '''
         result = self._values.get("private_key")
         assert result is not None, "Required property 'private_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username associated with the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the credential. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def private_key_passphrase(self) -> typing.Optional[builtins.str]:
         '''The passphrase of the private key associated with the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
         '''
         result = self._values.get("private_key_passphrase")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_store_static`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_store_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static).
+Refer to the Terraform Registory for docs: [`boundary_credential_store_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialStoreStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialStoreStatic.CredentialStoreStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static boundary_credential_store_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static boundary_credential_store_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -40,21 +40,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static boundary_credential_store_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static boundary_credential_store_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
-        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#description CredentialStoreStatic#description}
-        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#name CredentialStoreStatic#name}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
+        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#description CredentialStoreStatic#description}
+        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#name CredentialStoreStatic#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -187,17 +187,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
-        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#description CredentialStoreStatic#description}
-        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#name CredentialStoreStatic#name}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
+        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#description CredentialStoreStatic#description}
+        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#name CredentialStoreStatic#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9199286378c9cad7567fbfde5ad647f35cde57753384ceb6f5f8980c1bcd491a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -295,34 +295,34 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope for this credential store.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The static credential store description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#description CredentialStoreStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#description CredentialStoreStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The static credential store name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_static#name CredentialStoreStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_static#name CredentialStoreStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_store_vault`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_store_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault).
+Refer to the Terraform Registory for docs: [`boundary_credential_store_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialStoreVault(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialStoreVault.CredentialStoreVault",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault boundary_credential_store_vault}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault boundary_credential_store_vault}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         address: builtins.str,
@@ -49,30 +49,30 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault boundary_credential_store_vault} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault boundary_credential_store_vault} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#address CredentialStoreVault#address}
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
-        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#token CredentialStoreVault#token}
-        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
-        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
-        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
-        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#description CredentialStoreVault#description}
-        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#name CredentialStoreVault#name}
-        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
-        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
-        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
-        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
+        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#address CredentialStoreVault#address}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
+        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#token CredentialStoreVault#token}
+        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
+        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
+        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
+        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#description CredentialStoreVault#description}
+        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#name CredentialStoreVault#name}
+        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
+        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
+        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
+        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -430,26 +430,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#address CredentialStoreVault#address}
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
-        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#token CredentialStoreVault#token}
-        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
-        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
-        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
-        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#description CredentialStoreVault#description}
-        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#name CredentialStoreVault#name}
-        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
-        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
-        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
-        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
+        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#address CredentialStoreVault#address}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
+        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#token CredentialStoreVault#token}
+        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
+        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
+        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
+        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#description CredentialStoreVault#description}
+        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#name CredentialStoreVault#name}
+        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
+        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
+        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
+        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__98b4ccd3b8d782228826e5520d5bbf05d295e8cc284d74dbfbe4630aaff8c9ef)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -572,121 +572,121 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def address(self) -> builtins.str:
         '''The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#address CredentialStoreVault#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#address CredentialStoreVault#address}
         '''
         result = self._values.get("address")
         assert result is not None, "Required property 'address' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope for this credential store.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def token(self) -> builtins.str:
         '''A token used for accessing Vault.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#token CredentialStoreVault#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#token CredentialStoreVault#token}
         '''
         result = self._values.get("token")
         assert result is not None, "Required property 'token' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ca_cert(self) -> typing.Optional[builtins.str]:
         '''A PEM-encoded CA certificate to verify the Vault server's TLS certificate.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
         '''
         result = self._values.get("ca_cert")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate(self) -> typing.Optional[builtins.str]:
         '''A PEM-encoded client certificate to use for TLS authentication to the Vault server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
         '''
         result = self._values.get("client_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate_key(self) -> typing.Optional[builtins.str]:
         '''A PEM-encoded private key matching the client certificate from 'client_certificate'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
         '''
         result = self._values.get("client_certificate_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The Vault credential store description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#description CredentialStoreVault#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#description CredentialStoreVault#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The Vault credential store name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#name CredentialStoreVault#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#name CredentialStoreVault#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''The namespace within Vault to use.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tls_server_name(self) -> typing.Optional[builtins.str]:
         '''Name to use as the SNI host when connecting to Vault via TLS.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
         '''
         result = self._values.get("tls_server_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tls_skip_verify(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to skip TLS verification.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
         '''
         result = self._values.get("tls_skip_verify")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def worker_filter(self) -> typing.Optional[builtins.str]:
         '''HCP Only.
 
         A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
         '''
         result = self._values.get("worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_credential_username_password`
 
-Refer to the Terraform Registory for docs: [`boundary_credential_username_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password).
+Refer to the Terraform Registory for docs: [`boundary_credential_username_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class CredentialUsernamePassword(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialUsernamePassword.CredentialUsernamePassword",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password boundary_credential_username_password}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password boundary_credential_username_password}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password boundary_credential_username_password} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password boundary_credential_username_password} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
-        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
-        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
-        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
-        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
+        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
+        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
+        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
+        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
+        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -236,19 +236,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
-        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
-        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
-        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
-        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
+        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
+        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
+        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
+        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
+        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ffd92fc256fbcf6b17cc68b6fbac14f8859e600b946cff80399bbbf4c2cc960d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -350,54 +350,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The credential store in which to save this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def password(self) -> builtins.str:
         '''The password of this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
         '''
         result = self._values.get("password")
         assert result is not None, "Required property 'password' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username of this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of this username/password credential. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/group/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/group/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_group`
 
-Refer to the Terraform Registory for docs: [`boundary_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group).
+Refer to the Terraform Registory for docs: [`boundary_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Group(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.group.Group",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group boundary_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group boundary_group}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group boundary_group} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group boundary_group} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#scope_id Group#scope_id}
-        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#description Group#description}
-        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#member_ids Group#member_ids}
-        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#name Group#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#scope_id Group#scope_id}
+        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#description Group#description}
+        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#member_ids Group#member_ids}
+        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#name Group#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -213,18 +213,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#scope_id Group#scope_id}
-        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#description Group#description}
-        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#member_ids Group#member_ids}
-        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#name Group#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#scope_id Group#scope_id}
+        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#description Group#description}
+        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#member_ids Group#member_ids}
+        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#name Group#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4db7560a2c3e5e1eedd9ad833302c92daa20a64a18b6ee019a618c9566a07e3d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -325,43 +325,43 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#scope_id Group#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#scope_id Group#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The group description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#description Group#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#description Group#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def member_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Resource IDs for group members, these are most likely boundary users.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#member_ids Group#member_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#member_ids Group#member_ids}
         '''
         result = self._values.get("member_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The group name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/group#name Group#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/group#name Group#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_host`
 
-Refer to the Terraform Registory for docs: [`boundary_host`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host).
+Refer to the Terraform Registory for docs: [`boundary_host`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Host(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.host.Host",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host boundary_host}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host boundary_host}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host boundary_host} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host boundary_host} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#host_catalog_id Host#host_catalog_id}.
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#type Host#type}
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#address Host#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#description Host#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#name Host#name}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#host_catalog_id Host#host_catalog_id}.
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#type Host#type}
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#address Host#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#description Host#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#name Host#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -235,19 +235,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#host_catalog_id Host#host_catalog_id}.
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#type Host#type}
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#address Host#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#description Host#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#name Host#name}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#host_catalog_id Host#host_catalog_id}.
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#type Host#type}
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#address Host#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#description Host#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#name Host#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ebe99a87ead3c0ce0b9de7f0dc233a854652e290cf41e96b1c672f05484d1724)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,52 +348,52 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#host_catalog_id Host#host_catalog_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#host_catalog_id Host#host_catalog_id}.'''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of host.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#type Host#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#type Host#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address(self) -> typing.Optional[builtins.str]:
         '''The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#address Host#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#address Host#address}
         '''
         result = self._values.get("address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#description Host#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#description Host#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host#name Host#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host#name Host#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `boundary_host_catalog`
+# `boundary_host_catalog_static`
 
-Refer to the Terraform Registory for docs: [`boundary_host_catalog`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog).
+Refer to the Terraform Registory for docs: [`boundary_host_catalog_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,61 +17,58 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class HostCatalog(
+class HostCatalogStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-boundary.hostCatalog.HostCatalog",
+    jsii_type="@cdktf/provider-boundary.hostCatalogStatic.HostCatalogStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog boundary_host_catalog}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static boundary_host_catalog_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
-        type: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog boundary_host_catalog} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static boundary_host_catalog_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
-        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#type HostCatalog#type}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#description HostCatalog#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#name HostCatalog#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#description HostCatalogStatic#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#name HostCatalogStatic#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2e5a603f24f85d861e36f78fe548cde1b229c531c6c480cdb3dc6a0f29b5e770)
+            type_hints = typing.get_type_hints(_typecheckingstub__d41f660fd85a2635912920a4015b2e8bd24eca13307839327f80a04185608194)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        config = HostCatalogConfig(
+        config = HostCatalogStaticConfig(
             scope_id=scope_id,
-            type=type,
             description=description,
             name=name,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
@@ -115,131 +112,109 @@
 
     @builtins.property
     @jsii.member(jsii_name="scopeIdInput")
     def scope_id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "scopeIdInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="typeInput")
-    def type_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "typeInput"))
-
-    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "description"))
 
     @description.setter
     def description(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6f6284e6fb158527fc7a971ac6d6aa56c01d0c737e7f775385eda3704af24574)
+            type_hints = typing.get_type_hints(_typecheckingstub__0a3b7fff3c8db282b163e11fc5ec154f1bcdd929a5e6ee1f887a2d6821fbe72b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__975d07e0347b24b60dd1e24363bd0ef2bcfcd54dda0b162c72ee2a357056e5bc)
+            type_hints = typing.get_type_hints(_typecheckingstub__6a2518c7bd56f199c607e63841f8c602ef02588504de753de49c6e3a7546c98e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
     @jsii.member(jsii_name="scopeId")
     def scope_id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "scopeId"))
 
     @scope_id.setter
     def scope_id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8748d7d3baea6e1c846f9150d355d7ce536b709aa7f885f4db6ff6198ee3c09b)
+            type_hints = typing.get_type_hints(_typecheckingstub__68bb8739c944268e14f549fefe3781504df124b22514a2fb1df25b81bdc01365)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scopeId", value)
 
-    @builtins.property
-    @jsii.member(jsii_name="type")
-    def type(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "type"))
-
-    @type.setter
-    def type(self, value: builtins.str) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3ff5a6d1fcaf1c6ff8ebca34155f86880ecb37700cd68f383388702dd552223d)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "type", value)
-
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-boundary.hostCatalog.HostCatalogConfig",
+    jsii_type="@cdktf/provider-boundary.hostCatalogStatic.HostCatalogStaticConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "scope_id": "scopeId",
-        "type": "type",
         "description": "description",
         "name": "name",
     },
 )
-class HostCatalogConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class HostCatalogStaticConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         scope_id: builtins.str,
-        type: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
-        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#type HostCatalog#type}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#description HostCatalog#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#name HostCatalog#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#description HostCatalogStatic#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#name HostCatalogStatic#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__221287db26b11bf22cb1c1861301eb80b842c76934da2dfbe1504d9975a77502)
+            type_hints = typing.get_type_hints(_typecheckingstub__b9383c014a702a29d2bd6b4cb2cb8ffbdb1a1941e41b5c6c21399d435f4054ea)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument scope_id", value=scope_id, expected_type=type_hints["scope_id"])
-            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "scope_id": scope_id,
-            "type": type,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -320,119 +295,101 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def type(self) -> builtins.str:
-        '''The host catalog type. Only ``static`` is supported.
-
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#type HostCatalog#type}
-        '''
-        result = self._values.get("type")
-        assert result is not None, "Required property 'type' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host catalog description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#description HostCatalog#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#description HostCatalogStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host catalog name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog#name HostCatalog#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_static#name HostCatalogStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "HostCatalogConfig(%s)" % ", ".join(
+        return "HostCatalogStaticConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "HostCatalog",
-    "HostCatalogConfig",
+    "HostCatalogStatic",
+    "HostCatalogStaticConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__2e5a603f24f85d861e36f78fe548cde1b229c531c6c480cdb3dc6a0f29b5e770(
+def _typecheckingstub__d41f660fd85a2635912920a4015b2e8bd24eca13307839327f80a04185608194(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     scope_id: builtins.str,
-    type: builtins.str,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6f6284e6fb158527fc7a971ac6d6aa56c01d0c737e7f775385eda3704af24574(
-    value: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__975d07e0347b24b60dd1e24363bd0ef2bcfcd54dda0b162c72ee2a357056e5bc(
+def _typecheckingstub__0a3b7fff3c8db282b163e11fc5ec154f1bcdd929a5e6ee1f887a2d6821fbe72b(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8748d7d3baea6e1c846f9150d355d7ce536b709aa7f885f4db6ff6198ee3c09b(
+def _typecheckingstub__6a2518c7bd56f199c607e63841f8c602ef02588504de753de49c6e3a7546c98e(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3ff5a6d1fcaf1c6ff8ebca34155f86880ecb37700cd68f383388702dd552223d(
+def _typecheckingstub__68bb8739c944268e14f549fefe3781504df124b22514a2fb1df25b81bdc01365(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__221287db26b11bf22cb1c1861301eb80b842c76934da2dfbe1504d9975a77502(
+def _typecheckingstub__b9383c014a702a29d2bd6b4cb2cb8ffbdb1a1941e41b5c6c21399d435f4054ea(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     scope_id: builtins.str,
-    type: builtins.str,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_host_catalog_plugin`
 
-Refer to the Terraform Registory for docs: [`boundary_host_catalog_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin).
+Refer to the Terraform Registory for docs: [`boundary_host_catalog_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HostCatalogPlugin(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostCatalogPlugin.HostCatalogPlugin",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin boundary_host_catalog_plugin}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin boundary_host_catalog_plugin}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -48,29 +48,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin boundary_host_catalog_plugin} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin boundary_host_catalog_plugin} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
-        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
-        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
-        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
-        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
-        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
-        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
-        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
-        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
+        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
+        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
+        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
+        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
+        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
+        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
+        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
+        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -397,25 +397,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
-        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
-        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
-        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
-        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
-        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
-        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
-        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
-        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
+        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
+        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
+        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
+        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
+        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
+        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
+        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
+        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__352355fe94a5287d3aa37ee520dadb07588b2f1dd967fdfb5d4b31e89e6ad83a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -537,112 +537,112 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attributes_json(self) -> typing.Optional[builtins.str]:
         '''The attributes for the host catalog.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
         '''
         result = self._values.get("attributes_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host catalog description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def internal_force_update(self) -> typing.Optional[builtins.str]:
         '''Internal only. Used to force update so that we can always check the value of secrets.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
         '''
         result = self._values.get("internal_force_update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def internal_hmac_used_for_secrets_config_hmac(
         self,
     ) -> typing.Optional[builtins.str]:
         '''Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
         '''
         result = self._values.get("internal_hmac_used_for_secrets_config_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def internal_secrets_config_hmac(self) -> typing.Optional[builtins.str]:
         '''Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
         '''
         result = self._values.get("internal_secrets_config_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host catalog name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the plugin that should back the resource. This or plugin_name must be defined.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
         '''
         result = self._values.get("plugin_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_name(self) -> typing.Optional[builtins.str]:
         '''The name of the plugin that should back the resource. This or plugin_id must be defined.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
         '''
         result = self._values.get("plugin_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secrets_hmac(self) -> typing.Optional[builtins.str]:
         '''The HMAC'd secrets value returned from the server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
         '''
         result = self._values.get("secrets_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secrets_json(self) -> typing.Optional[builtins.str]:
         '''The secrets for the host catalog.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
         '''
         result = self._values.get("secrets_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `boundary_host_catalog_static`
+# `boundary_host_catalog`
 
-Refer to the Terraform Registory for docs: [`boundary_host_catalog_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static).
+Refer to the Terraform Registory for docs: [`boundary_host_catalog`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,58 +17,61 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class HostCatalogStatic(
+class HostCatalog(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-boundary.hostCatalogStatic.HostCatalogStatic",
+    jsii_type="@cdktf/provider-boundary.hostCatalog.HostCatalog",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static boundary_host_catalog_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog boundary_host_catalog}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
+        type: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static boundary_host_catalog_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog boundary_host_catalog} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#description HostCatalogStatic#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#name HostCatalogStatic#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
+        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#type HostCatalog#type}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#description HostCatalog#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#name HostCatalog#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d41f660fd85a2635912920a4015b2e8bd24eca13307839327f80a04185608194)
+            type_hints = typing.get_type_hints(_typecheckingstub__2e5a603f24f85d861e36f78fe548cde1b229c531c6c480cdb3dc6a0f29b5e770)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        config = HostCatalogStaticConfig(
+        config = HostCatalogConfig(
             scope_id=scope_id,
+            type=type,
             description=description,
             name=name,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
@@ -112,109 +115,131 @@
 
     @builtins.property
     @jsii.member(jsii_name="scopeIdInput")
     def scope_id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "scopeIdInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="typeInput")
+    def type_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "typeInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "description"))
 
     @description.setter
     def description(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0a3b7fff3c8db282b163e11fc5ec154f1bcdd929a5e6ee1f887a2d6821fbe72b)
+            type_hints = typing.get_type_hints(_typecheckingstub__6f6284e6fb158527fc7a971ac6d6aa56c01d0c737e7f775385eda3704af24574)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "description", value)
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6a2518c7bd56f199c607e63841f8c602ef02588504de753de49c6e3a7546c98e)
+            type_hints = typing.get_type_hints(_typecheckingstub__975d07e0347b24b60dd1e24363bd0ef2bcfcd54dda0b162c72ee2a357056e5bc)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
     @jsii.member(jsii_name="scopeId")
     def scope_id(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "scopeId"))
 
     @scope_id.setter
     def scope_id(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__68bb8739c944268e14f549fefe3781504df124b22514a2fb1df25b81bdc01365)
+            type_hints = typing.get_type_hints(_typecheckingstub__8748d7d3baea6e1c846f9150d355d7ce536b709aa7f885f4db6ff6198ee3c09b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "scopeId", value)
 
+    @builtins.property
+    @jsii.member(jsii_name="type")
+    def type(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "type"))
+
+    @type.setter
+    def type(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__3ff5a6d1fcaf1c6ff8ebca34155f86880ecb37700cd68f383388702dd552223d)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "type", value)
+
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-boundary.hostCatalogStatic.HostCatalogStaticConfig",
+    jsii_type="@cdktf/provider-boundary.hostCatalog.HostCatalogConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "scope_id": "scopeId",
+        "type": "type",
         "description": "description",
         "name": "name",
     },
 )
-class HostCatalogStaticConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class HostCatalogConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         scope_id: builtins.str,
+        type: builtins.str,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#description HostCatalogStatic#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#name HostCatalogStatic#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
+        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#type HostCatalog#type}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#description HostCatalog#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#name HostCatalog#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b9383c014a702a29d2bd6b4cb2cb8ffbdb1a1941e41b5c6c21399d435f4054ea)
+            type_hints = typing.get_type_hints(_typecheckingstub__221287db26b11bf22cb1c1861301eb80b842c76934da2dfbe1504d9975a77502)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument scope_id", value=scope_id, expected_type=type_hints["scope_id"])
+            check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "scope_id": scope_id,
+            "type": type,
         }
         if connection is not None:
             self._values["connection"] = connection
         if count is not None:
             self._values["count"] = count
         if depends_on is not None:
             self._values["depends_on"] = depends_on
@@ -295,101 +320,119 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
+    def type(self) -> builtins.str:
+        '''The host catalog type. Only ``static`` is supported.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#type HostCatalog#type}
+        '''
+        result = self._values.get("type")
+        assert result is not None, "Required property 'type' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host catalog description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#description HostCatalogStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#description HostCatalog#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host catalog name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_catalog_static#name HostCatalogStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_catalog#name HostCatalog#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "HostCatalogStaticConfig(%s)" % ", ".join(
+        return "HostCatalogConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "HostCatalogStatic",
-    "HostCatalogStaticConfig",
+    "HostCatalog",
+    "HostCatalogConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__d41f660fd85a2635912920a4015b2e8bd24eca13307839327f80a04185608194(
+def _typecheckingstub__2e5a603f24f85d861e36f78fe548cde1b229c531c6c480cdb3dc6a0f29b5e770(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     scope_id: builtins.str,
+    type: builtins.str,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0a3b7fff3c8db282b163e11fc5ec154f1bcdd929a5e6ee1f887a2d6821fbe72b(
+def _typecheckingstub__6f6284e6fb158527fc7a971ac6d6aa56c01d0c737e7f775385eda3704af24574(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__975d07e0347b24b60dd1e24363bd0ef2bcfcd54dda0b162c72ee2a357056e5bc(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6a2518c7bd56f199c607e63841f8c602ef02588504de753de49c6e3a7546c98e(
+def _typecheckingstub__8748d7d3baea6e1c846f9150d355d7ce536b709aa7f885f4db6ff6198ee3c09b(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__68bb8739c944268e14f549fefe3781504df124b22514a2fb1df25b81bdc01365(
+def _typecheckingstub__3ff5a6d1fcaf1c6ff8ebca34155f86880ecb37700cd68f383388702dd552223d(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b9383c014a702a29d2bd6b4cb2cb8ffbdb1a1941e41b5c6c21399d435f4054ea(
+def _typecheckingstub__221287db26b11bf22cb1c1861301eb80b842c76934da2dfbe1504d9975a77502(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     scope_id: builtins.str,
+    type: builtins.str,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_host_set`
 
-Refer to the Terraform Registory for docs: [`boundary_host_set`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set).
+Refer to the Terraform Registory for docs: [`boundary_host_set`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HostSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostSet.HostSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set boundary_host_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set boundary_host_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set boundary_host_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set boundary_host_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#type HostSet#type}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#description HostSet#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#host_ids HostSet#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#name HostSet#name}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#type HostSet#type}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#description HostSet#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#host_ids HostSet#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#name HostSet#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -235,19 +235,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#type HostSet#type}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#description HostSet#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#host_ids HostSet#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#name HostSet#name}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#type HostSet#type}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#description HostSet#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#host_ids HostSet#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#name HostSet#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4f0f7249da202193b7621aef5791ff05b5a4977c2a6ddd1052028d3fd7cdea2f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -350,53 +350,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
         '''The catalog for the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
         '''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#type HostSet#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#type HostSet#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host set description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#description HostSet#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#description HostSet#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of host IDs contained in this set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#host_ids HostSet#host_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#host_ids HostSet#host_ids}
         '''
         result = self._values.get("host_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host set name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set#name HostSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set#name HostSet#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_host_set_plugin`
 
-Refer to the Terraform Registory for docs: [`boundary_host_set_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin).
+Refer to the Terraform Registory for docs: [`boundary_host_set_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HostSetPlugin(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostSetPlugin.HostSetPlugin",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin boundary_host_set_plugin}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin boundary_host_set_plugin}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -44,25 +44,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin boundary_host_set_plugin} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin boundary_host_set_plugin} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
-        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#description HostSetPlugin#description}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#name HostSetPlugin#name}
-        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
-        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#type HostSetPlugin#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
+        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#description HostSetPlugin#description}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#name HostSetPlugin#name}
+        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
+        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#type HostSetPlugin#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -291,21 +291,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
-        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#description HostSetPlugin#description}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#name HostSetPlugin#name}
-        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
-        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#type HostSetPlugin#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
+        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#description HostSetPlugin#description}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#name HostSetPlugin#name}
+        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
+        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#type HostSetPlugin#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__118767d2d06e32bb053df9ba5727e72bfc2f7350f582cb3475bfc3b827e174f3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -415,72 +415,72 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
         '''The catalog for the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
         '''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attributes_json(self) -> typing.Optional[builtins.str]:
         '''The attributes for the host set.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
         '''
         result = self._values.get("attributes_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host set description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#description HostSetPlugin#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#description HostSetPlugin#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host set name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#name HostSetPlugin#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#name HostSetPlugin#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def preferred_endpoints(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The ordered list of preferred endpoints.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
         '''
         result = self._values.get("preferred_endpoints")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def sync_interval_seconds(self) -> typing.Optional[jsii.Number]:
         '''The value to set for the sync interval seconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
         '''
         result = self._values.get("sync_interval_seconds")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_plugin#type HostSetPlugin#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_plugin#type HostSetPlugin#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_host_set_static`
 
-Refer to the Terraform Registory for docs: [`boundary_host_set_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static).
+Refer to the Terraform Registory for docs: [`boundary_host_set_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HostSetStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostSetStatic.HostSetStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static boundary_host_set_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static boundary_host_set_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static boundary_host_set_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static boundary_host_set_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#description HostSetStatic#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#name HostSetStatic#name}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#type HostSetStatic#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#description HostSetStatic#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#name HostSetStatic#name}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#type HostSetStatic#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -239,19 +239,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#description HostSetStatic#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#name HostSetStatic#name}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#type HostSetStatic#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#description HostSetStatic#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#name HostSetStatic#name}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#type HostSetStatic#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5e378da7fa60e1ab50df3e685f2e8b19f77831f1ea60d61b9137fa43f412a047)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -355,52 +355,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
         '''The catalog for the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
         '''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host set description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#description HostSetStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#description HostSetStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of host IDs contained in this set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
         '''
         result = self._values.get("host_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host set name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#name HostSetStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#name HostSetStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_set_static#type HostSetStatic#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_set_static#type HostSetStatic#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/host_static/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/host_static/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_host_static`
 
-Refer to the Terraform Registory for docs: [`boundary_host_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static).
+Refer to the Terraform Registory for docs: [`boundary_host_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HostStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostStatic.HostStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static boundary_host_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static boundary_host_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +42,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static boundary_host_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static boundary_host_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#address HostStatic#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#description HostStatic#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#name HostStatic#name}
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#type HostStatic#type}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#address HostStatic#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#description HostStatic#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#name HostStatic#name}
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#type HostStatic#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -239,19 +239,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#address HostStatic#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#description HostStatic#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#name HostStatic#name}
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#type HostStatic#type}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#address HostStatic#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#description HostStatic#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#name HostStatic#name}
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#type HostStatic#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__eeda198263353c7d24b1fe17ba6fe23a0aa061206aff004195ac1d8a9bc85ecb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -353,51 +353,51 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.'''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address(self) -> typing.Optional[builtins.str]:
         '''The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#address HostStatic#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#address HostStatic#address}
         '''
         result = self._values.get("address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#description HostStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#description HostStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#name HostStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#name HostStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of host.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/host_static#type HostStatic#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/host_static#type HostStatic#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_managed_group`
 
-Refer to the Terraform Registory for docs: [`boundary_managed_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group).
+Refer to the Terraform Registory for docs: [`boundary_managed_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class ManagedGroup(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.managedGroup.ManagedGroup",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group boundary_managed_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group boundary_managed_group}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group boundary_managed_group} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group boundary_managed_group} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
-        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#filter ManagedGroup#filter}
-        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#description ManagedGroup#description}
-        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#name ManagedGroup#name}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
+        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#filter ManagedGroup#filter}
+        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#description ManagedGroup#description}
+        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#name ManagedGroup#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -209,18 +209,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
-        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#filter ManagedGroup#filter}
-        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#description ManagedGroup#description}
-        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#name ManagedGroup#name}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
+        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#filter ManagedGroup#filter}
+        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#description ManagedGroup#description}
+        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#name ManagedGroup#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__08f9b5aef6a5e8658e96841aaa7e0bc8f0561fd9010c936a6943512913fd8fcc)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -320,44 +320,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def filter(self) -> builtins.str:
         '''Boolean expression to filter the workers for this managed group.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#filter ManagedGroup#filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#filter ManagedGroup#filter}
         '''
         result = self._values.get("filter")
         assert result is not None, "Required property 'filter' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The managed group description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#description ManagedGroup#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#description ManagedGroup#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The managed group name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/managed_group#name ManagedGroup#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/managed_group#name ManagedGroup#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/provider/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/provider/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`boundary`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs).
+Refer to the Terraform Registory for docs: [`boundary`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,55 +22,61 @@
 
 
 class BoundaryProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.provider.BoundaryProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs boundary}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs boundary}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         addr: builtins.str,
         alias: typing.Optional[builtins.str] = None,
         auth_method_id: typing.Optional[builtins.str] = None,
+        auth_method_login_name: typing.Optional[builtins.str] = None,
+        auth_method_password: typing.Optional[builtins.str] = None,
         password_auth_method_login_name: typing.Optional[builtins.str] = None,
         password_auth_method_password: typing.Optional[builtins.str] = None,
         plugin_execution_dir: typing.Optional[builtins.str] = None,
         recovery_kms_hcl: typing.Optional[builtins.str] = None,
         scope_id: typing.Optional[builtins.str] = None,
         tls_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs boundary} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs boundary} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#addr BoundaryProvider#addr}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#alias BoundaryProvider#alias}
-        :param auth_method_id: The auth method ID e.g. ampw_1234567890. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#auth_method_id BoundaryProvider#auth_method_id}
-        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
-        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
-        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
-        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
-        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#scope_id BoundaryProvider#scope_id}
-        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#tls_insecure BoundaryProvider#tls_insecure}
-        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#token BoundaryProvider#token}
+        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#addr BoundaryProvider#addr}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#alias BoundaryProvider#alias}
+        :param auth_method_id: The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_id BoundaryProvider#auth_method_id}
+        :param auth_method_login_name: The auth method login name for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
+        :param auth_method_password: The auth method password for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_password BoundaryProvider#auth_method_password}
+        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
+        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
+        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
+        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
+        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#scope_id BoundaryProvider#scope_id}
+        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#tls_insecure BoundaryProvider#tls_insecure}
+        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#token BoundaryProvider#token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce45866643ede5c3f23dda6c62ba4515b4bf12276ac23bc01292aac21f883d15)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = BoundaryProviderConfig(
             addr=addr,
             alias=alias,
             auth_method_id=auth_method_id,
+            auth_method_login_name=auth_method_login_name,
+            auth_method_password=auth_method_password,
             password_auth_method_login_name=password_auth_method_login_name,
             password_auth_method_password=password_auth_method_password,
             plugin_execution_dir=plugin_execution_dir,
             recovery_kms_hcl=recovery_kms_hcl,
             scope_id=scope_id,
             tls_insecure=tls_insecure,
             token=token,
@@ -82,14 +88,22 @@
     def reset_alias(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetAlias", []))
 
     @jsii.member(jsii_name="resetAuthMethodId")
     def reset_auth_method_id(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetAuthMethodId", []))
 
+    @jsii.member(jsii_name="resetAuthMethodLoginName")
+    def reset_auth_method_login_name(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAuthMethodLoginName", []))
+
+    @jsii.member(jsii_name="resetAuthMethodPassword")
+    def reset_auth_method_password(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetAuthMethodPassword", []))
+
     @jsii.member(jsii_name="resetPasswordAuthMethodLoginName")
     def reset_password_auth_method_login_name(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPasswordAuthMethodLoginName", []))
 
     @jsii.member(jsii_name="resetPasswordAuthMethodPassword")
     def reset_password_auth_method_password(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetPasswordAuthMethodPassword", []))
@@ -135,14 +149,24 @@
 
     @builtins.property
     @jsii.member(jsii_name="authMethodIdInput")
     def auth_method_id_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "authMethodIdInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="authMethodLoginNameInput")
+    def auth_method_login_name_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "authMethodLoginNameInput"))
+
+    @builtins.property
+    @jsii.member(jsii_name="authMethodPasswordInput")
+    def auth_method_password_input(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "authMethodPasswordInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="passwordAuthMethodLoginNameInput")
     def password_auth_method_login_name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "passwordAuthMethodLoginNameInput"))
 
     @builtins.property
     @jsii.member(jsii_name="passwordAuthMethodPasswordInput")
     def password_auth_method_password_input(self) -> typing.Optional[builtins.str]:
@@ -208,14 +232,38 @@
     def auth_method_id(self, value: typing.Optional[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a2725d022c2deea8b625155d570f7db08889b9e2501b025b8bcd3c0bb37333a0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "authMethodId", value)
 
     @builtins.property
+    @jsii.member(jsii_name="authMethodLoginName")
+    def auth_method_login_name(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "authMethodLoginName"))
+
+    @auth_method_login_name.setter
+    def auth_method_login_name(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__53c1a2ef3122bc21ec37d300d33b2c01a908ff9b85c93c6934e4ca1de8aba1cb)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "authMethodLoginName", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="authMethodPassword")
+    def auth_method_password(self) -> typing.Optional[builtins.str]:
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "authMethodPassword"))
+
+    @auth_method_password.setter
+    def auth_method_password(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e01e0464f8b958da50ea13e286fab96f54ca1046db1b813376c776e314fb3d73)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "authMethodPassword", value)
+
+    @builtins.property
     @jsii.member(jsii_name="passwordAuthMethodLoginName")
     def password_auth_method_login_name(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "passwordAuthMethodLoginName"))
 
     @password_auth_method_login_name.setter
     def password_auth_method_login_name(
         self,
@@ -310,14 +358,16 @@
 @jsii.data_type(
     jsii_type="@cdktf/provider-boundary.provider.BoundaryProviderConfig",
     jsii_struct_bases=[],
     name_mapping={
         "addr": "addr",
         "alias": "alias",
         "auth_method_id": "authMethodId",
+        "auth_method_login_name": "authMethodLoginName",
+        "auth_method_password": "authMethodPassword",
         "password_auth_method_login_name": "passwordAuthMethodLoginName",
         "password_auth_method_password": "passwordAuthMethodPassword",
         "plugin_execution_dir": "pluginExecutionDir",
         "recovery_kms_hcl": "recoveryKmsHcl",
         "scope_id": "scopeId",
         "tls_insecure": "tlsInsecure",
         "token": "token",
@@ -326,53 +376,63 @@
 class BoundaryProviderConfig:
     def __init__(
         self,
         *,
         addr: builtins.str,
         alias: typing.Optional[builtins.str] = None,
         auth_method_id: typing.Optional[builtins.str] = None,
+        auth_method_login_name: typing.Optional[builtins.str] = None,
+        auth_method_password: typing.Optional[builtins.str] = None,
         password_auth_method_login_name: typing.Optional[builtins.str] = None,
         password_auth_method_password: typing.Optional[builtins.str] = None,
         plugin_execution_dir: typing.Optional[builtins.str] = None,
         recovery_kms_hcl: typing.Optional[builtins.str] = None,
         scope_id: typing.Optional[builtins.str] = None,
         tls_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#addr BoundaryProvider#addr}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#alias BoundaryProvider#alias}
-        :param auth_method_id: The auth method ID e.g. ampw_1234567890. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#auth_method_id BoundaryProvider#auth_method_id}
-        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
-        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
-        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
-        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
-        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#scope_id BoundaryProvider#scope_id}
-        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#tls_insecure BoundaryProvider#tls_insecure}
-        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#token BoundaryProvider#token}
+        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#addr BoundaryProvider#addr}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#alias BoundaryProvider#alias}
+        :param auth_method_id: The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_id BoundaryProvider#auth_method_id}
+        :param auth_method_login_name: The auth method login name for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
+        :param auth_method_password: The auth method password for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_password BoundaryProvider#auth_method_password}
+        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
+        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
+        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
+        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
+        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#scope_id BoundaryProvider#scope_id}
+        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#tls_insecure BoundaryProvider#tls_insecure}
+        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#token BoundaryProvider#token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1eb8f2baf8fdc05f14b99407eb26d4ce7c1d5cfdffa21ca1c28275218ffd85f4)
             check_type(argname="argument addr", value=addr, expected_type=type_hints["addr"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument auth_method_id", value=auth_method_id, expected_type=type_hints["auth_method_id"])
+            check_type(argname="argument auth_method_login_name", value=auth_method_login_name, expected_type=type_hints["auth_method_login_name"])
+            check_type(argname="argument auth_method_password", value=auth_method_password, expected_type=type_hints["auth_method_password"])
             check_type(argname="argument password_auth_method_login_name", value=password_auth_method_login_name, expected_type=type_hints["password_auth_method_login_name"])
             check_type(argname="argument password_auth_method_password", value=password_auth_method_password, expected_type=type_hints["password_auth_method_password"])
             check_type(argname="argument plugin_execution_dir", value=plugin_execution_dir, expected_type=type_hints["plugin_execution_dir"])
             check_type(argname="argument recovery_kms_hcl", value=recovery_kms_hcl, expected_type=type_hints["recovery_kms_hcl"])
             check_type(argname="argument scope_id", value=scope_id, expected_type=type_hints["scope_id"])
             check_type(argname="argument tls_insecure", value=tls_insecure, expected_type=type_hints["tls_insecure"])
             check_type(argname="argument token", value=token, expected_type=type_hints["token"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "addr": addr,
         }
         if alias is not None:
             self._values["alias"] = alias
         if auth_method_id is not None:
             self._values["auth_method_id"] = auth_method_id
+        if auth_method_login_name is not None:
+            self._values["auth_method_login_name"] = auth_method_login_name
+        if auth_method_password is not None:
+            self._values["auth_method_password"] = auth_method_password
         if password_auth_method_login_name is not None:
             self._values["password_auth_method_login_name"] = password_auth_method_login_name
         if password_auth_method_password is not None:
             self._values["password_auth_method_password"] = password_auth_method_password
         if plugin_execution_dir is not None:
             self._values["plugin_execution_dir"] = plugin_execution_dir
         if recovery_kms_hcl is not None:
@@ -384,103 +444,121 @@
         if token is not None:
             self._values["token"] = token
 
     @builtins.property
     def addr(self) -> builtins.str:
         '''The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#addr BoundaryProvider#addr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#addr BoundaryProvider#addr}
         '''
         result = self._values.get("addr")
         assert result is not None, "Required property 'addr' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#alias BoundaryProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#alias BoundaryProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def auth_method_id(self) -> typing.Optional[builtins.str]:
-        '''The auth method ID e.g. ampw_1234567890.
+        '''The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#auth_method_id BoundaryProvider#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_id BoundaryProvider#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def auth_method_login_name(self) -> typing.Optional[builtins.str]:
+        '''The auth method login name for password-style or ldap-style auth methods.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
+        '''
+        result = self._values.get("auth_method_login_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def auth_method_password(self) -> typing.Optional[builtins.str]:
+        '''The auth method password for password-style or ldap-style auth methods.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#auth_method_password BoundaryProvider#auth_method_password}
+        '''
+        result = self._values.get("auth_method_password")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def password_auth_method_login_name(self) -> typing.Optional[builtins.str]:
         '''The auth method login name for password-style auth methods.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
         '''
         result = self._values.get("password_auth_method_login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password_auth_method_password(self) -> typing.Optional[builtins.str]:
         '''The auth method password for password-style auth methods.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
         '''
         result = self._values.get("password_auth_method_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_execution_dir(self) -> typing.Optional[builtins.str]:
         '''Specifies a directory that the Boundary provider can use to write and execute its built-in plugins.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
         '''
         result = self._values.get("plugin_execution_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def recovery_kms_hcl(self) -> typing.Optional[builtins.str]:
         '''Can be a heredoc string or a path on disk.
 
         If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
         '''
         result = self._values.get("recovery_kms_hcl")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope ID for the default auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#scope_id BoundaryProvider#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#scope_id BoundaryProvider#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tls_insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When set to true, does not validate the Boundary API endpoint certificate.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#tls_insecure BoundaryProvider#tls_insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#tls_insecure BoundaryProvider#tls_insecure}
         '''
         result = self._values.get("tls_insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''The Boundary token to use, as a string or path on disk containing just the string.
 
         If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs#token BoundaryProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs#token BoundaryProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -503,14 +581,16 @@
 def _typecheckingstub__ce45866643ede5c3f23dda6c62ba4515b4bf12276ac23bc01292aac21f883d15(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     addr: builtins.str,
     alias: typing.Optional[builtins.str] = None,
     auth_method_id: typing.Optional[builtins.str] = None,
+    auth_method_login_name: typing.Optional[builtins.str] = None,
+    auth_method_password: typing.Optional[builtins.str] = None,
     password_auth_method_login_name: typing.Optional[builtins.str] = None,
     password_auth_method_password: typing.Optional[builtins.str] = None,
     plugin_execution_dir: typing.Optional[builtins.str] = None,
     recovery_kms_hcl: typing.Optional[builtins.str] = None,
     scope_id: typing.Optional[builtins.str] = None,
     tls_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     token: typing.Optional[builtins.str] = None,
@@ -532,14 +612,26 @@
 
 def _typecheckingstub__a2725d022c2deea8b625155d570f7db08889b9e2501b025b8bcd3c0bb37333a0(
     value: typing.Optional[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__53c1a2ef3122bc21ec37d300d33b2c01a908ff9b85c93c6934e4ca1de8aba1cb(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e01e0464f8b958da50ea13e286fab96f54ca1046db1b813376c776e314fb3d73(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__fabd5c6761b8bcfcdfeab1c4614c3239afc5c5195cb0737e2c7a072f825ae1c1(
     value: typing.Optional[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2cb9757d3fb77bebe1705c5c5bae845725893d4d6695b748681b2ae0bc5b414b(
@@ -579,14 +671,16 @@
     pass
 
 def _typecheckingstub__1eb8f2baf8fdc05f14b99407eb26d4ce7c1d5cfdffa21ca1c28275218ffd85f4(
     *,
     addr: builtins.str,
     alias: typing.Optional[builtins.str] = None,
     auth_method_id: typing.Optional[builtins.str] = None,
+    auth_method_login_name: typing.Optional[builtins.str] = None,
+    auth_method_password: typing.Optional[builtins.str] = None,
     password_auth_method_login_name: typing.Optional[builtins.str] = None,
     password_auth_method_password: typing.Optional[builtins.str] = None,
     plugin_execution_dir: typing.Optional[builtins.str] = None,
     recovery_kms_hcl: typing.Optional[builtins.str] = None,
     scope_id: typing.Optional[builtins.str] = None,
     tls_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     token: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/role/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/role/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_role`
 
-Refer to the Terraform Registory for docs: [`boundary_role`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role).
+Refer to the Terraform Registory for docs: [`boundary_role`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Role(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.role.Role",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role boundary_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role boundary_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role boundary_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role boundary_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#scope_id Role#scope_id}
-        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#description Role#description}
-        :param grant_scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#grant_scope_id Role#grant_scope_id}.
-        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#grant_strings Role#grant_strings}
-        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#name Role#name}
-        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#principal_ids Role#principal_ids}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#scope_id Role#scope_id}
+        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#description Role#description}
+        :param grant_scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#grant_scope_id Role#grant_scope_id}.
+        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#grant_strings Role#grant_strings}
+        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#name Role#name}
+        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#principal_ids Role#principal_ids}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -265,20 +265,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#scope_id Role#scope_id}
-        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#description Role#description}
-        :param grant_scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#grant_scope_id Role#grant_scope_id}.
-        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#grant_strings Role#grant_strings}
-        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#name Role#name}
-        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#principal_ids Role#principal_ids}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#scope_id Role#scope_id}
+        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#description Role#description}
+        :param grant_scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#grant_scope_id Role#grant_scope_id}.
+        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#grant_strings Role#grant_strings}
+        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#name Role#name}
+        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#principal_ids Role#principal_ids}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a0d9a550fe5793affacbae0f009d3344df6182595218cea1c9b59021276c36f2)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -385,58 +385,58 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#scope_id Role#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#scope_id Role#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The role description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#description Role#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#description Role#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grant_scope_id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#grant_scope_id Role#grant_scope_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#grant_scope_id Role#grant_scope_id}.'''
         result = self._values.get("grant_scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grant_strings(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of stringified grants for the role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#grant_strings Role#grant_strings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#grant_strings Role#grant_strings}
         '''
         result = self._values.get("grant_strings")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The role name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#name Role#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#name Role#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def principal_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of principal (user or group) IDs to add as principals on the role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/role#principal_ids Role#principal_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/role#principal_ids Role#principal_ids}
         '''
         result = self._values.get("principal_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/scope/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/scope/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_scope`
 
-Refer to the Terraform Registory for docs: [`boundary_scope`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope).
+Refer to the Terraform Registory for docs: [`boundary_scope`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Scope(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.scope.Scope",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope boundary_scope}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope boundary_scope}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +43,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope boundary_scope} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope boundary_scope} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#scope_id Scope#scope_id}
-        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
-        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
-        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#description Scope#description}
-        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#global_scope Scope#global_scope}
-        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#name Scope#name}
+        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#scope_id Scope#scope_id}
+        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
+        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
+        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#description Scope#description}
+        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#global_scope Scope#global_scope}
+        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#name Scope#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -284,20 +284,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#scope_id Scope#scope_id}
-        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
-        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
-        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#description Scope#description}
-        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#global_scope Scope#global_scope}
-        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#name Scope#name}
+        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#scope_id Scope#scope_id}
+        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
+        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
+        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#description Scope#description}
+        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#global_scope Scope#global_scope}
+        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#name Scope#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e623dbf4353f12f9cc9aff6267dbb8619be6780c3fa9407450c3f5986ce9a4c6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -404,71 +404,71 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID containing the sub scope resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#scope_id Scope#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#scope_id Scope#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def auto_create_admin_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user.
 
         Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
         '''
         result = self._values.get("auto_create_admin_role")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def auto_create_default_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Only relevant when creating an org scope.
 
         If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
         '''
         result = self._values.get("auto_create_default_role")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The scope description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#description Scope#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#description Scope#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def global_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#global_scope Scope#global_scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#global_scope Scope#global_scope}
         '''
         result = self._values.get("global_scope")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The scope name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/scope#name Scope#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/scope#name Scope#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/target/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/target/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_target`
 
-Refer to the Terraform Registory for docs: [`boundary_target`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target).
+Refer to the Terraform Registory for docs: [`boundary_target`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,25 +22,26 @@
 
 
 class Target(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.target.Target",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target boundary_target}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target boundary_target}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
         type: builtins.str,
         address: typing.Optional[builtins.str] = None,
         brokered_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
+        default_client_port: typing.Optional[jsii.Number] = None,
         default_port: typing.Optional[jsii.Number] = None,
         description: typing.Optional[builtins.str] = None,
         egress_worker_filter: typing.Optional[builtins.str] = None,
         host_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         ingress_worker_filter: typing.Optional[builtins.str] = None,
         injected_application_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         name: typing.Optional[builtins.str] = None,
@@ -51,32 +52,33 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target boundary_target} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target boundary_target} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#scope_id Target#scope_id}
-        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#type Target#type}
-        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#address Target#address}
-        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
-        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#default_port Target#default_port}
-        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#description Target#description}
-        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
-        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#host_source_ids Target#host_source_ids}
-        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
-        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
-        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#name Target#name}
-        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#session_connection_limit Target#session_connection_limit}.
-        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#session_max_seconds Target#session_max_seconds}.
-        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#worker_filter Target#worker_filter}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#scope_id Target#scope_id}
+        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#type Target#type}
+        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#address Target#address}
+        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
+        :param default_client_port: The default client port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#default_client_port Target#default_client_port}
+        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#default_port Target#default_port}
+        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#description Target#description}
+        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
+        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#host_source_ids Target#host_source_ids}
+        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
+        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
+        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#name Target#name}
+        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#session_connection_limit Target#session_connection_limit}.
+        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#session_max_seconds Target#session_max_seconds}.
+        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#worker_filter Target#worker_filter}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -86,14 +88,15 @@
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = TargetConfig(
             scope_id=scope_id,
             type=type,
             address=address,
             brokered_credential_source_ids=brokered_credential_source_ids,
+            default_client_port=default_client_port,
             default_port=default_port,
             description=description,
             egress_worker_filter=egress_worker_filter,
             host_source_ids=host_source_ids,
             ingress_worker_filter=ingress_worker_filter,
             injected_application_credential_source_ids=injected_application_credential_source_ids,
             name=name,
@@ -115,14 +118,18 @@
     def reset_address(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetAddress", []))
 
     @jsii.member(jsii_name="resetBrokeredCredentialSourceIds")
     def reset_brokered_credential_source_ids(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetBrokeredCredentialSourceIds", []))
 
+    @jsii.member(jsii_name="resetDefaultClientPort")
+    def reset_default_client_port(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetDefaultClientPort", []))
+
     @jsii.member(jsii_name="resetDefaultPort")
     def reset_default_port(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetDefaultPort", []))
 
     @jsii.member(jsii_name="resetDescription")
     def reset_description(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetDescription", []))
@@ -182,14 +189,19 @@
     @jsii.member(jsii_name="brokeredCredentialSourceIdsInput")
     def brokered_credential_source_ids_input(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "brokeredCredentialSourceIdsInput"))
 
     @builtins.property
+    @jsii.member(jsii_name="defaultClientPortInput")
+    def default_client_port_input(self) -> typing.Optional[jsii.Number]:
+        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "defaultClientPortInput"))
+
+    @builtins.property
     @jsii.member(jsii_name="defaultPortInput")
     def default_port_input(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "defaultPortInput"))
 
     @builtins.property
     @jsii.member(jsii_name="descriptionInput")
     def description_input(self) -> typing.Optional[builtins.str]:
@@ -268,14 +280,26 @@
     def brokered_credential_source_ids(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fc2d85aca1b17af87cd56f9f72cb476381b44805f888013726836aff0b115fe1)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "brokeredCredentialSourceIds", value)
 
     @builtins.property
+    @jsii.member(jsii_name="defaultClientPort")
+    def default_client_port(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "defaultClientPort"))
+
+    @default_client_port.setter
+    def default_client_port(self, value: jsii.Number) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e476bc2f762d60541597a12cf70e3cbc3484d4e3c28a1ce779bc61e5582d3235)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "defaultClientPort", value)
+
+    @builtins.property
     @jsii.member(jsii_name="defaultPort")
     def default_port(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "defaultPort"))
 
     @default_port.setter
     def default_port(self, value: jsii.Number) -> None:
         if __debug__:
@@ -430,14 +454,15 @@
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "scope_id": "scopeId",
         "type": "type",
         "address": "address",
         "brokered_credential_source_ids": "brokeredCredentialSourceIds",
+        "default_client_port": "defaultClientPort",
         "default_port": "defaultPort",
         "description": "description",
         "egress_worker_filter": "egressWorkerFilter",
         "host_source_ids": "hostSourceIds",
         "ingress_worker_filter": "ingressWorkerFilter",
         "injected_application_credential_source_ids": "injectedApplicationCredentialSourceIds",
         "name": "name",
@@ -457,14 +482,15 @@
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
         scope_id: builtins.str,
         type: builtins.str,
         address: typing.Optional[builtins.str] = None,
         brokered_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
+        default_client_port: typing.Optional[jsii.Number] = None,
         default_port: typing.Optional[jsii.Number] = None,
         description: typing.Optional[builtins.str] = None,
         egress_worker_filter: typing.Optional[builtins.str] = None,
         host_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         ingress_worker_filter: typing.Optional[builtins.str] = None,
         injected_application_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
         name: typing.Optional[builtins.str] = None,
@@ -476,28 +502,29 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#scope_id Target#scope_id}
-        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#type Target#type}
-        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#address Target#address}
-        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
-        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#default_port Target#default_port}
-        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#description Target#description}
-        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
-        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#host_source_ids Target#host_source_ids}
-        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
-        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
-        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#name Target#name}
-        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#session_connection_limit Target#session_connection_limit}.
-        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#session_max_seconds Target#session_max_seconds}.
-        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#worker_filter Target#worker_filter}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#scope_id Target#scope_id}
+        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#type Target#type}
+        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#address Target#address}
+        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
+        :param default_client_port: The default client port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#default_client_port Target#default_client_port}
+        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#default_port Target#default_port}
+        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#description Target#description}
+        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
+        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#host_source_ids Target#host_source_ids}
+        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
+        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
+        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#name Target#name}
+        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#session_connection_limit Target#session_connection_limit}.
+        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#session_max_seconds Target#session_max_seconds}.
+        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#worker_filter Target#worker_filter}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b3790b32773af6299bc7839606b6164e1bada068e491dd6db09b0641a30f5e25)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -506,14 +533,15 @@
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
             check_type(argname="argument scope_id", value=scope_id, expected_type=type_hints["scope_id"])
             check_type(argname="argument type", value=type, expected_type=type_hints["type"])
             check_type(argname="argument address", value=address, expected_type=type_hints["address"])
             check_type(argname="argument brokered_credential_source_ids", value=brokered_credential_source_ids, expected_type=type_hints["brokered_credential_source_ids"])
+            check_type(argname="argument default_client_port", value=default_client_port, expected_type=type_hints["default_client_port"])
             check_type(argname="argument default_port", value=default_port, expected_type=type_hints["default_port"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument egress_worker_filter", value=egress_worker_filter, expected_type=type_hints["egress_worker_filter"])
             check_type(argname="argument host_source_ids", value=host_source_ids, expected_type=type_hints["host_source_ids"])
             check_type(argname="argument ingress_worker_filter", value=ingress_worker_filter, expected_type=type_hints["ingress_worker_filter"])
             check_type(argname="argument injected_application_credential_source_ids", value=injected_application_credential_source_ids, expected_type=type_hints["injected_application_credential_source_ids"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
@@ -538,14 +566,16 @@
             self._values["provider"] = provider
         if provisioners is not None:
             self._values["provisioners"] = provisioners
         if address is not None:
             self._values["address"] = address
         if brokered_credential_source_ids is not None:
             self._values["brokered_credential_source_ids"] = brokered_credential_source_ids
+        if default_client_port is not None:
+            self._values["default_client_port"] = default_client_port
         if default_port is not None:
             self._values["default_port"] = default_port
         if description is not None:
             self._values["description"] = description
         if egress_worker_filter is not None:
             self._values["egress_worker_filter"] = egress_worker_filter
         if host_source_ids is not None:
@@ -627,134 +657,143 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#scope_id Target#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#scope_id Target#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The target resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#type Target#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#type Target#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address(self) -> typing.Optional[builtins.str]:
         '''Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#address Target#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#address Target#address}
         '''
         result = self._values.get("address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def brokered_credential_source_ids(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of brokered credential source ID's.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
         '''
         result = self._values.get("brokered_credential_source_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def default_client_port(self) -> typing.Optional[jsii.Number]:
+        '''The default client port for this target.
+
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#default_client_port Target#default_client_port}
+        '''
+        result = self._values.get("default_client_port")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def default_port(self) -> typing.Optional[jsii.Number]:
         '''The default port for this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#default_port Target#default_port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#default_port Target#default_port}
         '''
         result = self._values.get("default_port")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The target description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#description Target#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#description Target#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def egress_worker_filter(self) -> typing.Optional[builtins.str]:
         '''Boolean expression to filter the workers used to access this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
         '''
         result = self._values.get("egress_worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host_source_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of host source ID's. Cannot be used alongside address.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#host_source_ids Target#host_source_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#host_source_ids Target#host_source_ids}
         '''
         result = self._values.get("host_source_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def ingress_worker_filter(self) -> typing.Optional[builtins.str]:
         '''HCP Only.
 
         Boolean expression to filter the workers a user will connect to when initiating a session against this target
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
         '''
         result = self._values.get("ingress_worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def injected_application_credential_source_ids(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of injected application credential source ID's.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
         '''
         result = self._values.get("injected_application_credential_source_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The target name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#name Target#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#name Target#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def session_connection_limit(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#session_connection_limit Target#session_connection_limit}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#session_connection_limit Target#session_connection_limit}.'''
         result = self._values.get("session_connection_limit")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def session_max_seconds(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#session_max_seconds Target#session_max_seconds}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#session_max_seconds Target#session_max_seconds}.'''
         result = self._values.get("session_max_seconds")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def worker_filter(self) -> typing.Optional[builtins.str]:
         '''Boolean expression to filter the workers for this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/target#worker_filter Target#worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/target#worker_filter Target#worker_filter}
         '''
         result = self._values.get("worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -778,14 +817,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     scope_id: builtins.str,
     type: builtins.str,
     address: typing.Optional[builtins.str] = None,
     brokered_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
+    default_client_port: typing.Optional[jsii.Number] = None,
     default_port: typing.Optional[jsii.Number] = None,
     description: typing.Optional[builtins.str] = None,
     egress_worker_filter: typing.Optional[builtins.str] = None,
     host_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     ingress_worker_filter: typing.Optional[builtins.str] = None,
     injected_application_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     name: typing.Optional[builtins.str] = None,
@@ -811,14 +851,20 @@
 
 def _typecheckingstub__fc2d85aca1b17af87cd56f9f72cb476381b44805f888013726836aff0b115fe1(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__e476bc2f762d60541597a12cf70e3cbc3484d4e3c28a1ce779bc61e5582d3235(
+    value: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__e97b18eb3a15bc6ab1b42641e60d81d079f8f7d823b41c19ca5a4b2da786085e(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__018aafdcf46c5443bea080998e12df13e2909b4fdace106e9818b3fc9ed11a04(
@@ -896,14 +942,15 @@
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     scope_id: builtins.str,
     type: builtins.str,
     address: typing.Optional[builtins.str] = None,
     brokered_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
+    default_client_port: typing.Optional[jsii.Number] = None,
     default_port: typing.Optional[jsii.Number] = None,
     description: typing.Optional[builtins.str] = None,
     egress_worker_filter: typing.Optional[builtins.str] = None,
     host_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     ingress_worker_filter: typing.Optional[builtins.str] = None,
     injected_application_credential_source_ids: typing.Optional[typing.Sequence[builtins.str]] = None,
     name: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/user/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/user/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_user`
 
-Refer to the Terraform Registory for docs: [`boundary_user`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user).
+Refer to the Terraform Registory for docs: [`boundary_user`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class User(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.user.User",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user boundary_user}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user boundary_user}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user boundary_user} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user boundary_user} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#scope_id User#scope_id}
-        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#account_ids User#account_ids}
-        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#description User#description}
-        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#name User#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#scope_id User#scope_id}
+        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#account_ids User#account_ids}
+        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#description User#description}
+        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#name User#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -213,18 +213,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#scope_id User#scope_id}
-        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#account_ids User#account_ids}
-        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#description User#description}
-        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#name User#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#scope_id User#scope_id}
+        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#account_ids User#account_ids}
+        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#description User#description}
+        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#name User#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e5abd1b3d9322f90ebf0dff710e71ef2c316c6fb92dd740ef40f6a4d5bb5f496)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -325,43 +325,43 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#scope_id User#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#scope_id User#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def account_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Account ID's to associate with this user resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#account_ids User#account_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#account_ids User#account_ids}
         '''
         result = self._values.get("account_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The user description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#description User#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#description User#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The username. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/user#name User#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/user#name User#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary/worker/__init__.py` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary/worker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `boundary_worker`
 
-Refer to the Terraform Registory for docs: [`boundary_worker`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker).
+Refer to the Terraform Registory for docs: [`boundary_worker`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Worker(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.worker.Worker",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker boundary_worker}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker boundary_worker}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         description: typing.Optional[builtins.str] = None,
@@ -41,22 +41,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker boundary_worker} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker boundary_worker} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#description Worker#description}
-        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#name Worker#name}
-        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#scope_id Worker#scope_id}
-        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
+        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#description Worker#description}
+        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#name Worker#name}
+        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#scope_id Worker#scope_id}
+        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -237,18 +237,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#description Worker#description}
-        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#name Worker#name}
-        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#scope_id Worker#scope_id}
-        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
+        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#description Worker#description}
+        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#name Worker#name}
+        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#scope_id Worker#scope_id}
+        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__87814f62730dab1883e5e4cb04d8df44dd248528f40ec027645b1ad9f9de86b1)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -349,44 +349,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description for the worker.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#description Worker#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#description Worker#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name for the worker.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#name Worker#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#name Worker#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope for the worker. Defaults to ``global``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#scope_id Worker#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#scope_id Worker#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def worker_generated_auth_token(self) -> typing.Optional[builtins.str]:
         '''The worker authentication token required to register the worker for the worker-led authentication flow.
 
         Leaving this blank will result in a controller generated token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.7/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.8/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
         '''
         result = self._values.get("worker_generated_auth_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-boundary
-Version: 4.0.4
+Version: 4.0.5
 Summary: Prebuilt boundary Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-boundary.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-boundary.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-boundary-4.0.4/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-boundary-4.0.5/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 src/cdktf_cdktf_provider_boundary/py.typed
 src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_boundary.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_boundary.egg-info/requires.txt
 src/cdktf_cdktf_provider_boundary.egg-info/top_level.txt
 src/cdktf_cdktf_provider_boundary/_jsii/__init__.py
-src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@4.0.4.jsii.tgz
+src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@4.0.5.jsii.tgz
 src/cdktf_cdktf_provider_boundary/account/__init__.py
+src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py
 src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py
 src/cdktf_cdktf_provider_boundary/account_password/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method/__init__.py
+src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_json/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py
@@ -31,13 +33,14 @@
 src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py
 src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py
 src/cdktf_cdktf_provider_boundary/host_set/__init__.py
 src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py
 src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py
 src/cdktf_cdktf_provider_boundary/host_static/__init__.py
 src/cdktf_cdktf_provider_boundary/managed_group/__init__.py
+src/cdktf_cdktf_provider_boundary/managed_group_ldap/__init__.py
 src/cdktf_cdktf_provider_boundary/provider/__init__.py
 src/cdktf_cdktf_provider_boundary/role/__init__.py
 src/cdktf_cdktf_provider_boundary/scope/__init__.py
 src/cdktf_cdktf_provider_boundary/target/__init__.py
 src/cdktf_cdktf_provider_boundary/user/__init__.py
 src/cdktf_cdktf_provider_boundary/worker/__init__.py
```

