# Comparing `tmp/devvio_util-1.5.3.tar.gz` & `tmp/devvio_util-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.3.tar", last modified: Fri Jun  9 02:51:03 2023, max compression
+gzip compressed data, was "devvio_util-1.5.4.tar", last modified: Wed Jun 14 01:07:21 2023, max compression
```

## Comparing `devvio_util-1.5.3.tar` & `devvio_util-1.5.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.498459 devvio_util-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 02:51:03.498459 devvio_util-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:50:54.000000 devvio_util-1.5.3/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.490459 devvio_util-1.5.3/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.494459 devvio_util-1.5.3/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-09 02:50:54.000000 devvio_util-1.5.3/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:51:03.490459 devvio_util-1.5.3/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-09 02:51:03.000000 devvio_util-1.5.3/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 02:51:03.498459 devvio_util-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 02:50:54.000000 devvio_util-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:07:21.519782 devvio_util-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:14.000000 devvio_util-1.5.4/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 01:07:21.523782 devvio_util-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 01:07:14.000000 devvio_util-1.5.4/setup.py
```

### Comparing `devvio_util-1.5.3/devvio_util/config.py` & `devvio_util-1.5.4/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/lib_creds.py` & `devvio_util-1.5.4/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/address.py` & `devvio_util-1.5.4/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.4/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.4/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/devv_sign.py` & `devvio_util-1.5.4/devvio_util/primitives/devv_sign.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/final_block.py` & `devvio_util-1.5.4/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/signature.py` & `devvio_util-1.5.4/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.4/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/summary.py` & `devvio_util-1.5.4/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/transaction.py` & `devvio_util-1.5.4/devvio_util/primitives/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
         if self._payload_size < kMIN_PAYLOAD_SIZE:
             raise ValueError(f"Failed to serialize transaction, payload too small ({self._payload_size})")
 
         self._canonical = bytes()
         self._canonical += set_uint64(self._payload_size)
 
-        if set_uint8(oper) >= OpType.NUM_OPS:
+        if oper >= OpType.NUM_OPS:
             raise ValueError(f"Invalid Transaction: bad OpType ({oper} >= {OpType.NUM_OPS})")
         self._canonical += set_uint8(oper)
         if flags != 0:
             raise ValueError("Invalid Transaction: unknown flags")
         self._canonical += set_uint8(flags)
         self._canonical += set_uint64(timestamp)
         self._canonical += signer.get_canonical()
```

### Comparing `devvio_util-1.5.3/devvio_util/primitives/transfer.py` & `devvio_util-1.5.4/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/utils.py` & `devvio_util-1.5.4/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/primitives/validation.py` & `devvio_util-1.5.4/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util/psql_mixin.py` & `devvio_util-1.5.4/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.3/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.4/devvio_util.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 devvio_util/config.py
 devvio_util/lib_creds.py
 devvio_util/psql_mixin.py
 devvio_util.egg-info/PKG-INFO
 devvio_util.egg-info/SOURCES.txt
 devvio_util.egg-info/dependency_links.txt
 devvio_util.egg-info/not-zip-safe
+devvio_util.egg-info/requires.txt
 devvio_util.egg-info/top_level.txt
 devvio_util/primitives/__init__.py
 devvio_util/primitives/address.py
 devvio_util/primitives/atomic_transaction_set.py
 devvio_util/primitives/chainstate.py
 devvio_util/primitives/devv_constants.py
 devvio_util/primitives/devv_sign.py
```

