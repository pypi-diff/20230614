# Comparing `tmp/mcai_worker_sdk_media-2.0.0rc8.tar.gz` & `tmp/mcai_worker_sdk_media-2.0.0rc9.tar.gz`

## Comparing `mcai_worker_sdk_media-2.0.0rc8.tar` & `mcai_worker_sdk_media-2.0.0rc9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 mcai_worker_sdk_media-2.0.0rc8/Cargo.toml
--rwxrwxrwx   0        0        0     1154 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/.chglog/CHANGELOG.tpl.md
--rwxrwxrwx   0        0        0      554 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/.chglog/config.yml
--rw-rw-rw-   0        0        0      283 2023-02-13 14:28:57.000000 mcai_worker_sdk_media-2.0.0rc8/.gitignore
--rw-rw-rw-   0        0        0     2302 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      500 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/.readthedocs.yaml
--rw-rw-rw-   0        0        0     2075 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/CHANGELOG.md
--rw-rw-rw-   0        0        0     1083 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/LICENSE
--rw-rw-rw-   0        0        0     2834 2023-02-13 11:19:02.000000 mcai_worker_sdk_media-2.0.0rc8/README.md
--rw-rw-rw-   0        0        0     2371 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/build.rs
--rw-rw-rw-   0        0        0      634 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/Makefile
--rw-rw-rw-   0        0        0     2281 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/docs/conf.py
--rw-rw-rw-   0        0        0     7288 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/docs/index.rst
--rw-rw-rw-   0        0        0       92 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/job_status.rst
--rw-rw-rw-   0        0        0      765 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/make.bat
--rw-rw-rw-   0        0        0       98 2023-02-13 11:19:02.000000 mcai_worker_sdk_media-2.0.0rc8/docs/mcai_channel.rst
--rw-rw-rw-   0        0        0       94 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/media/filter.rst
--rw-rw-rw-   0        0        0       88 2023-01-11 10:58:19.000000 mcai_worker_sdk_media-2.0.0rc8/docs/media/format_context.rst
--rw-rw-rw-   0        0        0       62 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/media/frame.rst
--rw-rw-rw-   0        0        0      486 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/media/stream_descriptor.rst
--rw-rw-rw-   0        0        0       22 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/docs/requirements.media.txt
--rw-rw-rw-   0        0        0       16 2023-03-03 15:50:27.000000 mcai_worker_sdk_media-2.0.0rc8/docs/requirements.txt
--rw-rw-rw-   0        0        0      764 2023-02-13 11:19:02.000000 mcai_worker_sdk_media-2.0.0rc8/docs/sphinx-ext/toctree_filter.py
--rw-rw-rw-   0        0        0      264 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/worker.rst
--rw-rw-rw-   0        0        0      145 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/docs/worker_description.rst
--rw-rw-rw-   0        0        0       96 2023-01-11 10:58:19.000000 mcai_worker_sdk_media-2.0.0rc8/docs/worker_parameters.rst
--rw-rw-rw-   0        0        0     5181 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/examples/media_worker.py
--rw-rw-rw-   0        0        0      693 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/examples/message.json
--rw-rw-rw-   0        0        0     1892 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/examples/worker.py
--rw-r--r--   0        0        0      460 2023-03-03 16:37:29.000000 mcai_worker_sdk_media-2.0.0rc8/pyproject.toml
--rw-rw-rw-   0        0        0       16 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/release.toml
--rw-rw-rw-   0        0        0       15 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/rustfmt.toml
--rw-rw-rw-   0        0        0     2058 2023-03-03 15:06:39.000000 mcai_worker_sdk_media-2.0.0rc8/src/callback.rs
--rw-rw-rw-   0        0        0     4168 2023-03-03 15:06:39.000000 mcai_worker_sdk_media-2.0.0rc8/src/description.rs
--rw-rw-rw-   0        0        0     2330 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/helper.rs
--rw-rw-rw-   0        0        0     6517 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/instance.rs
--rw-rw-rw-   0        0        0     1093 2023-01-11 10:58:19.000000 mcai_worker_sdk_media-2.0.0rc8/src/lib.rs
--rw-rw-rw-   0        0        0      166 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/logger/mcai_logs_handler.py
--rw-rw-rw-   0        0        0     1619 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/logger/mod.rs
--rw-rw-rw-   0        0        0     5991 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/ebu_ttml_live/mod.rs
--rw-rw-rw-   0        0        0     4811 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/ebu_ttml_live/time_expression.rs
--rw-rw-rw-   0        0        0     3812 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/filter.rs
--rw-rw-rw-   0        0        0     4022 2023-01-11 10:58:19.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/format_context.rs
--rw-rw-rw-   0        0        0     3797 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/frame.rs
--rw-rw-rw-   0        0        0      674 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/mod.rs
--rw-rw-rw-   0        0        0     6282 2023-01-10 15:08:49.000000 mcai_worker_sdk_media-2.0.0rc8/src/media/stream_descriptor.rs
--rw-rw-rw-   0        0        0     9189 2023-03-03 15:06:39.000000 mcai_worker_sdk_media-2.0.0rc8/src/parameters.rs
--rw-rw-rw-   0        0        0     5549 2023-03-03 15:06:39.000000 mcai_worker_sdk_media-2.0.0rc8/src/worker.rs
--rw-rw-rw-   0        0        0    86305 2023-03-03 16:11:04.000000 mcai_worker_sdk_media-2.0.0rc8/Cargo.lock
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 mcai_worker_sdk_media-2.0.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 mcai_worker_sdk_media-2.0.0rc9/Cargo.toml
+-rw-rw-rw-   0        0        0      112 2023-03-29 11:10:14.000000 mcai_worker_sdk_media-2.0.0rc9/.cargo/config.toml
+-rwxrwxrwx   0        0        0     1154 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/.chglog/CHANGELOG.tpl.md
+-rwxrwxrwx   0        0        0      554 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/.chglog/config.yml
+-rw-rw-rw-   0        0        0      283 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/.gitignore
+-rw-rw-rw-   0        0        0     2302 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      500 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     2075 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1083 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc9/LICENSE
+-rw-rw-rw-   0        0        0     2964 2023-04-13 11:40:22.000000 mcai_worker_sdk_media-2.0.0rc9/README.md
+-rw-rw-rw-   0        0        0     2371 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/build.rs
+-rw-rw-rw-   0        0        0      634 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/Makefile
+-rw-rw-rw-   0        0        0     2281 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/conf.py
+-rw-rw-rw-   0        0        0     7288 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/index.rst
+-rw-rw-rw-   0        0        0       92 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/job_status.rst
+-rw-rw-rw-   0        0        0      765 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/make.bat
+-rw-rw-rw-   0        0        0       98 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/mcai_channel.rst
+-rw-rw-rw-   0        0        0       94 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/media/filter.rst
+-rw-rw-rw-   0        0        0       88 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/media/format_context.rst
+-rw-rw-rw-   0        0        0       62 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/media/frame.rst
+-rw-rw-rw-   0        0        0      486 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/media/stream_descriptor.rst
+-rw-rw-rw-   0        0        0       22 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/requirements.media.txt
+-rw-rw-rw-   0        0        0       16 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/requirements.txt
+-rw-rw-rw-   0        0        0      764 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/sphinx-ext/toctree_filter.py
+-rw-rw-rw-   0        0        0      264 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/worker.rst
+-rw-rw-rw-   0        0        0      145 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/worker_description.rst
+-rw-rw-rw-   0        0        0       96 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/docs/worker_parameters.rst
+-rw-rw-rw-   0        0        0     5181 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/examples/media_worker.py
+-rw-rw-rw-   0        0        0      693 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/examples/message.json
+-rw-rw-rw-   0        0        0     1892 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/examples/worker.py
+-rw-r--r--   0        0        0      460 2023-04-17 09:05:10.000000 mcai_worker_sdk_media-2.0.0rc9/pyproject.toml
+-rw-rw-rw-   0        0        0       16 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/release.toml
+-rw-rw-rw-   0        0        0       15 2023-01-10 14:53:55.000000 mcai_worker_sdk_media-2.0.0rc9/rustfmt.toml
+-rw-rw-rw-   0        0        0     2058 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/callback.rs
+-rw-rw-rw-   0        0        0     4168 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/description.rs
+-rw-rw-rw-   0        0        0     3200 2023-04-03 08:59:14.000000 mcai_worker_sdk_media-2.0.0rc9/src/helper.rs
+-rw-rw-rw-   0        0        0     6560 2023-04-13 10:16:54.000000 mcai_worker_sdk_media-2.0.0rc9/src/instance.rs
+-rw-rw-rw-   0        0        0     1093 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/lib.rs
+-rw-rw-rw-   0        0        0      166 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/logger/mcai_logs_handler.py
+-rw-rw-rw-   0        0        0     1619 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/logger/mod.rs
+-rw-rw-rw-   0        0        0     5991 2023-03-28 07:32:53.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/ebu_ttml_live/mod.rs
+-rw-rw-rw-   0        0        0     4811 2023-03-28 07:32:53.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/ebu_ttml_live/time_expression.rs
+-rw-rw-rw-   0        0        0     3812 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/filter.rs
+-rw-rw-rw-   0        0        0     4140 2023-04-13 10:16:54.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/format_context.rs
+-rw-rw-rw-   0        0        0     3797 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/frame.rs
+-rw-rw-rw-   0        0        0      674 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/mod.rs
+-rw-rw-rw-   0        0        0     6282 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/media/stream_descriptor.rs
+-rw-rw-rw-   0        0        0     9704 2023-04-03 08:59:14.000000 mcai_worker_sdk_media-2.0.0rc9/src/parameters.rs
+-rw-rw-rw-   0        0        0     5549 2023-03-28 14:16:45.000000 mcai_worker_sdk_media-2.0.0rc9/src/worker.rs
+-rw-rw-rw-   0        0        0    86206 2023-04-17 08:38:32.000000 mcai_worker_sdk_media-2.0.0rc9/Cargo.lock
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 mcai_worker_sdk_media-2.0.0rc9/PKG-INFO
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/Cargo.toml` & `mcai_worker_sdk_media-2.0.0rc9/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py_mcai_worker_sdk"
-version = "2.0.0-rc8"
+version = "2.0.0-rc9"
 authors = [
   "Valentin NOEL <valentin.noel@media-io.com>",
   "Marc-Antoine Arnaud <maarnaud@media-io.com>",
   "Thibaud Le Graverend <thibaud.legraverend@luminvent.com>"
 ]
 description = "MCAI SDK to develop Python worker"
 keywords = ["AMQP", "micro-service", "python"]
@@ -19,24 +19,26 @@
 name = "mcai_worker_sdk"
 crate-type = ["cdylib"]
 
 [features]
 default = []
 media = [
   "mcai_worker_sdk/media",
+  "stainless_ffmpeg",
 ]
 extension-module = ["pyo3/extension-module"]
 
 [dependencies]
 async-std = "1.12.0"
 jsonschema = "0.16.0"
-mcai_worker_sdk = "2.0.0-rc4"
+mcai_worker_sdk = "2.0.0-rc5"
 pyo3 = {version="0.17.2", features=["multiple-pymethods"]}
 pyproject-toml = "0.3"
 schemars = "0.8.0"
 serde = "^1.0"
 serde_derive = "^1.0"
 serde_json = "^1.0"
+stainless_ffmpeg = { version = "0.3.5", optional = true }
 
 [build-dependencies]
 serde = "^1.0"
 toml = "0.5.9"
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/.chglog/CHANGELOG.tpl.md` & `mcai_worker_sdk_media-2.0.0rc9/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/.chglog/config.yml` & `mcai_worker_sdk_media-2.0.0rc9/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/.gitlab-ci.yml` & `mcai_worker_sdk_media-2.0.0rc9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/CHANGELOG.md` & `mcai_worker_sdk_media-2.0.0rc9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/LICENSE` & `mcai_worker_sdk_media-2.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/README.md` & `mcai_worker_sdk_media-2.0.0rc9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,20 +39,20 @@
 ### Supported version
 
 We intempt to support as many distribution and architecture as we can, however if `pip` doesn't find any compatible version for your installation it will download the source and try to compile them directly.
 
 This operation supposes that you have at least __Rust 1.62__.
 
 We currently support the following version of Python implementations:
-- [x] CPython 3.8
-- [x] CPython 3.9
-- [x] CPython 3.10
-- [x] CPython 3.11
-- [x] Pypy 3.8
-- [x] Pypy 3.9
+- [x] CPython 3.8 : manylinux
+- [x] CPython 3.9 : manylinux, macosx x86_64
+- [x] CPython 3.10 : manylinux, macosx x86_64, macosx arm64
+- [x] CPython 3.11 : manylinux, macosx arm54
+- [x] Pypy 3.8 : manylinux
+- [x] Pypy 3.9 : manylinux
 
 And the following core architectures:
 - [x] x86_64
 
 
 ## Test
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/build.rs` & `mcai_worker_sdk_media-2.0.0rc9/build.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/docs/Makefile` & `mcai_worker_sdk_media-2.0.0rc9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/docs/conf.py` & `mcai_worker_sdk_media-2.0.0rc9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/docs/index.rst` & `mcai_worker_sdk_media-2.0.0rc9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/docs/make.bat` & `mcai_worker_sdk_media-2.0.0rc9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/docs/sphinx-ext/toctree_filter.py` & `mcai_worker_sdk_media-2.0.0rc9/docs/sphinx-ext/toctree_filter.py`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/examples/media_worker.py` & `mcai_worker_sdk_media-2.0.0rc9/examples/media_worker.py`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/examples/message.json` & `mcai_worker_sdk_media-2.0.0rc9/examples/message.json`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/examples/worker.py` & `mcai_worker_sdk_media-2.0.0rc9/examples/worker.py`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/callback.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/callback.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/description.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/description.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/instance.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/instance.rs`

 * *Files 3% similar despite different names*

```diff
@@ -124,15 +124,15 @@
       .map_err(|error_message| {
         let result = job_result
           .with_status(JobStatus::Error)
           .with_message(&error_message.to_string());
         MessageError::ProcessingError(result)
       })?;
 
-      Ok(ProcessResult::new_json(&response.to_string()))
+      Ok(ProcessResult::new_json(response.to_string()))
     } else if !ebu_ttml_frames.is_empty() {
       let response = Python::with_gil(|py| -> PyResult<PyObject> {
         self.worker.call_method1(
           py,
           media::WORKER_METHOD_PROCESS_EBU_TTML_LIVE,
           (&job_result.get_str_job_id(), stream_index, ebu_ttml_frames),
         )
@@ -140,15 +140,15 @@
       .map_err(|error_message| {
         let result = job_result
           .with_status(JobStatus::Error)
           .with_message(&error_message.to_string());
         MessageError::ProcessingError(result)
       })?;
 
-      Ok(ProcessResult::new_json(&response.to_string()))
+      Ok(ProcessResult::new_json(response.to_string()))
     } else {
       Err(MessageError::NotImplemented())
     }
   }
 
   #[cfg(feature = "media")]
   fn ending_process(&mut self) -> Result<()> {
@@ -208,17 +208,18 @@
     .map_err(|error_message| {
       let result = job_result_cloned
         .with_status(JobStatus::Error)
         .with_message(&error_message.to_string());
       MessageError::ProcessingError(result)
     })?;
 
+    // If no status has been set, default to Completed
     let final_status = job_status
       .lock()
       .unwrap()
       .as_ref()
-      .unwrap_or_else(|| job_result.get_status())
+      .unwrap_or(&JobStatus::Completed)
       .clone();
 
     Ok(job_result.with_status(final_status))
   }
 }
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/lib.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/logger/mod.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/logger/mod.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/ebu_ttml_live/mod.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/ebu_ttml_live/mod.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/ebu_ttml_live/time_expression.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/ebu_ttml_live/time_expression.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/filter.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/filter.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/format_context.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/format_context.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use pyo3::prelude::*;
 use serde::{Deserialize, Serialize};
+use stainless_ffmpeg::stream::Stream;
 use std::{
   collections::{BTreeMap, HashMap},
   sync::{Arc, Mutex},
 };
 
 #[pyclass]
 #[derive(Debug, Deserialize, PartialEq, Serialize)]
@@ -55,30 +56,32 @@
     let packet_size = context.get_packet_size();
     let nb_streams = context.get_nb_streams();
 
     let metadata = context.get_metadata();
     let mut streams = vec![];
 
     for stream_index in 0..context.get_nb_streams() {
-      let stream = context.get_stream(stream_index as isize);
+      let stream = Stream::new(context.get_stream(stream_index as isize)).unwrap();
 
       let stream_descriptor = unsafe {
         StreamDescriptor {
-          index: stream_index as u32,
+          index: stream_index,
           start_time,
-          duration: duration.map(|value| value as f32),
-          stream_metadata: Default::default(),
-          nb_frames: (*stream).nb_frames as u64,
-          avg_frame_rate: (*stream).avg_frame_rate.num as f32 / (*stream).avg_frame_rate.den as f32,
-          r_frame_rate: (*stream).r_frame_rate.num as f32 / (*stream).r_frame_rate.den as f32,
-          kind: format!("{:?}", (*(*stream).codec).codec_type),
-          width: (*(*stream).codec).width as u32,
-          height: (*(*stream).codec).height as u32,
-          channels: (*(*stream).codec).channels as u32,
-          sample_rate: (*(*stream).codec).sample_rate as u32,
+          duration: stream.get_duration(),
+          stream_metadata: stream.get_stream_metadata(),
+          nb_frames: stream.get_nb_frames().unwrap_or_default() as u64,
+          avg_frame_rate: (*stream.stream).avg_frame_rate.num as f32
+            / (*stream.stream).avg_frame_rate.den as f32,
+          r_frame_rate: (*stream.stream).r_frame_rate.num as f32
+            / (*stream.stream).r_frame_rate.den as f32,
+          kind: format!("{:?}", context.get_stream_type(stream_index as isize)),
+          width: stream.get_width() as u32,
+          height: stream.get_height() as u32,
+          channels: stream.get_channels() as u32,
+          sample_rate: stream.get_sample_rate() as u32,
         }
       };
       streams.push(stream_descriptor);
     }
 
     FormatContext {
       format_name,
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/frame.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/frame.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/mod.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/mod.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/media/stream_descriptor.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/media/stream_descriptor.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/parameters.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/parameters.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use crate::helper::handle_automatic_job_parameters;
+
 use jsonschema::JSONSchema;
 use mcai_worker_sdk::prelude::*;
 use pyo3::{
   prelude::*,
   types::{PyDict, PyList, PyType},
 };
 use schemars::{schema::RootSchema, JsonSchema};
@@ -17,14 +19,17 @@
 ///   >>>   number: int
 ///   >>>   array_of_strings: list[str]
 ///   >>>   array_of_integers: list[int]
 ///
 /// Note:
 ///   Some parameters can be declared as optional. Use `Optional <https://docs.python.org/3/library/typing.html#typing.Optional>`_ from typing to do so.
 ///
+/// Note:
+///   The parameter class will also have an attribute :attr:`requirements` autogerenated by StepFlow and directly handled by the SDK.
+///
 /// Warning:
 ///   You should take special care when defining this class to type properly its attributes.
 ///   Under the hood, attributes types will be used by the SDK to cast parameters arriving from the backend into their proper Python type.
 #[pyclass(subclass)]
 #[derive(Clone, Debug, Default, Deserialize, JsonSchema, Serialize)]
 pub struct WorkerParameters {
   #[serde(flatten)]
@@ -45,17 +50,19 @@
       let json_module = py.import("json")?;
       let schema_module = py.import("strong_typing.schema")?;
 
       let parameters_schema = schema_module
         .getattr("classdef_to_schema")?
         .call1((parameters,))?;
 
+      let parameters_schema_extended = handle_automatic_job_parameters(py, parameters_schema)?;
+
       json_module
         .getattr("dumps")?
-        .call1((parameters_schema,))?
+        .call1((parameters_schema_extended,))?
         .extract::<String>()
     })?;
 
     Ok(
       serde_json::from_str(&parameters_schema_as_string).unwrap_or_else(|error| {
         panic!(
           "Could not deserialize parameters schema: {:?} (schema={})",
@@ -234,14 +241,23 @@
             }
           },
           "number": {
             "type": "integer"
           },
           "string_param": {
             "type": "string"
+          },
+          "requirements": {
+            "type": "object"
+          },
+          "source_paths": {
+            "type": "array",
+            "items": {
+              "type": "string"
+            }
           }
         },
         "additionalProperties": false
       })
     )
   })
 }
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/src/worker.rs` & `mcai_worker_sdk_media-2.0.0rc9/src/worker.rs`

 * *Files identical despite different names*

### Comparing `mcai_worker_sdk_media-2.0.0rc8/Cargo.lock` & `mcai_worker_sdk_media-2.0.0rc9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -14,43 +14,22 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "aes-ctr"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7729c3cde54d67063be556aeac75a81330d802f0259500ca40cb52967f975763"
-dependencies = [
- "aes-soft",
- "aesni",
- "cipher",
- "ctr",
-]
-
-[[package]]
-name = "aes-soft"
-version = "0.6.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be14c7498ea50828a38d0e24a765ed2effe92a705885b57d029cd67d45744072"
-dependencies = [
- "cipher",
- "opaque-debug",
-]
-
-[[package]]
-name = "aesni"
-version = "0.10.0"
+name = "aes"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea2e11f5e94c2f7d386164cc2aa1f97823fed6f259e486940a71c174dd01b0ce"
+checksum = "433cfd6710c9986c576a25ca913c39d66a6474107b406f34f91d4a8923395241"
 dependencies = [
+ "cfg-if",
  "cipher",
- "opaque-debug",
+ "cpufeatures",
 ]
 
 [[package]]
 name = "ahash"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
@@ -77,15 +56,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3b51c409a2b30e48826a593d56a26a43f37bf3df682821e55cd108e24de9ce7"
 dependencies = [
  "amq-protocol-tcp",
  "amq-protocol-types",
  "amq-protocol-uri",
  "cookie-factory",
- "nom 7.1.3",
+ "nom",
 ]
 
 [[package]]
 name = "amq-protocol-tcp"
 version = "6.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9797cd3a8f1491e4828818341aea5e1378029ec89dc2422cd85d62715f913080"
@@ -98,15 +77,15 @@
 [[package]]
 name = "amq-protocol-types"
 version = "6.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "028cb766932137535fe8a320245e385bac379506d7e9e3d0375be069bb6fb0de"
 dependencies = [
  "cookie-factory",
- "nom 7.1.3",
+ "nom",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "amq-protocol-uri"
 version = "6.1.0"
@@ -123,35 +102,38 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "ansi_term"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "anyhow"
 version = "1.0.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
+name = "array-init"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
+
+[[package]]
+name = "arraydeque"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d902e3d592a523def97af8f317b08ce16b7ab854c1985a0c671e6f15cebc236"
+
+[[package]]
 name = "async-amqp"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a5374e878d2cc33f231c40219990a9940381a31e21bb96fa5c5fe25ece60b6e"
 dependencies = [
  "async-lapin",
  "async-std",
@@ -209,15 +191,15 @@
  "concurrent-queue",
  "futures-lite",
  "libc",
  "log",
  "parking",
  "polling",
  "slab",
- "socket2",
+ "socket2 0.4.7",
  "waker-fn",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "async-lapin"
 version = "1.3.0"
@@ -338,33 +320,29 @@
 name = "base64"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
 
 [[package]]
 name = "bindgen"
-version = "0.58.1"
+version = "0.59.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f8523b410d7187a43085e7e064416ea32ded16bd0a4e6fc025e21616d01258f"
+checksum = "2bd2a9a458e8f4304c52c43ebb0cfbd520289f8379a52e329a38afda99bf8eb8"
 dependencies = [
  "bitflags",
  "cexpr",
  "clang-sys",
- "clap 2.34.0",
- "env_logger",
  "lazy_static",
  "lazycell",
- "log",
  "peeking_take_while",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "which",
 ]
 
 [[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
@@ -382,17 +360,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.9.0"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "blocking"
 version = "1.3.0"
@@ -446,19 +424,19 @@
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cexpr"
-version = "0.4.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4aedb84272dbe89af497cf81375129abda4fc0a9e7c5d317498c15cc30c0d27"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
- "nom 5.1.2",
+ "nom",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -477,19 +455,20 @@
  "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "cipher"
-version = "0.2.5"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12f8e7987cbd042a63249497f41aed09f8e65add917ea6566effbc56578d6801"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
- "generic-array",
+ "crypto-common",
+ "inout",
 ]
 
 [[package]]
 name = "clang-sys"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa2e27ae6ab525c3d369ded447057bca5438d86dc3a68f6faafb8269ba82ebf3"
@@ -497,29 +476,14 @@
  "glob",
  "libc",
  "libloading 0.7.4",
 ]
 
 [[package]]
 name = "clap"
-version = "2.34.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
-dependencies = [
- "ansi_term",
- "atty",
- "bitflags",
- "strsim 0.8.0",
- "textwrap",
- "unicode-width",
- "vec_map",
-]
-
-[[package]]
-name = "clap"
 version = "4.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f13b9c79b5d1dd500d20ef541215a6423c75829ef43117e1b4d17fd8af0b5d76"
 dependencies = [
  "bitflags",
  "clap_derive",
  "clap_lex",
@@ -567,14 +531,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c278839b831783b70278b14df4d45e1beb1aad306c07bb796637de9a0e323e8e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "convert_case"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
+
+[[package]]
 name = "cookie-factory"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "396de984970346b0d9e93d1415082923c679e5ae5c3ee3dcbd104f5610af126b"
 
 [[package]]
 name = "core-foundation"
@@ -651,38 +621,38 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "crypto-mac"
-version = "0.10.1"
+name = "crypto-common"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff07008ec701e8028e2ceb8f83f0e4274ee62bd2dbdc4fefff2e9a91824081a"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
- "subtle",
+ "typenum",
 ]
 
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "ctr"
-version = "0.6.0"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb4a30d54f7443bf3d6191dcd486aca19e67cb3c49fa7a06a319966346707e7f"
+checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
 name = "ctrlc"
 version = "3.2.5"
@@ -780,26 +750,41 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
+name = "derive_more"
+version = "0.99.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
+dependencies = [
+ "convert_case",
+ "proc-macro2",
+ "quote",
+ "rustc_version",
+ "syn",
+]
+
+[[package]]
 name = "destructure_traitobject"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c877555693c14d2f84191cfd3ad8582790fc52b5e2274b40b59cf5f5cea25c7"
 
 [[package]]
 name = "digest"
-version = "0.9.0"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
+checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
 dependencies = [
- "generic-array",
+ "block-buffer",
+ "crypto-common",
+ "subtle",
 ]
 
 [[package]]
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
@@ -912,25 +897,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a7a407cfaa3385c4ae6b23e84623d48c2798d06e3e6a1878f7f59f17b3f86499"
 dependencies = [
  "instant",
 ]
 
 [[package]]
-name = "ffmpeg-sys"
-version = "4.3.3"
+name = "ffmpeg-sys-next"
+version = "5.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc564a8a458c444d47428ea45c98cc30d7cec620c77e5f0511a6b3e6c346288"
+checksum = "d780b36e092254367e2f1f21191992735c8e23f31a5a5a8678db3a79f775021f"
 dependencies = [
  "bindgen",
  "cc",
  "libc",
  "num_cpus",
  "pkg-config",
- "regex",
  "vcpkg",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1141,15 +1125,15 @@
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
  "indexmap",
  "slab",
  "tokio",
- "tokio-util 0.7.7",
+ "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1191,20 +1175,25 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
+
+[[package]]
 name = "hmac"
-version = "0.10.1"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1441c6b1e930e2817404b5046f1f989899143a12bf92de603b69f4e0aee1e15"
+checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
- "crypto-mac",
  "digest",
 ]
 
 [[package]]
 name = "http"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1257,15 +1246,15 @@
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "socket2 0.4.7",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -1334,14 +1323,23 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "inout"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
@@ -1386,15 +1384,15 @@
 
 [[package]]
 name = "iso8601"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "296af15e112ec6dc38c9fd3ae027b5337a75466e8eed757bd7d5cf742ea85eb6"
 dependencies = [
- "nom 7.1.3",
+ "nom",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
@@ -1414,15 +1412,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6ca9e2b45609132ae2214d50482c03aeee78826cd6fd53a8940915b81acedf16"
 dependencies = [
  "ahash",
  "anyhow",
  "base64 0.13.1",
  "bytecount",
- "clap 4.1.4",
+ "clap",
  "fancy-regex",
  "fraction",
  "iso8601",
  "itoa",
  "lazy_static",
  "memchr",
  "num-cmp",
@@ -1434,14 +1432,23 @@
  "serde_json",
  "time 0.3.17",
  "url",
  "uuid 1.3.0",
 ]
 
 [[package]]
+name = "keyed_priority_queue"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2d63b6407b66fc81fc539dccf3ddecb669f393c5101b6a2be3976c95099a06e8"
+dependencies = [
+ "indexmap",
+]
+
+[[package]]
 name = "kv-log-macro"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0de8b303297635ad57c9f5059fd9cee7a47f8e8daa09df0fcd07dd39fb22977f"
 dependencies = [
  "log",
 ]
@@ -1606,17 +1613,17 @@
  "cargo_toml",
  "mcai-license",
  "serde_json",
 ]
 
 [[package]]
 name = "mcai_worker_sdk"
-version = "2.0.0-rc4"
+version = "2.0.0-rc5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0900a1847befe2c63eb578504aeccd5f92500f44d5dfebc5e3f610d0b787f30"
+checksum = "a1923bf30684fc85335ca65c2b56f7aa9cafd01614541f240869c8dd570d199b"
 dependencies = [
  "amq-protocol",
  "amq-protocol-types",
  "amq-protocol-uri",
  "anyhow",
  "async-amqp",
  "async-std",
@@ -1638,15 +1645,15 @@
  "mcai-license",
  "mcai_build",
  "nvml-wrapper",
  "regex",
  "reqwest",
  "ringbuf",
  "schemars",
- "semver",
+ "semver 0.11.0",
  "serde",
  "serde_derive",
  "serde_json",
  "srt-protocol",
  "srt-tokio",
  "stainless_ffmpeg",
  "sysinfo",
@@ -1764,24 +1771,14 @@
  "cfg-if",
  "libc",
  "static_assertions",
 ]
 
 [[package]]
 name = "nom"
-version = "5.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb4262d26ed83a1c0a33a38fe2bb15797329c85770da05e6b828ddb782627af"
-dependencies = [
- "memchr",
- "version_check",
-]
-
-[[package]]
-name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
@@ -1931,20 +1928,14 @@
 [[package]]
 name = "once_cell"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
 
 [[package]]
-name = "opaque-debug"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
-
-[[package]]
 name = "openssl"
 version = "0.10.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b102428fd03bc5edf97f62620f7298614c45cedf287c271e7ed450bbaf83f2e1"
 dependencies = [
  "bitflags",
  "cfg-if",
@@ -2027,19 +2018,19 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "pbkdf2"
-version = "0.6.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3b8c0d71734018084da0c0354193a5edfb81b20d2d57a92c5b154aefc554a4a"
+checksum = "f0ca0b5a68607598bf3bad68f32227a8164f6254833f84eafaac409cd6746c31"
 dependencies = [
- "crypto-mac",
+ "digest",
 ]
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
@@ -2151,25 +2142,26 @@
 checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_mcai_worker_sdk"
-version = "2.0.0-rc8"
+version = "2.0.0-rc9"
 dependencies = [
  "async-std",
  "jsonschema",
  "mcai_worker_sdk",
  "pyo3",
  "pyproject-toml",
  "schemars",
  "serde",
  "serde_derive",
  "serde_json",
+ "stainless_ffmpeg",
  "toml 0.5.11",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2400,14 +2392,23 @@
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
+name = "rustc_version"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver 1.0.17",
+]
+
+[[package]]
 name = "rustix"
 version = "0.36.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43abb88211988493c1abb44a70efa56ff0ce98f233b7b276146f1f3f7ba9644"
 dependencies = [
  "bitflags",
  "errno",
@@ -2498,14 +2499,20 @@
 checksum = "f301af10236f6df4160f7c3f04eec6dbc70ace82d23326abad5edee88801c6b6"
 dependencies = [
  "semver-parser",
  "serde",
 ]
 
 [[package]]
+name = "semver"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+
+[[package]]
 name = "semver-parser"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0bef5b7f9e0df16536d3961cfb6e84331c065b4066afb39768d0e319411f7"
 dependencies = [
  "pest",
 ]
@@ -2602,23 +2609,21 @@
  "ryu",
  "serde",
  "yaml-rust",
 ]
 
 [[package]]
 name = "sha-1"
-version = "0.9.8"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99cd6713db3cf16b6c84e06321e049a9b9f699826e16096d23bbcc44d15d51a6"
+checksum = "f5058ada175748e33390e40e872bd0fe59a19f265d0158daa551c5a88a76009c"
 dependencies = [
- "block-buffer",
  "cfg-if",
  "cpufeatures",
  "digest",
- "opaque-debug",
 ]
 
 [[package]]
 name = "shlex"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
@@ -2664,54 +2669,74 @@
 checksum = "02e2d2db9033d13a1567121ddd7a095ee144db4e1ca1b1bda3419bc0da294ebd"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "socket2"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc8d618c6641ae355025c449427f9e96b98abf99a772be3cef6708d15c77147a"
+dependencies = [
+ "libc",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
 name = "srt-protocol"
-version = "0.2.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a653e1dc84222215491d6c7563d80eab509d2ee82deaf50cea3c5e0e0e88fe9b"
+checksum = "b391aef8865a0ff098c48c28ad18b195f22cebd86b40ab68c4ee830f8ddcaff8"
 dependencies = [
- "aes-ctr",
- "aes-soft",
+ "aes",
+ "array-init",
+ "arraydeque",
  "bitflags",
  "bytes",
  "cipher",
+ "ctr",
+ "derive_more",
+ "hex",
  "hmac",
+ "keyed_priority_queue",
  "log",
  "pbkdf2",
  "rand",
+ "regex",
  "sha-1",
  "streaming-stats",
+ "take-until",
+ "thiserror",
+ "url",
 ]
 
 [[package]]
 name = "srt-tokio"
-version = "0.2.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24d5dc26e166f11a2bf8d2f70ca9a722bd6b6aea5900e8528f5558343acea3dd"
+checksum = "e105762c4aa4e3b7c4a0bc68d20820df0870688adb0addf9316de372f089afde"
 dependencies = [
  "bytes",
  "futures",
  "log",
+ "rand",
+ "socket2 0.5.1",
  "srt-protocol",
  "tokio",
  "tokio-stream",
- "tokio-util 0.6.10",
 ]
 
 [[package]]
 name = "stainless_ffmpeg"
-version = "0.2.8"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef11a55ecec742bfb5ae37790d4ad276e2e7c196393aec61f6f74084acfc50db"
+checksum = "ee193530c7484bc4385729152fc7eb9455ac0bebd2571996f12d145c34d243c2"
 dependencies = [
- "ffmpeg-sys",
+ "ffmpeg-sys-next",
  "libc",
  "log",
  "rand",
  "serde",
  "serde_derive",
  "serde_json",
 ]
@@ -2729,20 +2754,14 @@
 checksum = "b0d670ce4e348a2081843569e0f79b21c99c91bb9028b3b3ecb0f050306de547"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "strsim"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
-
-[[package]]
-name = "strsim"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6446ced80d6c486436db5c078dde11a9f73d42b57fb273121e160b84f63d894c"
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
@@ -2799,14 +2818,20 @@
  "ntapi",
  "once_cell",
  "rayon",
  "winapi",
 ]
 
 [[package]]
+name = "take-until"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4e17d8598067a8c134af59cd33c1c263470e089924a11ab61cf61690919fe3b"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "tcp-stream"
@@ -2840,23 +2865,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
-dependencies = [
- "unicode-width",
-]
-
-[[package]]
 name = "thiserror"
 version = "1.0.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
 dependencies = [
  "thiserror-impl",
 ]
@@ -2944,15 +2960,15 @@
  "autocfg",
  "bytes",
  "libc",
  "memchr",
  "mio 0.8.5",
  "num_cpus",
  "pin-project-lite",
- "socket2",
+ "socket2 0.4.7",
  "tokio-macros",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "1.8.2"
@@ -2979,28 +2995,15 @@
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d660770404473ccd7bc9f8b28494a811bc18542b915c0855c51e8f419d5223ce"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
-]
-
-[[package]]
-name = "tokio-util"
-version = "0.6.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36943ee01a6d67977dd3f84a5a1d2efeb4ada3a1ae771cadfaa535d9d9fc6507"
-dependencies = [
- "bytes",
- "futures-core",
- "futures-sink",
- "log",
- "pin-project-lite",
- "tokio",
+ "tokio-util",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.7.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
@@ -3207,20 +3210,14 @@
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
-name = "vec_map"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "waker-fn"
@@ -3332,23 +3329,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d743fdedc5c64377b5fc2bc036b01c7fd642205a0d96356034ae3404d49eb7fb"
 dependencies = [
  "cc",
 ]
 
 [[package]]
-name = "which"
-version = "3.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d011071ae14a2f6671d0b74080ae0cd8ebf3a6f8c9589a2cd45f23126fe29724"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
```

### Comparing `mcai_worker_sdk_media-2.0.0rc8/PKG-INFO` & `mcai_worker_sdk_media-2.0.0rc9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcai_worker_sdk_media
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Requires-Dist: json-strong-typing
 License-File: LICENSE
 Summary: MCAI SDK to develop Python worker
 Keywords: AMQP,micro-service,python
 Home-Page: https://gitlab.com/media-cloud-ai/sdks/py_mcai_worker_sdk
 Author: Valentin NOEL <valentin.noel@media-io.com>, Marc-Antoine Arnaud <maarnaud@media-io.com>, Thibaud Le Graverend <thibaud.legraverend@luminvent.com>
 Author-email: Valentin NOEL <valentin.noel@media-io.com>, Marc-Antoine Arnaud <maarnaud@media-io.com>, Thibaud Le Graverend <thibaud.legraverend@luminvent.com>
@@ -54,20 +54,20 @@
 ### Supported version
 
 We intempt to support as many distribution and architecture as we can, however if `pip` doesn't find any compatible version for your installation it will download the source and try to compile them directly.
 
 This operation supposes that you have at least __Rust 1.62__.
 
 We currently support the following version of Python implementations:
-- [x] CPython 3.8
-- [x] CPython 3.9
-- [x] CPython 3.10
-- [x] CPython 3.11
-- [x] Pypy 3.8
-- [x] Pypy 3.9
+- [x] CPython 3.8 : manylinux
+- [x] CPython 3.9 : manylinux, macosx x86_64
+- [x] CPython 3.10 : manylinux, macosx x86_64, macosx arm64
+- [x] CPython 3.11 : manylinux, macosx arm54
+- [x] Pypy 3.8 : manylinux
+- [x] Pypy 3.9 : manylinux
 
 And the following core architectures:
 - [x] x86_64
 
 
 ## Test
```

