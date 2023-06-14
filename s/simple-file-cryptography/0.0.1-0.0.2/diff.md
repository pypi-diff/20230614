# Comparing `tmp/simple_file_cryptography-0.0.1.tar.gz` & `tmp/simple_file_cryptography-0.0.2.tar.gz`

## Comparing `simple_file_cryptography-0.0.1.tar` & `simple_file_cryptography-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/__about__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/__main__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/crypto_utility.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/gui.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/mode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/src/simple_file_cryptography/py.typed
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/README.md
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/__about__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/__init__.py
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/__main__.py
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/crypto_utility.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/gui.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/mode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/src/simple_file_cryptography/py.typed
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/README.md
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 simple_file_cryptography-0.0.2/PKG-INFO
```

### Comparing `simple_file_cryptography-0.0.1/src/simple_file_cryptography/__main__.py` & `simple_file_cryptography-0.0.2/src/simple_file_cryptography/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from simple_file_cryptography.crypto_utility import generate_key, decrypt_file, encrypt_file
 import argparse
 import simple_file_cryptography.gui as gui
 
+
 def main():
     parser = argparse.ArgumentParser(
         prog='Simple file cryptography',
         description='Encrypts and decrypts files.')
 
     parser.add_argument(
         "-m",
```

### Comparing `simple_file_cryptography-0.0.1/src/simple_file_cryptography/crypto_utility.py` & `simple_file_cryptography-0.0.2/src/simple_file_cryptography/crypto_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import os
 from typing import Union
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
+
 def _encrypt_file(file_path_from: str, file_path_to: str, key: bytes):
     nonce = os.urandom(16)
     cipher = Cipher(algorithms.AES(key), modes.CTR(nonce))
     encryptor = cipher.encryptor()
 
-    with open(file_path_to, 'wb') as file_to:
+    with open(file_path_to, 'wb', buffering=33554432) as file_to:
         file_to.write(nonce)
 
-        with open(file_path_from, 'rb') as file_from:
+        with open(file_path_from, 'rb', buffering=33554432) as file_from:
             while True:
                 piece = file_from.read(16)
                 file_to.write(encryptor.update(piece))
 
                 if len(piece) < 16:
                     break
 
             file_to.write(encryptor.finalize())
 
 
 def _decrypt_file(file_path_from: str, file_path_to: str, key: bytes):
 
-    with open(file_path_from, 'rb') as file_from:
+    with open(file_path_from, 'rb', buffering=33554432) as file_from:
         nonce = file_from.read(16)
         cipher = Cipher(algorithms.AES(key), modes.CTR(nonce))
         decryptor = cipher.decryptor()
-        with open(file_path_to, 'wb') as file_to:
+        with open(file_path_to, 'wb', buffering=33554432) as file_to:
             while True:
                 piece = file_from.read(16)
                 file_to.write(decryptor.update(piece))
 
                 if len(piece) < 16:
                     break
 
@@ -71,8 +72,8 @@
 
 def generate_key(size: int = 16) -> bytes:
     """
     A simple convenience function that will generate 16 random bytes (128 bits).
     You may use `.hex()` method on received `bytes`, to get hexadecimal string
     representation.
     """
-    return os.urandom(size)
+    return os.urandom(size)
```

### Comparing `simple_file_cryptography-0.0.1/src/simple_file_cryptography/gui.py` & `simple_file_cryptography-0.0.2/src/simple_file_cryptography/gui.py`

 * *Files identical despite different names*

### Comparing `simple_file_cryptography-0.0.1/LICENSE.txt` & `simple_file_cryptography-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_file_cryptography-0.0.1/README.md` & `simple_file_cryptography-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simple_file_cryptography-0.0.1/pyproject.toml` & `simple_file_cryptography-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_file_cryptography-0.0.1/PKG-INFO` & `simple_file_cryptography-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-file-cryptography
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/simple-file-cryptography#readme
 Project-URL: Issues, https://github.com/unknown/simple-file-cryptography/issues
 Project-URL: Source, https://github.com/unknown/simple-file-cryptography
 Author-email: Filip Strajnar <filip.strajnar@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

