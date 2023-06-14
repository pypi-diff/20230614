# Comparing `tmp/eth-blocky-0.2.2.tar.gz` & `tmp/eth_blocky-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/vonum/code/eth-blocky/dist/tmp6i4idoj2/eth-blocky-0.2.2.tar", last modified: Tue May 10 10:38:16 2022, max compression
+gzip compressed data, was "eth_blocky-0.2.3.tar", max compression
```

## Comparing `eth-blocky-0.2.2.tar` & `eth_blocky-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,6 @@
-drwxr-xr-x   0 vonum      (501) staff       (20)        0 2022-05-10 10:38:16.634951 eth-blocky-0.2.2/
--rw-r--r--   0 vonum      (501) staff       (20)     2589 2022-05-10 10:38:16.634831 eth-blocky-0.2.2/PKG-INFO
--rw-r--r--   0 vonum      (501) staff       (20)     1724 2022-04-30 17:52:37.000000 eth-blocky-0.2.2/README.md
-drwxr-xr-x   0 vonum      (501) staff       (20)        0 2022-05-10 10:38:16.634060 eth-blocky-0.2.2/eth_blocky/
--rw-r--r--   0 vonum      (501) staff       (20)       57 2022-05-10 10:36:37.000000 eth-blocky-0.2.2/eth_blocky/__init__.py
--rw-r--r--   0 vonum      (501) staff       (20)     3919 2022-05-09 12:56:21.000000 eth-blocky-0.2.2/eth_blocky/eth_blocky.py
-drwxr-xr-x   0 vonum      (501) staff       (20)        0 2022-05-10 10:38:16.634669 eth-blocky-0.2.2/eth_blocky.egg-info/
--rw-r--r--   0 vonum      (501) staff       (20)     2589 2022-05-10 10:38:16.000000 eth-blocky-0.2.2/eth_blocky.egg-info/PKG-INFO
--rw-r--r--   0 vonum      (501) staff       (20)      235 2022-05-10 10:38:16.000000 eth-blocky-0.2.2/eth_blocky.egg-info/SOURCES.txt
--rw-r--r--   0 vonum      (501) staff       (20)        1 2022-05-10 10:38:16.000000 eth-blocky-0.2.2/eth_blocky.egg-info/dependency_links.txt
--rw-r--r--   0 vonum      (501) staff       (20)       26 2022-05-10 10:38:16.000000 eth-blocky-0.2.2/eth_blocky.egg-info/requires.txt
--rw-r--r--   0 vonum      (501) staff       (20)       11 2022-05-10 10:38:16.000000 eth-blocky-0.2.2/eth_blocky.egg-info/top_level.txt
--rw-r--r--   0 vonum      (501) staff       (20)       38 2022-05-10 10:38:16.634990 eth-blocky-0.2.2/setup.cfg
--rw-r--r--   0 vonum      (501) staff       (20)      709 2022-05-10 10:36:19.000000 eth-blocky-0.2.2/setup.py
+-rw-r--r--   0        0        0     1068 2022-04-19 14:45:07.343419 eth_blocky-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1724 2022-04-30 17:52:37.146028 eth_blocky-0.2.3/README.md
+-rw-r--r--   0        0        0       57 2023-06-14 14:34:48.687635 eth_blocky-0.2.3/eth_blocky/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-14 14:33:55.889507 eth_blocky-0.2.3/eth_blocky/eth_blocky.py
+-rw-r--r--   0        0        0      423 2023-06-14 14:42:23.860520 eth_blocky-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 eth_blocky-0.2.3/PKG-INFO
```

### Comparing `eth-blocky-0.2.2/PKG-INFO` & `eth_blocky-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 Metadata-Version: 2.1
 Name: eth-blocky
-Version: 0.2.2
-Summary: Ethereum utilities for mapping blocks to timestamps
-Home-page: https://github.com/vonum/eth-blocky
-Author: Milan Keca
+Version: 0.2.3
+Summary: 
+Author: vonum
 Author-email: vonum.mk@gmail.com
-License: UNKNOWN
-Description: # eth-blocky
-        [![Build Status](https://vonum.semaphoreci.com/badges/eth-blocky.svg)](https://vonum.semaphoreci.com/projects/eth-blocky)
-        [![PyPI version](https://badge.fury.io/py/eth-blocky.svg)](https://badge.fury.io/py/eth-blocky)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        Package providing date utilities for finding blocks.
-        
-        With `eth-blocky`, you can:
-        1. Find the closest block to a given timestamp that happened before
-        2. Find the closest block to a given timestamp that happened at the exact same
-           time or after
-        
-        ### Installation
-        1. `pip install eth-blocky`
-        
-        ### Usage
-        Provide a timestamp for which you want to find the closest block, and as a
-        result you will get the block object. For more information check out [web3
-        docs](https://web3py.readthedocs.io/en/stable/)
-        
-        ```Python
-        from eth_blocky import EthBlocky
-        
-        client = EthBlocky(NODE_URL)
-        
-        # 2021-03-11T12:00:00
-        timestamp = 1615464000
-        
-        block = client.closest_block(timestamp, before=True)
-        print(block.number)
-        # 12017166
-        
-        block = client.closest_block(timestamp)
-        print(block.number)
-        # 12017167
-        ```
-        
-        ### Method
-        `eth-blocky` works as an optimized binary search.
-        Start with finding the first and latest block as the boundry. Left and right
-        block.
-        
-        Steps:
-        1. Get left and right block and their timestamps
-        2. Calculate the average time for blocks to being mined in this time range
-        3. Estimate distance from start block based on timestamps [1, 3, 10] -> 0.3
-        4. Estimate wanted block based on distance
-        5. Calculate potential error
-        6. Repeat from step 1 with [estimated block - error, estimated block + error] as
-           the left and right block
-        
-        The process is repeated until left block is equal to right block.
-        
-Platform: UNKNOWN
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arrow (>=1.2.3,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Description-Content-Type: text/markdown
+
+# eth-blocky
+[![Build Status](https://vonum.semaphoreci.com/badges/eth-blocky.svg)](https://vonum.semaphoreci.com/projects/eth-blocky)
+[![PyPI version](https://badge.fury.io/py/eth-blocky.svg)](https://badge.fury.io/py/eth-blocky)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+Package providing date utilities for finding blocks.
+
+With `eth-blocky`, you can:
+1. Find the closest block to a given timestamp that happened before
+2. Find the closest block to a given timestamp that happened at the exact same
+   time or after
+
+### Installation
+1. `pip install eth-blocky`
+
+### Usage
+Provide a timestamp for which you want to find the closest block, and as a
+result you will get the block object. For more information check out [web3
+docs](https://web3py.readthedocs.io/en/stable/)
+
+```Python
+from eth_blocky import EthBlocky
+
+client = EthBlocky(NODE_URL)
+
+# 2021-03-11T12:00:00
+timestamp = 1615464000
+
+block = client.closest_block(timestamp, before=True)
+print(block.number)
+# 12017166
+
+block = client.closest_block(timestamp)
+print(block.number)
+# 12017167
+```
+
+### Method
+`eth-blocky` works as an optimized binary search.
+Start with finding the first and latest block as the boundry. Left and right
+block.
+
+Steps:
+1. Get left and right block and their timestamps
+2. Calculate the average time for blocks to being mined in this time range
+3. Estimate distance from start block based on timestamps [1, 3, 10] -> 0.3
+4. Estimate wanted block based on distance
+5. Calculate potential error
+6. Repeat from step 1 with [estimated block - error, estimated block + error] as
+   the left and right block
+
+The process is repeated until left block is equal to right block.
+
```

### Comparing `eth-blocky-0.2.2/README.md` & `eth_blocky-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `eth-blocky-0.2.2/eth_blocky/eth_blocky.py` & `eth_blocky-0.2.3/eth_blocky/eth_blocky.py`

 * *Files identical despite different names*

