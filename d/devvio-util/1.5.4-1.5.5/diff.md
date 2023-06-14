# Comparing `tmp/devvio_util-1.5.4.tar.gz` & `tmp/devvio_util-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.4.tar", last modified: Wed Jun 14 01:07:21 2023, max compression
+gzip compressed data, was "devvio_util-1.5.5.tar", last modified: Wed Jun 14 01:58:09 2023, max compression
```

## Comparing `devvio_util-1.5.4.tar` & `devvio_util-1.5.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:07:21.519782 devvio_util-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:14.000000 devvio_util-1.5.4/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 01:07:14.000000 devvio_util-1.5.4/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:07:21.519782 devvio_util-1.5.4/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:07:21.000000 devvio_util-1.5.4/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 01:07:21.523782 devvio_util-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 01:07:14.000000 devvio_util-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.220946 devvio_util-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:58:09.220946 devvio_util-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:01.000000 devvio_util-1.5.5/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.216946 devvio_util-1.5.5/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.220946 devvio_util-1.5.5/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-14 01:58:01.000000 devvio_util-1.5.5/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:58:09.216946 devvio_util-1.5.5/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 01:58:09.000000 devvio_util-1.5.5/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-14 01:58:09.220946 devvio_util-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-14 01:58:01.000000 devvio_util-1.5.5/setup.py
```

### Comparing `devvio_util-1.5.4/devvio_util/config.py` & `devvio_util-1.5.5/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/lib_creds.py` & `devvio_util-1.5.5/devvio_util/lib_creds.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/address.py` & `devvio_util-1.5.5/devvio_util/primitives/address.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.5/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.5/devvio_util/primitives/devv_constants.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/devv_sign.py` & `devvio_util-1.5.5/devvio_util/primitives/devv_sign.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/final_block.py` & `devvio_util-1.5.5/devvio_util/primitives/final_block.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/signature.py` & `devvio_util-1.5.5/devvio_util/primitives/signature.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.5/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/summary.py` & `devvio_util-1.5.5/devvio_util/primitives/summary.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/transaction.py` & `devvio_util-1.5.5/devvio_util/primitives/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,19 +195,22 @@
         :type flags: int
         :param timestamp: time of tx to be stored as an uint64
         :type timestamp: int
         :param sig: signature to assign to this transaction
         :type sig: Signature or str
         :param is_legacy: if True, will follow canonical patterns for legacy blocks
         :type is_legacy: bool
+        :return: the initialized Transaction object
+        :rtype: Transaction
         """
         self._is_legacy = is_legacy
         self._pre_signature_init(oper, self._signer, xfers, payload, flags, timestamp)
         if sig:
             self.set_sig(sig)
+        return self
 
     def set_sig(self, sig: Signature or str):
         """
         Add the given signature to the Transaction's current canonical form.
         If the Transaction is initialized with is_legacy = True, the signature size prefix will be excluded.
 
         :param sig: signature to assign to this transaction
@@ -248,14 +251,16 @@
         - 'flags': int
         - 'timestamp': int
         - (optional) 'sig': str
         - (optional) 'legacy': bool
 
         :param props: dict of transaction properties
         :type props: dict
+        :return: the initialized Transaction object
+        :rtype: Transaction
         """
         try:
             # construct xfers
             xfers = [Transfer(xfer) for xfer in props['xfers']]
             if not xfers:
                 raise Exception('Invalid Transaction: failed to parse any xfers')
             self._signer = None
@@ -277,15 +282,15 @@
                     raise Exception(f"Invalid Transaction: bad op string {props['op']}")
             elif props['op'] >= OpType.NUM_OPS:
                 raise Exception(f"Invalid Transaction: bad op int {props['op']}")
             else:
                 op = props['op']
 
             # initialize attributes and construct canonical
-            self.serialize(op, xfers, payload, props['flags'], props['timestamp'],
-                           sig=props.get('sig'), is_legacy=props.get('legacy'))
+            return self.serialize(op, xfers, payload, props['flags'], props['timestamp'],
+                                  sig=props.get('sig'), is_legacy=props.get('legacy'))
         except KeyError as ke:
             raise Exception(f"Invalid Transaction: failed to set property ({ke})")
 
     def get_signer(self) -> Address:
         return self._signer
```

### Comparing `devvio_util-1.5.4/devvio_util/primitives/transfer.py` & `devvio_util-1.5.5/devvio_util/primitives/transfer.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/utils.py` & `devvio_util-1.5.5/devvio_util/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/primitives/validation.py` & `devvio_util-1.5.5/devvio_util/primitives/validation.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util/psql_mixin.py` & `devvio_util-1.5.5/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.4/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.5/devvio_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

