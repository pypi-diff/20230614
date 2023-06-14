# Comparing `tmp/eversa-0.3.0-py3.10.egg` & `tmp/eversa-0.4.0-py3.10.egg`

## zipinfo {}

```diff
@@ -1,44 +1,44 @@
-Zip file size: 45376 bytes, number of entries: 42
--rw-r--r--  2.0 unx      594 b- defN 23-Jun-14 11:57 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      865 b- defN 23-Jun-14 11:57 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-14 11:57 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       48 b- defN 23-Jun-14 11:57 EGG-INFO/entry_points.txt
+Zip file size: 47500 bytes, number of entries: 42
+-rw-r--r--  2.0 unx      594 b- defN 23-Jun-14 18:22 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      865 b- defN 23-Jun-14 18:22 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-14 18:22 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-14 18:22 EGG-INFO/entry_points.txt
 -rw-r--r--  2.0 unx        1 b- defN 23-Jun-07 20:07 EGG-INFO/not-zip-safe
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-14 11:57 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-14 11:57 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx     1633 b- defN 23-Jun-09 00:11 eversa/.config.json.example
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-14 18:22 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-14 18:22 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx     1665 b- defN 23-Jun-14 15:53 eversa/.config.json.example
 -rw-r--r--  2.0 unx      324 b- defN 23-Jun-14 11:55 eversa/__init__.py
--rw-r--r--  2.0 unx     6266 b- defN 23-Jun-14 11:55 eversa/esa_cli.py
--rw-r--r--  2.0 unx     1527 b- defN 23-Jun-07 03:08 eversa/esa_config.py
+-rw-r--r--  2.0 unx     8234 b- defN 23-Jun-14 18:21 eversa/esa_cli.py
+-rw-r--r--  2.0 unx     1801 b- defN 23-Jun-14 18:09 eversa/esa_config.py
 -rw-r--r--  2.0 unx      619 b- defN 23-Jun-08 22:41 eversa/esa_constants.py
--rw-r--r--  2.0 unx    10657 b- defN 23-Jun-08 13:27 eversa/esa_contract.py
+-rw-r--r--  2.0 unx    10741 b- defN 23-Jun-14 17:34 eversa/esa_contract.py
 -rw-r--r--  2.0 unx     2119 b- defN 23-Jun-07 03:09 eversa/esa_graphql.py
 -rw-r--r--  2.0 unx     5636 b- defN 23-Jun-07 03:10 eversa/esa_lowlevel_bc.py
--rw-r--r--  2.0 unx     2962 b- defN 23-Jun-08 22:34 eversa/esa_lowlevel_util.py
+-rw-r--r--  2.0 unx     2962 b- defN 23-Jun-14 14:02 eversa/esa_lowlevel_util.py
 -rw-r--r--  2.0 unx     2970 b- defN 23-Jun-08 02:32 eversa/esa_return_values.py
--rw-r--r--  2.0 unx     5424 b- defN 23-Jun-14 11:55 eversa/eversa.py
--rw-r--r--  2.0 unx      439 b- defN 23-Jun-14 11:57 eversa/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     4633 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_cli.cpython-310.pyc
--rw-r--r--  2.0 unx     1067 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_config.cpython-310.pyc
--rw-r--r--  2.0 unx      619 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_constants.cpython-310.pyc
--rw-r--r--  2.0 unx     8533 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_contract.cpython-310.pyc
--rw-r--r--  2.0 unx     1800 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_graphql.cpython-310.pyc
--rw-r--r--  2.0 unx     3793 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_lowlevel_bc.cpython-310.pyc
--rw-r--r--  2.0 unx     3175 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_lowlevel_util.cpython-310.pyc
--rw-r--r--  2.0 unx     2692 b- defN 23-Jun-14 11:57 eversa/__pycache__/esa_return_values.cpython-310.pyc
--rw-r--r--  2.0 unx     5150 b- defN 23-Jun-14 11:57 eversa/__pycache__/eversa.cpython-310.pyc
+-rw-r--r--  2.0 unx     5485 b- defN 23-Jun-14 15:55 eversa/eversa.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Jun-14 18:22 eversa/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_cli.cpython-310.pyc
+-rw-r--r--  2.0 unx     1222 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_config.cpython-310.pyc
+-rw-r--r--  2.0 unx      619 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_constants.cpython-310.pyc
+-rw-r--r--  2.0 unx     8761 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_contract.cpython-310.pyc
+-rw-r--r--  2.0 unx     1800 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_graphql.cpython-310.pyc
+-rw-r--r--  2.0 unx     3793 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_lowlevel_bc.cpython-310.pyc
+-rw-r--r--  2.0 unx     3163 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_lowlevel_util.cpython-310.pyc
+-rw-r--r--  2.0 unx     2692 b- defN 23-Jun-14 18:22 eversa/__pycache__/esa_return_values.cpython-310.pyc
+-rw-r--r--  2.0 unx     5182 b- defN 23-Jun-14 18:22 eversa/__pycache__/eversa.cpython-310.pyc
 -rw-r--r--  2.0 unx      663 b- defN 23-Jun-07 15:10 eversa/bin/HighloadSinglesig.abi.json
 -rw-r--r--  2.0 unx      780 b- defN 23-Jun-07 15:10 eversa/bin/HighloadSinglesig.tvc
 -rw-r--r--  2.0 unx     3158 b- defN 23-Jun-07 15:11 eversa/bin/SafeMultisig.abi.json
 -rw-r--r--  2.0 unx     4352 b- defN 23-Jun-07 15:11 eversa/bin/SafeMultisig.tvc
 -rwxrwxrwx  2.0 unx     4155 b- defN 21-Oct-12 20:55 eversa/bin/SetcodeMultisig.abi.json
 -rwxrwxrwx  2.0 unx     6672 b- defN 21-Oct-12 20:55 eversa/bin/SetcodeMultisig.tvc
 -rwxr-xr-x  2.0 unx     4155 b- defN 23-Jun-07 15:15 eversa/bin/Surf.abi.json
 -rwxr-xr-x  2.0 unx     4800 b- defN 23-Jun-07 15:15 eversa/bin/Surf.tvc
 -rwxrwxrwx  2.0 unx      460 b- defN 21-Oct-12 20:55 eversa/bin/local_giver.abi.json
 -rw-r--r--  2.0 unx       26 b- defN 23-Jun-07 19:27 eversa/sample/.gitignore
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 18:44 eversa/sample/ISample.sol
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 18:44 eversa/sample/Sample.sol
--rw-r--r--  2.0 unx     1640 b- defN 23-Jun-14 11:55 eversa/sample/test.py
--rw-r--r--  2.0 unx      842 b- defN 23-Jun-14 11:57 eversa/sample/__pycache__/test.cpython-310.pyc
-42 files, 105287 bytes uncompressed, 39620 bytes compressed:  62.4%
+-rw-r--r--  2.0 unx     2004 b- defN 23-Jun-14 15:11 eversa/sample/test.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jun-14 18:22 eversa/sample/__pycache__/test.cpython-310.pyc
+42 files, 110453 bytes uncompressed, 41744 bytes compressed:  62.2%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eversa
-Version: 0.3.0
+Version: 0.4.0
 Summary: Everscale/Venom rapid application development and testing tools.
 Home-page: https://github.com/SolderingArmor/eversa
 Author: Anton Platonov
 Author-email: anton@platonov.us
 License: MIT
 Keywords: ever everscale venom python package blockchain
 Platform: UNKNOWN
```

## eversa/.config.json.example

### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'giver_enabled'": "['local']"}*

```diff
@@ -62,10 +62,13 @@
             "giver": "",
             "name": "ton_mainnet",
             "phrase": "",
             "workchain": 0
         }
     ],
     "everdev": "everdev",
+    "giver_enabled": [
+        "local"
+    ],
     "source_dir": "contracts",
     "verbose": false
 }
```

## eversa/esa_cli.py

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
 
 import os
+import sys
 import argparse
 import json
 import shutil
+import imp
+from   io import StringIO 
 from   inspect import getmodule, getmembers, isfunction, signature
 from  .esa_lowlevel_util import generateRandomMnemonic, generateRandomSigner, saveSigner
 from  .eversa import eversa
 
 # ==============================================================================
 #
 parser = argparse.ArgumentParser(description="eversa CLI helps to automate building and testing Everscale/Venom smart contracts")
@@ -20,14 +23,15 @@
 parserBuild = subparsers.add_parser('build', help="TODO")
 parserBuild.add_argument('contracts', metavar='contracts', type=str, nargs='*', help='List of contract names to build')
 
 parserMeta = subparsers.add_parser('meta',  help="Show metadata/function list for a specific contract")
 parserMeta.add_argument('contracts', metavar='contracts', type=str, nargs='+', help='List of contract names to show metadta for')
 
 parserTest = subparsers.add_parser('test',  help="Run test script to test the contracts")
+parserTest.add_argument('environment', metavar='environment', type=str, nargs=1, help='Test environment (use a name from .config.json file), for example `local`')
 
 parserSeed = subparsers.add_parser('new-seed', help="Create a random seed phrase with an option to save it to file")
 parserSeed.add_argument('output', metavar='output', type=str, nargs='*', help='File name to save seed to')
 
 parserKeys = subparsers.add_parser('new-keys',  help="Create a random private/public keypair with an option to save it to file")
 parserKeys.add_argument('output', metavar='output', type=str, nargs='*', help='File name to save keys to')
 
@@ -109,16 +113,67 @@
                 continue
             if name == "deploy":
                 name = "constructor"
             print(f"    {name}{signature(func)}")
 
 # ==============================================================================
 #
+def getLibraryFunctions():
+    functionList = []
+    for (name, _func) in getmembers(sys.modules["eversa"], isfunction):
+        functionList.append(name)
+    return functionList
+
+def getPyFilesList(dir: str):
+    result = []
+    for file in os.listdir(dir):
+        # check only text files
+        if file.endswith('.py'):
+            result.append(file)
+    return result
+
+class Capturing(list):
+    def __enter__(self):
+        self._stdout = sys.stdout
+        sys.stdout = self._stringio = StringIO()
+        return self
+    def __exit__(self, *args):
+        self.extend(self._stringio.getvalue().splitlines())
+        del self._stringio # free up some memory
+        sys.stdout = self._stdout
+
 def runTest(args):
-    print("runTest")
+    # 1. parse environment for eversa to run tests in
+    esa = eversa(args.environment[0])
+
+    # 2. List all .py files in test directory
+    pyTestFiles = getPyFilesList(os.path.join(esa.WORK_DIR, "tests"))
+    pyToRun     = {}
+
+    # 3. Import each file as a separate module
+    for testFile in pyTestFiles:
+        pyToRun[testFile] = []
+        module = imp.load_source(f"esaTest_{testFile}", os.path.join(esa.WORK_DIR, "tests", testFile))
+        pyToRun[testFile] = []
+
+        functionsInEversa = getLibraryFunctions()
+
+        for (name, _func) in getmembers(module, isfunction):
+            if name in functionsInEversa:
+                continue
+            pyToRun[testFile].append(getattr(module, name))
+
+    for module in pyToRun:
+        for function in pyToRun[module]:
+            print(f"Running {module}:{function.__name__}:")
+            with Capturing() as output:
+                function(esa)
+            print("    OK")
+            # TODO: parse output for errors, or raise errors to catch here
+            # TODO: count tests, print summary at the end
 
 # ==============================================================================
 #
 def runSeed(args):
     if len(args.output) == 0:
         phrase = generateRandomMnemonic()
         print(phrase)
```

## eversa/esa_config.py

```diff
@@ -6,40 +6,43 @@
 from   tonclient.client import *
 from   tonclient.types  import *
 
 # ==============================================================================
 # 
 class EsaConfig(object):
     def __init__(self, target: str):
-        self.EVERDEV    = ""
-        self.SOURCE_DIR = ""
-        self.BIN_DIR    = ""
-        self.VERBOSE    = False
-        self.NAME       = ""
-        self.ENDPOINTS  = [""]
-        self.WORKCHAIN  = 0
-        self.GIVER      = ""
-        self.PHRASE     = ""
+        self.EVERDEV       = ""
+        self.SOURCE_DIR    = ""
+        self.BIN_DIR       = ""
+        self.VERBOSE       = False
+        self.NAME          = ""
+        self.ENDPOINTS     = [""]
+        self.WORKCHAIN     = 0
+        self.GIVER         = ""
+        self.GIVER_ENABLED = False
+        self.PHRASE        = ""
 
         # TODO: check if config exists and give a graceful error throw
 
         with open('.config.json') as jsonConfig:
             config = json.load(jsonConfig)
 
             # Project-wide config
-            self.EVERDEV    = config["everdev"]
-            self.SOURCE_DIR = config["source_dir"]
-            self.BIN_DIR    = config["bin_dir"]
-            self.VERBOSE    = config["verbose"]
+            self.EVERDEV       = config["everdev"]
+            self.SOURCE_DIR    = config["source_dir"]
+            self.BIN_DIR       = config["bin_dir"]
+            self.VERBOSE       = config["verbose"]
+            self.GIVER_ENABLED = target in config["giver_enabled"]
 
             # Target-wide config
             for configElm in config["configs"]:
                 if configElm["name"] == target:
                     self.NAME       = configElm["name"]
                     self.ENDPOINTS  = configElm["endpoints"]
                     self.WORKCHAIN  = configElm["workchain"]
                     self.GIVER      = configElm["giver"]
                     self.PHRASE     = configElm["phrase"]
-                    break
+                    return
+            raise BaseException(f"Invalid configuration target: {target}!\nPlease use valid configuration name from .config.json!")
 
 # ==============================================================================
 #
```

## eversa/esa_contract.py

```diff
@@ -219,10 +219,16 @@
         `0` - uninit.
         `1` - active.
         `2` - frozen.
         `3` - nonExist.
         """
         result = self.GRAPHQL.getAccountGraphQL(accountID=self.ADDRESS, fields="acc_type")
         return int(result["acc_type"]) if result is not None else 0
+    
+    def getSalt():
+        pass # TODO
+
+    def setSalt():
+        pass # TODO
 
 # ==============================================================================
 #
```

## eversa/esa_lowlevel_util.py

```diff
@@ -67,16 +67,16 @@
             public=crypto.hdkey_public_from_xprv(params=ParamsOfHDKeyPublicFromXPrv(xprv=hdkey)).public
         )
         signer = Signer.Keys(keys=keypair)
         return signer
     except:
         raise "Invalid Mnemonic!"
 
-def saveSigner(filename: str, signer: Signer = generateRandomSigner()):
-    signer.keys.dump(filename, False)
+def saveSigner(keysFile: str, signer: Signer = generateRandomSigner()):
+    signer.keys.dump(keysFile, False)
 
 def loadSigner(keysFile=None) -> Signer:
     if keysFile is None:
         signer = Signer.External(ZERO_PUBKEY)
     else:
         signer = Signer.Keys(KeyPair.load(keysFile, False))
     return signer
```

## eversa/eversa.py

```diff
@@ -99,10 +99,12 @@
     def getEverClient(self):
         return TonClient(config=ClientConfig(network=NetworkConfig(endpoints=self.CONFIG.ENDPOINTS), abi=AbiConfig(workchain=self.CONFIG.WORKCHAIN)))
 
     def airdrop(self, contractAddress: str, value: int):
         """
         Top-up or fund or give native coin to a contract using Giver (currently works for local node only).
         """
+        if not self.CONFIG.GIVER_ENABLED:
+            return
         self.Log(f"eversa.airdrop(contractAddress: {contractAddress}, value: {value})")
         abiPath = self.findArtifact("local_giver", "abi.json")
         return callFunction(self.EVERCLIENT, abiPath, self.CONFIG.GIVER, "sendGrams", {"dest":contractAddress,"amount":value}, Signer.NoSigner())
```

## eversa/__pycache__/esa_cli.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 14 08:55:40 2023 UTC, .py size: 6266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,290 +1,395 @@
-00000000: 6f0d 0d0a 0000 0000 8c80 8964 7a18 0000  o..........dz...
+00000000: 6f0d 0d0a 0000 0000 e9da 8964 2a20 0000  o..........d* ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 ba01 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0073 1002 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
-00000050: 6402 6c04 6d05 5a05 6d06 5a06 6d07 5a07  d.l.m.Z.m.Z.m.Z.
-00000060: 6d08 5a08 0100 6403 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
-00000070: 6d0b 5a0b 6d0c 5a0c 0100 6403 6405 6c0d  m.Z.m.Z...d.d.l.
-00000080: 6d0d 5a0d 0100 6501 6a0e 6406 6407 8d01  m.Z...e.j.d.d...
-00000090: 5a0f 650f 6a10 6408 6409 640a 8d02 5a11  Z.e.j.d.d.d...Z.
-000000a0: 6511 6a12 640b 640c 640d 8d02 5a13 6513  e.j.d.d.d...Z.e.
-000000b0: 6a14 640e 640f 6410 6411 8d03 0100 6513  j.d.d.d.d.....e.
-000000c0: 6a14 6412 640f 6413 6411 8d03 0100 6511  j.d.d.d.d.....e.
-000000d0: 6a12 6414 6415 640d 8d02 5a15 6515 6a14  j.d.d.d...Z.e.j.
-000000e0: 6416 6416 6516 6417 6418 6419 8d05 0100  d.d.e.d.d.d.....
-000000f0: 6511 6a12 641a 641b 640d 8d02 5a17 6517  e.j.d.d.d...Z.e.
-00000100: 6a14 6416 6416 6516 641c 641d 6419 8d05  j.d.d.e.d.d.d...
-00000110: 0100 6511 6a12 641e 641f 640d 8d02 5a18  ..e.j.d.d.d...Z.
-00000120: 6511 6a12 6420 6421 640d 8d02 5a19 6519  e.j.d d!d...Z.e.
-00000130: 6a14 6422 6422 6516 6417 6423 6419 8d05  j.d"d"e.d.d#d...
-00000140: 0100 6511 6a12 6424 6425 640d 8d02 5a1a  ..e.j.d$d%d...Z.
-00000150: 651a 6a14 6422 6422 6516 6417 6426 6419  e.j.d"d"e.d.d&d.
-00000160: 8d05 0100 6427 6428 8400 5a1b 6429 642a  ....d'd(..Z.d)d*
-00000170: 8400 5a1c 642b 642c 8400 5a1d 642d 642e  ..Z.d+d,..Z.d-d.
-00000180: 8400 5a1e 642f 6430 8400 5a1f 6431 6432  ..Z.d/d0..Z.d1d2
-00000190: 8400 5a20 6513 6a21 651b 6433 8d01 0100  ..Z e.j!e.d3....
-000001a0: 6515 6a21 651c 6433 8d01 0100 6517 6a21  e.j!e.d3....e.j!
-000001b0: 651d 6433 8d01 0100 6518 6a21 651e 6433  e.d3....e.j!e.d3
-000001c0: 8d01 0100 6519 6a21 651f 6433 8d01 0100  ....e.j!e.d3....
-000001d0: 651a 6a21 6520 6433 8d01 0100 6434 6435  e.j!e d3....d4d5
-000001e0: 8400 5a22 6401 5300 2936 e900 0000 004e  ..Z"d.S.)6.....N
-000001f0: 2904 da09 6765 746d 6f64 756c 65da 0a67  )...getmodule..g
-00000200: 6574 6d65 6d62 6572 73da 0a69 7366 756e  etmembers..isfun
-00000210: 6374 696f 6eda 0973 6967 6e61 7475 7265  ction..signature
-00000220: e901 0000 0029 03da 1667 656e 6572 6174  .....)...generat
-00000230: 6552 616e 646f 6d4d 6e65 6d6f 6e69 63da  eRandomMnemonic.
-00000240: 1467 656e 6572 6174 6552 616e 646f 6d53  .generateRandomS
-00000250: 6967 6e65 72da 0a73 6176 6553 6967 6e65  igner..saveSigne
-00000260: 7229 01da 0665 7665 7273 617a 5165 7665  r)...eversazQeve
-00000270: 7273 6120 434c 4920 6865 6c70 7320 746f  rsa CLI helps to
-00000280: 2061 7574 6f6d 6174 6520 6275 696c 6469   automate buildi
-00000290: 6e67 2061 6e64 2074 6573 7469 6e67 2045  ng and testing E
-000002a0: 7665 7273 6361 6c65 2f56 656e 6f6d 2073  verscale/Venom s
-000002b0: 6d61 7274 2063 6f6e 7472 6163 7473 2901  mart contracts).
-000002c0: da0b 6465 7363 7269 7074 696f 6eda 0763  ..description..c
-000002d0: 6f6d 6d61 6e64 5429 02da 0464 6573 74da  ommandT)...dest.
-000002e0: 0872 6571 7569 7265 64da 0469 6e69 747a  .required..initz
-000002f0: 3a49 6e69 7469 616c 697a 6520 656d 7074  :Initialize empt
-00000300: 7920 7072 6f6a 6563 7420 7769 7468 2073  y project with s
-00000310: 616d 706c 6573 2069 6e20 6375 7272 656e  amples in curren
-00000320: 7420 6469 7265 6374 6f72 7929 01da 0468  t directory)...h
-00000330: 656c 707a 072d 2d66 6f72 6365 da0a 7374  elpz.--force..st
-00000340: 6f72 655f 7472 7565 7a33 4669 7273 6520  ore_truez3Firse 
-00000350: 696e 6974 6961 6c69 7a61 7469 6f6e 2065  initialization e
-00000360: 7665 6e20 6966 2064 6972 6563 746f 7279  ven if directory
-00000370: 2069 7320 6e6f 7420 656d 7074 7929 02da   is not empty)..
-00000380: 0661 6374 696f 6e72 1000 0000 7a0b 2d2d  .actionr....z.--
-00000390: 6e6f 2d73 616d 706c 657a 1c44 6f20 6e6f  no-samplez.Do no
-000003a0: 7420 636f 7079 2061 6e79 2073 616d 706c  t copy any sampl
-000003b0: 6520 6669 6c65 73da 0562 7569 6c64 da04  e files..build..
-000003c0: 544f 444f da09 636f 6e74 7261 6374 73da  TODO..contracts.
-000003d0: 012a 7a1f 4c69 7374 206f 6620 636f 6e74  .*z.List of cont
-000003e0: 7261 6374 206e 616d 6573 2074 6f20 6275  ract names to bu
-000003f0: 696c 6429 04da 076d 6574 6176 6172 da04  ild)...metavar..
-00000400: 7479 7065 da05 6e61 7267 7372 1000 0000  type..nargsr....
-00000410: da04 6d65 7461 7a33 5368 6f77 206d 6574  ..metaz3Show met
-00000420: 6164 6174 612f 6675 6e63 7469 6f6e 206c  adata/function l
-00000430: 6973 7420 666f 7220 6120 7370 6563 6966  ist for a specif
-00000440: 6963 2063 6f6e 7472 6163 74fa 012b 7a2a  ic contract..+z*
-00000450: 4c69 7374 206f 6620 636f 6e74 7261 6374  List of contract
-00000460: 206e 616d 6573 2074 6f20 7368 6f77 206d   names to show m
-00000470: 6574 6164 7461 2066 6f72 da04 7465 7374  etadta for..test
-00000480: 7a25 5275 6e20 7465 7374 2073 6372 6970  z%Run test scrip
-00000490: 7420 746f 2074 6573 7420 7468 6520 636f  t to test the co
-000004a0: 6e74 7261 6374 737a 086e 6577 2d73 6565  ntractsz.new-see
-000004b0: 647a 3d43 7265 6174 6520 6120 7261 6e64  dz=Create a rand
-000004c0: 6f6d 2073 6565 6420 7068 7261 7365 2077  om seed phrase w
-000004d0: 6974 6820 616e 206f 7074 696f 6e20 746f  ith an option to
-000004e0: 2073 6176 6520 6974 2074 6f20 6669 6c65   save it to file
-000004f0: da06 6f75 7470 7574 7a19 4669 6c65 206e  ..outputz.File n
-00000500: 616d 6520 746f 2073 6176 6520 7365 6564  ame to save seed
-00000510: 2074 6f7a 086e 6577 2d6b 6579 737a 4843   toz.new-keyszHC
-00000520: 7265 6174 6520 6120 7261 6e64 6f6d 2070  reate a random p
-00000530: 7269 7661 7465 2f70 7562 6c69 6320 6b65  rivate/public ke
-00000540: 7970 6169 7220 7769 7468 2061 6e20 6f70  ypair with an op
-00000550: 7469 6f6e 2074 6f20 7361 7665 2069 7420  tion to save it 
-00000560: 746f 2066 696c 657a 1946 696c 6520 6e61  to filez.File na
-00000570: 6d65 2074 6f20 7361 7665 206b 6579 7320  me to save keys 
-00000580: 746f 6301 0000 0000 0000 0000 0000 0008  toc.............
-00000590: 0000 0009 0000 0043 0000 0073 5202 0000  .......C...sR...
-000005a0: 7400 6401 8301 0100 7c00 6a01 0100 7c00  t.d.....|.j...|.
-000005b0: 6a02 0100 7403 a004 a100 7d01 7403 6a05  j...t.....}.t.j.
-000005c0: a006 7403 6a05 a007 7408 a101 a101 7d02  ..t.j...t.....}.
-000005d0: 7409 7403 a00a 7c01 a101 8301 6402 6b01  t.t...|.....d.k.
-000005e0: 7d03 7c03 732c 7c00 6a01 732c 7400 6403  }.|.s,|.j.s,t.d.
-000005f0: 8301 0100 6400 5300 7a0c 7403 a00b 7403  ....d.S.z.t...t.
-00000600: 6a05 a00c 7c01 6404 a102 a101 0100 5700  j...|.d.......W.
-00000610: 6e09 0400 740d 7941 0100 0100 0100 5900  n...t.yA......Y.
-00000620: 6e01 7700 7a0c 7403 a00b 7403 6a05 a00c  n.w.z.t...t.j...
-00000630: 7c01 6405 a102 a101 0100 5700 6e09 0400  |.d.......W.n...
-00000640: 740d 7957 0100 0100 0100 5900 6e01 7700  t.yW......Y.n.w.
-00000650: 7a0c 7403 a00b 7403 6a05 a00c 7c01 6406  z.t...t.j...|.d.
-00000660: a102 a101 0100 5700 6e09 0400 740d 796d  ......W.n...t.ym
-00000670: 0100 0100 0100 5900 6e01 7700 7a0c 7403  ......Y.n.w.z.t.
-00000680: a00b 7403 6a05 a00c 7c01 6407 a102 a101  ..t.j...|.d.....
-00000690: 0100 5700 6e09 0400 740d 7983 0100 0100  ..W.n...t.y.....
-000006a0: 0100 5900 6e01 7700 740e 7403 6a05 a00c  ..Y.n.w.t.t.j...
-000006b0: 7c02 6408 a102 8301 8f43 7d04 740f a010  |.d......C}.t...
-000006c0: 7c04 a101 7d05 7c05 6409 1900 4400 5d0f  |...}.|.d...D.].
-000006d0: 7d06 7c06 640a 1900 640b 6b02 72a6 7411  }.|.d...d.k.r.t.
-000006e0: 8300 7c06 640c 3c00 0100 6e01 7197 740e  ..|.d.<...n.q.t.
-000006f0: 7403 6a05 a00c 7c01 640d a102 640e 8302  t.j...|.d...d...
-00000700: 8f10 7d07 740f 6a12 7c05 7c07 640f 6410  ..}.t.j.|.|.d.d.
-00000710: 8d03 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000720: 6e08 3100 73c4 7701 0100 0100 0100 5900  n.1.s.w.......Y.
-00000730: 0100 5700 6400 0400 0400 8303 0100 6e08  ..W.d.........n.
-00000740: 3100 73d3 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
-00000750: 7c00 6a02 9001 7323 7413 a014 7403 6a05  |.j...s#t...t.j.
-00000760: a00c 7c02 6411 6412 a103 7403 6a05 a00c  ..|.d.d...t.j...
-00000770: 7c01 6406 6412 a103 a102 0100 7413 a014  |.d.d.......t...
-00000780: 7403 6a05 a00c 7c02 6411 6413 a103 7403  t.j...|.d.d...t.
-00000790: 6a05 a00c 7c01 6405 6413 a103 a102 0100  j...|.d.d.......
-000007a0: 7413 a014 7403 6a05 a00c 7c02 6411 6414  t...t.j...|.d.d.
-000007b0: a103 7403 6a05 a00c 7c01 6407 6414 a103  ..t.j...|.d.d...
-000007c0: a102 0100 7413 a014 7403 6a05 a00c 7c02  ....t...t.j...|.
-000007d0: 6411 6415 a103 7403 6a05 a00c 7c01 6415  d.d...t.j...|.d.
-000007e0: a102 a102 0100 7400 6416 8301 0100 6400  ......t.d.....d.
-000007f0: 5300 2917 4e7a 1649 6e69 7469 616c 697a  S.).Nz.Initializ
-00000800: 696e 6720 6576 6572 7361 2e2e 2e72 0100  ing eversa...r..
-00000810: 0000 7a5b 4572 726f 7221 2043 7572 7265  ..z[Error! Curre
-00000820: 6e74 2064 6972 6563 746f 7279 2069 7320  nt directory is 
-00000830: 6e6f 7420 656d 7074 7921 0a50 6c65 6173  not empty!.Pleas
-00000840: 6520 7573 6520 666c 6167 202d 2d66 6f72  e use flag --for
-00000850: 6365 2074 6f20 696e 6974 6961 6c69 7a65  ce to initialize
-00000860: 2065 7665 7273 6120 616e 7977 6179 2eda   eversa anyway..
-00000870: 0362 696e 7215 0000 00da 0a69 6e74 6572  .binr......inter
-00000880: 6661 6365 73da 0574 6573 7473 7a14 2e63  faces..testsz..c
-00000890: 6f6e 6669 672e 6a73 6f6e 2e65 7861 6d70  onfig.json.examp
-000008a0: 6c65 da07 636f 6e66 6967 73da 046e 616d  le..configs..nam
-000008b0: 65da 056c 6f63 616c da06 7068 7261 7365  e..local..phrase
-000008c0: 7a0c 2e63 6f6e 6669 672e 6a73 6f6e da01  z..config.json..
-000008d0: 77e9 0400 0000 2901 da06 696e 6465 6e74  w.....)...indent
-000008e0: da06 7361 6d70 6c65 7a0b 4953 616d 706c  ..samplez.ISampl
-000008f0: 652e 736f 6c7a 0a53 616d 706c 652e 736f  e.solz.Sample.so
-00000900: 6c7a 0774 6573 742e 7079 7a0a 2e67 6974  lz.test.pyz..git
-00000910: 6967 6e6f 7265 7a05 446f 6e65 2129 15da  ignorez.Done!)..
-00000920: 0570 7269 6e74 da05 666f 7263 65da 096e  .print..force..n
-00000930: 6f5f 7361 6d70 6c65 da02 6f73 da06 6765  o_sample..os..ge
-00000940: 7463 7764 da04 7061 7468 da07 6469 726e  tcwd..path..dirn
-00000950: 616d 65da 0872 6561 6c70 6174 68da 085f  ame..realpath.._
-00000960: 5f66 696c 655f 5fda 036c 656e da07 6c69  _file__..len..li
-00000970: 7374 6469 72da 056d 6b64 6972 da04 6a6f  stdir..mkdir..jo
-00000980: 696e da07 4f53 4572 726f 72da 046f 7065  in..OSError..ope
-00000990: 6eda 046a 736f 6eda 046c 6f61 6472 0700  n..json..loadr..
-000009a0: 0000 da04 6475 6d70 da06 7368 7574 696c  ....dump..shutil
-000009b0: da08 636f 7079 6669 6c65 2908 da04 6172  ..copyfile)...ar
-000009c0: 6773 da07 776f 726b 4469 72da 096d 6f64  gs..workDir..mod
-000009d0: 756c 6544 6972 da08 6469 7245 6d70 7479  uleDir..dirEmpty
-000009e0: da0a 6a73 6f6e 436f 6e66 6967 da06 636f  ..jsonConfig..co
-000009f0: 6e66 6967 da09 636f 6e66 6967 456c 6d72  nfig..configElmr
-00000a00: 1d00 0000 a900 7244 0000 00fa 2e62 7569  ......rD.....bui
-00000a10: 6c64 2f62 6469 7374 2e6c 696e 7578 2d78  ld/bdist.linux-x
-00000a20: 3836 5f36 342f 6567 672f 6576 6572 7361  86_64/egg/eversa
-00000a30: 2f65 7361 5f63 6c69 2e70 79da 0772 756e  /esa_cli.py..run
-00000a40: 496e 6974 2400 0000 735e 0000 0008 0106  Init$...s^......
-00000a50: 0106 0108 0114 0112 020a 0108 0104 0102  ................
-00000a60: 0318 010c 0104 0102 ff02 0218 010c 0104  ................
-00000a70: 0102 ff02 0218 010c 0104 0102 ff02 0218  ................
-00000a80: 010c 0104 0102 ff14 040a 010c 010c 010a  ................
-00000a90: 0104 0102 fe16 0312 011c ff02 801c fa08  ................
-00000aa0: 0a24 0124 0124 0122 010c 0272 4600 0000  .$.$.$."...rF...
-00000ab0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000ac0: 0005 0000 0043 0000 0073 3c00 0000 7400  .....C...s<...t.
-00000ad0: 6401 8301 0100 7c00 6a01 6400 7500 720c  d.....|.j.d.u.r.
-00000ae0: 6700 7d01 6e03 7c00 6a01 7d01 7c01 4400  g.}.n.|.j.}.|.D.
-00000af0: 5d0a 7d02 7400 6402 7c02 9b00 6403 9d03  ].}.t.d.|...d...
-00000b00: 8301 0100 7111 6400 5300 2904 4eda 0872  ....q.d.S.).N..r
-00000b10: 756e 4275 696c 647a 0a42 7569 6c64 696e  unBuildz.Buildin
-00000b20: 6720 22fa 0422 2e2e 2e29 0272 2900 0000  g ".."...).r)...
-00000b30: 7215 0000 0029 0372 3d00 0000 da0d 636f  r....).r=.....co
-00000b40: 6e74 7261 6374 734c 6973 74da 0863 6f6e  ntractsList..con
-00000b50: 7472 6163 7472 4400 0000 7244 0000 0072  tractrD...rD...r
-00000b60: 4500 0000 7247 0000 0057 0000 0073 1000  E...rG...W...s..
-00000b70: 0000 0801 0a01 0601 0602 0802 1001 0201  ................
-00000b80: 04fe 7247 0000 0063 0100 0000 0000 0000  ..rG...c........
-00000b90: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
-00000ba0: 7380 0000 0074 0083 007d 0174 0164 0183  s....t...}.t.d..
-00000bb0: 0101 007c 006a 0244 005d 337d 0274 019d  ...|.j.D.]3}.t..
-00000bc0: 0083 0101 0074 0164 027c 029b 0064 039d  .....t.d.|...d..
-00000bd0: 0383 0101 007c 01a0 037c 02a1 017d 0374  .....|...|...}.t
-00000be0: 047c 0374 0583 0244 005d 1a5c 027d 047d  .|.t...D.].\.}.}
-00000bf0: 057c 0464 046b 0272 2b71 227c 0464 056b  .|.d.k.r+q"|.d.k
-00000c00: 0272 3164 067d 0474 0164 077c 049b 0074  .r1d.}.t.d.|...t
-00000c10: 067c 0583 019b 009d 0383 0101 0071 2271  .|...........q"q
-00000c20: 0a64 0053 0029 084e 7a24 5368 6f77 696e  .d.S.).Nz$Showin
-00000c30: 6720 616c 6c20 6675 6e63 7469 6f6e 7320  g all functions 
-00000c40: 666f 7220 636f 6e74 7261 6374 733a fa01  for contracts:..
-00000c50: 227a 0222 3ada 1165 7361 5570 6461 7465  "z.":..esaUpdate
-00000c60: 496e 6974 4461 7461 da06 6465 706c 6f79  InitData..deploy
-00000c70: da0b 636f 6e73 7472 7563 746f 727a 0420  ..constructorz. 
-00000c80: 2020 2029 0772 0a00 0000 7229 0000 0072     ).r....r)...r
-00000c90: 1500 0000 da0b 4765 7443 6f6e 7472 6163  ......GetContrac
-00000ca0: 7472 0300 0000 7204 0000 0072 0500 0000  tr....r....r....
-00000cb0: 2906 723d 0000 00da 0365 7361 da0c 636f  ).r=.....esa..co
-00000cc0: 6e74 7261 6374 4e61 6d65 724a 0000 0072  ntractNamerJ...r
-00000cd0: 2200 0000 da04 6675 6e63 7244 0000 0072  ".....funcrD...r
-00000ce0: 4400 0000 7245 0000 00da 0772 756e 4d65  D...rE.....runMe
-00000cf0: 7461 6400 0000 731c 0000 0006 0108 010a  tad...s.........
-00000d00: 0108 0110 010a 0112 0108 0102 0108 0104  ................
-00000d10: 0118 0102 fb04 fc72 5300 0000 6301 0000  .......rS...c...
-00000d20: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00000d30: 0043 0000 0073 0c00 0000 7400 6401 8301  .C...s....t.d...
-00000d40: 0100 6400 5300 2902 4eda 0772 756e 5465  ..d.S.).N..runTe
-00000d50: 7374 2901 7229 0000 00a9 0172 3d00 0000  st).r).....r=...
-00000d60: 7244 0000 0072 4400 0000 7245 0000 0072  rD...rD...rE...r
-00000d70: 5400 0000 7400 0000 7302 0000 000c 0172  T...t...s......r
-00000d80: 5400 0000 6301 0000 0000 0000 0000 0000  T...c...........
-00000d90: 0005 0000 0009 0000 0043 0000 0073 7e00  .........C...s~.
-00000da0: 0000 7400 7c00 6a01 8301 6401 6b02 7210  ..t.|.j...d.k.r.
-00000db0: 7402 8300 7d01 7403 7c01 8301 0100 6400  t...}.t.|.....d.
-00000dc0: 5300 7c00 6a01 7d02 7c02 4400 5d27 7d03  S.|.j.}.|.D.]'}.
-00000dd0: 7403 6402 7c03 9b00 6403 9d03 8301 0100  t.d.|...d.......
-00000de0: 7402 8300 7d01 7404 7c03 6404 8302 8f0d  t...}.t.|.d.....
-00000df0: 7d04 7c04 a005 7c01 a101 0100 5700 6400  }.|...|.....W.d.
-00000e00: 0400 0400 8303 0100 6e08 3100 7337 7701  ........n.1.s7w.
-00000e10: 0100 0100 0100 5900 0100 7115 6400 5300  ......Y...q.d.S.
-00000e20: 2905 4e72 0100 0000 7a1e 5361 7669 6e67  ).Nr....z.Saving
-00000e30: 2072 616e 646f 6d20 7365 6564 2070 6872   random seed phr
-00000e40: 6173 6520 746f 2022 7248 0000 0072 2500  ase to "rH...r%.
-00000e50: 0000 2906 7232 0000 0072 1d00 0000 7207  ..).r2...r....r.
-00000e60: 0000 0072 2900 0000 7237 0000 00da 0577  ...r)...r7.....w
-00000e70: 7269 7465 2905 723d 0000 0072 2400 0000  rite).r=...r$...
-00000e80: da08 6669 6c65 4c69 7374 da04 6669 6c65  ..fileList..file
-00000e90: da01 6672 4400 0000 7244 0000 0072 4500  ..frD...rD...rE.
-00000ea0: 0000 da07 7275 6e53 6565 6479 0000 0073  ....runSeedy...s
-00000eb0: 1a00 0000 0e01 0601 0801 0401 0602 0801  ................
-00000ec0: 1001 0601 0c01 0c01 1cff 0280 04fd 725a  ..............rZ
-00000ed0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000ee0: 0400 0000 0500 0000 4300 0000 7358 0000  ........C...sX..
-00000ef0: 0074 007c 006a 0183 0164 016b 0272 1274  .t.|.j...d.k.r.t
-00000f00: 0283 007d 0174 037c 016a 046a 0583 0101  ...}.t.|.j.j....
-00000f10: 0064 0053 007c 006a 017d 027c 0244 005d  .d.S.|.j.}.|.D.]
-00000f20: 127d 0374 0364 027c 039b 0064 039d 0383  .}.t.d.|...d....
-00000f30: 0101 0074 0283 007d 0174 067c 037c 0183  ...t...}.t.|.|..
-00000f40: 0201 0071 1764 0053 0029 044e 7201 0000  ...q.d.S.).Nr...
-00000f50: 007a 1753 6176 696e 6720 7261 6e64 6f6d  .z.Saving random
-00000f60: 206b 6579 7320 746f 2022 7248 0000 0029   keys to "rH...)
-00000f70: 0772 3200 0000 721d 0000 0072 0800 0000  .r2...r....r....
-00000f80: 7229 0000 00da 046b 6579 73da 0464 6963  r).....keys..dic
-00000f90: 7472 0900 0000 2904 723d 0000 00da 0673  tr....).r=.....s
-00000fa0: 6967 6e65 7272 5700 0000 7258 0000 0072  ignerrW...rX...r
-00000fb0: 4400 0000 7244 0000 0072 4500 0000 da07  D...rD...rE.....
-00000fc0: 7275 6e4b 6579 7388 0000 0073 1400 0000  runKeys....s....
-00000fd0: 0e01 0601 0c01 0401 0602 0801 1001 0601  ................
-00000fe0: 0c01 04fd 725e 0000 0029 0172 5200 0000  ....r^...).rR...
-00000ff0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00001000: 0003 0000 0043 0000 0073 2400 0000 7400  .....C...s$...t.
-00001010: a001 a100 7d00 7c00 6a02 6400 7500 720b  ....}.|.j.d.u.r.
-00001020: 6400 5300 7c00 a003 7c00 a101 0100 6400  d.S.|...|.....d.
-00001030: 5300 2901 4e29 04da 0670 6172 7365 72da  S.).N)...parser.
-00001040: 0a70 6172 7365 5f61 7267 7372 0c00 0000  .parse_argsr....
-00001050: 7252 0000 0072 5500 0000 7244 0000 0072  rR...rU...rD...r
-00001060: 4400 0000 7245 0000 00da 046d 6169 6e9f  D...rE.....main.
-00001070: 0000 0073 0800 0000 0801 0a01 0401 0e02  ...s............
-00001080: 7261 0000 0029 2372 2c00 0000 da08 6172  ra...)#r,.....ar
-00001090: 6770 6172 7365 7238 0000 0072 3b00 0000  gparser8...r;...
-000010a0: da07 696e 7370 6563 7472 0200 0000 7203  ..inspectr....r.
-000010b0: 0000 0072 0400 0000 7205 0000 00da 1165  ...r....r......e
-000010c0: 7361 5f6c 6f77 6c65 7665 6c5f 7574 696c  sa_lowlevel_util
-000010d0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-000010e0: 0a00 0000 da0e 4172 6775 6d65 6e74 5061  ......ArgumentPa
-000010f0: 7273 6572 725f 0000 00da 0e61 6464 5f73  rserr_.....add_s
-00001100: 7562 7061 7273 6572 73da 0a73 7562 7061  ubparsers..subpa
-00001110: 7273 6572 73da 0a61 6464 5f70 6172 7365  rsers..add_parse
-00001120: 72da 0a70 6172 7365 7249 6e69 74da 0c61  r..parserInit..a
-00001130: 6464 5f61 7267 756d 656e 74da 0b70 6172  dd_argument..par
-00001140: 7365 7242 7569 6c64 da03 7374 72da 0a70  serBuild..str..p
-00001150: 6172 7365 724d 6574 61da 0a70 6172 7365  arserMeta..parse
-00001160: 7254 6573 74da 0a70 6172 7365 7253 6565  rTest..parserSee
-00001170: 64da 0a70 6172 7365 724b 6579 7372 4600  d..parserKeysrF.
-00001180: 0000 7247 0000 0072 5300 0000 7254 0000  ..rG...rS...rT..
-00001190: 0072 5a00 0000 725e 0000 00da 0c73 6574  .rZ...r^.....set
-000011a0: 5f64 6566 6175 6c74 7372 6100 0000 7244  _defaultsra...rD
-000011b0: 0000 0072 4400 0000 7244 0000 0072 4500  ...rD...rD...rE.
-000011c0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000011d0: 7344 0000 0008 0208 0108 0108 0118 0114  sD..............
-000011e0: 010c 010c 040e 010e 0210 0110 010e 0214  ................
-000011f0: 010e 0214 010e 020e 0214 010e 0214 0108  ................
-00001200: 0408 3308 0d08 1008 0508 0f0c 0e0c 010c  ..3.............
-00001210: 010c 010c 010c 010c 04                   .........
+00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
+00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c08  d.l.m.Z...d.d.l.
+00000070: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
+00000080: 0100 6404 6405 6c0d 6d0e 5a0e 6d0f 5a0f  ..d.d.l.m.Z.m.Z.
+00000090: 6d10 5a10 0100 6404 6406 6c11 6d11 5a11  m.Z...d.d.l.m.Z.
+000000a0: 0100 6502 6a12 6407 6408 8d01 5a13 6513  ..e.j.d.d...Z.e.
+000000b0: 6a14 6409 640a 640b 8d02 5a15 6515 6a16  j.d.d.d...Z.e.j.
+000000c0: 640c 640d 640e 8d02 5a17 6517 6a18 640f  d.d.d...Z.e.j.d.
+000000d0: 6410 6411 6412 8d03 0100 6517 6a18 6413  d.d.d.....e.j.d.
+000000e0: 6410 6414 6412 8d03 0100 6515 6a16 6415  d.d.d.....e.j.d.
+000000f0: 6416 640e 8d02 5a19 6519 6a18 6417 6417  d.d...Z.e.j.d.d.
+00000100: 651a 6418 6419 641a 8d05 0100 6515 6a16  e.d.d.d.....e.j.
+00000110: 641b 641c 640e 8d02 5a1b 651b 6a18 6417  d.d.d...Z.e.j.d.
+00000120: 6417 651a 641d 641e 641a 8d05 0100 6515  d.e.d.d.d.....e.
+00000130: 6a16 641f 6420 640e 8d02 5a1c 651c 6a18  j.d.d d...Z.e.j.
+00000140: 6421 6421 651a 6404 6422 641a 8d05 0100  d!d!e.d.d"d.....
+00000150: 6515 6a16 6423 6424 640e 8d02 5a1d 651d  e.j.d#d$d...Z.e.
+00000160: 6a18 6425 6425 651a 6418 6426 641a 8d05  j.d%d%e.d.d&d...
+00000170: 0100 6515 6a16 6427 6428 640e 8d02 5a1e  ..e.j.d'd(d...Z.
+00000180: 651e 6a18 6425 6425 651a 6418 6429 641a  e.j.d%d%e.d.d)d.
+00000190: 8d05 0100 642a 642b 8400 5a1f 642c 642d  ....d*d+..Z.d,d-
+000001a0: 8400 5a20 642e 642f 8400 5a21 6430 6431  ..Z d.d/..Z!d0d1
+000001b0: 8400 5a22 6432 651a 6602 6433 6434 8404  ..Z"d2e.f.d3d4..
+000001c0: 5a23 4700 6435 6436 8400 6436 6524 8303  Z#G.d5d6..d6e$..
+000001d0: 5a25 6437 6438 8400 5a26 6439 643a 8400  Z%d7d8..Z&d9d:..
+000001e0: 5a27 643b 643c 8400 5a28 6517 6a29 651f  Z'd;d<..Z(e.j)e.
+000001f0: 643d 8d01 0100 6519 6a29 6520 643d 8d01  d=....e.j)e d=..
+00000200: 0100 651b 6a29 6521 643d 8d01 0100 651c  ..e.j)e!d=....e.
+00000210: 6a29 6526 643d 8d01 0100 651d 6a29 6527  j)e&d=....e.j)e'
+00000220: 643d 8d01 0100 651e 6a29 6528 643d 8d01  d=....e.j)e(d=..
+00000230: 0100 643e 643f 8400 5a2a 6401 5300 2940  ..d>d?..Z*d.S.)@
+00000240: e900 0000 004e 2901 da08 5374 7269 6e67  .....N)...String
+00000250: 494f 2904 da09 6765 746d 6f64 756c 65da  IO)...getmodule.
+00000260: 0a67 6574 6d65 6d62 6572 73da 0a69 7366  .getmembers..isf
+00000270: 756e 6374 696f 6eda 0973 6967 6e61 7475  unction..signatu
+00000280: 7265 e901 0000 0029 03da 1667 656e 6572  re.....)...gener
+00000290: 6174 6552 616e 646f 6d4d 6e65 6d6f 6e69  ateRandomMnemoni
+000002a0: 63da 1467 656e 6572 6174 6552 616e 646f  c..generateRando
+000002b0: 6d53 6967 6e65 72da 0a73 6176 6553 6967  mSigner..saveSig
+000002c0: 6e65 7229 01da 0665 7665 7273 617a 5165  ner)...eversazQe
+000002d0: 7665 7273 6120 434c 4920 6865 6c70 7320  versa CLI helps 
+000002e0: 746f 2061 7574 6f6d 6174 6520 6275 696c  to automate buil
+000002f0: 6469 6e67 2061 6e64 2074 6573 7469 6e67  ding and testing
+00000300: 2045 7665 7273 6361 6c65 2f56 656e 6f6d   Everscale/Venom
+00000310: 2073 6d61 7274 2063 6f6e 7472 6163 7473   smart contracts
+00000320: 2901 da0b 6465 7363 7269 7074 696f 6eda  )...description.
+00000330: 0763 6f6d 6d61 6e64 5429 02da 0464 6573  .commandT)...des
+00000340: 74da 0872 6571 7569 7265 64da 0469 6e69  t..required..ini
+00000350: 747a 3a49 6e69 7469 616c 697a 6520 656d  tz:Initialize em
+00000360: 7074 7920 7072 6f6a 6563 7420 7769 7468  pty project with
+00000370: 2073 616d 706c 6573 2069 6e20 6375 7272   samples in curr
+00000380: 656e 7420 6469 7265 6374 6f72 7929 01da  ent directory)..
+00000390: 0468 656c 707a 072d 2d66 6f72 6365 da0a  .helpz.--force..
+000003a0: 7374 6f72 655f 7472 7565 7a33 4669 7273  store_truez3Firs
+000003b0: 6520 696e 6974 6961 6c69 7a61 7469 6f6e  e initialization
+000003c0: 2065 7665 6e20 6966 2064 6972 6563 746f   even if directo
+000003d0: 7279 2069 7320 6e6f 7420 656d 7074 7929  ry is not empty)
+000003e0: 02da 0661 6374 696f 6e72 1100 0000 7a0b  ...actionr....z.
+000003f0: 2d2d 6e6f 2d73 616d 706c 657a 1c44 6f20  --no-samplez.Do 
+00000400: 6e6f 7420 636f 7079 2061 6e79 2073 616d  not copy any sam
+00000410: 706c 6520 6669 6c65 73da 0562 7569 6c64  ple files..build
+00000420: da04 544f 444f da09 636f 6e74 7261 6374  ..TODO..contract
+00000430: 73da 012a 7a1f 4c69 7374 206f 6620 636f  s..*z.List of co
+00000440: 6e74 7261 6374 206e 616d 6573 2074 6f20  ntract names to 
+00000450: 6275 696c 6429 04da 076d 6574 6176 6172  build)...metavar
+00000460: da04 7479 7065 da05 6e61 7267 7372 1100  ..type..nargsr..
+00000470: 0000 da04 6d65 7461 7a33 5368 6f77 206d  ....metaz3Show m
+00000480: 6574 6164 6174 612f 6675 6e63 7469 6f6e  etadata/function
+00000490: 206c 6973 7420 666f 7220 6120 7370 6563   list for a spec
+000004a0: 6966 6963 2063 6f6e 7472 6163 74fa 012b  ific contract..+
+000004b0: 7a2a 4c69 7374 206f 6620 636f 6e74 7261  z*List of contra
+000004c0: 6374 206e 616d 6573 2074 6f20 7368 6f77  ct names to show
+000004d0: 206d 6574 6164 7461 2066 6f72 da04 7465   metadta for..te
+000004e0: 7374 7a25 5275 6e20 7465 7374 2073 6372  stz%Run test scr
+000004f0: 6970 7420 746f 2074 6573 7420 7468 6520  ipt to test the 
+00000500: 636f 6e74 7261 6374 73da 0b65 6e76 6972  contracts..envir
+00000510: 6f6e 6d65 6e74 7a49 5465 7374 2065 6e76  onmentzITest env
+00000520: 6972 6f6e 6d65 6e74 2028 7573 6520 6120  ironment (use a 
+00000530: 6e61 6d65 2066 726f 6d20 2e63 6f6e 6669  name from .confi
+00000540: 672e 6a73 6f6e 2066 696c 6529 2c20 666f  g.json file), fo
+00000550: 7220 6578 616d 706c 6520 606c 6f63 616c  r example `local
+00000560: 607a 086e 6577 2d73 6565 647a 3d43 7265  `z.new-seedz=Cre
+00000570: 6174 6520 6120 7261 6e64 6f6d 2073 6565  ate a random see
+00000580: 6420 7068 7261 7365 2077 6974 6820 616e  d phrase with an
+00000590: 206f 7074 696f 6e20 746f 2073 6176 6520   option to save 
+000005a0: 6974 2074 6f20 6669 6c65 da06 6f75 7470  it to file..outp
+000005b0: 7574 7a19 4669 6c65 206e 616d 6520 746f  utz.File name to
+000005c0: 2073 6176 6520 7365 6564 2074 6f7a 086e   save seed toz.n
+000005d0: 6577 2d6b 6579 737a 4843 7265 6174 6520  ew-keyszHCreate 
+000005e0: 6120 7261 6e64 6f6d 2070 7269 7661 7465  a random private
+000005f0: 2f70 7562 6c69 6320 6b65 7970 6169 7220  /public keypair 
+00000600: 7769 7468 2061 6e20 6f70 7469 6f6e 2074  with an option t
+00000610: 6f20 7361 7665 2069 7420 746f 2066 696c  o save it to fil
+00000620: 657a 1946 696c 6520 6e61 6d65 2074 6f20  ez.File name to 
+00000630: 7361 7665 206b 6579 7320 746f 6301 0000  save keys toc...
+00000640: 0000 0000 0000 0000 0008 0000 0009 0000  ................
+00000650: 0043 0000 0073 5202 0000 7400 6401 8301  .C...sR...t.d...
+00000660: 0100 7c00 6a01 0100 7c00 6a02 0100 7403  ..|.j...|.j...t.
+00000670: a004 a100 7d01 7403 6a05 a006 7403 6a05  ....}.t.j...t.j.
+00000680: a007 7408 a101 a101 7d02 7409 7403 a00a  ..t.....}.t.t...
+00000690: 7c01 a101 8301 6402 6b01 7d03 7c03 732c  |.....d.k.}.|.s,
+000006a0: 7c00 6a01 732c 7400 6403 8301 0100 6400  |.j.s,t.d.....d.
+000006b0: 5300 7a0c 7403 a00b 7403 6a05 a00c 7c01  S.z.t...t.j...|.
+000006c0: 6404 a102 a101 0100 5700 6e09 0400 740d  d.......W.n...t.
+000006d0: 7941 0100 0100 0100 5900 6e01 7700 7a0c  yA......Y.n.w.z.
+000006e0: 7403 a00b 7403 6a05 a00c 7c01 6405 a102  t...t.j...|.d...
+000006f0: a101 0100 5700 6e09 0400 740d 7957 0100  ....W.n...t.yW..
+00000700: 0100 0100 5900 6e01 7700 7a0c 7403 a00b  ....Y.n.w.z.t...
+00000710: 7403 6a05 a00c 7c01 6406 a102 a101 0100  t.j...|.d.......
+00000720: 5700 6e09 0400 740d 796d 0100 0100 0100  W.n...t.ym......
+00000730: 5900 6e01 7700 7a0c 7403 a00b 7403 6a05  Y.n.w.z.t...t.j.
+00000740: a00c 7c01 6407 a102 a101 0100 5700 6e09  ..|.d.......W.n.
+00000750: 0400 740d 7983 0100 0100 0100 5900 6e01  ..t.y.......Y.n.
+00000760: 7700 740e 7403 6a05 a00c 7c02 6408 a102  w.t.t.j...|.d...
+00000770: 8301 8f43 7d04 740f a010 7c04 a101 7d05  ...C}.t...|...}.
+00000780: 7c05 6409 1900 4400 5d0f 7d06 7c06 640a  |.d...D.].}.|.d.
+00000790: 1900 640b 6b02 72a6 7411 8300 7c06 640c  ..d.k.r.t...|.d.
+000007a0: 3c00 0100 6e01 7197 740e 7403 6a05 a00c  <...n.q.t.t.j...
+000007b0: 7c01 640d a102 640e 8302 8f10 7d07 740f  |.d...d.....}.t.
+000007c0: 6a12 7c05 7c07 640f 6410 8d03 0100 5700  j.|.|.d.d.....W.
+000007d0: 6400 0400 0400 8303 0100 6e08 3100 73c4  d.........n.1.s.
+000007e0: 7701 0100 0100 0100 5900 0100 5700 6400  w.......Y...W.d.
+000007f0: 0400 0400 8303 0100 6e08 3100 73d3 7701  ........n.1.s.w.
+00000800: 0100 0100 0100 5900 0100 7c00 6a02 9001  ......Y...|.j...
+00000810: 7323 7413 a014 7403 6a05 a00c 7c02 6411  s#t...t.j...|.d.
+00000820: 6412 a103 7403 6a05 a00c 7c01 6406 6412  d...t.j...|.d.d.
+00000830: a103 a102 0100 7413 a014 7403 6a05 a00c  ......t...t.j...
+00000840: 7c02 6411 6413 a103 7403 6a05 a00c 7c01  |.d.d...t.j...|.
+00000850: 6405 6413 a103 a102 0100 7413 a014 7403  d.d.......t...t.
+00000860: 6a05 a00c 7c02 6411 6414 a103 7403 6a05  j...|.d.d...t.j.
+00000870: a00c 7c01 6407 6414 a103 a102 0100 7413  ..|.d.d.......t.
+00000880: a014 7403 6a05 a00c 7c02 6411 6415 a103  ..t.j...|.d.d...
+00000890: 7403 6a05 a00c 7c01 6415 a102 a102 0100  t.j...|.d.......
+000008a0: 7400 6416 8301 0100 6400 5300 2917 4e7a  t.d.....d.S.).Nz
+000008b0: 1649 6e69 7469 616c 697a 696e 6720 6576  .Initializing ev
+000008c0: 6572 7361 2e2e 2e72 0100 0000 7a5b 4572  ersa...r....z[Er
+000008d0: 726f 7221 2043 7572 7265 6e74 2064 6972  ror! Current dir
+000008e0: 6563 746f 7279 2069 7320 6e6f 7420 656d  ectory is not em
+000008f0: 7074 7921 0a50 6c65 6173 6520 7573 6520  pty!.Please use 
+00000900: 666c 6167 202d 2d66 6f72 6365 2074 6f20  flag --force to 
+00000910: 696e 6974 6961 6c69 7a65 2065 7665 7273  initialize evers
+00000920: 6120 616e 7977 6179 2eda 0362 696e 7216  a anyway...binr.
+00000930: 0000 00da 0a69 6e74 6572 6661 6365 73da  .....interfaces.
+00000940: 0574 6573 7473 7a14 2e63 6f6e 6669 672e  .testsz..config.
+00000950: 6a73 6f6e 2e65 7861 6d70 6c65 da07 636f  json.example..co
+00000960: 6e66 6967 73da 046e 616d 65da 056c 6f63  nfigs..name..loc
+00000970: 616c da06 7068 7261 7365 7a0c 2e63 6f6e  al..phrasez..con
+00000980: 6669 672e 6a73 6f6e da01 77e9 0400 0000  fig.json..w.....
+00000990: 2901 da06 696e 6465 6e74 da06 7361 6d70  )...indent..samp
+000009a0: 6c65 7a0b 4953 616d 706c 652e 736f 6c7a  lez.ISample.solz
+000009b0: 0a53 616d 706c 652e 736f 6c7a 0774 6573  .Sample.solz.tes
+000009c0: 742e 7079 7a0a 2e67 6974 6967 6e6f 7265  t.pyz..gitignore
+000009d0: 7a05 446f 6e65 2129 15da 0570 7269 6e74  z.Done!)...print
+000009e0: da05 666f 7263 65da 096e 6f5f 7361 6d70  ..force..no_samp
+000009f0: 6c65 da02 6f73 da06 6765 7463 7764 da04  le..os..getcwd..
+00000a00: 7061 7468 da07 6469 726e 616d 65da 0872  path..dirname..r
+00000a10: 6561 6c70 6174 68da 085f 5f66 696c 655f  ealpath..__file_
+00000a20: 5fda 036c 656e da07 6c69 7374 6469 72da  _..len..listdir.
+00000a30: 056d 6b64 6972 da04 6a6f 696e da07 4f53  .mkdir..join..OS
+00000a40: 4572 726f 72da 046f 7065 6eda 046a 736f  Error..open..jso
+00000a50: 6eda 046c 6f61 6472 0800 0000 da04 6475  n..loadr......du
+00000a60: 6d70 da06 7368 7574 696c da08 636f 7079  mp..shutil..copy
+00000a70: 6669 6c65 2908 da04 6172 6773 da07 776f  file)...args..wo
+00000a80: 726b 4469 72da 096d 6f64 756c 6544 6972  rkDir..moduleDir
+00000a90: da08 6469 7245 6d70 7479 da0a 6a73 6f6e  ..dirEmpty..json
+00000aa0: 436f 6e66 6967 da06 636f 6e66 6967 da09  Config..config..
+00000ab0: 636f 6e66 6967 456c 6d72 1f00 0000 a900  configElmr......
+00000ac0: 7246 0000 00fa 2e62 7569 6c64 2f62 6469  rF.....build/bdi
+00000ad0: 7374 2e6c 696e 7578 2d78 3836 5f36 342f  st.linux-x86_64/
+00000ae0: 6567 672f 6576 6572 7361 2f65 7361 5f63  egg/eversa/esa_c
+00000af0: 6c69 2e70 79da 0772 756e 496e 6974 2800  li.py..runInit(.
+00000b00: 0000 735e 0000 0008 0106 0106 0108 0114  ..s^............
+00000b10: 0112 020a 0108 0104 0102 0318 010c 0104  ................
+00000b20: 0102 ff02 0218 010c 0104 0102 ff02 0218  ................
+00000b30: 010c 0104 0102 ff02 0218 010c 0104 0102  ................
+00000b40: ff14 040a 010c 010c 010a 0104 0102 fe16  ................
+00000b50: 0312 011c ff02 801c fa08 0a24 0124 0124  ...........$.$.$
+00000b60: 0122 010c 0272 4800 0000 6301 0000 0000  ."...rH...c.....
+00000b70: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+00000b80: 0000 0073 3c00 0000 7400 6401 8301 0100  ...s<...t.d.....
+00000b90: 7c00 6a01 6400 7500 720c 6700 7d01 6e03  |.j.d.u.r.g.}.n.
+00000ba0: 7c00 6a01 7d01 7c01 4400 5d0a 7d02 7400  |.j.}.|.D.].}.t.
+00000bb0: 6402 7c02 9b00 6403 9d03 8301 0100 7111  d.|...d.......q.
+00000bc0: 6400 5300 2904 4eda 0872 756e 4275 696c  d.S.).N..runBuil
+00000bd0: 647a 0a42 7569 6c64 696e 6720 22fa 0422  dz.Building ".."
+00000be0: 2e2e 2e29 0272 2b00 0000 7216 0000 0029  ...).r+...r....)
+00000bf0: 0372 3f00 0000 da0d 636f 6e74 7261 6374  .r?.....contract
+00000c00: 734c 6973 74da 0863 6f6e 7472 6163 7472  sList..contractr
+00000c10: 4600 0000 7246 0000 0072 4700 0000 7249  F...rF...rG...rI
+00000c20: 0000 005b 0000 0073 1000 0000 0801 0a01  ...[...s........
+00000c30: 0601 0602 0802 1001 0201 04fe 7249 0000  ............rI..
+00000c40: 0063 0100 0000 0000 0000 0000 0000 0600  .c..............
+00000c50: 0000 0700 0000 4300 0000 7380 0000 0074  ......C...s....t
+00000c60: 0083 007d 0174 0164 0183 0101 007c 006a  ...}.t.d.....|.j
+00000c70: 0244 005d 337d 0274 019d 0083 0101 0074  .D.]3}.t.......t
+00000c80: 0164 027c 029b 0064 039d 0383 0101 007c  .d.|...d.......|
+00000c90: 01a0 037c 02a1 017d 0374 047c 0374 0583  ...|...}.t.|.t..
+00000ca0: 0244 005d 1a5c 027d 047d 057c 0464 046b  .D.].\.}.}.|.d.k
+00000cb0: 0272 2b71 227c 0464 056b 0272 3164 067d  .r+q"|.d.k.r1d.}
+00000cc0: 0474 0164 077c 049b 0074 067c 0583 019b  .t.d.|...t.|....
+00000cd0: 009d 0383 0101 0071 2271 0a64 0053 0029  .......q"q.d.S.)
+00000ce0: 084e 7a24 5368 6f77 696e 6720 616c 6c20  .Nz$Showing all 
+00000cf0: 6675 6e63 7469 6f6e 7320 666f 7220 636f  functions for co
+00000d00: 6e74 7261 6374 733a fa01 227a 0222 3ada  ntracts:.."z.":.
+00000d10: 1165 7361 5570 6461 7465 496e 6974 4461  .esaUpdateInitDa
+00000d20: 7461 da06 6465 706c 6f79 da0b 636f 6e73  ta..deploy..cons
+00000d30: 7472 7563 746f 727a 0420 2020 2029 0772  tructorz.    ).r
+00000d40: 0b00 0000 722b 0000 0072 1600 0000 da0b  ....r+...r......
+00000d50: 4765 7443 6f6e 7472 6163 7472 0400 0000  GetContractr....
+00000d60: 7205 0000 0072 0600 0000 2906 723f 0000  r....r....).r?..
+00000d70: 00da 0365 7361 da0c 636f 6e74 7261 6374  ...esa..contract
+00000d80: 4e61 6d65 724c 0000 0072 2400 0000 da04  NamerL...r$.....
+00000d90: 6675 6e63 7246 0000 0072 4600 0000 7247  funcrF...rF...rG
+00000da0: 0000 00da 0772 756e 4d65 7461 6800 0000  .....runMetah...
+00000db0: 731c 0000 0006 0108 010a 0108 0110 010a  s...............
+00000dc0: 0112 0108 0102 0108 0104 0118 0102 fb04  ................
+00000dd0: fc72 5500 0000 6300 0000 0000 0000 0000  .rU...c.........
+00000de0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00000df0: 2c00 0000 6700 7d00 7400 7401 6a02 6401  ,...g.}.t.t.j.d.
+00000e00: 1900 7403 8302 4400 5d09 5c02 7d01 7d02  ..t...D.].\.}.}.
+00000e10: 7c00 a004 7c01 a101 0100 710a 7c00 5300  |...|.....q.|.S.
+00000e20: 2902 4e72 0b00 0000 2905 7204 0000 00da  ).Nr....).r.....
+00000e30: 0373 7973 da07 6d6f 6475 6c65 7372 0500  .sys..modulesr..
+00000e40: 0000 da06 6170 7065 6e64 2903 da0c 6675  ....append)...fu
+00000e50: 6e63 7469 6f6e 4c69 7374 7224 0000 00da  nctionListr$....
+00000e60: 055f 6675 6e63 7246 0000 0072 4600 0000  ._funcrF...rF...
+00000e70: 7247 0000 00da 1367 6574 4c69 6272 6172  rG.....getLibrar
+00000e80: 7946 756e 6374 696f 6e73 7800 0000 7308  yFunctionsx...s.
+00000e90: 0000 0004 0118 010c 0104 0172 5b00 0000  ...........r[...
+00000ea0: da03 6469 7263 0100 0000 0000 0000 0000  ..dirc..........
+00000eb0: 0000 0300 0000 0400 0000 4300 0000 732c  ..........C...s,
+00000ec0: 0000 0067 007d 0174 00a0 017c 00a1 0144  ...g.}.t...|...D
+00000ed0: 005d 0c7d 027c 02a0 0264 01a1 0172 137c  .].}.|...d...r.|
+00000ee0: 01a0 037c 02a1 0101 0071 077c 0153 0029  ...|.....q.|.S.)
+00000ef0: 024e 7a03 2e70 7929 0472 2e00 0000 7235  .Nz..py).r....r5
+00000f00: 0000 00da 0865 6e64 7377 6974 6872 5800  .....endswithrX.
+00000f10: 0000 2903 725c 0000 00da 0672 6573 756c  ..).r\.....resul
+00000f20: 74da 0466 696c 6572 4600 0000 7246 0000  t..filerF...rF..
+00000f30: 0072 4700 0000 da0e 6765 7450 7946 696c  .rG.....getPyFil
+00000f40: 6573 4c69 7374 7e00 0000 730c 0000 0004  esList~...s.....
+00000f50: 010e 010a 020a 0102 8004 0172 6000 0000  ...........r`...
+00000f60: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000f70: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
+00000f80: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
+00000f90: 6404 8400 5a04 6405 5300 2906 da09 4361  d...Z.d.S.)...Ca
+00000fa0: 7074 7572 696e 6763 0100 0000 0000 0000  pturingc........
+00000fb0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00000fc0: 731a 0000 0074 006a 017c 005f 0274 0383  s....t.j.|._.t..
+00000fd0: 0004 0074 005f 017c 005f 047c 0053 00a9  ...t._.|._.|.S..
+00000fe0: 014e 2905 7256 0000 00da 0673 7464 6f75  .N).rV.....stdou
+00000ff0: 74da 075f 7374 646f 7574 7202 0000 00da  t.._stdoutr.....
+00001000: 095f 7374 7269 6e67 696f 2901 da04 7365  ._stringio)...se
+00001010: 6c66 7246 0000 0072 4600 0000 7247 0000  lfrF...rF...rG..
+00001020: 00da 095f 5f65 6e74 6572 5f5f 8700 0000  ...__enter__....
+00001030: 7306 0000 0008 010e 0104 017a 1343 6170  s..........z.Cap
+00001040: 7475 7269 6e67 2e5f 5f65 6e74 6572 5f5f  turing.__enter__
+00001050: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001060: 0004 0000 0047 0000 0073 2400 0000 7c00  .....G...s$...|.
+00001070: a000 7c00 6a01 a002 a100 a003 a100 a101  ..|.j...........
+00001080: 0100 7c00 6001 7c00 6a04 7405 5f06 6400  ..|.`.|.j.t._.d.
+00001090: 5300 7262 0000 0029 07da 0665 7874 656e  S.rb...)...exten
+000010a0: 6472 6500 0000 da08 6765 7476 616c 7565  dre.....getvalue
+000010b0: da0a 7370 6c69 746c 696e 6573 7264 0000  ..splitlinesrd..
+000010c0: 0072 5600 0000 7263 0000 0029 0272 6600  .rV...rc...).rf.
+000010d0: 0000 723f 0000 0072 4600 0000 7246 0000  ..r?...rF...rF..
+000010e0: 0072 4700 0000 da08 5f5f 6578 6974 5f5f  .rG.....__exit__
+000010f0: 8b00 0000 7306 0000 0014 0104 010c 017a  ....s..........z
+00001100: 1243 6170 7475 7269 6e67 2e5f 5f65 7869  .Capturing.__exi
+00001110: 745f 5f4e 2905 da08 5f5f 6e61 6d65 5f5f  t__N)...__name__
+00001120: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00001130: 7175 616c 6e61 6d65 5f5f 7267 0000 0072  qualname__rg...r
+00001140: 6b00 0000 7246 0000 0072 4600 0000 7246  k...rF...rF...rF
+00001150: 0000 0072 4700 0000 7261 0000 0086 0000  ...rG...ra......
+00001160: 0073 0600 0000 0800 0801 0c04 7261 0000  .s..........ra..
+00001170: 0063 0100 0000 0000 0000 0000 0000 0b00  .c..............
+00001180: 0000 0a00 0000 4300 0000 7302 0100 0074  ......C...s....t
+00001190: 007c 006a 0164 0119 0083 017d 0174 0274  .|.j.d.....}.t.t
+000011a0: 036a 04a0 057c 016a 0664 02a1 0283 017d  .j...|.j.d.....}
+000011b0: 0269 007d 037c 0244 005d 367d 0467 007c  .i.}.|.D.]6}.g.|
+000011c0: 037c 043c 0074 07a0 0864 037c 049b 009d  .|.<.t...d.|....
+000011d0: 0274 036a 04a0 057c 016a 0664 027c 04a1  .t.j...|.j.d.|..
+000011e0: 03a1 027d 0567 007c 037c 043c 0074 0983  ...}.g.|.|.<.t..
+000011f0: 007d 0674 0a7c 0574 0b83 0244 005d 135c  .}.t.|.t...D.].\
+00001200: 027d 077d 087c 077c 0676 0072 4071 377c  .}.}.|.|.v.r@q7|
+00001210: 037c 0419 00a0 0c74 0d7c 057c 0783 02a1  .|.....t.|.|....
+00001220: 0101 0071 3771 157c 0344 005d 307d 057c  ...q7q.|.D.]0}.|
+00001230: 037c 0519 0044 005d 297d 0974 0e64 047c  .|...D.])}.t.d.|
+00001240: 059b 0064 057c 096a 0f9b 0064 059d 0583  ...d.|.j...d....
+00001250: 0101 0074 1083 008f 0c7d 0a7c 097c 0183  ...t.....}.|.|..
+00001260: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00001270: 0831 0073 7477 0101 0001 0001 0059 0001  .1.stw.......Y..
+00001280: 0074 0e64 0683 0101 0071 5471 4e64 0053  .t.d.....qTqNd.S
+00001290: 0029 074e 7201 0000 0072 2200 0000 da08  .).Nr....r".....
+000012a0: 6573 6154 6573 745f 7a08 5275 6e6e 696e  esaTest_z.Runnin
+000012b0: 6720 fa01 3a7a 0620 2020 204f 4b29 1172  g ..:z.    OK).r
+000012c0: 0b00 0000 721e 0000 0072 6000 0000 722e  ....r....r`...r.
+000012d0: 0000 0072 3000 0000 7237 0000 00da 0857  ...r0...r7.....W
+000012e0: 4f52 4b5f 4449 52da 0369 6d70 da0b 6c6f  ORK_DIR..imp..lo
+000012f0: 6164 5f73 6f75 7263 6572 5b00 0000 7204  ad_sourcer[...r.
+00001300: 0000 0072 0500 0000 7258 0000 00da 0767  ...r....rX.....g
+00001310: 6574 6174 7472 722b 0000 0072 6c00 0000  etattrr+...rl...
+00001320: 7261 0000 0029 0b72 3f00 0000 7252 0000  ra...).r?...rR..
+00001330: 00da 0b70 7954 6573 7446 696c 6573 da07  ...pyTestFiles..
+00001340: 7079 546f 5275 6eda 0874 6573 7446 696c  pyToRun..testFil
+00001350: 65da 066d 6f64 756c 65da 1166 756e 6374  e..module..funct
+00001360: 696f 6e73 496e 4576 6572 7361 7224 0000  ionsInEversar$..
+00001370: 0072 5a00 0000 da08 6675 6e63 7469 6f6e  .rZ.....function
+00001380: 721f 0000 0072 4600 0000 7246 0000 0072  r....rF...rF...r
+00001390: 4700 0000 da07 7275 6e54 6573 7490 0000  G.....runTest...
+000013a0: 0073 2c00 0000 0e02 1403 0401 0803 0801  .s,.............
+000013b0: 2001 0801 0602 1202 0801 0201 1601 02fd   ...............
+000013c0: 0805 0c01 1801 0801 0a01 1cff 0a02 02fc  ................
+000013d0: 04ff 727b 0000 0063 0100 0000 0000 0000  ..r{...c........
+000013e0: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
+000013f0: 737e 0000 0074 007c 006a 0183 0164 016b  s~...t.|.j...d.k
+00001400: 0272 1074 0283 007d 0174 037c 0183 0101  .r.t...}.t.|....
+00001410: 0064 0053 007c 006a 017d 027c 0244 005d  .d.S.|.j.}.|.D.]
+00001420: 277d 0374 0364 027c 039b 0064 039d 0383  '}.t.d.|...d....
+00001430: 0101 0074 0283 007d 0174 047c 0364 0483  ...t...}.t.|.d..
+00001440: 028f 0d7d 047c 04a0 057c 01a1 0101 0057  ...}.|...|.....W
+00001450: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00001460: 3777 0101 0001 0001 0059 0001 0071 1564  7w.......Y...q.d
+00001470: 0053 0029 054e 7201 0000 007a 1e53 6176  .S.).Nr....z.Sav
+00001480: 696e 6720 7261 6e64 6f6d 2073 6565 6420  ing random seed 
+00001490: 7068 7261 7365 2074 6f20 2272 4a00 0000  phrase to "rJ...
+000014a0: 7227 0000 0029 0672 3400 0000 721f 0000  r'...).r4...r...
+000014b0: 0072 0800 0000 722b 0000 0072 3900 0000  .r....r+...r9...
+000014c0: da05 7772 6974 6529 0572 3f00 0000 7226  ..write).r?...r&
+000014d0: 0000 00da 0866 696c 654c 6973 7472 5f00  .....fileListr_.
+000014e0: 0000 da01 6672 4600 0000 7246 0000 0072  ....frF...rF...r
+000014f0: 4700 0000 da07 7275 6e53 6565 64b0 0000  G.....runSeed...
+00001500: 0073 1a00 0000 0e01 0601 0801 0401 0602  .s..............
+00001510: 0801 1001 0601 0c01 0c01 1cff 0280 04fd  ................
+00001520: 727f 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001530: 0000 0400 0000 0500 0000 4300 0000 7358  ..........C...sX
+00001540: 0000 0074 007c 006a 0183 0164 016b 0272  ...t.|.j...d.k.r
+00001550: 1274 0283 007d 0174 037c 016a 046a 0583  .t...}.t.|.j.j..
+00001560: 0101 0064 0053 007c 006a 017d 027c 0244  ...d.S.|.j.}.|.D
+00001570: 005d 127d 0374 0364 027c 039b 0064 039d  .].}.t.d.|...d..
+00001580: 0383 0101 0074 0283 007d 0174 067c 037c  .....t...}.t.|.|
+00001590: 0183 0201 0071 1764 0053 0029 044e 7201  .....q.d.S.).Nr.
+000015a0: 0000 007a 1753 6176 696e 6720 7261 6e64  ...z.Saving rand
+000015b0: 6f6d 206b 6579 7320 746f 2022 724a 0000  om keys to "rJ..
+000015c0: 0029 0772 3400 0000 721f 0000 0072 0900  .).r4...r....r..
+000015d0: 0000 722b 0000 00da 046b 6579 73da 0464  ..r+.....keys..d
+000015e0: 6963 7472 0a00 0000 2904 723f 0000 00da  ictr....).r?....
+000015f0: 0673 6967 6e65 7272 7d00 0000 725f 0000  .signerr}...r_..
+00001600: 0072 4600 0000 7246 0000 0072 4700 0000  .rF...rF...rG...
+00001610: da07 7275 6e4b 6579 73bf 0000 0073 1400  ..runKeys....s..
+00001620: 0000 0e01 0601 0c01 0401 0602 0801 1001  ................
+00001630: 0601 0c01 04fd 7283 0000 0029 0172 5400  ......r....).rT.
+00001640: 0000 6300 0000 0000 0000 0000 0000 0001  ..c.............
+00001650: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
+00001660: 7400 a001 a100 7d00 7c00 6a02 6400 7500  t.....}.|.j.d.u.
+00001670: 720b 6400 5300 7c00 a003 7c00 a101 0100  r.d.S.|...|.....
+00001680: 6400 5300 7262 0000 0029 04da 0670 6172  d.S.rb...)...par
+00001690: 7365 72da 0a70 6172 7365 5f61 7267 7372  ser..parse_argsr
+000016a0: 0d00 0000 7254 0000 0029 0172 3f00 0000  ....rT...).r?...
+000016b0: 7246 0000 0072 4600 0000 7247 0000 00da  rF...rF...rG....
+000016c0: 046d 6169 6ed6 0000 0073 0800 0000 0801  .main....s......
+000016d0: 0a01 0401 0e02 7286 0000 0029 2b72 2e00  ......r....)+r..
+000016e0: 0000 7256 0000 00da 0861 7267 7061 7273  ..rV.....argpars
+000016f0: 6572 3a00 0000 723d 0000 0072 7200 0000  er:...r=...rr...
+00001700: da02 696f 7202 0000 00da 0769 6e73 7065  ..ior......inspe
+00001710: 6374 7203 0000 0072 0400 0000 7205 0000  ctr....r....r...
+00001720: 0072 0600 0000 da11 6573 615f 6c6f 776c  .r......esa_lowl
+00001730: 6576 656c 5f75 7469 6c72 0800 0000 7209  evel_utilr....r.
+00001740: 0000 0072 0a00 0000 720b 0000 00da 0e41  ...r....r......A
+00001750: 7267 756d 656e 7450 6172 7365 7272 8400  rgumentParserr..
+00001760: 0000 da0e 6164 645f 7375 6270 6172 7365  ....add_subparse
+00001770: 7273 da0a 7375 6270 6172 7365 7273 da0a  rs..subparsers..
+00001780: 6164 645f 7061 7273 6572 da0a 7061 7273  add_parser..pars
+00001790: 6572 496e 6974 da0c 6164 645f 6172 6775  erInit..add_argu
+000017a0: 6d65 6e74 da0b 7061 7273 6572 4275 696c  ment..parserBuil
+000017b0: 64da 0373 7472 da0a 7061 7273 6572 4d65  d..str..parserMe
+000017c0: 7461 da0a 7061 7273 6572 5465 7374 da0a  ta..parserTest..
+000017d0: 7061 7273 6572 5365 6564 da0a 7061 7273  parserSeed..pars
+000017e0: 6572 4b65 7973 7248 0000 0072 4900 0000  erKeysrH...rI...
+000017f0: 7255 0000 0072 5b00 0000 7260 0000 00da  rU...r[...r`....
+00001800: 046c 6973 7472 6100 0000 727b 0000 0072  .listra...r{...r
+00001810: 7f00 0000 7283 0000 00da 0c73 6574 5f64  ....r......set_d
+00001820: 6566 6175 6c74 7372 8600 0000 7246 0000  efaultsr....rF..
+00001830: 0072 4600 0000 7246 0000 0072 4700 0000  .rF...rF...rG...
+00001840: da08 3c6d 6f64 756c 653e 0100 0000 7352  ..<module>....sR
+00001850: 0000 0008 0208 0108 0108 0108 0108 010c  ................
+00001860: 0118 0114 010c 010c 040e 010e 0210 0110  ................
+00001870: 010e 0214 010e 0214 010e 0214 010e 0214  ................
+00001880: 010e 0214 0108 0408 3308 0d08 100e 0610  ........3.......
+00001890: 0808 0a08 2008 0f0c 0e0c 010c 010c 010c  .... ...........
+000018a0: 010c 010c 04                             .....
```

## eversa/__pycache__/esa_config.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 00:08:42 2023 UTC, .py size: 1527 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,67 +1,77 @@
-00000000: 6f0d 0d0a 0000 0000 8aca 7f64 f705 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 37d8 8964 0907 0000  o.......7..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 5400 6400  d.l.Z.d.d.l.T.d.
 00000040: 6402 6c02 5400 4700 6403 6404 8400 6404  d.l.T.G.d.d...d.
 00000050: 6503 8303 5a04 6401 5300 2905 e900 0000  e...Z.d.S.).....
 00000060: 004e 2901 da01 2a63 0000 0000 0000 0000  .N)...*c........
 00000070: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
 00000080: 731a 0000 0065 005a 0164 005a 0264 0165  s....e.Z.d.Z.d.e
 00000090: 0366 0264 0264 0384 045a 0464 0453 0029  .f.d.d...Z.d.S.)
 000000a0: 05da 0945 7361 436f 6e66 6967 da06 7461  ...EsaConfig..ta
 000000b0: 7267 6574 6302 0000 0000 0000 0000 0000  rgetc...........
-000000c0: 0005 0000 0008 0000 0043 0000 0073 f800  .........C...s..
+000000c0: 0005 0000 0008 0000 0043 0000 0073 0a01  .........C...s..
 000000d0: 0000 6401 7c00 5f00 6401 7c00 5f01 6401  ..d.|._.d.|._.d.
 000000e0: 7c00 5f02 6402 7c00 5f03 6401 7c00 5f04  |._.d.|._.d.|._.
 000000f0: 6401 6701 7c00 5f05 6403 7c00 5f06 6401  d.g.|._.d.|._.d.
-00000100: 7c00 5f07 6401 7c00 5f08 7409 6404 8301  |._.d.|._.t.d...
-00000110: 8f52 7d02 740a a00b 7c02 a101 7d03 7c03  .R}.t...|...}.|.
-00000120: 6405 1900 7c00 5f00 7c03 6406 1900 7c00  d...|._.|.d...|.
-00000130: 5f01 7c03 6407 1900 7c00 5f02 7c03 6408  _.|.d...|._.|.d.
-00000140: 1900 7c00 5f03 7c03 6409 1900 4400 5d23  ..|._.|.d...D.]#
-00000150: 7d04 7c04 640a 1900 7c01 6b02 7261 7c04  }.|.d...|.k.ra|.
-00000160: 640a 1900 7c00 5f04 7c04 640b 1900 7c00  d...|._.|.d...|.
-00000170: 5f05 7c04 640c 1900 7c00 5f06 7c04 640d  _.|.d...|._.|.d.
-00000180: 1900 7c00 5f07 7c04 640e 1900 7c00 5f08  ..|._.|.d...|._.
-00000190: 0100 6e09 713e 5700 6400 0400 0400 8303  ..n.q>W.d.......
-000001a0: 0100 6400 5300 5700 6400 0400 0400 8303  ..d.S.W.d.......
-000001b0: 0100 6400 5300 3100 7375 7701 0100 0100  ..d.S.1.suw.....
-000001c0: 0100 5900 0100 6400 5300 290f 4eda 0046  ..Y...d.S.).N..F
-000001d0: 7201 0000 007a 0c2e 636f 6e66 6967 2e6a  r....z..config.j
-000001e0: 736f 6eda 0765 7665 7264 6576 da0a 736f  son..everdev..so
-000001f0: 7572 6365 5f64 6972 da07 6269 6e5f 6469  urce_dir..bin_di
-00000200: 72da 0776 6572 626f 7365 da07 636f 6e66  r..verbose..conf
-00000210: 6967 73da 046e 616d 65da 0965 6e64 706f  igs..name..endpo
-00000220: 696e 7473 da09 776f 726b 6368 6169 6eda  ints..workchain.
-00000230: 0567 6976 6572 da06 7068 7261 7365 290c  .giver..phrase).
-00000240: da07 4556 4552 4445 56da 0a53 4f55 5243  ..EVERDEV..SOURC
-00000250: 455f 4449 52da 0742 494e 5f44 4952 da07  E_DIR..BIN_DIR..
-00000260: 5645 5242 4f53 45da 044e 414d 45da 0945  VERBOSE..NAME..E
-00000270: 4e44 504f 494e 5453 da09 574f 524b 4348  NDPOINTS..WORKCH
-00000280: 4149 4eda 0547 4956 4552 da06 5048 5241  AIN..GIVER..PHRA
-00000290: 5345 da04 6f70 656e da04 6a73 6f6e da04  SE..open..json..
-000002a0: 6c6f 6164 2905 da04 7365 6c66 7204 0000  load)...selfr...
-000002b0: 00da 0a6a 736f 6e43 6f6e 6669 67da 0663  ...jsonConfig..c
-000002c0: 6f6e 6669 67da 0963 6f6e 6669 6745 6c6d  onfig..configElm
-000002d0: a900 7220 0000 00fa 3162 7569 6c64 2f62  ..r ....1build/b
-000002e0: 6469 7374 2e6c 696e 7578 2d78 3836 5f36  dist.linux-x86_6
-000002f0: 342f 6567 672f 6576 6572 7361 2f65 7361  4/egg/eversa/esa
-00000300: 5f63 6f6e 6669 672e 7079 da08 5f5f 696e  _config.py..__in
-00000310: 6974 5f5f 0c00 0000 7338 0000 0006 0106  it__....s8......
-00000320: 0106 0106 0106 0108 0106 0106 0106 010a  ................
-00000330: 040a 010a 030a 010a 010a 010c 030c 010a  ................
-00000340: 010a 010a 010a 010a 0104 0102 fa02 ff0e  ................
-00000350: f602 1122 ef7a 1245 7361 436f 6e66 6967  ...".z.EsaConfig
-00000360: 2e5f 5f69 6e69 745f 5f4e 2905 da08 5f5f  .__init__N)...__
-00000370: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000380: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000390: da03 7374 7272 2200 0000 7220 0000 0072  ..strr"...r ...r
-000003a0: 2000 0000 7220 0000 0072 2100 0000 7203   ...r ...r!...r.
-000003b0: 0000 000b 0000 0073 0400 0000 0800 1201  .......s........
-000003c0: 7203 0000 0029 0572 1a00 0000 da10 746f  r....).r......to
-000003d0: 6e63 6c69 656e 742e 636c 6965 6e74 da0f  nclient.client..
-000003e0: 746f 6e63 6c69 656e 742e 7479 7065 73da  tonclient.types.
-000003f0: 066f 626a 6563 7472 0300 0000 7220 0000  .objectr....r ..
-00000400: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-00000410: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
-00000420: 0000 0008 0408 0108 0114 04              ...........
+00000100: 7c00 5f07 6402 7c00 5f08 6401 7c00 5f09  |._.d.|._.d.|._.
+00000110: 740a 6404 8301 8f58 7d02 740b a00c 7c02  t.d....X}.t...|.
+00000120: a101 7d03 7c03 6405 1900 7c00 5f00 7c03  ..}.|.d...|._.|.
+00000130: 6406 1900 7c00 5f01 7c03 6407 1900 7c00  d...|._.|.d...|.
+00000140: 5f02 7c03 6408 1900 7c00 5f03 7c01 7c03  _.|.d...|._.|.|.
+00000150: 6409 1900 7600 7c00 5f08 7c03 640a 1900  d...v.|._.|.d...
+00000160: 4400 5d2a 7d04 7c04 640b 1900 7c01 6b02  D.]*}.|.d...|.k.
+00000170: 7272 7c04 640b 1900 7c00 5f04 7c04 640c  rr|.d...|._.|.d.
+00000180: 1900 7c00 5f05 7c04 640d 1900 7c00 5f06  ..|._.|.d...|._.
+00000190: 7c04 640e 1900 7c00 5f07 7c04 640f 1900  |.d...|._.|.d...
+000001a0: 7c00 5f09 0100 5700 6400 0400 0400 8303  |._...W.d.......
+000001b0: 0100 6400 5300 7148 740d 6410 7c01 9b00  ..d.S.qHt.d.|...
+000001c0: 6411 9d03 8301 8201 3100 737e 7701 0100  d.......1.s~w...
+000001d0: 0100 0100 5900 0100 6400 5300 2912 4eda  ....Y...d.S.).N.
+000001e0: 0046 7201 0000 007a 0c2e 636f 6e66 6967  .Fr....z..config
+000001f0: 2e6a 736f 6eda 0765 7665 7264 6576 da0a  .json..everdev..
+00000200: 736f 7572 6365 5f64 6972 da07 6269 6e5f  source_dir..bin_
+00000210: 6469 72da 0776 6572 626f 7365 da0d 6769  dir..verbose..gi
+00000220: 7665 725f 656e 6162 6c65 64da 0763 6f6e  ver_enabled..con
+00000230: 6669 6773 da04 6e61 6d65 da09 656e 6470  figs..name..endp
+00000240: 6f69 6e74 73da 0977 6f72 6b63 6861 696e  oints..workchain
+00000250: da05 6769 7665 72da 0670 6872 6173 657a  ..giver..phrasez
+00000260: 1e49 6e76 616c 6964 2063 6f6e 6669 6775  .Invalid configu
+00000270: 7261 7469 6f6e 2074 6172 6765 743a 207a  ration target: z
+00000280: 3821 0a50 6c65 6173 6520 7573 6520 7661  8!.Please use va
+00000290: 6c69 6420 636f 6e66 6967 7572 6174 696f  lid configuratio
+000002a0: 6e20 6e61 6d65 2066 726f 6d20 2e63 6f6e  n name from .con
+000002b0: 6669 672e 6a73 6f6e 2129 0eda 0745 5645  fig.json!)...EVE
+000002c0: 5244 4556 da0a 534f 5552 4345 5f44 4952  RDEV..SOURCE_DIR
+000002d0: da07 4249 4e5f 4449 52da 0756 4552 424f  ..BIN_DIR..VERBO
+000002e0: 5345 da04 4e41 4d45 da09 454e 4450 4f49  SE..NAME..ENDPOI
+000002f0: 4e54 53da 0957 4f52 4b43 4841 494e da05  NTS..WORKCHAIN..
+00000300: 4749 5645 52da 0d47 4956 4552 5f45 4e41  GIVER..GIVER_ENA
+00000310: 424c 4544 da06 5048 5241 5345 da04 6f70  BLED..PHRASE..op
+00000320: 656e da04 6a73 6f6e da04 6c6f 6164 da0d  en..json..load..
+00000330: 4261 7365 4578 6365 7074 696f 6e29 05da  BaseException)..
+00000340: 0473 656c 6672 0400 0000 da0a 6a73 6f6e  .selfr......json
+00000350: 436f 6e66 6967 da06 636f 6e66 6967 da09  Config..config..
+00000360: 636f 6e66 6967 456c 6da9 0072 2300 0000  configElm..r#...
+00000370: fa31 6275 696c 642f 6264 6973 742e 6c69  .1build/bdist.li
+00000380: 6e75 782d 7838 365f 3634 2f65 6767 2f65  nux-x86_64/egg/e
+00000390: 7665 7273 612f 6573 615f 636f 6e66 6967  versa/esa_config
+000003a0: 2e70 79da 085f 5f69 6e69 745f 5f0c 0000  .py..__init__...
+000003b0: 0073 3a00 0000 0601 0601 0601 0601 0601  .s:.............
+000003c0: 0801 0601 0601 0601 0601 0a04 0a01 0a03  ................
+000003d0: 0a01 0a01 0a01 0e01 0c03 0c01 0a01 0a01  ................
+000003e0: 0a01 0a01 0a01 0201 10ee 020c 1007 14ed  ................
+000003f0: 7a12 4573 6143 6f6e 6669 672e 5f5f 696e  z.EsaConfig.__in
+00000400: 6974 5f5f 4e29 05da 085f 5f6e 616d 655f  it__N)...__name_
+00000410: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00000420: 5f71 7561 6c6e 616d 655f 5fda 0373 7472  _qualname__..str
+00000430: 7225 0000 0072 2300 0000 7223 0000 0072  r%...r#...r#...r
+00000440: 2300 0000 7224 0000 0072 0300 0000 0b00  #...r$...r......
+00000450: 0000 7304 0000 0008 0012 0172 0300 0000  ..s........r....
+00000460: 2905 721c 0000 00da 1074 6f6e 636c 6965  ).r......tonclie
+00000470: 6e74 2e63 6c69 656e 74da 0f74 6f6e 636c  nt.client..toncl
+00000480: 6965 6e74 2e74 7970 6573 da06 6f62 6a65  ient.types..obje
+00000490: 6374 7203 0000 0072 2300 0000 7223 0000  ctr....r#...r#..
+000004a0: 0072 2300 0000 7224 0000 00da 083c 6d6f  .r#...r$.....<mo
+000004b0: 6475 6c65 3e01 0000 0073 0800 0000 0804  dule>....s......
+000004c0: 0801 0801 1404                           ......
```

## eversa/__pycache__/esa_contract.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 10:27:27 2023 UTC, .py size: 10657 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0fad 8164 a129 0000  o..........d.)..
+00000000: 6f0d 0d0a 0000 0000 13d0 8964 f529 0000  o..........d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6402 6c02 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
 00000050: 6d03 5a03 0100 6404 6401 6c04 5400 6404  m.Z...d.d.l.T.d.
 00000060: 6401 6c05 5400 6404 6401 6c06 5400 6404  d.l.T.d.d.l.T.d.
 00000070: 6401 6c07 5400 6400 6405 6c08 6d09 5a09  d.l.T.d.d.l.m.Z.
@@ -266,18 +266,18 @@
 00001090: 616d 6963 616c 6c79 2066 726f 6d20 4142  amically from AB
 000010a0: 492e 0a0a 2020 2020 466f 7220 696e 7465  I...    For inte
 000010b0: 726e 616c 2075 7365 206f 6e6c 792c 2075  rnal use only, u
 000010c0: 7365 2069 7420 6f6e 6c79 2069 6620 796f  se it only if yo
 000010d0: 7520 6b6e 6f77 2077 6861 7420 796f 7520  u know what you 
 000010e0: 6172 6520 646f 696e 672e 0a20 2020 2063  are doing..    c
 000010f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001100: 0100 0000 4300 0000 7304 0000 0064 0053  ....C...s....d.S
+00001100: 0100 0000 4300 0000 f304 0000 0064 0053  ....C........d.S
 00001110: 0072 0d00 0000 7219 0000 0029 0172 1500  .r....r....).r..
 00001120: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00001130: 0072 1b00 0000 6100 0000 7302 0000 0004  .r....a...s.....
+00001130: 0072 1b00 0000 6100 0000 f302 0000 0004  .r....a.........
 00001140: 017a 1d45 7361 436f 6e74 7261 6374 4765  .z.EsaContractGe
 00001150: 6e65 7261 746f 722e 5f5f 696e 6974 5f5f  nerator.__init__
 00001160: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
 00001170: 0000 0000 0004 0000 0009 0000 004b 0000  .............K..
 00001180: 0073 2400 0000 7400 7c00 6a01 7c00 7c00  .s$...t.|.j.|.|.
 00001190: 6a02 7c00 6a03 7c00 6a04 7c01 6a05 7c02  j.|.j.|.j.|.j.|.
 000011a0: 6401 8d07 7d03 7c03 5300 2902 4e29 0772  d...}.|.S.).N).r
@@ -303,36 +303,36 @@
 000012e0: 496e 7075 74da 0b69 6e69 7469 616c 4461  Input..initialDa
 000012f0: 7461 721c 0000 00da 0d69 6e69 7469 616c  tar......initial
 00001300: 5075 626b 6579 2908 da0b 434f 4e53 5452  Pubkey)...CONSTR
 00001310: 5543 544f 52da 0e64 6570 6c6f 7943 6f6e  UCTOR..deployCon
 00001320: 7472 6163 7472 0e00 0000 720f 0000 0072  tractr....r....r
 00001330: 1000 0000 da08 494e 4954 4441 5441 7220  ......INITDATAr 
 00001340: 0000 00da 0e49 4e49 5449 414c 5f50 5542  .....INITIAL_PUB
-00001350: 4b45 5929 0472 1500 0000 7244 0000 0072  KEY).r....rD...r
-00001360: 4500 0000 7223 0000 0072 1900 0000 7219  E...r#...r....r.
+00001350: 4b45 5929 0472 1500 0000 7246 0000 0072  KEY).r....rF...r
+00001360: 4700 0000 7223 0000 0072 1900 0000 7219  G...r#...r....r.
 00001370: 0000 0072 1a00 0000 da16 5f67 656e 6572  ...r......_gener
 00001380: 6963 4465 706c 6f79 4675 6e63 7469 6f6e  icDeployFunction
 00001390: 6c00 0000 7306 0000 0006 0124 0104 017a  l...s......$...z
 000013a0: 2b45 7361 436f 6e74 7261 6374 4765 6e65  +EsaContractGene
 000013b0: 7261 746f 722e 5f67 656e 6572 6963 4465  rator._genericDe
 000013c0: 706c 6f79 4675 6e63 7469 6f6e 6302 0000  ployFunctionc...
 000013d0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
 000013e0: 004b 0000 0073 5800 0000 7c02 6401 1900  .K...sX...|.d...
 000013f0: 7d03 7c02 6402 1900 7d04 7c02 6401 3d00  }.|.d...}.|.d.=.
 00001400: 7c02 6402 3d00 7c03 6400 7501 7215 7c03  |.d.=.|.d.u.r.|.
 00001410: 7c00 5f00 7c02 7c00 5f01 7c04 7c00 5f02  |._.|.|._.|.|._.
 00001420: 7403 7c00 6a04 7c00 6a05 7c00 6a00 7c00  t.|.j.|.j.|.j.|.
 00001430: 6a02 7c00 6a01 6403 8d05 7c00 5f06 6400  j.|.j.d...|._.d.
-00001440: 5300 2904 4e72 1c00 0000 724a 0000 0029  S.).Nr....rJ...)
+00001440: 5300 2904 4e72 1c00 0000 724c 0000 0029  S.).Nr....rL...)
 00001450: 0572 0a00 0000 720b 0000 0072 1c00 0000  .r....r....r....
-00001460: 724a 0000 0072 4900 0000 2907 7220 0000  rJ...rI...).r ..
-00001470: 0072 4d00 0000 724e 0000 00da 0a67 6574  .rM...rN.....get
+00001460: 724c 0000 0072 4b00 0000 2907 7220 0000  rL...rK...).r ..
+00001470: 0072 4f00 0000 7250 0000 00da 0a67 6574  .rO...rP.....get
 00001480: 4164 6472 6573 7372 0f00 0000 7210 0000  Addressr....r...
-00001490: 0072 1100 0000 2905 7215 0000 0072 4400  .r....).r....rD.
-000014a0: 0000 7245 0000 0072 1c00 0000 724a 0000  ..rE...r....rJ..
+00001490: 0072 1100 0000 2905 7215 0000 0072 4600  .r....).r....rF.
+000014a0: 0000 7247 0000 0072 1c00 0000 724c 0000  ..rG...r....rL..
 000014b0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
 000014c0: da1e 5f67 656e 6572 6963 5570 6461 7465  .._genericUpdate
 000014d0: 496e 6974 4461 7461 4675 6e63 7469 6f6e  InitDataFunction
 000014e0: 7300 0000 7312 0000 0008 0108 0106 0106  s...s...........
 000014f0: 0108 0206 0106 0106 0122 017a 3345 7361  .........".z3Esa
 00001500: 436f 6e74 7261 6374 4765 6e65 7261 746f  ContractGenerato
 00001510: 722e 5f67 656e 6572 6963 5570 6461 7465  r._genericUpdate
@@ -371,35 +371,35 @@
 00001720: 0064 0e6b 0272 5c74 077c 0064 0f74 087c  .d.k.r\t.|.d.t.|
 00001730: 006a 0a7c 0664 0f64 108d 027c 006a 0b64  .j.|.d.d...|.j.d
 00001740: 0b64 0c8d 0383 0301 0071 4274 077c 007c  .d.......qBt.|.|
 00001750: 0664 0219 0074 087c 006a 0a7c 0664 118d  .d...t.|.j.|.d..
 00001760: 017c 006a 0c64 0b64 0c8d 0383 0301 0071  .|.j.d.d.......q
 00001770: 4257 0064 0004 0004 0083 0301 0064 0053  BW.d.........d.S
 00001780: 0031 0073 7a77 0101 0001 0001 0059 0001  .1.szw.......Y..
-00001790: 0064 0053 0029 124e da04 6461 7461 7252  .d.S.).N..datarR
-000017a0: 0000 0072 1e00 0000 7201 0000 0072 5500  ...r....r....rU.
+00001790: 0064 0053 0029 124e da04 6461 7461 7254  .d.S.).N..datarT
+000017a0: 0000 0072 1e00 0000 7201 0000 0072 5700  ...r....r....rW.
 000017b0: 0000 7a31 2c69 6e69 7469 616c 5075 626b  ..z1,initialPubk
 000017c0: 6579 3a73 7472 3d5a 4552 4f5f 5055 424b  ey:str=ZERO_PUBK
 000017d0: 4559 2c73 6967 6e65 723a 5369 676e 6572  EY,signer:Signer
 000017e0: 3d4e 6f6e 657a 3069 6e69 7469 616c 5075  =Nonez0initialPu
 000017f0: 626b 6579 3a73 7472 3d5a 4552 4f5f 5055  bkey:str=ZERO_PU
 00001800: 424b 4559 2c73 6967 6e65 723a 5369 676e  BKEY,signer:Sign
 00001810: 6572 3d4e 6f6e 65da 1165 7361 5570 6461  er=None..esaUpda
 00001820: 7465 496e 6974 4461 7461 7a12 6573 6155  teInitDataz.esaU
-00001830: 7064 6174 6549 6e69 7444 6174 6128 7256  pdateInitData(rV
+00001830: 7064 6174 6549 6e69 7444 6174 6128 7258  pdateInitData(rX
 00001840: 0000 0054 2901 da13 696e 6a65 6374 5f61  ...T)...inject_a
 00001850: 735f 6669 7273 745f 6172 67da 0966 756e  s_first_arg..fun
 00001860: 6374 696f 6e73 da0b 636f 6e73 7472 7563  ctions..construc
-00001870: 746f 72da 0664 6570 6c6f 7929 0272 5900  tor..deploy).rY.
-00001880: 0000 7217 0000 0029 0172 5900 0000 290d  ..r....).rY...).
+00001870: 746f 72da 0664 6570 6c6f 7929 0272 5b00  tor..deploy).r[.
+00001880: 0000 7217 0000 0029 0172 5b00 0000 290d  ..r....).r[...).
 00001890: da04 6f70 656e 720f 0000 00da 046a 736f  ..openr......jso
-000018a0: 6eda 046c 6f61 6472 5700 0000 da03 6c65  n..loadrW.....le
-000018b0: 6e72 5800 0000 da07 7365 7461 7474 7272  nrX.....setattrr
-000018c0: 0600 0000 7251 0000 0072 5d00 0000 724f  ....rQ...r]...rO
-000018d0: 0000 0072 4700 0000 2907 7215 0000 00da  ...rG...).r.....
+000018a0: 6eda 046c 6f61 6472 5900 0000 da03 6c65  n..loadrY.....le
+000018b0: 6e72 5a00 0000 da07 7365 7461 7474 7272  nrZ.....setattrr
+000018c0: 0600 0000 7253 0000 0072 5f00 0000 7251  ....rS...r_...rQ
+000018d0: 0000 0072 4900 0000 2907 7215 0000 00da  ...rI...).r.....
 000018e0: 0b61 6269 436f 6e74 656e 7473 da09 6162  .abiContents..ab
 000018f0: 6943 6f6e 6669 67da 0e69 6e69 7444 6174  iConfig..initDat
 00001900: 6146 6965 6c64 73da 0566 6965 6c64 da0e  aFields..field..
 00001910: 696e 6974 4461 7461 5061 7261 6d73 da08  initDataParams..
 00001920: 6675 6e63 7469 6f6e 7219 0000 0072 1900  functionr....r..
 00001930: 0000 721a 0000 00da 1867 656e 6572 6174  ..r......generat
 00001940: 6546 756e 6374 696f 6e73 4672 6f6d 4162  eFunctionsFromAb
@@ -409,126 +409,140 @@
 00001980: 0201 0201 0e01 0601 04ff 06fd 0207 0201  ................
 00001990: 0601 0c01 0601 04ff 06fd 02f6 22e9 7a2d  ............".z-
 000019a0: 4573 6143 6f6e 7472 6163 7447 656e 6572  EsaContractGener
 000019b0: 6174 6f72 2e67 656e 6572 6174 6546 756e  ator.generateFun
 000019c0: 6374 696f 6e73 4672 6f6d 4162 6929 024e  ctionsFromAbi).N
 000019d0: 4e29 0b72 3800 0000 7239 0000 0072 3a00  N).r8...r9...r:.
 000019e0: 0000 723b 0000 0072 1b00 0000 7208 0000  ..r;...r....r...
-000019f0: 0072 4700 0000 724f 0000 0072 5100 0000  .rG...rO...rQ...
-00001a00: 725d 0000 0072 6f00 0000 7219 0000 0072  r]...ro...r....r
+000019f0: 0072 4900 0000 7251 0000 0072 5300 0000  .rI...rQ...rS...
+00001a00: 725f 0000 0072 7100 0000 7219 0000 0072  r_...rq...r....r
 00001a10: 1900 0000 7219 0000 0072 1a00 0000 7242  ....r....r....rB
 00001a20: 0000 005b 0000 0073 1000 0000 0800 0401  ...[...s........
 00001a30: 0805 0e05 0806 0807 0a0e 0c0d 7242 0000  ............rB..
 00001a40: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00001a50: 0000 0d00 0000 4000 0000 735c 0000 0065  ......@...s\...e
+00001a50: 0000 0d00 0000 4000 0000 736c 0000 0065  ......@...sl...e
 00001a60: 005a 0164 005a 0264 015a 0364 0265 0464  .Z.d.Z.d.Z.d.e.d
 00001a70: 0266 0364 0365 0564 0465 0664 0565 0664  .f.d.e.d.e.d.e.d
 00001a80: 0665 0764 0765 0664 0865 0666 0c64 0964  .e.d.e.d.e.f.d.d
-00001a90: 0a84 055a 0864 1364 0c65 0966 0264 0d64  ...Z.d.d.e.f.d.d
-00001aa0: 0e84 055a 0a64 1364 0f64 1084 015a 0b64  ...Z.d.d.d...Z.d
-00001ab0: 1164 1284 005a 0c64 0253 0029 14da 0b45  .d...Z.d.S.)...E
-00001ac0: 7361 436f 6e74 7261 6374 7a21 0a20 2020  saContractz!.   
-00001ad0: 2047 656e 6572 6963 2063 6f6e 7472 6163   Generic contrac
-00001ae0: 7420 636c 6173 732e 0a20 2020 204e 7209  t class..    Nr.
-00001af0: 0000 0072 0a00 0000 720b 0000 0072 1c00  ...r....r....r..
-00001b00: 0000 724a 0000 00da 0761 6464 7265 7373  ..rJ.....address
-00001b10: 6307 0000 0000 0000 0000 0000 0007 0000  c...............
-00001b20: 0003 0000 0043 0000 0073 7400 0000 7c04  .....C...st...|.
-00001b30: 6400 7501 7206 7c04 6e02 7400 8300 7c00  d.u.r.|.n.t...|.
-00001b40: 5f01 7c01 7c00 5f02 7403 7c01 6401 8d01  _.|.|._.t.|.d...
-00001b50: 7c00 5f04 6400 7c00 5f05 7c02 7c00 5f06  |._.d.|._.|.|._.
-00001b60: 7c03 7c00 5f07 7408 7c00 6402 8302 7323  |.|._.t.|.d...s#
-00001b70: 6900 6e02 7c00 6a09 7c00 5f09 7408 7c00  i.n.|.j.|._.t.|.
-00001b80: 6403 8302 732e 6900 6e02 7c00 6a0a 7c00  d...s.i.n.|.j.|.
-00001b90: 5f0a 7c05 7c00 5f0b 7c06 7c00 5f0c 6400  _.|.|._.|.|._.d.
-00001ba0: 5300 2904 4e29 0172 0900 0000 724b 0000  S.).N).r....rK..
-00001bb0: 0072 4d00 0000 290d da14 6765 6e65 7261  .rM...)...genera
-00001bc0: 7465 5261 6e64 6f6d 5369 676e 6572 7220  teRandomSignerr 
-00001bd0: 0000 0072 0e00 0000 da0a 4573 6147 7261  ...r......EsaGra
-00001be0: 7068 514c da07 4752 4150 4851 4cda 0342  phQL..GRAPHQL..B
-00001bf0: 4f43 720f 0000 0072 1000 0000 721f 0000  OCr....r....r...
-00001c00: 0072 4b00 0000 724d 0000 0072 4e00 0000  .rK...rM...rN...
-00001c10: 7211 0000 0029 0772 1500 0000 7209 0000  r....).r....r...
-00001c20: 0072 0a00 0000 720b 0000 0072 1c00 0000  .r....r....r....
-00001c30: 724a 0000 0072 7100 0000 7219 0000 0072  rJ...rq...r....r
-00001c40: 1900 0000 721a 0000 0072 1b00 0000 bd00  ....r....r......
-00001c50: 0000 7314 0000 0014 0106 010c 0106 0106  ..s.............
-00001c60: 0106 0116 0116 0106 010a 017a 1445 7361  ...........z.Esa
-00001c70: 436f 6e74 7261 6374 2e5f 5f69 6e69 745f  Contract.__init_
-00001c80: 5f46 da0b 666f 7263 6555 7064 6174 6563  _F..forceUpdatec
-00001c90: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00001ca0: 0400 0000 4300 0000 7350 0000 007c 0173  ....C...sP...|.s
-00001cb0: 077c 006a 0064 0075 0072 257c 006a 016a  .|.j.d.u.r%|.j.j
-00001cc0: 027c 006a 0364 0164 028d 027d 027c 0264  .|.j.d.d...}.|.d
-00001cd0: 0075 0073 1a7c 0264 0119 0064 0075 0072  .u.s.|.d...d.u.r
-00001ce0: 2064 007c 005f 007c 006a 0053 007c 0264   d.|._.|.j.S.|.d
-00001cf0: 0119 007c 005f 007c 006a 0053 0029 034e  ...|._.|.j.S.).N
-00001d00: 7234 0000 00a9 02da 0961 6363 6f75 6e74  r4.......account
-00001d10: 4944 da06 6669 656c 6473 2904 7275 0000  ID..fields).ru..
-00001d20: 0072 7400 0000 da11 6765 7441 6363 6f75  .rt.....getAccou
-00001d30: 6e74 4772 6170 6851 4c72 1100 0000 2903  ntGraphQLr....).
-00001d40: 7215 0000 0072 7600 0000 7223 0000 0072  r....rv...r#...r
-00001d50: 1900 0000 7219 0000 0072 1a00 0000 7235  ....r....r....r5
-00001d60: 0000 00c9 0000 0073 0e00 0000 0e01 1201  .......s........
-00001d70: 1401 0601 0603 0aff 0601 7a12 4573 6143  ..........z.EsaC
-00001d80: 6f6e 7472 6163 742e 6765 7442 4f43 6302  ontract.getBOCc.
-00001d90: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00001da0: 0000 0043 0000 0073 3a00 0000 7c00 6a00  ...C...s:...|.j.
-00001db0: 6a01 7c00 6a02 6401 6402 8d02 7d02 7c02  j.|.j.d.d...}.|.
-00001dc0: 6400 7501 7213 7403 7c02 6403 1900 8301  d.u.r.t.|.d.....
-00001dd0: 6e01 6404 7d03 7c01 721b 7c03 7404 1b00  n.d.}.|.r.|.t...
-00001de0: 5300 7c03 5300 2905 4e7a 1362 616c 616e  S.|.S.).Nz.balan
-00001df0: 6365 2866 6f72 6d61 743a 4445 4329 7277  ce(format:DEC)rw
-00001e00: 0000 00da 0762 616c 616e 6365 7201 0000  .....balancer...
-00001e10: 0029 0572 7400 0000 727a 0000 0072 1100  .).rt...rz...r..
-00001e20: 0000 7241 0000 00da 0445 5645 5229 0472  ..rA.....EVER).r
-00001e30: 1500 0000 da0b 7368 6f77 496e 4576 6572  ......showInEver
-00001e40: 7372 2300 0000 727b 0000 0072 1900 0000  sr#...r{...r....
-00001e50: 7219 0000 0072 1a00 0000 da0a 6765 7442  r....r......getB
-00001e60: 616c 616e 6365 d200 0000 7306 0000 0012  alance....s.....
-00001e70: 0118 0110 017a 1645 7361 436f 6e74 7261  .....z.EsaContra
-00001e80: 6374 2e67 6574 4261 6c61 6e63 6563 0100  ct.getBalancec..
-00001e90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001ea0: 0000 4300 0000 732a 0000 007c 006a 006a  ..C...s*...|.j.j
-00001eb0: 017c 006a 0264 0164 028d 027d 017c 0164  .|.j.d.d...}.|.d
-00001ec0: 0375 0172 1374 037c 0164 0119 0083 0153  .u.r.t.|.d.....S
-00001ed0: 0064 0453 0029 057a a00a 2020 2020 2020  .d.S.).z..      
-00001ee0: 2020 4765 7473 2041 6363 6f75 6e74 2074    Gets Account t
-00001ef0: 7970 6520 6672 6f6d 2062 6c6f 636b 6368  ype from blockch
-00001f00: 6169 6e2e 2050 6f73 7369 626c 6520 7661  ain. Possible va
-00001f10: 6c75 6573 3a0a 0a20 2020 2020 2020 2060  lues:..        `
-00001f20: 3060 202d 2075 6e69 6e69 742e 0a20 2020  0` - uninit..   
-00001f30: 2020 2020 2060 3160 202d 2061 6374 6976       `1` - activ
-00001f40: 652e 0a20 2020 2020 2020 2060 3260 202d  e..        `2` -
-00001f50: 2066 726f 7a65 6e2e 0a20 2020 2020 2020   frozen..       
-00001f60: 2060 3360 202d 206e 6f6e 4578 6973 742e   `3` - nonExist.
-00001f70: 0a20 2020 2020 2020 20da 0861 6363 5f74  .        ..acc_t
-00001f80: 7970 6572 7700 0000 4e72 0100 0000 2904  yperw...Nr....).
-00001f90: 7274 0000 0072 7a00 0000 7211 0000 0072  rt...rz...r....r
-00001fa0: 4100 0000 2902 7215 0000 0072 2300 0000  A...).r....r#...
-00001fb0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00001fc0: 0a67 6574 4163 6354 7970 65d7 0000 0073  .getAccType....s
-00001fd0: 0400 0000 1209 1801 7a16 4573 6143 6f6e  ........z.EsaCon
-00001fe0: 7472 6163 742e 6765 7441 6363 5479 7065  tract.getAccType
-00001ff0: 2901 4629 0d72 3800 0000 7239 0000 0072  ).F).r8...r9...r
-00002000: 3a00 0000 723b 0000 00da 0b5a 4552 4f5f  :...r;.....ZERO_
-00002010: 5055 424b 4559 723c 0000 0072 3d00 0000  PUBKEYr<...r=...
-00002020: 723e 0000 0072 1b00 0000 723f 0000 0072  r>...r....r?...r
-00002030: 3500 0000 727e 0000 0072 8000 0000 7219  5...r~...r....r.
-00002040: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00002050: 0000 7270 0000 00b9 0000 0073 0c00 0000  ..rp.......s....
-00002060: 0800 0401 2a03 100c 0a09 0c05 7270 0000  ....*.......rp..
-00002070: 004e 2910 da10 746f 6e63 6c69 656e 742e  .N)...tonclient.
-00002080: 636c 6965 6e74 da0f 746f 6e63 6c69 656e  client..tonclien
-00002090: 742e 7479 7065 7372 0300 0000 7204 0000  t.typesr....r...
-000020a0: 00da 1165 7361 5f6c 6f77 6c65 7665 6c5f  ...esa_lowlevel_
-000020b0: 7574 696c da0f 6573 615f 6c6f 776c 6576  util..esa_lowlev
-000020c0: 656c 5f62 63da 0d65 7361 5f63 6f6e 7374  el_bc..esa_const
-000020d0: 616e 7473 da0b 6573 615f 6772 6170 6871  ants..esa_graphq
-000020e0: 6cda 076d 616b 6566 756e 7206 0000 00da  l..makefunr.....
-000020f0: 0769 6e73 7065 6374 7207 0000 00da 066f  .inspectr......o
-00002100: 626a 6563 7472 0800 0000 7242 0000 0072  bjectr....rB...r
-00002110: 7000 0000 7219 0000 0072 1900 0000 7219  p...r....r....r.
-00002120: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
-00002130: 653e 0100 0000 731a 0000 0008 0408 010c  e>....s.........
-00002140: 010c 0108 0108 0108 0108 010c 010c 0110  ................
-00002150: 0410 4914 5e                             ..I.^
+00001a90: 0a84 055a 0864 1764 0c65 0966 0264 0d64  ...Z.d.d.e.f.d.d
+00001aa0: 0e84 055a 0a64 1764 0f64 1084 015a 0b64  ...Z.d.d.d...Z.d
+00001ab0: 1164 1284 005a 0c64 1364 1484 005a 0d64  .d...Z.d.d...Z.d
+00001ac0: 1564 1684 005a 0e64 0253 0029 18da 0b45  .d...Z.d.S.)...E
+00001ad0: 7361 436f 6e74 7261 6374 7a21 0a20 2020  saContractz!.   
+00001ae0: 2047 656e 6572 6963 2063 6f6e 7472 6163   Generic contrac
+00001af0: 7420 636c 6173 732e 0a20 2020 204e 7209  t class..    Nr.
+00001b00: 0000 0072 0a00 0000 720b 0000 0072 1c00  ...r....r....r..
+00001b10: 0000 724c 0000 00da 0761 6464 7265 7373  ..rL.....address
+00001b20: 6307 0000 0000 0000 0000 0000 0007 0000  c...............
+00001b30: 0003 0000 0043 0000 0073 7400 0000 7c04  .....C...st...|.
+00001b40: 6400 7501 7206 7c04 6e02 7400 8300 7c00  d.u.r.|.n.t...|.
+00001b50: 5f01 7c01 7c00 5f02 7403 7c01 6401 8d01  _.|.|._.t.|.d...
+00001b60: 7c00 5f04 6400 7c00 5f05 7c02 7c00 5f06  |._.d.|._.|.|._.
+00001b70: 7c03 7c00 5f07 7408 7c00 6402 8302 7323  |.|._.t.|.d...s#
+00001b80: 6900 6e02 7c00 6a09 7c00 5f09 7408 7c00  i.n.|.j.|._.t.|.
+00001b90: 6403 8302 732e 6900 6e02 7c00 6a0a 7c00  d...s.i.n.|.j.|.
+00001ba0: 5f0a 7c05 7c00 5f0b 7c06 7c00 5f0c 6400  _.|.|._.|.|._.d.
+00001bb0: 5300 2904 4e29 0172 0900 0000 724d 0000  S.).N).r....rM..
+00001bc0: 0072 4f00 0000 290d da14 6765 6e65 7261  .rO...)...genera
+00001bd0: 7465 5261 6e64 6f6d 5369 676e 6572 7220  teRandomSignerr 
+00001be0: 0000 0072 0e00 0000 da0a 4573 6147 7261  ...r......EsaGra
+00001bf0: 7068 514c da07 4752 4150 4851 4cda 0342  phQL..GRAPHQL..B
+00001c00: 4f43 720f 0000 0072 1000 0000 721f 0000  OCr....r....r...
+00001c10: 0072 4d00 0000 724f 0000 0072 5000 0000  .rM...rO...rP...
+00001c20: 7211 0000 0029 0772 1500 0000 7209 0000  r....).r....r...
+00001c30: 0072 0a00 0000 720b 0000 0072 1c00 0000  .r....r....r....
+00001c40: 724c 0000 0072 7300 0000 7219 0000 0072  rL...rs...r....r
+00001c50: 1900 0000 721a 0000 0072 1b00 0000 bd00  ....r....r......
+00001c60: 0000 7314 0000 0014 0106 010c 0106 0106  ..s.............
+00001c70: 0106 0116 0116 0106 010a 017a 1445 7361  ...........z.Esa
+00001c80: 436f 6e74 7261 6374 2e5f 5f69 6e69 745f  Contract.__init_
+00001c90: 5f46 da0b 666f 7263 6555 7064 6174 6563  _F..forceUpdatec
+00001ca0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00001cb0: 0400 0000 4300 0000 7350 0000 007c 0173  ....C...sP...|.s
+00001cc0: 077c 006a 0064 0075 0072 257c 006a 016a  .|.j.d.u.r%|.j.j
+00001cd0: 027c 006a 0364 0164 028d 027d 027c 0264  .|.j.d.d...}.|.d
+00001ce0: 0075 0073 1a7c 0264 0119 0064 0075 0072  .u.s.|.d...d.u.r
+00001cf0: 2064 007c 005f 007c 006a 0053 007c 0264   d.|._.|.j.S.|.d
+00001d00: 0119 007c 005f 007c 006a 0053 0029 034e  ...|._.|.j.S.).N
+00001d10: 7234 0000 00a9 02da 0961 6363 6f75 6e74  r4.......account
+00001d20: 4944 da06 6669 656c 6473 2904 7277 0000  ID..fields).rw..
+00001d30: 0072 7600 0000 da11 6765 7441 6363 6f75  .rv.....getAccou
+00001d40: 6e74 4772 6170 6851 4c72 1100 0000 2903  ntGraphQLr....).
+00001d50: 7215 0000 0072 7800 0000 7223 0000 0072  r....rx...r#...r
+00001d60: 1900 0000 7219 0000 0072 1a00 0000 7235  ....r....r....r5
+00001d70: 0000 00c9 0000 0073 0e00 0000 0e01 1201  .......s........
+00001d80: 1401 0601 0603 0aff 0601 7a12 4573 6143  ..........z.EsaC
+00001d90: 6f6e 7472 6163 742e 6765 7442 4f43 6302  ontract.getBOCc.
+00001da0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00001db0: 0000 0043 0000 0073 3a00 0000 7c00 6a00  ...C...s:...|.j.
+00001dc0: 6a01 7c00 6a02 6401 6402 8d02 7d02 7c02  j.|.j.d.d...}.|.
+00001dd0: 6400 7501 7213 7403 7c02 6403 1900 8301  d.u.r.t.|.d.....
+00001de0: 6e01 6404 7d03 7c01 721b 7c03 7404 1b00  n.d.}.|.r.|.t...
+00001df0: 5300 7c03 5300 2905 4e7a 1362 616c 616e  S.|.S.).Nz.balan
+00001e00: 6365 2866 6f72 6d61 743a 4445 4329 7279  ce(format:DEC)ry
+00001e10: 0000 00da 0762 616c 616e 6365 7201 0000  .....balancer...
+00001e20: 0029 0572 7600 0000 727c 0000 0072 1100  .).rv...r|...r..
+00001e30: 0000 7241 0000 00da 0445 5645 5229 0472  ..rA.....EVER).r
+00001e40: 1500 0000 da0b 7368 6f77 496e 4576 6572  ......showInEver
+00001e50: 7372 2300 0000 727d 0000 0072 1900 0000  sr#...r}...r....
+00001e60: 7219 0000 0072 1a00 0000 da0a 6765 7442  r....r......getB
+00001e70: 616c 616e 6365 d200 0000 7306 0000 0012  alance....s.....
+00001e80: 0118 0110 017a 1645 7361 436f 6e74 7261  .....z.EsaContra
+00001e90: 6374 2e67 6574 4261 6c61 6e63 6563 0100  ct.getBalancec..
+00001ea0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00001eb0: 0000 4300 0000 732a 0000 007c 006a 006a  ..C...s*...|.j.j
+00001ec0: 017c 006a 0264 0164 028d 027d 017c 0164  .|.j.d.d...}.|.d
+00001ed0: 0375 0172 1374 037c 0164 0119 0083 0153  .u.r.t.|.d.....S
+00001ee0: 0064 0453 0029 057a a00a 2020 2020 2020  .d.S.).z..      
+00001ef0: 2020 4765 7473 2041 6363 6f75 6e74 2074    Gets Account t
+00001f00: 7970 6520 6672 6f6d 2062 6c6f 636b 6368  ype from blockch
+00001f10: 6169 6e2e 2050 6f73 7369 626c 6520 7661  ain. Possible va
+00001f20: 6c75 6573 3a0a 0a20 2020 2020 2020 2060  lues:..        `
+00001f30: 3060 202d 2075 6e69 6e69 742e 0a20 2020  0` - uninit..   
+00001f40: 2020 2020 2060 3160 202d 2061 6374 6976       `1` - activ
+00001f50: 652e 0a20 2020 2020 2020 2060 3260 202d  e..        `2` -
+00001f60: 2066 726f 7a65 6e2e 0a20 2020 2020 2020   frozen..       
+00001f70: 2060 3360 202d 206e 6f6e 4578 6973 742e   `3` - nonExist.
+00001f80: 0a20 2020 2020 2020 20da 0861 6363 5f74  .        ..acc_t
+00001f90: 7970 6572 7900 0000 4e72 0100 0000 2904  ypery...Nr....).
+00001fa0: 7276 0000 0072 7c00 0000 7211 0000 0072  rv...r|...r....r
+00001fb0: 4100 0000 2902 7215 0000 0072 2300 0000  A...).r....r#...
+00001fc0: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00001fd0: 0a67 6574 4163 6354 7970 65d7 0000 0073  .getAccType....s
+00001fe0: 0400 0000 1209 1801 7a16 4573 6143 6f6e  ........z.EsaCon
+00001ff0: 7472 6163 742e 6765 7441 6363 5479 7065  tract.getAccType
+00002000: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00002010: 0001 0000 0043 0000 0072 4300 0000 720d  .....C...rC...r.
+00002020: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
+00002030: 0000 7219 0000 0072 1a00 0000 da07 6765  ..r....r......ge
+00002040: 7453 616c 74e3 0000 0072 4400 0000 7a13  tSalt....rD...z.
+00002050: 4573 6143 6f6e 7472 6163 742e 6765 7453  EsaContract.getS
+00002060: 616c 7463 0000 0000 0000 0000 0000 0000  altc............
+00002070: 0000 0000 0100 0000 4300 0000 7243 0000  ........C...rC..
+00002080: 0072 0d00 0000 7219 0000 0072 1900 0000  .r....r....r....
+00002090: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+000020a0: 0773 6574 5361 6c74 e600 0000 7244 0000  .setSalt....rD..
+000020b0: 007a 1345 7361 436f 6e74 7261 6374 2e73  .z.EsaContract.s
+000020c0: 6574 5361 6c74 2901 4629 0f72 3800 0000  etSalt).F).r8...
+000020d0: 7239 0000 0072 3a00 0000 723b 0000 00da  r9...r:...r;....
+000020e0: 0b5a 4552 4f5f 5055 424b 4559 723c 0000  .ZERO_PUBKEYr<..
+000020f0: 0072 3d00 0000 723e 0000 0072 1b00 0000  .r=...r>...r....
+00002100: 723f 0000 0072 3500 0000 7280 0000 0072  r?...r5...r....r
+00002110: 8200 0000 7283 0000 0072 8400 0000 7219  ....r....r....r.
+00002120: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00002130: 0000 7272 0000 00b9 0000 0073 1000 0000  ..rr.......s....
+00002140: 0800 0401 2a03 100c 0a09 0805 080c 0c03  ....*...........
+00002150: 7272 0000 004e 2910 da10 746f 6e63 6c69  rr...N)...toncli
+00002160: 656e 742e 636c 6965 6e74 da0f 746f 6e63  ent.client..tonc
+00002170: 6c69 656e 742e 7479 7065 7372 0300 0000  lient.typesr....
+00002180: 7204 0000 00da 1165 7361 5f6c 6f77 6c65  r......esa_lowle
+00002190: 7665 6c5f 7574 696c da0f 6573 615f 6c6f  vel_util..esa_lo
+000021a0: 776c 6576 656c 5f62 63da 0d65 7361 5f63  wlevel_bc..esa_c
+000021b0: 6f6e 7374 616e 7473 da0b 6573 615f 6772  onstants..esa_gr
+000021c0: 6170 6871 6cda 076d 616b 6566 756e 7206  aphql..makefunr.
+000021d0: 0000 00da 0769 6e73 7065 6374 7207 0000  .....inspectr...
+000021e0: 00da 066f 626a 6563 7472 0800 0000 7242  ...objectr....rB
+000021f0: 0000 0072 7200 0000 7219 0000 0072 1900  ...rr...r....r..
+00002200: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
+00002210: 6f64 756c 653e 0100 0000 731a 0000 0008  odule>....s.....
+00002220: 0408 010c 010c 0108 0108 0108 0108 010c  ................
+00002230: 010c 0110 0410 4914 5e                   ......I.^
```

## eversa/__pycache__/esa_lowlevel_util.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 19:34:24 2023 UTC, .py size: 2962 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 402d 8264 920b 0000  o.......@-.d....
+00000000: 6f0d 0d0a 0000 0000 5c9e 8964 920b 0000  o.......\..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 5400 6400  d.l.Z.d.d.l.T.d.
 00000040: 6402 6c02 5400 6400 6403 6c03 6d03 5a03  d.l.T.d.d.l.m.Z.
 00000050: 0100 6404 6405 6c04 6d05 5a05 0100 6406  ..d.d.l.m.Z...d.
 00000060: 6407 8400 5a06 6408 6409 8400 5a07 640a  d...Z.d.d...Z.d.
 00000070: 640b 8400 5a08 640c 640d 8400 5a09 640e  d...Z.d.d...Z.d.
@@ -158,42 +158,41 @@
 000009d0: 4700 0000 724a 0000 0072 3a00 0000 7248  G...rJ...r:...rH
 000009e0: 0000 00da 0568 646b 6579 7244 0000 0072  .....hdkeyrD...r
 000009f0: 4500 0000 720b 0000 0072 0b00 0000 720c  E...r....r....r.
 00000a00: 0000 00da 1a67 656e 6572 6174 6553 6967  .....generateSig
 00000a10: 6e65 7246 726f 6d4d 6e65 6d6f 6e69 633c  nerFromMnemonic<
 00000a20: 0000 0073 1800 0000 0201 0e01 1401 1801  ...s............
 00000a30: 0201 1201 1201 06fe 0c04 0601 0601 0401  ................
-00000a40: 7257 0000 00da 0866 696c 656e 616d 6572  rW.....filenamer
+00000a40: 7257 0000 00da 086b 6579 7346 696c 6572  rW.....keysFiler
 00000a50: 4500 0000 6302 0000 0000 0000 0000 0000  E...c...........
 00000a60: 0002 0000 0004 0000 0043 0000 0073 1200  .........C...s..
 00000a70: 0000 7c01 6a00 a001 7c00 6401 a102 0100  ..|.j...|.d.....
 00000a80: 6400 5300 a902 4e46 2902 7240 0000 00da  d.S...NF).r@....
-00000a90: 0464 756d 7029 0272 5800 0000 7245 0000  .dump).rX...rE..
+00000a90: 0464 756d 70a9 0272 5800 0000 7245 0000  .dump..rX...rE..
 00000aa0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
 00000ab0: da0a 7361 7665 5369 676e 6572 4a00 0000  ..saveSignerJ...
-00000ac0: 722e 0000 0072 5b00 0000 6301 0000 0000  r....r[...c.....
+00000ac0: 722e 0000 0072 5c00 0000 6301 0000 0000  r....r\...c.....
 00000ad0: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
 00000ae0: 0000 0073 2c00 0000 7c00 6400 7500 720b  ...s,...|.d.u.r.
 00000af0: 7400 a001 7402 a101 7d01 7c01 5300 7400  t...t...}.|.S.t.
 00000b00: a003 7404 a005 7c00 6401 a102 a101 7d01  ..t...|.d.....}.
 00000b10: 7c01 5300 7259 0000 0029 0672 4200 0000  |.S.rY...).rB...
 00000b20: da08 4578 7465 726e 616c 7205 0000 0072  ..Externalr....r
-00000b30: 4300 0000 7251 0000 00da 046c 6f61 6429  C...rQ.....load)
-00000b40: 02da 086b 6579 7346 696c 6572 4500 0000  ...keysFilerE...
-00000b50: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
-00000b60: 0a6c 6f61 6453 6967 6e65 724d 0000 0073  .loadSignerM...s
-00000b70: 0a00 0000 0801 0a01 0403 12ff 0401 725f  ..............r_
-00000b80: 0000 0029 0272 0100 0000 5472 1900 0000  ...).r....Tr....
-00000b90: 2915 7210 0000 00da 1074 6f6e 636c 6965  ).r......tonclie
-00000ba0: 6e74 2e63 6c69 656e 74da 0f74 6f6e 636c  nt.client..toncl
-00000bb0: 6965 6e74 2e74 7970 6573 7203 0000 00da  ient.typesr.....
-00000bc0: 0d65 7361 5f63 6f6e 7374 616e 7473 7205  .esa_constantsr.
-00000bd0: 0000 0072 0d00 0000 7218 0000 0072 1a00  ...r....r....r..
-00000be0: 0000 7228 0000 0072 2d00 0000 7232 0000  ..r(...r-...r2..
-00000bf0: 0072 3800 0000 7229 0000 0072 3e00 0000  .r8...r)...r>...
-00000c00: 7242 0000 0072 4600 0000 da03 696e 7472  rB...rF.....intr
-00000c10: 5700 0000 725b 0000 0072 5f00 0000 720b  W...r[...r_...r.
-00000c20: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000c30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000c40: 7322 0000 0008 0408 0108 010c 010c 0108  s"..............
-00000c50: 0408 0408 0608 0308 0908 0308 050e 070e  ................
-00000c60: 0518 0518 0e14 03                        .......
+00000b30: 4300 0000 7251 0000 00da 046c 6f61 6472  C...rQ.....loadr
+00000b40: 5b00 0000 720b 0000 0072 0b00 0000 720c  [...r....r....r.
+00000b50: 0000 00da 0a6c 6f61 6453 6967 6e65 724d  .....loadSignerM
+00000b60: 0000 0073 0a00 0000 0801 0a01 0403 12ff  ...s............
+00000b70: 0401 725f 0000 0029 0272 0100 0000 5472  ..r_...).r....Tr
+00000b80: 1900 0000 2915 7210 0000 00da 1074 6f6e  ....).r......ton
+00000b90: 636c 6965 6e74 2e63 6c69 656e 74da 0f74  client.client..t
+00000ba0: 6f6e 636c 6965 6e74 2e74 7970 6573 7203  onclient.typesr.
+00000bb0: 0000 00da 0d65 7361 5f63 6f6e 7374 616e  .....esa_constan
+00000bc0: 7473 7205 0000 0072 0d00 0000 7218 0000  tsr....r....r...
+00000bd0: 0072 1a00 0000 7228 0000 0072 2d00 0000  .r....r(...r-...
+00000be0: 7232 0000 0072 3800 0000 7229 0000 0072  r2...r8...r)...r
+00000bf0: 3e00 0000 7242 0000 0072 4600 0000 da03  >...rB...rF.....
+00000c00: 696e 7472 5700 0000 725c 0000 0072 5f00  intrW...r\...r_.
+00000c10: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00000c20: 0072 0c00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00000c30: 0100 0000 7322 0000 0008 0408 0108 010c  ....s"..........
+00000c40: 010c 0108 0408 0408 0608 0308 0908 0308  ................
+00000c50: 050e 070e 0518 0518 0e14 03              ...........
```

## eversa/__pycache__/eversa.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 14 08:55:48 2023 UTC, .py size: 5424 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9480 8964 3015 0000  o..........d0...
+00000000: 6f0d 0d0a 0000 0000 d3b8 8964 6d15 0000  o..........dm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 5400 6400 6403 6c04  ..d.d.l.T.d.d.l.
 00000050: 5400 6404 6405 6c05 6d06 5a06 0100 6404  T.d.d.l.m.Z...d.
 00000060: 6406 6c07 6d08 5a08 0100 6404 6403 6c09  d.l.m.Z...d.d.l.
 00000070: 5400 4700 6407 6408 8400 6408 650a 8303  T.G.d.d...d.e...
@@ -267,56 +267,58 @@
 000010a0: 524b 4348 4149 4e29 0172 1600 0000 7217  RKCHAIN).r....r.
 000010b0: 0000 0072 1700 0000 7218 0000 0072 0c00  ...r....r....r..
 000010c0: 0000 6300 0000 7302 0000 0026 017a 1465  ..c...s....&.z.e
 000010d0: 7665 7273 612e 6765 7445 7665 7243 6c69  versa.getEverCli
 000010e0: 656e 74da 0f63 6f6e 7472 6163 7441 6464  ent..contractAdd
 000010f0: 7265 7373 da05 7661 6c75 6563 0300 0000  ress..valuec....
 00001100: 0000 0000 0000 0000 0400 0000 0800 0000  ................
-00001110: 4300 0000 7346 0000 007c 00a0 0064 017c  C...sF...|...d.|
-00001120: 019b 0064 027c 029b 0064 039d 05a1 0101  ...d.|...d......
-00001130: 007c 00a0 0164 0464 05a1 027d 0374 027c  .|...d.d...}.t.|
-00001140: 006a 037c 037c 006a 046a 0564 067c 017c  .j.|.|.j.j.d.|.|
-00001150: 0264 079c 0274 06a0 07a1 0083 0653 0029  .d...t.......S.)
-00001160: 087a 750a 2020 2020 2020 2020 546f 702d  .zu.        Top-
-00001170: 7570 206f 7220 6675 6e64 206f 7220 6769  up or fund or gi
-00001180: 7665 206e 6174 6976 6520 636f 696e 2074  ve native coin t
-00001190: 6f20 6120 636f 6e74 7261 6374 2075 7369  o a contract usi
-000011a0: 6e67 2047 6976 6572 2028 6375 7272 656e  ng Giver (curren
-000011b0: 746c 7920 776f 726b 7320 666f 7220 6c6f  tly works for lo
-000011c0: 6361 6c20 6e6f 6465 206f 6e6c 7929 2e0a  cal node only)..
-000011d0: 2020 2020 2020 2020 7a20 6576 6572 7361          z eversa
-000011e0: 2e61 6972 6472 6f70 2863 6f6e 7472 6163  .airdrop(contrac
-000011f0: 7441 6464 7265 7373 3a20 7a09 2c20 7661  tAddress: z., va
-00001200: 6c75 653a 20fa 0129 da0b 6c6f 6361 6c5f  lue: ..)..local_
-00001210: 6769 7665 7272 3200 0000 da09 7365 6e64  giverr2.....send
-00001220: 4772 616d 7329 02da 0464 6573 74da 0661  Grams)...dest..a
-00001230: 6d6f 756e 7429 0872 1d00 0000 722d 0000  mount).r....r-..
-00001240: 0072 0600 0000 720d 0000 0072 0b00 0000  .r....r....r....
-00001250: da05 4749 5645 52da 0653 6967 6e65 72da  ..GIVER..Signer.
-00001260: 084e 6f53 6967 6e65 7229 0472 1600 0000  .NoSigner).r....
-00001270: 7251 0000 0072 5200 0000 7235 0000 0072  rQ...rR...r5...r
-00001280: 1700 0000 7217 0000 0072 1800 0000 da07  ....r....r......
-00001290: 6169 7264 726f 7066 0000 0073 0600 0000  airdropf...s....
-000012a0: 1804 0c01 2201 7a0e 6576 6572 7361 2e61  ....".z.eversa.a
-000012b0: 6972 6472 6f70 2901 7208 0000 0029 0272  irdrop).r....).r
-000012c0: 0100 0000 5429 10da 085f 5f6e 616d 655f  ....T)...__name_
-000012d0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000012e0: 5f71 7561 6c6e 616d 655f 5f72 3d00 0000  _qualname__r=...
-000012f0: 7219 0000 0072 1d00 0000 da03 696e 7472  r....r......intr
-00001300: 2300 0000 722d 0000 00da 0b5a 4552 4f5f  #...r-.....ZERO_
-00001310: 5055 424b 4559 7259 0000 0072 3900 0000  PUBKEYrY...r9...
-00001320: 7243 0000 0072 4500 0000 720c 0000 0072  rC...rE...r....r
-00001330: 5b00 0000 7217 0000 0072 1700 0000 7217  [...r....r....r.
-00001340: 0000 0072 1800 0000 7207 0000 000f 0000  ...r....r.......
-00001350: 0073 1200 0000 0800 1001 0806 1004 120c  .s..............
-00001360: 2011 0e28 0804 1603 7207 0000 0029 0c72   ..(....r....).r
-00001370: 0e00 0000 da07 7061 7468 6c69 6272 0200  ......pathlibr..
-00001380: 0000 da10 746f 6e63 6c69 656e 742e 636c  ....tonclient.cl
-00001390: 6965 6e74 da0f 746f 6e63 6c69 656e 742e  ient..tonclient.
-000013a0: 7479 7065 73da 0a65 7361 5f63 6f6e 6669  types..esa_confi
-000013b0: 6772 0500 0000 da0f 6573 615f 6c6f 776c  gr......esa_lowl
-000013c0: 6576 656c 5f62 6372 0600 0000 da0c 6573  evel_bcr......es
-000013d0: 615f 636f 6e74 7261 6374 da06 6f62 6a65  a_contract..obje
-000013e0: 6374 7207 0000 0072 1700 0000 7217 0000  ctr....r....r...
-000013f0: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
-00001400: 6475 6c65 3e01 0000 0073 1000 0000 0804  dule>....s......
-00001410: 0c01 0801 0801 0c01 0c01 0801 1404       ..............
+00001110: 4300 0000 7352 0000 007c 006a 006a 0173  C...sR...|.j.j.s
+00001120: 0664 0153 007c 00a0 0264 027c 019b 0064  .d.S.|...d.|...d
+00001130: 037c 029b 0064 049d 05a1 0101 007c 00a0  .|...d.......|..
+00001140: 0364 0564 06a1 027d 0374 047c 006a 057c  .d.d...}.t.|.j.|
+00001150: 037c 006a 006a 0664 077c 017c 0264 089c  .|.j.j.d.|.|.d..
+00001160: 0274 07a0 08a1 0083 0653 0029 097a 750a  .t.......S.).zu.
+00001170: 2020 2020 2020 2020 546f 702d 7570 206f          Top-up o
+00001180: 7220 6675 6e64 206f 7220 6769 7665 206e  r fund or give n
+00001190: 6174 6976 6520 636f 696e 2074 6f20 6120  ative coin to a 
+000011a0: 636f 6e74 7261 6374 2075 7369 6e67 2047  contract using G
+000011b0: 6976 6572 2028 6375 7272 656e 746c 7920  iver (currently 
+000011c0: 776f 726b 7320 666f 7220 6c6f 6361 6c20  works for local 
+000011d0: 6e6f 6465 206f 6e6c 7929 2e0a 2020 2020  node only)..    
+000011e0: 2020 2020 4e7a 2065 7665 7273 612e 6169      Nz eversa.ai
+000011f0: 7264 726f 7028 636f 6e74 7261 6374 4164  rdrop(contractAd
+00001200: 6472 6573 733a 207a 092c 2076 616c 7565  dress: z., value
+00001210: 3a20 fa01 29da 0b6c 6f63 616c 5f67 6976  : ..)..local_giv
+00001220: 6572 7232 0000 00da 0973 656e 6447 7261  err2.....sendGra
+00001230: 6d73 2902 da04 6465 7374 da06 616d 6f75  ms)...dest..amou
+00001240: 6e74 2909 720b 0000 00da 0d47 4956 4552  nt).r......GIVER
+00001250: 5f45 4e41 424c 4544 721d 0000 0072 2d00  _ENABLEDr....r-.
+00001260: 0000 7206 0000 0072 0d00 0000 da05 4749  ..r....r......GI
+00001270: 5645 52da 0653 6967 6e65 72da 084e 6f53  VER..Signer..NoS
+00001280: 6967 6e65 7229 0472 1600 0000 7251 0000  igner).r....rQ..
+00001290: 0072 5200 0000 7235 0000 0072 1700 0000  .rR...r5...r....
+000012a0: 7217 0000 0072 1800 0000 da07 6169 7264  r....r......aird
+000012b0: 726f 7066 0000 0073 0a00 0000 0804 0401  ropf...s........
+000012c0: 1801 0c01 2201 7a0e 6576 6572 7361 2e61  ....".z.eversa.a
+000012d0: 6972 6472 6f70 2901 7208 0000 0029 0272  irdrop).r....).r
+000012e0: 0100 0000 5429 10da 085f 5f6e 616d 655f  ....T)...__name_
+000012f0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001300: 5f71 7561 6c6e 616d 655f 5f72 3d00 0000  _qualname__r=...
+00001310: 7219 0000 0072 1d00 0000 da03 696e 7472  r....r......intr
+00001320: 2300 0000 722d 0000 00da 0b5a 4552 4f5f  #...r-.....ZERO_
+00001330: 5055 424b 4559 725a 0000 0072 3900 0000  PUBKEYrZ...r9...
+00001340: 7243 0000 0072 4500 0000 720c 0000 0072  rC...rE...r....r
+00001350: 5c00 0000 7217 0000 0072 1700 0000 7217  \...r....r....r.
+00001360: 0000 0072 1800 0000 7207 0000 000f 0000  ...r....r.......
+00001370: 0073 1200 0000 0800 1001 0806 1004 120c  .s..............
+00001380: 2011 0e28 0804 1603 7207 0000 0029 0c72   ..(....r....).r
+00001390: 0e00 0000 da07 7061 7468 6c69 6272 0200  ......pathlibr..
+000013a0: 0000 da10 746f 6e63 6c69 656e 742e 636c  ....tonclient.cl
+000013b0: 6965 6e74 da0f 746f 6e63 6c69 656e 742e  ient..tonclient.
+000013c0: 7479 7065 73da 0a65 7361 5f63 6f6e 6669  types..esa_confi
+000013d0: 6772 0500 0000 da0f 6573 615f 6c6f 776c  gr......esa_lowl
+000013e0: 6576 656c 5f62 6372 0600 0000 da0c 6573  evel_bcr......es
+000013f0: 615f 636f 6e74 7261 6374 da06 6f62 6a65  a_contract..obje
+00001400: 6374 7207 0000 0072 1700 0000 7217 0000  ctr....r....r...
+00001410: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
+00001420: 6475 6c65 3e01 0000 0073 1000 0000 0804  dule>....s......
+00001430: 0c01 0801 0801 0c01 0c01 0801 1404       ..............
```

## eversa/sample/test.py

```diff
@@ -1,45 +1,52 @@
 #!/usr/bin/env python3
 
 # ==============================================================================
 # 
 from eversa import *
 
 # ==============================================================================
-# EVERSA INIT
+# SIGNERS
 # ==============================================================================
-# 
-# eversa main class
-esa = eversa()
+def testSigners(esa: eversa):
+    #
+    # Generate random mnemonic and get Signer from it
+    phrase  = generateRandomMnemonic()
+    signer1 = generateSignerFromMnemonic(phrase=phrase, childIndex=1)
+
+    # Generate Signer from mnemonic from `.config.json`
+    signer2 = esa.getSigner(childIndex=7)
+
+    # Generate completely random Signer
+    signer3 = generateRandomSigner()
+
+    # Save and load Signer to/from JSON file
+    saveSigner(keysFile="signer3.json", signer=signer3)
+    signer4 = loadSigner(keysFile="signer3.json")
 
 # ==============================================================================
-# SIGNERS
+# CONTRACTS
 # ==============================================================================
-#
-# Generate random mnemonic and get Signer from it
-phrase  = generateRandomMnemonic()
-signer1 = generateSignerFromMnemonic(phrase=phrase, childIndex=1)
-
-# Generate Signer from mnemonic from `.config.json`
-signer2 = esa.getSigner(childIndex=7)
-
-# Generate completely random Signer
-signer3 = generateRandomSigner()
-
-# Save and load Signer to/from JSON file
-saveSigner(filename="signer3.json", signer=signer3)
-signer4 = loadSigner(filename="signer3.json")
+def testContracts(esa: eversa):
+    #
+    # Generate completely random Signer
+    signer = generateRandomSigner()
+    #
+    # Dynamically create `SetcodeMultisig` contract class
+    msig1 = esa.GetContract("SetcodeMultisig", signer=signer, initialPubkey=signer.keys.public)
+    esa.airdrop(msig1.ADDRESS, EVER)
+    print(f"Multisig 1 address: {msig1.ADDRESS}")
+    print(f"Multisig 1 balance: {msig1.getBalance(showInEvers=True)}")
+
+    # Specify contract constructor params in `deploy` function and print results
+    result = msig1.deploy(owners=[f"0x{signer.keys.public}"], reqConfirms=1)
+    print(result["result"], result["exception"])
 
 # ==============================================================================
-# CONTRACTS
+# RUNNING MANUALLY
 # ==============================================================================
+# Keep this part if you want to manually run the tests without `eversa test` wrapper
 #
-# Dynamically create `SetcodeMultisig` contract class
-msig1 = esa.GetContract("SetcodeMultisig", signer=signer1, initialPubkey=signer1.keys.public)
-esa.airdrop(msig1.ADDRESS, EVER)
-print(f"Multisig 1 address: {msig1.ADDRESS}")
-print(f"Multisig 1 balance: {msig1.getBalance(showInEvers=True)}")
-
-# Specify contract constructor params in `deploy` function and print results
-result = msig1.deploy(owners=[f"0x{signer1.keys.public}"], reqConfirms=1)
-print(result["result"], result["exception"])
-
+if __name__ == "__main__":
+    esa = eversa()
+    testSigners(esa)
+    testContracts(esa)
```

## eversa/sample/__pycache__/test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun 14 08:55:50 2023 UTC, .py size: 1640 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,53 +1,72 @@
-00000000: 6f0d 0d0a 0000 0000 9680 8964 6806 0000  o..........dh...
+00000000: 6f0d 0d0a 0000 0000 7aae 8964 d407 0000  o.......z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
-00000030: 6401 6c00 5400 6500 8300 5a01 6502 8300  d.l.T.e...Z.e...
-00000040: 5a03 6504 6503 6402 6403 8d02 5a05 6501  Z.e.e.d.d...Z.e.
-00000050: 6a06 6404 6405 8d01 5a07 6508 8300 5a09  j.d.d...Z.e...Z.
-00000060: 650a 6406 6509 6407 8d02 0100 650b 6406  e.d.e.d.....e.d.
-00000070: 6408 8d01 5a0c 6501 6a0d 6409 6505 6505  d...Z.e.j.d.e.e.
-00000080: 6a0e 6a0f 640a 8d03 5a10 6501 a011 6510  j.j.d...Z.e...e.
-00000090: 6a12 6513 a102 0100 6514 640b 6510 6a12  j.e.....e.d.e.j.
-000000a0: 9b00 9d02 8301 0100 6514 640c 6510 6a15  ........e.d.e.j.
-000000b0: 640d 640e 8d01 9b00 9d02 8301 0100 6510  d.d...........e.
-000000c0: 6a16 640f 6505 6a0e 6a0f 9b00 9d02 6701  j.d.e.j.j.....g.
-000000d0: 6402 6410 8d02 5a17 6514 6517 6411 1900  d.d...Z.e.e.d...
-000000e0: 6517 6412 1900 8302 0100 6413 5300 2914  e.d.......d.S.).
-000000f0: e900 0000 0029 01da 012a e901 0000 0029  .....)...*.....)
-00000100: 02da 0670 6872 6173 65da 0a63 6869 6c64  ...phrase..child
-00000110: 496e 6465 78e9 0700 0000 2901 7205 0000  Index.....).r...
-00000120: 007a 0c73 6967 6e65 7233 2e6a 736f 6e29  .z.signer3.json)
-00000130: 02da 0866 696c 656e 616d 65da 0673 6967  ...filename..sig
-00000140: 6e65 7229 0172 0700 0000 da0f 5365 7463  ner).r......Setc
-00000150: 6f64 654d 756c 7469 7369 6729 0272 0800  odeMultisig).r..
-00000160: 0000 da0d 696e 6974 6961 6c50 7562 6b65  ....initialPubke
-00000170: 797a 144d 756c 7469 7369 6720 3120 6164  yz.Multisig 1 ad
-00000180: 6472 6573 733a 207a 144d 756c 7469 7369  dress: z.Multisi
-00000190: 6720 3120 6261 6c61 6e63 653a 2054 2901  g 1 balance: T).
-000001a0: da0b 7368 6f77 496e 4576 6572 73da 0230  ..showInEvers..0
-000001b0: 7829 02da 066f 776e 6572 73da 0b72 6571  x)...owners..req
-000001c0: 436f 6e66 6972 6d73 da06 7265 7375 6c74  Confirms..result
-000001d0: da09 6578 6365 7074 696f 6e4e 2918 da06  ..exceptionN)...
-000001e0: 6576 6572 7361 da03 6573 61da 1667 656e  eversa..esa..gen
-000001f0: 6572 6174 6552 616e 646f 6d4d 6e65 6d6f  erateRandomMnemo
-00000200: 6e69 6372 0400 0000 da1a 6765 6e65 7261  nicr......genera
-00000210: 7465 5369 676e 6572 4672 6f6d 4d6e 656d  teSignerFromMnem
-00000220: 6f6e 6963 da07 7369 676e 6572 31da 0967  onic..signer1..g
-00000230: 6574 5369 676e 6572 da07 7369 676e 6572  etSigner..signer
-00000240: 32da 1467 656e 6572 6174 6552 616e 646f  2..generateRando
-00000250: 6d53 6967 6e65 72da 0773 6967 6e65 7233  mSigner..signer3
-00000260: da0a 7361 7665 5369 676e 6572 da0a 6c6f  ..saveSigner..lo
-00000270: 6164 5369 676e 6572 da07 7369 676e 6572  adSigner..signer
-00000280: 34da 0b47 6574 436f 6e74 7261 6374 da04  4..GetContract..
-00000290: 6b65 7973 da06 7075 626c 6963 da05 6d73  keys..public..ms
-000002a0: 6967 31da 0761 6972 6472 6f70 da07 4144  ig1..airdrop..AD
-000002b0: 4452 4553 53da 0445 5645 52da 0570 7269  DRESS..EVER..pri
-000002c0: 6e74 da0a 6765 7442 616c 616e 6365 da06  nt..getBalance..
-000002d0: 6465 706c 6f79 720f 0000 00a9 0072 2700  deployr......r'.
-000002e0: 0000 7227 0000 00fa 3262 7569 6c64 2f62  ..r'....2build/b
-000002f0: 6469 7374 2e6c 696e 7578 2d78 3836 5f36  dist.linux-x86_6
-00000300: 342f 6567 672f 6576 6572 7361 2f73 616d  4/egg/eversa/sam
-00000310: 706c 652f 7465 7374 2e70 79da 083c 6d6f  ple/test.py..<mo
-00000320: 6475 6c65 3e01 0000 0073 1c00 0000 0804  dule>....s......
-00000330: 0607 0607 0c01 0c03 0603 0c03 0a01 1407  ................
-00000340: 0e01 1001 1601 1a03 1601                 ..........
+00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
+00000030: 6401 6c00 5400 6402 6500 6602 6403 6404  d.l.T.d.e.f.d.d.
+00000040: 8404 5a01 6402 6500 6602 6405 6406 8404  ..Z.d.e.f.d.d...
+00000050: 5a02 6503 6407 6b02 7223 6500 8300 5a04  Z.e.d.k.r#e...Z.
+00000060: 6501 6504 8301 0100 6502 6504 8301 0100  e.e.....e.e.....
+00000070: 6408 5300 6408 5300 2909 e900 0000 0029  d.S.d.S.)......)
+00000080: 01da 012a da03 6573 6163 0100 0000 0000  ...*..esac......
+00000090: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
+000000a0: 0000 733e 0000 0074 0083 007d 0174 017c  ..s>...t...}.t.|
+000000b0: 0164 0164 028d 027d 027c 006a 0264 0364  .d.d...}.|.j.d.d
+000000c0: 048d 017d 0374 0383 007d 0474 0464 057c  ...}.t...}.t.d.|
+000000d0: 0464 068d 0201 0074 0564 0564 078d 017d  .d.....t.d.d...}
+000000e0: 0564 0053 0029 084e e901 0000 0029 02da  .d.S.).N.....)..
+000000f0: 0670 6872 6173 65da 0a63 6869 6c64 496e  .phrase..childIn
+00000100: 6465 78e9 0700 0000 2901 7206 0000 007a  dex.....).r....z
+00000110: 0c73 6967 6e65 7233 2e6a 736f 6e29 02da  .signer3.json)..
+00000120: 086b 6579 7346 696c 65da 0673 6967 6e65  .keysFile..signe
+00000130: 7229 0172 0800 0000 2906 da16 6765 6e65  r).r....)...gene
+00000140: 7261 7465 5261 6e64 6f6d 4d6e 656d 6f6e  rateRandomMnemon
+00000150: 6963 da1a 6765 6e65 7261 7465 5369 676e  ic..generateSign
+00000160: 6572 4672 6f6d 4d6e 656d 6f6e 6963 da09  erFromMnemonic..
+00000170: 6765 7453 6967 6e65 72da 1467 656e 6572  getSigner..gener
+00000180: 6174 6552 616e 646f 6d53 6967 6e65 72da  ateRandomSigner.
+00000190: 0a73 6176 6553 6967 6e65 72da 0a6c 6f61  .saveSigner..loa
+000001a0: 6453 6967 6e65 7229 0672 0300 0000 7205  dSigner).r....r.
+000001b0: 0000 00da 0773 6967 6e65 7231 da07 7369  .....signer1..si
+000001c0: 676e 6572 32da 0773 6967 6e65 7233 da07  gner2..signer3..
+000001d0: 7369 676e 6572 34a9 0072 1400 0000 fa32  signer4..r.....2
+000001e0: 6275 696c 642f 6264 6973 742e 6c69 6e75  build/bdist.linu
+000001f0: 782d 7838 365f 3634 2f65 6767 2f65 7665  x-x86_64/egg/eve
+00000200: 7273 612f 7361 6d70 6c65 2f74 6573 742e  rsa/sample/test.
+00000210: 7079 da0b 7465 7374 5369 676e 6572 730a  py..testSigners.
+00000220: 0000 0073 0c00 0000 0603 0c01 0c03 0603  ...s............
+00000230: 0c03 0e01 7216 0000 0063 0100 0000 0000  ....r....c......
+00000240: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00000250: 0000 737e 0000 0074 0083 007d 017c 006a  ..s~...t...}.|.j
+00000260: 0164 017c 017c 016a 026a 0364 028d 037d  .d.|.|.j.j.d...}
+00000270: 027c 00a0 047c 026a 0574 06a1 0201 0074  .|...|.j.t.....t
+00000280: 0764 037c 026a 059b 009d 0283 0101 0074  .d.|.j.........t
+00000290: 0764 047c 026a 0864 0564 068d 019b 009d  .d.|.j.d.d......
+000002a0: 0283 0101 007c 026a 0964 077c 016a 026a  .....|.j.d.|.j.j
+000002b0: 039b 009d 0267 0164 0864 098d 027d 0374  .....g.d.d...}.t
+000002c0: 077c 0364 0a19 007c 0364 0b19 0083 0201  .|.d...|.d......
+000002d0: 0064 0053 0029 0c4e da0f 5365 7463 6f64  .d.S.).N..Setcod
+000002e0: 654d 756c 7469 7369 6729 0272 0900 0000  eMultisig).r....
+000002f0: da0d 696e 6974 6961 6c50 7562 6b65 797a  ..initialPubkeyz
+00000300: 144d 756c 7469 7369 6720 3120 6164 6472  .Multisig 1 addr
+00000310: 6573 733a 207a 144d 756c 7469 7369 6720  ess: z.Multisig 
+00000320: 3120 6261 6c61 6e63 653a 2054 2901 da0b  1 balance: T)...
+00000330: 7368 6f77 496e 4576 6572 73da 0230 7872  showInEvers..0xr
+00000340: 0400 0000 2902 da06 6f77 6e65 7273 da0b  ....)...owners..
+00000350: 7265 7143 6f6e 6669 726d 73da 0672 6573  reqConfirms..res
+00000360: 756c 74da 0965 7863 6570 7469 6f6e 290a  ult..exception).
+00000370: 720d 0000 00da 0b47 6574 436f 6e74 7261  r......GetContra
+00000380: 6374 da04 6b65 7973 da06 7075 626c 6963  ct..keys..public
+00000390: da07 6169 7264 726f 70da 0741 4444 5245  ..airdrop..ADDRE
+000003a0: 5353 da04 4556 4552 da05 7072 696e 74da  SS..EVER..print.
+000003b0: 0a67 6574 4261 6c61 6e63 65da 0664 6570  .getBalance..dep
+000003c0: 6c6f 7929 0472 0300 0000 7209 0000 00da  loy).r....r.....
+000003d0: 056d 7369 6731 721d 0000 0072 1400 0000  .msig1r....r....
+000003e0: 7214 0000 0072 1500 0000 da0d 7465 7374  r....r......test
+000003f0: 436f 6e74 7261 6374 731d 0000 0073 0e00  Contracts....s..
+00000400: 0000 0603 1403 0e01 1001 1601 1a03 1601  ................
+00000410: 7229 0000 00da 085f 5f6d 6169 6e5f 5f4e  r).....__main__N
+00000420: 2905 da06 6576 6572 7361 7216 0000 0072  )...eversar....r
+00000430: 2900 0000 da08 5f5f 6e61 6d65 5f5f 7203  ).....__name__r.
+00000440: 0000 0072 1400 0000 7214 0000 0072 1400  ...r....r....r..
+00000450: 0000 7215 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000460: 3e01 0000 0073 1000 0000 0804 0e05 0e13  >....s..........
+00000470: 0814 0601 0801 0c01 04fd                 ..........
```

