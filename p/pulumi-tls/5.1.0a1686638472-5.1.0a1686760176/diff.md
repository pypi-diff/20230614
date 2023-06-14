# Comparing `tmp/pulumi_tls-5.1.0a1686638472.tar.gz` & `tmp/pulumi_tls-5.1.0a1686760176.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1686638472.tar", last modified: Tue Jun 13 06:48:04 2023, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1686760176.tar", last modified: Wed Jun 14 16:34:52 2023, max compression
```

## Comparing `pulumi_tls-5.1.0a1686638472.tar` & `pulumi_tls-5.1.0a1686760176.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:48:04.074416 pulumi_tls-5.1.0a1686638472/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-13 06:48:04.074416 pulumi_tls-5.1.0a1686638472/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:48:04.074416 pulumi_tls-5.1.0a1686638472/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    24351 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:48:04.074416 pulumi_tls-5.1.0a1686638472/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    42903 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26381 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54199 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:48:04.074416 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-13 06:48:04.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 06:48:04.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:48:04.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:48:04.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:48:04.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 06:48:04.000000 pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:48:04.074416 pulumi_tls-5.1.0a1686638472/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 06:48:03.000000 pulumi_tls-5.1.0a1686638472/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:52.428479 pulumi_tls-5.1.0a1686760176/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-14 16:34:52.428479 pulumi_tls-5.1.0a1686760176/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:52.428479 pulumi_tls-5.1.0a1686760176/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22603 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:52.428479 pulumi_tls-5.1.0a1686760176/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41155 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22201 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 16:34:52.428479 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-14 16:34:52.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-14 16:34:52.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:34:52.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 16:34:52.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-14 16:34:52.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-14 16:34:52.000000 pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 16:34:52.428479 pulumi_tls-5.1.0a1686760176/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-14 16:34:51.000000 pulumi_tls-5.1.0a1686760176/setup.py
```

### Comparing `pulumi_tls-5.1.0a1686638472/PKG-INFO` & `pulumi_tls-5.1.0a1686760176/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1686638472
+Version: 5.1.0a1686760176
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-tls/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-tls/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Ftls.svg)](https://www.npmjs.com/package/@pulumi/tls)
 [![Python version](https://badge.fury.io/py/pulumi-tls.svg)](https://pypi.org/project/pulumi-tls)
 [![NuGet version](https://badge.fury.io/nu/pulumi.tls.svg)](https://badge.fury.io/nu/pulumi.tls)
```

### Comparing `pulumi_tls-5.1.0a1686638472/README.md` & `pulumi_tls-5.1.0a1686760176/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/cert_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -112,19 +112,15 @@
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  key_algorithm: Optional[pulumi.Input[str]] = None,
                  private_key_pem: Optional[pulumi.Input[str]] = None,
                  subject: Optional[pulumi.Input['CertRequestSubjectArgs']] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering CertRequest resources.
-        :param pulumi.Input[str] cert_request_pem: The certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-               [underlying](https://pkg.go.dev/encoding/pem#Encode)
-               [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-               the end of the PEM. In case this disrupts your use case, we recommend using
-               [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        :param pulumi.Input[str] cert_request_pem: The certificate request data in PEM (RFC 1421).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[str] key_algorithm: Name of the algorithm used when generating the private key provided in `private_key_pem`.
         :param pulumi.Input[str] private_key_pem: Private key in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format, that the certificate will belong
                to. This can be read from a separate file using the [`file`](https://www.terraform.io/language/functions/file)
                interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state.
         :param pulumi.Input['CertRequestSubjectArgs'] subject: The subject for which a certificate is being requested. The acceptable arguments are all optional and their naming is based upon [Issuer Distinguished Names (RFC5280)](https://tools.ietf.org/html/rfc5280#section-4.1.2.4) section.
@@ -145,19 +141,15 @@
         if uris is not None:
             pulumi.set(__self__, "uris", uris)
 
     @property
     @pulumi.getter(name="certRequestPem")
     def cert_request_pem(self) -> Optional[pulumi.Input[str]]:
         """
-        The certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-        [underlying](https://pkg.go.dev/encoding/pem#Encode)
-        [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-        the end of the PEM. In case this disrupts your use case, we recommend using
-        [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        The certificate request data in PEM (RFC 1421).
         """
         return pulumi.get(self, "cert_request_pem")
 
     @cert_request_pem.setter
     def cert_request_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert_request_pem", value)
 
@@ -353,19 +345,15 @@
         """
         Get an existing CertRequest resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cert_request_pem: The certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-               [underlying](https://pkg.go.dev/encoding/pem#Encode)
-               [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-               the end of the PEM. In case this disrupts your use case, we recommend using
-               [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        :param pulumi.Input[str] cert_request_pem: The certificate request data in PEM (RFC 1421).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[str] key_algorithm: Name of the algorithm used when generating the private key provided in `private_key_pem`.
         :param pulumi.Input[str] private_key_pem: Private key in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format, that the certificate will belong
                to. This can be read from a separate file using the [`file`](https://www.terraform.io/language/functions/file)
                interpolation function. Only an irreversible secure hash of the private key will be stored in the Terraform state.
         :param pulumi.Input[pulumi.InputType['CertRequestSubjectArgs']] subject: The subject for which a certificate is being requested. The acceptable arguments are all optional and their naming is based upon [Issuer Distinguished Names (RFC5280)](https://tools.ietf.org/html/rfc5280#section-4.1.2.4) section.
@@ -384,19 +372,15 @@
         __props__.__dict__["uris"] = uris
         return CertRequest(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="certRequestPem")
     def cert_request_pem(self) -> pulumi.Output[str]:
         """
-        The certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-        [underlying](https://pkg.go.dev/encoding/pem#Encode)
-        [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-        the end of the PEM. In case this disrupts your use case, we recommend using
-        [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        The certificate request data in PEM (RFC 1421).
         """
         return pulumi.get(self, "cert_request_pem")
 
     @property
     @pulumi.getter(name="dnsNames")
     def dns_names(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/get_public_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,25 @@
         The fingerprint of the public key data in OpenSSH SHA256 hash format, e.g. `SHA256:...`. Only available if the selected private key format is compatible, as per the rules for `public_key_openssh` and ECDSA P224 limitations.
         """
         return pulumi.get(self, "public_key_fingerprint_sha256")
 
     @property
     @pulumi.getter(name="publicKeyOpenssh")
     def public_key_openssh(self) -> str:
+        """
+        The public key, in  OpenSSH PEM (RFC 4716).
+        """
         return pulumi.get(self, "public_key_openssh")
 
     @property
     @pulumi.getter(name="publicKeyPem")
     def public_key_pem(self) -> str:
+        """
+        The public key, in PEM (RFC 1421).
+        """
         return pulumi.get(self, "public_key_pem")
 
 
 class AwaitableGetPublicKeyResult(GetPublicKeyResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
```

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/locally_signed_cert.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,19 +168,15 @@
                  validity_start_time: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering LocallySignedCert resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] ca_cert_pem: Certificate data of the Certificate Authority (CA) in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] ca_key_algorithm: Name of the algorithm used when generating the private key provided in `ca_private_key_pem`.
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
-        :param pulumi.Input[str] cert_pem: Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-               [underlying](https://pkg.go.dev/encoding/pem#Encode)
-               [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-               the end of the PEM. In case this disrupts your use case, we recommend using
-               [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[str] cert_request_pem: Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
@@ -265,19 +261,15 @@
     def ca_private_key_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_private_key_pem", value)
 
     @property
     @pulumi.getter(name="certPem")
     def cert_pem(self) -> Optional[pulumi.Input[str]]:
         """
-        Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-        [underlying](https://pkg.go.dev/encoding/pem#Encode)
-        [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-        the end of the PEM. In case this disrupts your use case, we recommend using
-        [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        Certificate data in PEM (RFC 1421).
         """
         return pulumi.get(self, "cert_pem")
 
     @cert_pem.setter
     def cert_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert_pem", value)
 
@@ -508,19 +500,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
         :param pulumi.Input[str] ca_cert_pem: Certificate data of the Certificate Authority (CA) in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[str] ca_key_algorithm: Name of the algorithm used when generating the private key provided in `ca_private_key_pem`.
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
-        :param pulumi.Input[str] cert_pem: Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-               [underlying](https://pkg.go.dev/encoding/pem#Encode)
-               [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-               the end of the PEM. In case this disrupts your use case, we recommend using
-               [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[str] cert_request_pem: Certificate request data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
@@ -581,19 +569,15 @@
         """
         return pulumi.get(self, "ca_private_key_pem")
 
     @property
     @pulumi.getter(name="certPem")
     def cert_pem(self) -> pulumi.Output[str]:
         """
-        Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-        [underlying](https://pkg.go.dev/encoding/pem#Encode)
-        [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-        the end of the PEM. In case this disrupts your use case, we recommend using
-        [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        Certificate data in PEM (RFC 1421).
         """
         return pulumi.get(self, "cert_pem")
 
     @property
     @pulumi.getter(name="certRequestPem")
     def cert_request_pem(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,14 +306,15 @@
                  public_key_algorithm: str,
                  serial_number: str,
                  sha1_fingerprint: str,
                  signature_algorithm: str,
                  subject: str,
                  version: int):
         """
+        :param str cert_pem: Certificate data in PEM (RFC 1421).
         :param bool is_ca: `true` if the certificate is of a CA (Certificate Authority).
         :param str issuer: Who verified and signed the certificate, roughly following [RFC2253](https://tools.ietf.org/html/rfc2253).
         :param str not_after: The time until which the certificate is invalid, as an [RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
         :param str not_before: The time after which the certificate is valid, as an [RFC3339](https://tools.ietf.org/html/rfc3339) timestamp.
         :param str public_key_algorithm: The key algorithm used to create the certificate.
         :param str serial_number: Number that uniquely identifies the certificate with the CA's system.
                The `format` function can be used to convert this *base 10* number into other bases, such as hex.
@@ -333,14 +334,17 @@
         pulumi.set(__self__, "signature_algorithm", signature_algorithm)
         pulumi.set(__self__, "subject", subject)
         pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="certPem")
     def cert_pem(self) -> str:
+        """
+        Certificate data in PEM (RFC 1421).
+        """
         return pulumi.get(self, "cert_pem")
 
     @property
     @pulumi.getter(name="isCa")
     def is_ca(self) -> bool:
         """
         `true` if the certificate is of a CA (Certificate Authority).
```

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1686760176/pulumi_tls/self_signed_cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,19 +224,15 @@
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validity_end_time: Optional[pulumi.Input[str]] = None,
                  validity_period_hours: Optional[pulumi.Input[int]] = None,
                  validity_start_time: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering SelfSignedCert resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
-        :param pulumi.Input[str] cert_pem: Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-               [underlying](https://pkg.go.dev/encoding/pem#Encode)
-               [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-               the end of the PEM. In case this disrupts your use case, we recommend using
-               [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
@@ -299,19 +295,15 @@
     def allowed_uses(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "allowed_uses", value)
 
     @property
     @pulumi.getter(name="certPem")
     def cert_pem(self) -> Optional[pulumi.Input[str]]:
         """
-        Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-        [underlying](https://pkg.go.dev/encoding/pem#Encode)
-        [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-        the end of the PEM. In case this disrupts your use case, we recommend using
-        [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        Certificate data in PEM (RFC 1421).
         """
         return pulumi.get(self, "cert_pem")
 
     @cert_pem.setter
     def cert_pem(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert_pem", value)
 
@@ -626,19 +618,15 @@
         Get an existing SelfSignedCert resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_uses: List of key usages allowed for the issued certificate. Values are defined in [RFC 5280](https://datatracker.ietf.org/doc/html/rfc5280) and combine flags defined by both [Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.3) and [Extended Key Usages](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.12). Accepted values: `any_extended`, `cert_signing`, `client_auth`, `code_signing`, `content_commitment`, `crl_signing`, `data_encipherment`, `decipher_only`, `digital_signature`, `email_protection`, `encipher_only`, `ipsec_end_system`, `ipsec_tunnel`, `ipsec_user`, `key_agreement`, `key_encipherment`, `microsoft_commercial_code_signing`, `microsoft_kernel_code_signing`, `microsoft_server_gated_crypto`, `netscape_server_gated_crypto`, `ocsp_signing`, `server_auth`, `timestamping`.
-        :param pulumi.Input[str] cert_pem: Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-               [underlying](https://pkg.go.dev/encoding/pem#Encode)
-               [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-               the end of the PEM. In case this disrupts your use case, we recommend using
-               [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        :param pulumi.Input[str] cert_pem: Certificate data in PEM (RFC 1421).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
@@ -686,19 +674,15 @@
         """
         return pulumi.get(self, "allowed_uses")
 
     @property
     @pulumi.getter(name="certPem")
     def cert_pem(self) -> pulumi.Output[str]:
         """
-        Certificate data in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format. **NOTE**: the
-        [underlying](https://pkg.go.dev/encoding/pem#Encode)
-        [libraries](https://pkg.go.dev/golang.org/x/crypto/ssh#MarshalAuthorizedKey) that generate this value append a `\\n` at
-        the end of the PEM. In case this disrupts your use case, we recommend using
-        [`trimspace()`](https://www.terraform.io/language/functions/trimspace).
+        Certificate data in PEM (RFC 1421).
         """
         return pulumi.get(self, "cert_pem")
 
     @property
     @pulumi.getter(name="dnsNames")
     def dns_names(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-tls
-Version: 5.1.0a1686638472
+Version: 5.1.0a1686760176
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi tls
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-tls/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-tls/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Ftls.svg)](https://www.npmjs.com/package/@pulumi/tls)
 [![Python version](https://badge.fury.io/py/pulumi-tls.svg)](https://pypi.org/project/pulumi-tls)
 [![NuGet version](https://badge.fury.io/nu/pulumi.tls.svg)](https://badge.fury.io/nu/pulumi.tls)
```

### Comparing `pulumi_tls-5.1.0a1686638472/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1686760176/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1686638472/setup.py` & `pulumi_tls-5.1.0a1686760176/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.1.0a1686638472"
-PLUGIN_VERSION = "5.1.0-alpha.1686638472+dc554b10"
+VERSION = "5.1.0a1686760176"
+PLUGIN_VERSION = "5.1.0-alpha.1686760176+103baca8"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'tls', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "tls Pulumi Package - Development Version"
 
 
 setup(name='pulumi_tls',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package to create TLS resources in Pulumi programs.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

