# Comparing `tmp/pyxirr-0.9.1.tar.gz` & `tmp/pyxirr-0.9.2.tar.gz`

## Comparing `pyxirr-0.9.1.tar` & `pyxirr-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 pyxirr-0.9.1/Cargo.toml
--rw-r--r--   0     1001      123     1211 2023-06-03 15:24:17.000000 pyxirr-0.9.1/LICENSE
--rw-r--r--   0     1001      123     5742 2023-06-03 15:24:17.000000 pyxirr-0.9.1/README.md
--rw-r--r--   0     1001      123      895 2023-06-03 15:24:17.000000 pyxirr-0.9.1/pyproject.toml
--rw-r--r--   0     1001      123     7998 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/broadcasting.rs
--rw-r--r--   0     1001      123     8776 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/conversions.rs
--rw-r--r--   0     1001      123      263 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/mod.rs
--rw-r--r--   0     1001      123     1942 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/models.rs
--rw-r--r--   0     1001      123     4026 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/optimize.rs
--rw-r--r--   0     1001      123    14548 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/periodic.rs
--rw-r--r--   0     1001      123    12268 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/day_count.rs
--rw-r--r--   0     1001      123      151 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/mod.rs
--rw-r--r--   0     1001      123     1963 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/xirr.rs
--rw-r--r--   0     1001      123     1253 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/core/scheduled/xnfv.rs
--rw-r--r--   0     1001      123    14395 2023-06-03 15:24:17.000000 pyxirr-0.9.1/src/lib.rs
--rw-r--r--   0     1001      123    13819 2023-06-03 15:24:17.000000 pyxirr-0.9.1/Cargo.lock
--rw-r--r--   0     1001      123      374 2023-06-03 15:24:17.000000 pyxirr-0.9.1/.cargo/config
--rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 pyxirr-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 pyxirr-0.9.2/Cargo.toml
+-rw-r--r--   0     1001      123     1211 2023-06-14 08:44:13.000000 pyxirr-0.9.2/LICENSE
+-rw-r--r--   0     1001      123     5742 2023-06-14 08:44:13.000000 pyxirr-0.9.2/README.md
+-rw-r--r--   0     1001      123      895 2023-06-14 08:44:13.000000 pyxirr-0.9.2/pyproject.toml
+-rw-r--r--   0     1001      123     7998 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/broadcasting.rs
+-rw-r--r--   0     1001      123     8776 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/conversions.rs
+-rw-r--r--   0     1001      123      263 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/mod.rs
+-rw-r--r--   0     1001      123     1942 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/models.rs
+-rw-r--r--   0     1001      123     4026 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/optimize.rs
+-rw-r--r--   0     1001      123    14548 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/periodic.rs
+-rw-r--r--   0     1001      123    12268 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/scheduled/day_count.rs
+-rw-r--r--   0     1001      123      151 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/scheduled/mod.rs
+-rw-r--r--   0     1001      123     1963 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/scheduled/xirr.rs
+-rw-r--r--   0     1001      123     1253 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/core/scheduled/xnfv.rs
+-rw-r--r--   0     1001      123    14523 2023-06-14 08:44:13.000000 pyxirr-0.9.2/src/lib.rs
+-rw-r--r--   0     1001      123    13819 2023-06-14 08:44:13.000000 pyxirr-0.9.2/Cargo.lock
+-rw-r--r--   0     1001      123      374 2023-06-14 08:44:13.000000 pyxirr-0.9.2/.cargo/config
+-rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 pyxirr-0.9.2/PKG-INFO
```

### Comparing `pyxirr-0.9.1/Cargo.toml` & `pyxirr-0.9.2/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyxirr"
-version = "0.9.1"
+version = "0.9.2"
 authors = ["Anexen"]
 edition = "2021"
 description = "Rust-powered collection of financial functions for Python."
 readme = "README.md"
 homepage = "https://github.com/Anexen/pyxirr"
 license = "Unlicense"
 keywords = [
@@ -23,19 +23,19 @@
 ]
 
 [lib]
 name = "pyxirr"
 crate-type = ["rlib", "cdylib"]
 
 [dependencies]
-pyo3 = "0.18"
-numpy = "0.18"
+pyo3 = "0.19"
+numpy = "0.19"
 time = { version = "0.3", features = ["parsing", "macros"] }
 ndarray = "0.15"
 
 [dev-dependencies]
-rstest = "0.16"
+rstest = "0.17"
 
 [features]
 default = ["pyo3/extension-module"]
 tests = ["pyo3/auto-initialize"]
 nonumpy = []
```

### Comparing `pyxirr-0.9.1/LICENSE` & `pyxirr-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/README.md` & `pyxirr-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/pyproject.toml` & `pyxirr-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/broadcasting.rs` & `pyxirr-0.9.2/src/broadcasting.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/conversions.rs` & `pyxirr-0.9.2/src/conversions.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/core/models.rs` & `pyxirr-0.9.2/src/core/models.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/core/optimize.rs` & `pyxirr-0.9.2/src/core/optimize.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/core/periodic.rs` & `pyxirr-0.9.2/src/core/periodic.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/core/scheduled/day_count.rs` & `pyxirr-0.9.2/src/core/scheduled/day_count.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/core/scheduled/xirr.rs` & `pyxirr-0.9.2/src/core/scheduled/xirr.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/core/scheduled/xnfv.rs` & `pyxirr-0.9.2/src/core/scheduled/xnfv.rs`

 * *Files identical despite different names*

### Comparing `pyxirr-0.9.1/src/lib.rs` & `pyxirr-0.9.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -186,26 +186,30 @@
             day_count,
         )))
     })
 }
 
 /// Net future value of a series of irregular cash flows
 #[pyfunction]
-#[pyo3(signature = (rate, dates, amounts=None, *, day_count=None))]
-#[pyo3(text_signature = "(rate, dates, *, amounts=None, day_count=None)")]
+#[pyo3(signature = (rate, dates, amounts=None, *, silent=false, day_count=None))]
+#[pyo3(text_signature = "(rate, dates, amounts=None, *, silent=False, day_count=None)")]
 fn xnfv(
     py: Python,
     rate: f64,
     dates: &PyAny,
     amounts: Option<&PyAny>,
+    silent: Option<bool>,
     day_count: Option<PyDayCount>,
 ) -> PyResult<Option<f64>> {
     let (dates, amounts) = conversions::extract_payments(dates, amounts)?;
     let day_count = day_count.map(|x| x.try_into()).transpose()?;
-    py.allow_threads(move || Ok(float_or_none(core::xnfv(rate, &dates, &amounts, day_count)?)))
+    py.allow_threads(move || {
+        let result = core::xnfv(rate, &dates, &amounts, day_count);
+        fallible_float_or_none(result, silent.unwrap_or(false))
+    })
 }
 
 /// Present Value
 #[pyfunction]
 #[pyo3(signature = (rate, nper, pmt, fv=Arg::Scalar(0.0), *, pmt_at_beginning=Arg::Scalar(false)))]
 #[pyo3(text_signature = "(rate, nper, pmt, fv=0, *, pmt_at_beginning=False)")]
 fn pv<'a>(
```

### Comparing `pyxirr-0.9.1/Cargo.lock` & `pyxirr-0.9.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.4"
@@ -209,17 +209,17 @@
 checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
+checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -274,75 +274,75 @@
 checksum = "dd96a1e8ed2596c337f8eae5f24924ec83f5ad5ab21ea8e455d3566c69fbcaf7"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyxirr"
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
  "ndarray",
  "numpy",
  "pyo3",
  "rstest",
  "time",
 ]
@@ -369,29 +369,29 @@
 checksum = "62f25bc4c7e55e0b0b7a1d43fb893f4fa1361d0abe38b9ce4f323c2adfe6ef42"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rstest"
-version = "0.16.0"
+version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b07f2d176c472198ec1e6551dc7da28f1c089652f66a7b722676c2238ebc0edf"
+checksum = "de1bb486a691878cd320c2f0d319ba91eeaa2e894066d8b5f8f117c000e9d962"
 dependencies = [
  "futures",
  "futures-timer",
  "rstest_macros",
  "rustc_version",
 ]
 
 [[package]]
 name = "rstest_macros"
-version = "0.16.0"
+version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7229b505ae0706e64f37ffc54a9c163e11022a6636d58fe1f3f52018257ff9f7"
+checksum = "290ca1a1c8ca7edb7c3283bd44dc35dd54fdec6253a3912e201ba1072018fca8"
 dependencies = [
  "cfg-if",
  "proc-macro2",
  "quote",
  "rustc_version",
  "syn",
  "unicode-ident",
```

### Comparing `pyxirr-0.9.1/PKG-INFO` & `pyxirr-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxirr
-Version: 0.9.1
+Version: 0.9.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

