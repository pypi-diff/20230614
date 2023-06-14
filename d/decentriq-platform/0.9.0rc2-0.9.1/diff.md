# Comparing `tmp/decentriq-platform-0.9.0rc2.tar.gz` & `tmp/decentriq-platform-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentriq-platform-0.9.0rc2.tar", max compression
+gzip compressed data, was "decentriq-platform-0.9.1.tar", max compression
```

## Comparing `decentriq-platform-0.9.0rc2.tar` & `decentriq-platform-0.9.1.tar`

### file list

```diff
@@ -1,63 +1,47 @@
--rw-r--r--   0        0        0       72 2022-02-24 08:14:29.789439 decentriq-platform-0.9.0rc2/README.md
--rw-r--r--   0        0        0      797 2022-03-03 21:15:47.890201 decentriq-platform-0.9.0rc2/decentriq_platform/__init__.py
--rw-r--r--   0        0        0     6349 2022-03-02 08:15:56.247035 decentriq-platform-0.9.0rc2/decentriq_platform/api.py
--rw-r--r--   0        0        0     6162 2022-03-04 11:13:25.540778 decentriq-platform-0.9.0rc2/decentriq_platform/attestation.py
--rw-r--r--   0        0        0     2626 2022-02-24 08:14:29.789759 decentriq-platform-0.9.0rc2/decentriq_platform/authentication.py
--rw-r--r--   0        0        0     9072 2022-03-03 21:15:47.890822 decentriq-platform-0.9.0rc2/decentriq_platform/builders.py
--rw-r--r--   0        0        0     4018 2022-02-24 08:14:29.789898 decentriq-platform-0.9.0rc2/decentriq_platform/certs.py
--rw-r--r--   0        0        0    20283 2022-03-03 21:15:47.891193 decentriq-platform-0.9.0rc2/decentriq_platform/client.py
--rw-r--r--   0        0        0     2049 2022-03-04 12:51:18.550771 decentriq-platform-0.9.0rc2/decentriq_platform/compute.py
--rw-r--r--   0        0        0      605 2022-02-28 13:24:32.483905 decentriq-platform-0.9.0rc2/decentriq_platform/config.py
--rw-r--r--   0        0        0      287 2022-02-28 13:24:32.484250 decentriq-platform-0.9.0rc2/decentriq_platform/container/__init__.py
--rw-r--r--   0        0        0      468 2022-02-28 13:26:06.057798 decentriq-platform-0.9.0rc2/decentriq_platform/container/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      819 2022-02-16 17:09:24.873942 decentriq-platform-0.9.0rc2/decentriq_platform/container/__pycache__/attestation.cpython-39.pyc
--rw-r--r--   0        0        0     3062 2022-03-04 12:51:45.341258 decentriq-platform-0.9.0rc2/decentriq_platform/container/__pycache__/compute.cpython-39.pyc
--rw-r--r--   0        0        0      750 2022-02-28 13:26:06.060257 decentriq-platform-0.9.0rc2/decentriq_platform/container/__pycache__/helpers.cpython-39.pyc
--rw-r--r--   0        0        0     2758 2022-03-03 21:15:47.891520 decentriq-platform-0.9.0rc2/decentriq_platform/container/compute.py
--rw-r--r--   0        0        0      474 2022-02-28 13:24:32.484907 decentriq-platform-0.9.0rc2/decentriq_platform/container/helpers.py
--rw-r--r--   0        0        0       46 2022-02-24 08:14:29.790998 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/__init__.py
--rw-r--r--   0        0        0      253 2022-02-25 16:25:35.302188 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3108 2022-02-02 18:16:15.310903 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/__pycache__/attestation_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1524 2022-02-25 16:25:35.302795 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/__pycache__/compute_container_pb2.cpython-39.pyc
--rw-r--r--   0        0        0      991 2022-02-02 17:28:20.544495 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/__pycache__/length_delimited.cpython-39.pyc
--rw-r--r--   0        0        0     2633 2022-02-25 09:43:58.678591 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/compute_container_pb2.py
--rw-r--r--   0        0        0     2897 2022-02-25 14:33:53.449030 decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/compute_container_pb2.pyi
--rw-r--r--   0        0        0      681 2022-02-24 08:14:29.791213 decentriq-platform-0.9.0rc2/decentriq_platform/helpers.py
--rw-r--r--   0        0        0      846 2022-03-03 21:15:47.891793 decentriq-platform-0.9.0rc2/decentriq_platform/node.py
--rw-r--r--   0        0        0     2579 2022-02-24 08:14:29.791271 decentriq-platform-0.9.0rc2/decentriq_platform/permission.py
--rw-r--r--   0        0        0    27076 2022-03-03 21:15:47.892291 decentriq-platform-0.9.0rc2/decentriq_platform/platform.py
--rw-r--r--   0        0        0     1669 2022-02-28 13:24:32.485726 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__init__.py
--rw-r--r--   0        0        0     2254 2022-02-28 13:26:05.841178 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3132 2022-02-28 13:26:05.860252 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__pycache__/attestation_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5285 2022-02-28 13:26:05.842681 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__pycache__/data_room_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     2925 2022-02-28 13:26:05.873520 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__pycache__/delta_enclave_api_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     9263 2022-02-25 16:25:35.062773 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__pycache__/gcg_pb2.cpython-39.pyc
--rw-r--r--   0        0        0      973 2022-02-25 16:25:35.067664 decentriq-platform-0.9.0rc2/decentriq_platform/proto/__pycache__/length_delimited.cpython-39.pyc
--rw-r--r--   0        0        0     6924 2022-02-28 13:24:32.485867 decentriq-platform-0.9.0rc2/decentriq_platform/proto/attestation_pb2.py
--rw-r--r--   0        0        0     9554 2022-02-28 13:24:32.485997 decentriq-platform-0.9.0rc2/decentriq_platform/proto/attestation_pb2.pyi
--rw-r--r--   0        0        0    12176 2022-02-28 13:24:32.486143 decentriq-platform-0.9.0rc2/decentriq_platform/proto/data_room_pb2.py
--rw-r--r--   0        0        0    14960 2022-02-28 13:24:32.486367 decentriq-platform-0.9.0rc2/decentriq_platform/proto/data_room_pb2.pyi
--rw-r--r--   0        0        0     6848 2022-02-28 13:24:32.486489 decentriq-platform-0.9.0rc2/decentriq_platform/proto/delta_enclave_api_pb2.py
--rw-r--r--   0        0        0    13244 2022-02-28 13:24:32.486613 decentriq-platform-0.9.0rc2/decentriq_platform/proto/delta_enclave_api_pb2.pyi
--rw-r--r--   0        0        0    22247 2022-02-25 09:43:58.432183 decentriq-platform-0.9.0rc2/decentriq_platform/proto/gcg_pb2.py
--rw-r--r--   0        0        0    31871 2022-02-25 14:33:53.450774 decentriq-platform-0.9.0rc2/decentriq_platform/proto/gcg_pb2.pyi
--rw-r--r--   0        0        0      808 2022-02-24 08:14:29.792272 decentriq-platform-0.9.0rc2/decentriq_platform/proto/length_delimited.py
--rw-r--r--   0        0        0    28977 2022-03-03 21:15:47.892951 decentriq-platform-0.9.0rc2/decentriq_platform/session.py
--rw-r--r--   0        0        0      655 2022-02-28 13:24:32.487072 decentriq-platform-0.9.0rc2/decentriq_platform/sql/__init__.py
--rw-r--r--   0        0        0      708 2022-03-01 13:27:44.826600 decentriq-platform-0.9.0rc2/decentriq_platform/sql/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1035 2022-02-16 17:08:18.704595 decentriq-platform-0.9.0rc2/decentriq_platform/sql/__pycache__/attestation.cpython-39.pyc
--rw-r--r--   0        0        0     4378 2022-03-01 13:27:44.827721 decentriq-platform-0.9.0rc2/decentriq_platform/sql/__pycache__/compute.cpython-39.pyc
--rw-r--r--   0        0        0    15646 2022-03-04 12:51:45.355025 decentriq-platform-0.9.0rc2/decentriq_platform/sql/__pycache__/helpers.cpython-39.pyc
--rw-r--r--   0        0        0     4999 2022-02-28 13:24:32.487398 decentriq-platform-0.9.0rc2/decentriq_platform/sql/compute.py
--rw-r--r--   0        0        0    15559 2022-03-03 21:16:01.538092 decentriq-platform-0.9.0rc2/decentriq_platform/sql/helpers.py
--rw-r--r--   0        0        0      226 2022-02-24 08:14:29.792740 decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/__init__.py
--rw-r--r--   0        0        0      458 2022-03-01 13:27:44.839637 decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2826 2022-03-01 13:27:44.840742 decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/__pycache__/compute_sql_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5822 2022-02-25 09:43:58.553034 decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/compute_sql_pb2.py
--rw-r--r--   0        0        0     6887 2022-02-25 14:33:53.451213 decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/compute_sql_pb2.pyi
--rw-r--r--   0        0        0     3582 2022-03-03 21:15:47.893554 decentriq-platform-0.9.0rc2/decentriq_platform/storage.py
--rw-r--r--   0        0        0     4187 2022-03-03 21:15:47.893944 decentriq-platform-0.9.0rc2/decentriq_platform/types.py
--rw-r--r--   0        0        0    13779 2022-02-28 13:24:32.488062 decentriq-platform-0.9.0rc2/decentriq_platform/verification.py
--rw-r--r--   0        0        0      808 2022-03-04 13:08:01.459308 decentriq-platform-0.9.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1262 2022-03-04 13:18:30.255064 decentriq-platform-0.9.0rc2/setup.py
--rw-r--r--   0        0        0     1121 2022-03-04 13:18:30.255226 decentriq-platform-0.9.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       72 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/README.md
+-rw-r--r--   0        0        0      797 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/__init__.py
+-rw-r--r--   0        0        0     4730 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/api.py
+-rw-r--r--   0        0        0     6117 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/attestation.py
+-rw-r--r--   0        0        0     2626 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/authentication.py
+-rw-r--r--   0        0        0     9072 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/builders.py
+-rw-r--r--   0        0        0     4018 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/certs.py
+-rw-r--r--   0        0        0    20279 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/client.py
+-rw-r--r--   0        0        0     2049 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/compute.py
+-rw-r--r--   0        0        0      605 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/config.py
+-rw-r--r--   0        0        0      287 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/container/__init__.py
+-rw-r--r--   0        0        0     2758 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/container/compute.py
+-rw-r--r--   0        0        0      474 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/container/helpers.py
+-rw-r--r--   0        0        0       46 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/container/proto/__init__.py
+-rw-r--r--   0        0        0     2633 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/container/proto/compute_container_pb2.py
+-rw-r--r--   0        0        0     2897 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/container/proto/compute_container_pb2.pyi
+-rw-r--r--   0        0        0      681 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/helpers.py
+-rw-r--r--   0        0        0      846 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/node.py
+-rw-r--r--   0        0        0     2579 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/permission.py
+-rw-r--r--   0        0        0    27076 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/platform.py
+-rw-r--r--   0        0        0     1745 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/proto/__init__.py
+-rw-r--r--   0        0        0     6924 2022-04-01 16:41:23.790364 decentriq-platform-0.9.1/decentriq_platform/proto/attestation_pb2.py
+-rw-r--r--   0        0        0     9554 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/attestation_pb2.pyi
+-rw-r--r--   0        0        0     5822 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/compute_sql_pb2.py
+-rw-r--r--   0        0        0     6887 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/compute_sql_pb2.pyi
+-rw-r--r--   0        0        0    12176 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/data_room_pb2.py
+-rw-r--r--   0        0        0    14960 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/data_room_pb2.pyi
+-rw-r--r--   0        0        0     6848 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/delta_enclave_api_pb2.py
+-rw-r--r--   0        0        0    13244 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/delta_enclave_api_pb2.pyi
+-rw-r--r--   0        0        0    22247 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/gcg_pb2.py
+-rw-r--r--   0        0        0    31871 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/gcg_pb2.pyi
+-rw-r--r--   0        0        0      808 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/length_delimited.py
+-rw-r--r--   0        0        0     2940 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/synth_data_pb2.py
+-rw-r--r--   0        0        0     3777 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/proto/synth_data_pb2.pyi
+-rw-r--r--   0        0        0    28977 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/session.py
+-rw-r--r--   0        0        0      655 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/sql/__init__.py
+-rw-r--r--   0        0        0     4999 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/sql/compute.py
+-rw-r--r--   0        0        0    15970 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/sql/helpers.py
+-rw-r--r--   0        0        0      226 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/sql/proto/__init__.py
+-rw-r--r--   0        0        0     5822 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/sql/proto/compute_sql_pb2.py
+-rw-r--r--   0        0        0     6887 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/sql/proto/compute_sql_pb2.pyi
+-rw-r--r--   0        0        0     3582 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/storage.py
+-rw-r--r--   0        0        0     4187 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/types.py
+-rw-r--r--   0        0        0    13779 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/decentriq_platform/verification.py
+-rw-r--r--   0        0        0      805 2022-04-01 16:41:23.794365 decentriq-platform-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1259 2022-04-01 16:41:55.484592 decentriq-platform-0.9.1/setup.py
+-rw-r--r--   0        0        0     1118 2022-04-01 16:41:55.484881 decentriq-platform-0.9.1/PKG-INFO
```

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/__init__.py` & `decentriq-platform-0.9.1/decentriq_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/attestation.py` & `decentriq-platform-0.9.1/decentriq_platform/attestation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from typing import Dict, List, Tuple
-import hashlib
 from .types import EnclaveSpecification
 from .proto import (
     AttestationSpecification,
     AttestationSpecificationIntelEpid,
     AttestationSpecificationIntelDcap,
     AttestationSpecificationAwsNitro,
     ComputeNodeProtocol,
-    serialize_length_delimited
 )
 import asn1crypto.pem
 from .certs import (
     aws_nitro_root_ca_pem,
     intel_sgx_dcap_root_ca,
     intel_sgx_ias_root_ca
 )
 
+
 intel_sgx_dcap_root_ca_der = asn1crypto.pem.unarmor(intel_sgx_dcap_root_ca)[2]
 intel_sgx_ias_root_ca_der = asn1crypto.pem.unarmor(intel_sgx_ias_root_ca)[2]
 aws_nitro_root_ca_der = asn1crypto.pem.unarmor(aws_nitro_root_ca_pem)[2]
 
 
 SPECIFICATIONS = {
     "decentriq.driver:v2": EnclaveSpecification(
```

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/authentication.py` & `decentriq-platform-0.9.1/decentriq_platform/authentication.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/builders.py` & `decentriq-platform-0.9.1/decentriq_platform/builders.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/certs.py` & `decentriq-platform-0.9.1/decentriq_platform/certs.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/client.py` & `decentriq-platform-0.9.1/decentriq_platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,40 +147,40 @@
         response: ScopeJson = self._api.post(
                 url,
                 json.dumps(req_body),
                 {"Content-type": "application/json"}
         ).json()
         return response["scopeId"]
 
-    def _get_scope(self, email: str, scope_id: str) -> ScopeJson:
+    def get_scope(self, email: str, scope_id: str) -> ScopeJson:
         url = Endpoints.USER_SCOPE \
                 .replace(":userId", email) \
                 .replace(":scopeId", scope_id)
         response: ScopeJson = self._api.get(url).json()
         return response
 
-    def _get_scope_by_metadata(self, email: str, metadata: Dict[str, str]) -> Optional[str]:
+    def get_scope_by_metadata(self, email: str, metadata: Dict[str, str]) -> Optional[str]:
         url = Endpoints.USER_SCOPES_COLLECTION.replace(":userId", email)
         response: List[ScopeJson] = self._api.get(
                 url,
                 params={"metadata": json.dumps(metadata)}
             ).json()
         if len(response) == 0:
             return None
         else:
             scope = response[0]
             return scope["scopeId"]
 
     def _ensure_scope_with_metadata(self, email: str, metadata: Dict[str, str]) -> str:
-        scope = self._get_scope_by_metadata(email, metadata)
+        scope = self.get_scope_by_metadata(email, metadata)
         if scope is None:
             scope = self._create_scope(email, metadata)
         return scope
 
-    def _delete_scope(self, email: str, scope_id: str):
+    def delete_scope(self, email: str, scope_id: str):
         url = Endpoints.USER_SCOPE \
             .replace(":userId", email) \
             .replace(":scopeId", scope_id)
         self._api.delete(url)
 
     def upload_dataset(
             self,
```

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/compute.py` & `decentriq-platform-0.9.1/decentriq_platform/compute.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/config.py` & `decentriq-platform-0.9.1/decentriq_platform/config.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/container/compute.py` & `decentriq-platform-0.9.1/decentriq_platform/container/compute.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/compute_container_pb2.py` & `decentriq-platform-0.9.1/decentriq_platform/container/proto/compute_container_pb2.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/container/proto/compute_container_pb2.pyi` & `decentriq-platform-0.9.1/decentriq_platform/container/proto/compute_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/helpers.py` & `decentriq-platform-0.9.1/decentriq_platform/helpers.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/node.py` & `decentriq-platform-0.9.1/decentriq_platform/node.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/permission.py` & `decentriq-platform-0.9.1/decentriq_platform/permission.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/platform.py` & `decentriq-platform-0.9.1/decentriq_platform/platform.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/__init__.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,8 +37,12 @@
     StaticContentConfig,
 )
 from .length_delimited import parse_length_delimited, serialize_length_delimited
 from .delta_enclave_api_pb2 import (
     ChunkHeader, EncryptionHeader, VersionHeader,
     DataNoncePubkey, Request, Response
 )
-
+from .synth_data_pb2 import (
+    SyntheticDataConf,
+    Mask,
+    Column,
+)
```

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/attestation_pb2.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/attestation_pb2.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/attestation_pb2.pyi` & `decentriq-platform-0.9.1/decentriq_platform/proto/attestation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/data_room_pb2.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/data_room_pb2.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/data_room_pb2.pyi` & `decentriq-platform-0.9.1/decentriq_platform/proto/data_room_pb2.pyi`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/delta_enclave_api_pb2.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/delta_enclave_api_pb2.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/delta_enclave_api_pb2.pyi` & `decentriq-platform-0.9.1/decentriq_platform/proto/delta_enclave_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/gcg_pb2.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/gcg_pb2.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/gcg_pb2.pyi` & `decentriq-platform-0.9.1/decentriq_platform/proto/gcg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/proto/length_delimited.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/length_delimited.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/session.py` & `decentriq-platform-0.9.1/decentriq_platform/session.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/sql/__init__.py` & `decentriq-platform-0.9.1/decentriq_platform/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/sql/__pycache__/helpers.cpython-39.pyc` & `decentriq-platform-0.9.1/decentriq_platform/sql/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,978 +1,999 @@
-00000000: 610d 0d0a 0000 0000 1130 2162 c73c 0000  a........0!b.<..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000a 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
-00000050: 6d05 5a05 6d06 5a06 0100 6403 6404 6c07  m.Z.m.Z...d.d.l.
-00000060: 6d08 5a08 0100 6405 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 0100 6405  m.Z.m.Z.m.Z...d.
-00000080: 6407 6c07 6d0e 5a0e 0100 6403 6408 6c0f  d.l.m.Z...d.d.l.
-00000090: 6d10 5a10 0100 6405 6409 6c0f 6d11 5a11  m.Z...d.d.l.m.Z.
-000000a0: 6d12 5a12 0100 6405 640a 6c13 6d14 5a14  m.Z...d.d.l.m.Z.
-000000b0: 0100 6515 640b 9c01 640c 640d 8404 5a16  ..e.d...d.d...Z.
-000000c0: 6515 640b 9c01 640e 640f 8404 5a17 4700  e.d...d.d...Z.G.
-000000d0: 6410 6411 8400 6411 8302 5a18 6412 6412  d.d...d...Z.d.d.
-000000e0: 6413 6414 9c03 6515 6519 6519 6501 6a1a  d.d...e.e.e.e.j.
-000000f0: 6415 9c04 6416 6417 8406 5a1b 6412 6412  d...d.d...Z.d.d.
-00000100: 6418 9c02 6515 6519 6519 6501 6a1a 6419  d...e.e.e.e.j.d.
-00000110: 9c04 641a 641b 8406 5a1c 6412 6412 6418  ..d.d...Z.d.d.d.
-00000120: 9c02 6501 6a1d 6519 6519 6501 6a1a 641c  ..e.j.e.e.e.j.d.
-00000130: 9c04 641d 641e 8406 5a1e 641f 6412 6420  ..d.d...Z.d.d.d 
-00000140: 9c02 6501 6a1a 650c 6515 6515 650b 6515  ..e.j.e.e.e.e.e.
-00000150: 6519 6515 6421 9c08 6422 6423 8406 5a1f  e.e.d!..d"d#..Z.
-00000160: 6520 6505 6515 6510 6602 1900 6424 9c02  e e.e.e.f...d$..
-00000170: 6425 6426 8404 5a21 6520 6505 6504 6504  d%d&..Z!e e.e.e.
-00000180: 6515 1900 1900 6510 6602 1900 6424 9c02  e.....e.f...d$..
-00000190: 6427 6428 8404 5a22 642c 6520 6519 6515  d'd(..Z"d,e e.e.
-000001a0: 6429 9c03 642a 642b 8405 5a23 6401 5300  d)..d*d+..Z#d.S.
-000001b0: 292d e900 0000 004e 2903 da04 4c69 7374  )-.....N)...List
-000001c0: da05 5475 706c 65da 0341 6e79 e901 0000  ..Tuple..Any....
-000001d0: 0029 01da 1153 716c 5363 6865 6d61 5665  .)...SqlSchemaVe
-000001e0: 7269 6669 6572 e902 0000 0029 04da 0b50  rifier.....)...P
-000001f0: 6572 6d69 7373 696f 6e73 da07 5365 7373  ermissions..Sess
-00000200: 696f 6eda 034b 6579 da0f 4461 7461 526f  ion..Key..DataRo
-00000210: 6f6d 4275 696c 6465 7229 01da 044e 6f6f  omBuilder)...Noo
-00000220: 7029 01da 0b54 6162 6c65 5363 6865 6d61  p)...TableSchema
-00000230: 2902 da0a 5065 726d 6973 7369 6f6e da14  )...Permission..
-00000240: 4175 7468 656e 7469 6361 7469 6f6e 4d65  AuthenticationMe
-00000250: 7468 6f64 2901 da16 7061 7273 655f 6c65  thod)...parse_le
-00000260: 6e67 7468 5f64 656c 696d 6974 6564 a901  ngth_delimited..
-00000270: da04 6e6f 6465 6301 0000 0000 0000 0000  ..nodec.........
-00000280: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-00000290: 0c00 0000 6401 7c00 9b00 6402 9d03 5300  ....d.|...d...S.
-000002a0: 2903 4efa 0740 7461 626c 652f 7a08 2f64  ).N..@table/z./d
-000002b0: 6174 6173 6574 a900 7211 0000 0072 1400  ataset..r....r..
-000002c0: 0000 7214 0000 00fa 782f 5573 6572 732f  ..r.....x/Users/
-000002d0: 7268 6166 656e 2f64 712f 6465 762f 6465  rhafen/dq/dev/de
-000002e0: 6c74 612f 6176 6174 6f2d 636c 6965 6e74  lta/avato-client
-000002f0: 732f 6465 6365 6e74 7269 715f 706c 6174  s/decentriq_plat
-00000300: 666f 726d 5f64 6f63 732f 2e2e 2f64 6563  form_docs/../dec
-00000310: 656e 7472 6971 5f70 6c61 7466 6f72 6d2f  entriq_platform/
-00000320: 6465 6365 6e74 7269 715f 706c 6174 666f  decentriq_platfo
-00000330: 726d 2f73 716c 2f68 656c 7065 7273 2e70  rm/sql/helpers.p
-00000340: 79da 0f5f 6461 7461 5f6e 6f64 655f 6e61  y.._data_node_na
-00000350: 6d65 0d00 0000 7302 0000 0000 0172 1600  me....s......r..
-00000360: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000370: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
-00000380: 6401 7c00 9b00 6402 9d03 5300 2903 4e72  d.|...d...S.).Nr
-00000390: 1300 0000 7a0b 2f76 616c 6964 6174 696f  ....z./validatio
-000003a0: 6e72 1400 0000 7211 0000 0072 1400 0000  nr....r....r....
-000003b0: 7214 0000 0072 1500 0000 da0f 5f6e 6f6f  r....r......_noo
-000003c0: 705f 6e6f 6465 5f6e 616d 6511 0000 0073  p_node_name....s
-000003d0: 0200 0000 0001 7217 0000 0063 0000 0000  ......r....c....
-000003e0: 0000 0000 0000 0000 0000 0000 0700 0000  ................
-000003f0: 4000 0000 7394 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00000400: 0264 015a 0364 0264 039c 0165 0465 0565  .d.Z.d.d...e.e.e
-00000410: 0665 0465 0765 0866 0319 0019 0065 0864  .e.e.e.f.....e.d
-00000420: 049c 0364 0564 0684 065a 0965 0a65 0b65  ...d.d...Z.e.e.e
-00000430: 0565 0419 0064 079c 0364 0864 0984 045a  .e...d...d.d...Z
-00000440: 0c65 0d65 0e64 0a9c 0164 0b64 0c84 0483  .e.e.d...d.d....
-00000450: 015a 0f65 0d65 0e64 0a9c 0164 0d64 0e84  .Z.e.e.d...d.d..
-00000460: 0483 015a 1065 0d65 0464 0a9c 0164 0f64  ...Z.e.e.d...d.d
-00000470: 1084 0483 015a 1165 0d65 0464 0a9c 0164  .....Z.e.e.d...d
-00000480: 1164 1284 0483 015a 1264 1353 0029 14da  .d.....Z.d.S.)..
-00000490: 1654 6162 756c 6172 4461 7461 4e6f 6465  .TabularDataNode
-000004a0: 4275 696c 6465 7261 7808 0000 0a20 2020  Builderax....   
-000004b0: 2048 656c 7065 7220 636c 6173 7320 746f   Helper class to
-000004c0: 2063 6f6e 7374 7275 6374 2074 6865 2074   construct the t
-000004d0: 7269 706c 6574 206f 6620 6e6f 6465 7320  riplet of nodes 
-000004e0: 636f 6e73 6973 7469 6e67 206f 6620 6120  consisting of a 
-000004f0: 6461 7461 206e 6f64 6520 746f 0a20 2020  data node to.   
-00000500: 2073 746f 7265 2074 6162 756c 6172 2069   store tabular i
-00000510: 6e70 7574 2064 6174 612c 2061 7320 7765  nput data, as we
-00000520: 6c6c 2061 7320 6120 7363 6865 6d61 2076  ll as a schema v
-00000530: 616c 6964 6174 696f 6e20 636f 6d70 7574  alidation comput
-00000540: 6174 696f 6e2e 0a0a 2020 2020 496e 2061  ation...    In a
-00000550: 2064 6174 6120 636c 6561 6e20 726f 6f6d   data clean room
-00000560: 2063 6f6d 7075 7461 7469 6f6e 7320 616e   computations an
-00000570: 6420 7468 6520 6461 7461 2074 6865 7920  d the data they 
-00000580: 6465 7065 6e64 206f 6e20 6172 6520 6578  depend on are ex
-00000590: 7072 6573 7365 6420 696e 2074 6572 6d73  pressed in terms
-000005a0: 0a20 2020 206f 6620 6772 6170 6873 2077  .    of graphs w
-000005b0: 6865 7265 2063 6f6d 7075 7461 7469 6f6e  here computation
-000005c0: 7320 6172 6520 7265 7072 6573 656e 7465  s are represente
-000005d0: 6420 6279 202a 636f 6d70 7574 6520 6e6f  d by *compute no
-000005e0: 6465 732a 2061 6e64 2069 6e70 7574 2064  des* and input d
-000005f0: 6174 6173 6574 7320 6172 650a 2020 2020  atasets are.    
-00000600: 7265 7072 6573 656e 7465 6420 6279 202a  represented by *
-00000610: 6461 7461 206e 6f64 6573 2a2e 0a20 2020  data nodes*..   
-00000620: 2057 6974 6820 7461 6275 6c61 7220 696e   With tabular in
-00000630: 7075 7420 6461 7461 2c20 6974 2069 7320  put data, it is 
-00000640: 706f 7373 6962 6c65 2074 6f20 7661 6c69  possible to vali
-00000650: 6461 7465 2074 6865 2069 6e70 7574 2064  date the input d
-00000660: 6174 6120 616e 6420 6368 6563 6b20 7768  ata and check wh
-00000670: 6574 6865 7220 6974 0a20 2020 2063 6f72  ether it.    cor
-00000680: 7265 7370 6f6e 6473 2074 6f20 6120 7072  responds to a pr
-00000690: 652d 6465 6669 6e65 6420 7363 6865 6d61  e-defined schema
-000006a0: 2e20 5468 6973 2076 616c 6964 6174 696f  . This validatio
-000006b0: 6e20 6973 2061 2063 6f6d 7075 7461 7469  n is a computati
-000006c0: 6f6e 2069 6e20 6974 7365 6c66 2073 6f20  on in itself so 
-000006d0: 696e 0a20 2020 206f 7264 6572 2074 6f20  in.    order to 
-000006e0: 7661 6c69 6461 7465 2074 6865 2069 6e70  validate the inp
-000006f0: 7574 2064 6174 612c 2077 6520 6e65 6564  ut data, we need
-00000700: 2074 6f20 6164 6420 616e 2061 6464 6974   to add an addit
-00000710: 696f 6e61 6c20 636f 6d70 7574 6520 6e6f  ional compute no
-00000720: 6465 206f 6e20 746f 7020 6f66 2074 6865  de on top of the
-00000730: 0a20 2020 2064 6174 6120 6e6f 6465 2e20  .    data node. 
-00000740: 4265 6361 7573 6520 6974 206d 7573 7420  Because it must 
-00000750: 6265 2070 6f73 7369 626c 6520 746f 2074  be possible to t
-00000760: 7269 6767 6572 2074 6869 7320 7661 6c69  rigger this vali
-00000770: 6461 7469 6f6e 202a 7768 696c 6520 7265  dation *while re
-00000780: 7374 7269 6374 696e 6720 6163 6365 7373  stricting access
-00000790: 0a20 2020 2074 6f20 7468 6520 7265 7375  .    to the resu
-000007a0: 6c74 696e 6720 6461 7461 2a2c 2061 6e6f  lting data*, ano
-000007b0: 7468 6572 2073 7065 6369 616c 206e 6f64  ther special nod
-000007c0: 652c 2074 6865 202a 6e6f 6f70 206e 6f64  e, the *noop nod
-000007d0: 652a 206e 6565 6473 2074 6f20 6265 2061  e* needs to be a
-000007e0: 6464 6564 2e0a 0a20 2020 2054 6869 7320  dded...    This 
-000007f0: 636c 6173 7320 7769 6c6c 2061 6464 2074  class will add t
-00000800: 6865 206e 6563 6573 7361 7279 206e 6f64  he necessary nod
-00000810: 6573 2074 6f20 796f 7572 2064 6174 6120  es to your data 
-00000820: 636c 6561 6e20 726f 6f6d 2e0a 0a20 2020  clean room...   
-00000830: 2041 6674 6572 2068 6176 696e 6720 636f   After having co
-00000840: 6e73 7472 7563 7465 6420 616e 206f 626a  nstructed an obj
-00000850: 6563 7420 6f66 2074 6869 7320 636c 6173  ect of this clas
-00000860: 732c 2063 616c 6c20 6974 7320 6061 6464  s, call its `add
-00000870: 5f74 6f5f 6275 696c 6465 7260 206d 6574  _to_builder` met
-00000880: 686f 640a 2020 2020 616e 6420 7061 7373  hod.    and pass
-00000890: 2069 7420 6120 6044 6174 6152 6f6f 6d42   it a `DataRoomB
-000008a0: 7569 6c64 6572 6020 696e 7374 616e 6365  uilder` instance
-000008b0: 2e20 5468 6973 2077 696c 6c20 6164 6420  . This will add 
-000008c0: 7468 6520 6e65 6365 7373 6172 7920 6e6f  the necessary no
-000008d0: 6465 7320 616e 6420 7265 7175 6972 6564  des and required
-000008e0: 0a20 2020 2075 7365 7220 7065 726d 6973  .    user permis
-000008f0: 7369 6f6e 7320 746f 2074 6865 2062 7569  sions to the bui
-00000900: 6c64 6572 2069 6e73 7461 6e63 652e 0a0a  lder instance...
-00000910: 2020 2020 4461 7461 2073 686f 756c 6420      Data should 
-00000920: 6265 2070 7562 6c69 7368 6564 2074 6f20  be published to 
-00000930: 7468 6520 6e6f 6465 206e 616d 6564 2060  the node named `
-00000940: 696e 7075 745f 6e6f 6465 5f6e 616d 6560  input_node_name`
-00000950: 2061 6e64 2062 6520 7265 6164 2066 726f   and be read fro
-00000960: 6d20 606f 7574 7075 745f 6e6f 6465 5f6e  m `output_node_n
-00000970: 616d 6560 2e0a 2020 2020 5468 6520 6e61  ame`..    The na
-00000980: 6d65 206f 6620 7468 6520 7661 6c69 6461  me of the valida
-00000990: 7469 6f6e 2063 6f6d 7075 7461 7469 6f6e  tion computation
-000009a0: 2063 616e 2062 6520 6163 6365 7373 6564   can be accessed
-000009b0: 2075 7369 6e67 2074 6865 2066 6965 6c64   using the field
-000009c0: 2060 7661 6c69 6461 7469 6f6e 5f63 6f6d   `validation_com
-000009d0: 7075 7461 7469 6f6e 5f6e 616d 6560 2e0a  putation_name`..
-000009e0: 0a20 2020 2054 6869 7320 636c 6173 7320  .    This class 
-000009f0: 7573 6573 2061 2073 7065 6369 616c 206e  uses a special n
-00000a00: 616d 696e 6720 636f 6e76 656e 7469 6f6e  aming convention
-00000a10: 2074 6f20 6e61 6d65 2074 6865 206e 6f64   to name the nod
-00000a20: 6573 2061 6464 6564 2074 6f20 7468 6520  es added to the 
-00000a30: 6461 7461 2072 6f6f 6d20 6261 7365 6420  data room based 
-00000a40: 6f6e 0a20 2020 2074 6865 2074 6162 6c65  on.    the table
-00000a50: 206e 616d 6520 6769 7665 6e20 746f 2074   name given to t
-00000a60: 6865 2062 7569 6c64 6572 2e20 4173 7375  he builder. Assu
-00000a70: 6d69 6e67 2079 6f75 2075 7365 2060 226d  ming you use `"m
-00000a80: 795f 7461 626c 6522 6020 6173 2074 6865  y_table"` as the
-00000a90: 2060 7461 626c 655f 6e61 6d65 6020 7768   `table_name` wh
-00000aa0: 656e 0a20 2020 2069 6e73 7461 6e74 6961  en.    instantia
-00000ab0: 7469 6e67 2074 6865 2060 5461 6275 6c61  ting the `Tabula
-00000ac0: 7244 6174 614e 6f64 6542 7569 6c64 6572  rDataNodeBuilder
-00000ad0: 602c 2074 6865 6e20 7468 6520 666f 6c6c  `, then the foll
-00000ae0: 6f77 696e 6720 7468 7265 6520 6e6f 6465  owing three node
-00000af0: 7320 7769 6c6c 2062 6520 6164 6465 643a  s will be added:
-00000b00: 0a0a 2020 2020 312e 2060 4074 6162 6c65  ..    1. `@table
-00000b10: 2f6d 795f 7461 626c 652f 6461 7461 7365  /my_table/datase
-00000b20: 7460 202d 2074 6865 2064 6174 6120 6e6f  t` - the data no
-00000b30: 6465 2074 6f20 7768 6963 6820 796f 7520  de to which you 
-00000b40: 6361 6e20 7570 6c6f 6164 2064 6174 612e  can upload data.
-00000b50: 0a20 2020 2032 2e20 606d 795f 7461 626c  .    2. `my_tabl
-00000b60: 6560 202d 2074 6865 206e 616d 6520 6f66  e` - the name of
-00000b70: 2074 6865 2063 6f6d 7075 7465 206e 6f64   the compute nod
-00000b80: 6520 7468 6174 2076 6572 6966 6965 7320  e that verifies 
-00000b90: 7468 6520 7363 6865 6d61 206f 6620 7468  the schema of th
-00000ba0: 6520 6461 7461 2e0a 2020 2020 2020 2020  e data..        
-00000bb0: 5375 6273 6571 7565 6e74 2053 514c 2063  Subsequent SQL c
-00000bc0: 6f6d 7075 7465 206e 6f64 6573 2073 686f  ompute nodes sho
-00000bd0: 756c 6420 7265 6164 2064 6174 6120 6672  uld read data fr
-00000be0: 6f6d 2074 6869 7320 6e6f 6465 2e0a 2020  om this node..  
-00000bf0: 2020 332e 2060 4074 6162 6c65 2f6d 795f    3. `@table/my_
-00000c00: 7461 626c 652f 7661 6c69 6461 7469 6f6e  table/validation
-00000c10: 6020 2d20 7468 6520 6e61 6d65 206f 6620  ` - the name of 
-00000c20: 6120 7370 6563 6961 6c20 7472 6967 6765  a special trigge
-00000c30: 7220 6e6f 6465 2074 6861 7420 6361 6e20  r node that can 
-00000c40: 6265 2075 7365 6420 746f 2074 7269 6767  be used to trigg
-00000c50: 6572 2074 6865 2076 616c 6964 6174 696f  er the validatio
-00000c60: 6e20 636f 6d70 7574 6174 696f 6e2e 0a0a  n computation...
-00000c70: 2020 2020 5468 6520 6865 6c70 6572 2066      The helper f
-00000c80: 756e 6374 696f 6e20 6075 706c 6f61 645f  unction `upload_
-00000c90: 616e 645f 7075 626c 6973 685f 7461 6275  and_publish_tabu
-00000ca0: 6c61 725f 6461 7461 7365 7460 2077 696c  lar_dataset` wil
-00000cb0: 6c20 7570 6c6f 6164 2c20 7075 626c 6973  l upload, publis
-00000cc0: 682c 2061 6e64 2076 616c 6964 6174 6520  h, and validate 
-00000cd0: 796f 7572 0a20 2020 2064 6174 6120 6175  your.    data au
-00000ce0: 746f 6d61 7469 6361 6c6c 792c 2077 6974  tomatically, wit
-00000cf0: 686f 7574 2079 6f75 2068 6176 696e 6720  hout you having 
-00000d00: 746f 2077 6f72 7279 2061 626f 7574 2069  to worry about i
-00000d10: 6e74 6572 6e61 6c20 6e61 6d69 6e67 2e0a  nternal naming..
-00000d20: 2020 2020 46a9 01da 0b69 735f 7265 7175      F....is_requ
-00000d30: 6972 6564 2903 da0a 7461 626c 655f 6e61  ired)...table_na
-00000d40: 6d65 da06 7363 6865 6d61 721a 0000 0063  me..schemar....c
-00000d50: 0300 0000 0000 0000 0100 0000 0400 0000  ................
-00000d60: 0500 0000 4300 0000 7354 0000 007c 017c  ....C...sT...|.|
-00000d70: 005f 007c 037c 005f 0174 027c 0183 017c  ._.|.|._.t.|...|
-00000d80: 005f 037c 017c 005f 0474 057c 0183 017c  ._.|.|._.t.|...|
-00000d90: 005f 0674 077c 006a 047c 006a 037c 0264  ._.t.|.j.|.j.|.d
-00000da0: 018d 037c 005f 0874 097c 006a 067c 006a  ...|._.t.|.j.|.j
-00000db0: 086a 0a67 0164 028d 027c 005f 0b64 0353  .j.g.d...|._.d.S
-00000dc0: 0029 0461 b302 0000 0a20 2020 2020 2020  .).a.....       
-00000dd0: 2043 7265 6174 6520 6120 6054 6162 756c   Create a `Tabul
-00000de0: 6172 4461 7461 4e6f 6465 4275 696c 6465  arDataNodeBuilde
-00000df0: 7260 2e0a 0a20 2020 2020 2020 202a 2a50  r`...        **P
-00000e00: 6172 616d 6574 6572 732a 2a3a 0a20 2020  arameters**:.   
-00000e10: 2020 2020 202d 2060 7461 626c 655f 6e61       - `table_na
-00000e20: 6d65 603a 2057 6861 7420 796f 7572 2064  me`: What your d
-00000e30: 6174 6173 6574 2073 686f 756c 6420 6265  ataset should be
-00000e40: 2063 616c 6c65 642e 2054 6869 7320 6973   called. This is
-00000e50: 2074 6865 206e 616d 6520 796f 7520 7769   the name you wi
-00000e60: 6c6c 206c 6174 6572 2075 7365 2069 6e0a  ll later use in.
-00000e70: 2020 2020 2020 2020 2020 2020 796f 7572              your
-00000e80: 2053 514c 2071 7565 7269 6573 2e0a 2020   SQL queries..  
-00000e90: 2020 2020 2020 2d20 6073 6368 656d 6160        - `schema`
-00000ea0: 3a20 5468 6520 6c69 7374 206f 6620 636f  : The list of co
-00000eb0: 6c75 6d6e 732e 2054 6869 7320 6973 2061  lumns. This is a
-00000ec0: 206c 6973 7420 6f66 2074 7570 6c65 732c   list of tuples,
-00000ed0: 2065 6163 6820 636f 6e74 6169 6e69 6e67   each containing
-00000ee0: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
-00000ef0: 2063 6f6c 756d 6e2c 0a20 2020 2020 2020   column,.       
-00000f00: 2020 2020 2074 6865 2064 6174 6120 7479       the data ty
-00000f10: 7065 2028 6064 6563 656e 7472 6971 5f70  pe (`decentriq_p
-00000f20: 6c61 7466 6f72 6d2e 7371 6c2e 7072 6f74  latform.sql.prot
-00000f30: 6f2e 5072 696d 6974 6976 6554 7970 6560  o.PrimitiveType`
-00000f40: 292c 2061 6e64 2077 6865 7468 6572 2074  ), and whether t
-00000f50: 6865 2063 6f6c 756d 6e20 6973 206e 756c  he column is nul
-00000f60: 6c61 626c 6520 2863 616e 2068 6176 6520  lable (can have 
-00000f70: 656d 7074 7920 7661 6c75 6573 292e 0a20  empty values).. 
-00000f80: 2020 2020 2020 2020 2020 2054 6865 2064             The d
-00000f90: 6174 6120 7479 7065 2069 7320 616e 2065  ata type is an e
-00000fa0: 6e75 6d20 6c69 6b65 206f 626a 6563 7420  num like object 
-00000fb0: 7769 7468 2076 616c 7565 7320 6050 7269  with values `Pri
-00000fc0: 6d69 7469 7665 5479 7065 2e53 5452 494e  mitiveType.STRIN
-00000fd0: 4760 2c20 6050 7269 6d69 7469 7665 5479  G`, `PrimitiveTy
-00000fe0: 7065 2e49 4e54 3634 602c 0a20 2020 2020  pe.INT64`,.     
-00000ff0: 2020 2020 2020 2060 5072 696d 6974 6976         `Primitiv
-00001000: 6554 7970 652e 464c 4f41 5436 3460 2e0a  eType.FLOAT64`..
-00001010: 2020 2020 2020 2020 2d20 6069 735f 7265          - `is_re
-00001020: 7175 6972 6564 603a 2057 6865 7468 6572  quired`: Whether
-00001030: 2074 6865 2064 6174 6173 6574 206e 6565   the dataset nee
-00001040: 6473 2074 6f20 6265 2070 7265 7365 6e74  ds to be present
-00001050: 2066 6f72 2063 6f6d 7075 7461 7469 6f6e   for computation
-00001060: 7320 746f 2062 6520 7472 6967 6765 7265  s to be triggere
-00001070: 642e 0a20 2020 2020 2020 2029 02da 0f69  d..        )...i
-00001080: 6e70 7574 5f64 6174 615f 6e6f 6465 da07  nput_data_node..
-00001090: 636f 6c75 6d6e 7329 01da 0c64 6570 656e  columns)...depen
-000010a0: 6465 6e63 6965 734e 290c 721b 0000 0072  denciesN).r....r
-000010b0: 1a00 0000 7216 0000 00da 0f5f 6c65 6166  ....r......_leaf
-000010c0: 5f6e 6f64 655f 6e61 6d65 da13 5f76 6572  _node_name.._ver
-000010d0: 6966 6965 725f 6e6f 6465 5f6e 616d 6572  ifier_node_namer
-000010e0: 1700 0000 da1b 7661 6c69 6461 7469 6f6e  ......validation
-000010f0: 5f63 6f6d 7075 7461 7469 6f6e 5f6e 616d  _computation_nam
-00001100: 6572 0600 0000 da09 5f76 6572 6966 6965  er......_verifie
-00001110: 7272 0c00 0000 da04 6e61 6d65 da05 5f6e  rr......name.._n
-00001120: 6f6f 7029 04da 0473 656c 6672 1b00 0000  oop)...selfr....
-00001130: 721c 0000 0072 1a00 0000 7214 0000 0072  r....r....r....r
-00001140: 1400 0000 7215 0000 00da 085f 5f69 6e69  ....r......__ini
-00001150: 745f 5f38 0000 0073 1600 0000 0013 0601  t__8...s........
-00001160: 0601 0a01 0602 0a03 0201 0401 0401 02fd  ................
-00001170: 0806 7a1f 5461 6275 6c61 7244 6174 614e  ..z.TabularDataN
-00001180: 6f64 6542 7569 6c64 6572 2e5f 5f69 6e69  odeBuilder.__ini
-00001190: 745f 5f29 03da 0762 7569 6c64 6572 da0e  t__)...builder..
-000011a0: 6175 7468 656e 7469 6361 7469 6f6e da05  authentication..
-000011b0: 7573 6572 7363 0400 0000 0000 0000 0000  usersc..........
-000011c0: 0000 0500 0000 0600 0000 4300 0000 7350  ..........C...sP
-000011d0: 0000 007c 016a 007c 006a 017c 006a 0264  ...|.j.|.j.|.j.d
-000011e0: 018d 0201 007c 01a0 037c 006a 04a1 0101  .....|...|.j....
-000011f0: 007c 01a0 037c 006a 05a1 0101 007c 0344  .|...|.j.....|.D
-00001200: 005d 1c7d 047c 016a 067c 047c 027c 006a  .].}.|.j.|.|.|.j
-00001210: 077c 006a 0867 0264 028d 0301 0071 2e64  .|.j.g.d.....q.d
-00001220: 0353 0029 0461 ba03 0000 0a20 2020 2020  .S.).a.....     
-00001230: 2020 2043 6f6e 6669 6775 7265 2074 6865     Configure the
-00001240: 2067 6976 656e 2060 4461 7461 526f 6f6d   given `DataRoom
-00001250: 4275 696c 6465 7260 2074 6f20 6275 696c  Builder` to buil
-00001260: 6420 7465 2066 696e 616c 2064 6174 6120  d te final data 
-00001270: 636c 6561 6e20 726f 6f6d 2077 6974 6820  clean room with 
-00001280: 7468 650a 2020 2020 2020 2020 6e65 6365  the.        nece
-00001290: 7373 6172 7920 636f 6d70 7574 6520 616e  ssary compute an
-000012a0: 6420 6461 7461 206e 6f64 6573 2e0a 2020  d data nodes..  
-000012b0: 2020 2020 2020 5468 6973 2063 616c 6c20        This call 
-000012c0: 7769 6c6c 2061 6c73 6f20 6164 6420 7468  will also add th
-000012d0: 6520 6e65 6365 7373 6172 7920 7065 726d  e necessary perm
-000012e0: 6973 7369 6f6e 7320 746f 2074 6865 2064  issions to the d
-000012f0: 6174 6120 726f 6f6d 0a20 2020 2020 2020  ata room.       
-00001300: 2062 7569 6c64 6572 2074 6861 7420 6c65   builder that le
-00001310: 7420 6561 6368 2075 7365 7220 696e 2074  t each user in t
-00001320: 6865 206c 6973 7420 6f66 2075 7365 7273  he list of users
-00001330: 2070 6572 666f 726d 2074 6865 2066 6f6c   perform the fol
-00001340: 6c6f 7769 6e67 0a20 2020 2020 2020 2074  lowing.        t
-00001350: 6173 6b73 3a0a 0a20 2020 2020 2020 2031  asks:..        1
-00001360: 2e20 5570 6c6f 6164 2064 6174 6120 746f  . Upload data to
-00001370: 2074 6865 2064 6174 6120 6e6f 6465 2e0a   the data node..
-00001380: 2020 2020 2020 2020 322e 2055 7365 2074          2. Use t
-00001390: 6865 2064 6174 6120 696e 2064 6f77 6e73  he data in downs
-000013a0: 7472 6561 6d20 636f 6d70 7574 6174 696f  tream computatio
-000013b0: 6e73 2077 6869 6c65 206d 616b 696e 6720  ns while making 
-000013c0: 7375 7265 0a20 2020 2020 2020 2020 2020  sure.           
-000013d0: 7468 6520 7363 6865 6d61 2069 7320 7661  the schema is va
-000013e0: 6c69 642e 0a20 2020 2020 2020 2033 2e20  lid..        3. 
-000013f0: 5472 6967 6765 7220 7468 6520 7363 6865  Trigger the sche
-00001400: 6d61 2076 616c 6964 6174 696f 6e20 7374  ma validation st
-00001410: 6570 2073 6570 6172 6174 656c 7920 6173  ep separately as
-00001420: 2069 7473 206f 776e 2063 6f6d 7075 7461   its own computa
-00001430: 7469 6f6e 2e0a 0a20 2020 2020 2020 202a  tion...        *
-00001440: 2a50 6172 616d 6574 6572 732a 2a3a 0a20  *Parameters**:. 
-00001450: 2020 2020 2020 202d 2060 6275 696c 6465         - `builde
-00001460: 7260 3a20 5468 6520 6275 696c 6465 7220  r`: The builder 
-00001470: 6f62 6a65 6374 2074 6f20 7768 6963 6820  object to which 
-00001480: 746f 2061 6464 2074 6865 2064 6174 6120  to add the data 
-00001490: 616e 6420 636f 6d70 7574 6520 6173 2077  and compute as w
-000014a0: 656c 6c20 6173 0a20 2020 2020 2020 2020  ell as.         
-000014b0: 2020 2074 6865 2070 6572 6d69 7373 696f     the permissio
-000014c0: 6e73 2e0a 2020 2020 2020 2020 2d20 6061  ns..        - `a
-000014d0: 7574 6865 6e74 6963 6174 696f 6e60 3a20  uthentication`: 
-000014e0: 5468 6520 6175 7468 656e 7469 6361 7469  The authenticati
-000014f0: 6f6e 206d 6574 686f 6420 7573 6564 2074  on method used t
-00001500: 6f20 6175 7468 656e 7469 6361 7465 2074  o authenticate t
-00001510: 6865 2075 7365 7273 0a20 2020 2020 2020  he users.       
-00001520: 2020 2020 2066 726f 6d20 7769 7468 696e       from within
-00001530: 2074 6865 2065 6e63 6c61 7665 2e0a 2020   the enclave..  
-00001540: 2020 2020 2020 2d20 6075 7365 7273 603a        - `users`:
-00001550: 2041 206c 6973 7420 6f66 2065 6d61 696c   A list of email
-00001560: 2061 6464 7265 7373 6573 2074 6861 7420   addresses that 
-00001570: 7769 6c6c 2062 6520 6769 7665 6e20 7065  will be given pe
-00001580: 726d 6973 7369 6f6e 7320 626f 7468 2066  rmissions both f
-00001590: 6f72 0a20 2020 2020 2020 2020 2020 2074  or.            t
-000015a0: 6865 2076 616c 6964 6174 696f 6e20 6f66  he validation of
-000015b0: 2074 6865 2064 6174 6120 6173 2077 656c   the data as wel
-000015c0: 6c20 6173 2074 6865 2075 706c 6f61 6469  l as the uploadi
-000015d0: 6e67 206f 6620 6461 7461 2e0a 2020 2020  ng of data..    
-000015e0: 2020 2020 7219 0000 0029 03da 0565 6d61      r....)...ema
-000015f0: 696c da15 6175 7468 656e 7469 6361 7469  il..authenticati
-00001600: 6f6e 5f6d 6574 686f 64da 0b70 6572 6d69  on_method..permi
-00001610: 7373 696f 6e73 4e29 09da 0d61 6464 5f64  ssionsN)...add_d
-00001620: 6174 615f 6e6f 6465 7220 0000 0072 1a00  ata_noder ...r..
-00001630: 0000 da10 6164 645f 636f 6d70 7574 655f  ....add_compute_
-00001640: 6e6f 6465 7223 0000 0072 2500 0000 da13  noder#...r%.....
-00001650: 6164 645f 7573 6572 5f70 6572 6d69 7373  add_user_permiss
-00001660: 696f 6eda 1576 616c 6964 6174 696f 6e5f  ion..validation_
-00001670: 7065 726d 6973 7369 6f6e da14 6c65 6166  permission..leaf
-00001680: 5f63 7275 645f 7065 726d 6973 7369 6f6e  _crud_permission
-00001690: 2905 7226 0000 0072 2800 0000 7229 0000  ).r&...r(...r)..
-000016a0: 0072 2a00 0000 722b 0000 0072 1400 0000  .r*...r+...r....
-000016b0: 7214 0000 0072 1500 0000 da0e 6164 645f  r....r......add_
-000016c0: 746f 5f62 7569 6c64 6572 5b00 0000 7316  to_builder[...s.
-000016d0: 0000 0000 1a12 010c 010c 0108 0104 0102  ................
-000016e0: 0102 0204 0104 fe02 fd7a 2554 6162 756c  .........z%Tabul
-000016f0: 6172 4461 7461 4e6f 6465 4275 696c 6465  arDataNodeBuilde
-00001700: 722e 6164 645f 746f 5f62 7569 6c64 6572  r.add_to_builder
-00001710: 2901 da06 7265 7475 726e 6301 0000 0000  )...returnc.....
-00001720: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00001730: 0000 0073 0c00 0000 7400 a001 7c00 6a02  ...s....t...|.j.
-00001740: a101 5300 2901 7a37 5468 6520 7065 726d  ..S.).z7The perm
-00001750: 6973 7369 6f6e 2072 6571 7569 7265 6420  ission required 
-00001760: 746f 2074 7269 6767 6572 2074 6865 2064  to trigger the d
-00001770: 6174 6120 7661 6c69 6461 7469 6f6e 2e29  ata validation.)
-00001780: 0372 0800 0000 da0f 6578 6563 7574 655f  .r......execute_
-00001790: 636f 6d70 7574 6572 2200 0000 a901 7226  computer".....r&
-000017a0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-000017b0: 0000 7231 0000 0082 0000 0073 0200 0000  ..r1.......s....
-000017c0: 0003 7a2c 5461 6275 6c61 7244 6174 614e  ..z,TabularDataN
-000017d0: 6f64 6542 7569 6c64 6572 2e76 616c 6964  odeBuilder.valid
-000017e0: 6174 696f 6e5f 7065 726d 6973 7369 6f6e  ation_permission
-000017f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001800: 0003 0000 0043 0000 0073 0c00 0000 7400  .....C...s....t.
-00001810: a001 7c00 6a02 a101 5300 2901 7a3e 5468  ..|.j...S.).z>Th
-00001820: 6520 7065 726d 6973 7369 6f6e 2072 6571  e permission req
-00001830: 7569 7265 6420 746f 2075 706c 6f61 6420  uired to upload 
-00001840: 7468 6520 7261 772c 206e 6f6e 2d76 616c  the raw, non-val
-00001850: 6964 6174 6564 2064 6174 612e 2903 7208  idated data.).r.
-00001860: 0000 00da 096c 6561 665f 6372 7564 7220  .....leaf_crudr 
-00001870: 0000 0072 3600 0000 7214 0000 0072 1400  ...r6...r....r..
-00001880: 0000 7215 0000 0072 3200 0000 8700 0000  ..r....r2.......
-00001890: 7302 0000 0000 037a 2b54 6162 756c 6172  s......z+Tabular
-000018a0: 4461 7461 4e6f 6465 4275 696c 6465 722e  DataNodeBuilder.
-000018b0: 6c65 6166 5f63 7275 645f 7065 726d 6973  leaf_crud_permis
-000018c0: 7369 6f6e 6301 0000 0000 0000 0000 0000  sionc...........
-000018d0: 0001 0000 0001 0000 0043 0000 0073 0600  .........C...s..
-000018e0: 0000 7c00 6a00 5300 2901 7a2f 5468 6520  ..|.j.S.).z/The 
-000018f0: 6e6f 6465 206e 616d 6520 746f 2077 6869  node name to whi
-00001900: 6368 2064 6174 6120 7368 6f75 6c64 2062  ch data should b
-00001910: 6520 7570 6c6f 6164 6564 2e29 0172 2000  e uploaded.).r .
-00001920: 0000 7236 0000 0072 1400 0000 7214 0000  ..r6...r....r...
-00001930: 0072 1500 0000 da0f 696e 7075 745f 6e6f  .r......input_no
-00001940: 6465 5f6e 616d 658c 0000 0073 0200 0000  de_name....s....
-00001950: 0003 7a26 5461 6275 6c61 7244 6174 614e  ..z&TabularDataN
-00001960: 6f64 6542 7569 6c64 6572 2e69 6e70 7574  odeBuilder.input
-00001970: 5f6e 6f64 655f 6e61 6d65 6301 0000 0000  _node_namec.....
-00001980: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
-00001990: 0000 0073 0600 0000 7c00 6a00 5300 2901  ...s....|.j.S.).
-000019a0: 7a5e 5468 6520 6e6f 6465 206e 616d 6520  z^The node name 
-000019b0: 6672 6f6d 2077 6869 6368 2064 6174 6120  from which data 
-000019c0: 6361 6e20 6265 2072 6561 642c 2065 2e67  can be read, e.g
-000019d0: 2e20 7468 6520 6e61 6d65 2074 6f20 7573  . the name to us
-000019e0: 6520 696e 2061 6e79 2064 6f77 6e73 7472  e in any downstr
-000019f0: 6561 6d20 5351 4c20 7175 6572 6965 732e  eam SQL queries.
-00001a00: 2901 7221 0000 0072 3600 0000 7214 0000  ).r!...r6...r...
-00001a10: 0072 1400 0000 7215 0000 00da 106f 7574  .r....r......out
-00001a20: 7075 745f 6e6f 6465 5f6e 616d 6591 0000  put_node_name...
-00001a30: 0073 0200 0000 0003 7a27 5461 6275 6c61  .s......z'Tabula
-00001a40: 7244 6174 614e 6f64 6542 7569 6c64 6572  rDataNodeBuilder
-00001a50: 2e6f 7574 7075 745f 6e6f 6465 5f6e 616d  .output_node_nam
-00001a60: 654e 2913 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
-00001a70: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00001a80: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00001a90: 5fda 0373 7472 7202 0000 0072 0300 0000  _..strr....r....
-00001aa0: 7204 0000 00da 0462 6f6f 6c72 2700 0000  r......boolr'...
-00001ab0: 720b 0000 0072 0f00 0000 7233 0000 00da  r....r....r3....
-00001ac0: 0870 726f 7065 7274 7972 0e00 0000 7231  .propertyr....r1
-00001ad0: 0000 0072 3200 0000 7238 0000 0072 3900  ...r2...r8...r9.
-00001ae0: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00001af0: 0072 1500 0000 7218 0000 0015 0000 0073  .r....r........s
-00001b00: 2600 0000 0801 0427 02fb 0402 0201 1002  &......'........
-00001b10: 02fb 0c25 0201 0201 06fc 0c27 0201 1004  ...%.......'....
-00001b20: 0201 1004 0201 1004 0201 7218 0000 0054  ..........r....T
-00001b30: 7a05 7574 662d 3829 03da 0a68 6173 5f68  z.utf-8)...has_h
-00001b40: 6561 6465 72da 0c63 6865 636b 5f68 6561  eader..check_hea
-00001b50: 6465 72da 0865 6e63 6f64 696e 6729 04da  der..encoding)..
-00001b60: 0470 6174 6872 4100 0000 7242 0000 0072  .pathrA...rB...r
-00001b70: 3400 0000 6301 0000 0001 0000 0003 0000  4...c...........
-00001b80: 0007 0000 0008 0000 004b 0000 0073 4c00  .........K...sL.
-00001b90: 0000 6700 7d05 7400 7c00 6401 7c03 6402  ..g.}.t.|.d.|.d.
-00001ba0: 8d03 8f26 7d06 7401 7c06 6601 7c01 7c02  ...&}.t.|.f.|.|.
-00001bb0: 6403 9c02 7c04 a401 8e01 5700 0200 6404  d...|.....W...d.
-00001bc0: 0400 0400 8303 0100 5300 3100 733e 3000  ........S.1.s>0.
-00001bd0: 0100 0100 0100 5900 0100 6404 5300 2905  ......Y...d.S.).
-00001be0: 6114 0500 000a 2020 2020 5265 6164 2043  a.....    Read C
-00001bf0: 5356 2066 726f 6d20 6120 6669 6c65 2061  SV from a file a
-00001c00: 6e64 2074 7572 6e20 6974 2069 6e74 6f20  nd turn it into 
-00001c10: 6120 6279 7465 7320 6172 7261 7920 6f66  a bytes array of
-00001c20: 2074 6865 2063 6f72 7265 6374 2066 6f72   the correct for
-00001c30: 6d61 7420 736f 2074 6861 7420 6974 2063  mat so that it c
-00001c40: 616e 2062 6520 7570 6c6f 6164 6564 0a20  an be uploaded. 
-00001c50: 2020 2074 6f20 7468 6520 4465 6365 6e74     to the Decent
-00001c60: 7269 7120 706c 6174 666f 726d 2e0a 0a20  riq platform... 
-00001c70: 2020 202a 2a50 6172 616d 6574 6572 732a     **Parameters*
-00001c80: 2a3a 0a20 2020 202d 2060 7061 7468 603a  *:.    - `path`:
-00001c90: 2054 6865 2070 6174 6820 746f 2074 6865   The path to the
-00001ca0: 2043 5356 2066 696c 652e 0a20 2020 202d   CSV file..    -
-00001cb0: 2060 6861 735f 6865 6164 6572 603a 2057   `has_header`: W
-00001cc0: 6865 7468 6572 2074 6865 2073 7472 696e  hether the strin
-00001cd0: 6720 636f 6e74 6169 6e73 2061 2068 6561  g contains a hea
-00001ce0: 6465 7220 726f 772e 0a20 2020 202d 2060  der row..    - `
-00001cf0: 6368 6563 6b5f 6865 6164 6572 603a 2057  check_header`: W
-00001d00: 6865 7468 6572 2074 6865 2066 756e 6374  hether the funct
-00001d10: 696f 6e20 7368 6f75 6c64 2074 7279 2074  ion should try t
-00001d20: 6f20 6465 7465 726d 696e 6520 7768 6574  o determine whet
-00001d30: 6865 7220 7468 6520 6669 6c65 2068 6173  her the file has
-00001d40: 2061 2068 6561 6465 722e 0a20 2020 2020   a header..     
-00001d50: 2020 2049 6620 7468 6520 6669 6c65 2068     If the file h
-00001d60: 6173 2061 2068 6561 6465 7220 726f 7720  as a header row 
-00001d70: 6275 7420 796f 7520 6469 646e 2774 2073  but you didn't s
-00001d80: 6574 2074 6865 2060 6861 735f 6865 6164  et the `has_head
-00001d90: 6572 6020 666c 6167 2c20 616e 0a20 2020  er` flag, an.   
-00001da0: 2020 2020 2065 7863 6570 7469 6f6e 2077       exception w
-00001db0: 696c 6c20 6265 2072 6169 7365 642e 2049  ill be raised. I
-00001dc0: 6620 796f 7527 7265 2073 7572 6520 7468  f you're sure th
-00001dd0: 6174 2074 6865 2077 6179 2079 6f75 2075  at the way you u
-00001de0: 7365 2074 6865 2066 756e 6374 696f 6e0a  se the function.
-00001df0: 2020 2020 2020 2020 6973 2063 6f72 7265          is corre
-00001e00: 6374 2c20 796f 7520 6361 6e20 6469 7361  ct, you can disa
-00001e10: 626c 6520 7468 6973 2063 6865 636b 2075  ble this check u
-00001e20: 7369 6e67 2074 6869 7320 7061 7261 6d65  sing this parame
-00001e30: 7465 722e 0a20 2020 202d 2060 656e 636f  ter..    - `enco
-00001e40: 6469 6e67 603a 2054 6865 2065 6e63 6f64  ding`: The encod
-00001e50: 696e 6720 6f66 2074 6865 2043 5356 2066  ing of the CSV f
-00001e60: 696c 652e 2049 6620 796f 7520 7772 6f74  ile. If you wrot
-00001e70: 6520 7468 6520 4353 5620 6669 6c65 2075  e the CSV file u
-00001e80: 7369 6e67 2061 206c 6962 7261 7279 206c  sing a library l
-00001e90: 696b 6520 7061 6e64 6173 2c0a 2020 2020  ike pandas,.    
-00001ea0: 2020 2020 796f 7520 6e65 6564 2074 6f20      you need to 
-00001eb0: 6368 6563 6b20 7468 6520 646f 6375 6d65  check the docume
-00001ec0: 6e74 6174 696f 6e20 746f 2073 6565 2077  ntation to see w
-00001ed0: 6861 7420 656e 636f 6469 6e67 2074 6865  hat encoding the
-00001ee0: 7920 7573 6520 6279 2064 6566 6175 6c74  y use by default
-00001ef0: 0a20 2020 2020 2020 2077 6865 6e20 7772  .        when wr
-00001f00: 6974 696e 6720 6669 6c65 7320 286c 696b  iting files (lik
-00001f10: 656c 7920 6022 7574 662d 3822 6020 696e  ely `"utf-8"` in
-00001f20: 2077 6869 6368 2063 6173 6520 7468 6973   which case this
-00001f30: 2063 616e 2062 6520 6c65 6674 2061 7420   can be left at 
-00001f40: 6974 7320 6465 6661 756c 7420 7661 6c75  its default valu
-00001f50: 6529 2e0a 2020 2020 2d20 6064 656c 696d  e)..    - `delim
-00001f60: 6974 6572 603a 2057 6861 7420 6465 6c69  iter`: What deli
-00001f70: 6d69 7465 7220 6973 2075 7365 6420 696e  miter is used in
-00001f80: 2074 6865 2074 6865 2043 5356 2066 696c   the the CSV fil
-00001f90: 652e 2044 6566 6175 6c74 2069 7320 7468  e. Default is th
-00001fa0: 6520 636f 6d6d 612e 0a20 2020 202d 2060  e comma..    - `
-00001fb0: 2a2a 6b77 6172 6773 603a 2041 6464 6974  **kwargs`: Addit
-00001fc0: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
-00001fd0: 6775 6d65 6e74 7320 7061 7373 6564 2074  guments passed t
-00001fe0: 6f20 7468 6520 5079 7468 6f6e 2043 5356  o the Python CSV
-00001ff0: 2070 6172 7365 722e 2052 6566 6572 2074   parser. Refer t
-00002000: 6f20 7468 650a 2020 2020 2020 2020 5b6f  o the.        [o
-00002010: 6666 6963 6961 6c20 646f 6375 6d65 6e74  fficial document
-00002020: 6174 696f 6e5d 2868 7474 7073 3a2f 2f64  ation](https://d
-00002030: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00002040: 2f6c 6962 7261 7279 2f63 7376 2e68 746d  /library/csv.htm
-00002050: 6c23 6373 762d 666d 742d 7061 7261 6d73  l#csv-fmt-params
-00002060: 290a 2020 2020 2020 2020 666f 7220 6120  ).        for a 
-00002070: 6c69 7374 206f 6620 7375 7070 6f72 7465  list of supporte
-00002080: 6420 6172 6775 6d65 6e74 732e 0a0a 2020  d arguments...  
-00002090: 2020 2a2a 5265 7475 726e 732a 2a3a 0a20    **Returns**:. 
-000020a0: 2020 2041 2042 7974 6573 494f 206f 626a     A BytesIO obj
-000020b0: 6563 7420 7468 6174 2063 616e 2062 6520  ect that can be 
-000020c0: 7061 7373 6564 2074 6f20 7468 6520 6d65  passed to the me
-000020d0: 7468 6f64 7320 7265 7370 6f73 6962 6c65  thods resposible
-000020e0: 2066 6f72 2075 706c 6f61 6469 6e67 2064   for uploading d
-000020f0: 6174 612e 0a20 2020 20da 0172 2901 7243  ata..    ..r).rC
-00002100: 0000 00a9 0272 4100 0000 7242 0000 004e  .....rA...rB...N
-00002110: 2902 da04 6f70 656e da0f 5f72 6561 645f  )...open.._read_
-00002120: 696e 7075 745f 6373 7629 0772 4400 0000  input_csv).rD...
-00002130: 7241 0000 0072 4200 0000 7243 0000 00da  rA...rB...rC....
-00002140: 066b 7761 7267 73da 056c 696e 6573 5a07  .kwargs..linesZ.
-00002150: 6373 7666 696c 6572 1400 0000 7214 0000  csvfiler....r...
-00002160: 0072 1500 0000 da13 7265 6164 5f69 6e70  .r......read_inp
-00002170: 7574 5f63 7376 5f66 696c 6597 0000 0073  ut_csv_file....s
-00002180: 1400 0000 001e 0401 1001 0201 02ff 0202  ................
-00002190: 0201 02fd 0404 02fc 724b 0000 0072 4600  ........rK...rF.
-000021a0: 0000 2904 da07 636f 6e74 656e 7472 4100  ..)...contentrA.
-000021b0: 0000 7242 0000 0072 3400 0000 6301 0000  ..rB...r4...c...
-000021c0: 0001 0000 0002 0000 0004 0000 0005 0000  ................
-000021d0: 004b 0000 0073 2000 0000 7400 7401 a002  .K...s ...t.t...
-000021e0: 7c00 a003 a100 a101 6601 7c01 7c02 6401  |.......f.|.|.d.
-000021f0: 9c02 7c03 a401 8e01 5300 2902 61bb 0400  ..|.....S.).a...
-00002200: 000a 2020 2020 5265 6164 2043 5356 2066  ..    Read CSV f
-00002210: 726f 6d20 6120 7374 7269 6e67 2061 6e64  rom a string and
-00002220: 2074 7572 6e20 6974 2069 6e74 6f20 6120   turn it into a 
-00002230: 6279 7465 7320 6172 7261 7920 6f66 2074  bytes array of t
-00002240: 6865 2063 6f72 7265 6374 2066 6f72 6d61  he correct forma
-00002250: 7420 736f 2074 6861 7420 6974 2063 616e  t so that it can
-00002260: 2062 6520 7570 6c6f 6164 6564 0a20 2020   be uploaded.   
-00002270: 2074 6f20 7468 6520 4465 6365 6e74 7269   to the Decentri
-00002280: 7120 706c 6174 666f 726d 2e0a 0a20 2020  q platform...   
-00002290: 202a 2a50 6172 616d 6574 6572 732a 2a3a   **Parameters**:
-000022a0: 0a20 2020 202d 2060 636f 6e74 656e 7460  .    - `content`
-000022b0: 3a20 5468 6520 7374 7269 6e67 2063 6f6e  : The string con
-000022c0: 7461 696e 696e 6720 7468 6520 4353 5620  taining the CSV 
-000022d0: 6669 6c65 2e0a 2020 2020 2d20 6068 6173  file..    - `has
-000022e0: 5f68 6561 6465 7260 3a20 5768 6574 6865  _header`: Whethe
-000022f0: 7220 7468 6520 7374 7269 6e67 2063 6f6e  r the string con
-00002300: 7461 696e 7320 6120 6865 6164 6572 2072  tains a header r
-00002310: 6f77 2e0a 2020 2020 2d20 6063 6865 636b  ow..    - `check
-00002320: 5f68 6561 6465 7260 3a20 5768 6574 6865  _header`: Whethe
-00002330: 7220 7468 6520 6675 6e63 7469 6f6e 2073  r the function s
-00002340: 686f 756c 6420 7472 7920 746f 2064 6574  hould try to det
-00002350: 6572 6d69 6e65 2077 6865 7468 6572 2074  ermine whether t
-00002360: 6865 2066 696c 6520 6861 7320 6120 6865  he file has a he
-00002370: 6164 6572 2e0a 2020 2020 2020 2020 4966  ader..        If
-00002380: 2074 6865 2066 696c 6520 6861 7320 6120   the file has a 
-00002390: 6865 6164 6572 2072 6f77 2062 7574 2079  header row but y
-000023a0: 6f75 2064 6964 6e27 7420 7365 7420 7468  ou didn't set th
-000023b0: 6520 6068 6173 5f68 6561 6465 7260 2066  e `has_header` f
-000023c0: 6c61 672c 2061 6e0a 2020 2020 2020 2020  lag, an.        
-000023d0: 6578 6365 7074 696f 6e20 7769 6c6c 2062  exception will b
-000023e0: 6520 7261 6973 6564 2e20 4966 2079 6f75  e raised. If you
-000023f0: 2772 6520 7375 7265 2074 6861 7420 7468  're sure that th
-00002400: 6520 7761 7920 796f 7520 7573 6520 7468  e way you use th
-00002410: 6520 6675 6e63 7469 6f6e 0a20 2020 2020  e function.     
-00002420: 2020 2069 7320 636f 7272 6563 742c 2079     is correct, y
-00002430: 6f75 2063 616e 2064 6973 6162 6c65 2074  ou can disable t
-00002440: 6869 7320 6368 6563 6b20 7573 696e 6720  his check using 
-00002450: 7468 6973 2070 6172 616d 6574 6572 2e0a  this parameter..
-00002460: 2020 2020 2d20 6065 6e63 6f64 696e 6760      - `encoding`
-00002470: 3a20 5468 6520 656e 636f 6469 6e67 206f  : The encoding o
-00002480: 6620 7468 6520 736f 7572 6365 2066 696c  f the source fil
-00002490: 652e 2049 6620 796f 7520 7772 6f74 6520  e. If you wrote 
-000024a0: 7468 6520 4353 5620 6669 6c65 2075 7369  the CSV file usi
-000024b0: 6e67 2061 206c 6962 7261 7279 206c 696b  ng a library lik
-000024c0: 6520 7061 6e64 6173 2c0a 2020 2020 2020  e pandas,.      
-000024d0: 2020 796f 7520 6e65 6564 2074 6f20 6368    you need to ch
-000024e0: 6563 6b20 7468 6520 646f 6375 6d65 6e74  eck the document
-000024f0: 6174 696f 6e20 746f 2073 6565 2077 6861  ation to see wha
-00002500: 7420 656e 636f 6469 6e67 2074 6865 7920  t encoding they 
-00002510: 7573 6520 6279 2064 6566 6175 6c74 0a20  use by default. 
-00002520: 2020 2020 2020 2077 6865 6e20 7772 6974         when writ
-00002530: 696e 6720 6669 6c65 732e 0a20 2020 202d  ing files..    -
-00002540: 2060 6465 6c69 6d69 7465 7260 3a20 5768   `delimiter`: Wh
-00002550: 6174 2064 656c 696d 6974 6572 2069 7320  at delimiter is 
-00002560: 7573 6564 2069 6e20 7468 6520 7468 6520  used in the the 
-00002570: 4353 5620 6669 6c65 2e20 4465 6661 756c  CSV file. Defaul
-00002580: 7420 6973 2074 6865 2063 6f6d 6d61 2e0a  t is the comma..
-00002590: 2020 2020 2d20 602a 2a6b 7761 7267 7360      - `**kwargs`
-000025a0: 3a20 4164 6469 7469 6f6e 616c 206b 6579  : Additional key
-000025b0: 776f 7264 2061 7267 756d 656e 7473 2070  word arguments p
-000025c0: 6173 7365 6420 746f 2074 6865 2050 7974  assed to the Pyt
-000025d0: 686f 6e20 4353 5620 7061 7273 6572 2e20  hon CSV parser. 
-000025e0: 5768 6174 2066 6c61 6773 2063 616e 2062  What flags can b
-000025f0: 6520 7061 7373 6564 2063 616e 2062 650a  e passed can be.
-00002600: 2020 2020 2020 2020 7365 656e 205b 6865          seen [he
-00002610: 7265 5d28 6874 7470 733a 2f2f 646f 6373  re](https://docs
-00002620: 2e70 7974 686f 6e2e 6f72 672f 332f 6c69  .python.org/3/li
-00002630: 6272 6172 792f 6373 762e 6874 6d6c 2363  brary/csv.html#c
-00002640: 7376 2d66 6d74 2d70 6172 616d 7329 2e0a  sv-fmt-params)..
-00002650: 0a20 2020 202a 2a52 6574 7572 6e73 2a2a  .    **Returns**
-00002660: 3a0a 2020 2020 4120 4279 7465 7349 4f20  :.    A BytesIO 
-00002670: 6f62 6a65 6374 2074 6861 7420 6361 6e20  object that can 
-00002680: 6265 2070 6173 7365 6420 746f 2074 6865  be passed to the
-00002690: 206d 6574 686f 6473 2072 6573 706f 7369   methods resposi
-000026a0: 626c 6520 666f 7220 7570 6c6f 6164 696e  ble for uploadin
-000026b0: 6720 6461 7461 2e0a 2020 2020 7246 0000  g data..    rF..
-000026c0: 0029 0472 4800 0000 da02 696f da08 5374  .).rH.....io..St
-000026d0: 7269 6e67 494f da05 7374 7269 7029 0472  ringIO..strip).r
-000026e0: 4c00 0000 7241 0000 0072 4200 0000 7249  L...rA...rB...rI
-000026f0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00002700: 0000 da15 7265 6164 5f69 6e70 7574 5f63  ....read_input_c
-00002710: 7376 5f73 7472 696e 67bf 0000 0073 1000  sv_string....s..
-00002720: 0000 001c 0201 0cff 0202 0201 02fd 0404  ................
-00002730: 02fc 7250 0000 0029 04da 0464 6174 6172  ..rP...)...datar
-00002740: 4100 0000 7242 0000 0072 3400 0000 6301  A...rB...r4...c.
-00002750: 0000 0001 0000 0002 0000 0009 0000 0006  ................
-00002760: 0000 000b 0000 0073 b200 0000 6700 7d04  .......s....g.}.
-00002770: 7c02 7266 6401 a000 8700 6601 6402 6403  |.rfd.....f.d.d.
-00002780: 8408 7401 6404 8301 4400 8301 a101 7d05  ..t.d...D.....}.
-00002790: 7402 a003 a100 a004 7c05 a101 7d06 7c06  t.......|...}.|.
-000027a0: 7248 7c01 6405 7500 7248 7405 6406 8301  rH|.d.u.rHt.d...
-000027b0: 8201 6e14 7c06 735c 7c01 6407 7500 725c  ..n.|.s\|.d.u.r\
-000027c0: 7405 6408 8301 8201 8800 a006 6409 a101  t.d.........d...
-000027d0: 0100 7402 6a07 8800 6601 6900 7c03 a401  ..t.j...f.i.|...
-000027e0: 8e01 7d07 7c01 7284 7408 7c07 8301 0100  ..}.|.r.t.|.....
-000027f0: 7c07 4400 5d14 7d08 7c04 a009 640a a000  |.D.].}.|...d...
-00002800: 7c08 a101 a101 0100 7188 740a a00b 6401  |.......q.t...d.
-00002810: a000 7c04 a101 a00c a100 a101 5300 290b  ..|.........S.).
-00002820: 4eda 010a 6301 0000 0000 0000 0000 0000  N...c...........
-00002830: 0002 0000 0003 0000 0033 0000 0073 1600  .........3...s..
-00002840: 0000 7c00 5d0e 7d01 8800 a000 a100 5600  ..|.].}.......V.
-00002850: 0100 7102 6400 5300 2901 4e29 01da 0872  ..q.d.S.).N)...r
-00002860: 6561 646c 696e 6529 02da 022e 30da 015f  eadline)....0.._
-00002870: a901 7251 0000 0072 1400 0000 7215 0000  ..rQ...r....r...
-00002880: 00da 093c 6765 6e65 7870 723e ec00 0000  ...<genexpr>....
-00002890: f300 0000 007a 225f 7265 6164 5f69 6e70  .....z"_read_inp
-000028a0: 7574 5f63 7376 2e3c 6c6f 6361 6c73 3e2e  ut_csv.<locals>.
-000028b0: 3c67 656e 6578 7072 3ee9 1400 0000 467a  <genexpr>.....Fz
-000028c0: 9a57 6172 6e69 6e67 3a20 7468 6520 6669  .Warning: the fi
-000028d0: 6c65 2073 6565 6d73 2074 6f20 6861 7665  le seems to have
-000028e0: 2061 2068 6561 6465 7220 6275 7420 7468   a header but th
-000028f0: 6520 6865 6164 6572 2066 6c61 6720 6973  e header flag is
-00002900: 206e 6f74 2073 6574 2074 6f20 7472 7565   not set to true
-00002910: 2120 5468 6973 2066 6c61 6720 6e65 6564  ! This flag need
-00002920: 7320 746f 2062 6520 7365 7420 636f 7272  s to be set corr
-00002930: 6563 746c 7920 696e 206f 7264 6572 2066  ectly in order f
-00002940: 6f72 2074 6865 2064 6174 6120 746f 2062  or the data to b
-00002950: 6520 7570 6c6f 6164 6564 2e54 7a95 5761  e uploaded.Tz.Wa
-00002960: 726e 696e 673a 2074 6865 2066 696c 6520  rning: the file 
-00002970: 646f 6573 6e27 7420 7365 656d 2074 6f20  doesn't seem to 
-00002980: 6861 7665 2061 2068 6561 6465 7220 6275  have a header bu
-00002990: 7420 7468 6520 6865 6164 6572 2066 6c61  t the header fla
-000029a0: 6720 6973 2073 6574 2120 5468 6973 2066  g is set! This f
-000029b0: 6c61 6720 6e65 6564 7320 746f 2062 6520  lag needs to be 
-000029c0: 7365 7420 636f 7272 6563 746c 7920 696e  set correctly in
-000029d0: 206f 7264 6572 2066 6f72 2074 6865 2064   order for the d
-000029e0: 6174 6120 746f 2062 6520 7570 6c6f 6164  ata to be upload
-000029f0: 6564 2e72 0100 0000 da01 2c29 0dda 046a  ed.r......,)...j
-00002a00: 6f69 6eda 0572 616e 6765 da03 6373 765a  oin..range..csvZ
-00002a10: 0753 6e69 6666 6572 7241 0000 00da 0945  .SnifferrA.....E
-00002a20: 7863 6570 7469 6f6e da04 7365 656b da06  xception..seek..
-00002a30: 7265 6164 6572 da04 6e65 7874 da06 6170  reader..next..ap
-00002a40: 7065 6e64 724d 0000 00da 0742 7974 6573  pendrM.....Bytes
-00002a50: 494f da06 656e 636f 6465 2909 7251 0000  IO..encode).rQ..
-00002a60: 0072 4100 0000 7242 0000 0072 4900 0000  .rA...rB...rI...
-00002a70: 724a 0000 00da 0673 616d 706c 655a 0f66  rJ.....sampleZ.f
-00002a80: 696c 655f 6861 735f 6865 6164 6572 7260  ile_has_headerr`
-00002a90: 0000 00da 0372 6f77 7214 0000 0072 5600  .....rowr....rV.
-00002aa0: 0000 7215 0000 0072 4800 0000 e300 0000  ..r....rH.......
-00002ab0: 7326 0000 0000 0704 0104 011c 010e 010c  s&..............
-00002ac0: 0102 0102 ff06 040c 0102 0102 ff04 040a  ................
-00002ad0: 0112 0104 0108 0108 0112 0172 4800 0000  ...........rH...
-00002ae0: da00 2902 da0b 6465 7363 7269 7074 696f  ..)...descriptio
-00002af0: 6eda 0876 616c 6964 6174 6529 0872 5100  n..validate).rQ.
-00002b00: 0000 da03 6b65 79da 0c64 6174 615f 726f  ....key..data_ro
-00002b10: 6f6d 5f69 64da 0574 6162 6c65 da07 7365  om_id..table..se
-00002b20: 7373 696f 6e72 6800 0000 7269 0000 0072  ssionrh...ri...r
-00002b30: 3400 0000 6303 0000 0000 0000 0004 0000  4...c...........
-00002b40: 000a 0000 000a 0000 004b 0000 0073 7e00  .........K...s~.
-00002b50: 0000 7c04 6a00 a001 7c00 7c01 7c03 a103  ..|.j...|.|.|...
-00002b60: 7d08 7c04 6a02 7c02 7c08 7403 7c03 8301  }.|.j.|.|.t.|...
-00002b70: 7c01 6401 8d04 0100 7c06 727a 7a1c 7c04  |.d.....|.rzz.|.
-00002b80: 6a04 7c02 7405 7c03 8301 6602 6900 7c07  j.|.t.|...f.i.|.
-00002b90: a401 8e01 0100 5700 6e32 0400 7406 7978  ......W.n2..t.yx
-00002ba0: 0100 7d09 0100 7a1a 7406 6402 a007 7c09  ..}...z.t.d...|.
-00002bb0: a101 8301 8201 5700 5900 6403 7d09 7e09  ......W.Y.d.}.~.
-00002bc0: 6e0a 6403 7d09 7e09 3000 3000 7c08 5300  n.d.}.~.0.0.|.S.
-00002bd0: 2904 618f 0400 000a 2020 2020 436f 6e76  ).a.....    Conv
-00002be0: 656e 6965 6e63 6520 6675 6e63 7469 6f6e  enience function
-00002bf0: 2066 6f72 2075 706c 6f61 6469 6e67 2064   for uploading d
-00002c00: 6174 6120 616e 6420 7661 6c69 6461 7469  ata and validati
-00002c10: 6e67 2074 6865 2073 6368 656d 6120 6f66  ng the schema of
-00002c20: 2074 6865 2075 706c 6f61 6465 640a 2020   the uploaded.  
-00002c30: 2020 6461 7461 2e0a 0a20 2020 2056 616c    data...    Val
-00002c40: 6964 6174 696f 6e20 6f66 2074 6162 756c  idation of tabul
-00002c50: 6172 2064 6174 6120 6973 2061 2073 6570  ar data is a sep
-00002c60: 6172 6174 6520 636f 6d70 7574 6174 696f  arate computatio
-00002c70: 6e20 666f 7220 7768 6963 6820 7370 6563  n for which spec
-00002c80: 6966 6963 2063 6f6d 7075 7465 206e 6f64  ific compute nod
-00002c90: 6573 0a20 2020 206e 6565 6420 746f 2062  es.    need to b
-00002ca0: 6520 7072 6573 656e 7420 696e 2074 6865  e present in the
-00002cb0: 2063 6f6d 7075 7465 2067 7261 7068 2064   compute graph d
-00002cc0: 6566 696e 6564 2062 7920 7468 6520 6461  efined by the da
-00002cd0: 7461 2072 6f6f 6d20 6465 6669 6e69 7469  ta room definiti
-00002ce0: 6f6e 2e0a 2020 2020 5468 6973 2066 756e  on..    This fun
-00002cf0: 6374 696f 6e20 7769 6c6c 2074 616b 6520  ction will take 
-00002d00: 6361 7265 206f 6620 7472 6967 6765 7269  care of triggeri
-00002d10: 6e67 2074 6865 2076 616c 6964 6174 696f  ng the validatio
-00002d20: 6e20 6163 7469 6f6e 2066 6f72 2079 6f75  n action for you
-00002d30: 2e0a 2020 2020 496e 2063 6173 6520 7661  ..    In case va
-00002d40: 6c69 6461 7469 6f6e 2066 6169 6c73 2c20  lidation fails, 
-00002d50: 616e 2065 7863 6570 7469 6f6e 2077 696c  an exception wil
-00002d60: 6c20 6265 2072 6169 7365 642e 2056 616c  l be raised. Val
-00002d70: 6964 6174 696f 6e20 6361 6e20 6265 2074  idation can be t
-00002d80: 7572 6e65 6420 6f66 660a 2020 2020 7573  urned off.    us
-00002d90: 696e 6720 7468 6520 6076 616c 6964 6174  ing the `validat
-00002da0: 6560 2070 6172 616d 6574 6572 2e0a 0a20  e` parameter... 
-00002db0: 2020 202a 2a50 6172 616d 6574 6572 732a     **Parameters*
-00002dc0: 2a3a 0a20 2020 202d 2060 6461 7461 603a  *:.    - `data`:
-00002dd0: 2054 6865 2069 6e70 7574 2064 6174 6120   The input data 
-00002de0: 746f 2062 6520 7570 6c6f 6164 6564 2e20  to be uploaded. 
-00002df0: 5573 6520 6f6e 6520 6f66 2074 6865 2072  Use one of the r
-00002e00: 6561 6465 7220 6675 6e63 7469 6f6e 7320  eader functions 
-00002e10: 7072 6f76 6964 6564 2069 6e20 7468 6973  provided in this
-00002e20: 0a20 2020 2020 2020 2070 6163 6b61 6765  .        package
-00002e30: 2074 6f20 7265 6164 2043 5356 2d6c 696b   to read CSV-lik
-00002e40: 6520 6461 7461 2e0a 2020 2020 2d20 606b  e data..    - `k
-00002e50: 6579 603a 2041 206b 6579 2066 6f72 2065  ey`: A key for e
-00002e60: 6e63 7279 7074 696e 6720 7468 6520 6461  ncrypting the da
-00002e70: 7461 2074 6f2d 6265 2d75 706c 6f61 6465  ta to-be-uploade
-00002e80: 642e 0a20 2020 202d 2060 6461 7461 5f72  d..    - `data_r
-00002e90: 6f6f 6d5f 6964 603a 2054 6f20 7768 6963  oom_id`: To whic
-00002ea0: 6820 6461 7461 2072 6f6f 6d20 7468 6520  h data room the 
-00002eb0: 6461 7461 7365 7420 7368 6f75 6c64 2062  dataset should b
-00002ec0: 6520 7075 626c 6973 6865 642e 2054 6869  e published. Thi
-00002ed0: 7320 6973 2074 6865 2069 6420 796f 750a  s is the id you.
-00002ee0: 2020 2020 2020 2020 6765 7420 7768 656e          get when
-00002ef0: 2070 7562 6c69 7368 696e 6720 6120 6461   publishing a da
-00002f00: 7461 2072 6f6f 6d2e 0a20 2020 202d 2060  ta room..    - `
-00002f10: 7461 626c 6560 3a20 5468 6520 6e61 6d65  table`: The name
-00002f20: 206f 6620 7468 6520 6461 7461 206e 6f64   of the data nod
-00002f30: 6520 6275 696c 6465 722e 0a20 2020 202d  e builder..    -
-00002f40: 2060 7365 7373 696f 6e60 3a20 5468 6520   `session`: The 
-00002f50: 7365 7373 696f 6e20 7769 7468 2077 6869  session with whi
-00002f60: 6368 2074 6f20 636f 6d6d 756e 6963 6174  ch to communicat
-00002f70: 6520 7769 7468 2074 6865 2065 6e63 6c61  e with the encla
-00002f80: 7665 2e0a 2020 2020 2d20 6064 6573 6372  ve..    - `descr
-00002f90: 6970 7469 6f6e 603a 2041 6e20 6f70 7469  iption`: An opti
-00002fa0: 6f6e 616c 2064 6573 6372 6970 7469 6f6e  onal description
-00002fb0: 206f 6620 7468 6520 6461 7461 7365 742e   of the dataset.
-00002fc0: 0a20 2020 202d 2060 7661 6c69 6461 7465  .    - `validate
-00002fd0: 603a 2057 6865 7468 6572 2074 6f20 7065  `: Whether to pe
-00002fe0: 7266 6f72 6d20 7468 6520 7661 6c69 6461  rform the valida
-00002ff0: 7469 6f6e 206f 7065 7261 7469 6f6e 2e0a  tion operation..
-00003000: 0a20 2020 202a 2a52 6574 7572 6e73 2a2a  .    **Returns**
-00003010: 3a0a 2020 2020 5468 6520 6d61 6e69 6665  :.    The manife
-00003020: 7374 2068 6173 6820 2864 6174 6173 6574  st hash (dataset
-00003030: 2069 6429 2069 6e20 6361 7365 2074 6865   id) in case the
-00003040: 2075 706c 6f61 6420 616e 6420 7661 6c69   upload and vali
-00003050: 6461 7469 6f6e 2073 7563 6365 6564 6564  dation succeeded
-00003060: 2e0a 2020 2020 2902 da09 6c65 6166 5f6e  ..    )...leaf_n
-00003070: 616d 6572 6a00 0000 7a28 5661 6c69 6461  amerj...z(Valida
-00003080: 7469 6f6e 206f 6620 6461 7461 7365 7420  tion of dataset 
-00003090: 6661 696c 6564 2120 5265 6173 6f6e 3a20  failed! Reason: 
-000030a0: 7b7d 4e29 08da 0663 6c69 656e 74da 0e75  {}N)...client..u
-000030b0: 706c 6f61 645f 6461 7461 7365 74da 0f70  pload_dataset..p
-000030c0: 7562 6c69 7368 5f64 6174 6173 6574 7216  ublish_datasetr.
-000030d0: 0000 00da 1f72 756e 5f63 6f6d 7075 7461  .....run_computa
-000030e0: 7469 6f6e 5f61 6e64 5f67 6574 5f72 6573  tion_and_get_res
-000030f0: 756c 7473 7217 0000 0072 5e00 0000 da06  ultsr....r^.....
-00003100: 666f 726d 6174 290a 7251 0000 0072 6a00  format).rQ...rj.
-00003110: 0000 726b 0000 0072 6c00 0000 726d 0000  ..rk...rl...rm..
-00003120: 0072 6800 0000 7269 0000 0072 4900 0000  .rh...ri...rI...
-00003130: da0d 6d61 6e69 6665 7374 5f68 6173 68da  ..manifest_hash.
-00003140: 0165 7214 0000 0072 1400 0000 7215 0000  .er....r....r...
-00003150: 00da 2275 706c 6f61 645f 616e 645f 7075  .."upload_and_pu
-00003160: 626c 6973 685f 7461 6275 6c61 725f 6461  blish_tabular_da
-00003170: 7461 7365 7401 0100 0073 2a00 0000 0023  taset....s*....#
-00003180: 0601 0201 0201 02fd 0405 0401 0401 0601  ................
-00003190: 02fd 0606 0401 0201 0401 0201 06fe 0403  ................
-000031a0: 02fd 0a05 0e01 2402 7276 0000 0029 02da  ......$.rv...)..
-000031b0: 0672 6573 756c 7472 3400 0000 6301 0000  .resultr4...c...
-000031c0: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-000031d0: 0043 0000 0073 6a00 0000 7400 a001 7402  .C...sj...t...t.
-000031e0: a003 7c00 a101 6401 a102 7d01 7404 7c01  ..|...d...}.t.|.
-000031f0: a005 a100 8301 6402 6403 6802 6b03 723e  ......d.d.h.k.r>
-00003200: 7406 6404 a007 6405 a008 7c01 a005 a100  t.d...d...|.....
-00003210: a101 a101 8301 8201 7c01 a009 6402 a101  ........|...d...
-00003220: a00a a100 7d02 740b 8300 7d03 740c 7c01  ....}.t...}.t.|.
-00003230: a009 6403 a101 7c03 8302 0100 7c02 7c03  ..d...|.....|.|.
-00003240: 6602 5300 2906 4e72 4500 0000 7a0b 6461  f.S.).NrE...z.da
-00003250: 7461 7365 742e 6373 76da 0574 7970 6573  taset.csv..types
-00003260: 7a89 5468 6520 6769 7665 6e20 7265 7375  z.The given resu
-00003270: 6c74 2063 616e 6e6f 7420 6265 2072 6561  lt cannot be rea
-00003280: 6420 6173 2069 7420 646f 6573 6e27 7420  d as it doesn't 
-00003290: 636f 6e74 6169 6e20 616c 6c20 7468 6520  contain all the 
-000032a0: 7265 7175 6972 6564 2066 696c 6573 2e20  required files. 
-000032b0: 4578 7065 6374 6564 2066 696c 6573 3a20  Expected files: 
-000032c0: 2764 6174 6173 6574 2e63 7376 2720 616e  'dataset.csv' an
-000032d0: 6420 2774 7970 6573 272c 206f 6e6c 7920  d 'types', only 
-000032e0: 666f 756e 643a 205b 7b7d 5d7a 022c 2029  found: [{}]z., )
-000032f0: 0dda 077a 6970 6669 6c65 da07 5a69 7046  ...zipfile..ZipF
-00003300: 696c 6572 4d00 0000 7263 0000 00da 0373  ilerM...rc.....s
-00003310: 6574 da08 6e61 6d65 6c69 7374 725e 0000  et..namelistr^..
-00003320: 0072 7300 0000 725b 0000 00da 0472 6561  .rs...r[.....rea
-00003330: 64da 0664 6563 6f64 6572 0d00 0000 7210  d..decoder....r.
-00003340: 0000 0029 0472 7700 0000 da07 6172 6368  ...).rw.....arch
-00003350: 6976 6572 5d00 0000 721c 0000 0072 1400  iver]...r....r..
-00003360: 0000 7214 0000 0072 1500 0000 da16 5f72  ..r....r......_r
-00003370: 6561 645f 7371 6c5f 7175 6572 795f 7265  ead_sql_query_re
-00003380: 7375 6c74 3c01 0000 7316 0000 0000 0112  sult<...s.......
-00003390: 0214 0102 0104 020c fe02 ff04 070e 0106  ................
-000033a0: 0110 0272 8000 0000 6301 0000 0000 0000  ...r....c.......
-000033b0: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
-000033c0: 0073 2800 0000 7400 7c00 8301 5c02 7d01  .s(...t.|...\.}.
-000033d0: 7d02 7401 a002 7403 a004 7c01 a101 a101  }.t...t...|.....
-000033e0: 7d03 7405 7c03 8301 7c02 6602 5300 2901  }.t.|...|.f.S.).
-000033f0: 618a 0100 000a 2020 2020 5265 6164 2074  a.....    Read t
-00003400: 6865 2067 6976 656e 2072 6177 2043 5356  he given raw CSV
-00003410: 206f 7574 7075 7420 6672 6f6d 2061 6e20   output from an 
-00003420: 5351 4c20 7175 6572 7920 7265 7375 6c74  SQL query result
-00003430: 2061 6e64 2074 7261 6e73 666f 726d 2069   and transform i
-00003440: 7420 696e 746f 2061 206c 6973 7420 6f66  t into a list of
-00003450: 0a20 2020 206c 6973 7473 2c20 7768 6572  .    lists, wher
-00003460: 6520 6561 6368 2069 6e6e 6572 206c 6973  e each inner lis
-00003470: 7420 636f 7272 6573 706f 6e64 7320 746f  t corresponds to
-00003480: 2061 2072 6f77 2069 6e20 7468 6520 7461   a row in the ta
-00003490: 6275 6c61 7220 6f75 7470 7574 2064 6174  bular output dat
-000034a0: 612e 0a20 2020 2054 6865 2068 6561 6465  a..    The heade
-000034b0: 7220 726f 7720 776f 6e27 7420 6265 2063  r row won't be c
-000034c0: 6f6e 7461 696e 6564 2069 6e20 7468 6520  ontained in the 
-000034d0: 7265 7375 6c74 696e 6720 6f75 7470 7574  resulting output
-000034e0: 2061 6e64 2061 6c6c 2074 6865 2069 6e6e   and all the inn
-000034f0: 6572 2076 616c 7565 730a 2020 2020 7769  er values.    wi
-00003500: 6c6c 2062 6520 6f66 2074 7970 6520 7374  ll be of type st
-00003510: 7269 6e67 2e0a 2020 2020 5468 6520 6163  ring..    The ac
-00003520: 7475 616c 2063 6f6c 756d 6e20 7479 7065  tual column type
-00003530: 7320 6173 2077 656c 6c20 6173 2074 6865  s as well as the
-00003540: 6972 206e 616d 6573 2077 696c 6c20 6265  ir names will be
-00003550: 2072 6574 7572 6e65 6420 6173 2070 6172   returned as par
-00003560: 7420 6f66 2074 6865 2073 6368 656d 610a  t of the schema.
-00003570: 2020 2020 7661 6c75 652e 0a20 2020 2029      value..    )
-00003580: 0672 8000 0000 725d 0000 0072 6000 0000  .r....r]...r`...
-00003590: 724d 0000 0072 4e00 0000 da04 6c69 7374  rM...rN.....list
-000035a0: 2904 7277 0000 005a 0b63 7376 5f63 6f6e  ).rw...Z.csv_con
-000035b0: 7465 6e74 721c 0000 0072 6000 0000 7214  tentr....r`...r.
-000035c0: 0000 0072 1400 0000 7215 0000 00da 1d72  ...r....r......r
-000035d0: 6561 645f 7371 6c5f 7175 6572 795f 7265  ead_sql_query_re
-000035e0: 7375 6c74 5f61 735f 6c69 7374 4e01 0000  sult_as_listN...
-000035f0: 7306 0000 0000 090c 0110 0172 8200 0000  s..........r....
-00003600: 2903 7277 0000 00da 0e69 6e63 6c75 6465  ).rw.....include
-00003610: 5f68 6561 6465 7272 3400 0000 6302 0000  _headerr4...c...
-00003620: 0000 0000 0000 0000 0008 0000 0005 0000  ................
-00003630: 0043 0000 0073 7000 0000 7400 7c00 8301  .C...sp...t.|...
-00003640: 5c02 7d02 7d03 7c01 7264 6401 6402 8400  \.}.}.|.rdd.d...
-00003650: 7c03 6a01 4400 8301 7d04 6403 6402 8400  |.j.D...}.d.d...
-00003660: 7402 6404 7403 7c04 8301 6404 1700 8302  t.d.t.|...d.....
-00003670: 4400 8301 7d05 6405 6402 8400 7404 7c04  D...}.d.d...t.|.
-00003680: 7c05 8302 4400 8301 7d06 6406 a005 7c06  |...D...}.d...|.
-00003690: a101 6407 1700 7c02 1700 7d07 6e04 7c02  ..d...|...}.n.|.
-000036a0: 7d07 7c07 a006 a100 5300 2908 61a3 0200  }.|.....S.).a...
-000036b0: 000a 2020 2020 5265 6164 2074 6865 2067  ..    Read the g
-000036c0: 6976 656e 2072 6177 2043 5356 206f 7574  iven raw CSV out
-000036d0: 7075 7420 6672 6f6d 2061 6e20 5351 4c20  put from an SQL 
-000036e0: 7175 6572 7920 7265 7375 6c74 2061 6e64  query result and
-000036f0: 2074 7261 6e73 666f 726d 2069 7420 696e   transform it in
-00003700: 746f 2061 2073 7472 696e 670a 2020 2020  to a string.    
-00003710: 636f 6e74 6169 6e69 6e67 2074 6865 2066  containing the f
-00003720: 756c 6c20 4353 5620 6669 6c65 2069 6e63  ull CSV file inc
-00003730: 6c75 6469 6e67 2074 6865 2068 6561 6465  luding the heade
-00003740: 7220 726f 772e 0a20 2020 2054 6865 2072  r row..    The r
-00003750: 6573 756c 7469 6e67 2073 7472 696e 6720  esulting string 
-00003760: 6361 6e20 6265 2077 7269 7474 656e 2064  can be written d
-00003770: 6972 6563 746c 7920 746f 2061 2066 696c  irectly to a fil
-00003780: 6520 6672 6f6d 2077 6865 7265 2069 7420  e from where it 
-00003790: 6361 6e20 6265 2072 6561 640a 2020 2020  can be read.    
-000037a0: 7573 696e 6720 796f 7572 2064 6174 6120  using your data 
-000037b0: 616e 616c 7973 6973 206c 6962 7261 7279  analysis library
-000037c0: 206f 6620 6368 6f69 6365 2e0a 0a20 2020   of choice...   
-000037d0: 202a 2a50 6172 616d 6574 6572 732a 2a3a   **Parameters**:
-000037e0: 0a20 2020 202d 2060 7265 7375 6c74 603a  .    - `result`:
-000037f0: 2054 6865 2072 6573 756c 7420 6672 6f6d   The result from
-00003800: 2077 6869 6368 2074 6f20 6578 7472 6163   which to extrac
-00003810: 7420 6120 4353 5620 6669 6c65 2061 7320  t a CSV file as 
-00003820: 6120 7374 7269 6e67 2e0a 2020 2020 2d20  a string..    - 
-00003830: 6069 6e63 6c75 6465 5f68 6561 6465 7260  `include_header`
-00003840: 3a20 5768 6574 6865 7220 746f 2069 6e63  : Whether to inc
-00003850: 6c75 6465 2061 6e20 6164 6469 7469 6f6e  lude an addition
-00003860: 616c 2068 6561 6465 7220 726f 7720 7468  al header row th
-00003870: 6174 2063 6f6e 7461 696e 730a 2020 2020  at contains.    
-00003880: 2020 2020 636f 6c75 6d6e 206e 616d 6573      column names
-00003890: 2028 7072 6f76 6964 6564 2066 6f72 2065   (provided for e
-000038a0: 7861 6d70 6c65 2062 7920 7573 696e 6720  xample by using 
-000038b0: 616c 6961 7320 6578 7072 6573 7369 6f6e  alias expression
-000038c0: 730a 2020 2020 2020 2020 696e 2053 454c  s.        in SEL
-000038d0: 4543 5420 7374 6174 656d 656e 7473 292e  ECT statements).
-000038e0: 2049 6620 7468 6973 2073 6574 7469 6e67   If this setting
-000038f0: 2069 7320 7472 7565 2c20 6275 7420 6e6f   is true, but no
-00003900: 2063 6f6c 756d 6e0a 2020 2020 2020 2020   column.        
-00003910: 6e61 6d65 7320 636f 756c 6420 6265 2066  names could be f
-00003920: 6f75 6e64 2c20 7468 6520 6e61 6d65 7320  ound, the names 
-00003930: 2256 3122 2c20 2256 3222 2061 6e64 2073  "V1", "V2" and s
-00003940: 6f20 7769 6c6c 2062 6520 7573 6564 2e0a  o will be used..
-00003950: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
-00003960: 0002 0000 0003 0000 0053 0000 0073 1200  .........S...s..
-00003970: 0000 6700 7c00 5d0a 7d01 7c01 6a00 9102  ..g.|.].}.|.j...
-00003980: 7104 5300 7214 0000 0029 0172 2400 0000  q.S.r....).r$...
-00003990: 2902 7254 0000 00da 0363 6f6c 7214 0000  ).rT.....colr...
-000039a0: 0072 1400 0000 7215 0000 00da 0a3c 6c69  .r....r......<li
-000039b0: 7374 636f 6d70 3e70 0100 0072 5800 0000  stcomp>p...rX...
-000039c0: 7a33 7265 6164 5f73 716c 5f71 7565 7279  z3read_sql_query
-000039d0: 5f72 6573 756c 745f 6173 5f73 7472 696e  _result_as_strin
-000039e0: 672e 3c6c 6f63 616c 733e 2e3c 6c69 7374  g.<locals>.<list
-000039f0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
-00003a00: 0000 0200 0000 0400 0000 5300 0000 7316  ..........S...s.
-00003a10: 0000 0067 007c 005d 0e7d 0164 007c 019b  ...g.|.].}.d.|..
-00003a20: 009d 0291 0271 0453 0029 01da 0156 7214  .....q.S.)...Vr.
-00003a30: 0000 0029 0272 5400 0000 5a02 6978 7214  ...).rT...Z.ixr.
-00003a40: 0000 0072 1400 0000 7215 0000 0072 8500  ...r....r....r..
-00003a50: 0000 7201 0000 7258 0000 0072 0500 0000  ..r...rX...r....
-00003a60: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00003a70: 0004 0000 0053 0000 0073 1c00 0000 6700  .....S...s....g.
-00003a80: 7c00 5d14 5c02 7d01 7d02 7c01 7214 7c01  |.].\.}.}.|.r.|.
-00003a90: 6e02 7c02 9102 7104 5300 7214 0000 0072  n.|...q.S.r....r
-00003aa0: 1400 0000 2903 7254 0000 00da 0263 31da  ....).rT.....c1.
-00003ab0: 0263 3272 1400 0000 7214 0000 0072 1500  .c2r....r....r..
-00003ac0: 0000 7285 0000 0073 0100 0072 5800 0000  ..r....s...rX...
-00003ad0: 725a 0000 0072 5200 0000 2907 7280 0000  rZ...rR...).r...
-00003ae0: 00da 0c6e 616d 6564 436f 6c75 6d6e 7372  ...namedColumnsr
-00003af0: 5c00 0000 da03 6c65 6eda 037a 6970 725b  \.....len..zipr[
-00003b00: 0000 0072 4f00 0000 2908 7277 0000 0072  ...rO...).rw...r
-00003b10: 8300 0000 724c 0000 0072 1c00 0000 5a0b  ....rL...r....Z.
-00003b20: 6f70 745f 636f 6c75 6d6e 735a 1372 6570  opt_columnsZ.rep
-00003b30: 6c61 6365 6d65 6e74 5f63 6f6c 756d 6e73  lacement_columns
-00003b40: 721e 0000 005a 1072 6574 7572 6e65 645f  r....Z.returned_
-00003b50: 636f 6e74 656e 7472 1400 0000 7214 0000  contentr....r...
-00003b60: 0072 1500 0000 da1f 7265 6164 5f73 716c  .r......read_sql
-00003b70: 5f71 7565 7279 5f72 6573 756c 745f 6173  _query_result_as
-00003b80: 5f73 7472 696e 675c 0100 0073 1000 0000  _string\...s....
-00003b90: 0011 0c02 0401 1002 1c01 1401 1402 0403  ................
-00003ba0: 728c 0000 0029 0154 2924 7279 0000 0072  r....).T)$ry...r
-00003bb0: 4d00 0000 725d 0000 00da 0674 7970 696e  M...r].....typin
-00003bc0: 6772 0200 0000 7203 0000 0072 0400 0000  gr....r....r....
-00003bd0: da07 636f 6d70 7574 6572 0600 0000 7267  ..computer....rg
-00003be0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00003bf0: 0000 720b 0000 0072 0c00 0000 da05 7072  ..r....r......pr
-00003c00: 6f74 6f72 0d00 0000 720e 0000 0072 0f00  otor....r....r..
-00003c10: 0000 5a16 7072 6f74 6f2e 6c65 6e67 7468  ..Z.proto.length
-00003c20: 5f64 656c 696d 6974 6564 7210 0000 0072  _delimitedr....r
-00003c30: 3e00 0000 7216 0000 0072 1700 0000 7218  >...r....r....r.
-00003c40: 0000 0072 3f00 0000 7263 0000 0072 4b00  ...r?...rc...rK.
-00003c50: 0000 7250 0000 00da 0a54 6578 7449 4f42  ..rP.....TextIOB
-00003c60: 6173 6572 4800 0000 7276 0000 00da 0562  aserH...rv.....b
-00003c70: 7974 6573 7280 0000 0072 8200 0000 728c  ytesr....r....r.
-00003c80: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
-00003c90: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00003ca0: 3e01 0000 0073 7400 0000 0801 0801 0801  >....st.........
-00003cb0: 1401 0c01 1801 0c01 0c01 1001 0c03 0e04  ................
-00003cc0: 0e04 0e7f 0006 0201 0201 02fb 0401 0202  ................
-00003cd0: 0201 0203 04f9 0c2b 0201 02fc 0401 0202  .......+........
-00003ce0: 0201 0202 04fa 0c27 0201 02fc 0401 0402  .......'........
-00003cf0: 0201 0202 04fa 0c25 0201 02f8 0401 0401  .......%........
-00003d00: 0201 0202 0201 0201 0201 0202 02f6 0c3b  ...............;
-00003d10: 1812 2010 00fe 0201 0201 0201 02fd       .. ...........
+00000000: 696d 706f 7274 207a 6970 6669 6c65 0a69  import zipfile.i
+00000010: 6d70 6f72 7420 696f 0a69 6d70 6f72 7420  mport io.import 
+00000020: 6373 760a 6672 6f6d 2074 7970 696e 6720  csv.from typing 
+00000030: 696d 706f 7274 204c 6973 742c 2054 7570  import List, Tup
+00000040: 6c65 2c20 416e 790a 6672 6f6d 202e 636f  le, Any.from .co
+00000050: 6d70 7574 6520 696d 706f 7274 2053 716c  mpute import Sql
+00000060: 5363 6865 6d61 5665 7269 6669 6572 0a66  SchemaVerifier.f
+00000070: 726f 6d20 2e2e 2069 6d70 6f72 7420 5065  rom .. import Pe
+00000080: 726d 6973 7369 6f6e 732c 2053 6573 7369  rmissions, Sessi
+00000090: 6f6e 2c20 4b65 792c 2044 6174 6152 6f6f  on, Key, DataRoo
+000000a0: 6d42 7569 6c64 6572 0a66 726f 6d20 2e2e  mBuilder.from ..
+000000b0: 636f 6d70 7574 6520 696d 706f 7274 204e  compute import N
+000000c0: 6f6f 700a 6672 6f6d 202e 7072 6f74 6f20  oop.from .proto 
+000000d0: 696d 706f 7274 2054 6162 6c65 5363 6865  import TableSche
+000000e0: 6d61 0a66 726f 6d20 2e2e 7072 6f74 6f20  ma.from ..proto 
+000000f0: 696d 706f 7274 2050 6572 6d69 7373 696f  import Permissio
+00000100: 6e2c 2041 7574 6865 6e74 6963 6174 696f  n, Authenticatio
+00000110: 6e4d 6574 686f 640a 6672 6f6d 202e 2e70  nMethod.from ..p
+00000120: 726f 746f 2e6c 656e 6774 685f 6465 6c69  roto.length_deli
+00000130: 6d69 7465 6420 696d 706f 7274 2070 6172  mited import par
+00000140: 7365 5f6c 656e 6774 685f 6465 6c69 6d69  se_length_delimi
+00000150: 7465 640a 0a0a 6465 6620 5f64 6174 615f  ted...def _data_
+00000160: 6e6f 6465 5f6e 616d 6528 6e6f 6465 3a20  node_name(node: 
+00000170: 7374 7229 3a0a 2020 2020 7265 7475 726e  str):.    return
+00000180: 2066 2240 7461 626c 652f 7b6e 6f64 657d   f"@table/{node}
+00000190: 2f64 6174 6173 6574 220a 0a0a 6465 6620  /dataset"...def 
+000001a0: 5f6e 6f6f 705f 6e6f 6465 5f6e 616d 6528  _noop_node_name(
+000001b0: 6e6f 6465 3a20 7374 7229 3a0a 2020 2020  node: str):.    
+000001c0: 7265 7475 726e 2066 2240 7461 626c 652f  return f"@table/
+000001d0: 7b6e 6f64 657d 2f76 616c 6964 6174 696f  {node}/validatio
+000001e0: 6e22 0a0a 0a63 6c61 7373 2054 6162 756c  n"...class Tabul
+000001f0: 6172 4461 7461 4e6f 6465 4275 696c 6465  arDataNodeBuilde
+00000200: 723a 0a20 2020 2022 2222 0a20 2020 2048  r:.    """.    H
+00000210: 656c 7065 7220 636c 6173 7320 746f 2063  elper class to c
+00000220: 6f6e 7374 7275 6374 2074 6865 2074 7269  onstruct the tri
+00000230: 706c 6574 206f 6620 6e6f 6465 7320 636f  plet of nodes co
+00000240: 6e73 6973 7469 6e67 206f 6620 6120 6461  nsisting of a da
+00000250: 7461 206e 6f64 6520 746f 0a20 2020 2073  ta node to.    s
+00000260: 746f 7265 2074 6162 756c 6172 2069 6e70  tore tabular inp
+00000270: 7574 2064 6174 612c 2061 7320 7765 6c6c  ut data, as well
+00000280: 2061 7320 6120 7363 6865 6d61 2076 616c   as a schema val
+00000290: 6964 6174 696f 6e20 636f 6d70 7574 6174  idation computat
+000002a0: 696f 6e2e 0a0a 2020 2020 496e 2061 2064  ion...    In a d
+000002b0: 6174 6120 636c 6561 6e20 726f 6f6d 2063  ata clean room c
+000002c0: 6f6d 7075 7461 7469 6f6e 7320 616e 6420  omputations and 
+000002d0: 7468 6520 6461 7461 2074 6865 7920 6465  the data they de
+000002e0: 7065 6e64 206f 6e20 6172 6520 6578 7072  pend on are expr
+000002f0: 6573 7365 6420 696e 2074 6572 6d73 0a20  essed in terms. 
+00000300: 2020 206f 6620 6772 6170 6873 2077 6865     of graphs whe
+00000310: 7265 2063 6f6d 7075 7461 7469 6f6e 7320  re computations 
+00000320: 6172 6520 7265 7072 6573 656e 7465 6420  are represented 
+00000330: 6279 202a 636f 6d70 7574 6520 6e6f 6465  by *compute node
+00000340: 732a 2061 6e64 2069 6e70 7574 2064 6174  s* and input dat
+00000350: 6173 6574 7320 6172 650a 2020 2020 7265  asets are.    re
+00000360: 7072 6573 656e 7465 6420 6279 202a 6461  presented by *da
+00000370: 7461 206e 6f64 6573 2a2e 0a20 2020 2057  ta nodes*..    W
+00000380: 6974 6820 7461 6275 6c61 7220 696e 7075  ith tabular inpu
+00000390: 7420 6461 7461 2c20 6974 2069 7320 706f  t data, it is po
+000003a0: 7373 6962 6c65 2074 6f20 7661 6c69 6461  ssible to valida
+000003b0: 7465 2074 6865 2069 6e70 7574 2064 6174  te the input dat
+000003c0: 6120 616e 6420 6368 6563 6b20 7768 6574  a and check whet
+000003d0: 6865 7220 6974 0a20 2020 2063 6f72 7265  her it.    corre
+000003e0: 7370 6f6e 6473 2074 6f20 6120 7072 652d  sponds to a pre-
+000003f0: 6465 6669 6e65 6420 7363 6865 6d61 2e20  defined schema. 
+00000400: 5468 6973 2076 616c 6964 6174 696f 6e20  This validation 
+00000410: 6973 2061 2063 6f6d 7075 7461 7469 6f6e  is a computation
+00000420: 2069 6e20 6974 7365 6c66 2073 6f20 696e   in itself so in
+00000430: 0a20 2020 206f 7264 6572 2074 6f20 7661  .    order to va
+00000440: 6c69 6461 7465 2074 6865 2069 6e70 7574  lidate the input
+00000450: 2064 6174 612c 2077 6520 6e65 6564 2074   data, we need t
+00000460: 6f20 6164 6420 616e 2061 6464 6974 696f  o add an additio
+00000470: 6e61 6c20 636f 6d70 7574 6520 6e6f 6465  nal compute node
+00000480: 206f 6e20 746f 7020 6f66 2074 6865 0a20   on top of the. 
+00000490: 2020 2064 6174 6120 6e6f 6465 2e20 4265     data node. Be
+000004a0: 6361 7573 6520 6974 206d 7573 7420 6265  cause it must be
+000004b0: 2070 6f73 7369 626c 6520 746f 2074 7269   possible to tri
+000004c0: 6767 6572 2074 6869 7320 7661 6c69 6461  gger this valida
+000004d0: 7469 6f6e 202a 7768 696c 6520 7265 7374  tion *while rest
+000004e0: 7269 6374 696e 6720 6163 6365 7373 0a20  ricting access. 
+000004f0: 2020 2074 6f20 7468 6520 7265 7375 6c74     to the result
+00000500: 696e 6720 6461 7461 2a2c 2061 6e6f 7468  ing data*, anoth
+00000510: 6572 2073 7065 6369 616c 206e 6f64 652c  er special node,
+00000520: 2074 6865 202a 6e6f 6f70 206e 6f64 652a   the *noop node*
+00000530: 206e 6565 6473 2074 6f20 6265 2061 6464   needs to be add
+00000540: 6564 2e0a 0a20 2020 2054 6869 7320 636c  ed...    This cl
+00000550: 6173 7320 7769 6c6c 2061 6464 2074 6865  ass will add the
+00000560: 206e 6563 6573 7361 7279 206e 6f64 6573   necessary nodes
+00000570: 2074 6f20 796f 7572 2064 6174 6120 636c   to your data cl
+00000580: 6561 6e20 726f 6f6d 2e0a 0a20 2020 2041  ean room...    A
+00000590: 6674 6572 2068 6176 696e 6720 636f 6e73  fter having cons
+000005a0: 7472 7563 7465 6420 616e 206f 626a 6563  tructed an objec
+000005b0: 7420 6f66 2074 6869 7320 636c 6173 732c  t of this class,
+000005c0: 2063 616c 6c20 6974 7320 6061 6464 5f74   call its `add_t
+000005d0: 6f5f 6275 696c 6465 7260 206d 6574 686f  o_builder` metho
+000005e0: 640a 2020 2020 616e 6420 7061 7373 2069  d.    and pass i
+000005f0: 7420 6120 6044 6174 6152 6f6f 6d42 7569  t a `DataRoomBui
+00000600: 6c64 6572 6020 696e 7374 616e 6365 2e20  lder` instance. 
+00000610: 5468 6973 2077 696c 6c20 6164 6420 7468  This will add th
+00000620: 6520 6e65 6365 7373 6172 7920 6e6f 6465  e necessary node
+00000630: 7320 616e 6420 7265 7175 6972 6564 0a20  s and required. 
+00000640: 2020 2075 7365 7220 7065 726d 6973 7369     user permissi
+00000650: 6f6e 7320 746f 2074 6865 2062 7569 6c64  ons to the build
+00000660: 6572 2069 6e73 7461 6e63 652e 0a0a 2020  er instance...  
+00000670: 2020 4461 7461 2073 686f 756c 6420 6265    Data should be
+00000680: 2070 7562 6c69 7368 6564 2074 6f20 7468   published to th
+00000690: 6520 6e6f 6465 206e 616d 6564 2060 696e  e node named `in
+000006a0: 7075 745f 6e6f 6465 5f6e 616d 6560 2061  put_node_name` a
+000006b0: 6e64 2062 6520 7265 6164 2066 726f 6d20  nd be read from 
+000006c0: 606f 7574 7075 745f 6e6f 6465 5f6e 616d  `output_node_nam
+000006d0: 6560 2e0a 2020 2020 5468 6520 6e61 6d65  e`..    The name
+000006e0: 206f 6620 7468 6520 7661 6c69 6461 7469   of the validati
+000006f0: 6f6e 2063 6f6d 7075 7461 7469 6f6e 2063  on computation c
+00000700: 616e 2062 6520 6163 6365 7373 6564 2075  an be accessed u
+00000710: 7369 6e67 2074 6865 2066 6965 6c64 2060  sing the field `
+00000720: 7661 6c69 6461 7469 6f6e 5f63 6f6d 7075  validation_compu
+00000730: 7461 7469 6f6e 5f6e 616d 6560 2e0a 0a20  tation_name`... 
+00000740: 2020 2054 6869 7320 636c 6173 7320 7573     This class us
+00000750: 6573 2061 2073 7065 6369 616c 206e 616d  es a special nam
+00000760: 696e 6720 636f 6e76 656e 7469 6f6e 2074  ing convention t
+00000770: 6f20 6e61 6d65 2074 6865 206e 6f64 6573  o name the nodes
+00000780: 2061 6464 6564 2074 6f20 7468 6520 6461   added to the da
+00000790: 7461 2072 6f6f 6d20 6261 7365 6420 6f6e  ta room based on
+000007a0: 0a20 2020 2074 6865 2074 6162 6c65 206e  .    the table n
+000007b0: 616d 6520 6769 7665 6e20 746f 2074 6865  ame given to the
+000007c0: 2062 7569 6c64 6572 2e20 4173 7375 6d69   builder. Assumi
+000007d0: 6e67 2079 6f75 2075 7365 2060 226d 795f  ng you use `"my_
+000007e0: 7461 626c 6522 6020 6173 2074 6865 2060  table"` as the `
+000007f0: 7461 626c 655f 6e61 6d65 6020 7768 656e  table_name` when
+00000800: 0a20 2020 2069 6e73 7461 6e74 6961 7469  .    instantiati
+00000810: 6e67 2074 6865 2060 5461 6275 6c61 7244  ng the `TabularD
+00000820: 6174 614e 6f64 6542 7569 6c64 6572 602c  ataNodeBuilder`,
+00000830: 2074 6865 6e20 7468 6520 666f 6c6c 6f77   then the follow
+00000840: 696e 6720 7468 7265 6520 6e6f 6465 7320  ing three nodes 
+00000850: 7769 6c6c 2062 6520 6164 6465 643a 0a0a  will be added:..
+00000860: 2020 2020 312e 2060 4074 6162 6c65 2f6d      1. `@table/m
+00000870: 795f 7461 626c 652f 6461 7461 7365 7460  y_table/dataset`
+00000880: 202d 2074 6865 2064 6174 6120 6e6f 6465   - the data node
+00000890: 2074 6f20 7768 6963 6820 796f 7520 6361   to which you ca
+000008a0: 6e20 7570 6c6f 6164 2064 6174 612e 0a20  n upload data.. 
+000008b0: 2020 2032 2e20 606d 795f 7461 626c 6560     2. `my_table`
+000008c0: 202d 2074 6865 206e 616d 6520 6f66 2074   - the name of t
+000008d0: 6865 2063 6f6d 7075 7465 206e 6f64 6520  he compute node 
+000008e0: 7468 6174 2076 6572 6966 6965 7320 7468  that verifies th
+000008f0: 6520 7363 6865 6d61 206f 6620 7468 6520  e schema of the 
+00000900: 6461 7461 2e0a 2020 2020 2020 2020 5375  data..        Su
+00000910: 6273 6571 7565 6e74 2053 514c 2063 6f6d  bsequent SQL com
+00000920: 7075 7465 206e 6f64 6573 2073 686f 756c  pute nodes shoul
+00000930: 6420 7265 6164 2064 6174 6120 6672 6f6d  d read data from
+00000940: 2074 6869 7320 6e6f 6465 2e0a 2020 2020   this node..    
+00000950: 332e 2060 4074 6162 6c65 2f6d 795f 7461  3. `@table/my_ta
+00000960: 626c 652f 7661 6c69 6461 7469 6f6e 6020  ble/validation` 
+00000970: 2d20 7468 6520 6e61 6d65 206f 6620 6120  - the name of a 
+00000980: 7370 6563 6961 6c20 7472 6967 6765 7220  special trigger 
+00000990: 6e6f 6465 2074 6861 7420 6361 6e20 6265  node that can be
+000009a0: 2075 7365 6420 746f 2074 7269 6767 6572   used to trigger
+000009b0: 2074 6865 2076 616c 6964 6174 696f 6e20   the validation 
+000009c0: 636f 6d70 7574 6174 696f 6e2e 0a0a 2020  computation...  
+000009d0: 2020 5468 6520 6865 6c70 6572 2066 756e    The helper fun
+000009e0: 6374 696f 6e20 6075 706c 6f61 645f 616e  ction `upload_an
+000009f0: 645f 7075 626c 6973 685f 7461 6275 6c61  d_publish_tabula
+00000a00: 725f 6461 7461 7365 7460 2077 696c 6c20  r_dataset` will 
+00000a10: 7570 6c6f 6164 2c20 7075 626c 6973 682c  upload, publish,
+00000a20: 2061 6e64 2076 616c 6964 6174 6520 796f   and validate yo
+00000a30: 7572 0a20 2020 2064 6174 6120 6175 746f  ur.    data auto
+00000a40: 6d61 7469 6361 6c6c 792c 2077 6974 686f  matically, witho
+00000a50: 7574 2079 6f75 2068 6176 696e 6720 746f  ut you having to
+00000a60: 2077 6f72 7279 2061 626f 7574 2069 6e74   worry about int
+00000a70: 6572 6e61 6c20 6e61 6d69 6e67 2e0a 2020  ernal naming..  
+00000a80: 2020 2222 220a 2020 2020 6465 6620 5f5f    """.    def __
+00000a90: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+00000aa0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00000ab0: 2020 2020 2020 7461 626c 655f 6e61 6d65        table_name
+00000ac0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
+00000ad0: 2020 2073 6368 656d 613a 204c 6973 745b     schema: List[
+00000ae0: 5475 706c 655b 7374 722c 2041 6e79 2c20  Tuple[str, Any, 
+00000af0: 626f 6f6c 5d5d 2c0a 2020 2020 2020 2020  bool]],.        
+00000b00: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
+00000b10: 2020 2069 735f 7265 7175 6972 6564 3a20     is_required: 
+00000b20: 626f 6f6c 203d 2046 616c 7365 0a20 2020  bool = False.   
+00000b30: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00000b40: 2222 220a 2020 2020 2020 2020 4372 6561  """.        Crea
+00000b50: 7465 2061 2060 5461 6275 6c61 7244 6174  te a `TabularDat
+00000b60: 614e 6f64 6542 7569 6c64 6572 602e 0a0a  aNodeBuilder`...
+00000b70: 2020 2020 2020 2020 2a2a 5061 7261 6d65          **Parame
+00000b80: 7465 7273 2a2a 3a0a 2020 2020 2020 2020  ters**:.        
+00000b90: 2d20 6074 6162 6c65 5f6e 616d 6560 3a20  - `table_name`: 
+00000ba0: 5768 6174 2079 6f75 7220 6461 7461 7365  What your datase
+00000bb0: 7420 7368 6f75 6c64 2062 6520 6361 6c6c  t should be call
+00000bc0: 6564 2e20 5468 6973 2069 7320 7468 6520  ed. This is the 
+00000bd0: 6e61 6d65 2079 6f75 2077 696c 6c20 6c61  name you will la
+00000be0: 7465 7220 7573 6520 696e 0a20 2020 2020  ter use in.     
+00000bf0: 2020 2020 2020 2079 6f75 7220 5351 4c20         your SQL 
+00000c00: 7175 6572 6965 732e 0a20 2020 2020 2020  queries..       
+00000c10: 202d 2060 7363 6865 6d61 603a 2054 6865   - `schema`: The
+00000c20: 206c 6973 7420 6f66 2063 6f6c 756d 6e73   list of columns
+00000c30: 2e20 5468 6973 2069 7320 6120 6c69 7374  . This is a list
+00000c40: 206f 6620 7475 706c 6573 2c20 6561 6368   of tuples, each
+00000c50: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00000c60: 6e61 6d65 206f 6620 7468 6520 636f 6c75  name of the colu
+00000c70: 6d6e 2c0a 2020 2020 2020 2020 2020 2020  mn,.            
+00000c80: 7468 6520 6461 7461 2074 7970 6520 2860  the data type (`
+00000c90: 6465 6365 6e74 7269 715f 706c 6174 666f  decentriq_platfo
+00000ca0: 726d 2e73 716c 2e70 726f 746f 2e50 7269  rm.sql.proto.Pri
+00000cb0: 6d69 7469 7665 5479 7065 6029 2c20 616e  mitiveType`), an
+00000cc0: 6420 7768 6574 6865 7220 7468 6520 636f  d whether the co
+00000cd0: 6c75 6d6e 2069 7320 6e75 6c6c 6162 6c65  lumn is nullable
+00000ce0: 2028 6361 6e20 6861 7665 2065 6d70 7479   (can have empty
+00000cf0: 2076 616c 7565 7329 2e0a 2020 2020 2020   values)..      
+00000d00: 2020 2020 2020 5468 6520 6461 7461 2074        The data t
+00000d10: 7970 6520 6973 2061 6e20 656e 756d 206c  ype is an enum l
+00000d20: 696b 6520 6f62 6a65 6374 2077 6974 6820  ike object with 
+00000d30: 7661 6c75 6573 2060 5072 696d 6974 6976  values `Primitiv
+00000d40: 6554 7970 652e 5354 5249 4e47 602c 2060  eType.STRING`, `
+00000d50: 5072 696d 6974 6976 6554 7970 652e 494e  PrimitiveType.IN
+00000d60: 5436 3460 2c0a 2020 2020 2020 2020 2020  T64`,.          
+00000d70: 2020 6050 7269 6d69 7469 7665 5479 7065    `PrimitiveType
+00000d80: 2e46 4c4f 4154 3634 602e 0a20 2020 2020  .FLOAT64`..     
+00000d90: 2020 202d 2060 6973 5f72 6571 7569 7265     - `is_require
+00000da0: 6460 3a20 5768 6574 6865 7220 7468 6520  d`: Whether the 
+00000db0: 6461 7461 7365 7420 6e65 6564 7320 746f  dataset needs to
+00000dc0: 2062 6520 7072 6573 656e 7420 666f 7220   be present for 
+00000dd0: 636f 6d70 7574 6174 696f 6e73 2074 6f20  computations to 
+00000de0: 6265 2074 7269 6767 6572 6564 2e0a 2020  be triggered..  
+00000df0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000e00: 2020 7365 6c66 2e74 6162 6c65 5f6e 616d    self.table_nam
+00000e10: 6520 3d20 7461 626c 655f 6e61 6d65 0a20  e = table_name. 
+00000e20: 2020 2020 2020 2073 656c 662e 6973 5f72         self.is_r
+00000e30: 6571 7569 7265 6420 3d20 6973 5f72 6571  equired = is_req
+00000e40: 7569 7265 640a 2020 2020 2020 2020 7365  uired.        se
+00000e50: 6c66 2e5f 6c65 6166 5f6e 6f64 655f 6e61  lf._leaf_node_na
+00000e60: 6d65 203d 205f 6461 7461 5f6e 6f64 655f  me = _data_node_
+00000e70: 6e61 6d65 2874 6162 6c65 5f6e 616d 6529  name(table_name)
+00000e80: 0a20 2020 2020 2020 2073 656c 662e 5f76  .        self._v
+00000e90: 6572 6966 6965 725f 6e6f 6465 5f6e 616d  erifier_node_nam
+00000ea0: 6520 3d20 7461 626c 655f 6e61 6d65 0a0a  e = table_name..
+00000eb0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00000ec0: 6964 6174 696f 6e5f 636f 6d70 7574 6174  idation_computat
+00000ed0: 696f 6e5f 6e61 6d65 203d 205f 6e6f 6f70  ion_name = _noop
+00000ee0: 5f6e 6f64 655f 6e61 6d65 2874 6162 6c65  _node_name(table
+00000ef0: 5f6e 616d 6529 0a20 2020 2020 2020 2022  _name).        "
+00000f00: 2222 5468 6520 6e61 6d65 206f 6620 7468  ""The name of th
+00000f10: 6520 636f 6d70 7574 6174 696f 6e20 7468  e computation th
+00000f20: 6174 2077 696c 6c20 7065 7266 6f72 6d20  at will perform 
+00000f30: 7468 6520 6461 7461 2076 616c 6964 6174  the data validat
+00000f40: 696f 6e2e 2222 220a 0a20 2020 2020 2020  ion."""..       
+00000f50: 2073 656c 662e 5f76 6572 6966 6965 7220   self._verifier 
+00000f60: 3d20 5371 6c53 6368 656d 6156 6572 6966  = SqlSchemaVerif
+00000f70: 6965 7228 0a20 2020 2020 2020 2020 2020  ier(.           
+00000f80: 2073 656c 662e 5f76 6572 6966 6965 725f   self._verifier_
+00000f90: 6e6f 6465 5f6e 616d 652c 0a20 2020 2020  node_name,.     
+00000fa0: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+00000fb0: 615f 6e6f 6465 3d73 656c 662e 5f6c 6561  a_node=self._lea
+00000fc0: 665f 6e6f 6465 5f6e 616d 652c 0a20 2020  f_node_name,.   
+00000fd0: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+00000fe0: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+00000ff0: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00001000: 2e5f 6e6f 6f70 203d 204e 6f6f 7028 7365  ._noop = Noop(se
+00001010: 6c66 2e76 616c 6964 6174 696f 6e5f 636f  lf.validation_co
+00001020: 6d70 7574 6174 696f 6e5f 6e61 6d65 2c20  mputation_name, 
+00001030: 6465 7065 6e64 656e 6369 6573 3d5b 7365  dependencies=[se
+00001040: 6c66 2e5f 7665 7269 6669 6572 2e6e 616d  lf._verifier.nam
+00001050: 655d 290a 0a20 2020 2064 6566 2061 6464  e])..    def add
+00001060: 5f74 6f5f 6275 696c 6465 7228 0a20 2020  _to_builder(.   
+00001070: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00001080: 2020 2020 2020 2020 2020 2062 7569 6c64             build
+00001090: 6572 3a20 4461 7461 526f 6f6d 4275 696c  er: DataRoomBuil
+000010a0: 6465 722c 0a20 2020 2020 2020 2020 2020  der,.           
+000010b0: 2061 7574 6865 6e74 6963 6174 696f 6e3a   authentication:
+000010c0: 2041 7574 6865 6e74 6963 6174 696f 6e4d   AuthenticationM
+000010d0: 6574 686f 642c 0a20 2020 2020 2020 2020  ethod,.         
+000010e0: 2020 2075 7365 7273 3a20 4c69 7374 5b73     users: List[s
+000010f0: 7472 5d0a 2020 2020 293a 0a20 2020 2020  tr].    ):.     
+00001100: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00001110: 6f6e 6669 6775 7265 2074 6865 2067 6976  onfigure the giv
+00001120: 656e 2060 4461 7461 526f 6f6d 4275 696c  en `DataRoomBuil
+00001130: 6465 7260 2074 6f20 6275 696c 6420 7465  der` to build te
+00001140: 2066 696e 616c 2064 6174 6120 636c 6561   final data clea
+00001150: 6e20 726f 6f6d 2077 6974 6820 7468 650a  n room with the.
+00001160: 2020 2020 2020 2020 6e65 6365 7373 6172          necessar
+00001170: 7920 636f 6d70 7574 6520 616e 6420 6461  y compute and da
+00001180: 7461 206e 6f64 6573 2e0a 2020 2020 2020  ta nodes..      
+00001190: 2020 5468 6973 2063 616c 6c20 7769 6c6c    This call will
+000011a0: 2061 6c73 6f20 6164 6420 7468 6520 6e65   also add the ne
+000011b0: 6365 7373 6172 7920 7065 726d 6973 7369  cessary permissi
+000011c0: 6f6e 7320 746f 2074 6865 2064 6174 6120  ons to the data 
+000011d0: 726f 6f6d 0a20 2020 2020 2020 2062 7569  room.        bui
+000011e0: 6c64 6572 2074 6861 7420 6c65 7420 6561  lder that let ea
+000011f0: 6368 2075 7365 7220 696e 2074 6865 206c  ch user in the l
+00001200: 6973 7420 6f66 2075 7365 7273 2070 6572  ist of users per
+00001210: 666f 726d 2074 6865 2066 6f6c 6c6f 7769  form the followi
+00001220: 6e67 0a20 2020 2020 2020 2074 6173 6b73  ng.        tasks
+00001230: 3a0a 0a20 2020 2020 2020 2031 2e20 5570  :..        1. Up
+00001240: 6c6f 6164 2064 6174 6120 746f 2074 6865  load data to the
+00001250: 2064 6174 6120 6e6f 6465 2e0a 2020 2020   data node..    
+00001260: 2020 2020 322e 2055 7365 2074 6865 2064      2. Use the d
+00001270: 6174 6120 696e 2064 6f77 6e73 7472 6561  ata in downstrea
+00001280: 6d20 636f 6d70 7574 6174 696f 6e73 2077  m computations w
+00001290: 6869 6c65 206d 616b 696e 6720 7375 7265  hile making sure
+000012a0: 0a20 2020 2020 2020 2020 2020 7468 6520  .           the 
+000012b0: 7363 6865 6d61 2069 7320 7661 6c69 642e  schema is valid.
+000012c0: 0a20 2020 2020 2020 2033 2e20 5472 6967  .        3. Trig
+000012d0: 6765 7220 7468 6520 7363 6865 6d61 2076  ger the schema v
+000012e0: 616c 6964 6174 696f 6e20 7374 6570 2073  alidation step s
+000012f0: 6570 6172 6174 656c 7920 6173 2069 7473  eparately as its
+00001300: 206f 776e 2063 6f6d 7075 7461 7469 6f6e   own computation
+00001310: 2e0a 0a20 2020 2020 2020 202a 2a50 6172  ...        **Par
+00001320: 616d 6574 6572 732a 2a3a 0a20 2020 2020  ameters**:.     
+00001330: 2020 202d 2060 6275 696c 6465 7260 3a20     - `builder`: 
+00001340: 5468 6520 6275 696c 6465 7220 6f62 6a65  The builder obje
+00001350: 6374 2074 6f20 7768 6963 6820 746f 2061  ct to which to a
+00001360: 6464 2074 6865 2064 6174 6120 616e 6420  dd the data and 
+00001370: 636f 6d70 7574 6520 6173 2077 656c 6c20  compute as well 
+00001380: 6173 0a20 2020 2020 2020 2020 2020 2074  as.            t
+00001390: 6865 2070 6572 6d69 7373 696f 6e73 2e0a  he permissions..
+000013a0: 2020 2020 2020 2020 2d20 6061 7574 6865          - `authe
+000013b0: 6e74 6963 6174 696f 6e60 3a20 5468 6520  ntication`: The 
+000013c0: 6175 7468 656e 7469 6361 7469 6f6e 206d  authentication m
+000013d0: 6574 686f 6420 7573 6564 2074 6f20 6175  ethod used to au
+000013e0: 7468 656e 7469 6361 7465 2074 6865 2075  thenticate the u
+000013f0: 7365 7273 0a20 2020 2020 2020 2020 2020  sers.           
+00001400: 2066 726f 6d20 7769 7468 696e 2074 6865   from within the
+00001410: 2065 6e63 6c61 7665 2e0a 2020 2020 2020   enclave..      
+00001420: 2020 2d20 6075 7365 7273 603a 2041 206c    - `users`: A l
+00001430: 6973 7420 6f66 2065 6d61 696c 2061 6464  ist of email add
+00001440: 7265 7373 6573 2074 6861 7420 7769 6c6c  resses that will
+00001450: 2062 6520 6769 7665 6e20 7065 726d 6973   be given permis
+00001460: 7369 6f6e 7320 626f 7468 2066 6f72 0a20  sions both for. 
+00001470: 2020 2020 2020 2020 2020 2074 6865 2076             the v
+00001480: 616c 6964 6174 696f 6e20 6f66 2074 6865  alidation of the
+00001490: 2064 6174 6120 6173 2077 656c 6c20 6173   data as well as
+000014a0: 2074 6865 2075 706c 6f61 6469 6e67 206f   the uploading o
+000014b0: 6620 6461 7461 2e0a 2020 2020 2020 2020  f data..        
+000014c0: 2222 220a 2020 2020 2020 2020 6275 696c  """.        buil
+000014d0: 6465 722e 6164 645f 6461 7461 5f6e 6f64  der.add_data_nod
+000014e0: 6528 7365 6c66 2e5f 6c65 6166 5f6e 6f64  e(self._leaf_nod
+000014f0: 655f 6e61 6d65 2c20 6973 5f72 6571 7569  e_name, is_requi
+00001500: 7265 643d 7365 6c66 2e69 735f 7265 7175  red=self.is_requ
+00001510: 6972 6564 290a 2020 2020 2020 2020 6275  ired).        bu
+00001520: 696c 6465 722e 6164 645f 636f 6d70 7574  ilder.add_comput
+00001530: 655f 6e6f 6465 2873 656c 662e 5f76 6572  e_node(self._ver
+00001540: 6966 6965 7229 0a20 2020 2020 2020 2062  ifier).        b
+00001550: 7569 6c64 6572 2e61 6464 5f63 6f6d 7075  uilder.add_compu
+00001560: 7465 5f6e 6f64 6528 7365 6c66 2e5f 6e6f  te_node(self._no
+00001570: 6f70 290a 2020 2020 2020 2020 666f 7220  op).        for 
+00001580: 656d 6169 6c20 696e 2075 7365 7273 3a0a  email in users:.
+00001590: 2020 2020 2020 2020 2020 2020 6275 696c              buil
+000015a0: 6465 722e 6164 645f 7573 6572 5f70 6572  der.add_user_per
+000015b0: 6d69 7373 696f 6e28 0a20 2020 2020 2020  mission(.       
+000015c0: 2020 2020 2020 2020 2065 6d61 696c 3d65           email=e
+000015d0: 6d61 696c 2c0a 2020 2020 2020 2020 2020  mail,.          
+000015e0: 2020 2020 2020 6175 7468 656e 7469 6361        authentica
+000015f0: 7469 6f6e 5f6d 6574 686f 643d 6175 7468  tion_method=auth
+00001600: 656e 7469 6361 7469 6f6e 2c0a 2020 2020  entication,.    
+00001610: 2020 2020 2020 2020 2020 2020 7065 726d              perm
+00001620: 6973 7369 6f6e 733d 5b0a 2020 2020 2020  issions=[.      
+00001630: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001640: 6c66 2e76 616c 6964 6174 696f 6e5f 7065  lf.validation_pe
+00001650: 726d 6973 7369 6f6e 2c0a 2020 2020 2020  rmission,.      
+00001660: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00001670: 6c66 2e6c 6561 665f 6372 7564 5f70 6572  lf.leaf_crud_per
+00001680: 6d69 7373 696f 6e0a 2020 2020 2020 2020  mission.        
+00001690: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+000016a0: 2020 2020 2020 290a 0a20 2020 2040 7072        )..    @pr
+000016b0: 6f70 6572 7479 0a20 2020 2064 6566 2076  operty.    def v
+000016c0: 616c 6964 6174 696f 6e5f 7065 726d 6973  alidation_permis
+000016d0: 7369 6f6e 2873 656c 6629 202d 3e20 5065  sion(self) -> Pe
+000016e0: 726d 6973 7369 6f6e 3a0a 2020 2020 2020  rmission:.      
+000016f0: 2020 2222 2254 6865 2070 6572 6d69 7373    """The permiss
+00001700: 696f 6e20 7265 7175 6972 6564 2074 6f20  ion required to 
+00001710: 7472 6967 6765 7220 7468 6520 6461 7461  trigger the data
+00001720: 2076 616c 6964 6174 696f 6e2e 2222 220a   validation.""".
+00001730: 2020 2020 2020 2020 7265 7475 726e 2050          return P
+00001740: 6572 6d69 7373 696f 6e73 2e65 7865 6375  ermissions.execu
+00001750: 7465 5f63 6f6d 7075 7465 2873 656c 662e  te_compute(self.
+00001760: 7661 6c69 6461 7469 6f6e 5f63 6f6d 7075  validation_compu
+00001770: 7461 7469 6f6e 5f6e 616d 6529 0a0a 2020  tation_name)..  
+00001780: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+00001790: 6465 6620 6c65 6166 5f63 7275 645f 7065  def leaf_crud_pe
+000017a0: 726d 6973 7369 6f6e 2873 656c 6629 202d  rmission(self) -
+000017b0: 3e20 5065 726d 6973 7369 6f6e 3a0a 2020  > Permission:.  
+000017c0: 2020 2020 2020 2222 2254 6865 2070 6572        """The per
+000017d0: 6d69 7373 696f 6e20 7265 7175 6972 6564  mission required
+000017e0: 2074 6f20 7570 6c6f 6164 2074 6865 2072   to upload the r
+000017f0: 6177 2c20 6e6f 6e2d 7661 6c69 6461 7465  aw, non-validate
+00001800: 6420 6461 7461 2e22 2222 0a20 2020 2020  d data.""".     
+00001810: 2020 2072 6574 7572 6e20 5065 726d 6973     return Permis
+00001820: 7369 6f6e 732e 6c65 6166 5f63 7275 6428  sions.leaf_crud(
+00001830: 7365 6c66 2e5f 6c65 6166 5f6e 6f64 655f  self._leaf_node_
+00001840: 6e61 6d65 290a 0a20 2020 2040 7072 6f70  name)..    @prop
+00001850: 6572 7479 0a20 2020 2064 6566 2069 6e70  erty.    def inp
+00001860: 7574 5f6e 6f64 655f 6e61 6d65 2873 656c  ut_node_name(sel
+00001870: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
+00001880: 2020 2022 2222 5468 6520 6e6f 6465 206e     """The node n
+00001890: 616d 6520 746f 2077 6869 6368 2064 6174  ame to which dat
+000018a0: 6120 7368 6f75 6c64 2062 6520 7570 6c6f  a should be uplo
+000018b0: 6164 6564 2e22 2222 0a20 2020 2020 2020  aded.""".       
+000018c0: 2072 6574 7572 6e20 7365 6c66 2e5f 6c65   return self._le
+000018d0: 6166 5f6e 6f64 655f 6e61 6d65 0a0a 2020  af_node_name..  
+000018e0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000018f0: 6465 6620 6f75 7470 7574 5f6e 6f64 655f  def output_node_
+00001900: 6e61 6d65 2873 656c 6629 202d 3e20 7374  name(self) -> st
+00001910: 723a 0a20 2020 2020 2020 2022 2222 5468  r:.        """Th
+00001920: 6520 6e6f 6465 206e 616d 6520 6672 6f6d  e node name from
+00001930: 2077 6869 6368 2064 6174 6120 6361 6e20   which data can 
+00001940: 6265 2072 6561 642c 2065 2e67 2e20 7468  be read, e.g. th
+00001950: 6520 6e61 6d65 2074 6f20 7573 6520 696e  e name to use in
+00001960: 2061 6e79 2064 6f77 6e73 7472 6561 6d20   any downstream 
+00001970: 5351 4c20 7175 6572 6965 732e 2222 220a  SQL queries.""".
+00001980: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00001990: 656c 662e 5f76 6572 6966 6965 725f 6e6f  elf._verifier_no
+000019a0: 6465 5f6e 616d 650a 0a0a 6465 6620 7265  de_name...def re
+000019b0: 6164 5f69 6e70 7574 5f63 7376 5f66 696c  ad_input_csv_fil
+000019c0: 6528 0a20 2020 2020 2020 2070 6174 683a  e(.        path:
+000019d0: 2073 7472 2c0a 2020 2020 2020 2020 2f2c   str,.        /,
+000019e0: 202a 2c0a 2020 2020 2020 2020 6861 735f   *,.        has_
+000019f0: 6865 6164 6572 3a20 626f 6f6c 203d 2054  header: bool = T
+00001a00: 7275 652c 0a20 2020 2020 2020 2063 6865  rue,.        che
+00001a10: 636b 5f68 6561 6465 723a 2062 6f6f 6c20  ck_header: bool 
+00001a20: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+00001a30: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00001a40: 2c0a 2020 2020 2020 2020 2a2a 6b77 6172  ,.        **kwar
+00001a50: 6773 0a29 202d 3e20 696f 2e42 7974 6573  gs.) -> io.Bytes
+00001a60: 494f 3a0a 2020 2020 2222 220a 2020 2020  IO:.    """.    
+00001a70: 5265 6164 2043 5356 2066 726f 6d20 6120  Read CSV from a 
+00001a80: 6669 6c65 2061 6e64 2074 7572 6e20 6974  file and turn it
+00001a90: 2069 6e74 6f20 6120 6279 7465 7320 6172   into a bytes ar
+00001aa0: 7261 7920 6f66 2074 6865 2063 6f72 7265  ray of the corre
+00001ab0: 6374 2066 6f72 6d61 7420 736f 2074 6861  ct format so tha
+00001ac0: 7420 6974 2063 616e 2062 6520 7570 6c6f  t it can be uplo
+00001ad0: 6164 6564 0a20 2020 2074 6f20 7468 6520  aded.    to the 
+00001ae0: 4465 6365 6e74 7269 7120 706c 6174 666f  Decentriq platfo
+00001af0: 726d 2e0a 0a20 2020 202a 2a50 6172 616d  rm...    **Param
+00001b00: 6574 6572 732a 2a3a 0a20 2020 202d 2060  eters**:.    - `
+00001b10: 7061 7468 603a 2054 6865 2070 6174 6820  path`: The path 
+00001b20: 746f 2074 6865 2043 5356 2066 696c 652e  to the CSV file.
+00001b30: 0a20 2020 202d 2060 6861 735f 6865 6164  .    - `has_head
+00001b40: 6572 603a 2057 6865 7468 6572 2074 6865  er`: Whether the
+00001b50: 2073 7472 696e 6720 636f 6e74 6169 6e73   string contains
+00001b60: 2061 2068 6561 6465 7220 726f 772e 0a20   a header row.. 
+00001b70: 2020 202d 2060 6368 6563 6b5f 6865 6164     - `check_head
+00001b80: 6572 603a 2057 6865 7468 6572 2074 6865  er`: Whether the
+00001b90: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
+00001ba0: 2074 7279 2074 6f20 6465 7465 726d 696e   try to determin
+00001bb0: 6520 7768 6574 6865 7220 7468 6520 6669  e whether the fi
+00001bc0: 6c65 2068 6173 2061 2068 6561 6465 722e  le has a header.
+00001bd0: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
+00001be0: 6669 6c65 2068 6173 2061 2068 6561 6465  file has a heade
+00001bf0: 7220 726f 7720 6275 7420 796f 7520 6469  r row but you di
+00001c00: 646e 2774 2073 6574 2074 6865 2060 6861  dn't set the `ha
+00001c10: 735f 6865 6164 6572 6020 666c 6167 2c20  s_header` flag, 
+00001c20: 616e 0a20 2020 2020 2020 2065 7863 6570  an.        excep
+00001c30: 7469 6f6e 2077 696c 6c20 6265 2072 6169  tion will be rai
+00001c40: 7365 642e 2049 6620 796f 7527 7265 2073  sed. If you're s
+00001c50: 7572 6520 7468 6174 2074 6865 2077 6179  ure that the way
+00001c60: 2079 6f75 2075 7365 2074 6865 2066 756e   you use the fun
+00001c70: 6374 696f 6e0a 2020 2020 2020 2020 6973  ction.        is
+00001c80: 2063 6f72 7265 6374 2c20 796f 7520 6361   correct, you ca
+00001c90: 6e20 6469 7361 626c 6520 7468 6973 2063  n disable this c
+00001ca0: 6865 636b 2075 7369 6e67 2074 6869 7320  heck using this 
+00001cb0: 7061 7261 6d65 7465 722e 0a20 2020 202d  parameter..    -
+00001cc0: 2060 656e 636f 6469 6e67 603a 2054 6865   `encoding`: The
+00001cd0: 2065 6e63 6f64 696e 6720 6f66 2074 6865   encoding of the
+00001ce0: 2043 5356 2066 696c 652e 2049 6620 796f   CSV file. If yo
+00001cf0: 7520 7772 6f74 6520 7468 6520 4353 5620  u wrote the CSV 
+00001d00: 6669 6c65 2075 7369 6e67 2061 206c 6962  file using a lib
+00001d10: 7261 7279 206c 696b 6520 7061 6e64 6173  rary like pandas
+00001d20: 2c0a 2020 2020 2020 2020 796f 7520 6e65  ,.        you ne
+00001d30: 6564 2074 6f20 6368 6563 6b20 7468 6520  ed to check the 
+00001d40: 646f 6375 6d65 6e74 6174 696f 6e20 746f  documentation to
+00001d50: 2073 6565 2077 6861 7420 656e 636f 6469   see what encodi
+00001d60: 6e67 2074 6865 7920 7573 6520 6279 2064  ng they use by d
+00001d70: 6566 6175 6c74 0a20 2020 2020 2020 2077  efault.        w
+00001d80: 6865 6e20 7772 6974 696e 6720 6669 6c65  hen writing file
+00001d90: 7320 286c 696b 656c 7920 6022 7574 662d  s (likely `"utf-
+00001da0: 3822 6020 696e 2077 6869 6368 2063 6173  8"` in which cas
+00001db0: 6520 7468 6973 2063 616e 2062 6520 6c65  e this can be le
+00001dc0: 6674 2061 7420 6974 7320 6465 6661 756c  ft at its defaul
+00001dd0: 7420 7661 6c75 6529 2e0a 2020 2020 2d20  t value)..    - 
+00001de0: 6064 656c 696d 6974 6572 603a 2057 6861  `delimiter`: Wha
+00001df0: 7420 6465 6c69 6d69 7465 7220 6973 2075  t delimiter is u
+00001e00: 7365 6420 696e 2074 6865 2074 6865 2043  sed in the the C
+00001e10: 5356 2066 696c 652e 2044 6566 6175 6c74  SV file. Default
+00001e20: 2069 7320 7468 6520 636f 6d6d 612e 0a20   is the comma.. 
+00001e30: 2020 202d 2060 2a2a 6b77 6172 6773 603a     - `**kwargs`:
+00001e40: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
+00001e50: 6f72 6420 6172 6775 6d65 6e74 7320 7061  ord arguments pa
+00001e60: 7373 6564 2074 6f20 7468 6520 5079 7468  ssed to the Pyth
+00001e70: 6f6e 2043 5356 2070 6172 7365 722e 2052  on CSV parser. R
+00001e80: 6566 6572 2074 6f20 7468 650a 2020 2020  efer to the.    
+00001e90: 2020 2020 5b6f 6666 6963 6961 6c20 646f      [official do
+00001ea0: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
+00001eb0: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
+00001ec0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f63  .org/3/library/c
+00001ed0: 7376 2e68 746d 6c23 6373 762d 666d 742d  sv.html#csv-fmt-
+00001ee0: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
+00001ef0: 666f 7220 6120 6c69 7374 206f 6620 7375  for a list of su
+00001f00: 7070 6f72 7465 6420 6172 6775 6d65 6e74  pported argument
+00001f10: 732e 0a0a 2020 2020 2a2a 5265 7475 726e  s...    **Return
+00001f20: 732a 2a3a 0a20 2020 2041 2042 7974 6573  s**:.    A Bytes
+00001f30: 494f 206f 626a 6563 7420 7468 6174 2063  IO object that c
+00001f40: 616e 2062 6520 7061 7373 6564 2074 6f20  an be passed to 
+00001f50: 7468 6520 6d65 7468 6f64 7320 7265 7370  the methods resp
+00001f60: 6f73 6962 6c65 2066 6f72 2075 706c 6f61  osible for uploa
+00001f70: 6469 6e67 2064 6174 612e 0a20 2020 2022  ding data..    "
+00001f80: 2222 0a20 2020 2077 6974 6820 6f70 656e  "".    with open
+00001f90: 2870 6174 682c 2027 7227 2c20 656e 636f  (path, 'r', enco
+00001fa0: 6469 6e67 3d65 6e63 6f64 696e 6729 2061  ding=encoding) a
+00001fb0: 7320 6373 7666 696c 653a 0a20 2020 2020  s csvfile:.     
+00001fc0: 2020 2072 6574 7572 6e20 5f72 6561 645f     return _read_
+00001fd0: 696e 7075 745f 6373 7628 0a20 2020 2020  input_csv(.     
+00001fe0: 2020 2020 2020 2063 7376 6669 6c65 2c0a         csvfile,.
+00001ff0: 2020 2020 2020 2020 2020 2020 6861 735f              has_
+00002000: 6865 6164 6572 3d68 6173 5f68 6561 6465  header=has_heade
+00002010: 722c 0a20 2020 2020 2020 2020 2020 2063  r,.            c
+00002020: 6865 636b 5f68 6561 6465 723d 6368 6563  heck_header=chec
+00002030: 6b5f 6865 6164 6572 2c0a 2020 2020 2020  k_header,.      
+00002040: 2020 2020 2020 2a2a 6b77 6172 6773 2c0a        **kwargs,.
+00002050: 2020 2020 2020 2020 290a 0a0a 6465 6620          )...def 
+00002060: 7265 6164 5f69 6e70 7574 5f63 7376 5f73  read_input_csv_s
+00002070: 7472 696e 6728 0a20 2020 2020 2020 2063  tring(.        c
+00002080: 6f6e 7465 6e74 3a20 7374 722c 0a20 2020  ontent: str,.   
+00002090: 2020 2020 202f 2c20 2a2c 0a20 2020 2020       /, *,.     
+000020a0: 2020 2068 6173 5f68 6561 6465 723a 2062     has_header: b
+000020b0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
+000020c0: 2020 2020 6368 6563 6b5f 6865 6164 6572      check_header
+000020d0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+000020e0: 2020 2020 2020 202a 2a6b 7761 7267 730a         **kwargs.
+000020f0: 2920 2d3e 2069 6f2e 4279 7465 7349 4f3a  ) -> io.BytesIO:
+00002100: 0a20 2020 2022 2222 0a20 2020 2052 6561  .    """.    Rea
+00002110: 6420 4353 5620 6672 6f6d 2061 2073 7472  d CSV from a str
+00002120: 696e 6720 616e 6420 7475 726e 2069 7420  ing and turn it 
+00002130: 696e 746f 2061 2062 7974 6573 2061 7272  into a bytes arr
+00002140: 6179 206f 6620 7468 6520 636f 7272 6563  ay of the correc
+00002150: 7420 666f 726d 6174 2073 6f20 7468 6174  t format so that
+00002160: 2069 7420 6361 6e20 6265 2075 706c 6f61   it can be uploa
+00002170: 6465 640a 2020 2020 746f 2074 6865 2044  ded.    to the D
+00002180: 6563 656e 7472 6971 2070 6c61 7466 6f72  ecentriq platfor
+00002190: 6d2e 0a0a 2020 2020 2a2a 5061 7261 6d65  m...    **Parame
+000021a0: 7465 7273 2a2a 3a0a 2020 2020 2d20 6063  ters**:.    - `c
+000021b0: 6f6e 7465 6e74 603a 2054 6865 2073 7472  ontent`: The str
+000021c0: 696e 6720 636f 6e74 6169 6e69 6e67 2074  ing containing t
+000021d0: 6865 2043 5356 2066 696c 652e 0a20 2020  he CSV file..   
+000021e0: 202d 2060 6861 735f 6865 6164 6572 603a   - `has_header`:
+000021f0: 2057 6865 7468 6572 2074 6865 2073 7472   Whether the str
+00002200: 696e 6720 636f 6e74 6169 6e73 2061 2068  ing contains a h
+00002210: 6561 6465 7220 726f 772e 0a20 2020 202d  eader row..    -
+00002220: 2060 6368 6563 6b5f 6865 6164 6572 603a   `check_header`:
+00002230: 2057 6865 7468 6572 2074 6865 2066 756e   Whether the fun
+00002240: 6374 696f 6e20 7368 6f75 6c64 2074 7279  ction should try
+00002250: 2074 6f20 6465 7465 726d 696e 6520 7768   to determine wh
+00002260: 6574 6865 7220 7468 6520 6669 6c65 2068  ether the file h
+00002270: 6173 2061 2068 6561 6465 722e 0a20 2020  as a header..   
+00002280: 2020 2020 2049 6620 7468 6520 6669 6c65       If the file
+00002290: 2068 6173 2061 2068 6561 6465 7220 726f   has a header ro
+000022a0: 7720 6275 7420 796f 7520 6469 646e 2774  w but you didn't
+000022b0: 2073 6574 2074 6865 2060 6861 735f 6865   set the `has_he
+000022c0: 6164 6572 6020 666c 6167 2c20 616e 0a20  ader` flag, an. 
+000022d0: 2020 2020 2020 2065 7863 6570 7469 6f6e         exception
+000022e0: 2077 696c 6c20 6265 2072 6169 7365 642e   will be raised.
+000022f0: 2049 6620 796f 7527 7265 2073 7572 6520   If you're sure 
+00002300: 7468 6174 2074 6865 2077 6179 2079 6f75  that the way you
+00002310: 2075 7365 2074 6865 2066 756e 6374 696f   use the functio
+00002320: 6e0a 2020 2020 2020 2020 6973 2063 6f72  n.        is cor
+00002330: 7265 6374 2c20 796f 7520 6361 6e20 6469  rect, you can di
+00002340: 7361 626c 6520 7468 6973 2063 6865 636b  sable this check
+00002350: 2075 7369 6e67 2074 6869 7320 7061 7261   using this para
+00002360: 6d65 7465 722e 0a20 2020 202d 2060 656e  meter..    - `en
+00002370: 636f 6469 6e67 603a 2054 6865 2065 6e63  coding`: The enc
+00002380: 6f64 696e 6720 6f66 2074 6865 2073 6f75  oding of the sou
+00002390: 7263 6520 6669 6c65 2e20 4966 2079 6f75  rce file. If you
+000023a0: 2077 726f 7465 2074 6865 2043 5356 2066   wrote the CSV f
+000023b0: 696c 6520 7573 696e 6720 6120 6c69 6272  ile using a libr
+000023c0: 6172 7920 6c69 6b65 2070 616e 6461 732c  ary like pandas,
+000023d0: 0a20 2020 2020 2020 2079 6f75 206e 6565  .        you nee
+000023e0: 6420 746f 2063 6865 636b 2074 6865 2064  d to check the d
+000023f0: 6f63 756d 656e 7461 7469 6f6e 2074 6f20  ocumentation to 
+00002400: 7365 6520 7768 6174 2065 6e63 6f64 696e  see what encodin
+00002410: 6720 7468 6579 2075 7365 2062 7920 6465  g they use by de
+00002420: 6661 756c 740a 2020 2020 2020 2020 7768  fault.        wh
+00002430: 656e 2077 7269 7469 6e67 2066 696c 6573  en writing files
+00002440: 2e0a 2020 2020 2d20 6064 656c 696d 6974  ..    - `delimit
+00002450: 6572 603a 2057 6861 7420 6465 6c69 6d69  er`: What delimi
+00002460: 7465 7220 6973 2075 7365 6420 696e 2074  ter is used in t
+00002470: 6865 2074 6865 2043 5356 2066 696c 652e  he the CSV file.
+00002480: 2044 6566 6175 6c74 2069 7320 7468 6520   Default is the 
+00002490: 636f 6d6d 612e 0a20 2020 202d 2060 2a2a  comma..    - `**
+000024a0: 6b77 6172 6773 603a 2041 6464 6974 696f  kwargs`: Additio
+000024b0: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+000024c0: 6d65 6e74 7320 7061 7373 6564 2074 6f20  ments passed to 
+000024d0: 7468 6520 5079 7468 6f6e 2043 5356 2070  the Python CSV p
+000024e0: 6172 7365 722e 2057 6861 7420 666c 6167  arser. What flag
+000024f0: 7320 6361 6e20 6265 2070 6173 7365 6420  s can be passed 
+00002500: 6361 6e20 6265 0a20 2020 2020 2020 2073  can be.        s
+00002510: 6565 6e20 5b68 6572 655d 2868 7474 7073  een [here](https
+00002520: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00002530: 7267 2f33 2f6c 6962 7261 7279 2f63 7376  rg/3/library/csv
+00002540: 2e68 746d 6c23 6373 762d 666d 742d 7061  .html#csv-fmt-pa
+00002550: 7261 6d73 292e 0a0a 2020 2020 2a2a 5265  rams)...    **Re
+00002560: 7475 726e 732a 2a3a 0a20 2020 2041 2042  turns**:.    A B
+00002570: 7974 6573 494f 206f 626a 6563 7420 7468  ytesIO object th
+00002580: 6174 2063 616e 2062 6520 7061 7373 6564  at can be passed
+00002590: 2074 6f20 7468 6520 6d65 7468 6f64 7320   to the methods 
+000025a0: 7265 7370 6f73 6962 6c65 2066 6f72 2075  resposible for u
+000025b0: 706c 6f61 6469 6e67 2064 6174 612e 0a20  ploading data.. 
+000025c0: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
+000025d0: 6e20 5f72 6561 645f 696e 7075 745f 6373  n _read_input_cs
+000025e0: 7628 0a20 2020 2020 2020 2069 6f2e 5374  v(.        io.St
+000025f0: 7269 6e67 494f 2863 6f6e 7465 6e74 2e73  ringIO(content.s
+00002600: 7472 6970 2829 292c 0a20 2020 2020 2020  trip()),.       
+00002610: 2068 6173 5f68 6561 6465 723d 6861 735f   has_header=has_
+00002620: 6865 6164 6572 2c0a 2020 2020 2020 2020  header,.        
+00002630: 6368 6563 6b5f 6865 6164 6572 3d63 6865  check_header=che
+00002640: 636b 5f68 6561 6465 722c 0a20 2020 2020  ck_header,.     
+00002650: 2020 202a 2a6b 7761 7267 730a 2020 2020     **kwargs.    
+00002660: 290a 0a0a 6465 6620 5f72 6561 645f 696e  )...def _read_in
+00002670: 7075 745f 6373 7628 0a20 2020 2020 2020  put_csv(.       
+00002680: 2064 6174 613a 2069 6f2e 5465 7874 494f   data: io.TextIO
+00002690: 4261 7365 2c0a 2020 2020 2020 2020 2f2c  Base,.        /,
+000026a0: 202a 2c0a 2020 2020 2020 2020 6861 735f   *,.        has_
+000026b0: 6865 6164 6572 3a20 626f 6f6c 203d 2054  header: bool = T
+000026c0: 7275 652c 0a20 2020 2020 2020 2063 6865  rue,.        che
+000026d0: 636b 5f68 6561 6465 723a 2062 6f6f 6c20  ck_header: bool 
+000026e0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+000026f0: 2a2a 6b77 6172 6773 0a29 202d 3e20 696f  **kwargs.) -> io
+00002700: 2e42 7974 6573 494f 3a0a 2020 2020 6966  .BytesIO:.    if
+00002710: 2063 6865 636b 5f68 6561 6465 723a 0a20   check_header:. 
+00002720: 2020 2020 2020 2073 616d 706c 6520 3d20         sample = 
+00002730: 275c 6e27 2e6a 6f69 6e28 6461 7461 2e72  '\n'.join(data.r
+00002740: 6561 646c 696e 6528 2920 666f 7220 5f20  eadline() for _ 
+00002750: 696e 2072 616e 6765 2832 3029 290a 2020  in range(20)).  
+00002760: 2020 2020 2020 6669 6c65 5f68 6173 5f68        file_has_h
+00002770: 6561 6465 7220 3d20 6373 762e 536e 6966  eader = csv.Snif
+00002780: 6665 7228 292e 6861 735f 6865 6164 6572  fer().has_header
+00002790: 2873 616d 706c 6529 0a20 2020 2020 2020  (sample).       
+000027a0: 2069 6620 6669 6c65 5f68 6173 5f68 6561   if file_has_hea
+000027b0: 6465 7220 616e 6420 6861 735f 6865 6164  der and has_head
+000027c0: 6572 2069 7320 4661 6c73 653a 0a20 2020  er is False:.   
+000027d0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000027e0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+000027f0: 2020 2020 2020 2020 2020 2257 6172 6e69            "Warni
+00002800: 6e67 3a20 7468 6520 6669 6c65 2073 6565  ng: the file see
+00002810: 6d73 2074 6f20 6861 7665 2061 2068 6561  ms to have a hea
+00002820: 6465 7220 6275 7420 7468 6520 6865 6164  der but the head
+00002830: 6572 2066 6c61 6720 6973 206e 6f74 2073  er flag is not s
+00002840: 6574 2074 6f20 7472 7565 2122 0a20 2020  et to true!".   
+00002850: 2020 2020 2020 2020 2020 2020 2022 2054               " T
+00002860: 6869 7320 666c 6167 206e 6565 6473 2074  his flag needs t
+00002870: 6f20 6265 2073 6574 2063 6f72 7265 6374  o be set correct
+00002880: 6c79 2069 6e20 6f72 6465 7220 666f 7220  ly in order for 
+00002890: 7468 6520 6461 7461 2074 6f20 6265 2075  the data to be u
+000028a0: 706c 6f61 6465 642e 220a 2020 2020 2020  ploaded.".      
+000028b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000028c0: 656c 6966 206e 6f74 2066 696c 655f 6861  elif not file_ha
+000028d0: 735f 6865 6164 6572 2061 6e64 2068 6173  s_header and has
+000028e0: 5f68 6561 6465 7220 6973 2054 7275 653a  _header is True:
+000028f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00002900: 7365 2045 7863 6570 7469 6f6e 280a 2020  se Exception(.  
+00002910: 2020 2020 2020 2020 2020 2020 2020 2257                "W
+00002920: 6172 6e69 6e67 3a20 7468 6520 6669 6c65  arning: the file
+00002930: 2064 6f65 736e 2774 2073 6565 6d20 746f   doesn't seem to
+00002940: 2068 6176 6520 6120 6865 6164 6572 2062   have a header b
+00002950: 7574 2074 6865 2068 6561 6465 7220 666c  ut the header fl
+00002960: 6167 2069 7320 7365 7421 220a 2020 2020  ag is set!".    
+00002970: 2020 2020 2020 2020 2020 2020 2220 5468              " Th
+00002980: 6973 2066 6c61 6720 6e65 6564 7320 746f  is flag needs to
+00002990: 2062 6520 7365 7420 636f 7272 6563 746c   be set correctl
+000029a0: 7920 696e 206f 7264 6572 2066 6f72 2074  y in order for t
+000029b0: 6865 2064 6174 6120 746f 2062 6520 7570  he data to be up
+000029c0: 6c6f 6164 6564 2e22 0a20 2020 2020 2020  loaded.".       
+000029d0: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
+000029e0: 6174 612e 7365 656b 2830 290a 2020 2020  ata.seek(0).    
+000029f0: 7265 6164 6572 203d 2063 7376 2e72 6561  reader = csv.rea
+00002a00: 6465 7228 6461 7461 2c20 2a2a 6b77 6172  der(data, **kwar
+00002a10: 6773 290a 2020 2020 6f75 7470 7574 203d  gs).    output =
+00002a20: 2069 6f2e 5374 7269 6e67 494f 286e 6577   io.StringIO(new
+00002a30: 6c69 6e65 3d22 2229 0a20 2020 2077 7269  line="").    wri
+00002a40: 7465 7220 3d20 6373 762e 7772 6974 6572  ter = csv.writer
+00002a50: 280a 2020 2020 2020 2020 6f75 7470 7574  (.        output
+00002a60: 2c0a 2020 2020 2020 2020 6465 6c69 6d69  ,.        delimi
+00002a70: 7465 723d 222c 222c 0a20 2020 2020 2020  ter=",",.       
+00002a80: 2071 756f 7465 6368 6172 3d27 2227 2c0a   quotechar='"',.
+00002a90: 2020 2020 2020 2020 7175 6f74 696e 673d          quoting=
+00002aa0: 6373 762e 5155 4f54 455f 4d49 4e49 4d41  csv.QUOTE_MINIMA
+00002ab0: 4c2c 0a20 2020 2020 2020 2064 6961 6c65  L,.        diale
+00002ac0: 6374 3d22 756e 6978 220a 2020 2020 290a  ct="unix".    ).
+00002ad0: 2020 2020 6966 2068 6173 5f68 6561 6465      if has_heade
+00002ae0: 723a 0a20 2020 2020 2020 206e 6578 7428  r:.        next(
+00002af0: 7265 6164 6572 290a 2020 2020 2320 5468  reader).    # Th
+00002b00: 6973 2077 696c 6c20 7772 6974 6520 7468  is will write th
+00002b10: 6520 6675 6c6c 2066 696c 6520 696e 746f  e full file into
+00002b20: 206d 656d 6f72 7920 616e 6420 656e 636f   memory and enco
+00002b30: 6465 2069 7420 696e 2062 756c 6b2e 0a20  de it in bulk.. 
+00002b40: 2020 2023 2043 6f75 6c64 2062 6520 7772     # Could be wr
+00002b50: 6170 7065 6420 696e 2061 2049 4f20 6275  apped in a IO bu
+00002b60: 6666 6572 2d73 7479 6c65 2063 6c61 7373  ffer-style class
+00002b70: 2074 6861 7420 776f 756c 6420 7065 7266   that would perf
+00002b80: 6f72 6d20 7468 650a 2020 2020 2320 7265  orm the.    # re
+00002b90: 6164 2f77 7269 7465 2063 7376 206c 696e  ad/write csv lin
+00002ba0: 6573 206f 7065 7261 7469 6f6e 2069 6e20  es operation in 
+00002bb0: 6120 7374 7265 616d 696e 6720 6661 7368  a streaming fash
+00002bc0: 696f 6e2e 0a20 2020 2066 6f72 2072 6f77  ion..    for row
+00002bd0: 2069 6e20 7265 6164 6572 3a0a 2020 2020   in reader:.    
+00002be0: 2020 2020 7772 6974 6572 2e77 7269 7465      writer.write
+00002bf0: 726f 7728 726f 7729 0a20 2020 206f 7574  row(row).    out
+00002c00: 7075 742e 7365 656b 2830 290a 2020 2020  put.seek(0).    
+00002c10: 7265 7475 726e 2069 6f2e 4279 7465 7349  return io.BytesI
+00002c20: 4f28 6f75 7470 7574 2e72 6561 6428 292e  O(output.read().
+00002c30: 656e 636f 6465 2822 7574 662d 3822 2929  encode("utf-8"))
+00002c40: 0a0a 0a64 6566 2075 706c 6f61 645f 616e  ...def upload_an
+00002c50: 645f 7075 626c 6973 685f 7461 6275 6c61  d_publish_tabula
+00002c60: 725f 6461 7461 7365 7428 0a20 2020 2020  r_dataset(.     
+00002c70: 2020 2064 6174 613a 2069 6f2e 4279 7465     data: io.Byte
+00002c80: 7349 4f2c 0a20 2020 2020 2020 206b 6579  sIO,.        key
+00002c90: 3a20 4b65 792c 0a20 2020 2020 2020 2064  : Key,.        d
+00002ca0: 6174 615f 726f 6f6d 5f69 643a 2073 7472  ata_room_id: str
+00002cb0: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+00002cc0: 2020 2020 2074 6162 6c65 3a20 7374 722c       table: str,
+00002cd0: 0a20 2020 2020 2020 2073 6573 7369 6f6e  .        session
+00002ce0: 3a20 5365 7373 696f 6e2c 0a20 2020 2020  : Session,.     
+00002cf0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+00002d00: 7374 7220 3d20 2222 2c0a 2020 2020 2020  str = "",.      
+00002d10: 2020 7661 6c69 6461 7465 3a20 626f 6f6c    validate: bool
+00002d20: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
+00002d30: 202a 2a6b 7761 7267 730a 2920 2d3e 2073   **kwargs.) -> s
+00002d40: 7472 3a0a 2020 2020 2222 220a 2020 2020  tr:.    """.    
+00002d50: 436f 6e76 656e 6965 6e63 6520 6675 6e63  Convenience func
+00002d60: 7469 6f6e 2066 6f72 2075 706c 6f61 6469  tion for uploadi
+00002d70: 6e67 2064 6174 6120 616e 6420 7661 6c69  ng data and vali
+00002d80: 6461 7469 6e67 2074 6865 2073 6368 656d  dating the schem
+00002d90: 6120 6f66 2074 6865 2075 706c 6f61 6465  a of the uploade
+00002da0: 640a 2020 2020 6461 7461 2e0a 0a20 2020  d.    data...   
+00002db0: 2056 616c 6964 6174 696f 6e20 6f66 2074   Validation of t
+00002dc0: 6162 756c 6172 2064 6174 6120 6973 2061  abular data is a
+00002dd0: 2073 6570 6172 6174 6520 636f 6d70 7574   separate comput
+00002de0: 6174 696f 6e20 666f 7220 7768 6963 6820  ation for which 
+00002df0: 7370 6563 6966 6963 2063 6f6d 7075 7465  specific compute
+00002e00: 206e 6f64 6573 0a20 2020 206e 6565 6420   nodes.    need 
+00002e10: 746f 2062 6520 7072 6573 656e 7420 696e  to be present in
+00002e20: 2074 6865 2063 6f6d 7075 7465 2067 7261   the compute gra
+00002e30: 7068 2064 6566 696e 6564 2062 7920 7468  ph defined by th
+00002e40: 6520 6461 7461 2072 6f6f 6d20 6465 6669  e data room defi
+00002e50: 6e69 7469 6f6e 2e0a 2020 2020 5468 6973  nition..    This
+00002e60: 2066 756e 6374 696f 6e20 7769 6c6c 2074   function will t
+00002e70: 616b 6520 6361 7265 206f 6620 7472 6967  ake care of trig
+00002e80: 6765 7269 6e67 2074 6865 2076 616c 6964  gering the valid
+00002e90: 6174 696f 6e20 6163 7469 6f6e 2066 6f72  ation action for
+00002ea0: 2079 6f75 2e0a 2020 2020 496e 2063 6173   you..    In cas
+00002eb0: 6520 7661 6c69 6461 7469 6f6e 2066 6169  e validation fai
+00002ec0: 6c73 2c20 616e 2065 7863 6570 7469 6f6e  ls, an exception
+00002ed0: 2077 696c 6c20 6265 2072 6169 7365 642e   will be raised.
+00002ee0: 2056 616c 6964 6174 696f 6e20 6361 6e20   Validation can 
+00002ef0: 6265 2074 7572 6e65 6420 6f66 660a 2020  be turned off.  
+00002f00: 2020 7573 696e 6720 7468 6520 6076 616c    using the `val
+00002f10: 6964 6174 6560 2070 6172 616d 6574 6572  idate` parameter
+00002f20: 2e0a 0a20 2020 202a 2a50 6172 616d 6574  ...    **Paramet
+00002f30: 6572 732a 2a3a 0a20 2020 202d 2060 6461  ers**:.    - `da
+00002f40: 7461 603a 2054 6865 2069 6e70 7574 2064  ta`: The input d
+00002f50: 6174 6120 746f 2062 6520 7570 6c6f 6164  ata to be upload
+00002f60: 6564 2e20 5573 6520 6f6e 6520 6f66 2074  ed. Use one of t
+00002f70: 6865 2072 6561 6465 7220 6675 6e63 7469  he reader functi
+00002f80: 6f6e 7320 7072 6f76 6964 6564 2069 6e20  ons provided in 
+00002f90: 7468 6973 0a20 2020 2020 2020 2070 6163  this.        pac
+00002fa0: 6b61 6765 2074 6f20 7265 6164 2043 5356  kage to read CSV
+00002fb0: 2d6c 696b 6520 6461 7461 2e0a 2020 2020  -like data..    
+00002fc0: 2d20 606b 6579 603a 2041 206b 6579 2066  - `key`: A key f
+00002fd0: 6f72 2065 6e63 7279 7074 696e 6720 7468  or encrypting th
+00002fe0: 6520 6461 7461 2074 6f2d 6265 2d75 706c  e data to-be-upl
+00002ff0: 6f61 6465 642e 0a20 2020 202d 2060 6461  oaded..    - `da
+00003000: 7461 5f72 6f6f 6d5f 6964 603a 2054 6f20  ta_room_id`: To 
+00003010: 7768 6963 6820 6461 7461 2072 6f6f 6d20  which data room 
+00003020: 7468 6520 6461 7461 7365 7420 7368 6f75  the dataset shou
+00003030: 6c64 2062 6520 7075 626c 6973 6865 642e  ld be published.
+00003040: 2054 6869 7320 6973 2074 6865 2069 6420   This is the id 
+00003050: 796f 750a 2020 2020 2020 2020 6765 7420  you.        get 
+00003060: 7768 656e 2070 7562 6c69 7368 696e 6720  when publishing 
+00003070: 6120 6461 7461 2072 6f6f 6d2e 0a20 2020  a data room..   
+00003080: 202d 2060 7461 626c 6560 3a20 5468 6520   - `table`: The 
+00003090: 6e61 6d65 206f 6620 7468 6520 6461 7461  name of the data
+000030a0: 206e 6f64 6520 6275 696c 6465 722e 0a20   node builder.. 
+000030b0: 2020 202d 2060 7365 7373 696f 6e60 3a20     - `session`: 
+000030c0: 5468 6520 7365 7373 696f 6e20 7769 7468  The session with
+000030d0: 2077 6869 6368 2074 6f20 636f 6d6d 756e   which to commun
+000030e0: 6963 6174 6520 7769 7468 2074 6865 2065  icate with the e
+000030f0: 6e63 6c61 7665 2e0a 2020 2020 2d20 6064  nclave..    - `d
+00003100: 6573 6372 6970 7469 6f6e 603a 2041 6e20  escription`: An 
+00003110: 6f70 7469 6f6e 616c 2064 6573 6372 6970  optional descrip
+00003120: 7469 6f6e 206f 6620 7468 6520 6461 7461  tion of the data
+00003130: 7365 742e 0a20 2020 202d 2060 7661 6c69  set..    - `vali
+00003140: 6461 7465 603a 2057 6865 7468 6572 2074  date`: Whether t
+00003150: 6f20 7065 7266 6f72 6d20 7468 6520 7661  o perform the va
+00003160: 6c69 6461 7469 6f6e 206f 7065 7261 7469  lidation operati
+00003170: 6f6e 2e0a 0a20 2020 202a 2a52 6574 7572  on...    **Retur
+00003180: 6e73 2a2a 3a0a 2020 2020 5468 6520 6d61  ns**:.    The ma
+00003190: 6e69 6665 7374 2068 6173 6820 2864 6174  nifest hash (dat
+000031a0: 6173 6574 2069 6429 2069 6e20 6361 7365  aset id) in case
+000031b0: 2074 6865 2075 706c 6f61 6420 616e 6420   the upload and 
+000031c0: 7661 6c69 6461 7469 6f6e 2073 7563 6365  validation succe
+000031d0: 6564 6564 2e0a 2020 2020 2222 220a 2020  eded..    """.  
+000031e0: 2020 6d61 6e69 6665 7374 5f68 6173 6820    manifest_hash 
+000031f0: 3d20 7365 7373 696f 6e2e 636c 6965 6e74  = session.client
+00003200: 2e75 706c 6f61 645f 6461 7461 7365 7428  .upload_dataset(
+00003210: 0a20 2020 2020 2020 2064 6174 612c 0a20  .        data,. 
+00003220: 2020 2020 2020 206b 6579 2c0a 2020 2020         key,.    
+00003230: 2020 2020 7461 626c 652c 0a20 2020 2020      table,.     
+00003240: 2020 2064 6573 6372 6970 7469 6f6e 3d64     description=d
+00003250: 6573 6372 6970 7469 6f6e 0a20 2020 2029  escription.    )
+00003260: 0a20 2020 2073 6573 7369 6f6e 2e70 7562  .    session.pub
+00003270: 6c69 7368 5f64 6174 6173 6574 280a 2020  lish_dataset(.  
+00003280: 2020 2020 2020 6461 7461 5f72 6f6f 6d5f        data_room_
+00003290: 6964 2c20 6d61 6e69 6665 7374 5f68 6173  id, manifest_has
+000032a0: 682c 0a20 2020 2020 2020 206c 6561 665f  h,.        leaf_
+000032b0: 6e61 6d65 3d5f 6461 7461 5f6e 6f64 655f  name=_data_node_
+000032c0: 6e61 6d65 2874 6162 6c65 292c 0a20 2020  name(table),.   
+000032d0: 2020 2020 206b 6579 3d6b 6579 0a20 2020       key=key.   
+000032e0: 2029 0a0a 2020 2020 6966 2076 616c 6964   )..    if valid
+000032f0: 6174 653a 0a20 2020 2020 2020 2074 7279  ate:.        try
+00003300: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00003310: 7373 696f 6e2e 7275 6e5f 636f 6d70 7574  ssion.run_comput
+00003320: 6174 696f 6e5f 616e 645f 6765 745f 7265  ation_and_get_re
+00003330: 7375 6c74 7328 0a20 2020 2020 2020 2020  sults(.         
+00003340: 2020 2020 2020 2064 6174 615f 726f 6f6d         data_room
+00003350: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
+00003360: 2020 2020 205f 6e6f 6f70 5f6e 6f64 655f       _noop_node_
+00003370: 6e61 6d65 2874 6162 6c65 292c 0a20 2020  name(table),.   
+00003380: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
+00003390: 7761 7267 730a 2020 2020 2020 2020 2020  wargs.          
+000033a0: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
+000033b0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+000033c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000033d0: 6169 7365 2045 7863 6570 7469 6f6e 2822  aise Exception("
+000033e0: 5661 6c69 6461 7469 6f6e 206f 6620 6461  Validation of da
+000033f0: 7461 7365 7420 6661 696c 6564 2120 5265  taset failed! Re
+00003400: 6173 6f6e 3a20 7b7d 222e 666f 726d 6174  ason: {}".format
+00003410: 2865 2929 0a0a 2020 2020 7265 7475 726e  (e))..    return
+00003420: 206d 616e 6966 6573 745f 6861 7368 0a0a   manifest_hash..
+00003430: 0a64 6566 205f 7265 6164 5f73 716c 5f71  .def _read_sql_q
+00003440: 7565 7279 5f72 6573 756c 7428 7265 7375  uery_result(resu
+00003450: 6c74 3a20 6279 7465 7329 202d 3e20 5475  lt: bytes) -> Tu
+00003460: 706c 655b 7374 722c 2054 6162 6c65 5363  ple[str, TableSc
+00003470: 6865 6d61 5d3a 0a20 2020 2061 7263 6869  hema]:.    archi
+00003480: 7665 203d 207a 6970 6669 6c65 2e5a 6970  ve = zipfile.Zip
+00003490: 4669 6c65 2869 6f2e 4279 7465 7349 4f28  File(io.BytesIO(
+000034a0: 7265 7375 6c74 292c 2022 7222 290a 0a20  result), "r").. 
+000034b0: 2020 2069 6620 7365 7428 6172 6368 6976     if set(archiv
+000034c0: 652e 6e61 6d65 6c69 7374 2829 2920 213d  e.namelist()) !=
+000034d0: 207b 2264 6174 6173 6574 2e63 7376 222c   {"dataset.csv",
+000034e0: 2022 7479 7065 7322 7d3a 0a20 2020 2020   "types"}:.     
+000034f0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+00003500: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00003510: 2254 6865 2067 6976 656e 2072 6573 756c  "The given resul
+00003520: 7420 6361 6e6e 6f74 2062 6520 7265 6164  t cannot be read
+00003530: 2061 7320 6974 2064 6f65 736e 2774 2063   as it doesn't c
+00003540: 6f6e 7461 696e 2061 6c6c 2074 6865 2072  ontain all the r
+00003550: 6571 7569 7265 6420 6669 6c65 732e 220a  equired files.".
+00003560: 2020 2020 2020 2020 2020 2020 2220 4578              " Ex
+00003570: 7065 6374 6564 2066 696c 6573 3a20 2764  pected files: 'd
+00003580: 6174 6173 6574 2e63 7376 2720 616e 6420  ataset.csv' and 
+00003590: 2774 7970 6573 272c 206f 6e6c 7920 666f  'types', only fo
+000035a0: 756e 643a 205b 7b7d 5d22 2e66 6f72 6d61  und: [{}]".forma
+000035b0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000035c0: 2020 2027 2c20 272e 6a6f 696e 2861 7263     ', '.join(arc
+000035d0: 6869 7665 2e6e 616d 656c 6973 7428 2929  hive.namelist())
+000035e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000035f0: 2020 2020 2020 2029 0a0a 2020 2020 6373         )..    cs
+00003600: 7620 3d20 6172 6368 6976 652e 7265 6164  v = archive.read
+00003610: 2822 6461 7461 7365 742e 6373 7622 292e  ("dataset.csv").
+00003620: 6465 636f 6465 2829 0a20 2020 2073 6368  decode().    sch
+00003630: 656d 6120 3d20 5461 626c 6553 6368 656d  ema = TableSchem
+00003640: 6128 290a 2020 2020 7061 7273 655f 6c65  a().    parse_le
+00003650: 6e67 7468 5f64 656c 696d 6974 6564 2861  ngth_delimited(a
+00003660: 7263 6869 7665 2e72 6561 6428 2274 7970  rchive.read("typ
+00003670: 6573 2229 2c20 7363 6865 6d61 290a 0a20  es"), schema).. 
+00003680: 2020 2072 6574 7572 6e20 2863 7376 2c20     return (csv, 
+00003690: 7363 6865 6d61 290a 0a0a 6465 6620 7265  schema)...def re
+000036a0: 6164 5f73 716c 5f71 7565 7279 5f72 6573  ad_sql_query_res
+000036b0: 756c 745f 6173 5f6c 6973 7428 7265 7375  ult_as_list(resu
+000036c0: 6c74 3a20 6279 7465 7329 202d 3e20 5475  lt: bytes) -> Tu
+000036d0: 706c 655b 4c69 7374 5b4c 6973 745b 7374  ple[List[List[st
+000036e0: 725d 5d2c 2054 6162 6c65 5363 6865 6d61  r]], TableSchema
+000036f0: 5d3a 0a20 2020 2022 2222 0a20 2020 2052  ]:.    """.    R
+00003700: 6561 6420 7468 6520 6769 7665 6e20 7261  ead the given ra
+00003710: 7720 4353 5620 6f75 7470 7574 2066 726f  w CSV output fro
+00003720: 6d20 616e 2053 514c 2071 7565 7279 2072  m an SQL query r
+00003730: 6573 756c 7420 616e 6420 7472 616e 7366  esult and transf
+00003740: 6f72 6d20 6974 2069 6e74 6f20 6120 6c69  orm it into a li
+00003750: 7374 206f 660a 2020 2020 6c69 7374 732c  st of.    lists,
+00003760: 2077 6865 7265 2065 6163 6820 696e 6e65   where each inne
+00003770: 7220 6c69 7374 2063 6f72 7265 7370 6f6e  r list correspon
+00003780: 6473 2074 6f20 6120 726f 7720 696e 2074  ds to a row in t
+00003790: 6865 2074 6162 756c 6172 206f 7574 7075  he tabular outpu
+000037a0: 7420 6461 7461 2e0a 2020 2020 5468 6520  t data..    The 
+000037b0: 6865 6164 6572 2072 6f77 2077 6f6e 2774  header row won't
+000037c0: 2062 6520 636f 6e74 6169 6e65 6420 696e   be contained in
+000037d0: 2074 6865 2072 6573 756c 7469 6e67 206f   the resulting o
+000037e0: 7574 7075 7420 616e 6420 616c 6c20 7468  utput and all th
+000037f0: 6520 696e 6e65 7220 7661 6c75 6573 0a20  e inner values. 
+00003800: 2020 2077 696c 6c20 6265 206f 6620 7479     will be of ty
+00003810: 7065 2073 7472 696e 672e 0a20 2020 2054  pe string..    T
+00003820: 6865 2061 6374 7561 6c20 636f 6c75 6d6e  he actual column
+00003830: 2074 7970 6573 2061 7320 7765 6c6c 2061   types as well a
+00003840: 7320 7468 6569 7220 6e61 6d65 7320 7769  s their names wi
+00003850: 6c6c 2062 6520 7265 7475 726e 6564 2061  ll be returned a
+00003860: 7320 7061 7274 206f 6620 7468 6520 7363  s part of the sc
+00003870: 6865 6d61 0a20 2020 2076 616c 7565 2e0a  hema.    value..
+00003880: 2020 2020 2222 220a 2020 2020 6373 765f      """.    csv_
+00003890: 636f 6e74 656e 742c 2073 6368 656d 6120  content, schema 
+000038a0: 3d20 5f72 6561 645f 7371 6c5f 7175 6572  = _read_sql_quer
+000038b0: 795f 7265 7375 6c74 2872 6573 756c 7429  y_result(result)
+000038c0: 0a20 2020 2072 6561 6465 7220 3d20 6373  .    reader = cs
+000038d0: 762e 7265 6164 6572 2869 6f2e 5374 7269  v.reader(io.Stri
+000038e0: 6e67 494f 2863 7376 5f63 6f6e 7465 6e74  ngIO(csv_content
+000038f0: 2929 0a20 2020 2072 6574 7572 6e20 6c69  )).    return li
+00003900: 7374 2872 6561 6465 7229 2c20 7363 6865  st(reader), sche
+00003910: 6d61 0a0a 0a64 6566 2072 6561 645f 7371  ma...def read_sq
+00003920: 6c5f 7175 6572 795f 7265 7375 6c74 5f61  l_query_result_a
+00003930: 735f 7374 7269 6e67 280a 2020 2020 2020  s_string(.      
+00003940: 2020 7265 7375 6c74 3a20 6279 7465 732c    result: bytes,
+00003950: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
+00003960: 5f68 6561 6465 723a 2062 6f6f 6c20 3d20  _header: bool = 
+00003970: 5472 7565 0a29 202d 3e20 7374 723a 0a20  True.) -> str:. 
+00003980: 2020 2022 2222 0a20 2020 2052 6561 6420     """.    Read 
+00003990: 7468 6520 6769 7665 6e20 7261 7720 4353  the given raw CS
+000039a0: 5620 6f75 7470 7574 2066 726f 6d20 616e  V output from an
+000039b0: 2053 514c 2071 7565 7279 2072 6573 756c   SQL query resul
+000039c0: 7420 616e 6420 7472 616e 7366 6f72 6d20  t and transform 
+000039d0: 6974 2069 6e74 6f20 6120 7374 7269 6e67  it into a string
+000039e0: 0a20 2020 2063 6f6e 7461 696e 696e 6720  .    containing 
+000039f0: 7468 6520 6675 6c6c 2043 5356 2066 696c  the full CSV fil
+00003a00: 6520 696e 636c 7564 696e 6720 7468 6520  e including the 
+00003a10: 6865 6164 6572 2072 6f77 2e0a 2020 2020  header row..    
+00003a20: 5468 6520 7265 7375 6c74 696e 6720 7374  The resulting st
+00003a30: 7269 6e67 2063 616e 2062 6520 7772 6974  ring can be writ
+00003a40: 7465 6e20 6469 7265 6374 6c79 2074 6f20  ten directly to 
+00003a50: 6120 6669 6c65 2066 726f 6d20 7768 6572  a file from wher
+00003a60: 6520 6974 2063 616e 2062 6520 7265 6164  e it can be read
+00003a70: 0a20 2020 2075 7369 6e67 2079 6f75 7220  .    using your 
+00003a80: 6461 7461 2061 6e61 6c79 7369 7320 6c69  data analysis li
+00003a90: 6272 6172 7920 6f66 2063 686f 6963 652e  brary of choice.
+00003aa0: 0a0a 2020 2020 2a2a 5061 7261 6d65 7465  ..    **Paramete
+00003ab0: 7273 2a2a 3a0a 2020 2020 2d20 6072 6573  rs**:.    - `res
+00003ac0: 756c 7460 3a20 5468 6520 7265 7375 6c74  ult`: The result
+00003ad0: 2066 726f 6d20 7768 6963 6820 746f 2065   from which to e
+00003ae0: 7874 7261 6374 2061 2043 5356 2066 696c  xtract a CSV fil
+00003af0: 6520 6173 2061 2073 7472 696e 672e 0a20  e as a string.. 
+00003b00: 2020 202d 2060 696e 636c 7564 655f 6865     - `include_he
+00003b10: 6164 6572 603a 2057 6865 7468 6572 2074  ader`: Whether t
+00003b20: 6f20 696e 636c 7564 6520 616e 2061 6464  o include an add
+00003b30: 6974 696f 6e61 6c20 6865 6164 6572 2072  itional header r
+00003b40: 6f77 2074 6861 7420 636f 6e74 6169 6e73  ow that contains
+00003b50: 0a20 2020 2020 2020 2063 6f6c 756d 6e20  .        column 
+00003b60: 6e61 6d65 7320 2870 726f 7669 6465 6420  names (provided 
+00003b70: 666f 7220 6578 616d 706c 6520 6279 2075  for example by u
+00003b80: 7369 6e67 2061 6c69 6173 2065 7870 7265  sing alias expre
+00003b90: 7373 696f 6e73 0a20 2020 2020 2020 2069  ssions.        i
+00003ba0: 6e20 5345 4c45 4354 2073 7461 7465 6d65  n SELECT stateme
+00003bb0: 6e74 7329 2e20 4966 2074 6869 7320 7365  nts). If this se
+00003bc0: 7474 696e 6720 6973 2074 7275 652c 2062  tting is true, b
+00003bd0: 7574 206e 6f20 636f 6c75 6d6e 0a20 2020  ut no column.   
+00003be0: 2020 2020 206e 616d 6573 2063 6f75 6c64       names could
+00003bf0: 2062 6520 666f 756e 642c 2074 6865 206e   be found, the n
+00003c00: 616d 6573 2022 5631 222c 2022 5632 2220  ames "V1", "V2" 
+00003c10: 616e 6420 736f 2077 696c 6c20 6265 2075  and so will be u
+00003c20: 7365 642e 0a20 2020 2022 2222 0a20 2020  sed..    """.   
+00003c30: 2063 6f6e 7465 6e74 2c20 7363 6865 6d61   content, schema
+00003c40: 203d 205f 7265 6164 5f73 716c 5f71 7565   = _read_sql_que
+00003c50: 7279 5f72 6573 756c 7428 7265 7375 6c74  ry_result(result
+00003c60: 290a 0a20 2020 2069 6620 696e 636c 7564  )..    if includ
+00003c70: 655f 6865 6164 6572 3a0a 2020 2020 2020  e_header:.      
+00003c80: 2020 6f70 745f 636f 6c75 6d6e 7320 3d20    opt_columns = 
+00003c90: 5b63 6f6c 2e6e 616d 6520 666f 7220 636f  [col.name for co
+00003ca0: 6c20 696e 2073 6368 656d 612e 6e61 6d65  l in schema.name
+00003cb0: 6443 6f6c 756d 6e73 5d0a 2020 2020 2020  dColumns].      
+00003cc0: 2020 2320 5573 6520 5631 2c20 5632 2c20    # Use V1, V2, 
+00003cd0: 2e2e 2e20 666f 7220 756e 6b6e 6f77 6e20  ... for unknown 
+00003ce0: 636f 6c75 6d6e 206e 616d 6573 203d 3e20  column names => 
+00003cf0: 7361 6d65 2066 6f72 6d61 7420 6173 2052  same format as R
+00003d00: 2075 7365 732e 0a20 2020 2020 2020 2072   uses..        r
+00003d10: 6570 6c61 6365 6d65 6e74 5f63 6f6c 756d  eplacement_colum
+00003d20: 6e73 203d 205b 6622 567b 6978 7d22 2066  ns = [f"V{ix}" f
+00003d30: 6f72 2069 7820 696e 2072 616e 6765 2831  or ix in range(1
+00003d40: 2c20 6c65 6e28 6f70 745f 636f 6c75 6d6e  , len(opt_column
+00003d50: 7329 202b 2031 295d 0a20 2020 2020 2020  s) + 1)].       
+00003d60: 2063 6f6c 756d 6e73 203d 205b 2063 3120   columns = [ c1 
+00003d70: 6966 2063 3120 656c 7365 2063 3220 666f  if c1 else c2 fo
+00003d80: 7220 6331 2c20 6332 2069 6e20 7a69 7028  r c1, c2 in zip(
+00003d90: 6f70 745f 636f 6c75 6d6e 732c 2072 6570  opt_columns, rep
+00003da0: 6c61 6365 6d65 6e74 5f63 6f6c 756d 6e73  lacement_columns
+00003db0: 295d 0a20 2020 2020 2020 2072 6574 7572  )].        retur
+00003dc0: 6e65 645f 636f 6e74 656e 7420 3d20 272c  ned_content = ',
+00003dd0: 272e 6a6f 696e 2863 6f6c 756d 6e73 2920  '.join(columns) 
+00003de0: 2b20 275c 6e27 202b 2063 6f6e 7465 6e74  + '\n' + content
+00003df0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00003e00: 2020 2072 6574 7572 6e65 645f 636f 6e74     returned_cont
+00003e10: 656e 7420 3d20 636f 6e74 656e 740a 0a20  ent = content.. 
+00003e20: 2020 2023 2052 656d 6f76 6520 7472 6169     # Remove trai
+00003e30: 6c69 6e67 206e 6577 6c69 6e65 730a 2020  ling newlines.  
+00003e40: 2020 7265 7475 726e 2072 6574 7572 6e65    return returne
+00003e50: 645f 636f 6e74 656e 742e 7374 7269 7028  d_content.strip(
+00003e60: 290a                                     ).
```

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/sql/compute.py` & `decentriq-platform-0.9.1/decentriq_platform/sql/compute.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/compute_sql_pb2.py` & `decentriq-platform-0.9.1/decentriq_platform/proto/compute_sql_pb2.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/sql/proto/compute_sql_pb2.pyi` & `decentriq-platform-0.9.1/decentriq_platform/proto/compute_sql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/storage.py` & `decentriq-platform-0.9.1/decentriq_platform/storage.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/types.py` & `decentriq-platform-0.9.1/decentriq_platform/types.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/decentriq_platform/verification.py` & `decentriq-platform-0.9.1/decentriq_platform/verification.py`

 * *Files identical despite different names*

### Comparing `decentriq-platform-0.9.0rc2/pyproject.toml` & `decentriq-platform-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "decentriq-platform"
-version = "0.9.0rc2"
+version = "0.9.1"
 description = "Python client library for the Decentriq platform"
 authors = ["decentriq <opensource@decentriq.com>"]
 readme = 'README.md'
 repository = "https://github.com/decentriq/decentriq-platform"
 homepage = "https://github.com/decentriq/decentriq-platform"
 
 [tool.poetry.dependencies]
 # main package
 python = "^3.9"
 typing-extensions = "^3.10.0"
 protobuf = "^3.18.0"
-requests = "^2.26.0"
+requests = "^2.27.0"
 sgx-ias-structs = "^0.1.7"
 cryptography = "^3.4.8"
 chily = "^0.5.3"
 asn1crypto = "^1.4.0"
 oscrypto = "^1.2.1"
 certvalidator = "^0.11.1"
 ecdsa = "^0.17.0"
```

### Comparing `decentriq-platform-0.9.0rc2/setup.py` & `decentriq-platform-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,22 +17,22 @@
  'certvalidator>=0.11.1,<0.12.0',
  'chily>=0.5.3,<0.6.0',
  'cryptography>=3.4.8,<4.0.0',
  'ecdsa>=0.17.0,<0.18.0',
  'oscrypto>=1.2.1,<2.0.0',
  'pem>=21.2.0,<22.0.0',
  'protobuf>=3.18.0,<4.0.0',
- 'requests>=2.26.0,<3.0.0',
+ 'requests>=2.27.0,<3.0.0',
  'sgx-ias-structs>=0.1.7,<0.2.0',
  'sqloxide>=0.1.11,<0.2.0',
  'typing-extensions>=3.10.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'decentriq-platform',
-    'version': '0.9.0rc2',
+    'version': '0.9.1',
     'description': 'Python client library for the Decentriq platform',
     'long_description': '# decentriq-platform\n\nPython client library for the Decentriq platform.\n',
     'author': 'decentriq',
     'author_email': 'opensource@decentriq.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/decentriq/decentriq-platform',
```

### Comparing `decentriq-platform-0.9.0rc2/PKG-INFO` & `decentriq-platform-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentriq-platform
-Version: 0.9.0rc2
+Version: 0.9.1
 Summary: Python client library for the Decentriq platform
 Home-page: https://github.com/decentriq/decentriq-platform
 Author: decentriq
 Author-email: opensource@decentriq.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: certvalidator (>=0.11.1,<0.12.0)
 Requires-Dist: chily (>=0.5.3,<0.6.0)
 Requires-Dist: cryptography (>=3.4.8,<4.0.0)
 Requires-Dist: ecdsa (>=0.17.0,<0.18.0)
 Requires-Dist: oscrypto (>=1.2.1,<2.0.0)
 Requires-Dist: pem (>=21.2.0,<22.0.0)
 Requires-Dist: protobuf (>=3.18.0,<4.0.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: requests (>=2.27.0,<3.0.0)
 Requires-Dist: sgx-ias-structs (>=0.1.7,<0.2.0)
 Requires-Dist: sqloxide (>=0.1.11,<0.2.0)
 Requires-Dist: typing-extensions (>=3.10.0,<4.0.0)
 Project-URL: Repository, https://github.com/decentriq/decentriq-platform
 Description-Content-Type: text/markdown
 
 # decentriq-platform
```

