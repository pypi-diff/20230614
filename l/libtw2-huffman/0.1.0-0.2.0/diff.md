# Comparing `tmp/libtw2_huffman-0.1.0.tar.gz` & `tmp/libtw2_huffman-0.2.0.tar.gz`

## Comparing `libtw2_huffman-0.1.0.tar` & `libtw2_huffman-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 libtw2_huffman-0.1.0/local_dependencies/common/Cargo.toml
--rw-r--r--   0     1000      984     1312 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/benches/cast.rs
--rw-r--r--   0     1000      984        0 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/generate/__init__.py
--rw-r--r--   0     1000      984     4130 2023-05-31 13:36:12.000000 libtw2_huffman-0.1.0/local_dependencies/common/generate/cast.py
--rw-r--r--   0     1000      984      343 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/generate/types.py
--rw-r--r--   0     1000      984     3249 2022-08-03 22:47:18.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/digest.rs
--rw-r--r--   0     1000      984     1879 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/io.rs
--rw-r--r--   0     1000      984      439 2023-05-31 13:40:33.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/lib.rs
--rw-r--r--   0     1000      984     1330 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/macros.rs
--rw-r--r--   0     1000      984      754 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/map_iter.rs
--rw-r--r--   0     1000      984    26315 2023-05-31 13:36:15.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/num/cast.rs
--rw-r--r--   0     1000      984     6774 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/num/mod.rs
--rw-r--r--   0     1000      984     2687 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/pretty.rs
--rw-r--r--   0     1000      984      745 2022-11-28 23:32:05.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/slice.rs
--rw-r--r--   0     1000      984     1310 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/str.rs
--rw-r--r--   0     1000      984     1061 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/takeable.rs
--rw-r--r--   0     1000      984      432 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/common/src/vec.rs
--rw-r--r--   0        0        0      285 1970-01-01 00:00:00.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/Cargo.toml
--rw-r--r--   0     1000      984     4493 2022-11-28 16:12:20.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/benches/compression.rs
--rw-r--r--   0     1000      984      871 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/data/frequencies
--rw-r--r--   0     1000      984     2980 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/data/repr
--rw-r--r--   0     1000      984    26451 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/data/test_cases
--rw-r--r--   0     1000      984       64 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/src/instances/mod.rs
--rw-r--r--   0     1000      984    18241 2022-02-28 21:09:58.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/src/instances/teeworlds.rs
--rw-r--r--   0     1000      984    15451 2023-05-31 13:27:24.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/src/lib.rs
--rw-r--r--   0     1000      984      529 2022-11-28 15:50:04.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/src/main.rs
--rw-r--r--   0     1000      984     3179 2022-11-28 16:04:11.000000 libtw2_huffman-0.1.0/local_dependencies/huffman/tests/correctness.rs
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 libtw2_huffman-0.1.0/Cargo.toml
--rw-r--r--   0     1000      984       83 2023-06-14 10:56:32.000000 libtw2_huffman-0.1.0/build.rs
--rw-r--r--   0     1000      984      218 2023-06-14 10:54:17.000000 libtw2_huffman-0.1.0/pyproject.toml
--rw-r--r--   0     1000      984      593 2023-06-14 11:03:08.000000 libtw2_huffman-0.1.0/src/lib.rs
--rw-r--r--   0     1000      984      206 2023-05-24 09:55:38.000000 libtw2_huffman-0.1.0/src/libtw2_huffman.udl
--rw-r--r--   0     1000      984    20762 2023-06-14 11:28:49.000000 libtw2_huffman-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      244 1970-01-01 00:00:00.000000 libtw2_huffman-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 libtw2_huffman-0.2.0/local_dependencies/common/Cargo.toml
+-rw-r--r--   0     1000      984     1312 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/benches/cast.rs
+-rw-r--r--   0     1000      984        0 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/generate/__init__.py
+-rw-r--r--   0     1000      984     4130 2023-05-31 13:36:12.000000 libtw2_huffman-0.2.0/local_dependencies/common/generate/cast.py
+-rw-r--r--   0     1000      984      343 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/generate/types.py
+-rw-r--r--   0     1000      984     3249 2022-08-03 22:47:18.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/digest.rs
+-rw-r--r--   0     1000      984     1879 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/io.rs
+-rw-r--r--   0     1000      984      439 2023-05-31 13:40:33.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/lib.rs
+-rw-r--r--   0     1000      984     1330 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/macros.rs
+-rw-r--r--   0     1000      984      754 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/map_iter.rs
+-rw-r--r--   0     1000      984    26315 2023-05-31 13:36:15.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/num/cast.rs
+-rw-r--r--   0     1000      984     6774 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/num/mod.rs
+-rw-r--r--   0     1000      984     2687 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/pretty.rs
+-rw-r--r--   0     1000      984      745 2022-11-28 23:32:05.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/slice.rs
+-rw-r--r--   0     1000      984     1310 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/str.rs
+-rw-r--r--   0     1000      984     1061 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/takeable.rs
+-rw-r--r--   0     1000      984      432 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/common/src/vec.rs
+-rw-r--r--   0        0        0      285 1970-01-01 00:00:00.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/Cargo.toml
+-rw-r--r--   0     1000      984     4493 2022-11-28 16:12:20.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/benches/compression.rs
+-rw-r--r--   0     1000      984      871 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/data/frequencies
+-rw-r--r--   0     1000      984     2980 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/data/repr
+-rw-r--r--   0     1000      984    26451 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/data/test_cases
+-rw-r--r--   0     1000      984       64 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/src/instances/mod.rs
+-rw-r--r--   0     1000      984    18241 2022-02-28 21:09:58.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/src/instances/teeworlds.rs
+-rw-r--r--   0     1000      984    15451 2023-05-31 13:27:24.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/src/lib.rs
+-rw-r--r--   0     1000      984      529 2022-11-28 15:50:04.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/src/main.rs
+-rw-r--r--   0     1000      984     3179 2022-11-28 16:04:11.000000 libtw2_huffman-0.2.0/local_dependencies/huffman/tests/correctness.rs
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 libtw2_huffman-0.2.0/Cargo.toml
+-rw-r--r--   0     1000      984       83 2023-06-14 10:56:32.000000 libtw2_huffman-0.2.0/build.rs
+-rw-r--r--   0     1000      984      266 2023-06-14 12:20:03.000000 libtw2_huffman-0.2.0/pyproject.toml
+-rw-r--r--   0     1000      984      593 2023-06-14 11:03:08.000000 libtw2_huffman-0.2.0/src/lib.rs
+-rw-r--r--   0     1000      984      206 2023-05-24 09:55:38.000000 libtw2_huffman-0.2.0/src/libtw2_huffman.udl
+-rw-r--r--   0     1000      984    20762 2023-06-14 12:13:01.000000 libtw2_huffman-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      244 1970-01-01 00:00:00.000000 libtw2_huffman-0.2.0/PKG-INFO
```

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/benches/cast.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/benches/cast.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/generate/cast.py` & `libtw2_huffman-0.2.0/local_dependencies/common/generate/cast.py`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/digest.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/digest.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/io.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/io.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/macros.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/macros.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/map_iter.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/map_iter.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/num/cast.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/num/cast.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/num/mod.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/num/mod.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/pretty.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/pretty.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/slice.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/slice.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/str.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/str.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/common/src/takeable.rs` & `libtw2_huffman-0.2.0/local_dependencies/common/src/takeable.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/benches/compression.rs` & `libtw2_huffman-0.2.0/local_dependencies/huffman/benches/compression.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/data/frequencies` & `libtw2_huffman-0.2.0/local_dependencies/huffman/data/frequencies`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/data/test_cases` & `libtw2_huffman-0.2.0/local_dependencies/huffman/data/test_cases`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/src/instances/teeworlds.rs` & `libtw2_huffman-0.2.0/local_dependencies/huffman/src/instances/teeworlds.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/src/lib.rs` & `libtw2_huffman-0.2.0/local_dependencies/huffman/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/src/main.rs` & `libtw2_huffman-0.2.0/local_dependencies/huffman/src/main.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/local_dependencies/huffman/tests/correctness.rs` & `libtw2_huffman-0.2.0/local_dependencies/huffman/tests/correctness.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/Cargo.toml` & `libtw2_huffman-0.2.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uniffi-huffman"
-version = "0.1.0"
+version = "0.2.0"
 authors = ["heinrich5991 <heinrich5991@gmail.com>"]
 license = "MIT/Apache-2.0"
 
 [lib]
 name = "libtw2_huffman"
 crate-type = ["cdylib"]
```

### Comparing `libtw2_huffman-0.1.0/src/lib.rs` & `libtw2_huffman-0.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `libtw2_huffman-0.1.0/Cargo.lock` & `libtw2_huffman-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,15 @@
 version = "0.2.0"
 dependencies = [
  "uniffi",
 ]
 
 [[package]]
 name = "uniffi-huffman"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "huffman",
  "uniffi",
 ]
 
 [[package]]
 name = "uniffi_bindgen"
```

