# Comparing `tmp/libtw2_uniffi_bindgen-0.1.0.tar.gz` & `tmp/libtw2_uniffi_bindgen-0.2.0.tar.gz`

## Comparing `libtw2_uniffi_bindgen-0.1.0.tar` & `libtw2_uniffi_bindgen-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      283 1970-01-01 00:00:00.000000 libtw2_uniffi_bindgen-0.1.0/Cargo.toml
--rw-r--r--   0     1000      984      116 2023-06-14 09:53:13.000000 libtw2_uniffi_bindgen-0.1.0/pyproject.toml
--rw-r--r--   0     1000      984       70 2023-05-23 22:53:52.000000 libtw2_uniffi_bindgen-0.1.0/src/main.rs
--rw-r--r--   0     1000      984    20778 2023-06-14 09:48:25.000000 libtw2_uniffi_bindgen-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      187 1970-01-01 00:00:00.000000 libtw2_uniffi_bindgen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 libtw2_uniffi_bindgen-0.2.0/Cargo.toml
+-rw-r--r--   0     1000      984      116 2023-06-14 09:53:13.000000 libtw2_uniffi_bindgen-0.2.0/pyproject.toml
+-rw-r--r--   0     1000      984       70 2023-05-23 22:53:52.000000 libtw2_uniffi_bindgen-0.2.0/src/main.rs
+-rw-r--r--   0     1000      984    20771 2023-06-14 10:11:54.000000 libtw2_uniffi_bindgen-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      187 1970-01-01 00:00:00.000000 libtw2_uniffi_bindgen-0.2.0/PKG-INFO
```

### Comparing `libtw2_uniffi_bindgen-0.1.0/Cargo.lock` & `libtw2_uniffi_bindgen-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -340,21 +340,14 @@
 [[package]]
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
-name = "libtw2-uniffi-bindgen"
-version = "0.1.0"
-dependencies = [
- "uniffi",
-]
-
-[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "log"
@@ -617,14 +610,21 @@
  "uniffi_bindgen",
  "uniffi_build",
  "uniffi_core",
  "uniffi_macros",
 ]
 
 [[package]]
+name = "uniffi-bindgen"
+version = "0.2.0"
+dependencies = [
+ "uniffi",
+]
+
+[[package]]
 name = "uniffi-huffman"
 version = "0.0.1"
 dependencies = [
  "huffman",
  "uniffi",
 ]
```

