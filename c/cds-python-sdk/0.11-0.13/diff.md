# Comparing `tmp/cds-python-sdk-0.11.tar.gz` & `tmp/cds-python-sdk-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cds-python-sdk-0.11.tar", last modified: Wed May 31 09:03:33 2023, max compression
+gzip compressed data, was "cds-python-sdk-0.13.tar", last modified: Wed Jun 14 06:07:16 2023, max compression
```

## Comparing `cds-python-sdk-0.11.tar` & `cds-python-sdk-0.13.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.480455 cds-python-sdk-0.11/
--rw-rw-rw-   0        0        0    10313 2023-05-23 06:32:39.000000 cds-python-sdk-0.11/LICENSE
--rw-rw-rw-   0        0        0      221 2023-05-31 09:03:33.479530 cds-python-sdk-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     4500 2023-05-31 08:44:17.000000 cds-python-sdk-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.440857 cds-python-sdk-0.11/capitalonline/
--rw-rw-rw-   0        0        0       17 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.447510 cds-python-sdk-0.11/capitalonline/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/common/__init__.py
--rw-rw-rw-   0        0        0    18497 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/abstract_client.py
--rw-rw-rw-   0        0        0     1127 2023-05-11 07:27:33.000000 cds-python-sdk-0.11/capitalonline/common/client.py
--rw-rw-rw-   0        0        0     1761 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/credential.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.449513 cds-python-sdk-0.11/capitalonline/common/exception/
--rw-rw-rw-   0        0        0      122 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/exception/__init__.py
--rw-rw-rw-   0        0        0      706 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/exception/cds_sdk_exception.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.452505 cds-python-sdk-0.11/capitalonline/common/http/
--rw-rw-rw-   0        0        0        0 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/http/__init__.py
--rw-rw-rw-   0        0        0     5211 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/http/request.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.457467 cds-python-sdk-0.11/capitalonline/common/profile/
--rw-rw-rw-   0        0        0        0 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/profile/__init__.py
--rw-rw-rw-   0        0        0     1048 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/common/profile/client_profile.py
--rw-rw-rw-   0        0        0     1300 2023-05-30 06:44:49.000000 cds-python-sdk-0.11/capitalonline/common/profile/http_profile.py
--rw-rw-rw-   0        0        0     2782 2023-05-10 08:44:21.000000 cds-python-sdk-0.11/capitalonline/common/sign.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.462449 cds-python-sdk-0.11/capitalonline/haproxy/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/haproxy/__init__.py
--rw-rw-rw-   0        0        0    12947 2023-05-30 06:43:43.000000 cds-python-sdk-0.11/capitalonline/haproxy/client.py
--rw-rw-rw-   0        0        0     9175 2023-05-31 08:59:17.000000 cds-python-sdk-0.11/capitalonline/haproxy/client_test.py
--rw-rw-rw-   0        0        0     7938 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/haproxy/models.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.467425 cds-python-sdk-0.11/capitalonline/instance/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/instance/__init__.py
--rw-rw-rw-   0        0        0    12078 2023-05-30 06:35:06.000000 cds-python-sdk-0.11/capitalonline/instance/client.py
--rw-rw-rw-   0        0        0    11436 2023-05-31 01:32:34.000000 cds-python-sdk-0.11/capitalonline/instance/client_test.py
--rw-rw-rw-   0        0        0     5795 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/instance/models.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.473541 cds-python-sdk-0.11/capitalonline/vdc/
--rw-rw-rw-   0        0        0        0 2023-05-08 10:10:30.000000 cds-python-sdk-0.11/capitalonline/vdc/__init__.py
--rw-rw-rw-   0        0        0     5518 2023-05-30 06:43:43.000000 cds-python-sdk-0.11/capitalonline/vdc/client.py
--rw-rw-rw-   0        0        0     6335 2023-05-31 08:48:52.000000 cds-python-sdk-0.11/capitalonline/vdc/client_test.py
--rw-rw-rw-   0        0        0     6908 2023-05-29 07:01:55.000000 cds-python-sdk-0.11/capitalonline/vdc/model.py
-drwxrwxrwx   0        0        0        0 2023-05-31 09:03:33.478524 cds-python-sdk-0.11/cds_python_sdk.egg-info/
--rw-rw-rw-   0        0        0      221 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 09:03:33.000000 cds-python-sdk-0.11/cds_python_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 09:03:33.480455 cds-python-sdk-0.11/setup.cfg
--rw-rw-rw-   0        0        0      384 2023-05-31 09:03:01.000000 cds-python-sdk-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.676268 cds-python-sdk-0.13/
+-rw-rw-rw-   0        0        0    10313 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/LICENSE
+-rw-rw-rw-   0        0        0      221 2023-06-14 06:07:16.674252 cds-python-sdk-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     4807 2023-06-14 05:59:06.000000 cds-python-sdk-0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.632641 cds-python-sdk-0.13/capitalonline/
+-rw-rw-rw-   0        0        0       17 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.640258 cds-python-sdk-0.13/capitalonline/common/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/__init__.py
+-rw-rw-rw-   0        0        0    18497 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/abstract_client.py
+-rw-rw-rw-   0        0        0     1127 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/client.py
+-rw-rw-rw-   0        0        0     1761 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/credential.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.643611 cds-python-sdk-0.13/capitalonline/common/exception/
+-rw-rw-rw-   0        0        0      122 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/exception/__init__.py
+-rw-rw-rw-   0        0        0      706 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/exception/cds_sdk_exception.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.646518 cds-python-sdk-0.13/capitalonline/common/http/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/http/__init__.py
+-rw-rw-rw-   0        0        0     5211 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/http/request.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.649683 cds-python-sdk-0.13/capitalonline/common/profile/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/profile/__init__.py
+-rw-rw-rw-   0        0        0     1048 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/profile/client_profile.py
+-rw-rw-rw-   0        0        0     1300 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/profile/http_profile.py
+-rw-rw-rw-   0        0        0     2782 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/common/sign.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.654652 cds-python-sdk-0.13/capitalonline/haproxy/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/__init__.py
+-rw-rw-rw-   0        0        0    12947 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/client.py
+-rw-rw-rw-   0        0        0     9175 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/client_test.py
+-rw-rw-rw-   0        0        0     7938 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/haproxy/models.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.662485 cds-python-sdk-0.13/capitalonline/instance/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/instance/__init__.py
+-rw-rw-rw-   0        0        0    12078 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/instance/client.py
+-rw-rw-rw-   0        0        0    11860 2023-06-14 05:59:06.000000 cds-python-sdk-0.13/capitalonline/instance/client_test.py
+-rw-rw-rw-   0        0        0     6247 2023-06-14 03:18:20.000000 cds-python-sdk-0.13/capitalonline/instance/models.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.666920 cds-python-sdk-0.13/capitalonline/vdc/
+-rw-rw-rw-   0        0        0        0 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/__init__.py
+-rw-rw-rw-   0        0        0     5518 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/client.py
+-rw-rw-rw-   0        0        0     6335 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/client_test.py
+-rw-rw-rw-   0        0        0     6908 2023-06-13 08:29:06.000000 cds-python-sdk-0.13/capitalonline/vdc/model.py
+drwxrwxrwx   0        0        0        0 2023-06-14 06:07:16.672855 cds-python-sdk-0.13/cds_python_sdk.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-14 06:07:16.000000 cds-python-sdk-0.13/cds_python_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 06:07:16.676268 cds-python-sdk-0.13/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-06-14 06:07:11.000000 cds-python-sdk-0.13/setup.py
```

### Comparing `cds-python-sdk-0.11/LICENSE` & `cds-python-sdk-0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/README.md` & `cds-python-sdk-0.13/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -143,140 +143,159 @@
 000008e0: 616e 6365 2e63 6c69 656e 7420 696d 706f  ance.client impo
 000008f0: 7274 204e 6577 436c 6965 6e74 2c4e 6577  rt NewClient,New
 00000900: 4164 6449 6e73 7461 6e63 6552 6571 7565  AddInstanceReque
 00000910: 7374 0d0a 6672 6f6d 2063 6170 6974 616c  st..from capital
 00000920: 6f6e 6c69 6e65 2e69 6e73 7461 6e63 652e  online.instance.
 00000930: 6d6f 6465 6c73 2069 6d70 6f72 7420 4461  models import Da
 00000940: 7461 4469 736b 2c20 5072 6976 6174 6549  taDisk, PrivateI
-00000950: 702c 2053 7973 7465 6d44 6973 6b0d 0a61  p, SystemDisk..a
-00000960: 6b20 3d20 2727 0d0a 736b 203d 2027 270d  k = ''..sk = ''.
-00000970: 0a42 6569 6a69 6e67 5f72 6567 696f 6e20  .Beijing_region 
-00000980: 3d20 2742 6569 6a69 6e67 270d 0a0d 0a64  = 'Beijing'....d
-00000990: 6566 2054 6573 7443 6c69 656e 745f 4372  ef TestClient_Cr
-000009a0: 6561 7465 496e 7374 616e 6365 2829 3a0d  eateInstance():.
-000009b0: 0a20 2020 2023 2049 6e69 7420 6120 6372  .    # Init a cr
-000009c0: 6564 656e 7469 616c 2077 6974 6820 4163  edential with Ac
-000009d0: 6365 7373 204b 6579 2049 6420 616e 6420  cess Key Id and 
-000009e0: 5365 6372 6574 2041 6363 6573 7320 4b65  Secret Access Ke
-000009f0: 790d 0a20 2020 2023 2059 6f75 2063 616e  y..    # You can
-00000a00: 2061 7070 6c79 2074 6865 6d20 6672 6f6d   apply them from
-00000a10: 2074 6865 2043 4453 2077 6562 2070 6f72   the CDS web por
-00000a20: 7461 6c0d 0a20 2020 2023 696e 6974 2061  tal..    #init a
-00000a30: 2063 6c69 656e 740d 0a20 2020 2063 6c69   client..    cli
-00000a40: 656e 742c 2065 7272 203d 204e 6577 436c  ent, err = NewCl
-00000a50: 6965 6e74 2861 6b2c 2073 6b2c 2042 6569  ient(ak, sk, Bei
-00000a60: 6a69 6e67 5f72 6567 696f 6e29 0d0a 2020  jing_region)..  
-00000a70: 2020 6966 2065 7272 3a0d 0a20 2020 2020    if err:..     
-00000a80: 2020 2070 7269 6e74 2866 2741 5049 2072     print(f'API r
-00000a90: 6571 7565 7374 2066 6169 6c65 642c 6572  equest failed,er
-00000aa0: 723a 7b65 7272 7d27 290d 0a20 2020 2020  r:{err}')..     
-00000ab0: 2020 2072 6574 7572 6e0d 0a20 2020 2023     return..    #
-00000ac0: 696e 6974 2069 6e73 7461 6e63 6520 6461  init instance da
-00000ad0: 7461 0d0a 2020 2020 7265 7175 6573 7420  ta..    request 
-00000ae0: 3d20 4e65 7741 6464 496e 7374 616e 6365  = NewAddInstance
-00000af0: 5265 7175 6573 7428 290d 0a20 2020 2072  Request()..    r
-00000b00: 6571 7565 7374 2e52 6567 696f 6e49 6420  equest.RegionId 
-00000b10: 3d20 2743 4e5f 5368 616e 6768 6169 5f43  = 'CN_Shanghai_C
-00000b20: 2720 2020 2020 2020 2020 2372 6567 696f  '         #regio
-00000b30: 6e20 6964 206d 7573 7420 6265 2073 6574  n id must be set
-00000b40: 2e0d 0a20 2020 2072 6571 7565 7374 2e56  ...    request.V
-00000b50: 6463 4964 203d 2027 2720 2020 2020 2020  dcId = ''       
-00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2376 6463 2069 6420 6d75 7374 2062    #vdc id must b
-00000b80: 6520 7365 742e 0d0a 2020 2020 7265 7175  e set...    requ
-00000b90: 6573 742e 5061 7373 776f 7264 203d 2027  est.Password = '
-00000ba0: 2a2a 2a2a 2a2a 2a2a 2720 2020 2020 2020  ********'       
-00000bb0: 2020 2020 2020 2023 7061 7373 776f 7264         #password
-00000bc0: 206d 7573 7420 6265 2073 6574 2e0d 0a20   must be set... 
-00000bd0: 2020 2072 6571 7565 7374 2e49 6e73 7461     request.Insta
-00000be0: 6e63 654e 616d 6520 3d20 2774 6573 7431  nceName = 'test1
-00000bf0: 2720 2020 2020 2020 2020 2020 2020 2369  '             #i
-00000c00: 6e73 7461 6e63 6520 6e61 6d65 206d 7573  nstance name mus
-00000c10: 7420 6265 2073 6574 2e0d 0a20 2020 2072  t be set...    r
-00000c20: 6571 7565 7374 2e49 6e73 7461 6e63 6543  equest.InstanceC
-00000c30: 6861 7267 6554 7970 6520 3d20 2750 6f73  hargeType = 'Pos
-00000c40: 7450 6169 6427 0d0a 2020 2020 7265 7175  tPaid'..    requ
-00000c50: 6573 742e 4175 746f 5265 6e65 7720 3d20  est.AutoRenew = 
-00000c60: 300d 0a20 2020 2072 6571 7565 7374 2e43  0..    request.C
-00000c70: 7075 203d 2034 2020 2020 2020 2020 2020  pu = 4          
-00000c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c90: 2020 2363 7075 206d 7573 7420 6265 2073    #cpu must be s
-00000ca0: 6574 2e0d 0a20 2020 2072 6571 7565 7374  et...    request
-00000cb0: 2e52 616d 203d 2034 2020 2020 2020 2020  .Ram = 4        
-00000cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cd0: 2020 2020 2372 616d 206d 7573 7420 6265      #ram must be
-00000ce0: 2073 6574 2e0d 0a20 2020 2072 6571 7565   set...    reque
-00000cf0: 7374 2e49 6d61 6765 4964 203d 2027 4365  st.ImageId = 'Ce
-00000d00: 6e74 6f73 5f37 2e36 5f36 3427 0d0a 2020  ntos_7.6_64'..  
-00000d10: 2020 7265 7175 6573 742e 5075 626c 6963    request.Public
-00000d20: 4970 203d 205b 2761 7574 6f27 5d0d 0a20  Ip = ['auto'].. 
-00000d30: 2020 2072 6571 7565 7374 2e49 6e73 7461     request.Insta
-00000d40: 6e63 6554 7970 6520 3d20 2743 4353 2e49  nceType = 'CCS.I
-00000d50: 4333 5632 2720 2020 2020 2020 2020 2369  C3V2'         #i
-00000d60: 6e73 7461 6e63 6520 7479 7065 206d 7573  nstance type mus
-00000d70: 7420 6265 2073 6574 2e0d 0a20 2020 2072  t be set...    r
-00000d80: 6571 7565 7374 2e55 5443 203d 2046 616c  equest.UTC = Fal
-00000d90: 7365 0d0a 0d0a 2020 2020 6464 3120 3d20  se....    dd1 = 
-00000da0: 4461 7461 4469 736b 2829 0d0a 2020 2020  DataDisk()..    
-00000db0: 6464 312e 5369 7a65 203d 2032 3030 0d0a  dd1.Size = 200..
-00000dc0: 2020 2020 6464 312e 5479 7065 203d 2027      dd1.Type = '
-00000dd0: 6869 6768 5f64 6973 6b27 0d0a 0d0a 2020  high_disk'....  
-00000de0: 2020 6970 3120 3d20 5072 6976 6174 6549    ip1 = PrivateI
-00000df0: 7028 290d 0a20 2020 2069 7031 2e50 7269  p()..    ip1.Pri
-00000e00: 7661 7465 4964 203d 2027 2720 2020 2020  vateId = ''     
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 2369 6620 7365 7420 7072 6976      #if set priv
-00000e30: 6174 6520 6970 2c20 7072 6976 6174 6520  ate ip, private 
-00000e40: 6964 206d 7573 7420 6265 2073 6574 2e0d  id must be set..
-00000e50: 0a20 2020 2069 7031 2e49 5020 3d20 5b27  .    ip1.IP = ['
-00000e60: 6175 746f 275d 0d0a 0d0a 2020 2020 7265  auto']....    re
-00000e70: 7175 6573 742e 4461 7461 4469 736b 7320  quest.DataDisks 
-00000e80: 3d20 5b64 6431 5d0d 0a20 2020 2072 6571  = [dd1]..    req
-00000e90: 7565 7374 2e50 7269 7661 7465 4970 203d  uest.PrivateIp =
-00000ea0: 205b 6970 315d 0d0a 0d0a 2020 2020 7379   [ip1]....    sy
-00000eb0: 7374 656d 5f64 6973 6b20 3d20 5379 7374  stem_disk = Syst
-00000ec0: 656d 4469 736b 2829 0d0a 2020 2020 7379  emDisk()..    sy
-00000ed0: 7374 656d 5f64 6973 6b2e 494f 5053 203d  stem_disk.IOPS =
-00000ee0: 2035 0d0a 2020 2020 7379 7374 656d 5f64   5..    system_d
-00000ef0: 6973 6b2e 5369 7a65 203d 2032 300d 0a20  isk.Size = 20.. 
-00000f00: 2020 2073 7973 7465 6d5f 6469 736b 2e54     system_disk.T
-00000f10: 7970 6520 3d20 2773 7364 5f73 7973 7465  ype = 'ssd_syste
-00000f20: 6d5f 6469 736b 270d 0a0d 0a20 2020 2072  m_disk'....    r
-00000f30: 6571 7565 7374 2e53 7973 7465 6d44 6973  equest.SystemDis
-00000f40: 6b20 3d20 7379 7374 656d 5f64 6973 6b0d  k = system_disk.
-00000f50: 0a20 2020 2023 2073 656e 6420 7265 7175  .    # send requ
-00000f60: 6573 7420 6765 7420 7265 7370 6f6e 7365  est get response
-00000f70: 2e0d 0a20 2020 2072 6573 702c 2065 7272  ...    resp, err
-00000f80: 203d 2063 6c69 656e 742e 4372 6561 7465   = client.Create
-00000f90: 496e 7374 616e 6365 2872 6571 7565 7374  Instance(request
-00000fa0: 2920 2020 200d 0a20 2020 2070 7269 6e74  )    ..    print
-00000fb0: 2866 2743 7265 6174 6520 696e 7374 616e  (f'Create instan
-00000fc0: 6365 2072 6573 706f 6e73 653a 7b72 6573  ce response:{res
-00000fd0: 707d 2c20 6572 723a 7b65 7272 7d27 290d  p}, err:{err}').
-00000fe0: 0a20 2020 200d 0a69 6620 5f5f 6e61 6d65  .    ..if __name
-00000ff0: 5f5f 203d 3d20 275f 5f6d 6169 6e5f 5f27  __ == '__main__'
-00001000: 3a0d 0a20 2020 2054 6573 7443 6c69 656e  :..    TestClien
-00001010: 745f 4372 6561 7465 496e 7374 616e 6365  t_CreateInstance
-00001020: 2829 0d0a 6060 600d 0a0d 0a23 2320 436f  ()..```....## Co
-00001030: 6e74 7269 6275 7469 6e67 0d0a 0d0a 5765  ntributing....We
-00001040: 2077 6f72 6b20 6861 7264 2074 6f20 7072   work hard to pr
-00001050: 6f76 6964 6520 6120 6869 6768 2d71 7561  ovide a high-qua
-00001060: 6c69 7479 2061 6e64 2075 7365 6675 6c20  lity and useful 
-00001070: 5344 4b20 666f 7220 4361 7069 7461 6c4f  SDK for CapitalO
-00001080: 6e6c 696e 6520 436c 6f75 642c 2061 6e64  nline Cloud, and
-00001090: 2077 6520 6772 6561 746c 7920 7661 6c75   we greatly valu
-000010a0: 6520 6665 6564 6261 636b 2061 6e64 2063  e feedback and c
-000010b0: 6f6e 7472 6962 7574 696f 6e73 2066 726f  ontributions fro
-000010c0: 6d20 6f75 7220 636f 6d6d 756e 6974 792e  m our community.
-000010d0: 2050 6c65 6173 6520 7375 626d 6974 2079   Please submit y
-000010e0: 6f75 7220 6973 7375 6573 206f 7220 7075  our issues or pu
-000010f0: 6c6c 2072 6571 7565 7374 7320 7468 726f  ll requests thro
-00001100: 7567 6820 4769 7448 7562 2e0d 0a0d 0a23  ugh GitHub.....#
-00001110: 2320 5265 6665 7265 6e63 6573 0d0a 0d0a  # References....
-00001120: 2d20 5b43 4453 204f 7065 6e41 5049 2045  - [CDS OpenAPI E
-00001130: 7870 6c6f 7265 725d 2868 7474 7073 3a2f  xplorer](https:/
-00001140: 2f67 6974 6875 622e 636f 6d2f 6361 7069  /github.com/capi
-00001150: 7461 6c6f 6e6c 696e 652f 6f70 656e 6170  talonline/openap
-00001160: 6929 0d0a 0d0a 2323 204c 6963 656e 7365  i)....## License
-00001170: 0d0a 0d0a 5b41 7061 6368 6520 4c69 6365  ....[Apache Lice
-00001180: 6e73 6520 7632 2e30 5d28 2e2f 4c49 4345  nse v2.0](./LICE
-00001190: 4e53 4529                                NSE)
+00000950: 702c 2053 7973 7465 6d44 6973 6b2c 204f  p, SystemDisk, O
+00000960: 7264 6572 6564 4950 0d0a 616b 203d 2027  rderedIP..ak = '
+00000970: 270d 0a73 6b20 3d20 2727 0d0a 4265 696a  '..sk = ''..Beij
+00000980: 696e 675f 7265 6769 6f6e 203d 2027 4265  ing_region = 'Be
+00000990: 696a 696e 6727 0d0a 0d0a 6465 6620 5465  ijing'....def Te
+000009a0: 7374 436c 6965 6e74 5f43 7265 6174 6549  stClient_CreateI
+000009b0: 6e73 7461 6e63 6528 293a 0d0a 2020 2020  nstance():..    
+000009c0: 2320 496e 6974 2061 2063 7265 6465 6e74  # Init a credent
+000009d0: 6961 6c20 7769 7468 2041 6363 6573 7320  ial with Access 
+000009e0: 4b65 7920 4964 2061 6e64 2053 6563 7265  Key Id and Secre
+000009f0: 7420 4163 6365 7373 204b 6579 0d0a 2020  t Access Key..  
+00000a00: 2020 2320 596f 7520 6361 6e20 6170 706c    # You can appl
+00000a10: 7920 7468 656d 2066 726f 6d20 7468 6520  y them from the 
+00000a20: 4344 5320 7765 6220 706f 7274 616c 0d0a  CDS web portal..
+00000a30: 2020 2020 2369 6e69 7420 6120 636c 6965      #init a clie
+00000a40: 6e74 0d0a 2020 2020 636c 6965 6e74 2c20  nt..    client, 
+00000a50: 6572 7220 3d20 4e65 7743 6c69 656e 7428  err = NewClient(
+00000a60: 616b 2c20 736b 2c20 4265 696a 696e 675f  ak, sk, Beijing_
+00000a70: 7265 6769 6f6e 290d 0a20 2020 2069 6620  region)..    if 
+00000a80: 6572 723a 0d0a 2020 2020 2020 2020 7072  err:..        pr
+00000a90: 696e 7428 6627 4150 4920 7265 7175 6573  int(f'API reques
+00000aa0: 7420 6661 696c 6564 2c65 7272 3a7b 6572  t failed,err:{er
+00000ab0: 727d 2729 0d0a 2020 2020 2020 2020 7265  r}')..        re
+00000ac0: 7475 726e 0d0a 2020 2020 2369 6e69 7420  turn..    #init 
+00000ad0: 696e 7374 616e 6365 2064 6174 610d 0a20  instance data.. 
+00000ae0: 2020 2072 6571 7565 7374 203d 204e 6577     request = New
+00000af0: 4164 6449 6e73 7461 6e63 6552 6571 7565  AddInstanceReque
+00000b00: 7374 2829 0d0a 2020 2020 7265 7175 6573  st()..    reques
+00000b10: 742e 5265 6769 6f6e 4964 203d 2027 434e  t.RegionId = 'CN
+00000b20: 5f53 6861 6e67 6861 695f 4327 2020 2020  _Shanghai_C'    
+00000b30: 2020 2020 2023 7265 6769 6f6e 2069 6420       #region id 
+00000b40: 6d75 7374 2062 6520 7365 742e 0d0a 2020  must be set...  
+00000b50: 2020 7265 7175 6573 742e 5664 6349 6420    request.VdcId 
+00000b60: 3d20 2727 2020 2020 2020 2020 2020 2020  = ''            
+00000b70: 2020 2020 2020 2020 2020 2020 2023 7664               #vd
+00000b80: 6320 6964 206d 7573 7420 6265 2073 6574  c id must be set
+00000b90: 2e0d 0a20 2020 2072 6571 7565 7374 2e50  ...    request.P
+00000ba0: 6173 7377 6f72 6420 3d20 272a 2a2a 2a2a  assword = '*****
+00000bb0: 2a2a 2a27 2020 2020 2020 2020 2020 2020  ***'            
+00000bc0: 2020 2370 6173 7377 6f72 6420 6d75 7374    #password must
+00000bd0: 2062 6520 7365 742e 0d0a 2020 2020 7265   be set...    re
+00000be0: 7175 6573 742e 496e 7374 616e 6365 4e61  quest.InstanceNa
+00000bf0: 6d65 203d 2027 7465 7374 3127 2020 2020  me = 'test1'    
+00000c00: 2020 2020 2020 2020 2023 696e 7374 616e           #instan
+00000c10: 6365 206e 616d 6520 6d75 7374 2062 6520  ce name must be 
+00000c20: 7365 742e 0d0a 2020 2020 7265 7175 6573  set...    reques
+00000c30: 742e 496e 7374 616e 6365 4368 6172 6765  t.InstanceCharge
+00000c40: 5479 7065 203d 2027 506f 7374 5061 6964  Type = 'PostPaid
+00000c50: 270d 0a20 2020 2072 6571 7565 7374 2e41  '..    request.A
+00000c60: 7574 6f52 656e 6577 203d 2030 0d0a 2020  utoRenew = 0..  
+00000c70: 2020 7265 7175 6573 742e 4370 7520 3d20    request.Cpu = 
+00000c80: 3420 2020 2020 2020 2020 2020 2020 2020  4               
+00000c90: 2020 2020 2020 2020 2020 2020 2023 6370               #cp
+00000ca0: 7520 6d75 7374 2062 6520 7365 742e 0d0a  u must be set...
+00000cb0: 2020 2020 7265 7175 6573 742e 5261 6d20      request.Ram 
+00000cc0: 3d20 3420 2020 2020 2020 2020 2020 2020  = 4             
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000ce0: 7261 6d20 6d75 7374 2062 6520 7365 742e  ram must be set.
+00000cf0: 0d0a 2020 2020 7265 7175 6573 742e 496d  ..    request.Im
+00000d00: 6167 6549 6420 3d20 2743 656e 746f 735f  ageId = 'Centos_
+00000d10: 372e 365f 3634 270d 0a20 2020 2072 6571  7.6_64'..    req
+00000d20: 7565 7374 2e50 7562 6c69 6349 7020 3d20  uest.PublicIp = 
+00000d30: 5b27 6175 746f 275d 0d0a 2020 2020 7265  ['auto']..    re
+00000d40: 7175 6573 742e 496e 7374 616e 6365 5479  quest.InstanceTy
+00000d50: 7065 203d 2027 4343 532e 4943 3356 3227  pe = 'CCS.IC3V2'
+00000d60: 2020 2020 2020 2020 2023 696e 7374 616e           #instan
+00000d70: 6365 2074 7970 6520 6d75 7374 2062 6520  ce type must be 
+00000d80: 7365 742e 0d0a 2020 2020 7265 7175 6573  set...    reques
+00000d90: 742e 5554 4320 3d20 4661 6c73 650d 0a0d  t.UTC = False...
+00000da0: 0a20 2020 2064 6431 203d 2044 6174 6144  .    dd1 = DataD
+00000db0: 6973 6b28 290d 0a20 2020 2064 6431 2e53  isk()..    dd1.S
+00000dc0: 697a 6520 3d20 3230 300d 0a20 2020 2064  ize = 200..    d
+00000dd0: 6431 2e54 7970 6520 3d20 2768 6967 685f  d1.Type = 'high_
+00000de0: 6469 736b 270d 0a0d 0a20 2020 2069 7031  disk'....    ip1
+00000df0: 203d 2050 7269 7661 7465 4970 2829 0d0a   = PrivateIp()..
+00000e00: 2020 2020 6970 312e 5072 6976 6174 6549      ip1.PrivateI
+00000e10: 6420 3d20 2727 2020 2020 2020 2020 2020  d = ''          
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000e30: 6966 2073 6574 2070 7269 7661 7465 2069  if set private i
+00000e40: 702c 2070 7269 7661 7465 2069 6420 6d75  p, private id mu
+00000e50: 7374 2062 6520 7365 742e 0d0a 2020 2020  st be set...    
+00000e60: 6970 312e 4950 203d 205b 2761 7574 6f27  ip1.IP = ['auto'
+00000e70: 5d0d 0a0d 0a20 2020 2072 6571 7565 7374  ]....    request
+00000e80: 2e44 6174 6144 6973 6b73 203d 205b 6464  .DataDisks = [dd
+00000e90: 315d 0d0a 2020 2020 7265 7175 6573 742e  1]..    request.
+00000ea0: 5072 6976 6174 6549 7020 3d20 5b69 7031  PrivateIp = [ip1
+00000eb0: 5d0d 0a20 2020 200d 0a20 2020 206f 7264  ]..    ..    ord
+00000ec0: 6572 6564 5f69 7031 203d 204f 7264 6572  ered_ip1 = Order
+00000ed0: 6564 4950 2829 2020 2020 2020 2020 2020  edIP()          
+00000ee0: 2020 2020 2020 2020 2320 6966 2073 6574          # if set
+00000ef0: 206f 7264 6572 6564 2069 702c 2070 6970   ordered ip, pip
+00000f00: 6520 6964 206d 7573 7420 6265 2073 6574  e id must be set
+00000f10: 2e20 416e 6420 6966 2074 6869 7320 7061  . And if this pa
+00000f20: 7261 6d65 7465 7220 6973 2075 7365 642c  rameter is used,
+00000f30: 206f 7468 6572 2070 6172 616d 6574 6572   other parameter
+00000f40: 7328 7375 6368 2061 7320 5075 626c 6963  s(such as Public
+00000f50: 4970 204f 5220 5072 6976 6174 6549 7029  Ip OR PrivateIp)
+00000f60: 2064 6f20 6e6f 7420 7461 6b65 2065 6666   do not take eff
+00000f70: 6563 742e 0d0a 2020 2020 6f72 6465 7265  ect...    ordere
+00000f80: 645f 6970 312e 5069 7065 4964 203d 2027  d_ip1.PipeId = '
+00000f90: 270d 0a20 2020 206f 7264 6572 6564 5f69  '..    ordered_i
+00000fa0: 7031 2e49 5020 3d20 5b27 6175 746f 275d  p1.IP = ['auto']
+00000fb0: 0d0a 0d0a 2020 2020 7265 7175 6573 742e  ....    request.
+00000fc0: 4f72 6465 7265 6449 5020 3d20 5b6f 7264  OrderedIP = [ord
+00000fd0: 6572 6564 5f69 7031 5d0d 0a0d 0a20 2020  ered_ip1]....   
+00000fe0: 2073 7973 7465 6d5f 6469 736b 203d 2053   system_disk = S
+00000ff0: 7973 7465 6d44 6973 6b28 290d 0a20 2020  ystemDisk()..   
+00001000: 2073 7973 7465 6d5f 6469 736b 2e49 4f50   system_disk.IOP
+00001010: 5320 3d20 350d 0a20 2020 2073 7973 7465  S = 5..    syste
+00001020: 6d5f 6469 736b 2e53 697a 6520 3d20 3230  m_disk.Size = 20
+00001030: 0d0a 2020 2020 7379 7374 656d 5f64 6973  ..    system_dis
+00001040: 6b2e 5479 7065 203d 2027 7373 645f 7379  k.Type = 'ssd_sy
+00001050: 7374 656d 5f64 6973 6b27 0d0a 0d0a 2020  stem_disk'....  
+00001060: 2020 7265 7175 6573 742e 5379 7374 656d    request.System
+00001070: 4469 736b 203d 2073 7973 7465 6d5f 6469  Disk = system_di
+00001080: 736b 0d0a 2020 2020 2320 7365 6e64 2072  sk..    # send r
+00001090: 6571 7565 7374 2067 6574 2072 6573 706f  equest get respo
+000010a0: 6e73 652e 0d0a 2020 2020 7265 7370 2c20  nse...    resp, 
+000010b0: 6572 7220 3d20 636c 6965 6e74 2e43 7265  err = client.Cre
+000010c0: 6174 6549 6e73 7461 6e63 6528 7265 7175  ateInstance(requ
+000010d0: 6573 7429 2020 2020 0d0a 2020 2020 7072  est)    ..    pr
+000010e0: 696e 7428 6627 4372 6561 7465 2069 6e73  int(f'Create ins
+000010f0: 7461 6e63 6520 7265 7370 6f6e 7365 3a7b  tance response:{
+00001100: 7265 7370 7d2c 2065 7272 3a7b 6572 727d  resp}, err:{err}
+00001110: 2729 0d0a 2020 2020 0d0a 6966 205f 5f6e  ')..    ..if __n
+00001120: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
+00001130: 5f5f 273a 0d0a 2020 2020 5465 7374 436c  __':..    TestCl
+00001140: 6965 6e74 5f43 7265 6174 6549 6e73 7461  ient_CreateInsta
+00001150: 6e63 6528 290d 0a60 6060 0d0a 0d0a 2323  nce()..```....##
+00001160: 2043 6f6e 7472 6962 7574 696e 670d 0a0d   Contributing...
+00001170: 0a57 6520 776f 726b 2068 6172 6420 746f  .We work hard to
+00001180: 2070 726f 7669 6465 2061 2068 6967 682d   provide a high-
+00001190: 7175 616c 6974 7920 616e 6420 7573 6566  quality and usef
+000011a0: 756c 2053 444b 2066 6f72 2043 6170 6974  ul SDK for Capit
+000011b0: 616c 4f6e 6c69 6e65 2043 6c6f 7564 2c20  alOnline Cloud, 
+000011c0: 616e 6420 7765 2067 7265 6174 6c79 2076  and we greatly v
+000011d0: 616c 7565 2066 6565 6462 6163 6b20 616e  alue feedback an
+000011e0: 6420 636f 6e74 7269 6275 7469 6f6e 7320  d contributions 
+000011f0: 6672 6f6d 206f 7572 2063 6f6d 6d75 6e69  from our communi
+00001200: 7479 2e20 506c 6561 7365 2073 7562 6d69  ty. Please submi
+00001210: 7420 796f 7572 2069 7373 7565 7320 6f72  t your issues or
+00001220: 2070 756c 6c20 7265 7175 6573 7473 2074   pull requests t
+00001230: 6872 6f75 6768 2047 6974 4875 622e 0d0a  hrough GitHub...
+00001240: 0d0a 2323 2052 6566 6572 656e 6365 730d  ..## References.
+00001250: 0a0d 0a2d 205b 4344 5320 4f70 656e 4150  ...- [CDS OpenAP
+00001260: 4920 4578 706c 6f72 6572 5d28 6874 7470  I Explorer](http
+00001270: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00001280: 6170 6974 616c 6f6e 6c69 6e65 2f6f 7065  apitalonline/ope
+00001290: 6e61 7069 290d 0a0d 0a23 2320 4c69 6365  napi)....## Lice
+000012a0: 6e73 650d 0a0d 0a5b 4170 6163 6865 204c  nse....[Apache L
+000012b0: 6963 656e 7365 2076 322e 305d 282e 2f4c  icense v2.0](./L
+000012c0: 4943 454e 5345 29                        ICENSE)
```

### Comparing `cds-python-sdk-0.11/capitalonline/common/abstract_client.py` & `cds-python-sdk-0.13/capitalonline/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/client.py` & `cds-python-sdk-0.13/capitalonline/common/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/credential.py` & `cds-python-sdk-0.13/capitalonline/common/credential.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/exception/cds_sdk_exception.py` & `cds-python-sdk-0.13/capitalonline/common/exception/cds_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/http/request.py` & `cds-python-sdk-0.13/capitalonline/common/http/request.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/profile/client_profile.py` & `cds-python-sdk-0.13/capitalonline/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/profile/http_profile.py` & `cds-python-sdk-0.13/capitalonline/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/common/sign.py` & `cds-python-sdk-0.13/capitalonline/common/sign.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/haproxy/client.py` & `cds-python-sdk-0.13/capitalonline/haproxy/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/haproxy/client_test.py` & `cds-python-sdk-0.13/capitalonline/haproxy/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/haproxy/models.py` & `cds-python-sdk-0.13/capitalonline/haproxy/models.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/instance/client.py` & `cds-python-sdk-0.13/capitalonline/instance/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/instance/client_test.py` & `cds-python-sdk-0.13/capitalonline/instance/client_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from capitalonline.instance.client import NewClient, NewAddInstanceRequest, NewModifyInstanceNameRequest, \
     NewDescribeInstanceRequest, NewDeleteInstanceRequest, NewModifyInstanceSpecRequest, NewCreateDiskRequest, \
     NewResizeDiskRequest, NewDeleteDiskRequest, NewStartInstancesRequest, NewStopInstancesRequest, \
     NewRebootInstancesRequest, NewModifyIpRequest, NewExtendSystemDiskRequest, NewResetInstancesPasswordRequest, \
     NewResetImageRequest, NewModifyInstanceChargeTypeRequest
-from capitalonline.instance.models import DataDisk, PrivateIp, SystemDisk
+from capitalonline.instance.models import DataDisk, PrivateIp, SystemDisk, OrderedIP
 
 ak = ''
 sk = ''
 Beijing_region = 'Beijing'
 
 
 def TestClient_CreateInstance():
@@ -42,14 +42,24 @@
     ip1 = PrivateIp()
     ip1.PrivateId = ''                                     #if set private ip, private id must be set.
     ip1.IP = ['auto']
 
     request.DataDisks = [dd1]
     request.PrivateIp = [ip1]
 
+    ordered_ip1 = OrderedIP()                              # if set ordered ip, pipe id must be set. And if this parameter is used, other parameters(such as PublicIp OR PrivateIp) do not take effect.
+    ordered_ip1.PipeId = ''
+    ordered_ip1.IP = ['auto']
+
+    ordered_ip2 = OrderedIP()
+    ordered_ip2.PipeId = ''
+    ordered_ip2.IP = ['auto']
+
+    request.OrderedIP = [ordered_ip1] + [ordered_ip2]
+
     system_disk = SystemDisk()
     system_disk.IOPS = 5
     system_disk.Size = 20
     system_disk.Type = 'ssd_system_disk'
 
     request.SystemDisk = system_disk
     resp, err = client.CreateInstance(request)
```

### Comparing `cds-python-sdk-0.11/capitalonline/instance/models.py` & `cds-python-sdk-0.13/capitalonline/instance/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     AutoRenew: int
     PrepaidMonth: int
     _PublicIp = []
     Amount: int
     UTC: int
     ImagePassword: str
     _UserData = []
+    # 自定义排序网卡
+    _OrderedIP = []
 
     def __init__(self, service, version, action):
         super().__init__(service, version, action)
 
     def to_params(self):
         value = {}
         for k, v in self.__dict__.items():
@@ -54,25 +56,27 @@
             value['PrivateIp'] = self.PrivateIp
         if self._SystemDisk:
             value['SystemDisk'] = self.SystemDisk
         if self._PublicIp:
             value['PublicIp'] = self.PublicIp
         if self._UserData:
             value['UserData'] = self.UserData
+        if self._OrderedIP:
+            value['OrderedIP'] = self.OrderedIP
         return value
 
     @property
     def DataDisks(self):
         value = []
         for item in self._DataDisks:
             value.append(item.__dict__)
         return value
 
     @DataDisks.setter
-    def DataDisks(self, data: list):
+    def DataDisks(self, data: list):    
         self._DataDisks = data
 
     @property
     def PrivateIp(self):
         value = []
         for item in self._PrivateIp:
             value.append(item.__dict__)
@@ -107,14 +111,25 @@
             value.append(item.__dict__)
         return value
 
     @UserData.setter
     def UserData(self, user_data):
         self._UserData = user_data
 
+    @property
+    def OrderedIP(self):
+        value = []
+        for item in self._OrderedIP:
+            value.append(item.__dict__)
+        return value
+
+    @OrderedIP.setter
+    def OrderedIP(self, ordered_ips):
+        self._OrderedIP = ordered_ips
+
 
 class SystemDisk:
     Type: str
     IOPS: int
     Size: int
 
 
@@ -125,14 +140,19 @@
 
 
 class PrivateIp:
     PrivateId: str
     IP: list
 
 
+class OrderedIP:
+    PipeId: str
+    IP: list
+
+
 class DescribeInstanceRequest(BaseRequest):
     VdcId: str
     InstanceId: str
     PublicIp: list
     PageNumber: int
     PageSize: int
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cds-python-sdk-0.11/capitalonline/vdc/client.py` & `cds-python-sdk-0.13/capitalonline/vdc/client.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/vdc/client_test.py` & `cds-python-sdk-0.13/capitalonline/vdc/client_test.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/capitalonline/vdc/model.py` & `cds-python-sdk-0.13/capitalonline/vdc/model.py`

 * *Files identical despite different names*

### Comparing `cds-python-sdk-0.11/cds_python_sdk.egg-info/SOURCES.txt` & `cds-python-sdk-0.13/cds_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

