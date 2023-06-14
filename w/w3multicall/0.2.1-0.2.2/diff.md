# Comparing `tmp/w3multicall-0.2.1.tar.gz` & `tmp/w3multicall-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3multicall-0.2.1.tar", last modified: Tue Jun 13 06:56:58 2023, max compression
+gzip compressed data, was "w3multicall-0.2.2.tar", last modified: Tue Jun 13 12:48:32 2023, max compression
```

## Comparing `w3multicall-0.2.1.tar` & `w3multicall-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 06:56:58.162139 w3multicall-0.2.1/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.2.1/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5407 2023-06-13 06:56:58.162139 w3multicall-0.2.1/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3704 2023-06-13 04:30:27.000000 w3multicall-0.2.1/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-13 06:56:50.000000 w3multicall-0.2.1/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-13 06:56:58.162139 w3multicall-0.2.1/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 06:56:58.162139 w3multicall-0.2.1/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 06:56:58.162139 w3multicall-0.2.1/src/w3multicall/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.2.1/src/w3multicall/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     6256 2023-06-13 01:16:16.000000 w3multicall-0.2.1/src/w3multicall/multicall.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 06:56:58.162139 w3multicall-0.2.1/src/w3multicall/threading/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.2.1/src/w3multicall/threading/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5034 2023-06-13 04:23:57.000000 w3multicall-0.2.1/src/w3multicall/threading/w3multicall_executor.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 06:56:58.162139 w3multicall-0.2.1/src/w3multicall/web3/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:22:07.000000 w3multicall-0.2.1/src/w3multicall/web3/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2769 2023-06-13 06:55:52.000000 w3multicall-0.2.1/src/w3multicall/web3/web3.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 06:56:58.162139 w3multicall-0.2.1/src/w3multicall.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5407 2023-06-13 06:56:58.000000 w3multicall-0.2.1/src/w3multicall.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      443 2023-06-13 06:56:58.000000 w3multicall-0.2.1/src/w3multicall.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-13 06:56:58.000000 w3multicall-0.2.1/src/w3multicall.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-13 06:56:58.000000 w3multicall-0.2.1/src/w3multicall.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-13 06:56:58.000000 w3multicall-0.2.1/src/w3multicall.egg-info/top_level.txt
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 12:48:32.303653 w3multicall-0.2.2/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.2.2/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5407 2023-06-13 12:48:32.303653 w3multicall-0.2.2/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3704 2023-06-13 04:30:27.000000 w3multicall-0.2.2/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-13 12:48:27.000000 w3multicall-0.2.2/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-13 12:48:32.303653 w3multicall-0.2.2/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 12:48:32.299653 w3multicall-0.2.2/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 12:48:32.299653 w3multicall-0.2.2/src/w3multicall/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.2.2/src/w3multicall/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     6266 2023-06-13 12:12:45.000000 w3multicall-0.2.2/src/w3multicall/multicall.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 12:48:32.299653 w3multicall-0.2.2/src/w3multicall/threading/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.2.2/src/w3multicall/threading/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5034 2023-06-13 04:23:57.000000 w3multicall-0.2.2/src/w3multicall/threading/w3multicall_executor.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 12:48:32.303653 w3multicall-0.2.2/src/w3multicall/web3/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:22:07.000000 w3multicall-0.2.2/src/w3multicall/web3/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3785 2023-06-13 12:47:46.000000 w3multicall-0.2.2/src/w3multicall/web3/web3.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 12:48:32.299653 w3multicall-0.2.2/src/w3multicall.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5407 2023-06-13 12:48:32.000000 w3multicall-0.2.2/src/w3multicall.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      443 2023-06-13 12:48:32.000000 w3multicall-0.2.2/src/w3multicall.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-13 12:48:32.000000 w3multicall-0.2.2/src/w3multicall.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-13 12:48:32.000000 w3multicall-0.2.2/src/w3multicall.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-13 12:48:32.000000 w3multicall-0.2.2/src/w3multicall.egg-info/top_level.txt
```

### Comparing `w3multicall-0.2.1/LICENSE` & `w3multicall-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `w3multicall-0.2.1/PKG-INFO` & `w3multicall-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
```

### Comparing `w3multicall-0.2.1/README.md` & `w3multicall-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `w3multicall-0.2.1/pyproject.toml` & `w3multicall-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "w3multicall"
 description = "Python interface and utilities for Solidity multicall contract"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 keywords = ["blockchain", "web3", "etherum", "solidity"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `w3multicall-0.2.1/setup.cfg` & `w3multicall-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = w3multicall
-version = 0.2.1
+version = 0.2.2
 author = Ortis
 author_email = ortis@ortis.io
 description = Python interface and utilities for Solidity multicall contract
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/w3multicall
 project_urls =
```

### Comparing `w3multicall-0.2.1/src/w3multicall/multicall.py` & `w3multicall-0.2.2/src/w3multicall/multicall.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,36 +124,36 @@
                 self.args = (args,)
             else:
                 self.args = args
             self.name, self.input_types, self.output_types = _parse_signature(signature)
             self.selector = eth_utils.function_signature_to_4byte_selector(self.name)
             self.data = _encode_data(self.selector, self.input_types, self.args)
 
-    def __init__(self, w3, address='0xcA11bde05977b3631167028862bE2a173976CA11', calls: List['W3Multicall.Call'] = None):
+    def __init__(self, web3, address='0xcA11bde05977b3631167028862bE2a173976CA11', calls: List['W3Multicall.Call'] = None):
         """
-        :param w3: Web3 instance
+        :param web3: Web3 instance
         :param address: (optional) address of the multicall3.sol contract
         :param calls: (optional) list of W3Multicall.Call to perform
         """
-        self.w3 = w3
+        self.web3 = web3
         self.address = address
         self.calls: List['W3Multicall.Call'] = [] if calls is None else calls.copy()
         self.require_success = True
 
     def add(self, call: 'W3Multicall.Call'):
         self.calls.append(call)
 
     def call(self) -> list:
         args = self._get_args()
         data = _encode_data(W3Multicall.MULTICALL_SELECTOR, W3Multicall.MULTICALL_INPUT_TYPES, args)
         eth_call_params = {
             'to': self.address,
             'data': data
         }
-        rpc_response = self.w3.eth.call(eth_call_params)
+        rpc_response = self.web3.eth.call(eth_call_params)
         aggregated = _decode_output(rpc_response, W3Multicall.MULTICALL_OUTPUT_TYPES)
         unpacked = _unpack_aggregate_outputs(aggregated[1])
         outputs = []
         for call, (success, output) in zip(self.calls, unpacked):
             call_output = _decode_output(output, call.output_types, None, True)
             outputs.append(call_output)
         return outputs
```

### Comparing `w3multicall-0.2.1/src/w3multicall/threading/w3multicall_executor.py` & `w3multicall-0.2.2/src/w3multicall/threading/w3multicall_executor.py`

 * *Files identical despite different names*

### Comparing `w3multicall-0.2.1/src/w3multicall/web3/web3.py` & `w3multicall-0.2.2/src/w3multicall/web3/web3.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,37 @@
         self.logger = logger
         self.lock = threading.RLock()
 
     def add_w3(self, w3: W3) -> 'W3Pool':
         self.w3s.append(w3)
         return self
 
+    def use_specific(self, w3_target: Union[W3, str], block: bool = True):
+        while True:
+            target = None
+            with self.lock:
+                for i in range(len(self.w3s)):
+                    if self.w3s[i] == w3_target or self.w3s[i].label == w3_target:
+                        tau = self.w3s[i].usable_in()
+                        if tau <= 0:
+                            if self.logger is not None:
+                                self.logger.debug("Using {}".format(self.w3s[i]))
+                            return self.w3s[i].use()
+                        target = self.w3s[i]
+                        break
+
+            if target is None:
+                raise Exception("Target w3 '{}' not found".format(w3_target))
+            if block:
+                sleep = target.usable_in()
+                if sleep > 0:
+                    if self.logger is not None:
+                        self.logger.warning("Waiting {}s for {}".format(sleep, target))
+                    time.sleep(sleep)
+
     def use(self, block: bool = True) -> Union[Web3, None]:
         """
         Return a Web3 instance that will not hit the rate limit upon calling (may block until the rate limit windows has passed)
         :param block: (default: true) block until a Web3 instance is available
         :return: Web3 instance
         """
```

### Comparing `w3multicall-0.2.1/src/w3multicall.egg-info/PKG-INFO` & `w3multicall-0.2.2/src/w3multicall.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
```

