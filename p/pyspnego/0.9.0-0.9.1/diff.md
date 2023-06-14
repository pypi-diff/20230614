# Comparing `tmp/pyspnego-0.9.0.tar.gz` & `tmp/pyspnego-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspnego-0.9.0.tar", last modified: Fri Apr 28 22:32:32 2023, max compression
+gzip compressed data, was "pyspnego-0.9.1.tar", last modified: Wed Jun 14 04:23:50 2023, max compression
```

## Comparing `pyspnego-0.9.0.tar` & `pyspnego-0.9.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.927079 pyspnego-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-04-28 22:32:25.000000 pyspnego-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-28 22:32:25.000000 pyspnego-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 22:32:25.000000 pyspnego-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-28 22:32:32.927079 pyspnego-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-28 22:32:25.000000 pyspnego-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.907079 pyspnego-0.9.0/build_helpers/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2768 2023-04-28 22:32:25.000000 pyspnego-0.9.0/build_helpers/lib.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-04-28 22:32:25.000000 pyspnego-0.9.0/build_helpers/run-ci.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-04-28 22:32:25.000000 pyspnego-0.9.0/build_helpers/run-container.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-04-28 22:32:25.000000 pyspnego-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 22:32:25.000000 pyspnego-0.9.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:32:32.927079 pyspnego-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-28 22:32:25.000000 pyspnego-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.903079 pyspnego-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.907079 pyspnego-0.9.0/src/pyspnego.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 22:32:32.000000 pyspnego-0.9.0/src/pyspnego.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.911079 pyspnego-0.9.0/src/spnego/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33434 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)    34578 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_credssp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_credssp_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    24467 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_gss.py
--rw-r--r--   0 runner    (1001) docker     (123)    56199 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_kerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)    36954 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.911079 pyspnego-0.9.0/src/spnego/_ntlm_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/md4.py
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_ntlm_raw/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_spnego.py
--rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.915079 pyspnego-0.9.0/src/spnego/_sspi_raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/security.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/text.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/text.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_sspi_raw/windows.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_tls_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/channel_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/gss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/iov.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/sspi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-04-28 22:32:25.000000 pyspnego-0.9.0/src/spnego/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.915079 pyspnego-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.919079 pyspnego-0.9.0/tests/_ntlm_raw/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_md4.py
--rw-r--r--   0 runner    (1001) docker     (123)    46406 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_ntlm_raw/test_security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.919079 pyspnego-0.9.0/tests/_sspi_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_sspi_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_sspi_raw/test_sspi.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/_sspi_raw/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.923079 pyspnego-0.9.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_password
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_remote_guard_empty_supplemental
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_remote_guard_multiple
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_remote_guard_no_supplemental
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_smart_card
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_credential_smart_card_full
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_remote_guard_ms_example
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/credssp_ts_request
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_krb_ap_rep
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_krb_ap_req
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_neg_token_init
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/initial_context_token_neg_token_init2
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_as_rep
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_as_req
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_error
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_tgs_rep
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/krb_tgs_req
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/neg_token_resp
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_authenticate
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_authenticate_no_sign_seal
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_challenge
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/ntlm_negotiate
--rw-r--r--   0 runner    (1001) docker     (123)    42066 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/pyspnego.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.0_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.0_server_hello
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.1_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.1_server_hello
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.2_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.2_client_key_exchange
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.2_server_hello
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.3_client_hello
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/data/tls1.3_server_hello
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.923079 pyspnego-0.9.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/inventory.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:32:32.923079 pyspnego-0.9.0/tests/integration/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/templates/generate_cert.sh.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/templates/krb5.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    60904 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/templates/test_integration.py.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/integration/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)    66365 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_auth_dce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_channel_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_credssp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_credssp_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_gss.py
--rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_kerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)    58565 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_negotiate.py
--rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_spnego.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_sspi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-28 22:32:25.000000 pyspnego-0.9.0/tests/test_tls_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.265745 pyspnego-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-06-14 04:23:41.000000 pyspnego-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-14 04:23:41.000000 pyspnego-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-14 04:23:41.000000 pyspnego-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-14 04:23:50.265745 pyspnego-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-14 04:23:41.000000 pyspnego-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.245748 pyspnego-0.9.1/build_helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2768 2023-06-14 04:23:41.000000 pyspnego-0.9.1/build_helpers/lib.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      144 2023-06-14 04:23:41.000000 pyspnego-0.9.1/build_helpers/run-ci.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-06-14 04:23:41.000000 pyspnego-0.9.1/build_helpers/run-container.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-14 04:23:41.000000 pyspnego-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-14 04:23:41.000000 pyspnego-0.9.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:23:50.265745 pyspnego-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-14 04:23:41.000000 pyspnego-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.241749 pyspnego-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.245748 pyspnego-0.9.1/src/pyspnego.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-14 04:23:50.000000 pyspnego-0.9.1/src/pyspnego.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-14 04:23:50.000000 pyspnego-0.9.1/src/pyspnego.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:23:50.000000 pyspnego-0.9.1/src/pyspnego.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 04:23:50.000000 pyspnego-0.9.1/src/pyspnego.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 04:23:50.000000 pyspnego-0.9.1/src/pyspnego.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 04:23:50.000000 pyspnego-0.9.1/src/pyspnego.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.249748 pyspnego-0.9.1/src/spnego/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33434 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20634 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34578 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26302 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_credssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_credssp_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24467 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_gss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56199 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_kerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18885 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37278 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.249748 pyspnego-0.9.1/src/spnego/_ntlm_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm_raw/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21201 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm_raw/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm_raw/md4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm_raw/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_ntlm_raw/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19451 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_spnego.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18586 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.253747 pyspnego-0.9.1/src/spnego/_sspi_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/security.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/sspi.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/sspi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/sspi.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/text.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/text.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_sspi_raw/windows.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32305 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_tls_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/channel_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15125 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/gss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/iov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-14 04:23:41.000000 pyspnego-0.9.1/src/spnego/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.253747 pyspnego-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.257746 pyspnego-0.9.1/tests/_ntlm_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_ntlm_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_ntlm_raw/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_ntlm_raw/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_ntlm_raw/test_md4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46406 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_ntlm_raw/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_ntlm_raw/test_security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.257746 pyspnego-0.9.1/tests/_sspi_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_sspi_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_sspi_raw/test_sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/_sspi_raw/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.265745 pyspnego-0.9.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_credential_password
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_credential_remote_guard_empty_supplemental
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_credential_remote_guard_multiple
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_credential_remote_guard_no_supplemental
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_credential_smart_card
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_credential_smart_card_full
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_remote_guard_ms_example
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/credssp_ts_request
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/initial_context_token_krb_ap_rep
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/initial_context_token_krb_ap_req
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/initial_context_token_neg_token_init
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/initial_context_token_neg_token_init2
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/krb_as_rep
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/krb_as_req
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/krb_error
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/krb_tgs_rep
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/krb_tgs_req
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/neg_token_resp
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/ntlm_authenticate
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/ntlm_authenticate_no_sign_seal
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/ntlm_challenge
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/ntlm_negotiate
+-rw-r--r--   0 runner    (1001) docker     (123)    42066 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/pyspnego.ps1
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.0_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.0_server_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.1_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.1_server_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.2_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.2_client_key_exchange
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.2_server_hello
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.3_client_hello
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/data/tls1.3_server_hello
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.265745 pyspnego-0.9.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/inventory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16553 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:23:50.265745 pyspnego-0.9.1/tests/integration/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/templates/generate_cert.sh.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/templates/krb5.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    60904 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/templates/test_integration.py.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/integration/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66365 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_auth_dce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_channel_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_credssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_credssp_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_gss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_kerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58565 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_negotiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30784 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_spnego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_sspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-14 04:23:41.000000 pyspnego-0.9.1/tests/test_tls_struct.py
```

### Comparing `pyspnego-0.9.0/CHANGELOG.md` & `pyspnego-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.9.1 - 2023-06-14
+
+* Always set the `NTLMSSP_REQUEST_VERSION` flag on the NTLM `Negotiate` message
+  * This aligns the behaviour with how SSPI generates this message
+
 ## 0.9.0 - 2023-04-29
 
 * Added the `spnego.ContextReq.dce_style` flag to enable DCE authentication mode
   * This is used in protocols like RPC/DCE
 * The value for `spnego.iov.BufferType.sign_only` on SSPI has changed from representing `SECBUFFER_MECHLIST` to `SECBUFFER_READONLY_WITH_CHECKSUM`
   * This is to better match what `sign_only` means when using it with GSSAPI
   * It is needed to support RPC encryption and signature headers on SSPI
```

### Comparing `pyspnego-0.9.0/LICENSE` & `pyspnego-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/PKG-INFO` & `pyspnego-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspnego
-Version: 0.9.0
+Version: 0.9.1
 Summary: Windows Negotiate Authentication Client and Server
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyspnego-0.9.0/README.md` & `pyspnego-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/build_helpers/lib.sh` & `pyspnego-0.9.1/build_helpers/lib.sh`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/build_helpers/run-container.sh` & `pyspnego-0.9.1/build_helpers/run-container.sh`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/pyproject.toml` & `pyspnego-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/setup.py` & `pyspnego-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/pyspnego.egg-info/PKG-INFO` & `pyspnego-0.9.1/src/pyspnego.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspnego
-Version: 0.9.0
+Version: 0.9.1
 Summary: Windows Negotiate Authentication Client and Server
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyspnego-0.9.0/src/pyspnego.egg-info/SOURCES.txt` & `pyspnego-0.9.1/src/pyspnego.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/__init__.py` & `pyspnego-0.9.1/src/spnego/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/__main__.py` & `pyspnego-0.9.1/src/spnego/__main__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_asn1.py` & `pyspnego-0.9.1/src/spnego/_asn1.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_context.py` & `pyspnego-0.9.1/src/spnego/_context.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_credential.py` & `pyspnego-0.9.1/src/spnego/_credential.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_credssp.py` & `pyspnego-0.9.1/src/spnego/_credssp.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_credssp_structures.py` & `pyspnego-0.9.1/src/spnego/_credssp_structures.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_gss.py` & `pyspnego-0.9.1/src/spnego/_gss.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_kerberos.py` & `pyspnego-0.9.1/src/spnego/_kerberos.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_negotiate.py` & `pyspnego-0.9.1/src/spnego/_negotiate.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_ntlm.py` & `pyspnego-0.9.1/src/spnego/_ntlm.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,19 @@
     def _step_initiate(
         self,
         in_token: typing.Optional[bytes] = None,
         *,
         channel_bindings: typing.Optional[GssChannelBindings] = None,
     ) -> bytes:
         if not self._temp_negotiate:
-            self._temp_negotiate = Negotiate(self._context_req)
+            # SSPI always sends the version even if it's optional. There have
+            # been reports that some NTLM servers expect this to produce a
+            # valid challenge/authentication token later in the exchange.
+            # https://github.com/jborean93/smbprotocol/issues/216
+            self._temp_negotiate = Negotiate(self._context_req, version=Version.get_current())
             return self._temp_negotiate.pack()
 
         in_token = in_token or b""
         challenge = Challenge.unpack(in_token)
 
         # Lots of mypy failures with self._credential, cast it to non Optional as it will always be set here.
         credential = typing.cast(_NTLMCredential, self._credential)
```

### Comparing `pyspnego-0.9.0/src/spnego/_ntlm_raw/crypto.py` & `pyspnego-0.9.1/src/spnego/_ntlm_raw/crypto.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_ntlm_raw/des.py` & `pyspnego-0.9.1/src/spnego/_ntlm_raw/des.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_ntlm_raw/md4.py` & `pyspnego-0.9.1/src/spnego/_ntlm_raw/md4.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_ntlm_raw/messages.py` & `pyspnego-0.9.1/src/spnego/_ntlm_raw/messages.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_ntlm_raw/security.py` & `pyspnego-0.9.1/src/spnego/_ntlm_raw/security.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_spnego.py` & `pyspnego-0.9.1/src/spnego/_spnego.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi.py` & `pyspnego-0.9.1/src/spnego/_sspi.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/__init__.py` & `pyspnego-0.9.1/src/spnego/_sspi_raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/security.pxd` & `pyspnego-0.9.1/src/spnego/_sspi_raw/security.pxd`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pxd` & `pyspnego-0.9.1/src/spnego/_sspi_raw/sspi.pxd`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyi` & `pyspnego-0.9.1/src/spnego/_sspi_raw/sspi.pyi`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/sspi.pyx` & `pyspnego-0.9.1/src/spnego/_sspi_raw/sspi.pyx`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/text.pyx` & `pyspnego-0.9.1/src/spnego/_sspi_raw/text.pyx`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_sspi_raw/windows.pxd` & `pyspnego-0.9.1/src/spnego/_sspi_raw/windows.pxd`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_text.py` & `pyspnego-0.9.1/src/spnego/_text.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/_tls_struct.py` & `pyspnego-0.9.1/src/spnego/_tls_struct.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/auth.py` & `pyspnego-0.9.1/src/spnego/auth.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/channel_bindings.py` & `pyspnego-0.9.1/src/spnego/channel_bindings.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/exceptions.py` & `pyspnego-0.9.1/src/spnego/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/iov.py` & `pyspnego-0.9.1/src/spnego/iov.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/src/spnego/tls.py` & `pyspnego-0.9.1/src/spnego/tls.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_ntlm_raw/__init__.py` & `pyspnego-0.9.1/tests/_ntlm_raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_ntlm_raw/test_crypto.py` & `pyspnego-0.9.1/tests/_ntlm_raw/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_ntlm_raw/test_des.py` & `pyspnego-0.9.1/tests/_ntlm_raw/test_des.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_ntlm_raw/test_md4.py` & `pyspnego-0.9.1/tests/_ntlm_raw/test_md4.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_ntlm_raw/test_messages.py` & `pyspnego-0.9.1/tests/_ntlm_raw/test_messages.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_ntlm_raw/test_security.py` & `pyspnego-0.9.1/tests/_ntlm_raw/test_security.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_sspi_raw/test_sspi.py` & `pyspnego-0.9.1/tests/_sspi_raw/test_sspi.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/_sspi_raw/test_text.py` & `pyspnego-0.9.1/tests/_sspi_raw/test_text.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/conftest.py` & `pyspnego-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/credssp_ts_remote_guard_ms_example` & `pyspnego-0.9.1/tests/data/credssp_ts_remote_guard_ms_example`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/initial_context_token_krb_ap_req` & `pyspnego-0.9.1/tests/data/initial_context_token_krb_ap_req`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/initial_context_token_neg_token_init` & `pyspnego-0.9.1/tests/data/initial_context_token_neg_token_init`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/krb_as_rep` & `pyspnego-0.9.1/tests/data/krb_as_rep`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/krb_tgs_rep` & `pyspnego-0.9.1/tests/data/krb_tgs_rep`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/krb_tgs_req` & `pyspnego-0.9.1/tests/data/krb_tgs_req`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/pyspnego.ps1` & `pyspnego-0.9.1/tests/data/pyspnego.ps1`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/test_context.py` & `pyspnego-0.9.1/tests/data/test_context.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/tls1.0_server_hello` & `pyspnego-0.9.1/tests/data/tls1.0_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/tls1.1_server_hello` & `pyspnego-0.9.1/tests/data/tls1.1_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/tls1.2_server_hello` & `pyspnego-0.9.1/tests/data/tls1.2_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/data/tls1.3_server_hello` & `pyspnego-0.9.1/tests/data/tls1.3_server_hello`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/README.md` & `pyspnego-0.9.1/tests/integration/README.md`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/Vagrantfile` & `pyspnego-0.9.1/tests/integration/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/inventory.yml` & `pyspnego-0.9.1/tests/integration/inventory.yml`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/main.yml` & `pyspnego-0.9.1/tests/integration/main.yml`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/templates/generate_cert.sh.tmpl` & `pyspnego-0.9.1/tests/integration/templates/generate_cert.sh.tmpl`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/templates/krb5.conf.tmpl` & `pyspnego-0.9.1/tests/integration/templates/krb5.conf.tmpl`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/templates/test_integration.py.tmpl` & `pyspnego-0.9.1/tests/integration/templates/test_integration.py.tmpl`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/integration/tests.yml` & `pyspnego-0.9.1/tests/integration/tests.yml`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_asn1.py` & `pyspnego-0.9.1/tests/test_asn1.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_auth.py` & `pyspnego-0.9.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_auth_dce.py` & `pyspnego-0.9.1/tests/test_auth_dce.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_channel_bindings.py` & `pyspnego-0.9.1/tests/test_channel_bindings.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_context.py` & `pyspnego-0.9.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_credssp.py` & `pyspnego-0.9.1/tests/test_credssp.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_credssp_structures.py` & `pyspnego-0.9.1/tests/test_credssp_structures.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_deprecation.py` & `pyspnego-0.9.1/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_exceptions.py` & `pyspnego-0.9.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_gss.py` & `pyspnego-0.9.1/tests/test_gss.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_kerberos.py` & `pyspnego-0.9.1/tests/test_kerberos.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_main.py` & `pyspnego-0.9.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_negotiate.py` & `pyspnego-0.9.1/tests/test_negotiate.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_ntlm.py` & `pyspnego-0.9.1/tests/test_ntlm.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_spnego.py` & `pyspnego-0.9.1/tests/test_spnego.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_sspi.py` & `pyspnego-0.9.1/tests/test_sspi.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_text.py` & `pyspnego-0.9.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pyspnego-0.9.0/tests/test_tls_struct.py` & `pyspnego-0.9.1/tests/test_tls_struct.py`

 * *Files identical despite different names*

