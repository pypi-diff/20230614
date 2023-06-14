# Comparing `tmp/mitmproxy_rs-0.2.0b8.tar.gz` & `tmp/mitmproxy_rs-0.2.0b9.tar.gz`

## Comparing `mitmproxy_rs-0.2.0b8.tar` & `mitmproxy_rs-0.2.0b9.tar`

### file list

```diff
@@ -1,56 +1,63 @@
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/Cargo.toml
--rw-r--r--   0     1001      123       84 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.cargo/config.toml
--rw-r--r--   0     1001      123       28 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/FUNDING.yml
--rw-r--r--   0     1001      123      205 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/dependabot.yml
--rw-r--r--   0     1001      123        5 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/python-version.txt
--rw-r--r--   0     1001      123     1048 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/workflows/autofix.yml
--rw-r--r--   0     1001      123     3982 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     1831 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/workflows/docs.yml
--rw-r--r--   0     1001      123       57 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.gitignore
--rw-r--r--   0     1001      123     4472 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/CHANGELOG.md
--rwxr-xr-x   0     1001      123     2085 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/LICENSE
--rw-r--r--   0     1001      123     3271 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/README.md
--rw-r--r--   0     1001      123   243520 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/architecture.png
--rw-r--r--   0     1001      123       22 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/.gitignore
--rw-r--r--   0     1001      123      220 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/local.conf
--rw-r--r--   0     1001      123      214 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/nonlocal.conf
--rw-r--r--   0     1001      123    10121 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/plot.py
--rwxr-xr-x   0     1001      123      426 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/process.rs
--rw-r--r--   0     1001      123     2375 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/py_echo_client.py
--rw-r--r--   0     1001      123     1246 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/py_echo_server.py
--rw-r--r--   0     1001      123     2346 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/wg_echo_client.py
--rw-r--r--   0     1001      123     2036 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/wg_echo_server.py
--rwxr-xr-x   0     1001      123      264 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/coverage.sh
--rwxr-xr-x   0     1001      123     3996 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/intercept_conf.rs
--rwxr-xr-x   0     1001      123      183 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/lib.rs
--rwxr-xr-x   0     1001      123     3830 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/messages.rs
--rwxr-xr-x   0     1001      123      126 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/mod.rs
--rwxr-xr-x   0     1001      123    21545 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/task.rs
--rwxr-xr-x   0     1001      123    22561 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/tests.rs
--rwxr-xr-x   0     1001      123     2678 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/virtual_device.rs
--rwxr-xr-x   0     1001      123      662 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/packet_sources/mod.rs
--rwxr-xr-x   0     1001      123     7946 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/packet_sources/windows.rs
--rwxr-xr-x   0     1001      123    13781 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs
--rwxr-xr-x   0     1001      123     3721 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/shutdown.rs
--rwxr-xr-x   0     1001      123        1 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/util.rs
--rwxr-xr-x   0     1001      123     8115 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/windows.rs
--rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b8/Cargo.toml
--rw-r--r--   0     1001      123       97 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/.gitignore
--rw-r--r--   0     1001      123     2850 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/README.md
--rwxr-xr-x   0     1001      123     1919 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/build.rs
--rw-r--r--   0     1001      123      132 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/mitmproxy_rs/__init__.py
--rw-r--r--   0     1001      123     1907 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/mitmproxy_rs/__init__.pyi
--rw-r--r--   0     1001      123      121 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/mitmproxy_rs/_pyinstaller/__init__.py
--rw-r--r--   0     1001      123       99 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
--rw-r--r--   0     1001      123        0 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/mitmproxy_rs/py.typed
--rw-r--r--   0     1001      123      687 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/pyproject.toml
--rwxr-xr-x   0     1001      123     3492 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/src/datagram_transport.rs
--rwxr-xr-x   0     1001      123     1522 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/src/lib.rs
--rwxr-xr-x   0     1001      123    10313 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/src/server.rs
--rwxr-xr-x   0     1001      123     7234 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/src/task.rs
--rwxr-xr-x   0     1001      123     5398 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/src/tcp_stream.rs
--rwxr-xr-x   0     1001      123     2036 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/src/util.rs
--rwxr-xr-x   0     1001      123       25 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/stubtest-allowlist.txt
--rw-r--r--   0     1001      123    60689 2023-02-13 17:25:34.000000 mitmproxy_rs-0.2.0b8/Cargo.lock
--rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/Cargo.toml
+-rw-r--r--   0     1001      123       84 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.cargo/config.toml
+-rw-r--r--   0     1001      123       28 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/FUNDING.yml
+-rw-r--r--   0     1001      123      511 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/dependabot.yml
+-rw-r--r--   0     1001      123        5 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/python-version.txt
+-rw-r--r--   0     1001      123     1158 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/autofix.yml
+-rw-r--r--   0     1001      123     4222 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     1869 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/docs.yml
+-rw-r--r--   0     1001      123       57 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.gitignore
+-rw-r--r--   0     1001      123     4472 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CHANGELOG.md
+-rwxr-xr-x   0     1001      123     2085 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/LICENSE
+-rw-r--r--   0     1001      123     3271 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/README.md
+-rw-r--r--   0     1001      123   243520 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/architecture.png
+-rw-r--r--   0     1001      123       22 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/.gitignore
+-rw-r--r--   0     1001      123      220 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/local.conf
+-rw-r--r--   0     1001      123      214 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/nonlocal.conf
+-rw-r--r--   0     1001      123    67352 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/openvpnserv.exe
+-rw-r--r--   0     1001      123    10121 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/plot.py
+-rwxr-xr-x   0     1001      123     1730 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/process.rs
+-rw-r--r--   0     1001      123     2375 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_client.py
+-rw-r--r--   0     1001      123     1246 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_server.py
+-rw-r--r--   0     1001      123     2346 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_client.py
+-rw-r--r--   0     1001      123     2036 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_server.py
+-rwxr-xr-x   0     1001      123      264 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/coverage.sh
+-rwxr-xr-x   0     1001      123     4188 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/intercept_conf.rs
+-rwxr-xr-x   0     1001      123      202 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/lib.rs
+-rwxr-xr-x   0     1001      123     3863 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/messages.rs
+-rwxr-xr-x   0     1001      123      126 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/mod.rs
+-rwxr-xr-x   0     1001      123    26177 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/task.rs
+-rwxr-xr-x   0     1001      123    26991 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/tests.rs
+-rwxr-xr-x   0     1001      123     2705 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/virtual_device.rs
+-rwxr-xr-x   0     1001      123      662 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/mod.rs
+-rwxr-xr-x   0     1001      123     7813 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/windows.rs
+-rwxr-xr-x   0     1001      123    13781 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs
+-rw-r--r--   0     1001      123      243 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/processes.rs
+-rwxr-xr-x   0     1001      123     3721 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/shutdown.rs
+-rwxr-xr-x   0     1001      123        1 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/util.rs
+-rw-r--r--   0     1001      123     5276 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/icons.rs
+-rw-r--r--   0     1001      123       51 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/mod.rs
+-rw-r--r--   0     1001      123     6828 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/network.rs
+-rw-r--r--   0     1001      123    10928 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/processes.rs
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b9/Cargo.toml
+-rw-r--r--   0     1001      123       97 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/.gitignore
+-rw-r--r--   0     1001      123     2850 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/README.md
+-rwxr-xr-x   0     1001      123     1919 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/build.rs
+-rw-r--r--   0     1001      123      132 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/__init__.py
+-rw-r--r--   0     1001      123     2296 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/__init__.pyi
+-rw-r--r--   0     1001      123      121 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/_pyinstaller/__init__.py
+-rw-r--r--   0     1001      123       99 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
+-rw-r--r--   0     1001      123        0 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/py.typed
+-rw-r--r--   0     1001      123      745 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/pyproject.toml
+-rwxr-xr-x   0     1001      123     3575 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/datagram_transport.rs
+-rwxr-xr-x   0     1001      123     1737 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/lib.rs
+-rw-r--r--   0     1001      123     2054 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/process_info.rs
+-rwxr-xr-x   0     1001      123    10062 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/server.rs
+-rwxr-xr-x   0     1001      123     7234 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/task.rs
+-rwxr-xr-x   0     1001      123     5452 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/tcp_stream.rs
+-rwxr-xr-x   0     1001      123     2036 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/util.rs
+-rwxr-xr-x   0     1001      123       70 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/stubtest-allowlist.txt
+-rw-r--r--   0     1001      123      125 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/test.py
+-rw-r--r--   0     1001      123    69220 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/Cargo.lock
+-rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b9/PKG-INFO
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/Cargo.toml` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,65 +7,71 @@
 ]
 
 [workspace.package]
 authors = [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version = "0.2.0-beta.8"
+version = "0.2.0-beta.9"
 publish = false
 repository = "https://github.com/mitmproxy/mitmproxy-rs"
 edition = "2021"
 rust-version = "1.65.0"
 
 [workspace.dependencies]
-bincode = "2.0.0-rc.2"
+bincode = "2.0.0-rc.3"
 
 [package]
 name = "mitmproxy"
 license = "MIT"
 authors= [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version= "0.2.0-beta.8"
+version= "0.2.0-beta.9"
 repository= "https://github.com/mitmproxy/mitmproxy-rs"
 edition= "2021"
 rust-version= "1.65.0"
 publish= false
 
 [dependencies]
-anyhow = { version = "1.0.68", features = ["backtrace"] }
-log = "0.4.17"
+anyhow = { version = "1.0.71", features = ["backtrace"] }
+log = "0.4.18"
 once_cell = "1"
 pretty-hex = "0.3.0"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
-smoltcp = "0.8"
-tokio = { version = "1.23", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util"] }
+smoltcp = "0.9"
+tokio = { version = "1.28.2", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util"] }
 boringtun = { version = "0.5", default-features = false }
-x25519-dalek = "2.0.0-pre.1"
-async-trait = "0.1.60"
-console-subscriber = { version = "0.1.8", optional = true }
+x25519-dalek = "=2.0.0-pre.1"
+async-trait = "0.1.68"
+console-subscriber = { version = "0.1.9", optional = true }
+image = "0.24.6"
 
 [patch.crates-io]
 # tokio = { path = "../tokio/tokio" }
-tokio = { git = 'https://github.com/mhils/tokio', branch = 'readmode-fix' }
+smoltcp = { git = 'https://github.com/mhils/smoltcp', rev = 'f65351adfa92db5193f368368cb668bac721fe43' }
 
 [target.'cfg(windows)'.dependencies]
-bincode.workspace = true
+bincode= "2.0.0-rc.3"
 
 [target.'cfg(windows)'.dependencies.windows]
-version = "0.44.0"
+version = "0.48.0"
 features = [
     "Win32_Foundation",
+    "Win32_Graphics_Dwm",
+    "Win32_Graphics_Gdi",
     "Win32_Networking_WinSock",
     "Win32_NetworkManagement_IpHelper",
+    "Win32_Storage_FileSystem",
+    "Win32_System_LibraryLoader",
+    "Win32_System_ProcessStatus",
+    "Win32_System_Threading",
     "Win32_UI_Shell",
     "Win32_UI_WindowsAndMessaging",
-    "Win32_System_Threading",
 ]
 
 [[bench]]
 name = "process"
 harness = false
 
 [profile.release]
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/workflows/autofix.yml` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/autofix.yml`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,17 @@
             ~/.cargo/registry/cache/
             ~/.cargo/git/db/
             target/
           key: autofix-${{ hashFiles('**/Cargo.lock') }}
 
       - run: rustup toolchain install ${{ env.rust_clippy }} --profile minimal --component rustfmt --component clippy
       - run: rustup default ${{ env.rust_clippy }}
+      - uses: actions/setup-python@v4
+        with:
+          python-version-file: .github/python-version.txt
 
       - if: runner.os == 'Windows'
         # workaround for https://github.com/rust-lang/cargo/issues/9096
         run: cargo build --package windows-redirector
 
       - run: cargo clippy --fix --workspace --allow-dirty
       - run: cargo fmt --all
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/workflows/ci.yml` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,17 @@
             ~/.cargo/registry/index/
             ~/.cargo/registry/cache/
             ~/.cargo/git/db/
             target/
           key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
       - name: Set up Rust toolchain
         run: rustup toolchain install ${{ matrix.rust }} --profile minimal
+      - uses: actions/setup-python@v4
+        with:
+          python-version-file: .github/python-version.txt
 
       - if: runner.os == 'Windows'
         # workaround for https://github.com/rust-lang/cargo/issues/9096
         run: cargo build --package windows-redirector
 
       - name: Run "cargo check"
         # the action-rs/cargo action adds inline annotations for "cargo check" output
@@ -73,15 +76,15 @@
             args: --compatibility manylinux2014 --zig --sdist
           - os: ubuntu-latest
             target: aarch64-unknown-linux-gnu
             args: --compatibility manylinux2014 --zig --target aarch64-unknown-linux-gnu
           - os: macos-latest
           - os: macos-latest
             target: aarch64-apple-darwin
-            args: --universal2
+            args: --target universal2-apple-darwin
     runs-on: ${{ matrix.os }}
     name: build-wheel (${{ matrix.os }}, ${{ matrix.target || 'x64' }})
     steps:
       - uses: actions/checkout@v3
       - uses: actions/cache@v3
         with:
           path: |
@@ -92,17 +95,20 @@
             target/
           key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
       - run: rustup toolchain install stable --profile minimal
       - run: rustup default stable
       - if: matrix.target
         run: rustup target add ${{ matrix.target }}
       - run: rustup show
+      - uses: actions/setup-python@v4
+        with:
+          python-version-file: .github/python-version.txt
 
       - name: Install maturin[zig] from PyPI
-        uses: install-pinned/maturin-with-zig@39e7f65d43a471e5acd36deeafbd31de3fe167fb
+        uses: install-pinned/maturin-with-zig@59341946682d2f69df7150f6941f53e026e344fd
 
       - if: runner.os == 'Windows'
         # workaround for https://github.com/rust-lang/cargo/issues/9096
         run: cargo build --release --package windows-redirector
 
       - run: maturin build --release ${{ matrix.args }}
         working-directory: ./ffi
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/.github/workflows/docs.yml` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -27,25 +27,25 @@
             ~/.cargo/registry/index/
             ~/.cargo/registry/cache/
             ~/.cargo/git/db/
             target/
           key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
 
       - name: Install maturin[zig] from PyPI
-        uses: install-pinned/maturin-with-zig@39e7f65d43a471e5acd36deeafbd31de3fe167fb
+        uses: install-pinned/maturin-with-zig@59341946682d2f69df7150f6941f53e026e344fd
       - name: Install mypy from PyPI
-        uses: install-pinned/mypy@1ad1914d18ad1479bb0f9f5dd4ab1acda49b5d73
+        uses: install-pinned/mypy@c581c551e8cff8b305445a9c8375b5d08f330887
       - name: Install pdoc from PyPI
-        uses: install-pinned/pdoc@1d14345ed3c020d3d3c8d4428cbed20f2c3d6222
+        uses: install-pinned/pdoc@fac9037f8ea1d23a645d9ffe26f67877834518c8
 
       - run: maturin build
         working-directory: ./ffi
       - run: pip install --no-index --find-links target/wheels/ mitmproxy_rs
 
-      - run: stubtest --allowlist ffi/stubtest-allowlist.txt mitmproxy_rs
+      - run: stubtest --allowlist ffi/stubtest-allowlist.txt --mypy-config-file ffi/pyproject.toml mitmproxy_rs
 
       - run: pdoc -o docs/ mitmproxy_rs
 
       - uses: actions/upload-pages-artifact@v1
         with:
           path: docs/
 
@@ -59,8 +59,8 @@
       pages: write
       id-token: write
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - id: deployment
-        uses: actions/deploy-pages@v1
+        uses: actions/deploy-pages@v2
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/CHANGELOG.md` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/CONTRIBUTING.md` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/LICENSE` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/LICENSE`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/README.md` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/architecture.png` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/architecture.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/plot.py` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/plot.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/py_echo_client.py` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/py_echo_server.py` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/wg_echo_client.py` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/benches/wg_echo_server.py` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/intercept_conf.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/intercept_conf.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 use anyhow::bail;
 #[cfg(windows)]
 use bincode::{Decode, Encode};
 use std::collections::HashSet;
+use std::path::PathBuf;
 
 pub type PID = u32;
 
 #[derive(Debug, Clone)]
 pub struct ProcessInfo {
     pub pid: PID,
-    pub process_name: Option<String>,
+    pub process_name: Option<PathBuf>,
 }
 
 #[cfg_attr(windows, derive(Decode, Encode))]
 #[derive(PartialEq, Eq, Debug, Clone)]
 pub struct InterceptConf {
     pids: HashSet<PID>,
     process_names: Vec<String>,
@@ -64,15 +65,18 @@
         }
     }
 
     pub fn should_intercept(&self, process_info: &ProcessInfo) -> bool {
         self.invert ^ {
             if self.pids.contains(&process_info.pid) {
                 true
+            } else if self.process_names.is_empty() {
+                false // fast path to avoid conversion below.
             } else if let Some(name) = &process_info.process_name {
+                let name = name.to_string_lossy();
                 self.process_names.iter().any(|n| name.contains(n))
             } else {
                 false
             }
         }
     }
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/messages.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/messages.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 use std::net::{IpAddr, Ipv4Addr, Ipv6Addr, SocketAddr};
+use std::path::PathBuf;
 
 use anyhow::{anyhow, Result};
 use smoltcp::wire::{IpProtocol, Ipv4Packet, Ipv6Packet};
 use tokio::sync::oneshot;
 
 #[derive(Debug, Clone)]
 pub enum TunnelInfo {
     WireGuard {
         src_addr: SocketAddr,
         dst_addr: SocketAddr,
     },
     Windows {
         pid: u32,
-        process_name: Option<String>,
+        process_name: Option<PathBuf>,
     },
 }
 
 /// Events that are sent by WireGuard to the TCP stack.
 #[derive(Debug)]
 pub enum NetworkEvent {
     ReceivePacket {
@@ -60,15 +61,15 @@
     SendDatagram {
         data: Vec<u8>,
         src_addr: SocketAddr,
         dst_addr: SocketAddr,
     },
 }
 
-/// Generic IPv4/IPv6 packet type that wraps both IPv4 and IPv6 packet buffers
+/// Generic IPv4/IPv6 packet type that wraps smoltcp's IPv4 and IPv6 packet buffers
 #[derive(Debug)]
 pub enum IpPacket {
     V4(Ipv4Packet<Vec<u8>>),
     V6(Ipv6Packet<Vec<u8>>),
 }
 
 impl From<Ipv4Packet<Vec<u8>>> for IpPacket {
@@ -112,15 +113,15 @@
             IpPacket::V4(packet) => IpAddr::V4(Ipv4Addr::from(packet.dst_addr())),
             IpPacket::V6(packet) => IpAddr::V6(Ipv6Addr::from(packet.dst_addr())),
         }
     }
 
     pub fn transport_protocol(&self) -> IpProtocol {
         match self {
-            IpPacket::V4(packet) => packet.protocol(),
+            IpPacket::V4(packet) => packet.next_header(),
             IpPacket::V6(packet) => {
                 log::debug!("TODO: Implement IPv6 next_header logic.");
                 packet.next_header()
             }
         }
     }
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/task.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/task.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 use std::cmp;
-use std::collections::{BTreeMap, HashMap, HashSet, VecDeque};
+use std::collections::{HashMap, HashSet, VecDeque};
 use std::fmt;
 use std::net::SocketAddr;
 
 use anyhow::Result;
 use pretty_hex::pretty_hex;
+use smoltcp::iface::{Config, SocketSet};
+use smoltcp::socket::{tcp, Socket};
+
+use smoltcp::wire::{
+    Icmpv4Message, Icmpv4Packet, Icmpv4Repr, Icmpv6Message, Icmpv6Packet, Icmpv6Repr,
+};
 use smoltcp::{
-    iface::{Interface, InterfaceBuilder, Routes, SocketHandle},
+    iface::{Interface, SocketHandle},
     phy::ChecksumCapabilities,
-    socket::{Socket, TcpSocket, TcpSocketBuffer, TcpState},
     time::{Duration, Instant},
     wire::{
         IpAddress, IpCidr, IpProtocol, IpRepr, Ipv4Address, Ipv4Packet, Ipv4Repr, Ipv6Address,
         Ipv6Packet, Ipv6Repr, TcpPacket, UdpPacket, UdpRepr,
     },
-    Error,
 };
 use tokio::sync::{
     broadcast::Receiver as BroadcastReceiver,
     mpsc::{Permit, Receiver, Sender, UnboundedReceiver},
     oneshot,
 };
 
@@ -41,51 +45,74 @@
     // Gets notified once there's data to be read.
     recv_waiter: Option<(u32, oneshot::Sender<Vec<u8>>)>,
     // Gets notified once there is enough space in the write buffer.
     drain_waiter: Vec<oneshot::Sender<()>>,
     addr_tuple: (SocketAddr, SocketAddr),
 }
 
-struct NetworkIO {
-    iface: Interface<'static, VirtualDevice>,
+struct NetworkIO<'a> {
+    iface: Interface,
+    device: VirtualDevice,
+    sockets: SocketSet<'a>,
+
     net_tx: Sender<NetworkCommand>,
 
     socket_data: HashMap<ConnectionId, SocketData>,
     active_connections: HashSet<(SocketAddr, SocketAddr)>,
     next_connection_id: ConnectionId,
 }
 
-impl NetworkIO {
-    fn new(iface: Interface<'static, VirtualDevice>, net_tx: Sender<NetworkCommand>) -> Self {
+impl<'a> NetworkIO<'a> {
+    fn new(net_tx: Sender<NetworkCommand>) -> Self {
+        let mut device = VirtualDevice::new(net_tx.clone());
+
+        let config = Config::new();
+        let mut iface = Interface::new(config, &mut device);
+
+        iface.set_any_ip(true);
+
+        iface.update_ip_addrs(|ip_address| {
+            ip_address
+                .push(IpCidr::new(IpAddress::v4(0, 0, 0, 1), 0))
+                .unwrap();
+        });
+        // TODO: IPv6
+        iface
+            .routes_mut()
+            .add_default_ipv4_route(Ipv4Address::new(0, 0, 0, 1))
+            .unwrap();
+
         NetworkIO {
             iface,
+            device,
+            sockets: SocketSet::new(Vec::new()),
             net_tx,
             socket_data: HashMap::new(),
             active_connections: HashSet::new(),
             next_connection_id: 0,
         }
     }
 
     fn receive_packet(
         &mut self,
         packet: IpPacket,
         tunnel_info: TunnelInfo,
         permit: Permit<'_, TransportEvent>,
     ) -> Result<()> {
-
         if let IpPacket::V4(p) = &packet {
             if !p.verify_checksum() {
                 log::warn!("Received invalid IP packet (checksum error).");
                 return Ok(());
             }
         }
 
         match packet.transport_protocol() {
             IpProtocol::Tcp => self.receive_packet_tcp(packet, tunnel_info, permit),
             IpProtocol::Udp => self.receive_packet_udp(packet, tunnel_info, permit),
+            IpProtocol::Icmp => self.receive_packet_icmp(packet),
             _ => {
                 log::debug!(
                     "Received IP packet for unknown protocol: {}",
                     packet.transport_protocol()
                 );
                 Ok(())
             }
@@ -155,24 +182,24 @@
         let src_addr = SocketAddr::new(src_ip, tcp_packet.src_port());
         let dst_addr = SocketAddr::new(dst_ip, tcp_packet.dst_port());
 
         if tcp_packet.syn()
             && !tcp_packet.ack()
             && !self.active_connections.contains(&(src_addr, dst_addr))
         {
-            let mut socket = TcpSocket::new(
-                TcpSocketBuffer::new(vec![0u8; 64 * 1024]),
-                TcpSocketBuffer::new(vec![0u8; 64 * 1024]),
+            let mut socket = tcp::Socket::new(
+                tcp::SocketBuffer::new(vec![0u8; 64 * 1024]),
+                tcp::SocketBuffer::new(vec![0u8; 64 * 1024]),
             );
 
             socket.listen(dst_addr)?;
             socket.set_timeout(Some(Duration::from_secs(60)));
             socket.set_keep_alive(Some(Duration::from_secs(28)));
 
-            let handle = self.iface.add_socket(socket);
+            let handle = self.sockets.add(socket);
 
             let connection_id = self.next_connection_id;
             self.next_connection_id += 1;
 
             let data = SocketData {
                 handle,
                 send_buffer: VecDeque::new(),
@@ -189,15 +216,35 @@
                 src_addr,
                 dst_addr,
                 tunnel_info,
             };
             permit.send(event);
         }
 
-        self.iface.device_mut().receive_packet(packet);
+        self.device.receive_packet(packet);
+        Ok(())
+    }
+
+    fn receive_packet_icmp(&mut self, packet: IpPacket) -> Result<()> {
+        // Some apps check network connectivity by sending ICMP pings. ICMP traffic is currently
+        // swallowed by mitmproxy_rs, which makes them believe that there is no network connectivity.
+        // Generating fake ICMP replies as a simple workaround.
+
+        if let Ok(permit) = self.net_tx.try_reserve() {
+            // Generating and sending fake replies for ICMP echo requests. Ignoring all other ICMP types.
+            let response_packet = match packet {
+                IpPacket::V4(packet) => handle_icmpv4_echo_request(packet),
+                IpPacket::V6(packet) => handle_icmpv6_echo_request(packet),
+            };
+            if let Some(response_packet) = response_packet {
+                permit.send(NetworkCommand::SendPacket(response_packet));
+            }
+        } else {
+            log::debug!("Channel full, discarding ICMP packet.");
+        }
         Ok(())
     }
 
     fn read_data(&mut self, id: ConnectionId, n: u32, tx: oneshot::Sender<Vec<u8>>) {
         if let Some(data) = self.socket_data.get_mut(&id) {
             assert!(data.recv_waiter.is_none());
             data.recv_waiter = Some((n, tx));
@@ -258,15 +305,15 @@
             dst_port: dst_addr.port(),
         };
 
         let ip_repr: IpRepr = match (src_addr, dst_addr) {
             (SocketAddr::V4(src_addr), SocketAddr::V4(dst_addr)) => IpRepr::Ipv4(Ipv4Repr {
                 src_addr: Ipv4Address::from(*src_addr.ip()),
                 dst_addr: Ipv4Address::from(*dst_addr.ip()),
-                protocol: IpProtocol::Udp,
+                next_header: IpProtocol::Udp,
                 payload_len: udp_repr.header_len() + data.len(),
                 hop_limit: 255,
             }),
             (SocketAddr::V6(src_addr), SocketAddr::V6(dst_addr)) => IpRepr::Ipv6(Ipv6Repr {
                 src_addr: Ipv6Address::from(*src_addr.ip()),
                 dst_addr: Ipv6Address::from(*dst_addr.ip()),
                 next_header: IpProtocol::Udp,
@@ -275,28 +322,27 @@
             }),
             _ => {
                 log::error!("Failed to assemble UDP datagram: mismatched IP address versions");
                 return;
             }
         };
 
-        let buf = vec![0u8; ip_repr.total_len()];
+        let buf = vec![0u8; ip_repr.buffer_len()];
 
         let mut ip_packet = match ip_repr {
             IpRepr::Ipv4(repr) => {
                 let mut packet = Ipv4Packet::new_unchecked(buf);
                 repr.emit(&mut packet, &ChecksumCapabilities::default());
                 IpPacket::from(packet)
             }
             IpRepr::Ipv6(repr) => {
                 let mut packet = Ipv6Packet::new_unchecked(buf);
                 repr.emit(&mut packet);
                 IpPacket::from(packet)
             }
-            _ => unreachable!(),
         };
 
         udp_repr.emit(
             &mut UdpPacket::new_unchecked(ip_packet.payload_mut()),
             &ip_repr.src_addr(),
             &ip_repr.dst_addr(),
             data.len(),
@@ -342,94 +388,156 @@
                 src_addr,
                 dst_addr,
             } => {
                 self.send_datagram(data, src_addr, dst_addr);
             }
         }
     }
+}
 
-    fn poll_smol(&mut self) {
-        #[cfg(debug_assertions)]
-        log::debug!("Polling virtual network device ...");
-
-        loop {
-            match self.iface.poll(Instant::now()) {
-                Ok(_) => break,
-                Err(Error::Exhausted) => {
-                    log::debug!("smoltcp: exhausted.");
-                    break;
-                }
-                Err(e) => {
-                    // these can happen for "normal" reasons such as invalid packets,
-                    // we just write a log message and keep going.
-                    log::debug!("smoltcp network error: {}", e)
-                }
-            }
-        }
+fn handle_icmpv4_echo_request(mut input_packet: Ipv4Packet<Vec<u8>>) -> Option<IpPacket> {
+    let src_addr = input_packet.src_addr();
+    let dst_addr = input_packet.dst_addr();
+
+    // Parsing ICMP Packet
+    let mut input_icmpv4_packet = match Icmpv4Packet::new_checked(input_packet.payload_mut()) {
+        Ok(p) => p,
+        Err(e) => {
+            log::debug!("Received invalid ICMPv4 packet: {}", e);
+            return None;
+        }
+    };
+
+    // Checking that it is an ICMP Echo Request.
+    if input_icmpv4_packet.msg_type() != Icmpv4Message::EchoRequest {
+        log::debug!(
+            "Unsupported ICMPv4 packet of type: {}",
+            input_icmpv4_packet.msg_type()
+        );
+        return None;
     }
+
+    // Creating fake response packet.
+    let icmp_repr = Icmpv4Repr::EchoReply {
+        ident: input_icmpv4_packet.echo_ident(),
+        seq_no: input_icmpv4_packet.echo_seq_no(),
+        data: input_icmpv4_packet.data_mut(),
+    };
+    let ip_repr = Ipv4Repr {
+        // Directing fake reply back to the original source address.
+        src_addr: dst_addr,
+        dst_addr: src_addr,
+        next_header: IpProtocol::Icmp,
+        payload_len: icmp_repr.buffer_len(),
+        hop_limit: 255,
+    };
+    let buf = vec![0u8; ip_repr.buffer_len() + icmp_repr.buffer_len()];
+    let mut output_ipv4_packet = Ipv4Packet::new_unchecked(buf);
+    ip_repr.emit(&mut output_ipv4_packet, &ChecksumCapabilities::default());
+    let mut output_ip_packet = IpPacket::from(output_ipv4_packet);
+    icmp_repr.emit(
+        &mut Icmpv4Packet::new_unchecked(output_ip_packet.payload_mut()),
+        &ChecksumCapabilities::default(),
+    );
+    Some(output_ip_packet)
+}
+
+fn handle_icmpv6_echo_request(mut input_packet: Ipv6Packet<Vec<u8>>) -> Option<IpPacket> {
+    let src_addr = input_packet.src_addr();
+    let dst_addr = input_packet.dst_addr();
+
+    // Parsing ICMP Packet
+    let mut input_icmpv6_packet = match Icmpv6Packet::new_checked(input_packet.payload_mut()) {
+        Ok(p) => p,
+        Err(e) => {
+            log::debug!("Received invalid ICMPv6 packet: {}", e);
+            return None;
+        }
+    };
+
+    // Checking that it is an ICMP Echo Request.
+    if input_icmpv6_packet.msg_type() != Icmpv6Message::EchoRequest {
+        log::debug!(
+            "Unsupported ICMPv6 packet of type: {}",
+            input_icmpv6_packet.msg_type()
+        );
+        return None;
+    }
+
+    // Creating fake response packet.
+    let icmp_repr = Icmpv6Repr::EchoReply {
+        ident: input_icmpv6_packet.echo_ident(),
+        seq_no: input_icmpv6_packet.echo_seq_no(),
+        data: input_icmpv6_packet.payload_mut(),
+    };
+    let ip_repr = Ipv6Repr {
+        // Directing fake reply back to the original source address.
+        src_addr: dst_addr,
+        dst_addr: src_addr,
+        next_header: IpProtocol::Icmp,
+        payload_len: icmp_repr.buffer_len(),
+        hop_limit: 255,
+    };
+    let buf = vec![0u8; ip_repr.buffer_len() + icmp_repr.buffer_len()];
+    let mut output_ipv6_packet = Ipv6Packet::new_unchecked(buf);
+    ip_repr.emit(&mut output_ipv6_packet);
+    let mut output_ip_packet = IpPacket::from(output_ipv6_packet);
+    icmp_repr.emit(
+        // Directing fake reply back to the original source address.
+        &IpAddress::from(dst_addr),
+        &IpAddress::from(src_addr),
+        &mut Icmpv6Packet::new_unchecked(output_ip_packet.payload_mut()),
+        &ChecksumCapabilities::default(),
+    );
+    Some(output_ip_packet)
 }
 
-pub struct NetworkTask {
-    iface: Interface<'static, VirtualDevice>,
+pub struct NetworkTask<'a> {
     net_tx: Sender<NetworkCommand>,
     net_rx: Receiver<NetworkEvent>,
     py_tx: Sender<TransportEvent>,
     py_rx: UnboundedReceiver<TransportCommand>,
 
     sd_watcher: BroadcastReceiver<()>,
+    io: NetworkIO<'a>,
 }
 
-impl NetworkTask {
+impl NetworkTask<'_> {
     pub fn new(
         net_tx: Sender<NetworkCommand>,
         net_rx: Receiver<NetworkEvent>,
         py_tx: Sender<TransportEvent>,
         py_rx: UnboundedReceiver<TransportCommand>,
         sd_watcher: BroadcastReceiver<()>,
     ) -> Result<Self> {
-        let device = VirtualDevice::new(net_tx.clone());
-
-        let builder = InterfaceBuilder::new(device, vec![]);
-        let ip_addrs = [IpCidr::new(IpAddress::v4(0, 0, 0, 1), 0)];
-        let mut routes = Routes::new(BTreeMap::new());
-        // TODO: v6
-        routes
-            .add_default_ipv4_route(Ipv4Address::new(0, 0, 0, 1))
-            .unwrap();
-
-        let iface = builder
-            .any_ip(true)
-            .ip_addrs(ip_addrs)
-            .routes(routes)
-            .finalize();
-
+        let io = NetworkIO::new(net_tx.clone());
         Ok(Self {
-            iface,
             net_tx,
             net_rx,
             py_tx,
             py_rx,
             sd_watcher,
+            io,
         })
     }
 
     pub async fn run(mut self) -> Result<()> {
-        let mut io = NetworkIO::new(self.iface, self.net_tx.clone());
+        let mut io = self.io;
         let mut remove_conns = Vec::new();
 
         let mut py_tx_permit: Option<Permit<TransportEvent>> = None;
 
         'task: loop {
             // On a high level, we do three things in our main loop:
             // 1. Wait for an event from either side and handle it, or wait until the next smoltcp timeout.
             // 2. `.poll()` the smoltcp interface until it's finished with everything for now.
             // 3. Check if we can wake up any waiters, move more data in the send buffer, or clean up sockets.
 
             // check device for timeouts
-            let delay = io.iface.poll_delay(Instant::now());
+            let delay = io.iface.poll_delay(Instant::now(), &io.sockets);
 
             #[cfg(debug_assertions)]
             if let Some(d) = delay {
                 log::debug!("Waiting for device timeout: {} ...", d);
             }
 
             #[cfg(debug_assertions)]
@@ -473,21 +581,24 @@
                 },
                 // wait until channels are no longer full
                 Ok(()) = wait_for_channel_capacity(&self.py_tx), if py_tx_permit.is_none() => {},
                 Ok(()) = wait_for_channel_capacity(&self.net_tx), if net_tx_full => {},
             }
 
             // poll virtual network device
-            io.poll_smol();
+            #[cfg(debug_assertions)]
+            log::debug!("Polling virtual network device ...");
+            io.iface
+                .poll(Instant::now(), &mut io.device, &mut io.sockets);
 
             #[cfg(debug_assertions)]
             log::debug!("Processing TCP connections ...");
 
             for (connection_id, data) in io.socket_data.iter_mut() {
-                let socket = io.iface.get_socket::<TcpSocket>(data.handle);
+                let socket = io.sockets.get_mut::<tcp::Socket>(data.handle);
 
                 // receive data over the socket
                 if data.recv_waiter.is_some() {
                     if socket.can_recv() {
                         let (n, tx) = data.recv_waiter.take().unwrap();
                         let bytes_available = socket.recv_queue();
 
@@ -496,15 +607,15 @@
 
                         buf.truncate(bytes_read);
                         if tx.send(buf).is_err() {
                             log::debug!("Cannot send received data, channel was already closed.");
                         }
                     } else {
                         // We can't use .may_recv() here as it returns false during establishment.
-                        use TcpState::*;
+                        use tcp::State::*;
                         match socket.state() {
                             // can we still receive something in the future?
                             CloseWait | LastAck | Closed | Closing | TimeWait => {
                                 let (_, tx) = data.recv_waiter.take().unwrap();
                                 if tx.send(Vec::new()).is_err() {
                                     log::debug!("Cannot send close, channel was already closed.");
                                 }
@@ -545,50 +656,60 @@
                 // if requested, close socket
                 if data.write_eof && data.send_buffer.is_empty() {
                     socket.close();
                     data.write_eof = false;
                 }
 
                 // if socket is closed, mark connection for removal
-                if socket.state() == TcpState::Closed {
+                if socket.state() == tcp::State::Closed {
                     remove_conns.push(*connection_id);
                 }
             }
 
             for connection_id in remove_conns.drain(..) {
                 let data = io.socket_data.remove(&connection_id).unwrap();
-                io.iface.remove_socket(data.handle);
+                io.sockets.remove(data.handle);
                 io.active_connections.remove(&data.addr_tuple);
             }
 
             // poll again. we may have new stuff to do.
-            io.poll_smol();
+            #[cfg(debug_assertions)]
+            log::debug!("Polling virtual network device ...");
+            io.iface
+                .poll(Instant::now(), &mut io.device, &mut io.sockets);
         }
 
         // TODO: process remaining pending data after the shutdown request was received?
 
         log::debug!("Virtual Network device task shutting down.");
         Ok(())
     }
 }
 
-impl fmt::Debug for NetworkTask {
+impl fmt::Debug for NetworkTask<'_> {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         let sockets: Vec<String> = self
-            .iface
-            .sockets()
+            .io
+            .sockets
+            .iter()
             .filter_map(|(_h, s)| match s {
                 Socket::Tcp(s) => Some(s),
                 _ => None,
             })
             .map(|sock| {
                 format!(
                     "TCP {:<21} {:<21} {}",
-                    sock.remote_endpoint(),
-                    sock.local_endpoint(),
+                    sock.remote_endpoint()
+                        .map(|e| e.to_string())
+                        .as_ref()
+                        .map_or("not connected", String::as_str),
+                    sock.local_endpoint()
+                        .map(|e| e.to_string())
+                        .as_ref()
+                        .map_or("not connected", String::as_str),
                     sock.state()
                 )
             })
             .collect();
 
         f.debug_struct("NetworkTask")
             .field("sockets", &sockets)
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/tests.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/tests.rs`

 * *Files 10% similar despite different names*

```diff
@@ -119,20 +119,20 @@
         sack_ranges: [None, None, None],
         payload,
     };
 
     let ip_repr = Ipv4Repr {
         src_addr,
         dst_addr,
-        protocol: IpProtocol::Tcp,
+        next_header: IpProtocol::Tcp,
         payload_len: tcp_repr.header_len() + payload.len(),
         hop_limit: 255,
     };
 
-    let buf = vec![0u8; IpRepr::Ipv4(ip_repr).total_len()];
+    let buf = vec![0u8; IpRepr::Ipv4(ip_repr).buffer_len()];
 
     let mut ip_packet = Ipv4Packet::new_unchecked(buf);
     ip_repr.emit(&mut ip_packet, &ChecksumCapabilities::default());
 
     tcp_repr.emit(
         &mut TcpPacket::new_unchecked(ip_packet.payload_mut()),
         &ip_repr.src_addr.into(),
@@ -172,15 +172,15 @@
         src_addr,
         dst_addr,
         next_header: IpProtocol::Tcp,
         payload_len: tcp_repr.header_len() + payload.len(),
         hop_limit: 255,
     };
 
-    let buf = vec![0u8; IpRepr::Ipv6(ip_repr).total_len()];
+    let buf = vec![0u8; IpRepr::Ipv6(ip_repr).buffer_len()];
 
     let mut ip_packet = Ipv6Packet::new_unchecked(buf);
     ip_repr.emit(&mut ip_packet);
 
     tcp_repr.emit(
         &mut TcpPacket::new_unchecked(ip_packet.payload_mut()),
         &ip_repr.src_addr.into(),
@@ -199,20 +199,20 @@
     payload: &[u8],
 ) -> Ipv4Packet<Vec<u8>> {
     let udp_repr = UdpRepr { src_port, dst_port };
 
     let ip_repr = Ipv4Repr {
         src_addr,
         dst_addr,
-        protocol: IpProtocol::Udp,
+        next_header: IpProtocol::Udp,
         payload_len: udp_repr.header_len() + payload.len(),
         hop_limit: 255,
     };
 
-    let buf = vec![0u8; IpRepr::Ipv4(ip_repr).total_len()];
+    let buf = vec![0u8; IpRepr::Ipv4(ip_repr).buffer_len()];
 
     let mut ip_packet = Ipv4Packet::new_unchecked(buf);
     ip_repr.emit(&mut ip_packet, &ChecksumCapabilities::default());
 
     udp_repr.emit(
         &mut UdpPacket::new_unchecked(ip_packet.payload_mut()),
         &ip_repr.src_addr.into(),
@@ -238,15 +238,15 @@
         src_addr,
         dst_addr,
         next_header: IpProtocol::Udp,
         payload_len: udp_repr.header_len() + payload.len(),
         hop_limit: 255,
     };
 
-    let buf = vec![0u8; IpRepr::Ipv6(ip_repr).total_len()];
+    let buf = vec![0u8; IpRepr::Ipv6(ip_repr).buffer_len()];
 
     let mut ip_packet = Ipv6Packet::new_unchecked(buf);
     ip_repr.emit(&mut ip_packet);
 
     udp_repr.emit(
         &mut UdpPacket::new_unchecked(ip_packet.payload_mut()),
         &ip_repr.src_addr.into(),
@@ -255,14 +255,80 @@
         |buf| buf.copy_from_slice(payload),
         &ChecksumCapabilities::default(),
     );
 
     ip_packet
 }
 
+fn build_icmp4_echo_packet(
+    src_addr: Ipv4Address,
+    dst_addr: Ipv4Address,
+    ident: u16,
+    seq_no: u16,
+    data: &[u8],
+) -> Ipv4Packet<Vec<u8>> {
+    let icmp_repr = Icmpv4Repr::EchoRequest {
+        ident,
+        seq_no,
+        data,
+    };
+
+    let ip_repr = Ipv4Repr {
+        src_addr,
+        dst_addr,
+        next_header: IpProtocol::Icmp,
+        payload_len: icmp_repr.buffer_len(),
+        hop_limit: 255,
+    };
+
+    let buf = vec![0u8; ip_repr.buffer_len() + icmp_repr.buffer_len()];
+    let mut output_ipv4_packet = Ipv4Packet::new_unchecked(buf);
+    ip_repr.emit(&mut output_ipv4_packet, &ChecksumCapabilities::default());
+    icmp_repr.emit(
+        &mut Icmpv4Packet::new_unchecked(output_ipv4_packet.payload_mut()),
+        &ChecksumCapabilities::default(),
+    );
+
+    output_ipv4_packet
+}
+
+fn build_icmp6_echo_packet(
+    src_addr: Ipv6Address,
+    dst_addr: Ipv6Address,
+    ident: u16,
+    seq_no: u16,
+    data: &[u8],
+) -> Ipv6Packet<Vec<u8>> {
+    let icmp_repr = Icmpv6Repr::EchoRequest {
+        ident,
+        seq_no,
+        data,
+    };
+
+    let ip_repr = Ipv6Repr {
+        src_addr,
+        dst_addr,
+        next_header: IpProtocol::Icmp,
+        payload_len: icmp_repr.buffer_len(),
+        hop_limit: 255,
+    };
+
+    let buf = vec![0u8; ip_repr.buffer_len() + icmp_repr.buffer_len()];
+    let mut output_ipv6_packet = Ipv6Packet::new_unchecked(buf);
+    ip_repr.emit(&mut output_ipv6_packet);
+    icmp_repr.emit(
+        &IpAddress::from(src_addr),
+        &IpAddress::from(dst_addr),
+        &mut Icmpv6Packet::new_unchecked(output_ipv6_packet.payload_mut()),
+        &ChecksumCapabilities::default(),
+    );
+
+    output_ipv6_packet
+}
+
 fn init_logger() {
     let _ = env_logger::builder()
         .filter_level(log::LevelFilter::Debug)
         .is_test(true)
         .try_init();
 }
 
@@ -785,7 +851,83 @@
         Some(ack),
         &[],
     );
     mock.push_wg_packet(tcp_ip_syn_packet.into()).await?;
 
     mock.stop().await
 }
+
+#[tokio::test]
+async fn receive_icmp4_echo() -> Result<()> {
+    init_logger();
+    let mut mock = MockNetwork::init().await?;
+
+    let src_addr = Ipv4Address([10, 0, 0, 1]);
+    let dst_addr = Ipv4Address([10, 0, 0, 42]);
+    let data = "hello world!".as_bytes();
+
+    let icmp_echo_ip_packet = build_icmp4_echo_packet(src_addr, dst_addr, 42, 31337, data);
+
+    mock.push_wg_packet(icmp_echo_ip_packet.into()).await?;
+
+    let response = mock.pull_wg_packet().await.unwrap();
+
+    if let IpPacket::V4(mut response) = response {
+        // Checking that source and destination addresses were flipped and data was the same.
+        assert_eq!(src_addr, response.dst_addr());
+        assert_eq!(dst_addr, response.src_addr());
+
+        let mut input_icmpv4_packet = match Icmpv4Packet::new_checked(response.payload_mut()) {
+            Ok(p) => p,
+            Err(e) => {
+                return Err(anyhow!("Invalid ICMPv4 packet emitted: {}", e.to_string()));
+            }
+        };
+
+        assert_eq!(input_icmpv4_packet.msg_type(), Icmpv4Message::EchoReply);
+        assert_eq!(42, input_icmpv4_packet.echo_ident());
+        assert_eq!(31337, input_icmpv4_packet.echo_seq_no());
+        assert_eq!(data, input_icmpv4_packet.data_mut());
+    } else {
+        return Err(anyhow!("Wrong packet IP type emitted!"));
+    }
+
+    mock.stop().await
+}
+
+#[tokio::test]
+async fn receive_icmp6_echo() -> Result<()> {
+    init_logger();
+    let mut mock = MockNetwork::init().await?;
+
+    let src_addr = Ipv6Address(b"cafecafecafe0001".to_owned());
+    let dst_addr = Ipv6Address(b"cafecafecafe0002".to_owned());
+    let data = "hello world!".as_bytes();
+
+    let icmp_echo_ip_packet = build_icmp6_echo_packet(src_addr, dst_addr, 42, 31337, data);
+
+    mock.push_wg_packet(icmp_echo_ip_packet.into()).await?;
+
+    let response = mock.pull_wg_packet().await.unwrap();
+
+    if let IpPacket::V6(mut response) = response {
+        // Checking that source and destination addresses were flipped and data was the same.
+        assert_eq!(src_addr, response.dst_addr());
+        assert_eq!(dst_addr, response.src_addr());
+
+        let mut input_icmpv6_packet = match Icmpv6Packet::new_checked(response.payload_mut()) {
+            Ok(p) => p,
+            Err(e) => {
+                return Err(anyhow!("Invalid ICMPv6 packet emitted: {}", e.to_string()));
+            }
+        };
+
+        assert_eq!(input_icmpv6_packet.msg_type(), Icmpv6Message::EchoReply);
+        assert_eq!(42, input_icmpv6_packet.echo_ident());
+        assert_eq!(31337, input_icmpv6_packet.echo_seq_no());
+        assert_eq!(data, input_icmpv6_packet.payload_mut());
+    } else {
+        return Err(anyhow!("Wrong packet IP type emitted!"));
+    }
+
+    mock.stop().await
+}
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/network/virtual_device.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/virtual_device.rs`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     }
 
     pub fn receive_packet(&mut self, packet: IpPacket) {
         self.rx_buffer.push_back(packet.into_inner());
     }
 }
 
-impl<'a> Device<'a> for VirtualDevice {
-    type RxToken = VirtualRxToken;
-    type TxToken = VirtualTxToken<'a>;
+impl Device for VirtualDevice {
+    type RxToken<'a> = VirtualRxToken where Self: 'a;
+    type TxToken<'a> = VirtualTxToken<'a> where Self: 'a;
 
-    fn receive(&'a mut self) -> Option<(Self::RxToken, Self::TxToken)> {
+    fn receive(&mut self, _timestamp: Instant) -> Option<(Self::RxToken<'_>, Self::TxToken<'_>)> {
         if self.rx_buffer.is_empty() {
             return None;
         }
 
         if let Ok(permit) = self.tx_channel.try_reserve() {
             if let Some(buffer) = self.rx_buffer.pop_front() {
                 let rx = Self::RxToken { buffer };
@@ -44,15 +44,15 @@
                 return Some((rx, tx));
             }
         }
 
         None
     }
 
-    fn transmit(&'a mut self) -> Option<Self::TxToken> {
+    fn transmit(&mut self, _timestamp: Instant) -> Option<Self::TxToken<'_>> {
         match self.tx_channel.try_reserve() {
             Ok(permit) => Some(VirtualTxToken { permit }),
             Err(_) => None,
         }
     }
 
     fn capabilities(&self) -> DeviceCapabilities {
@@ -64,36 +64,39 @@
 }
 
 pub struct VirtualTxToken<'a> {
     permit: Permit<'a, NetworkCommand>,
 }
 
 impl<'a> TxToken for VirtualTxToken<'a> {
-    fn consume<R, F>(self, _timestamp: Instant, len: usize, f: F) -> smoltcp::Result<R>
+    fn consume<R, F>(self, len: usize, f: F) -> R
     where
-        F: FnOnce(&mut [u8]) -> smoltcp::Result<R>,
+        F: FnOnce(&mut [u8]) -> R,
     {
         let mut buffer = vec![0; len];
         let result = f(&mut buffer);
 
-        if result.is_ok() {
-            let cmd = NetworkCommand::SendPacket(
-                IpPacket::try_from(buffer).map_err(|_| smoltcp::Error::Malformed)?,
-            );
-            self.permit.send(cmd);
+        match IpPacket::try_from(buffer) {
+            Ok(packet) => {
+                self.permit.send(NetworkCommand::SendPacket(packet));
+            }
+            Err(err) => {
+                log::error!("Failed to parse packet from smol: {:?}", err)
+            }
         }
+
         result
     }
 }
 
 pub struct VirtualRxToken {
     buffer: Vec<u8>,
 }
 
 impl RxToken for VirtualRxToken {
-    fn consume<R, F>(mut self, _timestamp: Instant, f: F) -> smoltcp::Result<R>
+    fn consume<R, F>(mut self, f: F) -> R
     where
-        F: FnOnce(&mut [u8]) -> smoltcp::Result<R>,
+        F: FnOnce(&mut [u8]) -> R,
     {
         f(&mut self.buffer[..])
     }
 }
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/packet_sources/mod.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/mod.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/packet_sources/windows.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/windows.rs`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 use tokio::io::{AsyncReadExt, AsyncWriteExt};
 use tokio::net::windows::named_pipe::{NamedPipeServer, PipeMode, ServerOptions};
 use tokio::sync::broadcast;
 use tokio::sync::mpsc::Sender;
 use tokio::sync::mpsc::{unbounded_channel, Receiver, UnboundedReceiver, UnboundedSender};
 use windows::core::PCWSTR;
 use windows::w;
-use windows::Win32::Foundation::GetLastError;
 use windows::Win32::UI::Shell::ShellExecuteW;
 use windows::Win32::UI::Shell::SE_ERR_ACCESSDENIED;
 use windows::Win32::UI::WindowsAndMessaging::{SW_HIDE, SW_SHOWNORMAL};
 
 use crate::intercept_conf::InterceptConf;
 use crate::messages::{IpPacket, NetworkCommand, NetworkEvent, TunnelInfo};
 use crate::network::MAX_PACKET_SIZE;
@@ -26,15 +25,15 @@
 pub const IPC_BUF_SIZE: usize = MAX_PACKET_SIZE + 4;
 
 #[derive(Decode, Encode, PartialEq, Eq, Debug)]
 pub enum WindowsIpcRecv {
     Packet {
         data: Vec<u8>,
         pid: u32,
-        process_name: Option<String>,
+        process_name: Option<PathBuf>,
     },
 }
 
 #[derive(Decode, Encode, PartialEq, Eq, Debug)]
 pub enum WindowsIpcSend {
     Packet(Vec<u8>),
     SetIntercept(InterceptConf),
@@ -100,24 +99,24 @@
                     SW_HIDE
                 },
             )
         };
 
         if cfg!(debug_assertions) {
             if result.0 <= 32 {
-                let error_msg = unsafe { GetLastError().to_hresult().message().to_string_lossy() };
-                log::warn!("Failed to start child process: {}", error_msg);
+                let err = windows::core::Error::from_win32();
+                log::warn!("Failed to start child process: {}", err);
             }
         } else if result.0 == SE_ERR_ACCESSDENIED as isize {
             return Err(anyhow!(
                 "Failed to start the interception process as administrator."
             ));
         } else if result.0 <= 32 {
-            let error_msg = unsafe { GetLastError().to_hresult().message().to_string_lossy() };
-            return Err(anyhow!("Failed to start the executable: {}", error_msg));
+            let err = windows::core::Error::from_win32();
+            return Err(anyhow!("Failed to start the executable: {}", err));
         }
 
         let (conf_tx, conf_rx) = unbounded_channel();
 
         Ok((
             WindowsTask {
                 ipc_server,
```

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/shutdown.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/shutdown.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/local_dependencies/mitmproxy/src/windows.rs` & `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/network.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,16 @@
-use std::net::{Ipv4Addr, Ipv6Addr, SocketAddr};
-
 use anyhow::{anyhow, Result};
-use windows::core::PWSTR;
-use windows::Win32::Foundation::{CloseHandle, ERROR_INSUFFICIENT_BUFFER, MAX_PATH, NO_ERROR};
+use std::net::{Ipv4Addr, Ipv6Addr, SocketAddr};
+use windows::Win32::Foundation::{ERROR_INSUFFICIENT_BUFFER, NO_ERROR};
 use windows::Win32::NetworkManagement::IpHelper::{
     GetExtendedTcpTable, GetExtendedUdpTable, MIB_TCP6ROW_OWNER_PID, MIB_TCP6TABLE_OWNER_PID,
     MIB_TCPROW_OWNER_PID, MIB_TCPTABLE_OWNER_PID, MIB_UDP6ROW_OWNER_PID, MIB_UDP6TABLE_OWNER_PID,
     MIB_UDPROW_OWNER_PID, MIB_UDPTABLE_OWNER_PID, TCP_TABLE_OWNER_PID_ALL, UDP_TABLE_OWNER_PID,
 };
 use windows::Win32::Networking::WinSock::{AF_INET, AF_INET6};
-use windows::Win32::System::Threading::{
-    OpenProcess, QueryFullProcessImageNameW, PROCESS_NAME_NATIVE, PROCESS_NAME_WIN32,
-    PROCESS_QUERY_LIMITED_INFORMATION,
-};
-
-use crate::intercept_conf::PID;
-
-pub fn get_process_name(pid: PID) -> Result<String> {
-    let mut buffer = [0u16; MAX_PATH as usize];
-    let path = PWSTR(buffer.as_mut_ptr());
-    let mut len = buffer.len() as u32;
-
-    unsafe {
-        let handle = OpenProcess(PROCESS_QUERY_LIMITED_INFORMATION, false, pid)?;
-        // K32GetProcessImageFileNameW(handle, &mut buffer);
-        let query_ok = QueryFullProcessImageNameW(handle, PROCESS_NAME_WIN32, path, &mut len)
-            .ok()
-            .or_else(|_|
-                // WSL wants PROCESS_NAME_NATIVE, see https://github.com/microsoft/WSL/issues/3478
-                QueryFullProcessImageNameW(
-                    handle,
-                    PROCESS_NAME_NATIVE,
-                    path,
-                    &mut len,
-                ).ok());
-        CloseHandle(handle).ok()?;
-        // checking for success only after closing the handle.
-        query_ok?;
-        path.to_string().map_err(|e| anyhow!(e))
-    }
-}
 
 #[derive(Debug, Clone)]
 pub struct NetworkTableEntry {
     pub protocol: u8,
     pub local_addr: SocketAddr,
     pub remote_addr: SocketAddr,
     pub pid: u32,
@@ -65,15 +32,15 @@
                 false,
                 AF_INET.0.into(),
                 TCP_TABLE_OWNER_PID_ALL,
                 0,
             )
         };
         if res == ERROR_INSUFFICIENT_BUFFER.0 {
-            buf.resize(buf.len() * 2, 0);
+            buf.reserve(buf.capacity() + buf_size as usize);
         } else if res == NO_ERROR.0 {
             break;
         } else {
             return Err(anyhow!("failed to get tcp table"));
         }
     }
     let table = unsafe { &*(buf.as_ptr() as *const MIB_TCPTABLE_OWNER_PID) };
@@ -105,15 +72,15 @@
                 false,
                 AF_INET6.0.into(),
                 TCP_TABLE_OWNER_PID_ALL,
                 0,
             )
         };
         if res == ERROR_INSUFFICIENT_BUFFER.0 {
-            buf.resize(buf.len() * 2, 0);
+            buf.reserve(buf.capacity() + buf_size as usize);
         } else if res == NO_ERROR.0 {
             break;
         } else {
             return Err(anyhow!("failed to get tcp6 table"));
         }
     }
     let table = unsafe { &*(buf.as_ptr() as *const MIB_TCP6TABLE_OWNER_PID) };
@@ -145,15 +112,15 @@
                 false,
                 AF_INET.0.into(),
                 UDP_TABLE_OWNER_PID,
                 0,
             )
         };
         if res == ERROR_INSUFFICIENT_BUFFER.0 {
-            buf.resize(buf.len() * 2, 0);
+            buf.reserve(buf.capacity() + buf_size as usize);
         } else if res == NO_ERROR.0 {
             break;
         } else {
             return Err(anyhow!("failed to get udp table"));
         }
     }
     let table = unsafe { &*(buf.as_ptr() as *const MIB_UDPTABLE_OWNER_PID) };
@@ -182,15 +149,15 @@
                 false,
                 AF_INET6.0.into(),
                 UDP_TABLE_OWNER_PID,
                 0,
             )
         };
         if res == ERROR_INSUFFICIENT_BUFFER.0 {
-            buf.resize(buf.len() * 2, 0);
+            buf.reserve(buf.capacity() + buf_size as usize);
         } else if res == NO_ERROR.0 {
             break;
         } else {
             return Err(anyhow!("failed to get udp6 table"));
         }
     }
     let table = unsafe { &*(buf.as_ptr() as *const MIB_UDP6TABLE_OWNER_PID) };
@@ -214,20 +181,14 @@
 }
 
 #[cfg(test)]
 mod tests {
     use std::net::{TcpListener, UdpSocket};
 
     #[test]
-    fn get_process_name() {
-        let name = super::get_process_name(std::process::id()).unwrap();
-        assert!(name.contains("mitmproxy"));
-    }
-
-    #[test]
     fn network_table() {
         let tcp_listener = TcpListener::bind("127.0.0.1:0").unwrap();
         let udp_socket = UdpSocket::bind("127.0.0.1:0").unwrap();
 
         let table = super::network_table().unwrap();
         println!("{table:#?}");
```

### Comparing `mitmproxy_rs-0.2.0b8/Cargo.toml` & `mitmproxy_rs-0.2.0b9/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [package]
 name = "mitmproxy_rs"
 license = "MIT"
 authors= [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version= "0.2.0-beta.8"
+version= "0.2.0-beta.9"
 repository= "https://github.com/mitmproxy/mitmproxy-rs"
 edition= "2021"
 rust-version= "1.65.0"
 publish= false
 
 [lib]
 name = "mitmproxy_rs"
 crate-type = ["cdylib"]
 
 [dependencies]
 mitmproxy = { path = "local_dependencies/mitmproxy" }
-anyhow = { version = "1.0.68", features = ["backtrace"] }
-data-encoding = "2.3.3"
-log = "0.4.17"
+anyhow = { version = "1.0.71", features = ["backtrace"] }
+data-encoding = "2.4.0"
+log = "0.4.18"
 once_cell = "1"
-pyo3 = { version = "0.17.3", features = ["abi3", "abi3-py39", "extension-module", "anyhow"] }
-pyo3-asyncio = { version = "0.17", features = ["tokio-runtime"] }
-pyo3-log = "0.8"
+pyo3 = { version = "0.18.2", features = ["abi3", "abi3-py310", "extension-module", "anyhow"] }
+pyo3-asyncio = { version = "0.18.0", features = ["tokio-runtime"] }
+pyo3-log = "0.8.1"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
-tokio = { version = "1.23", features = ["macros", "net", "rt-multi-thread", "sync"] }
+tokio = { version = "1.27", features = ["macros", "net", "rt-multi-thread", "sync"] }
 x25519-dalek = "2.0.0-pre.1"
 
 # optional dependencies for tracing support
-console-subscriber = { version = "0.1.8", optional = true }
+console-subscriber = { version = "0.1.9", optional = true }
 
 [features]
 tracing = ["console-subscriber"]
```

### Comparing `mitmproxy_rs-0.2.0b8/README.md` & `mitmproxy_rs-0.2.0b9/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/build.rs` & `mitmproxy_rs-0.2.0b9/build.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/mitmproxy_rs/__init__.pyi` & `mitmproxy_rs-0.2.0b9/mitmproxy_rs/__init__.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from __future__ import annotations
+
+from pathlib import Path
 from typing import Awaitable, Callable, Any
 from typing import final
 
 
 # WireGuard
 
 async def start_wireguard_server(
@@ -55,18 +57,37 @@
 
     def get_extra_info(self, name: str, default: Any = None) -> Any: ...
     def __repr__(self) -> str: ...
 
 
 @final
 class DatagramTransport:
-    def sendto(self, data: bytes, addr: tuple[str, int]): ...
+    def sendto(self, data: bytes, addr: tuple[str, int] | None = None): ...
     async def drain(self) -> None: ...
 
     def close(self): ...
     def is_closing(self) -> bool: ...
     async def wait_closed(self) -> None: ...
 
     def get_extra_info(self, name: str, default: Any = None) -> Any: ...
     def __repr__(self) -> str: ...
 
     def get_protocol(self) -> DatagramTransport: ...
+
+
+# Process Info
+
+
+def active_executables() -> list[Process]: ...
+def executable_icon(path: Path | str) -> bytes: ...
+
+@final
+class Process:
+    @property
+    def executable(self) -> str: ...
+    @property
+    def display_name(self) -> str: ...
+    @property
+    def is_visible(self) -> bool: ...
+    @property
+    def is_system(self) -> bool: ...
+
```

### Comparing `mitmproxy_rs-0.2.0b8/pyproject.toml` & `mitmproxy_rs-0.2.0b9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,12 @@
 
 [tool.black]
 line-length = 140
 include = '\.pyi?$'
 
 [project.entry-points.pyinstaller40]
 hook-dirs = "mitmproxy_rs._pyinstaller:hook_dirs"
+
+[tool.mypy]
+exclude = [
+    'mitmproxy_rs/_pyinstaller'
+]
```

### Comparing `mitmproxy_rs-0.2.0b8/src/datagram_transport.rs` & `mitmproxy_rs-0.2.0b9/src/datagram_transport.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 use pyo3::{exceptions::PyKeyError, prelude::*};
 use tokio::sync::mpsc;
 
 use mitmproxy::messages::{TransportCommand, TunnelInfo};
 
 use crate::util::{event_queue_unavailable, py_to_socketaddr, socketaddr_to_py};
 
-#[pyclass]
+#[pyclass(module = "mitmproxy_rs")]
 #[derive(Debug)]
 pub struct DatagramTransport {
     pub event_tx: mpsc::UnboundedSender<TransportCommand>,
     pub peername: SocketAddr,
     pub sockname: SocketAddr,
     pub tunnel_info: TunnelInfo,
 }
 
 #[pymethods]
 impl DatagramTransport {
-    #[args(addr = "None")]
+    #[pyo3(text_signature = "(self, data, addr=None)")]
     fn sendto(&self, data: Vec<u8>, addr: Option<&PyTuple>) -> PyResult<()> {
         let dst_addr = match addr {
             Some(addr) => py_to_socketaddr(addr)?,
             None => self.peername,
         };
         self.event_tx
             .send(TransportCommand::SendDatagram {
@@ -34,15 +34,15 @@
             .map_err(event_queue_unavailable)?;
         Ok(())
     }
 
     /// Query the UDP transport for details of the underlying network connection.
     ///
     /// Supported values: `peername`, `sockname`, `original_src`, and `original_dst`.
-    #[args(default = "None")]
+    #[pyo3(text_signature = "(self, name, default=None)")]
     fn get_extra_info(
         &self,
         py: Python,
         name: String,
         default: Option<PyObject>,
     ) -> PyResult<PyObject> {
         match (name.as_str(), default) {
```

### Comparing `mitmproxy_rs-0.2.0b8/src/lib.rs` & `mitmproxy_rs-0.2.0b9/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 use std::sync::RwLock;
 
 use once_cell::sync::Lazy;
 use pyo3::{exceptions::PyException, prelude::*};
 
 mod datagram_transport;
+mod process_info;
 mod server;
 mod task;
 mod tcp_stream;
 mod util;
 
 static LOGGER_INITIALIZED: Lazy<RwLock<bool>> = Lazy::new(|| RwLock::new(false));
 
@@ -42,12 +43,16 @@
     m.add_class::<server::WireGuardServer>()?;
     m.add_function(wrap_pyfunction!(util::genkey, m)?)?;
     m.add_function(wrap_pyfunction!(util::pubkey, m)?)?;
 
     m.add_function(wrap_pyfunction!(server::start_os_proxy, m)?)?;
     m.add_class::<server::OsProxy>()?;
 
+    m.add_function(wrap_pyfunction!(process_info::active_executables, m)?)?;
+    m.add_class::<process_info::Process>()?;
+    m.add_function(wrap_pyfunction!(process_info::executable_icon, m)?)?;
+
     m.add_class::<tcp_stream::TcpStream>()?;
     m.add_class::<datagram_transport::DatagramTransport>()?;
 
     Ok(())
 }
```

### Comparing `mitmproxy_rs-0.2.0b8/src/server.rs` & `mitmproxy_rs-0.2.0b9/src/server.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,305 +1,305 @@
-use std::net::SocketAddr;
-
-use std::sync::Arc;
-
-#[allow(unused_imports)]
-use anyhow::{anyhow, Result};
-use pyo3::prelude::*;
-use tokio::{sync::broadcast, sync::mpsc, sync::Notify};
-use x25519_dalek::PublicKey;
-
-use mitmproxy::intercept_conf::InterceptConf;
-use mitmproxy::network::NetworkTask;
-#[cfg(windows)]
-use mitmproxy::packet_sources::windows::{WindowsConf, WindowsIpcSend};
-
-use mitmproxy::packet_sources::wireguard::WireGuardConf;
-use mitmproxy::packet_sources::{PacketSourceConf, PacketSourceTask};
-use mitmproxy::shutdown::ShutdownTask;
-
-use crate::task::PyInteropTask;
-use crate::util::{socketaddr_to_py, string_to_key};
-
-#[derive(Debug)]
-pub struct Server {
-    /// channel for notifying subtasks of requested server shutdown
-    sd_trigger: broadcast::Sender<()>,
-    /// channel for getting notified of successful server shutdown
-    sd_barrier: Arc<Notify>,
-    /// flag to indicate whether server shutdown is in progress
-    closing: bool,
-}
-
-impl Server {
-    pub fn close(&mut self) {
-        if !self.closing {
-            self.closing = true;
-            log::info!("Shutting down.");
-
-            // notify tasks to shut down
-            let _ = self.sd_trigger.send(());
-        }
-    }
-
-    pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
-        let barrier = self.sd_barrier.clone();
-
-        pyo3_asyncio::tokio::future_into_py(py, async move {
-            barrier.notified().await;
-            Ok(())
-        })
-    }
-}
-
-impl Server {
-    /// Set up and initialize a new WireGuard server.
-    pub async fn init<T>(
-        packet_source_conf: T,
-        py_tcp_handler: PyObject,
-        py_udp_handler: PyObject,
-    ) -> Result<(Self, T::Data)>
-    where
-        T: PacketSourceConf,
-    {
-        let typ = packet_source_conf.name();
-        log::debug!("Initializing {} ...", typ);
-
-        // initialize channels between the WireGuard server and the virtual network device
-        let (wg_to_smol_tx, wg_to_smol_rx) = mpsc::channel(256);
-        let (smol_to_wg_tx, smol_to_wg_rx) = mpsc::channel(256);
-
-        // initialize channels between the virtual network device and the python interop task
-        // - only used to notify of incoming connections and datagrams
-        let (smol_to_py_tx, smol_to_py_rx) = mpsc::channel(256);
-        // - used to send data and to ask for packets
-        // This channel needs to be unbounded because write() is not async.
-        let (py_to_smol_tx, py_to_smol_rx) = mpsc::unbounded_channel();
-
-        // initialize barriers for handling graceful shutdown
-        let (sd_trigger, _sd_watcher) = broadcast::channel(1);
-        let sd_barrier = Arc::new(Notify::new());
-
-        let (wg_task, data) = packet_source_conf
-            .build(wg_to_smol_tx, smol_to_wg_rx, sd_trigger.subscribe())
-            .await?;
-
-        // initialize virtual network device
-        let nw_task = NetworkTask::new(
-            smol_to_wg_tx,
-            wg_to_smol_rx,
-            smol_to_py_tx,
-            py_to_smol_rx,
-            sd_trigger.subscribe(),
-        )?;
-
-        // initialize Python interop task
-        // Note: The current asyncio event loop needs to be determined here on the main thread.
-        let py_loop: PyObject = Python::with_gil(|py| {
-            let py_loop = pyo3_asyncio::tokio::get_current_loop(py)?.into_py(py);
-            Ok::<PyObject, PyErr>(py_loop)
-        })?;
-
-        let py_task = PyInteropTask::new(
-            py_loop,
-            py_to_smol_tx,
-            smol_to_py_rx,
-            py_tcp_handler,
-            py_udp_handler,
-            sd_trigger.subscribe(),
-        );
-
-        // spawn tasks
-        let wg_handle = tokio::spawn(async move { wg_task.run().await });
-        let net_handle = tokio::spawn(async move { nw_task.run().await });
-        let py_handle = tokio::spawn(async move { py_task.run().await });
-
-        // initialize and run shutdown handler
-        let sd_task = ShutdownTask::new(
-            py_handle,
-            wg_handle,
-            net_handle,
-            sd_trigger.clone(),
-            sd_barrier.clone(),
-        );
-        tokio::spawn(async move { sd_task.run().await });
-
-        log::debug!("{} successfully initialized.", typ);
-
-        Ok((
-            Server {
-                sd_trigger,
-                sd_barrier,
-                closing: false,
-            },
-            data,
-        ))
-    }
-}
-
-impl Drop for Server {
-    fn drop(&mut self) {
-        self.close()
-    }
-}
-
-#[pyclass]
-#[derive(Debug)]
-pub struct OsProxy {
-    server: Server,
-    #[cfg(windows)]
-    conf_tx: mpsc::UnboundedSender<WindowsIpcSend>,
-}
-
-#[pymethods]
-impl OsProxy {
-    /// Return a textual description of the given spec,
-    /// or raise a ValueError if the spec is invalid.
-    #[staticmethod]
-    fn describe_spec(spec: &str) -> PyResult<String> {
-        InterceptConf::try_from(spec)
-            .map(|conf| conf.description())
-            .map_err(|e| pyo3::exceptions::PyValueError::new_err(e.to_string()))
-    }
-
-    /// Set a new intercept spec.
-    pub fn set_intercept(&self, spec: &str) -> PyResult<()> {
-        let _conf = InterceptConf::try_from(spec)?;
-        #[cfg(windows)]
-        self.conf_tx
-            .send(WindowsIpcSend::SetIntercept(_conf))
-            .map_err(crate::util::event_queue_unavailable)?;
-        Ok(())
-    }
-
-    /// Close the OS proxy server.
-    pub fn close(&mut self) {
-        self.server.close()
-    }
-
-    pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
-        self.server.wait_closed(py)
-    }
-}
-
-/// A running WireGuard server.
-///
-/// A new server can be started by calling the `start_wireguard_server` coroutine. Its public API is intended
-/// to be similar to the API provided by
-/// [`asyncio.Server`](https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.Server)
-/// from the Python standard library.
-#[pyclass]
-#[derive(Debug)]
-pub struct WireGuardServer {
-    /// local address of the WireGuard UDP socket
-    local_addr: SocketAddr,
-    server: Server,
-}
-
-#[pymethods]
-impl WireGuardServer {
-    /// Request the WireGuard server to gracefully shut down.
-    ///
-    /// The server will stop accepting new connections on its UDP socket, but will flush pending
-    /// outgoing data before shutting down.
-    pub fn close(&mut self) {
-        self.server.close()
-    }
-
-    /// Wait until the WireGuard server has shut down.
-    ///
-    /// This coroutine will yield once pending data has been flushed and all server tasks have
-    /// successfully terminated after calling the `Server.close` method.
-    pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
-        self.server.wait_closed(py)
-    }
-
-    /// Get the local socket address that the WireGuard server is listening on.
-    pub fn getsockname(&self, py: Python) -> PyObject {
-        socketaddr_to_py(py, self.local_addr)
-    }
-
-    pub fn __repr__(&self) -> String {
-        format!("WireGuardServer({})", self.local_addr)
-    }
-}
-
-/// Start a WireGuard server that is configured with the given parameters:
-///
-/// - `host`: The host address for the WireGuard UDP socket.
-/// - `port`: The listen port for the WireGuard server. The default port for WireGuard is `51820`.
-/// - `private_key`: The private X25519 key for the WireGuard server as a base64-encoded string.
-/// - `peer_public_keys`: List of public X25519 keys for WireGuard peers as base64-encoded strings.
-/// - `handle_connection`: A coroutine that will be called for each new `TcpStream`.
-/// - `receive_datagram`: A function that will be called for each received UDP datagram.
-///
-/// The `receive_datagram` function will be called with the following arguments:
-///
-/// - payload of the UDP datagram as `bytes`
-/// - source address as `(host: str, port: int)` tuple
-/// - destination address as `(host: str, port: int)` tuple
-#[pyfunction]
-pub fn start_wireguard_server(
-    py: Python<'_>,
-    host: String,
-    port: u16,
-    private_key: String,
-    peer_public_keys: Vec<String>,
-    handle_connection: PyObject,
-    receive_datagram: PyObject,
-) -> PyResult<&PyAny> {
-    let private_key = string_to_key(private_key)?;
-
-    let peer_public_keys = peer_public_keys
-        .into_iter()
-        .map(string_to_key)
-        .collect::<PyResult<Vec<PublicKey>>>()?;
-
-    let conf = WireGuardConf {
-        host,
-        port,
-        private_key,
-        peer_public_keys,
-    };
-
-    pyo3_asyncio::tokio::future_into_py(py, async move {
-        let (server, local_addr) = Server::init(conf, handle_connection, receive_datagram).await?;
-        Ok(WireGuardServer { server, local_addr })
-    })
-}
-
-/// Start an OS-level proxy to intercept traffic from the current machine.
-///
-/// *Availability: Windows*
-#[pyfunction]
-#[allow(unused_variables)]
-pub fn start_os_proxy(
-    py: Python<'_>,
-    handle_connection: PyObject,
-    receive_datagram: PyObject,
-) -> PyResult<&PyAny> {
-    #[cfg(windows)]
-    {
-        // 2022: Ideally we'd use importlib.resources here, but that only provides `as_file` for
-        // individual files. We'd need something like `as_dir` to ensure that redirector.exe and the
-        // WinDivert dll/lib/sys files are in a single directory. So we just use __file__for now. 🤷
-        let filename = py.import("mitmproxy_rs")?.filename()?;
-        let executable_path = std::path::Path::new(filename)
-            .parent()
-            .ok_or_else(|| anyhow!("invalid path"))?
-            .join("windows-redirector.exe");
-
-        if !executable_path.exists() {
-            return Err(anyhow!("{} does not exist", executable_path.display()).into());
-        }
-        let conf = WindowsConf { executable_path };
+use std::net::SocketAddr;
+
+use std::sync::Arc;
+
+#[allow(unused_imports)]
+use anyhow::{anyhow, Result};
+use pyo3::prelude::*;
+use tokio::{sync::broadcast, sync::mpsc, sync::Notify};
+use x25519_dalek::PublicKey;
+
+use mitmproxy::intercept_conf::InterceptConf;
+use mitmproxy::network::NetworkTask;
+#[cfg(windows)]
+use mitmproxy::packet_sources::windows::{WindowsConf, WindowsIpcSend};
+
+use mitmproxy::packet_sources::wireguard::WireGuardConf;
+use mitmproxy::packet_sources::{PacketSourceConf, PacketSourceTask};
+use mitmproxy::shutdown::ShutdownTask;
+
+use crate::task::PyInteropTask;
+use crate::util::{socketaddr_to_py, string_to_key};
+
+#[derive(Debug)]
+pub struct Server {
+    /// channel for notifying subtasks of requested server shutdown
+    sd_trigger: broadcast::Sender<()>,
+    /// channel for getting notified of successful server shutdown
+    sd_barrier: Arc<Notify>,
+    /// flag to indicate whether server shutdown is in progress
+    closing: bool,
+}
+
+impl Server {
+    pub fn close(&mut self) {
+        if !self.closing {
+            self.closing = true;
+            log::info!("Shutting down.");
+
+            // notify tasks to shut down
+            let _ = self.sd_trigger.send(());
+        }
+    }
+
+    pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        let barrier = self.sd_barrier.clone();
+
+        pyo3_asyncio::tokio::future_into_py(py, async move {
+            barrier.notified().await;
+            Ok(())
+        })
+    }
+}
+
+impl Server {
+    /// Set up and initialize a new WireGuard server.
+    pub async fn init<T>(
+        packet_source_conf: T,
+        py_tcp_handler: PyObject,
+        py_udp_handler: PyObject,
+    ) -> Result<(Self, T::Data)>
+    where
+        T: PacketSourceConf,
+    {
+        let typ = packet_source_conf.name();
+        log::debug!("Initializing {} ...", typ);
+
+        // initialize channels between the WireGuard server and the virtual network device
+        let (wg_to_smol_tx, wg_to_smol_rx) = mpsc::channel(256);
+        let (smol_to_wg_tx, smol_to_wg_rx) = mpsc::channel(256);
+
+        // initialize channels between the virtual network device and the python interop task
+        // - only used to notify of incoming connections and datagrams
+        let (smol_to_py_tx, smol_to_py_rx) = mpsc::channel(256);
+        // - used to send data and to ask for packets
+        // This channel needs to be unbounded because write() is not async.
+        let (py_to_smol_tx, py_to_smol_rx) = mpsc::unbounded_channel();
+
+        // initialize barriers for handling graceful shutdown
+        let (sd_trigger, _sd_watcher) = broadcast::channel(1);
+        let sd_barrier = Arc::new(Notify::new());
+
+        let (wg_task, data) = packet_source_conf
+            .build(wg_to_smol_tx, smol_to_wg_rx, sd_trigger.subscribe())
+            .await?;
+
+        // initialize virtual network device
+        let nw_task = NetworkTask::new(
+            smol_to_wg_tx,
+            wg_to_smol_rx,
+            smol_to_py_tx,
+            py_to_smol_rx,
+            sd_trigger.subscribe(),
+        )?;
+
+        // initialize Python interop task
+        // Note: The current asyncio event loop needs to be determined here on the main thread.
+        let py_loop: PyObject = Python::with_gil(|py| {
+            let py_loop = pyo3_asyncio::tokio::get_current_loop(py)?.into_py(py);
+            Ok::<PyObject, PyErr>(py_loop)
+        })?;
+
+        let py_task = PyInteropTask::new(
+            py_loop,
+            py_to_smol_tx,
+            smol_to_py_rx,
+            py_tcp_handler,
+            py_udp_handler,
+            sd_trigger.subscribe(),
+        );
+
+        // spawn tasks
+        let wg_handle = tokio::spawn(async move { wg_task.run().await });
+        let net_handle = tokio::spawn(async move { nw_task.run().await });
+        let py_handle = tokio::spawn(async move { py_task.run().await });
+
+        // initialize and run shutdown handler
+        let sd_task = ShutdownTask::new(
+            py_handle,
+            wg_handle,
+            net_handle,
+            sd_trigger.clone(),
+            sd_barrier.clone(),
+        );
+        tokio::spawn(async move { sd_task.run().await });
+
+        log::debug!("{} successfully initialized.", typ);
+
+        Ok((
+            Server {
+                sd_trigger,
+                sd_barrier,
+                closing: false,
+            },
+            data,
+        ))
+    }
+}
+
+impl Drop for Server {
+    fn drop(&mut self) {
+        self.close()
+    }
+}
+
+#[pyclass(module = "mitmproxy_rs")]
+#[derive(Debug)]
+pub struct OsProxy {
+    server: Server,
+    #[cfg(windows)]
+    conf_tx: mpsc::UnboundedSender<WindowsIpcSend>,
+}
+
+#[pymethods]
+impl OsProxy {
+    /// Return a textual description of the given spec,
+    /// or raise a ValueError if the spec is invalid.
+    #[staticmethod]
+    fn describe_spec(spec: &str) -> PyResult<String> {
+        InterceptConf::try_from(spec)
+            .map(|conf| conf.description())
+            .map_err(|e| pyo3::exceptions::PyValueError::new_err(e.to_string()))
+    }
+
+    /// Set a new intercept spec.
+    pub fn set_intercept(&self, spec: &str) -> PyResult<()> {
+        let _conf = InterceptConf::try_from(spec)?;
+        #[cfg(windows)]
+        self.conf_tx
+            .send(WindowsIpcSend::SetIntercept(_conf))
+            .map_err(crate::util::event_queue_unavailable)?;
+        Ok(())
+    }
+
+    /// Close the OS proxy server.
+    pub fn close(&mut self) {
+        self.server.close()
+    }
+
+    pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        self.server.wait_closed(py)
+    }
+}
+
+/// A running WireGuard server.
+///
+/// A new server can be started by calling the `start_wireguard_server` coroutine. Its public API is intended
+/// to be similar to the API provided by
+/// [`asyncio.Server`](https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.Server)
+/// from the Python standard library.
+#[pyclass(module = "mitmproxy_rs")]
+#[derive(Debug)]
+pub struct WireGuardServer {
+    /// local address of the WireGuard UDP socket
+    local_addr: SocketAddr,
+    server: Server,
+}
+
+#[pymethods]
+impl WireGuardServer {
+    /// Request the WireGuard server to gracefully shut down.
+    ///
+    /// The server will stop accepting new connections on its UDP socket, but will flush pending
+    /// outgoing data before shutting down.
+    pub fn close(&mut self) {
+        self.server.close()
+    }
+
+    /// Wait until the WireGuard server has shut down.
+    ///
+    /// This coroutine will yield once pending data has been flushed and all server tasks have
+    /// successfully terminated after calling the `Server.close` method.
+    pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
+        self.server.wait_closed(py)
+    }
+
+    /// Get the local socket address that the WireGuard server is listening on.
+    pub fn getsockname(&self, py: Python) -> PyObject {
+        socketaddr_to_py(py, self.local_addr)
+    }
+
+    pub fn __repr__(&self) -> String {
+        format!("WireGuardServer({})", self.local_addr)
+    }
+}
+
+/// Start a WireGuard server that is configured with the given parameters:
+///
+/// - `host`: The host address for the WireGuard UDP socket.
+/// - `port`: The listen port for the WireGuard server. The default port for WireGuard is `51820`.
+/// - `private_key`: The private X25519 key for the WireGuard server as a base64-encoded string.
+/// - `peer_public_keys`: List of public X25519 keys for WireGuard peers as base64-encoded strings.
+/// - `handle_connection`: A coroutine that will be called for each new `TcpStream`.
+/// - `receive_datagram`: A function that will be called for each received UDP datagram.
+///
+/// The `receive_datagram` function will be called with the following arguments:
+///
+/// - payload of the UDP datagram as `bytes`
+/// - source address as `(host: str, port: int)` tuple
+/// - destination address as `(host: str, port: int)` tuple
+#[pyfunction]
+pub fn start_wireguard_server(
+    py: Python<'_>,
+    host: String,
+    port: u16,
+    private_key: String,
+    peer_public_keys: Vec<String>,
+    handle_connection: PyObject,
+    receive_datagram: PyObject,
+) -> PyResult<&PyAny> {
+    let private_key = string_to_key(private_key)?;
+
+    let peer_public_keys = peer_public_keys
+        .into_iter()
+        .map(string_to_key)
+        .collect::<PyResult<Vec<PublicKey>>>()?;
+
+    let conf = WireGuardConf {
+        host,
+        port,
+        private_key,
+        peer_public_keys,
+    };
+
+    pyo3_asyncio::tokio::future_into_py(py, async move {
+        let (server, local_addr) = Server::init(conf, handle_connection, receive_datagram).await?;
+        Ok(WireGuardServer { server, local_addr })
+    })
+}
+
+/// Start an OS-level proxy to intercept traffic from the current machine.
+///
+/// *Availability: Windows*
+#[pyfunction]
+#[allow(unused_variables)]
+pub fn start_os_proxy(
+    py: Python<'_>,
+    handle_connection: PyObject,
+    receive_datagram: PyObject,
+) -> PyResult<&PyAny> {
+    #[cfg(windows)]
+    {
+        // 2022: Ideally we'd use importlib.resources here, but that only provides `as_file` for
+        // individual files. We'd need something like `as_dir` to ensure that redirector.exe and the
+        // WinDivert dll/lib/sys files are in a single directory. So we just use __file__for now. 🤷
+        let filename = py.import("mitmproxy_rs")?.filename()?;
+        let executable_path = std::path::Path::new(filename)
+            .parent()
+            .ok_or_else(|| anyhow!("invalid path"))?
+            .join("windows-redirector.exe");
+
+        if !executable_path.exists() {
+            return Err(anyhow!("{} does not exist", executable_path.display()).into());
+        }
+        let conf = WindowsConf { executable_path };
         pyo3_asyncio::tokio::future_into_py(py, async move {
             let (server, conf_tx) = Server::init(conf, handle_connection, receive_datagram).await?;
 
             Ok(OsProxy { server, conf_tx })
-        })
-    }
-    #[cfg(not(windows))]
-    Err(pyo3::exceptions::PyNotImplementedError::new_err(
-        "OS proxy mode is only available on Windows",
-    ))
-}
+        })
+    }
+    #[cfg(not(windows))]
+    Err(pyo3::exceptions::PyNotImplementedError::new_err(
+        "OS proxy mode is only available on Windows",
+    ))
+}
```

### Comparing `mitmproxy_rs-0.2.0b8/src/task.rs` & `mitmproxy_rs-0.2.0b9/src/task.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/src/tcp_stream.rs` & `mitmproxy_rs-0.2.0b9/src/tcp_stream.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 use mitmproxy::messages::{ConnectionId, TransportCommand, TunnelInfo};
 
 use crate::util::{event_queue_unavailable, socketaddr_to_py};
 
 /// An individual TCP stream with an API that is similar to
 /// [`asyncio.StreamReader` and `asyncio.StreamWriter`](https://docs.python.org/3/library/asyncio-stream.html)
 /// from the Python standard library.
-#[pyclass]
+#[pyclass(module = "mitmproxy_rs")]
 #[derive(Debug)]
 pub struct TcpStream {
     pub connection_id: ConnectionId,
     pub event_tx: mpsc::UnboundedSender<TransportCommand>,
     pub peername: SocketAddr,
     pub sockname: SocketAddr,
     pub tunnel_info: TunnelInfo,
@@ -101,15 +101,15 @@
     fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
         pyo3_asyncio::tokio::future_into_py(py, std::future::ready(Ok(())))
     }
 
     /// Query the TCP stream for details of the underlying network connection.
     ///
     /// Supported values: `peername`, `sockname`, `original_dst`, and `original_src`.
-    #[args(default = "None")]
+    #[pyo3(text_signature = "(self, name, default=None)")]
     fn get_extra_info(
         &self,
         py: Python,
         name: String,
         default: Option<PyObject>,
     ) -> PyResult<PyObject> {
         match (name.as_str(), default) {
```

### Comparing `mitmproxy_rs-0.2.0b8/src/util.rs` & `mitmproxy_rs-0.2.0b9/src/util.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b8/Cargo.lock` & `mitmproxy_rs-0.2.0b9/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -15,88 +15,76 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aead"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c192eb8f11fc081b0fe4259ba5af04217d4e0faddd02417310a927911abd7c8"
+checksum = "d122413f284cf2d62fb1b7db97e02edb8cda96d769b16e443a4f6195e35662b0"
 dependencies = [
  "crypto-common",
  "generic-array",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anyhow"
-version = "1.0.69"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "224afbd727c3d6e4b90103ece64b8d1b67fbb1973b1046c2281eed3f3803f800"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+checksum = "8868f09ff8cea88b079da74ae569d9b8c62a23c68c746240b704ee6f7525c89c"
 
 [[package]]
-name = "async-stream"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dad5c83079eae9969be7fadefe640a1c566901f05ff91ab221de4b6f68d9507e"
-dependencies = [
- "async-stream-impl",
- "futures-core",
-]
-
-[[package]]
-name = "async-stream-impl"
-version = "0.3.3"
+name = "async-trait"
+version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10f203db73a71dfa2fb6dd22763990fa26f3d2625a6da2da900d23b87d26be27"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
-name = "async-trait"
-version = "0.1.64"
+name = "atomic-polyfill"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd7fce9ba8c3c042128ce72d8b2ddbf3a05747efb67ea0313c635e10bda47a2"
+checksum = "e3ff7eb3f316534d83a8a2c3d1674ace8a5a71198eba31e2e2b597833f699b28"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn",
+ "critical-section",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
@@ -110,17 +98,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "axum"
-version = "0.6.4"
+version = "0.6.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5694b64066a2459918d8074c2ce0d5a88f409431994c2356617c8ae0c4721fc"
+checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
 dependencies = [
  "async-trait",
  "axum-core",
  "bitflags",
  "bytes",
  "futures-util",
  "http",
@@ -132,24 +120,23 @@
  "mime",
  "percent-encoding",
  "pin-project-lite",
  "rustversion",
  "serde",
  "sync_wrapper",
  "tower",
- "tower-http",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
 name = "axum-core"
-version = "0.3.2"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cae3e661676ffbacb30f1a824089a8c9150e71017f7e1e38f2aa32009188d34"
+checksum = "759fa577a247914fd3f7f76d62972792636412fbfd634cd452f6a385a74d2d2c"
 dependencies = [
  "async-trait",
  "bytes",
  "futures-util",
  "http",
  "http-body",
  "mime",
@@ -164,76 +151,88 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
- "miniz_oxide",
+ "miniz_oxide 0.6.2",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
+name = "base64"
+version = "0.21.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
+
+[[package]]
 name = "bincode"
-version = "2.0.0-rc.2"
+version = "2.0.0-rc.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7bb50c5a2ef4b9b1e7ae73e3a73b52ea24b20312d629f9c4df28260b7ad2c3c4"
+checksum = "f11ea1a0346b94ef188834a65c068a03aec181c94896d481d7a0a40d85b0ce95"
 dependencies = [
  "bincode_derive",
  "serde",
 ]
 
 [[package]]
 name = "bincode_derive"
-version = "2.0.0-rc.2"
+version = "2.0.0-rc.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a45a23389446d2dd25dc8e73a7a3b3c43522b630cac068927f0649d43d719d2"
+checksum = "7e30759b3b99a1b802a7a3aa21c85c3ded5c28e1c83170d82d70f08bbf7f3e4c"
 dependencies = [
  "virtue",
 ]
 
 [[package]]
+name = "bit_field"
+version = "0.10.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc827186963e592360843fb5ba4b973e145841266c1357f7180c43526f2e5b61"
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
- "digest 0.10.6",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "boringtun"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "51d23af4567b268583ccc30a983a0f937fb5fc05e71e9de96012a72ad10d1a45"
 dependencies = [
  "aead",
- "base64",
+ "base64 0.13.1",
  "blake2",
  "chacha20poly1305",
  "hex",
  "hmac",
  "ip_network",
  "ip_network_table",
  "libc",
@@ -244,17 +243,23 @@
  "tracing",
  "untrusted 0.9.0",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
+name = "bytemuck"
+version = "1.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -280,17 +285,17 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chacha20"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7fc89c7c5b9e7a02dfe45cd2367bae382f9ed31c61ca8debe5f827c420a2f08"
+checksum = "c3613f74bd2eac03dad61bd53dbe620703d4371614fe0bc3b9f04dd36fe4e818"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
@@ -304,55 +309,55 @@
  "cipher",
  "poly1305",
  "zeroize",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
- "half",
+ "half 1.8.2",
 ]
 
 [[package]]
 name = "cipher"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1873270f8f7942c191139cb8a40fd228da6c3fd2fc376d7e92d47aa14aeb59e"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
  "crypto-common",
  "inout",
  "zeroize",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "bitflags",
  "clap_lex",
  "indexmap",
  "textwrap",
 ]
 
@@ -362,30 +367,36 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
+name = "color_quant"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
+
+[[package]]
 name = "console-api"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e57ff02e8ad8e06ab9731d5dc72dc23bef9200778eae1a89d555d8c42e5d4a86"
+checksum = "c2895653b4d9f1538a83970077cb01dfc77a4810524e51a110944688e916b18e"
 dependencies = [
  "prost",
  "prost-types",
  "tonic",
  "tracing-core",
 ]
 
 [[package]]
 name = "console-subscriber"
-version = "0.1.8"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22a3a81dfaf6b66bce5d159eddae701e3a002f194d378cbf7be5f053c281d9be"
+checksum = "57ab2224a0311582eb03adba4caaf18644f7b1f10a760803a803b9b605187fc7"
 dependencies = [
  "console-api",
  "crossbeam-channel",
  "crossbeam-utils",
  "futures",
  "hdrhistogram",
  "humantime",
@@ -399,17 +410,17 @@
  "tracing",
  "tracing-core",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -452,57 +463,69 @@
 checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
+name = "critical-section"
+version = "1.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6548a0ad5d2549e111e1f6a11a6c2e2d00ce6a3dafe22948d67c2b443f775e52"
+
+[[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset 0.9.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "rand_core 0.6.4",
@@ -520,32 +543,64 @@
  "rand_core 0.5.1",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.3.3"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
+
+[[package]]
+name = "defmt"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
+checksum = "956673bd3cb347512bf988d1e8d89ac9a82b64f6eec54d3c01c3529dac019882"
+dependencies = [
+ "bitflags",
+ "defmt-macros",
+]
+
+[[package]]
+name = "defmt-macros"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4abc4821bd84d3d8f49945ddb24d029be9385ed9b77c99bf2f6296847a6a9f0"
+dependencies = [
+ "defmt-parser",
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "defmt-parser"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "269924c02afd7f94bc4cecbfa5c379f6ffcf9766b3408fe63d22c728654eccd0"
+dependencies = [
+ "thiserror",
+]
 
 [[package]]
 name = "digest"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
@@ -565,21 +620,21 @@
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -594,105 +649,143 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "827292ea592108849932ad8e30218f8b1f21c0dfd0696698a18b5d0aed62d990"
 dependencies = [
  "arrayvec",
 ]
 
 [[package]]
+name = "exr"
+version = "1.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "279d3efcc55e19917fff7ab3ddd6c14afb6a90881a0078465196fe2f99d08c56"
+dependencies = [
+ "bit_field",
+ "flume",
+ "half 2.2.1",
+ "lebe",
+ "miniz_oxide 0.7.1",
+ "rayon-core",
+ "smallvec",
+ "zune-inflate",
+]
+
+[[package]]
+name = "fdeflate"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+dependencies = [
+ "simd-adler32",
+]
+
+[[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
- "miniz_oxide",
+ "miniz_oxide 0.7.1",
+]
+
+[[package]]
+name = "flume"
+version = "0.10.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+ "nanorand",
+ "pin-project",
+ "spin 0.9.8",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "futures"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e2792b0ff0340399d58445b88fd9770e3489eff258a4cbc1523418f12abf84"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e5317663a9089767a1ec00a487df42e0ca174b61b4483213ac24448e4664df5"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec90ff4d0fe1f57d600049061dc6bb68ed03c7d2fbd697274c41805dcb3f8608"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8de0a35a6ab97ec8869e32a2473f4b1324459e14c29275d14b10cb1fd19b50e"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfb8371b6fb2aeb2d280374607aeabfc99d95c72edfe51692e42d3d7f0d08531"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95a73af87da33b5acf53acfebdc339fe592ecf5357ac7c0a7734ab9d8c876a70"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f310820bb3e8cfd46c80db4d7fb8353e15dfff853a127158425f31e0be6c8364"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcf79a1bf610b10f42aea489289c5a2c478a786509693b80cd39c44ccd936366"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.26"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c1d6de3acfef38d2be4b1f543f553131788603495be83da675e180c8d6b7bd1"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -700,17 +793,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
@@ -721,34 +814,46 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
+ "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "gif"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
+dependencies = [
+ "color_quant",
+ "weezl",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.27.1"
+version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "221996f774192f0f718773def8201c4ae31f02616a54ccfc2d358bb0e5cefdec"
+checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
 
 [[package]]
 name = "h2"
-version = "0.3.15"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f9f29bc9dda355256b2916cf526ab02ce0aeaaaf2bad60d65ef3f12f11dd0f4"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -762,33 +867,64 @@
 [[package]]
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
+name = "half"
+version = "2.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
+dependencies = [
+ "crunchy",
+]
+
+[[package]]
+name = "hash32"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0c35f58762feb77d74ebe43bdbc3210f09be9fe6742234d573bacc26ed92b67"
+dependencies = [
+ "byteorder",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hdrhistogram"
 version = "7.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f19b9f54f7c7f55e31401bb647626ce0cf0f67b0004982ce815b3ee72a02aa8"
 dependencies = [
- "base64",
+ "base64 0.13.1",
  "byteorder",
  "flate2",
  "nom",
  "num-traits",
 ]
 
 [[package]]
+name = "heapless"
+version = "0.7.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db04bc24a18b9ea980628ecf00e6c0264f3c1426dac36c00cb49b6fbad8b0743"
+dependencies = [
+ "atomic-polyfill",
+ "hash32",
+ "rustc_version",
+ "spin 0.9.8",
+ "stable_deref_trait",
+]
+
+[[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
@@ -800,38 +936,38 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856b5cb0902c2b6d65d5fd97dfa30f9b70c7538e770b98eab5ed52d8db923e01"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
- "digest 0.10.6",
+ "digest 0.10.7",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75f43d41e26995c17e71ee126451dd3941010b0514a81a9d11f3b341debc2399"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
@@ -842,20 +978,14 @@
 dependencies = [
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
-name = "http-range-header"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bfe8eed0a9285ef776bb792479ea3834e8b94e13d615c2f66d03dd50a435a29"
-
-[[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "httpdate"
@@ -867,17 +997,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.24"
+version = "0.14.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e011372fa0b68db8350aa7a248930ecc7839bf46d8485577d69f117a75f164c"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -902,18 +1032,37 @@
  "hyper",
  "pin-project-lite",
  "tokio",
  "tokio-io-timeout",
 ]
 
 [[package]]
+name = "image"
+version = "0.24.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "527909aa81e20ac3a44803521443a765550f09b5130c2c2fa1ea59c2f8f50a3a"
+dependencies = [
+ "bytemuck",
+ "byteorder",
+ "color_quant",
+ "exr",
+ "gif",
+ "jpeg-decoder",
+ "num-rational",
+ "num-traits",
+ "png",
+ "qoi",
+ "tiff",
+]
+
+[[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
@@ -933,21 +1082,30 @@
 [[package]]
 name = "internet-checksum"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc6d6206008e25125b1f97fbe5d309eb7b85141cf9199d52dbd3729a1584dd16"
 
 [[package]]
+name = "internet-packet"
+version = "0.1.0"
+source = "git+https://github.com/mhils/internet-packet.git#9d706e0f6a28da91f63e3417c7bb4c2e977a2385"
+dependencies = [
+ "internet-checksum",
+]
+
+[[package]]
 name = "io-lifetimes"
-version = "1.0.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1abeb7a0dd0f8181267ff8adc397075586500b81b28a73e8a0208b00fc170fb3"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "ip_network"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa2f047c0a98b2f299aa5d6d7088443570faae494e9ae1305e48be000c9e0eb1"
@@ -966,84 +1124,96 @@
 name = "ip_network_table-deps-treebitmap"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e537132deb99c0eb4b752f0346b6a836200eaaa3516dd7e5514b63930a09e5d"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.3"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22e18b0a45d56fe973d6db23972bf5bc46f988a4a2385deac9cc29572f09daef"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
- "hermit-abi 0.3.0",
+ "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+
+[[package]]
+name = "jpeg-decoder"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
+dependencies = [
+ "rayon",
+]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
+name = "lebe"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
+
+[[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "lru_time_cache"
 version = "0.11.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9106e1d747ffd48e6be5bb2d97fa706ed25b144fbee4d5c02eae110cd8d6badd"
 
@@ -1081,26 +1251,35 @@
 checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "memoffset"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a60c7ce501c71e03a9c9c0d35b861413ae925bd979cc7a4e30d060069aaac8d"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
@@ -1110,62 +1289,72 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+ "simd-adler32",
+]
+
+[[package]]
 name = "mio"
-version = "0.8.5"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys 0.42.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "mitm-wg-test-client"
-version = "0.2.0-beta.8"
+version = "0.2.0-beta.9"
 dependencies = [
  "anyhow",
  "boringtun",
  "data-encoding",
  "hex",
  "smoltcp",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy"
-version = "0.2.0-beta.8"
+version = "0.2.0-beta.9"
 dependencies = [
  "anyhow",
  "async-trait",
  "bincode",
  "boringtun",
  "console-subscriber",
  "criterion",
  "env_logger",
+ "image",
  "log",
  "once_cell",
  "pretty-hex",
  "rand",
  "rand_core 0.6.4",
  "smoltcp",
  "tokio",
- "windows 0.44.0",
+ "windows 0.48.0",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy_rs"
-version = "0.2.0-beta.8"
+version = "0.2.0-beta.9"
 dependencies = [
  "anyhow",
  "console-subscriber",
  "data-encoding",
  "env_logger",
  "log",
  "mitmproxy",
@@ -1175,14 +1364,23 @@
  "pyo3-log",
  "rand_core 0.6.4",
  "tokio",
  "x25519-dalek",
 ]
 
 [[package]]
+name = "nanorand"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
+dependencies = [
+ "getrandom 0.2.10",
+]
+
+[[package]]
 name = "nix"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa52e972a9a719cecb6864fb88568781eb706bac2cd1d4f04a648542dbf78069"
 dependencies = [
  "bitflags",
  "cfg-if",
@@ -1197,14 +1395,35 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -1217,26 +1436,26 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.30.3"
+version = "0.30.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea86265d3d3dcb6a27fc51bd29a4bf387fae9d2986b823079d4986af253eb439"
+checksum = "03b4680b86d9cfafba8fc491dc9b6df26b68cf40e9e6cd73909194759a63c385"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
@@ -1244,65 +1463,65 @@
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1338,14 +1557,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9a81d2759aae1dae668f783c308bc5c8ebd191ff4184aaa1b37f65a6ae5a56f"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "png"
+version = "0.17.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "59871cc5b6cce7eaccca5a802b4173377a1c2ba90654246789a8fa2334426d11"
+dependencies = [
+ "bitflags",
+ "crc32fast",
+ "fdeflate",
+ "flate2",
+ "miniz_oxide 0.7.1",
+]
+
+[[package]]
 name = "poly1305"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8159bd90725d2df49889a078b54f4f79e87f1f8a8444194cdca81d38f5393abf"
 dependencies = [
  "cpufeatures",
  "opaque-debug",
@@ -1361,145 +1593,177 @@
 [[package]]
 name = "pretty-hex"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa0831dd7cc608c38a5e323422a0077678fa5744aa2be4ad91c4ece8eec8d5"
 
 [[package]]
+name = "proc-macro-error"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
+dependencies = [
+ "proc-macro-error-attr",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "version_check",
+]
+
+[[package]]
+name = "proc-macro-error-attr"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "version_check",
+]
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
-version = "0.11.6"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21dc42e00223fc37204bd4aa177e69420c604ca4a183209a8f9de30c6d934698"
+checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.11.6"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bda8c0881ea9f722eb9629376db3d0b903b462477c1aafcb0566610ac28ac5d"
+checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
  "itertools",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "prost-types"
-version = "0.11.6"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5e0526209433e96d83d750dd81a99118edbc55739e7e61a46764fd2ad537788"
+checksum = "213622a1460818959ac1181aaeb2dc9c7f63df720db7d788b3e24eacd1983e13"
 dependencies = [
- "bytes",
  "prost",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
-version = "0.17.0"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1febe3946b26194628f00526929ee6f8559f9e807f811257e94d4c456103be0e"
+checksum = "d3564762e37035cfc486228e10b0528460fa026d681b5763873c693aa0d5c260"
 dependencies = [
  "futures",
  "once_cell",
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9c8b57fe71fb5dcf38970ebedc2b1531cf1c14b1b9b4c560a182a57e115575c"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "qoi"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
+dependencies = [
+ "bytemuck",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1532,120 +1796,135 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.2"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "356a0625f1954f730c0201cdab48611198dc6ce21f4acff55089b5a78e6e835b"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "ring"
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
  "cc",
  "libc",
  "once_cell",
- "spin",
+ "spin 0.5.2",
  "untrusted 0.7.1",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+
+[[package]]
+name = "rustc_version"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
 
 [[package]]
 name = "rustix"
-version = "0.36.8"
+version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f43abb88211988493c1abb44a70efa56ff0ce98f233b7b276146f1f3f7ba9644"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5583e89e108996506031660fe09baa5011b9dd0341b89029313006d1fb508d70"
+checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1655,38 +1934,44 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "semver"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+
+[[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.92"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7434af0dc1cbd59268aa98b4c22c131c0584d2232f6fb166efb993e2832e896a"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1695,106 +1980,119 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
-name = "signal-hook-registry"
-version = "1.4.0"
+name = "simd-adler32"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
-dependencies = [
- "libc",
-]
+checksum = "238abfbb77c1915110ad968465608b68e869e0772622c9656714e73e5a1a522f"
 
 [[package]]
 name = "slab"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4614a76b2a8be0058caa9dbbaf66d988527d86d003c11a94fbd335d7661edcef"
+checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "smoltcp"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee34c1e1bfc7e9206cc0fb8030a90129b4e319ab53856249bb27642cab914fb3"
+version = "0.9.1"
+source = "git+https://github.com/mhils/smoltcp?rev=f65351adfa92db5193f368368cb668bac721fe43#f65351adfa92db5193f368368cb668bac721fe43"
 dependencies = [
  "bitflags",
  "byteorder",
+ "cfg-if",
+ "defmt",
+ "heapless",
  "libc",
  "log",
  "managed",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e2d2db9033d13a1567121ddd7a095ee144db4e1ca1b1bda3419bc0da294ebd"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
 
 [[package]]
+name = "spin"
+version = "0.9.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
+dependencies = [
+ "lock_api",
+]
+
+[[package]]
+name = "stable_deref_trait"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
+
+[[package]]
 name = "subtle"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "sync_wrapper"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
-
-[[package]]
-name = "synstructure"
-version = "0.12.6"
+name = "syn"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
- "unicode-xid",
+ "unicode-ident",
 ]
 
 [[package]]
+name = "sync_wrapper"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
+
+[[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
@@ -1805,107 +2103,118 @@
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.4"
+version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
+checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
+ "cfg-if",
  "once_cell",
 ]
 
 [[package]]
+name = "tiff"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7449334f9ff2baf290d55d73983a7d6fa15e01198faef72af07e2a8db851e471"
+dependencies = [
+ "flate2",
+ "jpeg-decoder",
+ "weezl",
+]
+
+[[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.24.2"
-source = "git+https://github.com/mhils/tokio?branch=readmode-fix#c582f04c614b3433b461936715edaed2774ecb7c"
+version = "1.28.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
- "parking_lot",
  "pin-project-lite",
- "signal-hook-registry",
  "socket2",
  "tokio-macros",
  "tracing",
- "windows-sys 0.42.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "tokio-io-timeout"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30b74022ada614a1b4834de765f9bb43877f910cc8ce4be40e89042c9223a8bf"
 dependencies = [
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
-source = "git+https://github.com/mhils/tokio?branch=readmode-fix#c582f04c614b3433b461936715edaed2774ecb7c"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.11"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d660770404473ccd7bc9f8b28494a811bc18542b915c0855c51e8f419d5223ce"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.4"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bb2e075f03b3d66d8d8785356224ba688d2906a371015e225beeb65ca92c740"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -1918,42 +2227,38 @@
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tonic"
-version = "0.8.3"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f219fad3b929bef19b1f86fbc0358d35daed8f2cac972037ac0dc10bbb8d5fb"
+checksum = "3082666a3a6433f7f511c7192923fa1fe07c69332d3c6a2e6bb040b569199d5a"
 dependencies = [
- "async-stream",
  "async-trait",
  "axum",
- "base64",
+ "base64 0.21.2",
  "bytes",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "hyper",
  "hyper-timeout",
  "percent-encoding",
  "pin-project",
  "prost",
- "prost-derive",
  "tokio",
  "tokio-stream",
- "tokio-util",
  "tower",
  "tower-layer",
  "tower-service",
  "tracing",
- "tracing-futures",
 ]
 
 [[package]]
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
@@ -1969,33 +2274,14 @@
  "tokio-util",
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
-name = "tower-http"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f873044bf02dd1e8239e9c1293ea39dad76dc594ec16185d0a1bf31d8dc8d858"
-dependencies = [
- "bitflags",
- "bytes",
- "futures-core",
- "futures-util",
- "http",
- "http-body",
- "http-range-header",
- "pin-project-lite",
- "tower",
- "tower-layer",
- "tower-service",
-]
-
-[[package]]
 name = "tower-layer"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
 
 [[package]]
 name = "tower-service"
@@ -2006,56 +2292,45 @@
 [[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
- "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
-name = "tracing-futures"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97d095ae15e245a057c8e8451bab9b3ee1e1f68e9ba2b4fbc18d0ac5237835f2"
-dependencies = [
- "pin-project",
- "tracing",
-]
-
-[[package]]
 name = "tracing-subscriber"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6176eae26dd70d0c919749377897b54a9276bd7061339665dd68777926b5a70"
+checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
 dependencies = [
  "matchers",
  "once_cell",
  "regex",
  "sharded-slab",
  "thread_local",
  "tracing",
@@ -2072,35 +2347,29 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
-
-[[package]]
-name = "unicode-xid"
-version = "0.2.4"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "universal-hash"
-version = "0.5.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d3160b73c9a19f7e2939a2fdad446c57c1bbbbf4d919d3213ff1267a580d8b5"
+checksum = "fc1de2c688dc15305988b563c3854064043356019f97a4b46276fe734c4f07ea"
 dependencies = [
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "untrusted"
@@ -2124,26 +2393,25 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "virtue"
-version = "0.0.8"
+version = "0.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b60dcd6a64dd45abf9bd426970c9843726da7fc08f44cd6fcebf68c21220a63"
+checksum = "9dcc60c0624df774c82a0ef104151231d37da4962957d691c011c852b2473314"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2163,77 +2431,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "weezl"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2258,156 +2532,183 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windivert"
-version = "0.5.4"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e15e12a11dfb3c18d1afbeea69102549902aceaa44aa4e650fea77ff3aea99d1"
+checksum = "697021beae81b1bc48ff5492bdb93bd38475bc27b587b2589334dff674775df0"
 dependencies = [
  "etherparse",
  "thiserror",
  "windivert-sys",
  "windows 0.43.0",
 ]
 
 [[package]]
 name = "windivert-sys"
-version = "0.9.0"
+version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac9cda38470fc786107d6133f2ce9c1a9b7bb6f0a221b375808bfa6105a601a1"
+checksum = "779ea0aef29d77f02df94ca639ba00ee287b563e2a388ca894e4201797d92366"
 dependencies = [
  "cc",
  "thiserror",
  "windows 0.43.0",
 ]
 
 [[package]]
 name = "windows"
 version = "0.43.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04662ed0e3e5630dfa9b26e4cb823b817f1a9addda855d973a9458c236556244"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows"
-version = "0.44.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e745dab35a0c4c77aa3ce42d595e13d2003d6902d6b08c9ef5fc326d08da12b"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-redirector"
-version = "0.2.0-beta.8"
+version = "0.2.0-beta.9"
 dependencies = [
  "anyhow",
  "bincode",
  "env_logger",
  "hex",
- "internet-checksum",
+ "internet-packet",
  "log",
  "lru_time_cache",
  "mitmproxy",
  "tokio",
  "windivert",
  "winres",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows-targets",
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
-name = "windows-targets"
-version = "0.42.1"
+name = "windows_aarch64_gnullvm"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
-dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
-]
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winres"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b68db261ef59e9e52806f688020631e987592bd83619edccda9c47d42cde4f6c"
 dependencies = [
@@ -2423,25 +2724,33 @@
  "curve25519-dalek",
  "rand_core 0.6.4",
  "zeroize",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
-version = "1.3.3"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44bf07cb3e50ea2003396695d58bf46bc9887a1f362260446fad6bc4e79bd36c"
+checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
- "synstructure",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "zune-inflate"
+version = "0.2.54"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73ab332fe2f6680068f3582b16a24f90ad7096d5d39b974d1c0aff0125116f02"
+dependencies = [
+ "simd-adler32",
 ]
```

### Comparing `mitmproxy_rs-0.2.0b8/PKG-INFO` & `mitmproxy_rs-0.2.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitmproxy_rs
-Version: 0.2.0b8
+Version: 0.2.0b9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

