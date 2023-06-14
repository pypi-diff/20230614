# Comparing `tmp/devvio_util-1.5.5.tar.gz` & `tmp/devvio_util-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.5.tar", last modified: Wed Jun 14 01:58:09 2023, max compression
+gzip compressed data, was "devvio_util-1.5.6.tar", last modified: Wed Jun 14 03:10:43 2023, max compression
```

## Comparing `devvio_util-1.5.5.tar` & `devvio_util-1.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.220946 devvio_util-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:58:09.220946 devvio_util-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:01.000000 devvio_util-1.5.5/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.216946 devvio_util-1.5.5/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.220946 devvio_util-1.5.5/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.216946 devvio_util-1.5.5/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 01:58:09.220946 devvio_util-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 01:58:01.000000 devvio_util-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 03:10:43.391799 devvio_util-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:35.000000 devvio_util-1.5.6/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 03:10:35.000000 devvio_util-1.5.6/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 03:10:43.391799 devvio_util-1.5.6/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 03:10:43.000000 devvio_util-1.5.6/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 03:10:43.395799 devvio_util-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 03:10:35.000000 devvio_util-1.5.6/setup.py
```

### Comparing `devvio_util-1.5.5/devvio_util/config.py` & `devvio_util-1.5.6/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/lib_creds.py` & `devvio_util-1.5.6/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/address.py` & `devvio_util-1.5.6/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.6/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.6/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/devv_sign.py` & `devvio_util-1.5.6/devvio_util/primitives/devv_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         return self._pk.decode('utf-8')[kPEM_PREFIX_SIZE:-kPEM_SUFFIX_SIZE].replace('\n', '')
 
     def get_pubkey(self) -> str:
         """
         :return: this EcSigner's public key as a hex string
         :rtype: str
         """
-        return self._pub.public_bytes(sz.Encoding.X962, sz.PublicFormat.CompressedPoint).hex()
+        return self._pub.public_bytes(sz.Encoding.X962, sz.PublicFormat.CompressedPoint).hex().upper()
 
     def get_signer_addr(self) -> Address:
         """
         :return: this EcSigner's public key as an Address object
         :rtype: Address
         """
         return Address(self.get_pubkey())
```

### Comparing `devvio_util-1.5.5/devvio_util/primitives/final_block.py` & `devvio_util-1.5.6/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/signature.py` & `devvio_util-1.5.6/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.6/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/summary.py` & `devvio_util-1.5.6/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/transaction.py` & `devvio_util-1.5.6/devvio_util/primitives/transaction.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/transfer.py` & `devvio_util-1.5.6/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/utils.py` & `devvio_util-1.5.6/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/primitives/validation.py` & `devvio_util-1.5.6/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util/psql_mixin.py` & `devvio_util-1.5.6/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.5/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.6/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

