# Comparing `tmp/winloop-0.0.5.tar.gz` & `tmp/winloop-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winloop-0.0.5.tar", last modified: Sat Jun 10 03:52:42 2023, max compression
+gzip compressed data, was "winloop-0.0.6.tar", last modified: Wed Jun 14 17:08:44 2023, max compression
```

## Comparing `winloop-0.0.5.tar` & `winloop-0.0.6.tar`

### file list

```diff
@@ -1,111 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:42.396910 winloop-0.0.5/
--rw-rw-rw-   0        0        0    11478 2023-06-09 20:31:23.000000 winloop-0.0.5/LICENSE-APACHE
--rw-rw-rw-   0        0        0     1124 2023-06-05 05:12:27.000000 winloop-0.0.5/LICENSE-MIT
--rw-rw-rw-   0        0        0      182 2023-06-10 02:27:36.000000 winloop-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     9013 2023-06-10 03:52:42.394461 winloop-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-06-10 03:43:07.000000 winloop-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 03:52:42.396910 winloop-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3055 2023-06-10 03:52:29.000000 winloop-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:36.991726 winloop-0.0.5/winloop/
--rw-rw-rw-   0        0        0     1591 2023-05-19 19:29:29.000000 winloop-0.0.5/winloop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:37.908890 winloop-0.0.5/winloop/__pycache__/
--rw-rw-rw-   0        0        0     1875 2023-05-27 19:27:48.000000 winloop-0.0.5/winloop/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      319 2023-05-27 19:27:49.000000 winloop-0.0.5/winloop/__pycache__/_noop.cpython-39.pyc
--rw-rw-rw-   0        0        0    16935 2023-06-06 00:54:24.000000 winloop-0.0.5/winloop/__pycache__/_testbase.cpython-39.pyc
--rw-rw-rw-   0        0        0       88 2023-05-18 18:45:23.000000 winloop-0.0.5/winloop/_noop.py
--rw-rw-rw-   0        0        0    15429 2023-06-06 00:54:18.000000 winloop-0.0.5/winloop/_testbase.py
--rw-rw-rw-   0        0        0      789 2023-05-19 02:16:25.000000 winloop-0.0.5/winloop/cbhandles.pxd
--rw-rw-rw-   0        0        0    12547 2023-05-16 20:27:16.000000 winloop-0.0.5/winloop/cbhandles.pyx
--rw-rw-rw-   0        0        0    15105 2023-05-19 19:33:41.000000 winloop-0.0.5/winloop/dns.pyx
--rw-rw-rw-   0        0        0     3258 2023-06-01 16:31:49.000000 winloop-0.0.5/winloop/errors.pyx
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:39.386612 winloop-0.0.5/winloop/handles/
--rw-rw-rw-   0        0        0      252 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/async_.pxd
--rw-rw-rw-   0        0        0     1500 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/async_.pyx
--rw-rw-rw-   0        0        0     1357 2023-05-16 23:36:49.000000 winloop-0.0.5/winloop/handles/basetransport.pxd
--rw-rw-rw-   0        0        0     9553 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/basetransport.pyx
--rw-rw-rw-   0        0        0      276 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/check.pxd
--rw-rw-rw-   0        0        0     1865 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/check.pyx
--rw-rw-rw-   0        0        0      326 2023-05-18 18:40:06.000000 winloop-0.0.5/winloop/handles/fsevent.pxd
--rw-rw-rw-   0        0        0     2842 2023-05-18 18:40:01.000000 winloop-0.0.5/winloop/handles/fsevent.pyx
--rw-rw-rw-   0        0        0     1189 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/handle.pxd
--rw-rw-rw-   0        0        0    13219 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/handle.pyx
--rw-rw-rw-   0        0        0      274 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/idle.pxd
--rw-rw-rw-   0        0        0     1843 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/idle.pyx
--rw-rw-rw-   0        0        0      999 2023-05-18 18:51:45.000000 winloop-0.0.5/winloop/handles/pipe.pxd
--rw-rw-rw-   0        0        0     7026 2023-06-01 21:07:42.000000 winloop-0.0.5/winloop/handles/pipe.pyx
--rw-rw-rw-   0        0        0      566 2023-05-17 19:12:56.000000 winloop-0.0.5/winloop/handles/poll.pxd
--rw-rw-rw-   0        0        0     6800 2023-05-27 20:29:03.000000 winloop-0.0.5/winloop/handles/poll.pyx
--rw-rw-rw-   0        0        0     2467 2023-05-31 02:16:54.000000 winloop-0.0.5/winloop/handles/process.pxd
--rw-rw-rw-   0        0        0    28304 2023-06-03 00:49:50.000000 winloop-0.0.5/winloop/handles/process.pyx
--rw-rw-rw-   0        0        0     1535 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/stream.pxd
--rw-rw-rw-   0        0        0    33531 2023-06-03 18:06:42.000000 winloop-0.0.5/winloop/handles/stream.pyx
--rw-rw-rw-   0        0        0      786 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/streamserver.pxd
--rw-rw-rw-   0        0        0     4650 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/handles/streamserver.pyx
--rw-rw-rw-   0        0        0     1038 2023-05-19 19:34:25.000000 winloop-0.0.5/winloop/handles/tcp.pxd
--rw-rw-rw-   0        0        0     7500 2023-05-18 18:41:59.000000 winloop-0.0.5/winloop/handles/tcp.pyx
--rw-rw-rw-   0        0        0      488 2023-05-19 02:16:51.000000 winloop-0.0.5/winloop/handles/timer.pxd
--rw-rw-rw-   0        0        0     2487 2023-05-16 20:31:22.000000 winloop-0.0.5/winloop/handles/timer.pyx
--rw-rw-rw-   0        0        0      704 2023-05-18 18:44:00.000000 winloop-0.0.5/winloop/handles/udp.pxd
--rw-rw-rw-   0        0        0    12035 2023-05-10 19:07:46.000000 winloop-0.0.5/winloop/handles/udp.pyx
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:40.282753 winloop-0.0.5/winloop/includes/
--rw-rw-rw-   0        0        0      361 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/includes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:40.397035 winloop-0.0.5/winloop/includes/__pycache__/
--rw-rw-rw-   0        0        0      553 2023-05-16 20:45:56.000000 winloop-0.0.5/winloop/includes/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      819 2023-05-27 18:58:15.000000 winloop-0.0.5/winloop/includes/_python.pxd
--rw-rw-rw-   0        0        0   194983 2023-05-17 00:04:22.000000 winloop-0.0.5/winloop/includes/_stdlib.html
--rw-rw-rw-   0        0        0     6963 2023-06-04 22:27:27.000000 winloop-0.0.5/winloop/includes/_stdlib.pxi
--rw-rw-rw-   0        0        0    21967 2023-05-17 00:04:22.000000 winloop-0.0.5/winloop/includes/consts.html
--rw-rw-rw-   0        0        0      687 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/includes/consts.pxi
--rw-rw-rw-   0        0        0      717 2023-05-21 02:39:56.000000 winloop-0.0.5/winloop/includes/context.h
--rw-rw-rw-   0        0        0       51 2023-05-19 02:33:37.000000 winloop-0.0.5/winloop/includes/debug.h
--rw-rw-rw-   0        0        0       63 2023-05-16 20:46:46.000000 winloop-0.0.5/winloop/includes/debug.pxd
--rw-rw-rw-   0        0        0      459 2023-05-16 23:34:31.000000 winloop-0.0.5/winloop/includes/flowcontrol.pxd
--rw-rw-rw-   0        0        0      425 2023-06-02 01:05:27.000000 winloop-0.0.5/winloop/includes/nfork_handler.h
--rw-rw-rw-   0        0        0     7013 2023-06-02 02:09:18.000000 winloop-0.0.5/winloop/includes/socketpair.h
--rw-rw-rw-   0        0        0     3002 2023-06-02 01:53:51.000000 winloop-0.0.5/winloop/includes/system.pxd
--rw-rw-rw-   0        0        0      670 2023-06-03 00:25:11.000000 winloop-0.0.5/winloop/includes/tcp.h
--rw-rw-rw-   0        0        0    18436 2023-06-03 18:23:26.000000 winloop-0.0.5/winloop/includes/uv.pxd
--rw-rw-rw-   0        0        0  7297948 2023-06-09 20:16:02.000000 winloop-0.0.5/winloop/loop.c
--rw-rw-rw-   0        0        0  1158656 2023-06-09 20:56:18.000000 winloop-0.0.5/winloop/loop.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0     6431 2023-06-05 17:57:17.000000 winloop-0.0.5/winloop/loop.pxd
--rw-rw-rw-   0        0        0    10449 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/loop.pyi
--rw-rw-rw-   0        0        0   121804 2023-06-05 00:13:20.000000 winloop-0.0.5/winloop/loop.pyx
--rw-rw-rw-   0        0        0     2423 2023-05-18 18:55:24.000000 winloop-0.0.5/winloop/lru.pyx
--rw-rw-rw-   0        0        0     5383 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/pseudosock.pyx
--rw-rw-rw-   0        0        0      145 2023-05-18 18:43:09.000000 winloop-0.0.5/winloop/request.pxd
--rw-rw-rw-   0        0        0     2415 2023-05-18 18:43:19.000000 winloop-0.0.5/winloop/request.pyx
--rw-rw-rw-   0        0        0      394 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/server.pxd
--rw-rw-rw-   0        0        0     3623 2023-01-15 16:27:26.000000 winloop-0.0.5/winloop/server.pyx
--rw-rw-rw-   0        0        0     3534 2023-05-16 23:33:29.000000 winloop-0.0.5/winloop/sslproto.pxd
--rw-rw-rw-   0        0        0    35914 2023-05-16 23:33:44.000000 winloop-0.0.5/winloop/sslproto.pyx
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:40.554200 winloop-0.0.5/winloop/vendor/
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:40.570093 winloop-0.0.5/winloop/vendor/include/
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:41.652795 winloop-0.0.5/winloop/vendor/include/uv/
--rw-rw-rw-   0        0        0     1615 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/aix.h
--rw-rw-rw-   0        0        0     1641 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/bsd.h
--rw-rw-rw-   0        0        0     3213 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/darwin.h
--rw-rw-rw-   0        0        0    10643 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/errno.h
--rw-rw-rw-   0        0        0     1781 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/linux.h
--rw-rw-rw-   0        0        0     1553 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/os390.h
--rw-rw-rw-   0        0        0     1606 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/posix.h
--rw-rw-rw-   0        0        0     7728 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/stdint-msvc2008.h
--rw-rw-rw-   0        0        0     1985 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/sunos.h
--rw-rw-rw-   0        0        0     1497 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/threadpool.h
--rw-rw-rw-   0        0        0    52889 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/tree.h
--rw-rw-rw-   0        0        0    19504 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/unix.h
--rw-rw-rw-   0        0        0     1831 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/version.h
--rw-rw-rw-   0        0        0    33252 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv/win.h
--rw-rw-rw-   0        0        0    67239 2022-07-12 16:16:33.000000 winloop-0.0.5/winloop/vendor/include/uv.h
--rw-rw-rw-   0        0        0   728242 2023-02-28 22:32:41.000000 winloop-0.0.5/winloop/vendor/uv_a.lib
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:42.389495 winloop-0.0.5/winloop/winloop.egg-info/
--rw-rw-rw-   0        0        0     9013 2023-06-10 03:25:16.000000 winloop-0.0.5/winloop/winloop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2538 2023-06-10 03:25:16.000000 winloop-0.0.5/winloop/winloop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 03:25:16.000000 winloop-0.0.5/winloop/winloop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 03:25:16.000000 winloop-0.0.5/winloop/winloop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 03:25:16.000000 winloop-0.0.5/winloop/winloop.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 03:52:37.662499 winloop-0.0.5/winloop.egg-info/
--rw-rw-rw-   0        0        0     9013 2023-06-10 03:52:35.000000 winloop-0.0.5/winloop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2707 2023-06-10 03:52:35.000000 winloop-0.0.5/winloop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 03:52:35.000000 winloop-0.0.5/winloop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 03:52:35.000000 winloop-0.0.5/winloop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 03:52:35.000000 winloop-0.0.5/winloop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:44.819769 winloop-0.0.6/
+-rw-rw-rw-   0        0        0    11478 2023-06-09 20:31:23.000000 winloop-0.0.6/LICENSE-APACHE
+-rw-rw-rw-   0        0        0     1124 2023-06-05 05:12:27.000000 winloop-0.0.6/LICENSE-MIT
+-rw-rw-rw-   0        0        0      182 2023-06-10 02:27:36.000000 winloop-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     9060 2023-06-14 17:08:44.814770 winloop-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-06-10 03:43:07.000000 winloop-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-14 17:08:44.819769 winloop-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3106 2023-06-14 05:32:53.000000 winloop-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:41.331860 winloop-0.0.6/winloop/
+-rw-rw-rw-   0        0        0     1591 2023-05-19 19:29:29.000000 winloop-0.0.6/winloop/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-05-18 18:45:23.000000 winloop-0.0.6/winloop/_noop.py
+-rw-rw-rw-   0        0        0      789 2023-05-19 02:16:25.000000 winloop-0.0.6/winloop/cbhandles.pxd
+-rw-rw-rw-   0        0        0    12547 2023-05-16 20:27:16.000000 winloop-0.0.6/winloop/cbhandles.pyx
+-rw-rw-rw-   0        0        0    15141 2023-06-13 18:46:07.000000 winloop-0.0.6/winloop/dns.pyx
+-rw-rw-rw-   0        0        0     3267 2023-06-13 18:46:40.000000 winloop-0.0.6/winloop/errors.pyx
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:42.159357 winloop-0.0.6/winloop/handles/
+-rw-rw-rw-   0        0        0      252 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/handles/async_.pxd
+-rw-rw-rw-   0        0        0     1509 2023-06-13 18:47:15.000000 winloop-0.0.6/winloop/handles/async_.pyx
+-rw-rw-rw-   0        0        0     1366 2023-06-13 18:48:09.000000 winloop-0.0.6/winloop/handles/basetransport.pxd
+-rw-rw-rw-   0        0        0     9571 2023-06-13 18:48:49.000000 winloop-0.0.6/winloop/handles/basetransport.pyx
+-rw-rw-rw-   0        0        0      276 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/handles/check.pxd
+-rw-rw-rw-   0        0        0     1874 2023-06-13 18:49:22.000000 winloop-0.0.6/winloop/handles/check.pyx
+-rw-rw-rw-   0        0        0      326 2023-05-18 18:40:06.000000 winloop-0.0.6/winloop/handles/fsevent.pxd
+-rw-rw-rw-   0        0        0     2851 2023-06-13 18:50:42.000000 winloop-0.0.6/winloop/handles/fsevent.pyx
+-rw-rw-rw-   0        0        0     1189 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/handles/handle.pxd
+-rw-rw-rw-   0        0        0    13246 2023-06-13 18:51:44.000000 winloop-0.0.6/winloop/handles/handle.pyx
+-rw-rw-rw-   0        0        0      274 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/handles/idle.pxd
+-rw-rw-rw-   0        0        0     1852 2023-06-13 18:52:12.000000 winloop-0.0.6/winloop/handles/idle.pyx
+-rw-rw-rw-   0        0        0      999 2023-05-18 18:51:45.000000 winloop-0.0.6/winloop/handles/pipe.pxd
+-rw-rw-rw-   0        0        0     7035 2023-06-13 18:52:36.000000 winloop-0.0.6/winloop/handles/pipe.pyx
+-rw-rw-rw-   0        0        0      575 2023-06-13 18:53:09.000000 winloop-0.0.6/winloop/handles/poll.pxd
+-rw-rw-rw-   0        0        0     6818 2023-06-13 18:53:53.000000 winloop-0.0.6/winloop/handles/poll.pyx
+-rw-rw-rw-   0        0        0     2467 2023-05-31 02:16:54.000000 winloop-0.0.6/winloop/handles/process.pxd
+-rw-rw-rw-   0        0        0    28322 2023-06-13 18:54:51.000000 winloop-0.0.6/winloop/handles/process.pyx
+-rw-rw-rw-   0        0        0     1535 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/handles/stream.pxd
+-rw-rw-rw-   0        0        0    33621 2023-06-13 18:58:38.000000 winloop-0.0.6/winloop/handles/stream.pyx
+-rw-rw-rw-   0        0        0      786 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/handles/streamserver.pxd
+-rw-rw-rw-   0        0        0     4659 2023-06-13 18:59:16.000000 winloop-0.0.6/winloop/handles/streamserver.pyx
+-rw-rw-rw-   0        0        0     1038 2023-05-19 19:34:25.000000 winloop-0.0.6/winloop/handles/tcp.pxd
+-rw-rw-rw-   0        0        0     7509 2023-06-13 19:00:13.000000 winloop-0.0.6/winloop/handles/tcp.pyx
+-rw-rw-rw-   0        0        0      488 2023-05-19 02:16:51.000000 winloop-0.0.6/winloop/handles/timer.pxd
+-rw-rw-rw-   0        0        0     2496 2023-06-13 19:00:27.000000 winloop-0.0.6/winloop/handles/timer.pyx
+-rw-rw-rw-   0        0        0      704 2023-05-18 18:44:00.000000 winloop-0.0.6/winloop/handles/udp.pxd
+-rw-rw-rw-   0        0        0    12071 2023-06-13 19:01:40.000000 winloop-0.0.6/winloop/handles/udp.pyx
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:43.099548 winloop-0.0.6/winloop/includes/
+-rw-rw-rw-   0        0        0      361 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/includes/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-05-27 18:58:15.000000 winloop-0.0.6/winloop/includes/_python.pxd
+-rw-rw-rw-   0        0        0     6963 2023-06-04 22:27:27.000000 winloop-0.0.6/winloop/includes/_stdlib.pxi
+-rw-rw-rw-   0        0        0      687 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/includes/consts.pxi
+-rw-rw-rw-   0        0        0      717 2023-05-21 02:39:56.000000 winloop-0.0.6/winloop/includes/context.h
+-rw-rw-rw-   0        0        0       51 2023-05-19 02:33:37.000000 winloop-0.0.6/winloop/includes/debug.h
+-rw-rw-rw-   0        0        0       63 2023-05-16 20:46:46.000000 winloop-0.0.6/winloop/includes/debug.pxd
+-rw-rw-rw-   0        0        0      459 2023-05-16 23:34:31.000000 winloop-0.0.6/winloop/includes/flowcontrol.pxd
+-rw-rw-rw-   0        0        0      425 2023-06-02 01:05:27.000000 winloop-0.0.6/winloop/includes/nfork_handler.h
+-rw-rw-rw-   0        0        0     7013 2023-06-02 02:09:18.000000 winloop-0.0.6/winloop/includes/socketpair.h
+-rw-rw-rw-   0        0        0     3002 2023-06-02 01:53:51.000000 winloop-0.0.6/winloop/includes/system.pxd
+-rw-rw-rw-   0        0        0      670 2023-06-03 00:25:11.000000 winloop-0.0.6/winloop/includes/tcp.h
+-rw-rw-rw-   0        0        0    18436 2023-06-03 18:23:26.000000 winloop-0.0.6/winloop/includes/uv.pxd
+-rw-rw-rw-   0        0        0  7295750 2023-06-13 19:05:53.000000 winloop-0.0.6/winloop/loop.c
+-rw-rw-rw-   0        0        0  1158656 2023-06-13 19:06:34.000000 winloop-0.0.6/winloop/loop.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0     6440 2023-06-13 19:02:18.000000 winloop-0.0.6/winloop/loop.pxd
+-rw-rw-rw-   0        0        0    10449 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/loop.pyi
+-rw-rw-rw-   0        0        0   121813 2023-06-13 19:02:41.000000 winloop-0.0.6/winloop/loop.pyx
+-rw-rw-rw-   0        0        0     2423 2023-05-18 18:55:24.000000 winloop-0.0.6/winloop/lru.pyx
+-rw-rw-rw-   0        0        0     5383 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/pseudosock.pyx
+-rw-rw-rw-   0        0        0      145 2023-05-18 18:43:09.000000 winloop-0.0.6/winloop/request.pxd
+-rw-rw-rw-   0        0        0     2415 2023-05-18 18:43:19.000000 winloop-0.0.6/winloop/request.pyx
+-rw-rw-rw-   0        0        0      394 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/server.pxd
+-rw-rw-rw-   0        0        0     3623 2023-01-15 16:27:26.000000 winloop-0.0.6/winloop/server.pyx
+-rw-rw-rw-   0        0        0     3552 2023-06-13 19:04:37.000000 winloop-0.0.6/winloop/sslproto.pxd
+-rw-rw-rw-   0        0        0    35932 2023-06-13 19:04:19.000000 winloop-0.0.6/winloop/sslproto.pyx
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:43.489556 winloop-0.0.6/winloop/vendor/
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:43.699541 winloop-0.0.6/winloop/vendor/include/
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:44.769816 winloop-0.0.6/winloop/vendor/include/uv/
+-rw-rw-rw-   0        0        0     1615 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/aix.h
+-rw-rw-rw-   0        0        0     1641 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/bsd.h
+-rw-rw-rw-   0        0        0     3213 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/darwin.h
+-rw-rw-rw-   0        0        0    10643 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/errno.h
+-rw-rw-rw-   0        0        0     1781 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/linux.h
+-rw-rw-rw-   0        0        0     1553 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/os390.h
+-rw-rw-rw-   0        0        0     1606 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/posix.h
+-rw-rw-rw-   0        0        0     7728 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/stdint-msvc2008.h
+-rw-rw-rw-   0        0        0     1985 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/sunos.h
+-rw-rw-rw-   0        0        0     1497 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/threadpool.h
+-rw-rw-rw-   0        0        0    52889 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/tree.h
+-rw-rw-rw-   0        0        0    19504 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/unix.h
+-rw-rw-rw-   0        0        0     1831 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/version.h
+-rw-rw-rw-   0        0        0    33252 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv/win.h
+-rw-rw-rw-   0        0        0    67239 2022-07-12 16:16:33.000000 winloop-0.0.6/winloop/vendor/include/uv.h
+-rw-rw-rw-   0        0        0   728242 2023-02-28 22:32:41.000000 winloop-0.0.6/winloop/vendor/uv_a.lib
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:41.447850 winloop-0.0.6/winloop.egg-info/
+-rw-rw-rw-   0        0        0     9060 2023-06-14 17:08:39.000000 winloop-0.0.6/winloop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2250 2023-06-14 17:08:39.000000 winloop-0.0.6/winloop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 17:08:39.000000 winloop-0.0.6/winloop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-14 17:08:39.000000 winloop-0.0.6/winloop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-14 17:08:39.000000 winloop-0.0.6/winloop.egg-info/top_level.txt
```

### Comparing `winloop-0.0.5/LICENSE-APACHE` & `winloop-0.0.6/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/LICENSE-MIT` & `winloop-0.0.6/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/PKG-INFO` & `winloop-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: winloop
-Version: 0.0.5
+Version: 0.0.6
 Summary: An Alternative library for uvloop compatability with windows
+Home-page: https://github.com/vizonex/winloop
 Author: Vizonex
 License: MIT
 Keywords: winloop,libuv,windows,cython,fast-asyncio,uvloop-alternative
 Platform: Microsoft Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `winloop-0.0.5/setup.py` & `winloop-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from Cython.Build import cythonize
 
 
 
 HERE = pathlib.Path("winloop")
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 
 # This is a temporary test Solution and is not the official file yet but this is to display/show what 
 # I'm currently using to compile the winloop library...
 def do_installation():
     try:
@@ -49,14 +49,15 @@
     ]
 
 
     setup(
         name="winloop",
         author="Vizonex",
         version=__version__,
+        url="https://github.com/vizonex/winloop",
         description="""An Alternative library for uvloop compatability with windows""",
         ext_modules=cythonize(ext),
         license="MIT",
         platforms=['Microsoft Windows'],
         keywords=[
             "winloop", 
             "libuv",
```

### Comparing `winloop-0.0.5/winloop/__init__.py` & `winloop-0.0.6/winloop/__init__.py`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/_testbase.py` & `winloop-0.0.6/winloop/handles/udp.pyx`

 * *Files 26% similar despite different names*

```diff
@@ -1,548 +1,404 @@
-"""Test utilities. Don't use outside of the uvloop project."""
+@cython.no_gc_clear
+@cython.freelist(DEFAULT_FREELIST_SIZE)
+cdef class _UDPSendContext:
+    # used to hold additional write request information for uv_write
 
+    cdef:
+        uv.uv_udp_send_t   req
 
-import asyncio
-import asyncio.events
-import collections
-import contextlib
-import gc
-import logging
-import os
-import pprint
-import re
-import select
-import socket
-import ssl
-import tempfile
-import threading
-import time
-import unittest
-import winloop as init 
+        uv.uv_buf_t     uv_buf
+        Py_buffer       py_buf
 
+        UDPTransport    udp
 
-class MockPattern(str):
-    def __eq__(self, other):
-        return bool(re.search(str(self), other, re.S))
+        bint            closed
 
+    cdef close(self):
+        if self.closed:
+            return
 
-class TestCaseDict(collections.UserDict):
-
-    def __init__(self, name):
-        super().__init__()
-        self.name = name
-
-    def __setitem__(self, key, value):
-        if key in self.data:
-            raise RuntimeError('duplicate test {}.{}'.format(
-                self.name, key))
-        super().__setitem__(key, value)
+        self.closed = 1
+        PyBuffer_Release(&self.py_buf)  # void
+        self.req.data = NULL
+        self.uv_buf.base = NULL
+        Py_DECREF(self)
+        self.udp = None
+
+    @staticmethod
+    cdef _UDPSendContext new(UDPTransport udp, object data):
+        cdef _UDPSendContext ctx
+        ctx = _UDPSendContext.__new__(_UDPSendContext)
+        ctx.udp = None
+        ctx.closed = 1
+
+        ctx.req.data = <void*> ctx
+        Py_INCREF(ctx)
+
+        PyObject_GetBuffer(data, &ctx.py_buf, PyBUF_SIMPLE)
+        ctx.uv_buf.base = <char*>ctx.py_buf.buf
+        ctx.uv_buf.len = ctx.py_buf.len
+        ctx.udp = udp
+
+        ctx.closed = 0
+        return ctx
+
+    def __dealloc__(self):
+        if UVLOOP_DEBUG:
+            if not self.closed:
+                raise RuntimeError(
+                    'open _UDPSendContext is being deallocated')
+        self.udp = None
+
+
+@cython.no_gc_clear
+cdef class UDPTransport(UVBaseTransport):
+    def __cinit__(self):
+        self._family = uv.AF_UNSPEC
+        self.__receiving = 0
+        self._address = None
+        self.context = Context_CopyCurrent()
+
+    cdef _init(self, Loop loop, unsigned int family):
+        cdef int err
+
+        self._start_init(loop)
+
+        self._handle = <uv.uv_handle_t*>PyMem_RawMalloc(sizeof(uv.uv_udp_t))
+        if self._handle is NULL:
+            self._abort_init()
+            raise MemoryError()
+
+        err = uv.uv_udp_init_ex(loop.uvloop,
+                                <uv.uv_udp_t*>self._handle,
+                                family)
+        if err < 0:
+            self._abort_init()
+            raise convert_error(err)
+
+        if family in (uv.AF_INET, uv.AF_INET6):
+            self._family = family
+
+        self._finish_init()
+
+    cdef _set_address(self, system.addrinfo *addr):
+        self._address = __convert_sockaddr_to_pyaddr(addr.ai_addr)
+
+    cdef _connect(self, system.sockaddr* addr, size_t addr_len):
+        cdef int err
+        err = uv.uv_udp_connect(<uv.uv_udp_t*>self._handle, addr)
+        if err < 0:
+            exc = convert_error(err)
+            raise exc
+
+    cdef open(self, int family, int sockfd):
+        if family in (uv.AF_INET, uv.AF_INET6, uv.AF_UNIX):
+            self._family = family
+        else:
+            raise ValueError(
+                'cannot open a UDP handle, invalid family {}'.format(family))
 
+        cdef int err
+        err = uv.uv_udp_open(<uv.uv_udp_t*>self._handle,
+                             <uv.uv_os_sock_t>sockfd)
 
-class BaseTestCaseMeta(type):
+        if err < 0:
+            exc = convert_error(err)
+            raise exc
 
-    @classmethod
-    def __prepare__(mcls, name, bases):
-        return TestCaseDict(name)
+    cdef _bind(self, system.sockaddr* addr):
+        cdef:
+            int err
+            int flags = 0
 
-    def __new__(mcls, name, bases, dct):
-        for test_name in dct:
-            if not test_name.startswith('test_'):
-                continue
-            for base in bases:
-                if hasattr(base, test_name):
-                    raise RuntimeError(
-                        'duplicate test {}.{} (also defined in {} '
-                        'parent class)'.format(
-                            name, test_name, base.__name__))
+        self._ensure_alive()
 
-        return super().__new__(mcls, name, bases, dict(dct))
+        err = uv.uv_udp_bind(<uv.uv_udp_t*>self._handle, addr, flags)
+        if err < 0:
+            exc = convert_error(err)
+            raise exc
 
+    cdef _set_broadcast(self, bint on):
+        cdef int err
 
-class BaseTestCase(unittest.TestCase, metaclass=BaseTestCaseMeta):
+        self._ensure_alive()
 
-    def new_loop(self):
-        raise NotImplementedError
+        err = uv.uv_udp_set_broadcast(<uv.uv_udp_t*>self._handle, on)
+        if err < 0:
+            exc = convert_error(err)
+            raise exc
 
-    def new_policy(self):
-        raise NotImplementedError
+    cdef size_t _get_write_buffer_size(self) noexcept:
+        if self._handle is NULL:
+            return 0
+        return (<uv.uv_udp_t*>self._handle).send_queue_size
 
-    def mock_pattern(self, str):
-        return MockPattern(str)
+    cdef bint _is_reading(self) noexcept:
+        return self.__receiving
 
-    async def wait_closed(self, obj):
-        if not isinstance(obj, asyncio.StreamWriter):
-            return
-        try:
-            await obj.wait_closed()
-        except (BrokenPipeError, ConnectionError):
-            pass
-
-    def is_asyncio_loop(self):
-        return type(self.loop).__module__.startswith('asyncio.')
-
-    def run_loop_briefly(self, *, delay=0.01):
-        self.loop.run_until_complete(asyncio.sleep(delay))
-
-    def loop_exception_handler(self, loop:init.Loop, context):
-        # print("default_exception_handler" in dir(loop))
-        self.__unhandled_exceptions.append(context)
-        self.loop.default_exception_handler(context)
-
-    def setUp(self):
-        self.loop = self.new_loop()
-        asyncio.set_event_loop_policy(self.new_policy())
-        asyncio.set_event_loop(self.loop)
-        self._check_unclosed_resources_in_debug = True
-
-        self.loop.set_exception_handler(self.loop_exception_handler)
-        self.__unhandled_exceptions = []
-
-    def tearDown(self):
-        self.loop.close()
-
-        if self.__unhandled_exceptions:
-            print('Unexpected calls to loop.call_exception_handler():')
-            pprint.pprint(self.__unhandled_exceptions)
-            self.fail('unexpected calls to loop.call_exception_handler()')
-            return
+    cdef _start_reading(self):
+        cdef int err
 
-        if not self._check_unclosed_resources_in_debug:
+        if self.__receiving:
             return
 
-        # GC to show any resource warnings as the test completes
-        gc.collect()
-        gc.collect()
-        gc.collect()
-
-        if getattr(self.loop, '_debug_cc', False):
-            gc.collect()
-            gc.collect()
-            gc.collect()
-
-            self.assertEqual(
-                self.loop._debug_uv_handles_total,
-                self.loop._debug_uv_handles_freed,
-                'not all uv_handle_t handles were freed')
-
-            self.assertEqual(
-                self.loop._debug_cb_handles_count, 0,
-                'not all callbacks (call_soon) are GCed')
-
-            self.assertEqual(
-                self.loop._debug_cb_timer_handles_count, 0,
-                'not all timer callbacks (call_later) are GCed')
-
-            self.assertEqual(
-                self.loop._debug_stream_write_ctx_cnt, 0,
-                'not all stream write contexts are GCed')
-
-            for h_name, h_cnt in self.loop._debug_handles_current.items():
-                with self.subTest('Alive handle after test',
-                                  handle_name=h_name):
-                    self.assertEqual(
-                        h_cnt, 0,
-                        'alive {} after test'.format(h_name))
-
-            for h_name, h_cnt in self.loop._debug_handles_total.items():
-                with self.subTest('Total/closed handles',
-                                  handle_name=h_name):
-                    self.assertEqual(
-                        h_cnt, self.loop._debug_handles_closed[h_name],
-                        'total != closed for {}'.format(h_name))
-
-        asyncio.set_event_loop(None)
-        asyncio.set_event_loop_policy(None)
-        self.loop = None
-
-    def skip_unclosed_handles_check(self):
-        self._check_unclosed_resources_in_debug = False
-
-    def tcp_server(self, server_prog, *,
-                   family=socket.AF_INET,
-                   addr=None,
-                   timeout=5,
-                   backlog=1,
-                   max_clients=10):
-
-        if addr is None:
-            if family == socket.AF_UNIX:
-                with tempfile.NamedTemporaryFile() as tmp:
-                    addr = tmp.name
-            else:
-                addr = ('127.0.0.1', 0)
+        self._ensure_alive()
 
-        sock = socket.socket(family, socket.SOCK_STREAM)
-
-        if timeout is None:
-            raise RuntimeError('timeout is required')
-        if timeout <= 0:
-            raise RuntimeError('only blocking sockets are supported')
-        sock.settimeout(timeout)
+        err = uv.uv_udp_recv_start(<uv.uv_udp_t*>self._handle,
+                                   __loop_alloc_buffer,
+                                   __uv_udp_on_receive)
+
+        if err < 0:
+            exc = convert_error(err)
+            self._fatal_error(exc, True)
+            return
+        else:
+            # UDPTransport must live until the read callback is called
+            self.__receiving_started()
 
-        try:
-            sock.bind(addr)
-            sock.listen(backlog)
-        except OSError as ex:
-            sock.close()
-            raise ex
-
-        return TestThreadedServer(
-            self, sock, server_prog, timeout, max_clients)
-
-    def tcp_client(self, client_prog,
-                   family=socket.AF_INET,
-                   timeout=10):
-
-        sock = socket.socket(family, socket.SOCK_STREAM)
-
-        if timeout is None:
-            raise RuntimeError('timeout is required')
-        if timeout <= 0:
-            raise RuntimeError('only blocking sockets are supported')
-        sock.settimeout(timeout)
-
-        return TestThreadedClient(
-            self, sock, client_prog, timeout)
-
-    def unix_server(self, *args, **kwargs):
-        return self.tcp_server(*args, family=socket.AF_UNIX, **kwargs)
-
-    def unix_client(self, *args, **kwargs):
-        return self.tcp_client(*args, family=socket.AF_UNIX, **kwargs)
-
-    @contextlib.contextmanager
-    def unix_sock_name(self):
-        with tempfile.TemporaryDirectory() as td:
-            fn = os.path.join(td, 'sock')
-            try:
-                yield fn
-            finally:
-                try:
-                    os.unlink(fn)
-                except OSError:
-                    pass
+    cdef _stop_reading(self):
+        cdef int err
 
-    def _abort_socket_test(self, ex):
-        try:
-            self.loop.stop()
-        finally:
-            self.fail(ex)
+        if not self.__receiving:
+            return
 
+        self._ensure_alive()
 
-def _cert_fullname(test_file_name, cert_file_name):
-    fullname = os.path.abspath(os.path.join(
-        os.path.dirname(test_file_name), 'certs', cert_file_name))
-    assert os.path.isfile(fullname)
-    return fullname
+        err = uv.uv_udp_recv_stop(<uv.uv_udp_t*>self._handle)
+        if err < 0:
+            exc = convert_error(err)
+            self._fatal_error(exc, True)
+            return
+        else:
+            self.__receiving_stopped()
 
+    cdef inline __receiving_started(self):
+        if self.__receiving:
+            return
+        self.__receiving = 1
+        Py_INCREF(self)
 
-@contextlib.contextmanager
-def silence_long_exec_warning():
+    cdef inline __receiving_stopped(self):
+        if not self.__receiving:
+            return
+        self.__receiving = 0
+        Py_DECREF(self)
 
-    class Filter(logging.Filter):
-        def filter(self, record):
-            return not (record.msg.startswith('Executing') and
-                        record.msg.endswith('seconds'))
+    cdef _new_socket(self):
+        if self._family not in (uv.AF_INET, uv.AF_INET6, uv.AF_UNIX):
+            raise RuntimeError(
+                'UDPTransport.family is undefined; '
+                'cannot create python socket')
+
+        fileno = self._fileno()
+        return PseudoSocket(self._family, uv.SOCK_DGRAM, 0, fileno)
+
+    cdef _send(self, object data, object addr):
+        cdef:
+            _UDPSendContext ctx
+            system.sockaddr_storage saddr_st
+            system.sockaddr *saddr
+            Py_buffer       try_pybuf
+            uv.uv_buf_t     try_uvbuf
 
-    logger = logging.getLogger('asyncio')
-    filter = Filter()
-    logger.addFilter(filter)
-    try:
-        yield
-    finally:
-        logger.removeFilter(filter)
+        self._ensure_alive()
 
+        if self._family not in (uv.AF_INET, uv.AF_INET6, uv.AF_UNIX):
+            raise RuntimeError('UDPTransport.family is undefined; cannot send')
 
-def find_free_port(start_from=50000):
-    for port in range(start_from, start_from + 500):
-        sock = socket.socket()
-        with sock:
+        if addr is None:
+            saddr = NULL
+        else:
             try:
-                sock.bind(('', port))
-            except socket.error:
-                continue
-            else:
-                return port
-    raise RuntimeError('could not find a free port')
-
-
-class SSLTestCase:
-
-    def _create_server_ssl_context(self, certfile, keyfile=None):
-        if hasattr(ssl, 'PROTOCOL_TLS'):
-            sslcontext = ssl.SSLContext(ssl.PROTOCOL_TLS)
+                __convert_pyaddr_to_sockaddr(self._family, addr,
+                                             <system.sockaddr*>&saddr_st)
+            except (ValueError, TypeError):
+                raise
+            except Exception:
+                raise ValueError(
+                    f'{addr!r}: socket family mismatch or '
+                    f'a DNS lookup is required')
+            saddr = <system.sockaddr*>(&saddr_st)
+
+        if self._get_write_buffer_size() == 0:
+            PyObject_GetBuffer(data, &try_pybuf, PyBUF_SIMPLE)
+            try_uvbuf.base = <char*>try_pybuf.buf
+            try_uvbuf.len = try_pybuf.len
+            err = uv.uv_udp_try_send(<uv.uv_udp_t*>self._handle,
+                                     &try_uvbuf,
+                                     1,
+                                     saddr)
+            PyBuffer_Release(&try_pybuf)
         else:
-            sslcontext = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
-        sslcontext.options |= ssl.OP_NO_SSLv2
-        sslcontext.load_cert_chain(certfile, keyfile)
-        return sslcontext
-
-    def _create_client_ssl_context(self, *, disable_verify=True):
-        sslcontext = ssl.create_default_context()
-        sslcontext.check_hostname = False
-        if disable_verify:
-            sslcontext.verify_mode = ssl.CERT_NONE
-        return sslcontext
-
-    @contextlib.contextmanager
-    def _silence_eof_received_warning(self):
-        # TODO This warning has to be fixed in asyncio.
-        logger = logging.getLogger('asyncio')
-        filter = logging.Filter('has no effect when using ssl')
-        logger.addFilter(filter)
-        try:
-            yield
-        finally:
-            logger.removeFilter(filter)
-
-
-class UVTestCase(BaseTestCase):
-
-    implementation = 'init'
-
-    def new_loop(self):
-        return init.new_event_loop()
-
-    def new_policy(self):
-        return init.WinLoopPolicy()
-
-
-class AIOTestCase(BaseTestCase):
-
-    implementation = 'asyncio'
-
-    def setUp(self):
-        super().setUp()
+            err = uv.EAGAIN
 
-        # watcher = asyncio.get_child_watcher()
-        # watcher.attach_loop(self.loop)
-        # asyncio.set_child_watcher(watcher)
+        if err == uv.EAGAIN:
+            ctx = _UDPSendContext.new(self, data)
+            err = uv.uv_udp_send(&ctx.req,
+                                 <uv.uv_udp_t*>self._handle,
+                                 &ctx.uv_buf,
+                                 1,
+                                 saddr,
+                                 __uv_udp_on_send)
 
-    def tearDown(self):
-        # asyncio.set_child_watcher(None)
-        super().tearDown()
-
-    def new_loop(self):
-        return asyncio.new_event_loop()
-
-    def new_policy(self):
-        return asyncio.DefaultEventLoopPolicy()
+            if err < 0:
+                ctx.close()
 
+                exc = convert_error(err)
+                self._fatal_error(exc, True)
+            else:
+                self._maybe_pause_protocol()
 
-def has_IPv6():
-    server_sock = socket.socket(socket.AF_INET6)
-    with server_sock:
-        try:
-            server_sock.bind(('::1', 0))
-        except OSError:
-            return False
         else:
-            return True
-
-
-has_IPv6 = has_IPv6()
-
-
-###############################################################################
-# Socket Testing Utilities
-###############################################################################
-
-
-class TestSocketWrapper:
-
-    def __init__(self, sock):
-        self.__sock = sock
-
-    def recv_all(self, n):
-        buf = b''
-        while len(buf) < n:
-            data = self.recv(n - len(buf))
-            if data == b'':
-                raise ConnectionAbortedError
-            buf += data
-        return buf
-
-    def starttls(self, ssl_context, *,
-                 server_side=False,
-                 server_hostname=None,
-                 do_handshake_on_connect=True):
-
-        assert isinstance(ssl_context, ssl.SSLContext)
-
-        ssl_sock = ssl_context.wrap_socket(
-            self.__sock, server_side=server_side,
-            server_hostname=server_hostname,
-            do_handshake_on_connect=do_handshake_on_connect)
-
-        if server_side:
-            ssl_sock.do_handshake()
-
-        self.__sock.close()
-        self.__sock = ssl_sock
-
-    def __getattr__(self, name):
-        return getattr(self.__sock, name)
-
-    def __repr__(self):
-        return '<{} {!r}>'.format(type(self).__name__, self.__sock)
-
-
-class SocketThread(threading.Thread):
-
-    def stop(self):
-        self._active = False
-        self.join()
+            if err < 0:
+                exc = convert_error(err)
+                self._fatal_error(exc, True)
+            else:
+                self._on_sent(None, self.context.copy())
 
-    def __enter__(self):
-        self.start()
-        return self
+    cdef _on_receive(self, bytes data, object exc, object addr):
+        if exc is None:
+            run_in_context2(
+                self.context, self._protocol.datagram_received, data, addr,
+            )
+        else:
+            run_in_context1(self.context, self._protocol.error_received, exc)
 
-    def __exit__(self, *exc):
-        self.stop()
+    cdef _on_sent(self, object exc, object context=None):
+        if exc is not None:
+            if isinstance(exc, OSError):
+                if context is None:
+                    context = self.context
+                run_in_context1(context, self._protocol.error_received, exc)
+            else:
+                self._fatal_error(
+                    exc, False, 'Fatal write error on datagram transport')
 
+        self._maybe_resume_protocol()
+        if not self._get_write_buffer_size():
+            if self._closing:
+                self._schedule_call_connection_lost(None)
+
+    # === Public API ===
+
+    def sendto(self, data, addr=None):
+        if not data:
+            # Replicating asyncio logic here.
+            return
 
-class TestThreadedClient(SocketThread):
+        if self._address:
+            if addr not in (None, self._address):
+                # Replicating asyncio logic here.
+                raise ValueError(
+                    'Invalid address: must be None or %s' % (self._address,))
+
+            # Instead of setting addr to self._address below like what asyncio
+            # does, we depend on previous uv_udp_connect() to set the address
+            addr = None
+
+        if self._conn_lost:
+            # Replicating asyncio logic here.
+            if self._conn_lost >= LOG_THRESHOLD_FOR_CONNLOST_WRITES:
+                aio_logger.warning('socket.send() raised exception.')
+            self._conn_lost += 1
+            return
 
-    def __init__(self, test, sock, prog, timeout):
-        threading.Thread.__init__(self, None, None, 'test-client')
-        self.daemon = True
+        self._send(data, addr)
 
-        self._timeout = timeout
-        self._sock = sock
-        self._active = True
-        self._prog = prog
-        self._test = test
 
-    def run(self):
+cdef void __uv_udp_on_receive(uv.uv_udp_t* handle,
+                              ssize_t nread,
+                              const uv.uv_buf_t* buf,
+                              const system.sockaddr* addr,
+                              unsigned flags) noexcept with gil:
+
+    if __ensure_handle_data(<uv.uv_handle_t*>handle,
+                            "UDPTransport receive callback") == 0:
+        return
+
+    cdef:
+        UDPTransport udp = <UDPTransport>handle.data
+        Loop loop = udp._loop
+        bytes data
+        object pyaddr
+
+    # It's OK to free the buffer early, since nothing will
+    # be able to touch it until this method is done.
+    __loop_free_buffer(loop)
+
+    if udp._closed:
+        # The handle was closed, there is no reason to
+        # do any work now.
+        udp.__receiving_stopped()  # Just in case.
+        return
+
+    if addr is NULL and nread == 0:
+        # From libuv docs:
+        #      addr: struct sockaddr* containing the address
+        #      of the sender. Can be NULL. Valid for the duration
+        #      of the callback only.
+        #      [...]
+        #      The receive callback will be called with
+        #      nread == 0 and addr == NULL when there is
+        #      nothing to read, and with nread == 0 and
+        #      addr != NULL when an empty UDP packet is
+        #      received.
+        return
+
+    if addr is NULL:
+        pyaddr = None
+    elif addr.sa_family == uv.AF_UNSPEC:
+        # https://github.com/MagicStack/uvloop/issues/304
+        IF UNAME_SYSNAME == "Linux":
+            pyaddr = None
+        ELSE:
+            pyaddr = ''
+    else:
         try:
-            self._prog(TestSocketWrapper(self._sock))
-        except (KeyboardInterrupt, SystemExit):
-            raise
-        except BaseException as ex:
-            self._test._abort_socket_test(ex)
-
-
-class TestThreadedServer(SocketThread):
-
-    def __init__(self, test, sock, prog, timeout, max_clients):
-        threading.Thread.__init__(self, None, None, 'test-server')
-        self.daemon = True
-
-        self._clients = 0
-        self._finished_clients = 0
-        self._max_clients = max_clients
-        self._timeout = timeout
-        self._sock = sock
-        self._active = True
-
-        self._prog = prog
-
-        self._s1, self._s2 = socket.socketpair()
-        self._s1.setblocking(False)
-
-        self._test = test
+            pyaddr = __convert_sockaddr_to_pyaddr(addr)
+        except BaseException as exc:
+            udp._error(exc, False)
+            return
 
-    def stop(self):
-        try:
-            if self._s2 and self._s2.fileno() != -1:
-                try:
-                    self._s2.send(b'stop')
-                except OSError:
-                    pass
-        finally:
-            super().stop()
+    if nread < 0:
+        exc = convert_error(nread)
+        udp._on_receive(None, exc, pyaddr)
+        return
+
+    if nread == 0:
+        data = b''
+    else:
+        data = loop._recv_buffer[:nread]
 
-    def run(self):
-        try:
-            with self._sock:
-                self._sock.setblocking(0)
-                self._run()
-        finally:
-            self._s1.close()
-            self._s2.close()
-
-    def _run(self):
-        while self._active:
-            if self._clients >= self._max_clients:
-                return
-
-            r, w, x = select.select(
-                [self._sock, self._s1], [], [], self._timeout)
-
-            if self._s1 in r:
-                return
-
-            if self._sock in r:
-                try:
-                    conn, addr = self._sock.accept()
-                except BlockingIOError:
-                    continue
-                except socket.timeout:
-                    if not self._active:
-                        return
-                    else:
-                        raise
-                else:
-                    self._clients += 1
-                    conn.settimeout(self._timeout)
-                    try:
-                        with conn:
-                            self._handle_client(conn)
-                    except (KeyboardInterrupt, SystemExit):
-                        raise
-                    except BaseException as ex:
-                        self._active = False
-                        try:
-                            raise
-                        finally:
-                            self._test._abort_socket_test(ex)
-
-    def _handle_client(self, sock):
-        self._prog(TestSocketWrapper(sock))
-
-    @property
-    def addr(self):
-        return self._sock.getsockname()
-
-
-###############################################################################
-# A few helpers from asyncio/tests/testutils.py
-###############################################################################
-
-
-def run_briefly(loop):
-    async def once():
-        pass
-    gen = once()
-    t = loop.create_task(gen)
-    # Don't log a warning if the task is not done after run_until_complete().
-    # It occurs if the loop is stopped or if a task raises a BaseException.
-    t._log_destroy_pending = False
     try:
-        loop.run_until_complete(t)
-    finally:
-        gen.close()
-
-
-def run_until(loop, pred, timeout=30):
-    deadline = time.time() + timeout
-    while not pred():
-        if timeout is not None:
-            timeout = deadline - time.time()
-            if timeout <= 0:
-                raise asyncio.futures.TimeoutError()
-        loop.run_until_complete(asyncio.tasks.sleep(0.001))
-
-
-@contextlib.contextmanager
-def disable_logger():
-    """Context manager to disable asyncio logger.
-
-    For example, it can be used to ignore warnings in debug mode.
-    """
-    old_level = asyncio.log.logger.level
+        udp._on_receive(data, None, pyaddr)
+    except BaseException as exc:
+        udp._error(exc, False)
+
+
+cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) noexcept with gil:
+
+    if req.data is NULL:
+        # Shouldn't happen as:
+        #    - _UDPSendContext does an extra INCREF in its 'init()'
+        #    - _UDPSendContext holds a ref to the relevant UDPTransport
+        aio_logger.error(
+            'UVStream.write callback called with NULL req.data, status=%r',
+            status)
+        return
+
+    cdef:
+        _UDPSendContext ctx = <_UDPSendContext> req.data
+        UDPTransport udp = <UDPTransport>ctx.udp
+
+    ctx.close()
+
+    if status < 0:
+        exc = convert_error(status)
+        print(exc)
+    else:
+        exc = None
+
     try:
-        asyncio.log.logger.setLevel(logging.CRITICAL + 1)
-        yield
-    finally:
-        asyncio.log.logger.setLevel(old_level)
+        udp._on_sent(exc)
+    except BaseException as exc:
+        udp._error(exc, False)
```

### Comparing `winloop-0.0.5/winloop/cbhandles.pxd` & `winloop-0.0.6/winloop/cbhandles.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/cbhandles.pyx` & `winloop-0.0.6/winloop/cbhandles.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/dns.pyx` & `winloop-0.0.6/winloop/dns.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -303,15 +303,15 @@
         self.data = NULL
 
     def __dealloc__(self):
         if self.data is not NULL:
             uv.uv_freeaddrinfo(self.data)  # returns void
             self.data = NULL
 
-    cdef void set_data(self, system.addrinfo *data):
+    cdef void set_data(self, system.addrinfo *data) noexcept:
         self.data = data
 
     cdef unpack(self):
         cdef:
             list result = []
             system.addrinfo *ptr
 
@@ -331,15 +331,15 @@
                 ))
 
             ptr = ptr.ai_next
 
         return result
 
     @staticmethod
-    cdef int isinstance(object other):
+    cdef int isinstance(object other) noexcept:
         return type(other) is AddrInfo
 
 
 cdef class AddrInfoRequest(UVRequest):
     cdef:
         system.addrinfo hints
         object callback
@@ -420,15 +420,15 @@
     try:
         return enum_klass(value)
     except ValueError:
         return value
 
 
 cdef void __on_addrinfo_resolved(uv.uv_getaddrinfo_t *resolver,
-                                 int status, system.addrinfo *res) with gil:
+                                 int status, system.addrinfo *res) noexcept with gil:
 
     if resolver.data is NULL:
         aio_logger.error(
             'AddrInfoRequest callback called with NULL resolver.data')
         return
 
     cdef:
@@ -451,15 +451,15 @@
     finally:
         request.on_done()
 
 
 cdef void __on_nameinfo_resolved(uv.uv_getnameinfo_t* req,
                                  int status,
                                  const char* hostname,
-                                 const char* service) with gil:
+                                 const char* service) noexcept with gil:
     cdef:
         NameInfoRequest request = <NameInfoRequest> req.data
         Loop loop = request.loop
         object callback = request.callback
 
     try:
         if status < 0:
```

### Comparing `winloop-0.0.5/winloop/errors.pyx` & `winloop-0.0.6/winloop/errors.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     elif uverr == uv.ETIMEDOUT:
         exc = TimeoutError
 
     return exc(oserr, __strerr(oserr))
 
 
-cdef int __convert_socket_error(int uverr):
+cdef int __convert_socket_error(int uverr) noexcept:
     cdef int sock_err = 0
 
     if uverr == uv.UV__EAI_ADDRFAMILY:
         sock_err = socket_EAI_ADDRFAMILY
 
     elif uverr == uv.EAI_AGAIN:
         sock_err = socket_EAI_AGAIN
```

### Comparing `winloop-0.0.5/winloop/handles/async_.pyx` & `winloop-0.0.6/winloop/handles/async_.pyx`

 * *Files 15% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     cdef UVAsync new(Loop loop, method_t callback, object ctx):
         cdef UVAsync handle
         handle = UVAsync.__new__(UVAsync)
         handle._init(loop, callback, ctx)
         return handle
 
 
-cdef void __uvasync_callback(uv.uv_async_t* handle) with gil:
+cdef void __uvasync_callback(uv.uv_async_t* handle) noexcept with gil:
     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVAsync callback") == 0:
         return
 
     cdef:
         UVAsync async_ = <UVAsync> handle.data
         method_t cb = async_.callback
     try:
```

### Comparing `winloop-0.0.5/winloop/handles/basetransport.pxd` & `winloop-0.0.6/winloop/handles/basetransport.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 
     cdef inline _init_protocol(self)
     cdef inline _add_extra_info(self, str name, object obj)
 
     # === overloads ===
 
     cdef _new_socket(self)
-    cdef size_t _get_write_buffer_size(self)
+    cdef size_t _get_write_buffer_size(self) noexcept
 
     cdef bint _is_reading(self)
     cdef _start_reading(self)
     cdef _stop_reading(self)
```

### Comparing `winloop-0.0.5/winloop/handles/basetransport.pyx` & `winloop-0.0.6/winloop/handles/basetransport.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self._waiter = None
         self._extra_info = None
 
         self._conn_lost = 0
 
         self._closing = 0
 
-    cdef size_t _get_write_buffer_size(self):
+    cdef size_t _get_write_buffer_size(self) noexcept:
         return 0
 
     cdef inline _schedule_call_connection_made(self):
         self._loop._call_soon_handle(
             new_MethodHandle(self._loop,
                              "UVTransport._call_connection_made",
                              <method_t>self._call_connection_made,
@@ -207,15 +207,15 @@
         self._schedule_call_connection_made()
 
     cdef inline _add_extra_info(self, str name, object obj):
         if self._extra_info is None:
             self._extra_info = {}
         self._extra_info[name] = obj
 
-    cdef bint _is_reading(self):
+    cdef bint _is_reading(self) noexcept:
         raise NotImplementedError
 
     cdef _start_reading(self):
         raise NotImplementedError
 
     cdef _stop_reading(self):
         raise NotImplementedError
```

### Comparing `winloop-0.0.5/winloop/handles/check.pyx` & `winloop-0.0.6/winloop/handles/check.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     cdef UVCheck new(Loop loop, Handle h):
         cdef UVCheck handle
         handle = UVCheck.__new__(UVCheck)
         handle._init(loop, h)
         return handle
 
 
-cdef void cb_check_callback(uv.uv_check_t* handle) with gil:
+cdef void cb_check_callback(uv.uv_check_t* handle) noexcept with gil:
     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVCheck callback") == 0:
         return
 
     cdef:
         UVCheck check = <UVCheck> handle.data
         Handle h = check.h
     try:
```

### Comparing `winloop-0.0.5/winloop/handles/fsevent.pyx` & `winloop-0.0.6/winloop/handles/fsevent.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         cdef UVFSEvent handle
         handle = UVFSEvent.__new__(UVFSEvent)
         handle._init(loop, callback, context)
         return handle
 
 
 cdef void __uvfsevent_callback(uv.uv_fs_event_t* handle, const char *filename,
-                               int events, int status) with gil:
+                               int events, int status) noexcept with gil:
     if __ensure_handle_data(
         <uv.uv_handle_t*>handle, "UVFSEvent callback"
     ) == 0:
         return
 
     cdef:
         UVFSEvent fs_event = <UVFSEvent> handle.data
```

### Comparing `winloop-0.0.5/winloop/handles/handle.pxd` & `winloop-0.0.6/winloop/handles/handle.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/handles/handle.pyx` & `winloop-0.0.6/winloop/handles/handle.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -331,15 +331,15 @@
                 handle_ctx.decode('latin-1'))
         })
         return 0
 
     return 1
 
 
-cdef void __uv_close_handle_cb(uv.uv_handle_t* handle) with gil:
+cdef void __uv_close_handle_cb(uv.uv_handle_t* handle) noexcept with gil:
     cdef UVHandle h
 
     if handle.data is NULL:
         # The original UVHandle is long dead. Just free the mem of
         # the uv_handle_t* handler.
 
         if UVLOOP_DEBUG:
@@ -359,22 +359,22 @@
                 h._loop._debug_handles_closed.update([
                     h.__class__.__name__])
             h._free()
         finally:
             Py_DECREF(h)  # Was INCREFed in UVHandle._close
 
 
-cdef void __close_all_handles(Loop loop):
+cdef void __close_all_handles(Loop loop) noexcept:
     uv.uv_walk(loop.uvloop,
                __uv_walk_close_all_handles_cb,
                <void*>loop)  # void
 
 
 cdef void __uv_walk_close_all_handles_cb(
-        uv.uv_handle_t* handle, void* arg) with gil:
+        uv.uv_handle_t* handle, void* arg) noexcept with gil:
 
     cdef:
         Loop loop = <Loop>arg
         UVHandle h
 
     if uv.uv_is_closing(handle):
         # The handle is closed or is closing.
```

### Comparing `winloop-0.0.5/winloop/handles/idle.pyx` & `winloop-0.0.6/winloop/handles/idle.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     cdef UVIdle new(Loop loop, Handle h):
         cdef UVIdle handle
         handle = UVIdle.__new__(UVIdle)
         handle._init(loop, h)
         return handle
 
 
-cdef void cb_idle_callback(uv.uv_idle_t* handle) with gil:
+cdef void cb_idle_callback(uv.uv_idle_t* handle) noexcept with gil:
     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVIdle callback") == 0:
         return
 
     cdef:
         UVIdle idle = <UVIdle> handle.data
         Handle h = idle.h
     try:
```

### Comparing `winloop-0.0.5/winloop/handles/pipe.pxd` & `winloop-0.0.6/winloop/handles/pipe.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/handles/pipe.pyx` & `winloop-0.0.6/winloop/handles/pipe.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     cdef connect(self, char* addr):
         # uv_pipe_connect returns void
         uv.uv_pipe_connect(<uv.uv_connect_t*>self.request,
                            <uv.uv_pipe_t*>self.transport._handle,
                            addr,
                            __pipe_connect_callback)
 
-cdef void __pipe_connect_callback(uv.uv_connect_t* req, int status) with gil:
+cdef void __pipe_connect_callback(uv.uv_connect_t* req, int status) noexcept with gil:
     cdef:
         _PipeConnectRequest wrapper
         UnixTransport transport
 
     wrapper = <_PipeConnectRequest> req.data
     transport = wrapper.transport
```

### Comparing `winloop-0.0.5/winloop/handles/poll.pyx` & `winloop-0.0.6/winloop/handles/poll.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     @staticmethod
     cdef UVPoll new(Loop loop, int fd):
         cdef UVPoll handle
         handle = UVPoll.__new__(UVPoll)
         handle._init(loop, fd)
         return handle
 
-    cdef int is_active(self):
+    cdef int is_active(self) noexcept:
         return (self.reading_handle is not None or
                 self.writing_handle is not None)
 
     cdef inline _poll_start(self, int flags):
         cdef int err
 
         self._ensure_alive()
@@ -192,15 +192,15 @@
                 self.writing_handle = None
 
         finally:
             self._close()
 
 
 cdef void __on_uvpoll_event(uv.uv_poll_t* handle,
-                            int status, int events) with gil:
+                            int status, int events) noexcept with gil:
 
     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVPoll callback") == 0:
         return
 
     cdef:
         UVPoll poll = <UVPoll> handle.data
```

### Comparing `winloop-0.0.5/winloop/handles/process.pxd` & `winloop-0.0.6/winloop/handles/process.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/handles/process.pyx` & `winloop-0.0.6/winloop/handles/process.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -755,15 +755,15 @@
         raise TypeError(
             '{!r}.fileno() returned non-integer'.format(obj))
     return fileno
 
 
 cdef void __uvprocess_on_exit_callback(uv.uv_process_t *handle,
                                        int64_t exit_status,
-                                       int term_signal) with gil:
+                                       int term_signal) noexcept with gil:
 
     if __ensure_handle_data(<uv.uv_handle_t*>handle,
                             "UVProcess exit callback") == 0:
         return
 
     cdef UVProcess proc = <UVProcess> handle.data
     try:
@@ -795,9 +795,9 @@
 
     os_set_inheritable(fds[0], False)
     os_set_inheritable(fds[1], False)
 
     return fds[0], fds[1]
 
 
-cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) with gil:
+cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) noexcept with gil:
     PyMem_RawFree(handle)
```

### Comparing `winloop-0.0.5/winloop/handles/stream.pxd` & `winloop-0.0.6/winloop/handles/stream.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/handles/stream.pyx` & `winloop-0.0.6/winloop/handles/stream.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,15 @@
             return
 
         self._on_accept()
 
     cdef inline _close_on_read_error(self):
         self.__read_error_close = 1
 
-    cdef bint _is_reading(self):
+    cdef bint _is_reading(self) noexcept:
         return self.__reading
 
     cdef _start_reading(self):
         cdef int err
 
         if self._closing:
             return
@@ -612,15 +612,15 @@
             # print("something failed on line 562")
             exc = convert_error(err)
             self._fatal_error(exc, True)
             return
 
         self._maybe_resume_protocol()
 
-    cdef size_t _get_write_buffer_size(self):
+    cdef size_t _get_write_buffer_size(self) noexcept:
         if self._handle is NULL:
             return 0
         return ((<uv.uv_stream_t*>self._handle).write_queue_size +
                 self._buffer_size)
 
     cdef _close(self):
         try:
@@ -757,15 +757,15 @@
     def resume_reading(self):
         if self._is_reading() or self._closing:
             return
         self._start_reading()
 
 
 cdef void __uv_stream_on_shutdown(uv.uv_shutdown_t* req,
-                                  int status) with gil:
+                                  int status) noexcept with gil:
 
     # callback for uv_shutdown
 
     if req.data is NULL:
         aio_logger.error(
             'UVStream.shutdown callback called with NULL req.data, status=%r',
             status)
@@ -786,15 +786,15 @@
         exc = convert_error(status)
         stream._fatal_error(
             exc, False, "error status in uv_stream_t.shutdown callback")
         return
 
 
 cdef inline bint __uv_stream_on_read_common(UVStream sc, Loop loop,
-                                            ssize_t nread):
+                                            ssize_t nread) noexcept:
     if sc._closed:
         # The stream was closed, there is no reason to
         # do any work now.
         sc.__reading_stopped()  # Just in case.
         return True
 
     if nread == uv.EOF:
@@ -846,15 +846,15 @@
         return True
 
     return False
 
 
 cdef inline void __uv_stream_on_read_impl(uv.uv_stream_t* stream,
                                           ssize_t nread,
-                                          const uv.uv_buf_t* buf):
+                                          const uv.uv_buf_t* buf) noexcept:
     cdef:
         UVStream sc = <UVStream>stream.data
         Loop loop = sc._loop
 
     # It's OK to free the buffer early, since nothing will
     # be able to touch it until this method is done.
     __loop_free_buffer(loop)
@@ -874,15 +874,15 @@
     except BaseException as exc:
         if UVLOOP_DEBUG:
             loop._debug_stream_read_cb_errors_total += 1
 
         sc._fatal_error(exc, False)
 
 
-cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status):
+cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status) noexcept:
     cdef:
         _StreamWriteContext ctx = <_StreamWriteContext> req.data
         UVStream stream = <UVStream>ctx.stream
 
     ctx.close()
 
     if stream._closed:
@@ -907,40 +907,40 @@
             stream._loop._debug_stream_write_cb_errors_total += 1
 
         stream._fatal_error(exc, False)
 
 
 cdef void __uv_stream_on_read(uv.uv_stream_t* stream,
                               ssize_t nread,
-                              const uv.uv_buf_t* buf) with gil:
+                              const uv.uv_buf_t* buf) noexcept with gil:
 
     if __ensure_handle_data(<uv.uv_handle_t*>stream,
                             "UVStream read callback") == 0:
         return
 
     # Don't need try-finally, __uv_stream_on_read_impl is void
     __uv_stream_on_read_impl(stream, nread, buf)
 
 
-cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) with gil:
+cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) noexcept with gil:
 
     if UVLOOP_DEBUG:
         if req.data is NULL:
             aio_logger.error(
                 'UVStream.write callback called with NULL req.data, status=%r',
                 status)
             return
 
     # Don't need try-finally, __uv_stream_on_write_impl is void
     __uv_stream_on_write_impl(req, status)
 
 
 cdef void __uv_stream_buffered_alloc(uv.uv_handle_t* stream,
                                      size_t suggested_size,
-                                     uv.uv_buf_t* uvbuf) with gil:
+                                     uv.uv_buf_t* uvbuf) noexcept with gil:
 
     if __ensure_handle_data(<uv.uv_handle_t*>stream,
                             "UVStream alloc buffer callback") == 0:
         return
 
     cdef:
         UVStream sc = <UVStream>stream.data
@@ -980,15 +980,15 @@
     sc._read_pybuf_acquired = 1
     uvbuf.base = <char*>pybuf.buf
     uvbuf.len = pybuf.len
 
 
 cdef void __uv_stream_buffered_on_read(uv.uv_stream_t* stream,
                                        ssize_t nread,
-                                       const uv.uv_buf_t* buf) with gil:
+                                       const uv.uv_buf_t* buf) noexcept with gil:
 
     if __ensure_handle_data(<uv.uv_handle_t*>stream,
                             "UVStream buffered read callback") == 0:
         return
 
     cdef:
         UVStream sc = <UVStream>stream.data
```

### Comparing `winloop-0.0.5/winloop/handles/streamserver.pxd` & `winloop-0.0.6/winloop/handles/streamserver.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/handles/streamserver.pyx` & `winloop-0.0.6/winloop/handles/streamserver.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     def __on_ssl_connected(self, transport, fut):
         exc = fut.exception()
         if exc is not None:
             transport._force_close(exc)
 
 
 cdef void __uv_streamserver_on_listen(uv.uv_stream_t* handle,
-                                      int status) with gil:
+                                      int status) noexcept with gil:
 
     # callback for uv_listen
 
     if __ensure_handle_data(<uv.uv_handle_t*>handle,
                             "UVStream listen callback") == 0:
         return
```

### Comparing `winloop-0.0.5/winloop/handles/tcp.pxd` & `winloop-0.0.6/winloop/handles/tcp.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/handles/tcp.pyx` & `winloop-0.0.6/winloop/handles/tcp.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                                 __tcp_connect_callback)
         if err < 0:
             exc = convert_error(err)
             self.on_done()
             raise exc
 
 
-cdef void __tcp_connect_callback(uv.uv_connect_t* req, int status) with gil:
+cdef void __tcp_connect_callback(uv.uv_connect_t* req, int status) noexcept with gil:
     cdef:
         _TCPConnectRequest wrapper
         TCPTransport transport
 
     wrapper = <_TCPConnectRequest> req.data
     transport = wrapper.transport
```

### Comparing `winloop-0.0.5/winloop/handles/timer.pyx` & `winloop-0.0.6/winloop/handles/timer.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
         cdef UVTimer handle
         handle = UVTimer.__new__(UVTimer)
         handle._init(loop, callback, ctx, timeout)
         return handle
 
 
-cdef void __uvtimer_callback(uv.uv_timer_t* handle) with gil:
+cdef void __uvtimer_callback(uv.uv_timer_t* handle) noexcept with gil:
     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVTimer callback") == 0:
         return
 
     cdef:
         UVTimer timer = <UVTimer> handle.data
         method_t cb = timer.callback
```

### Comparing `winloop-0.0.5/winloop/handles/udp.pxd` & `winloop-0.0.6/winloop/handles/udp.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/_python.pxd` & `winloop-0.0.6/winloop/includes/_python.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/_stdlib.pxi` & `winloop-0.0.6/winloop/includes/_stdlib.pxi`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/consts.pxi` & `winloop-0.0.6/winloop/includes/consts.pxi`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/context.h` & `winloop-0.0.6/winloop/includes/context.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/socketpair.h` & `winloop-0.0.6/winloop/includes/socketpair.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/system.pxd` & `winloop-0.0.6/winloop/includes/system.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/tcp.h` & `winloop-0.0.6/winloop/includes/tcp.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/includes/uv.pxd` & `winloop-0.0.6/winloop/includes/uv.pxd`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/loop.c` & `winloop-0.0.6/winloop/loop.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "_GNU_SOURCE",
@@ -57,16 +57,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -126,20 +126,16 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -1047,17 +1043,17 @@
   "winloop\\handles/fsevent.pyx",
   "winloop\\handles/udp.pyx",
   "winloop\\lru.pyx",
   "winloop\\request.pyx",
   "winloop\\sslproto.pyx",
   "winloop\\server.pyx",
   "winloop\\includes\\flowcontrol.pxd",
-  "test_package\\lib\\site-packages\\Cython\\Includes\\cpython\\type.pxd",
-  "test_package\\lib\\site-packages\\Cython\\Includes\\cpython\\bool.pxd",
-  "test_package\\lib\\site-packages\\Cython\\Includes\\cpython\\complex.pxd",
+  "type.pxd",
+  "bool.pxd",
+  "complex.pxd",
   "winloop\\includes/_stdlib.pxi",
 };
 /* NoFastGil.proto */
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
@@ -1311,51 +1307,51 @@
   PyObject *context;
 };
 
 /* "winloop/sslproto.pxd":124
  *     # Flow control for writes from APP socket
  * 
  *     cdef _control_app_writing(self, object context=*)             # <<<<<<<<<<<<<<
- *     cdef size_t _get_write_buffer_size(self)
+ *     cdef size_t _get_write_buffer_size(self) noexcept
  *     cdef _set_write_buffer_limits(self, high=*, low=*)
  */
 struct __pyx_opt_args_7winloop_4loop_11SSLProtocol__control_app_writing {
   int __pyx_n;
   PyObject *context;
 };
 
 /* "winloop/sslproto.pxd":126
  *     cdef _control_app_writing(self, object context=*)
- *     cdef size_t _get_write_buffer_size(self)
+ *     cdef size_t _get_write_buffer_size(self) noexcept
  *     cdef _set_write_buffer_limits(self, high=*, low=*)             # <<<<<<<<<<<<<<
  * 
  *     # Flow control for reads to APP socket
  */
 struct __pyx_opt_args_7winloop_4loop_11SSLProtocol__set_write_buffer_limits {
   int __pyx_n;
   PyObject *high;
   PyObject *low;
 };
 
 /* "winloop/sslproto.pxd":136
  * 
  *     cdef _control_ssl_reading(self)
  *     cdef _set_read_buffer_limits(self, high=*, low=*)             # <<<<<<<<<<<<<<
- *     cdef size_t _get_read_buffer_size(self)
+ *     cdef size_t _get_read_buffer_size(self) noexcept
  *     cdef _fatal_error(self, exc, message=*)
  */
 struct __pyx_opt_args_7winloop_4loop_11SSLProtocol__set_read_buffer_limits {
   int __pyx_n;
   PyObject *high;
   PyObject *low;
 };
 
 /* "winloop/sslproto.pxd":138
  *     cdef _set_read_buffer_limits(self, high=*, low=*)
- *     cdef size_t _get_read_buffer_size(self)
+ *     cdef size_t _get_read_buffer_size(self) noexcept
  *     cdef _fatal_error(self, exc, message=*)             # <<<<<<<<<<<<<<
  */
 struct __pyx_opt_args_7winloop_4loop_11SSLProtocol__fatal_error {
   int __pyx_n;
   PyObject *message;
 };
 
@@ -4613,30 +4609,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto
+#define __PYX_HAVE_RT_ImportType_proto
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize {
+   __Pyx_ImportType_CheckSize_Error = 0,
+   __Pyx_ImportType_CheckSize_Warn = 1,
+   __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* PatchInspect.proto */
 static PyObject* __Pyx_patch_inspect(PyObject* module);
 
 /* PatchAsyncIO.proto */
 static PyObject* __Pyx_patch_asyncio(PyObject* module);
@@ -8703,29 +8699,29 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/errors.pyx":65
  * 
  * 
- * cdef int __convert_socket_error(int uverr):             # <<<<<<<<<<<<<<
+ * cdef int __convert_socket_error(int uverr) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int sock_err = 0
  * 
  */
 
 static int __pyx_f_7winloop_4loop___convert_socket_error(int __pyx_v_uverr) {
   int __pyx_v_sock_err;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__convert_socket_error", 0);
 
   /* "winloop/errors.pyx":66
  * 
- * cdef int __convert_socket_error(int uverr):
+ * cdef int __convert_socket_error(int uverr) noexcept:
  *     cdef int sock_err = 0             # <<<<<<<<<<<<<<
  * 
  *     if uverr == uv.UV__EAI_ADDRFAMILY:
  */
   __pyx_v_sock_err = 0;
 
   /* "winloop/errors.pyx":68
@@ -9143,15 +9139,15 @@
  */
   __pyx_r = __pyx_v_sock_err;
   goto __pyx_L0;
 
   /* "winloop/errors.pyx":65
  * 
  * 
- * cdef int __convert_socket_error(int uverr):             # <<<<<<<<<<<<<<
+ * cdef int __convert_socket_error(int uverr) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int sock_err = 0
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -59699,15 +59695,15 @@
 }
 
 /* "winloop/loop.pyx":3333
  * 
  * 
  * cdef void __loop_alloc_buffer(uv.uv_handle_t* uvhandle,             # <<<<<<<<<<<<<<
  *                               size_t suggested_size,
- *                               uv.uv_buf_t* buf) with gil:
+ *                               uv.uv_buf_t* buf) noexcept with gil:
  */
 
 static void __pyx_f_7winloop_4loop___loop_alloc_buffer(uv_handle_t *__pyx_v_uvhandle, CYTHON_UNUSED size_t __pyx_v_suggested_size, uv_buf_t *__pyx_v_buf) {
   struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop = 0;
   PyObject *__pyx_v_exc = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
@@ -59718,15 +59714,15 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__loop_alloc_buffer", 0);
 
   /* "winloop/loop.pyx":3337
- *                               uv.uv_buf_t* buf) with gil:
+ *                               uv.uv_buf_t* buf) noexcept with gil:
  *     cdef:
  *         Loop loop = (<UVHandle>uvhandle.data)._loop             # <<<<<<<<<<<<<<
  * 
  *     if loop._recv_buffer_in_use == 1:
  */
   __pyx_t_1 = ((PyObject *)((struct __pyx_obj_7winloop_4loop_UVHandle *)__pyx_v_uvhandle->data)->_loop);
   __Pyx_INCREF(__pyx_t_1);
@@ -59821,15 +59817,15 @@
   __pyx_v_buf->len = (sizeof(__pyx_v_loop->_recv_buffer));
 
   /* "winloop/loop.pyx":3333
  * 
  * 
  * cdef void __loop_alloc_buffer(uv.uv_handle_t* uvhandle,             # <<<<<<<<<<<<<<
  *                               size_t suggested_size,
- *                               uv.uv_buf_t* buf) with gil:
+ *                               uv.uv_buf_t* buf) noexcept with gil:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_WriteUnraisable("winloop.loop.__loop_alloc_buffer", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
@@ -76236,15 +76232,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/handle.pyx":338
  * 
  * 
- * cdef void __uv_close_handle_cb(uv.uv_handle_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_close_handle_cb(uv.uv_handle_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef UVHandle h
  * 
  */
 
 static void __pyx_f_7winloop_4loop___uv_close_handle_cb(uv_handle_t *__pyx_v_handle) {
   struct __pyx_obj_7winloop_4loop_UVHandle *__pyx_v_h = 0;
   __Pyx_RefNannyDeclarations
@@ -76562,15 +76558,15 @@
     }
   }
   __pyx_L3:;
 
   /* "winloop/handles/handle.pyx":338
  * 
  * 
- * cdef void __uv_close_handle_cb(uv.uv_handle_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_close_handle_cb(uv.uv_handle_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef UVHandle h
  * 
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -76587,49 +76583,49 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "winloop/handles/handle.pyx":366
  * 
  * 
- * cdef void __close_all_handles(Loop loop):             # <<<<<<<<<<<<<<
+ * cdef void __close_all_handles(Loop loop) noexcept:             # <<<<<<<<<<<<<<
  *     uv.uv_walk(loop.uvloop,
  *                __uv_walk_close_all_handles_cb,
  */
 
 static void __pyx_f_7winloop_4loop___close_all_handles(struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__close_all_handles", 0);
 
   /* "winloop/handles/handle.pyx":367
  * 
- * cdef void __close_all_handles(Loop loop):
+ * cdef void __close_all_handles(Loop loop) noexcept:
  *     uv.uv_walk(loop.uvloop,             # <<<<<<<<<<<<<<
  *                __uv_walk_close_all_handles_cb,
  *                <void*>loop)  # void
  */
   uv_walk(__pyx_v_loop->uvloop, __pyx_f_7winloop_4loop___uv_walk_close_all_handles_cb, ((void *)__pyx_v_loop));
 
   /* "winloop/handles/handle.pyx":366
  * 
  * 
- * cdef void __close_all_handles(Loop loop):             # <<<<<<<<<<<<<<
+ * cdef void __close_all_handles(Loop loop) noexcept:             # <<<<<<<<<<<<<<
  *     uv.uv_walk(loop.uvloop,
  *                __uv_walk_close_all_handles_cb,
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 /* "winloop/handles/handle.pyx":372
  * 
  * 
  * cdef void __uv_walk_close_all_handles_cb(             # <<<<<<<<<<<<<<
- *         uv.uv_handle_t* handle, void* arg) with gil:
+ *         uv.uv_handle_t* handle, void* arg) noexcept with gil:
  * 
  */
 
 static void __pyx_f_7winloop_4loop___uv_walk_close_all_handles_cb(uv_handle_t *__pyx_v_handle, void *__pyx_v_arg) {
   struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop = 0;
   struct __pyx_obj_7winloop_4loop_UVHandle *__pyx_v_h = 0;
   __Pyx_RefNannyDeclarations
@@ -76802,15 +76798,15 @@
  */
   }
 
   /* "winloop/handles/handle.pyx":372
  * 
  * 
  * cdef void __uv_walk_close_all_handles_cb(             # <<<<<<<<<<<<<<
- *         uv.uv_handle_t* handle, void* arg) with gil:
+ *         uv.uv_handle_t* handle, void* arg) noexcept with gil:
  * 
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -77313,15 +77309,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/async_.pyx":44
  * 
  * 
- * cdef void __uvasync_callback(uv.uv_async_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uvasync_callback(uv.uv_async_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVAsync callback") == 0:
  *         return
  */
 
 static void __pyx_f_7winloop_4loop___uvasync_callback(uv_async_t *__pyx_v_handle) {
   struct __pyx_obj_7winloop_4loop_UVAsync *__pyx_v_async_ = 0;
   __pyx_t_7winloop_4loop_method_t __pyx_v_cb;
@@ -77351,34 +77347,34 @@
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__uvasync_callback", 0);
 
   /* "winloop/handles/async_.pyx":45
  * 
- * cdef void __uvasync_callback(uv.uv_async_t* handle) with gil:
+ * cdef void __uvasync_callback(uv.uv_async_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVAsync callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVAsync callback")) == 0) != 0);
   if (__pyx_t_1) {
 
     /* "winloop/handles/async_.pyx":46
- * cdef void __uvasync_callback(uv.uv_async_t* handle) with gil:
+ * cdef void __uvasync_callback(uv.uv_async_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVAsync callback") == 0:
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/async_.pyx":45
  * 
- * cdef void __uvasync_callback(uv.uv_async_t* handle) with gil:
+ * cdef void __uvasync_callback(uv.uv_async_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVAsync callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
   /* "winloop/handles/async_.pyx":49
@@ -77550,15 +77546,15 @@
     __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
     __pyx_L9_try_end:;
   }
 
   /* "winloop/handles/async_.pyx":44
  * 
  * 
- * cdef void __uvasync_callback(uv.uv_async_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uvasync_callback(uv.uv_async_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVAsync callback") == 0:
  *         return
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -78261,15 +78257,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/idle.pyx":60
  * 
  * 
- * cdef void cb_idle_callback(uv.uv_idle_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void cb_idle_callback(uv.uv_idle_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVIdle callback") == 0:
  *         return
  */
 
 static void __pyx_f_7winloop_4loop_cb_idle_callback(uv_idle_t *__pyx_v_handle) {
   struct __pyx_obj_7winloop_4loop_UVIdle *__pyx_v_idle = 0;
   struct __pyx_obj_7winloop_4loop_Handle *__pyx_v_h = 0;
@@ -78298,34 +78294,34 @@
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("cb_idle_callback", 0);
 
   /* "winloop/handles/idle.pyx":61
  * 
- * cdef void cb_idle_callback(uv.uv_idle_t* handle) with gil:
+ * cdef void cb_idle_callback(uv.uv_idle_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVIdle callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVIdle callback")) == 0) != 0);
   if (__pyx_t_1) {
 
     /* "winloop/handles/idle.pyx":62
- * cdef void cb_idle_callback(uv.uv_idle_t* handle) with gil:
+ * cdef void cb_idle_callback(uv.uv_idle_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVIdle callback") == 0:
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/idle.pyx":61
  * 
- * cdef void cb_idle_callback(uv.uv_idle_t* handle) with gil:
+ * cdef void cb_idle_callback(uv.uv_idle_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVIdle callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
   /* "winloop/handles/idle.pyx":65
@@ -78495,15 +78491,15 @@
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     __pyx_L9_try_end:;
   }
 
   /* "winloop/handles/idle.pyx":60
  * 
  * 
- * cdef void cb_idle_callback(uv.uv_idle_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void cb_idle_callback(uv.uv_idle_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVIdle callback") == 0:
  *         return
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -79207,15 +79203,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/check.pyx":60
  * 
  * 
- * cdef void cb_check_callback(uv.uv_check_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void cb_check_callback(uv.uv_check_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVCheck callback") == 0:
  *         return
  */
 
 static void __pyx_f_7winloop_4loop_cb_check_callback(uv_check_t *__pyx_v_handle) {
   struct __pyx_obj_7winloop_4loop_UVCheck *__pyx_v_check = 0;
   struct __pyx_obj_7winloop_4loop_Handle *__pyx_v_h = 0;
@@ -79244,34 +79240,34 @@
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("cb_check_callback", 0);
 
   /* "winloop/handles/check.pyx":61
  * 
- * cdef void cb_check_callback(uv.uv_check_t* handle) with gil:
+ * cdef void cb_check_callback(uv.uv_check_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVCheck callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVCheck callback")) == 0) != 0);
   if (__pyx_t_1) {
 
     /* "winloop/handles/check.pyx":62
- * cdef void cb_check_callback(uv.uv_check_t* handle) with gil:
+ * cdef void cb_check_callback(uv.uv_check_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVCheck callback") == 0:
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/check.pyx":61
  * 
- * cdef void cb_check_callback(uv.uv_check_t* handle) with gil:
+ * cdef void cb_check_callback(uv.uv_check_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVCheck callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
   /* "winloop/handles/check.pyx":65
@@ -79441,15 +79437,15 @@
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     __pyx_L9_try_end:;
   }
 
   /* "winloop/handles/check.pyx":60
  * 
  * 
- * cdef void cb_check_callback(uv.uv_check_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void cb_check_callback(uv.uv_check_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVCheck callback") == 0:
  *         return
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -80248,15 +80244,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/timer.pyx":75
  * 
  * 
- * cdef void __uvtimer_callback(uv.uv_timer_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uvtimer_callback(uv.uv_timer_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVTimer callback") == 0:
  *         return
  */
 
 static void __pyx_f_7winloop_4loop___uvtimer_callback(uv_timer_t *__pyx_v_handle) {
   struct __pyx_obj_7winloop_4loop_UVTimer *__pyx_v_timer = 0;
   __pyx_t_7winloop_4loop_method_t __pyx_v_cb;
@@ -80286,34 +80282,34 @@
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__uvtimer_callback", 0);
 
   /* "winloop/handles/timer.pyx":76
  * 
- * cdef void __uvtimer_callback(uv.uv_timer_t* handle) with gil:
+ * cdef void __uvtimer_callback(uv.uv_timer_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVTimer callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVTimer callback")) == 0) != 0);
   if (__pyx_t_1) {
 
     /* "winloop/handles/timer.pyx":77
- * cdef void __uvtimer_callback(uv.uv_timer_t* handle) with gil:
+ * cdef void __uvtimer_callback(uv.uv_timer_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVTimer callback") == 0:
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/timer.pyx":76
  * 
- * cdef void __uvtimer_callback(uv.uv_timer_t* handle) with gil:
+ * cdef void __uvtimer_callback(uv.uv_timer_t* handle) noexcept with gil:
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVTimer callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
   /* "winloop/handles/timer.pyx":80
@@ -80494,15 +80490,15 @@
     __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
     __pyx_L9_try_end:;
   }
 
   /* "winloop/handles/timer.pyx":75
  * 
  * 
- * cdef void __uvtimer_callback(uv.uv_timer_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uvtimer_callback(uv.uv_timer_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVTimer callback") == 0:
  *         return
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -80759,15 +80755,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "winloop/handles/poll.pyx":32
  *         handle = UVPoll.__new__(UVPoll)
  *         handle._init(loop, fd)
  *         return handle             # <<<<<<<<<<<<<<
  * 
- *     cdef int is_active(self):
+ *     cdef int is_active(self) noexcept:
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_handle));
   __pyx_r = __pyx_v_handle;
   goto __pyx_L0;
 
   /* "winloop/handles/poll.pyx":28
@@ -80789,57 +80785,57 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/poll.pyx":34
  *         return handle
  * 
- *     cdef int is_active(self):             # <<<<<<<<<<<<<<
+ *     cdef int is_active(self) noexcept:             # <<<<<<<<<<<<<<
  *         return (self.reading_handle is not None or
  *                 self.writing_handle is not None)
  */
 
 static int __pyx_f_7winloop_4loop_6UVPoll_is_active(struct __pyx_obj_7winloop_4loop_UVPoll *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("is_active", 0);
 
   /* "winloop/handles/poll.pyx":35
  * 
- *     cdef int is_active(self):
+ *     cdef int is_active(self) noexcept:
  *         return (self.reading_handle is not None or             # <<<<<<<<<<<<<<
  *                 self.writing_handle is not None)
  * 
  */
   __pyx_t_2 = (((PyObject *)__pyx_v_self->reading_handle) != Py_None);
   if (!__pyx_t_2) {
   } else {
     __pyx_t_1 = __pyx_t_2;
     goto __pyx_L3_bool_binop_done;
   }
 
   /* "winloop/handles/poll.pyx":36
- *     cdef int is_active(self):
+ *     cdef int is_active(self) noexcept:
  *         return (self.reading_handle is not None or
  *                 self.writing_handle is not None)             # <<<<<<<<<<<<<<
  * 
  *     cdef inline _poll_start(self, int flags):
  */
   __pyx_t_2 = (((PyObject *)__pyx_v_self->writing_handle) != Py_None);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "winloop/handles/poll.pyx":34
  *         return handle
  * 
- *     cdef int is_active(self):             # <<<<<<<<<<<<<<
+ *     cdef int is_active(self) noexcept:             # <<<<<<<<<<<<<<
  *         return (self.reading_handle is not None or
  *                 self.writing_handle is not None)
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -82585,15 +82581,15 @@
   return __pyx_r;
 }
 
 /* "winloop/handles/poll.pyx":198
  * 
  * 
  * cdef void __on_uvpoll_event(uv.uv_poll_t* handle,             # <<<<<<<<<<<<<<
- *                             int status, int events) with gil:
+ *                             int status, int events) noexcept with gil:
  * 
  */
 
 static void __pyx_f_7winloop_4loop___on_uvpoll_event(uv_poll_t *__pyx_v_handle, int __pyx_v_status, int __pyx_v_events) {
   struct __pyx_obj_7winloop_4loop_UVPoll *__pyx_v_poll = 0;
   PyObject *__pyx_v_exc = NULL;
   PyObject *__pyx_v_ex = NULL;
@@ -82624,15 +82620,15 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__on_uvpoll_event", 0);
 
   /* "winloop/handles/poll.pyx":201
- *                             int status, int events) with gil:
+ *                             int status, int events) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVPoll callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVPoll callback")) == 0) != 0);
   if (__pyx_t_1) {
@@ -82643,15 +82639,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/poll.pyx":201
- *                             int status, int events) with gil:
+ *                             int status, int events) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle, "UVPoll callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   }
 
@@ -83230,15 +83226,15 @@
  */
   }
 
   /* "winloop/handles/poll.pyx":198
  * 
  * 
  * cdef void __on_uvpoll_event(uv.uv_poll_t* handle,             # <<<<<<<<<<<<<<
- *                             int status, int events) with gil:
+ *                             int status, int events) noexcept with gil:
  * 
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -83397,15 +83393,15 @@
   __pyx_v_self->_conn_lost = 0;
 
   /* "winloop/handles/basetransport.pyx":19
  *         self._conn_lost = 0
  * 
  *         self._closing = 0             # <<<<<<<<<<<<<<
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  */
   __pyx_v_self->_closing = 0;
 
   /* "winloop/handles/basetransport.pyx":3
  * cdef class UVBaseTransport(UVSocketHandle):
  * 
  *     def __cinit__(self):             # <<<<<<<<<<<<<<
@@ -83418,38 +83414,38 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/basetransport.pyx":21
  *         self._closing = 0
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
 
 static size_t __pyx_f_7winloop_4loop_15UVBaseTransport__get_write_buffer_size(CYTHON_UNUSED struct __pyx_obj_7winloop_4loop_UVBaseTransport *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_get_write_buffer_size", 0);
 
   /* "winloop/handles/basetransport.pyx":22
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     cdef inline _schedule_call_connection_made(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
   /* "winloop/handles/basetransport.pyx":21
  *         self._closing = 0
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -86187,15 +86183,15 @@
   }
 
   /* "winloop/handles/basetransport.pyx":212
  *         if self._extra_info is None:
  *             self._extra_info = {}
  *         self._extra_info[name] = obj             # <<<<<<<<<<<<<<
  * 
- *     cdef bint _is_reading(self):
+ *     cdef bint _is_reading(self) noexcept:
  */
   if (unlikely(__pyx_v_self->_extra_info == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(15, 212, __pyx_L1_error)
   }
   if (unlikely(PyDict_SetItem(__pyx_v_self->_extra_info, __pyx_v_name, __pyx_v_obj) < 0)) __PYX_ERR(15, 212, __pyx_L1_error)
 
@@ -86219,41 +86215,41 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/basetransport.pyx":214
  *         self._extra_info[name] = obj
  * 
- *     cdef bint _is_reading(self):             # <<<<<<<<<<<<<<
+ *     cdef bint _is_reading(self) noexcept:             # <<<<<<<<<<<<<<
  *         raise NotImplementedError
  * 
  */
 
 static int __pyx_f_7winloop_4loop_15UVBaseTransport__is_reading(CYTHON_UNUSED struct __pyx_obj_7winloop_4loop_UVBaseTransport *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_is_reading", 0);
 
   /* "winloop/handles/basetransport.pyx":215
  * 
- *     cdef bint _is_reading(self):
+ *     cdef bint _is_reading(self) noexcept:
  *         raise NotImplementedError             # <<<<<<<<<<<<<<
  * 
  *     cdef _start_reading(self):
  */
   __Pyx_Raise(__pyx_builtin_NotImplementedError, 0, 0, 0);
   __PYX_ERR(15, 215, __pyx_L1_error)
 
   /* "winloop/handles/basetransport.pyx":214
  *         self._extra_info[name] = obj
  * 
- *     cdef bint _is_reading(self):             # <<<<<<<<<<<<<<
+ *     cdef bint _is_reading(self) noexcept:             # <<<<<<<<<<<<<<
  *         raise NotImplementedError
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("winloop.loop.UVBaseTransport._is_reading", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
@@ -90448,15 +90444,15 @@
   __Pyx_RefNannySetupContext("_close_on_read_error", 0);
 
   /* "winloop/handles/stream.pyx":282
  * 
  *     cdef inline _close_on_read_error(self):
  *         self.__read_error_close = 1             # <<<<<<<<<<<<<<
  * 
- *     cdef bint _is_reading(self):
+ *     cdef bint _is_reading(self) noexcept:
  */
   __pyx_v_self->__pyx___read_error_close = 1;
 
   /* "winloop/handles/stream.pyx":281
  *         self._on_accept()
  * 
  *     cdef inline _close_on_read_error(self):             # <<<<<<<<<<<<<<
@@ -90470,38 +90466,38 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/stream.pyx":284
  *         self.__read_error_close = 1
  * 
- *     cdef bint _is_reading(self):             # <<<<<<<<<<<<<<
+ *     cdef bint _is_reading(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self.__reading
  * 
  */
 
 static int __pyx_f_7winloop_4loop_8UVStream__is_reading(struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_is_reading", 0);
 
   /* "winloop/handles/stream.pyx":285
  * 
- *     cdef bint _is_reading(self):
+ *     cdef bint _is_reading(self) noexcept:
  *         return self.__reading             # <<<<<<<<<<<<<<
  * 
  *     cdef _start_reading(self):
  */
   __pyx_r = __pyx_v_self->__pyx___reading;
   goto __pyx_L0;
 
   /* "winloop/handles/stream.pyx":284
  *         self.__read_error_close = 1
  * 
- *     cdef bint _is_reading(self):             # <<<<<<<<<<<<<<
+ *     cdef bint _is_reading(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self.__reading
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -92988,15 +92984,15 @@
   }
 
   /* "winloop/handles/stream.pyx":617
  *             return
  * 
  *         self._maybe_resume_protocol()             # <<<<<<<<<<<<<<
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  */
   __pyx_t_5 = ((struct __pyx_vtabstruct_7winloop_4loop_UVStream *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_base.__pyx_vtab)->__pyx_base._maybe_resume_protocol(((struct __pyx_obj_7winloop_4loop_UVBaseTransport *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(17, 617, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "winloop/handles/stream.pyx":489
  *             self._loop._queue_write(self)
@@ -93028,48 +93024,48 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/stream.pyx":619
  *         self._maybe_resume_protocol()
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         if self._handle is NULL:
  *             return 0
  */
 
 static size_t __pyx_f_7winloop_4loop_8UVStream__get_write_buffer_size(struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("_get_write_buffer_size", 0);
 
   /* "winloop/handles/stream.pyx":620
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         if self._handle is NULL:             # <<<<<<<<<<<<<<
  *             return 0
  *         return ((<uv.uv_stream_t*>self._handle).write_queue_size +
  */
   __pyx_t_1 = ((__pyx_v_self->__pyx_base.__pyx_base.__pyx_base._handle == NULL) != 0);
   if (__pyx_t_1) {
 
     /* "winloop/handles/stream.pyx":621
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         if self._handle is NULL:
  *             return 0             # <<<<<<<<<<<<<<
  *         return ((<uv.uv_stream_t*>self._handle).write_queue_size +
  *                 self._buffer_size)
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
     /* "winloop/handles/stream.pyx":620
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         if self._handle is NULL:             # <<<<<<<<<<<<<<
  *             return 0
  *         return ((<uv.uv_stream_t*>self._handle).write_queue_size +
  */
   }
 
   /* "winloop/handles/stream.pyx":622
@@ -93081,15 +93077,15 @@
  */
   __pyx_r = (((uv_stream_t *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_base._handle)->write_queue_size + __pyx_v_self->_buffer_size);
   goto __pyx_L0;
 
   /* "winloop/handles/stream.pyx":619
  *         self._maybe_resume_protocol()
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         if self._handle is NULL:
  *             return 0
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -95272,15 +95268,15 @@
   return __pyx_r;
 }
 
 /* "winloop/handles/stream.pyx":763
  * 
  * 
  * cdef void __uv_stream_on_shutdown(uv.uv_shutdown_t* req,             # <<<<<<<<<<<<<<
- *                                   int status) with gil:
+ *                                   int status) noexcept with gil:
  * 
  */
 
 static void __pyx_f_7winloop_4loop___uv_stream_on_shutdown(uv_shutdown_t *__pyx_v_req, int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_stream = 0;
   PyObject *__pyx_v_exc = NULL;
   __Pyx_RefNannyDeclarations
@@ -95502,15 +95498,15 @@
  */
   }
 
   /* "winloop/handles/stream.pyx":763
  * 
  * 
  * cdef void __uv_stream_on_shutdown(uv.uv_shutdown_t* req,             # <<<<<<<<<<<<<<
- *                                   int status) with gil:
+ *                                   int status) noexcept with gil:
  * 
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -95529,15 +95525,15 @@
   #endif
 }
 
 /* "winloop/handles/stream.pyx":792
  * 
  * 
  * cdef inline bint __uv_stream_on_read_common(UVStream sc, Loop loop,             # <<<<<<<<<<<<<<
- *                                             ssize_t nread):
+ *                                             ssize_t nread) noexcept:
  *     if sc._closed:
  */
 
 static CYTHON_INLINE int __pyx_f_7winloop_4loop___uv_stream_on_read_common(struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_sc, struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop, Py_ssize_t __pyx_v_nread) {
   PyObject *__pyx_v_ex = NULL;
   PyObject *__pyx_v_exc = NULL;
   int __pyx_r;
@@ -95563,15 +95559,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__uv_stream_on_read_common", 0);
 
   /* "winloop/handles/stream.pyx":794
  * cdef inline bint __uv_stream_on_read_common(UVStream sc, Loop loop,
- *                                             ssize_t nread):
+ *                                             ssize_t nread) noexcept:
  *     if sc._closed:             # <<<<<<<<<<<<<<
  *         # The stream was closed, there is no reason to
  *         # do any work now.
  */
   __pyx_t_1 = (__pyx_v_sc->__pyx_base.__pyx_base.__pyx_base._closed != 0);
   if (__pyx_t_1) {
 
@@ -95594,15 +95590,15 @@
  *     if nread == uv.EOF:
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
     /* "winloop/handles/stream.pyx":794
  * cdef inline bint __uv_stream_on_read_common(UVStream sc, Loop loop,
- *                                             ssize_t nread):
+ *                                             ssize_t nread) noexcept:
  *     if sc._closed:             # <<<<<<<<<<<<<<
  *         # The stream was closed, there is no reason to
  *         # do any work now.
  */
   }
 
   /* "winloop/handles/stream.pyx":800
@@ -96050,15 +96046,15 @@
   __pyx_r = 0;
   goto __pyx_L0;
 
   /* "winloop/handles/stream.pyx":792
  * 
  * 
  * cdef inline bint __uv_stream_on_read_common(UVStream sc, Loop loop,             # <<<<<<<<<<<<<<
- *                                             ssize_t nread):
+ *                                             ssize_t nread) noexcept:
  *     if sc._closed:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7);
@@ -96074,15 +96070,15 @@
 }
 
 /* "winloop/handles/stream.pyx":851
  * 
  * 
  * cdef inline void __uv_stream_on_read_impl(uv.uv_stream_t* stream,             # <<<<<<<<<<<<<<
  *                                           ssize_t nread,
- *                                           const uv.uv_buf_t* buf):
+ *                                           const uv.uv_buf_t* buf) noexcept:
  */
 
 static CYTHON_INLINE void __pyx_f_7winloop_4loop___uv_stream_on_read_impl(uv_stream_t *__pyx_v_stream, Py_ssize_t __pyx_v_nread, CYTHON_UNUSED uv_buf_t const *__pyx_v_buf) {
   struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_sc = 0;
   struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop = 0;
   PyObject *__pyx_v_exc = NULL;
   __Pyx_RefNannyDeclarations
@@ -96105,15 +96101,15 @@
   PyObject *__pyx_t_17 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__uv_stream_on_read_impl", 0);
 
   /* "winloop/handles/stream.pyx":855
- *                                           const uv.uv_buf_t* buf):
+ *                                           const uv.uv_buf_t* buf) noexcept:
  *     cdef:
  *         UVStream sc = <UVStream>stream.data             # <<<<<<<<<<<<<<
  *         Loop loop = sc._loop
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_stream->data);
   __Pyx_INCREF(__pyx_t_1);
@@ -96410,15 +96406,15 @@
   }
 
   /* "winloop/handles/stream.pyx":851
  * 
  * 
  * cdef inline void __uv_stream_on_read_impl(uv.uv_stream_t* stream,             # <<<<<<<<<<<<<<
  *                                           ssize_t nread,
- *                                           const uv.uv_buf_t* buf):
+ *                                           const uv.uv_buf_t* buf) noexcept:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
@@ -96431,15 +96427,15 @@
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_RefNannyFinishContext();
 }
 
 /* "winloop/handles/stream.pyx":881
  * 
  * 
- * cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status):             # <<<<<<<<<<<<<<
+ * cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status) noexcept:             # <<<<<<<<<<<<<<
  *     cdef:
  *         _StreamWriteContext ctx = <_StreamWriteContext> req.data
  */
 
 static CYTHON_INLINE void __pyx_f_7winloop_4loop___uv_stream_on_write_impl(uv_write_t *__pyx_v_req, int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop__StreamWriteContext *__pyx_v_ctx = 0;
   struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_stream = 0;
@@ -96466,15 +96462,15 @@
   PyObject *__pyx_t_19 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__uv_stream_on_write_impl", 0);
 
   /* "winloop/handles/stream.pyx":883
- * cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status):
+ * cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status) noexcept:
  *     cdef:
  *         _StreamWriteContext ctx = <_StreamWriteContext> req.data             # <<<<<<<<<<<<<<
  *         UVStream stream = <UVStream>ctx.stream
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_req->data);
   __Pyx_INCREF(__pyx_t_1);
@@ -96796,15 +96792,15 @@
     __Pyx_ExceptionReset(__pyx_t_5, __pyx_t_6, __pyx_t_7);
     __pyx_L11_try_end:;
   }
 
   /* "winloop/handles/stream.pyx":881
  * 
  * 
- * cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status):             # <<<<<<<<<<<<<<
+ * cdef inline void __uv_stream_on_write_impl(uv.uv_write_t* req, int status) noexcept:             # <<<<<<<<<<<<<<
  *     cdef:
  *         _StreamWriteContext ctx = <_StreamWriteContext> req.data
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -96822,15 +96818,15 @@
 }
 
 /* "winloop/handles/stream.pyx":912
  * 
  * 
  * cdef void __uv_stream_on_read(uv.uv_stream_t* stream,             # <<<<<<<<<<<<<<
  *                               ssize_t nread,
- *                               const uv.uv_buf_t* buf) with gil:
+ *                               const uv.uv_buf_t* buf) noexcept with gil:
  */
 
 static void __pyx_f_7winloop_4loop___uv_stream_on_read(uv_stream_t *__pyx_v_stream, Py_ssize_t __pyx_v_nread, uv_buf_t const *__pyx_v_buf) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
@@ -96843,15 +96839,15 @@
  *                             "UVStream read callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_stream), ((char const *)"UVStream read callback")) == 0) != 0);
 
   /* "winloop/handles/stream.pyx":916
- *                               const uv.uv_buf_t* buf) with gil:
+ *                               const uv.uv_buf_t* buf) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>stream,             # <<<<<<<<<<<<<<
  *                             "UVStream read callback") == 0:
  *         return
  */
   if (__pyx_t_1) {
 
@@ -96861,15 +96857,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     # Don't need try-finally, __uv_stream_on_read_impl is void
  */
     goto __pyx_L0;
 
     /* "winloop/handles/stream.pyx":916
- *                               const uv.uv_buf_t* buf) with gil:
+ *                               const uv.uv_buf_t* buf) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>stream,             # <<<<<<<<<<<<<<
  *                             "UVStream read callback") == 0:
  *         return
  */
   }
 
@@ -96883,29 +96879,29 @@
   __pyx_f_7winloop_4loop___uv_stream_on_read_impl(__pyx_v_stream, __pyx_v_nread, __pyx_v_buf);
 
   /* "winloop/handles/stream.pyx":912
  * 
  * 
  * cdef void __uv_stream_on_read(uv.uv_stream_t* stream,             # <<<<<<<<<<<<<<
  *                               ssize_t nread,
- *                               const uv.uv_buf_t* buf) with gil:
+ *                               const uv.uv_buf_t* buf) noexcept with gil:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "winloop/handles/stream.pyx":924
  * 
  * 
- * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  * 
  *     if UVLOOP_DEBUG:
  */
 
 static void __pyx_f_7winloop_4loop___uv_stream_on_write(uv_write_t *__pyx_v_req, int __pyx_v_status) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -96920,15 +96916,15 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__uv_stream_on_write", 0);
 
   /* "winloop/handles/stream.pyx":926
- * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) with gil:
+ * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) noexcept with gil:
  * 
  *     if UVLOOP_DEBUG:             # <<<<<<<<<<<<<<
  *         if req.data is NULL:
  *             aio_logger.error(
  */
   __pyx_t_1 = (UVLOOP_DEBUG != 0);
   if (__pyx_t_1) {
@@ -97026,15 +97022,15 @@
  *         if req.data is NULL:             # <<<<<<<<<<<<<<
  *             aio_logger.error(
  *                 'UVStream.write callback called with NULL req.data, status=%r',
  */
     }
 
     /* "winloop/handles/stream.pyx":926
- * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) with gil:
+ * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) noexcept with gil:
  * 
  *     if UVLOOP_DEBUG:             # <<<<<<<<<<<<<<
  *         if req.data is NULL:
  *             aio_logger.error(
  */
   }
 
@@ -97046,15 +97042,15 @@
  * 
  */
   __pyx_f_7winloop_4loop___uv_stream_on_write_impl(__pyx_v_req, __pyx_v_status);
 
   /* "winloop/handles/stream.pyx":924
  * 
  * 
- * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_stream_on_write(uv.uv_write_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  * 
  *     if UVLOOP_DEBUG:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -97072,15 +97068,15 @@
 }
 
 /* "winloop/handles/stream.pyx":937
  * 
  * 
  * cdef void __uv_stream_buffered_alloc(uv.uv_handle_t* stream,             # <<<<<<<<<<<<<<
  *                                      size_t suggested_size,
- *                                      uv.uv_buf_t* uvbuf) with gil:
+ *                                      uv.uv_buf_t* uvbuf) noexcept with gil:
  */
 
 static void __pyx_f_7winloop_4loop___uv_stream_buffered_alloc(uv_handle_t *__pyx_v_stream, size_t __pyx_v_suggested_size, uv_buf_t *__pyx_v_uvbuf) {
   struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_sc = 0;
   CYTHON_UNUSED struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop = 0;
   Py_buffer *__pyx_v_pybuf;
   int __pyx_v_got_buf;
@@ -97111,15 +97107,15 @@
  *                             "UVStream alloc buffer callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_stream), ((char const *)"UVStream alloc buffer callback")) == 0) != 0);
 
   /* "winloop/handles/stream.pyx":941
- *                                      uv.uv_buf_t* uvbuf) with gil:
+ *                                      uv.uv_buf_t* uvbuf) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>stream,             # <<<<<<<<<<<<<<
  *                             "UVStream alloc buffer callback") == 0:
  *         return
  */
   if (__pyx_t_1) {
 
@@ -97129,15 +97125,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/stream.pyx":941
- *                                      uv.uv_buf_t* uvbuf) with gil:
+ *                                      uv.uv_buf_t* uvbuf) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>stream,             # <<<<<<<<<<<<<<
  *                             "UVStream alloc buffer callback") == 0:
  *         return
  */
   }
 
@@ -97526,15 +97522,15 @@
   __pyx_v_uvbuf->len = __pyx_t_10;
 
   /* "winloop/handles/stream.pyx":937
  * 
  * 
  * cdef void __uv_stream_buffered_alloc(uv.uv_handle_t* stream,             # <<<<<<<<<<<<<<
  *                                      size_t suggested_size,
- *                                      uv.uv_buf_t* uvbuf) with gil:
+ *                                      uv.uv_buf_t* uvbuf) noexcept with gil:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6);
@@ -97553,15 +97549,15 @@
 }
 
 /* "winloop/handles/stream.pyx":985
  * 
  * 
  * cdef void __uv_stream_buffered_on_read(uv.uv_stream_t* stream,             # <<<<<<<<<<<<<<
  *                                        ssize_t nread,
- *                                        const uv.uv_buf_t* buf) with gil:
+ *                                        const uv.uv_buf_t* buf) noexcept with gil:
  */
 
 static void __pyx_f_7winloop_4loop___uv_stream_buffered_on_read(uv_stream_t *__pyx_v_stream, Py_ssize_t __pyx_v_nread, CYTHON_UNUSED uv_buf_t const *__pyx_v_buf) {
   struct __pyx_obj_7winloop_4loop_UVStream *__pyx_v_sc = 0;
   struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop = 0;
   Py_buffer *__pyx_v_pybuf;
   PyObject *__pyx_v_exc = NULL;
@@ -97599,15 +97595,15 @@
  *                             "UVStream buffered read callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_stream), ((char const *)"UVStream buffered read callback")) == 0) != 0);
 
   /* "winloop/handles/stream.pyx":989
- *                                        const uv.uv_buf_t* buf) with gil:
+ *                                        const uv.uv_buf_t* buf) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>stream,             # <<<<<<<<<<<<<<
  *                             "UVStream buffered read callback") == 0:
  *         return
  */
   if (__pyx_t_1) {
 
@@ -97617,15 +97613,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/stream.pyx":989
- *                                        const uv.uv_buf_t* buf) with gil:
+ *                                        const uv.uv_buf_t* buf) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>stream,             # <<<<<<<<<<<<<<
  *                             "UVStream buffered read callback") == 0:
  *         return
  */
   }
 
@@ -98135,15 +98131,15 @@
   }
 
   /* "winloop/handles/stream.pyx":985
  * 
  * 
  * cdef void __uv_stream_buffered_on_read(uv.uv_stream_t* stream,             # <<<<<<<<<<<<<<
  *                                        ssize_t nread,
- *                                        const uv.uv_buf_t* buf) with gil:
+ *                                        const uv.uv_buf_t* buf) noexcept with gil:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
@@ -99773,15 +99769,15 @@
   return __pyx_r;
 }
 
 /* "winloop/handles/streamserver.pyx":124
  * 
  * 
  * cdef void __uv_streamserver_on_listen(uv.uv_stream_t* handle,             # <<<<<<<<<<<<<<
- *                                       int status) with gil:
+ *                                       int status) noexcept with gil:
  * 
  */
 
 static void __pyx_f_7winloop_4loop___uv_streamserver_on_listen(uv_stream_t *__pyx_v_handle, int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop_UVStreamServer *__pyx_v_stream = 0;
   PyObject *__pyx_v_exc = NULL;
   __Pyx_RefNannyDeclarations
@@ -100090,15 +100086,15 @@
     __pyx_L11_try_end:;
   }
 
   /* "winloop/handles/streamserver.pyx":124
  * 
  * 
  * cdef void __uv_streamserver_on_listen(uv.uv_stream_t* handle,             # <<<<<<<<<<<<<<
- *                                       int status) with gil:
+ *                                       int status) noexcept with gil:
  * 
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -102764,15 +102760,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/tcp.pyx":210
  * 
  * 
- * cdef void __tcp_connect_callback(uv.uv_connect_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __tcp_connect_callback(uv.uv_connect_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         _TCPConnectRequest wrapper
  */
 
 static void __pyx_f_7winloop_4loop___tcp_connect_callback(uv_connect_t *__pyx_v_req, int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop__TCPConnectRequest *__pyx_v_wrapper = 0;
   struct __pyx_obj_7winloop_4loop_TCPTransport *__pyx_v_transport = 0;
@@ -103089,15 +103085,15 @@
     }
     __pyx_L6:;
   }
 
   /* "winloop/handles/tcp.pyx":210
  * 
  * 
- * cdef void __tcp_connect_callback(uv.uv_connect_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __tcp_connect_callback(uv.uv_connect_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         _TCPConnectRequest wrapper
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -105899,15 +105895,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/pipe.pyx":211
  *                            __pipe_connect_callback)
  * 
- * cdef void __pipe_connect_callback(uv.uv_connect_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __pipe_connect_callback(uv.uv_connect_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         _PipeConnectRequest wrapper
  */
 
 static void __pyx_f_7winloop_4loop___pipe_connect_callback(uv_connect_t *__pyx_v_req, int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop__PipeConnectRequest *__pyx_v_wrapper = 0;
   struct __pyx_obj_7winloop_4loop_UnixTransport *__pyx_v_transport = 0;
@@ -106224,15 +106220,15 @@
     }
     __pyx_L6:;
   }
 
   /* "winloop/handles/pipe.pyx":211
  *                            __pipe_connect_callback)
  * 
- * cdef void __pipe_connect_callback(uv.uv_connect_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __pipe_connect_callback(uv.uv_connect_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  *     cdef:
  *         _PipeConnectRequest wrapper
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -117661,15 +117657,15 @@
 }
 
 /* "winloop/handles/process.pyx":760
  * 
  * 
  * cdef void __uvprocess_on_exit_callback(uv.uv_process_t *handle,             # <<<<<<<<<<<<<<
  *                                        int64_t exit_status,
- *                                        int term_signal) with gil:
+ *                                        int term_signal) noexcept with gil:
  */
 
 static void __pyx_f_7winloop_4loop___uvprocess_on_exit_callback(uv_process_t *__pyx_v_handle, int64_t __pyx_v_exit_status, int __pyx_v_term_signal) {
   struct __pyx_obj_7winloop_4loop_UVProcess *__pyx_v_proc = 0;
   PyObject *__pyx_v_ex = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
@@ -117703,15 +117699,15 @@
  *                             "UVProcess exit callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVProcess exit callback")) == 0) != 0);
 
   /* "winloop/handles/process.pyx":764
- *                                        int term_signal) with gil:
+ *                                        int term_signal) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle,             # <<<<<<<<<<<<<<
  *                             "UVProcess exit callback") == 0:
  *         return
  */
   if (__pyx_t_1) {
 
@@ -117721,15 +117717,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef UVProcess proc = <UVProcess> handle.data
  */
     goto __pyx_L0;
 
     /* "winloop/handles/process.pyx":764
- *                                        int term_signal) with gil:
+ *                                        int term_signal) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle,             # <<<<<<<<<<<<<<
  *                             "UVProcess exit callback") == 0:
  *         return
  */
   }
 
@@ -117894,15 +117890,15 @@
   }
 
   /* "winloop/handles/process.pyx":760
  * 
  * 
  * cdef void __uvprocess_on_exit_callback(uv.uv_process_t *handle,             # <<<<<<<<<<<<<<
  *                                        int64_t exit_status,
- *                                        int term_signal) with gil:
+ *                                        int term_signal) noexcept with gil:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7);
@@ -118191,36 +118187,36 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/process.pyx":802
  * 
  * 
- * cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     PyMem_RawFree(handle)
  */
 
 static void __pyx_f_7winloop_4loop___uv_close_process_handle_cb(uv_handle_t *__pyx_v_handle) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__uv_close_process_handle_cb", 0);
 
   /* "winloop/handles/process.pyx":803
  * 
- * cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) with gil:
+ * cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) noexcept with gil:
  *     PyMem_RawFree(handle)             # <<<<<<<<<<<<<<
  */
   PyMem_RawFree(__pyx_v_handle);
 
   /* "winloop/handles/process.pyx":802
  * 
  * 
- * cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_close_process_handle_cb(uv.uv_handle_t* handle) noexcept with gil:             # <<<<<<<<<<<<<<
  *     PyMem_RawFree(handle)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
@@ -119219,15 +119215,15 @@
   return __pyx_r;
 }
 
 /* "winloop/handles/fsevent.pyx":92
  * 
  * 
  * cdef void __uvfsevent_callback(uv.uv_fs_event_t* handle, const char *filename,             # <<<<<<<<<<<<<<
- *                                int events, int status) with gil:
+ *                                int events, int status) noexcept with gil:
  *     if __ensure_handle_data(
  */
 
 static void __pyx_f_7winloop_4loop___uvfsevent_callback(uv_fs_event_t *__pyx_v_handle, char const *__pyx_v_filename, int __pyx_v_events, CYTHON_UNUSED int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop_UVFSEvent *__pyx_v_fs_event = 0;
   struct __pyx_obj_7winloop_4loop_Handle *__pyx_v_h = 0;
   PyObject *__pyx_v_ex = NULL;
@@ -119267,15 +119263,15 @@
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UVFSEvent callback")) == 0) != 0);
 
   /* "winloop/handles/fsevent.pyx":94
  * cdef void __uvfsevent_callback(uv.uv_fs_event_t* handle, const char *filename,
- *                                int events, int status) with gil:
+ *                                int events, int status) noexcept with gil:
  *     if __ensure_handle_data(             # <<<<<<<<<<<<<<
  *         <uv.uv_handle_t*>handle, "UVFSEvent callback"
  *     ) == 0:
  */
   if (__pyx_t_1) {
 
     /* "winloop/handles/fsevent.pyx":97
@@ -119285,15 +119281,15 @@
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/fsevent.pyx":94
  * cdef void __uvfsevent_callback(uv.uv_fs_event_t* handle, const char *filename,
- *                                int events, int status) with gil:
+ *                                int events, int status) noexcept with gil:
  *     if __ensure_handle_data(             # <<<<<<<<<<<<<<
  *         <uv.uv_handle_t*>handle, "UVFSEvent callback"
  *     ) == 0:
  */
   }
 
   /* "winloop/handles/fsevent.pyx":100
@@ -119549,15 +119545,15 @@
     __pyx_L9_try_end:;
   }
 
   /* "winloop/handles/fsevent.pyx":92
  * 
  * 
  * cdef void __uvfsevent_callback(uv.uv_fs_event_t* handle, const char *filename,             # <<<<<<<<<<<<<<
- *                                int events, int status) with gil:
+ *                                int events, int status) noexcept with gil:
  *     if __ensure_handle_data(
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -120894,15 +120890,15 @@
     __pyx_t_1 = 0;
 
     /* "winloop/handles/udp.pyx":128
  *         if err < 0:
  *             exc = convert_error(err)
  *             raise exc             # <<<<<<<<<<<<<<
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  */
     __Pyx_Raise(__pyx_v_exc, 0, 0, 0);
     __PYX_ERR(21, 128, __pyx_L1_error)
 
     /* "winloop/handles/udp.pyx":126
  * 
  *         err = uv.uv_udp_set_broadcast(<uv.uv_udp_t*>self._handle, on)
@@ -120933,105 +120929,105 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/udp.pyx":130
  *             raise exc
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         if self._handle is NULL:
  *             return 0
  */
 
 static size_t __pyx_f_7winloop_4loop_12UDPTransport__get_write_buffer_size(struct __pyx_obj_7winloop_4loop_UDPTransport *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("_get_write_buffer_size", 0);
 
   /* "winloop/handles/udp.pyx":131
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         if self._handle is NULL:             # <<<<<<<<<<<<<<
  *             return 0
  *         return (<uv.uv_udp_t*>self._handle).send_queue_size
  */
   __pyx_t_1 = ((__pyx_v_self->__pyx_base.__pyx_base.__pyx_base._handle == NULL) != 0);
   if (__pyx_t_1) {
 
     /* "winloop/handles/udp.pyx":132
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         if self._handle is NULL:
  *             return 0             # <<<<<<<<<<<<<<
  *         return (<uv.uv_udp_t*>self._handle).send_queue_size
  * 
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
     /* "winloop/handles/udp.pyx":131
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         if self._handle is NULL:             # <<<<<<<<<<<<<<
  *             return 0
  *         return (<uv.uv_udp_t*>self._handle).send_queue_size
  */
   }
 
   /* "winloop/handles/udp.pyx":133
  *         if self._handle is NULL:
  *             return 0
  *         return (<uv.uv_udp_t*>self._handle).send_queue_size             # <<<<<<<<<<<<<<
  * 
- *     cdef bint _is_reading(self):
+ *     cdef bint _is_reading(self) noexcept:
  */
   __pyx_r = ((uv_udp_t *)__pyx_v_self->__pyx_base.__pyx_base.__pyx_base._handle)->send_queue_size;
   goto __pyx_L0;
 
   /* "winloop/handles/udp.pyx":130
  *             raise exc
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         if self._handle is NULL:
  *             return 0
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/handles/udp.pyx":135
  *         return (<uv.uv_udp_t*>self._handle).send_queue_size
  * 
- *     cdef bint _is_reading(self):             # <<<<<<<<<<<<<<
+ *     cdef bint _is_reading(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self.__receiving
  * 
  */
 
 static int __pyx_f_7winloop_4loop_12UDPTransport__is_reading(struct __pyx_obj_7winloop_4loop_UDPTransport *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_is_reading", 0);
 
   /* "winloop/handles/udp.pyx":136
  * 
- *     cdef bint _is_reading(self):
+ *     cdef bint _is_reading(self) noexcept:
  *         return self.__receiving             # <<<<<<<<<<<<<<
  * 
  *     cdef _start_reading(self):
  */
   __pyx_r = __pyx_v_self->__pyx___receiving;
   goto __pyx_L0;
 
   /* "winloop/handles/udp.pyx":135
  *         return (<uv.uv_udp_t*>self._handle).send_queue_size
  * 
- *     cdef bint _is_reading(self):             # <<<<<<<<<<<<<<
+ *     cdef bint _is_reading(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self.__receiving
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -123038,15 +123034,15 @@
  *                             "UDPTransport receive callback") == 0:             # <<<<<<<<<<<<<<
  *         return
  * 
  */
   __pyx_t_1 = ((__pyx_f_7winloop_4loop___ensure_handle_data(((uv_handle_t *)__pyx_v_handle), ((char const *)"UDPTransport receive callback")) == 0) != 0);
 
   /* "winloop/handles/udp.pyx":314
- *                               unsigned flags) with gil:
+ *                               unsigned flags) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle,             # <<<<<<<<<<<<<<
  *                             "UDPTransport receive callback") == 0:
  *         return
  */
   if (__pyx_t_1) {
 
@@ -123056,15 +123052,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/udp.pyx":314
- *                               unsigned flags) with gil:
+ *                               unsigned flags) noexcept with gil:
  * 
  *     if __ensure_handle_data(<uv.uv_handle_t*>handle,             # <<<<<<<<<<<<<<
  *                             "UDPTransport receive callback") == 0:
  *         return
  */
   }
 
@@ -123670,15 +123666,15 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "winloop/handles/udp.pyx":378
  * 
  * 
- * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  * 
  *     if req.data is NULL:
  */
 
 static void __pyx_f_7winloop_4loop___uv_udp_on_send(uv_udp_send_t *__pyx_v_req, int __pyx_v_status) {
   struct __pyx_obj_7winloop_4loop__UDPSendContext *__pyx_v_ctx = 0;
   struct __pyx_obj_7winloop_4loop_UDPTransport *__pyx_v_udp = 0;
@@ -123707,15 +123703,15 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__uv_udp_on_send", 0);
 
   /* "winloop/handles/udp.pyx":380
- * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) with gil:
+ * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) noexcept with gil:
  * 
  *     if req.data is NULL:             # <<<<<<<<<<<<<<
  *         # Shouldn't happen as:
  *         #    - _UDPSendContext does an extra INCREF in its 'init()'
  */
   __pyx_t_1 = ((__pyx_v_req->data == NULL) != 0);
   if (__pyx_t_1) {
@@ -123794,15 +123790,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/handles/udp.pyx":380
- * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) with gil:
+ * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) noexcept with gil:
  * 
  *     if req.data is NULL:             # <<<<<<<<<<<<<<
  *         # Shouldn't happen as:
  *         #    - _UDPSendContext does an extra INCREF in its 'init()'
  */
   }
 
@@ -124045,15 +124041,15 @@
     __Pyx_ExceptionReset(__pyx_t_8, __pyx_t_9, __pyx_t_10);
     __pyx_L10_try_end:;
   }
 
   /* "winloop/handles/udp.pyx":378
  * 
  * 
- * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) with gil:             # <<<<<<<<<<<<<<
+ * cdef void __uv_udp_on_send(uv.uv_udp_send_t* req, int status) noexcept with gil:             # <<<<<<<<<<<<<<
  * 
  *     if req.data is NULL:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -129340,15 +129336,15 @@
     uv_freeaddrinfo(__pyx_v_self->data);
 
     /* "winloop/dns.pyx":308
  *         if self.data is not NULL:
  *             uv.uv_freeaddrinfo(self.data)  # returns void
  *             self.data = NULL             # <<<<<<<<<<<<<<
  * 
- *     cdef void set_data(self, system.addrinfo *data):
+ *     cdef void set_data(self, system.addrinfo *data) noexcept:
  */
     __pyx_v_self->data = NULL;
 
     /* "winloop/dns.pyx":306
  * 
  *     def __dealloc__(self):
  *         if self.data is not NULL:             # <<<<<<<<<<<<<<
@@ -129368,36 +129364,36 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 /* "winloop/dns.pyx":310
  *             self.data = NULL
  * 
- *     cdef void set_data(self, system.addrinfo *data):             # <<<<<<<<<<<<<<
+ *     cdef void set_data(self, system.addrinfo *data) noexcept:             # <<<<<<<<<<<<<<
  *         self.data = data
  * 
  */
 
 static void __pyx_f_7winloop_4loop_8AddrInfo_set_data(struct __pyx_obj_7winloop_4loop_AddrInfo *__pyx_v_self, struct addrinfo *__pyx_v_data) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_data", 0);
 
   /* "winloop/dns.pyx":311
  * 
- *     cdef void set_data(self, system.addrinfo *data):
+ *     cdef void set_data(self, system.addrinfo *data) noexcept:
  *         self.data = data             # <<<<<<<<<<<<<<
  * 
  *     cdef unpack(self):
  */
   __pyx_v_self->data = __pyx_v_data;
 
   /* "winloop/dns.pyx":310
  *             self.data = NULL
  * 
- *     cdef void set_data(self, system.addrinfo *data):             # <<<<<<<<<<<<<<
+ *     cdef void set_data(self, system.addrinfo *data) noexcept:             # <<<<<<<<<<<<<<
  *         self.data = data
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
@@ -129691,40 +129687,40 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/dns.pyx":338
  * 
  *     @staticmethod
- *     cdef int isinstance(object other):             # <<<<<<<<<<<<<<
+ *     cdef int isinstance(object other) noexcept:             # <<<<<<<<<<<<<<
  *         return type(other) is AddrInfo
  * 
  */
 
 static int __pyx_f_7winloop_4loop_8AddrInfo_isinstance(PyObject *__pyx_v_other) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("isinstance", 0);
 
   /* "winloop/dns.pyx":339
  *     @staticmethod
- *     cdef int isinstance(object other):
+ *     cdef int isinstance(object other) noexcept:
  *         return type(other) is AddrInfo             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_1 = (((PyObject *)Py_TYPE(__pyx_v_other)) == ((PyObject *)__pyx_ptype_7winloop_4loop_AddrInfo));
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
   /* "winloop/dns.pyx":338
  * 
  *     @staticmethod
- *     cdef int isinstance(object other):             # <<<<<<<<<<<<<<
+ *     cdef int isinstance(object other) noexcept:             # <<<<<<<<<<<<<<
  *         return type(other) is AddrInfo
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -131054,15 +131050,15 @@
   return __pyx_r;
 }
 
 /* "winloop/dns.pyx":426
  * 
  * 
  * cdef void __on_addrinfo_resolved(uv.uv_getaddrinfo_t *resolver,             # <<<<<<<<<<<<<<
- *                                  int status, system.addrinfo *res) with gil:
+ *                                  int status, system.addrinfo *res) noexcept with gil:
  * 
  */
 
 static void __pyx_f_7winloop_4loop___on_addrinfo_resolved(uv_getaddrinfo_t *__pyx_v_resolver, int __pyx_v_status, struct addrinfo *__pyx_v_res) {
   struct __pyx_obj_7winloop_4loop_AddrInfoRequest *__pyx_v_request = 0;
   struct __pyx_obj_7winloop_4loop_Loop *__pyx_v_loop = 0;
   PyObject *__pyx_v_callback = 0;
@@ -131088,15 +131084,15 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__on_addrinfo_resolved", 0);
 
   /* "winloop/dns.pyx":429
- *                                  int status, system.addrinfo *res) with gil:
+ *                                  int status, system.addrinfo *res) noexcept with gil:
  * 
  *     if resolver.data is NULL:             # <<<<<<<<<<<<<<
  *         aio_logger.error(
  *             'AddrInfoRequest callback called with NULL resolver.data')
  */
   __pyx_t_1 = ((__pyx_v_resolver->data == NULL) != 0);
   if (__pyx_t_1) {
@@ -131133,15 +131129,15 @@
  *         return             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
     goto __pyx_L0;
 
     /* "winloop/dns.pyx":429
- *                                  int status, system.addrinfo *res) with gil:
+ *                                  int status, system.addrinfo *res) noexcept with gil:
  * 
  *     if resolver.data is NULL:             # <<<<<<<<<<<<<<
  *         aio_logger.error(
  *             'AddrInfoRequest callback called with NULL resolver.data')
  */
   }
 
@@ -131481,15 +131477,15 @@
     __pyx_L6:;
   }
 
   /* "winloop/dns.pyx":426
  * 
  * 
  * cdef void __on_addrinfo_resolved(uv.uv_getaddrinfo_t *resolver,             # <<<<<<<<<<<<<<
- *                                  int status, system.addrinfo *res) with gil:
+ *                                  int status, system.addrinfo *res) noexcept with gil:
  * 
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
@@ -131542,15 +131538,15 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("__on_nameinfo_resolved", 0);
 
   /* "winloop/dns.pyx":460
- *                                  const char* service) with gil:
+ *                                  const char* service) noexcept with gil:
  *     cdef:
  *         NameInfoRequest request = <NameInfoRequest> req.data             # <<<<<<<<<<<<<<
  *         Loop loop = request.loop
  *         object callback = request.callback
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_req->data);
   __Pyx_INCREF(__pyx_t_1);
@@ -145104,15 +145100,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/sslproto.pyx":888
  *                 })
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self._outgoing.pending + self._write_buffer_size
  * 
  */
 
 static size_t __pyx_f_7winloop_4loop_11SSLProtocol__get_write_buffer_size(struct __pyx_obj_7winloop_4loop_SSLProtocol *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -145123,15 +145119,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_write_buffer_size", 0);
 
   /* "winloop/sslproto.pyx":889
  * 
- *     cdef size_t _get_write_buffer_size(self):
+ *     cdef size_t _get_write_buffer_size(self) noexcept:
  *         return self._outgoing.pending + self._write_buffer_size             # <<<<<<<<<<<<<<
  * 
  *     cdef _set_write_buffer_limits(self, high=None, low=None):
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_outgoing, __pyx_n_s_pending); if (unlikely(!__pyx_t_1)) __PYX_ERR(24, 889, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_self->_write_buffer_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(24, 889, __pyx_L1_error)
@@ -145144,15 +145140,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   goto __pyx_L0;
 
   /* "winloop/sslproto.pyx":888
  *                 })
  * 
- *     cdef size_t _get_write_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_write_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self._outgoing.pending + self._write_buffer_size
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -145757,15 +145753,15 @@
   __pyx_v_self->_incoming_high_water = __pyx_t_6;
 
   /* "winloop/sslproto.pyx":928
  *             high, low, FLOW_CONTROL_HIGH_WATER_SSL_READ)
  *         self._incoming_high_water = high
  *         self._incoming_low_water = low             # <<<<<<<<<<<<<<
  * 
- *     cdef size_t _get_read_buffer_size(self):
+ *     cdef size_t _get_read_buffer_size(self) noexcept:
  */
   __pyx_t_6 = __Pyx_PyInt_As_size_t(__pyx_v_low); if (unlikely((__pyx_t_6 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(24, 928, __pyx_L1_error)
   __pyx_v_self->_incoming_low_water = __pyx_t_6;
 
   /* "winloop/sslproto.pyx":924
  *             self._transport.resume_reading()
  * 
@@ -145791,15 +145787,15 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "winloop/sslproto.pyx":930
  *         self._incoming_low_water = low
  * 
- *     cdef size_t _get_read_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_read_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self._incoming.pending
  * 
  */
 
 static size_t __pyx_f_7winloop_4loop_11SSLProtocol__get_read_buffer_size(struct __pyx_obj_7winloop_4loop_SSLProtocol *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -145808,30 +145804,30 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_read_buffer_size", 0);
 
   /* "winloop/sslproto.pyx":931
  * 
- *     cdef size_t _get_read_buffer_size(self):
+ *     cdef size_t _get_read_buffer_size(self) noexcept:
  *         return self._incoming.pending             # <<<<<<<<<<<<<<
  * 
  *     # Flow control for writes to SSL socket
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_incoming, __pyx_n_s_pending); if (unlikely(!__pyx_t_1)) __PYX_ERR(24, 931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyInt_As_size_t(__pyx_t_1); if (unlikely((__pyx_t_2 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(24, 931, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
   /* "winloop/sslproto.pyx":930
  *         self._incoming_low_water = low
  * 
- *     cdef size_t _get_read_buffer_size(self):             # <<<<<<<<<<<<<<
+ *     cdef size_t _get_read_buffer_size(self) noexcept:             # <<<<<<<<<<<<<<
  *         return self._incoming.pending
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -151462,15 +151458,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_Handle __pyx_vtable_7winloop_4loop_Handle;
 
 static struct __pyx_obj_7winloop_4loop_Handle *__pyx_freelist_7winloop_4loop_Handle[250];
 static int __pyx_freecount_7winloop_4loop_Handle = 0;
@@ -151647,15 +151643,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_TimerHandle __pyx_vtable_7winloop_4loop_TimerHandle;
 
 static struct __pyx_obj_7winloop_4loop_TimerHandle *__pyx_freelist_7winloop_4loop_TimerHandle[250];
 static int __pyx_freecount_7winloop_4loop_TimerHandle = 0;
@@ -151831,15 +151827,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVRequest __pyx_vtable_7winloop_4loop_UVRequest;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVRequest(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVRequest *p;
@@ -151959,15 +151955,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_7winloop_4loop__SSLProtocolTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop__SSLProtocolTransport *p;
   PyObject *o;
@@ -152139,15 +152135,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_SSLProtocol __pyx_vtable_7winloop_4loop_SSLProtocol;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_SSLProtocol(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_SSLProtocol *p;
@@ -152461,15 +152457,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_Server __pyx_vtable_7winloop_4loop_Server;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_Server(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_Server *p;
@@ -152631,15 +152627,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVHandle __pyx_vtable_7winloop_4loop_UVHandle;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVHandle(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVHandle *p;
@@ -152792,15 +152788,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVSocketHandle __pyx_vtable_7winloop_4loop_UVSocketHandle;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVSocketHandle(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVSocketHandle *p;
@@ -152934,15 +152930,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVAsync __pyx_vtable_7winloop_4loop_UVAsync;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVAsync(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVAsync *p;
@@ -153054,15 +153050,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVIdle __pyx_vtable_7winloop_4loop_UVIdle;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVIdle(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVIdle *p;
@@ -153174,15 +153170,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVCheck __pyx_vtable_7winloop_4loop_UVCheck;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVCheck(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVCheck *p;
@@ -153294,15 +153290,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVTimer __pyx_vtable_7winloop_4loop_UVTimer;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVTimer(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVTimer *p;
@@ -153414,15 +153410,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVPoll __pyx_vtable_7winloop_4loop_UVPoll;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVPoll(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVPoll *p;
@@ -153539,15 +153535,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVBaseTransport __pyx_vtable_7winloop_4loop_UVBaseTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVBaseTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVBaseTransport *p;
@@ -153730,15 +153726,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVStream __pyx_vtable_7winloop_4loop_UVStream;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVStream(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVStream *p;
@@ -153871,15 +153867,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVStreamServer __pyx_vtable_7winloop_4loop_UVStreamServer;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVStreamServer(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVStreamServer *p;
@@ -154016,15 +154012,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_TCPServer __pyx_vtable_7winloop_4loop_TCPServer;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_TCPServer(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_TCPServer *p;
@@ -154112,15 +154108,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_TCPTransport __pyx_vtable_7winloop_4loop_TCPTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_TCPTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_TCPTransport *p;
@@ -154209,15 +154205,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UnixServer __pyx_vtable_7winloop_4loop_UnixServer;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UnixServer(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UnixServer *p;
@@ -154305,15 +154301,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UnixTransport __pyx_vtable_7winloop_4loop_UnixTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UnixTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UnixTransport *p;
@@ -154401,15 +154397,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_ReadUnixTransport __pyx_vtable_7winloop_4loop_ReadUnixTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_ReadUnixTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_ReadUnixTransport *p;
@@ -154505,15 +154501,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_WriteUnixTransport __pyx_vtable_7winloop_4loop_WriteUnixTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_WriteUnixTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_WriteUnixTransport *p;
@@ -154603,15 +154599,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVProcess __pyx_vtable_7winloop_4loop_UVProcess;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVProcess(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVProcess *p;
@@ -154772,15 +154768,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVProcessTransport __pyx_vtable_7winloop_4loop_UVProcessTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVProcessTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVProcessTransport *p;
@@ -154954,15 +154950,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UVFSEvent __pyx_vtable_7winloop_4loop_UVFSEvent;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UVFSEvent(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UVFSEvent *p;
@@ -155076,15 +155072,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_UDPTransport __pyx_vtable_7winloop_4loop_UDPTransport;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_UDPTransport(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_UDPTransport *p;
@@ -155201,15 +155197,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_PseudoSocket __pyx_vtable_7winloop_4loop_PseudoSocket;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_PseudoSocket(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7winloop_4loop_PseudoSocket *p;
@@ -155389,15 +155385,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop__StreamWriteContext __pyx_vtable_7winloop_4loop__StreamWriteContext;
 
 static struct __pyx_obj_7winloop_4loop__StreamWriteContext *__pyx_freelist_7winloop_4loop__StreamWriteContext[250];
 static int __pyx_freecount_7winloop_4loop__StreamWriteContext = 0;
@@ -155531,15 +155527,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop__TCPConnectRequest __pyx_vtable_7winloop_4loop__TCPConnectRequest;
 
 static PyObject *__pyx_tp_new_7winloop_4loop__TCPConnectRequest(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop__TCPConnectRequest *p;
@@ -155657,15 +155653,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop__PipeConnectRequest __pyx_vtable_7winloop_4loop__PipeConnectRequest;
 
 static PyObject *__pyx_tp_new_7winloop_4loop__PipeConnectRequest(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop__PipeConnectRequest *p;
@@ -155783,15 +155779,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop__UDPSendContext __pyx_vtable_7winloop_4loop__UDPSendContext;
 
 static struct __pyx_obj_7winloop_4loop__UDPSendContext *__pyx_freelist_7winloop_4loop__UDPSendContext[250];
 static int __pyx_freecount_7winloop_4loop__UDPSendContext = 0;
@@ -155924,15 +155920,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_LruCache __pyx_vtable_7winloop_4loop_LruCache;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_LruCache(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_7winloop_4loop_LruCache *p;
@@ -156090,15 +156086,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop_SockAddrHolder *__pyx_freelist_7winloop_4loop_SockAddrHolder[250];
 static int __pyx_freecount_7winloop_4loop_SockAddrHolder = 0;
 
@@ -156201,15 +156197,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_AddrInfo __pyx_vtable_7winloop_4loop_AddrInfo;
 
 static struct __pyx_obj_7winloop_4loop_AddrInfo *__pyx_freelist_7winloop_4loop_AddrInfo[250];
 static int __pyx_freecount_7winloop_4loop_AddrInfo = 0;
@@ -156328,15 +156324,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_AddrInfoRequest __pyx_vtable_7winloop_4loop_AddrInfoRequest;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_AddrInfoRequest(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_AddrInfoRequest *p;
@@ -156454,15 +156450,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_7winloop_4loop_NameInfoRequest __pyx_vtable_7winloop_4loop_NameInfoRequest;
 
 static PyObject *__pyx_tp_new_7winloop_4loop_NameInfoRequest(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_7winloop_4loop_NameInfoRequest *p;
@@ -156580,15 +156576,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct___getaddrinfo *__pyx_freelist_7winloop_4loop___pyx_scope_struct___getaddrinfo[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct___getaddrinfo = 0;
 
@@ -156698,15 +156694,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_1__getnameinfo *__pyx_freelist_7winloop_4loop___pyx_scope_struct_1__getnameinfo[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_1__getnameinfo = 0;
 
@@ -156816,15 +156812,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_2___get__ *__pyx_freelist_7winloop_4loop___pyx_scope_struct_2___get__[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_2___get__ = 0;
 
@@ -156934,15 +156930,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_3_run_until_complete *__pyx_freelist_7winloop_4loop___pyx_scope_struct_3_run_until_complete[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_3_run_until_complete = 0;
 
@@ -157052,15 +157048,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_4_getaddrinfo *__pyx_freelist_7winloop_4loop___pyx_scope_struct_4_getaddrinfo[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_4_getaddrinfo = 0;
 
@@ -157173,15 +157169,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_5_getnameinfo *__pyx_freelist_7winloop_4loop___pyx_scope_struct_5_getnameinfo[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_5_getnameinfo = 0;
 
@@ -157298,15 +157294,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_6_start_tls *__pyx_freelist_7winloop_4loop___pyx_scope_struct_6_start_tls[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_6_start_tls = 0;
 
@@ -157471,15 +157467,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_7_create_server *__pyx_freelist_7winloop_4loop___pyx_scope_struct_7_create_server[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_7_create_server = 0;
 
@@ -157660,15 +157656,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_8_create_connection *__pyx_freelist_7winloop_4loop___pyx_scope_struct_8_create_connection[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_8_create_connection = 0;
 
@@ -157901,15 +157897,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_9_genexpr *__pyx_freelist_7winloop_4loop___pyx_scope_struct_9_genexpr[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_9_genexpr = 0;
 
@@ -158014,15 +158010,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_10_genexpr *__pyx_freelist_7winloop_4loop___pyx_scope_struct_10_genexpr[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_10_genexpr = 0;
 
@@ -158127,15 +158123,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_11_create_unix_server *__pyx_freelist_7winloop_4loop___pyx_scope_struct_11_create_unix_server[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_11_create_unix_server = 0;
 
@@ -158292,15 +158288,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_12_create_unix_connection *__pyx_freelist_7winloop_4loop___pyx_scope_struct_12_create_unix_connection[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_12_create_unix_connection = 0;
 
@@ -158473,15 +158469,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_13_sock_recv *__pyx_freelist_7winloop_4loop___pyx_scope_struct_13_sock_recv[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_13_sock_recv = 0;
 
@@ -158598,15 +158594,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_14_sock_recv_into *__pyx_freelist_7winloop_4loop___pyx_scope_struct_14_sock_recv_into[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_14_sock_recv_into = 0;
 
@@ -158723,15 +158719,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_15_sock_sendall *__pyx_freelist_7winloop_4loop___pyx_scope_struct_15_sock_sendall[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_15_sock_sendall = 0;
 
@@ -158848,15 +158844,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_16_sock_accept *__pyx_freelist_7winloop_4loop___pyx_scope_struct_16_sock_accept[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_16_sock_accept = 0;
 
@@ -158969,15 +158965,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_17_sock_connect *__pyx_freelist_7winloop_4loop___pyx_scope_struct_17_sock_connect[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_17_sock_connect = 0;
 
@@ -159098,15 +159094,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_18_sock_recvfrom *__pyx_freelist_7winloop_4loop___pyx_scope_struct_18_sock_recvfrom[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_18_sock_recvfrom = 0;
 
@@ -159215,15 +159211,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_19_sock_recvfrom_into *__pyx_freelist_7winloop_4loop___pyx_scope_struct_19_sock_recvfrom_into[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_19_sock_recvfrom_into = 0;
 
@@ -159336,15 +159332,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_20_sock_sendto *__pyx_freelist_7winloop_4loop___pyx_scope_struct_20_sock_sendto[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_20_sock_sendto = 0;
 
@@ -159457,15 +159453,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_21_connect_accepted_socket *__pyx_freelist_7winloop_4loop___pyx_scope_struct_21_connect_accepted_socket[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_21_connect_accepted_socket = 0;
 
@@ -159626,15 +159622,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_22___subprocess_run *__pyx_freelist_7winloop_4loop___pyx_scope_struct_22___subprocess_run[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_22___subprocess_run = 0;
 
@@ -159835,15 +159831,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_23_subprocess_shell *__pyx_freelist_7winloop_4loop___pyx_scope_struct_23_subprocess_shell[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_23_subprocess_shell = 0;
 
@@ -159964,15 +159960,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_24_subprocess_exec *__pyx_freelist_7winloop_4loop___pyx_scope_struct_24_subprocess_exec[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_24_subprocess_exec = 0;
 
@@ -160093,15 +160089,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_25_connect_read_pipe *__pyx_freelist_7winloop_4loop___pyx_scope_struct_25_connect_read_pipe[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_25_connect_read_pipe = 0;
 
@@ -160234,15 +160230,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_26_connect_write_pipe *__pyx_freelist_7winloop_4loop___pyx_scope_struct_26_connect_write_pipe[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_26_connect_write_pipe = 0;
 
@@ -160375,15 +160371,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_27_create_datagram_endpoint *__pyx_freelist_7winloop_4loop___pyx_scope_struct_27_create_datagram_endpoint[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_27_create_datagram_endpoint = 0;
 
@@ -160565,15 +160561,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_28_genexpr *__pyx_freelist_7winloop_4loop___pyx_scope_struct_28_genexpr[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_28_genexpr = 0;
 
@@ -160682,15 +160678,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_29_shutdown_asyncgens *__pyx_freelist_7winloop_4loop___pyx_scope_struct_29_shutdown_asyncgens[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_29_shutdown_asyncgens = 0;
 
@@ -160815,15 +160811,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_30_shutdown_default_executor *__pyx_freelist_7winloop_4loop___pyx_scope_struct_30_shutdown_default_executor[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_30_shutdown_default_executor = 0;
 
@@ -160932,15 +160928,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_31__start_handshake *__pyx_freelist_7winloop_4loop___pyx_scope_struct_31__start_handshake[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_31__start_handshake = 0;
 
@@ -161050,15 +161046,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_32__start_shutdown *__pyx_freelist_7winloop_4loop___pyx_scope_struct_32__start_shutdown[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_32__start_shutdown = 0;
 
@@ -161168,15 +161164,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_33___aenter__ *__pyx_freelist_7winloop_4loop___pyx_scope_struct_33___aenter__[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_33___aenter__ = 0;
 
@@ -161277,15 +161273,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_34___aexit__ *__pyx_freelist_7winloop_4loop___pyx_scope_struct_34___aexit__[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_34___aexit__ = 0;
 
@@ -161390,15 +161386,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_35_wait_closed *__pyx_freelist_7winloop_4loop___pyx_scope_struct_35_wait_closed[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_35_wait_closed = 0;
 
@@ -161503,15 +161499,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_36_start_serving *__pyx_freelist_7winloop_4loop___pyx_scope_struct_36_start_serving[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_36_start_serving = 0;
 
@@ -161612,15 +161608,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_37_serve_forever *__pyx_freelist_7winloop_4loop___pyx_scope_struct_37_serve_forever[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_37_serve_forever = 0;
 
@@ -161745,15 +161741,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_7winloop_4loop___pyx_scope_struct_38__test_coroutine_1 *__pyx_freelist_7winloop_4loop___pyx_scope_struct_38__test_coroutine_1[8];
 static int __pyx_freecount_7winloop_4loop___pyx_scope_struct_38__test_coroutine_1 = 0;
 
@@ -161841,15 +161837,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_object____Loop____bint___to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_object____Loop____bint___to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_object____Loop____bint___to_py = 0;
 
@@ -161937,15 +161933,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -166658,29 +166654,34 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(27, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(27, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(27, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(28, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(28, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT(PyBoolObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(28, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(29, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(29, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT(PyComplexObject),
+  __Pyx_ImportType_CheckSize_Warn);
+   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(29, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -172788,18 +172789,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -174165,18 +174163,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 #if PY_VERSION_HEX < 0x030500B1 || defined(__Pyx_IterableCoroutine_USED) || CYTHON_USE_ASYNC_SLOTS
 static CYTHON_INLINE PyObject *__Pyx__Coroutine_await(PyObject *coroutine) {
     __pyx_CoroutineAwaitObject *await = PyObject_GC_New(__pyx_CoroutineAwaitObject, __pyx_CoroutineAwaitType);
     if (unlikely(!await)) return NULL;
@@ -174320,18 +174315,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_Coroutine_init(void) {
     __pyx_CoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_CoroutineType = __Pyx_FetchCommonType(&__pyx_CoroutineType_type);
     if (unlikely(!__pyx_CoroutineType))
@@ -174399,15 +174391,15 @@
 #if PY_VERSION_HEX >= 0x030500B2 || defined(PyCoro_CheckExact)
     if (PyCoro_CheckExact(obj)) {
         return __Pyx_NewRef(obj);
     } else
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && defined(CO_ITERABLE_COROUTINE)
 #if PY_VERSION_HEX >= 0x030C00A6
-    if (PyGen_CheckExact(obj) && (PyGen_GetCode((PyGenObject*)obj)->co_flags & CO_ITERABLE_COROUTINE)) {
+    if (PyGen_CheckExact(obj) && (PyGen_GetCode(obj)->co_flags & CO_ITERABLE_COROUTINE)) {
 #else
     if (PyGen_CheckExact(obj) && ((PyGenObject*)obj)->gi_code && ((PyCodeObject *)((PyGenObject*)obj)->gi_code)->co_flags & CO_ITERABLE_COROUTINE) {
 #endif
         return __Pyx_NewRef(obj);
     } else
 #endif
     {
@@ -175509,18 +175501,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType
+#define __PYX_HAVE_RT_ImportType
+static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -175566,22 +175558,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -176150,15 +176142,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -176346,15 +176338,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -176580,15 +176572,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -176852,15 +176844,15 @@
                         } else if (8 * sizeof(unsigned long) >= 4 * PyLong_SHIFT) {
                             return (unsigned long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -177048,15 +177040,15 @@
                         } else if (8 * sizeof(unsigned int) >= 4 * PyLong_SHIFT) {
                             return (unsigned int) (((((((((unsigned int)digits[3]) << PyLong_SHIFT) | (unsigned int)digits[2]) << PyLong_SHIFT) | (unsigned int)digits[1]) << PyLong_SHIFT) | (unsigned int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -177320,15 +177312,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -177716,18 +177708,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_IterableCoroutine_init(void) {
     __pyx_IterableCoroutineType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_IterableCoroutineType = __Pyx_FetchCommonType(&__pyx_IterableCoroutineType_type);
     if (unlikely(!__pyx_IterableCoroutineType))
@@ -177820,18 +177809,15 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `winloop-0.0.5/winloop/loop.pxd` & `winloop-0.0.6/winloop/loop.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     cdef _call_soon(self, object callback, object args, object context)
     cdef _append_ready_handle(self, Handle handle)
     cdef _call_soon_handle(self, Handle handle)
 
     cdef _call_later(self, uint64_t delay, object callback, object args,
                      object context)
 
-    cdef void _handle_exception(self, object ex)
+    cdef void _handle_exception(self, object ex) noexcept
 
     cdef bint _is_main_thread(self)
 
     cdef _new_future(self)
     cdef _check_signal(self, sig)
     cdef _check_closed(self)
     cdef _check_thread(self)
```

### Comparing `winloop-0.0.5/winloop/loop.pyi` & `winloop-0.0.6/winloop/loop.pyi`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/loop.pyx` & `winloop-0.0.6/winloop/loop.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -3328,15 +3328,15 @@
 
 
 
 
 
 cdef void __loop_alloc_buffer(uv.uv_handle_t* uvhandle,
                               size_t suggested_size,
-                              uv.uv_buf_t* buf) with gil:
+                              uv.uv_buf_t* buf) noexcept with gil:
     cdef:
         Loop loop = (<UVHandle>uvhandle.data)._loop
 
     if loop._recv_buffer_in_use == 1:
         buf.len = 0
         exc = RuntimeError('concurrent allocations')
         loop._handle_exception(exc)
```

### Comparing `winloop-0.0.5/winloop/lru.pyx` & `winloop-0.0.6/winloop/lru.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/pseudosock.pyx` & `winloop-0.0.6/winloop/pseudosock.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/request.pyx` & `winloop-0.0.6/winloop/request.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/server.pyx` & `winloop-0.0.6/winloop/server.pyx`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/sslproto.pxd` & `winloop-0.0.6/winloop/sslproto.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,21 @@
     cdef _do_read__buffered(self)
     cdef _do_read__copied(self)
     cdef _call_eof_received(self, object context=*)
 
     # Flow control for writes from APP socket
 
     cdef _control_app_writing(self, object context=*)
-    cdef size_t _get_write_buffer_size(self)
+    cdef size_t _get_write_buffer_size(self) noexcept
     cdef _set_write_buffer_limits(self, high=*, low=*)
 
     # Flow control for reads to APP socket
 
     cdef _pause_reading(self)
     cdef _resume_reading(self, object context)
 
     # Flow control for reads from SSL socket
 
     cdef _control_ssl_reading(self)
     cdef _set_read_buffer_limits(self, high=*, low=*)
-    cdef size_t _get_read_buffer_size(self)
+    cdef size_t _get_read_buffer_size(self) noexcept
     cdef _fatal_error(self, exc, message=*)
```

### Comparing `winloop-0.0.5/winloop/sslproto.pyx` & `winloop-0.0.6/winloop/sslproto.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -881,15 +881,15 @@
                 self._loop.call_exception_handler({
                     'message': 'protocol.resume_writing() failed',
                     'exception': exc,
                     'transport': self._app_transport,
                     'protocol': self,
                 })
 
-    cdef size_t _get_write_buffer_size(self):
+    cdef size_t _get_write_buffer_size(self) noexcept:
         return self._outgoing.pending + self._write_buffer_size
 
     cdef _set_write_buffer_limits(self, high=None, low=None):
         high, low = add_flowcontrol_defaults(
             high, low, FLOW_CONTROL_HIGH_WATER_SSL_WRITE)
         self._outgoing_high_water = high
         self._outgoing_low_water = low
@@ -923,15 +923,15 @@
 
     cdef _set_read_buffer_limits(self, high=None, low=None):
         high, low = add_flowcontrol_defaults(
             high, low, FLOW_CONTROL_HIGH_WATER_SSL_READ)
         self._incoming_high_water = high
         self._incoming_low_water = low
 
-    cdef size_t _get_read_buffer_size(self):
+    cdef size_t _get_read_buffer_size(self) noexcept:
         return self._incoming.pending
 
     # Flow control for writes to SSL socket
 
     def pause_writing(self):
         """Called when the low-level transport's buffer goes over
         the high-water mark.
```

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/aix.h` & `winloop-0.0.6/winloop/vendor/include/uv/aix.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/bsd.h` & `winloop-0.0.6/winloop/vendor/include/uv/bsd.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/darwin.h` & `winloop-0.0.6/winloop/vendor/include/uv/darwin.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/errno.h` & `winloop-0.0.6/winloop/vendor/include/uv/errno.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/linux.h` & `winloop-0.0.6/winloop/vendor/include/uv/linux.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/os390.h` & `winloop-0.0.6/winloop/vendor/include/uv/os390.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/posix.h` & `winloop-0.0.6/winloop/vendor/include/uv/posix.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/stdint-msvc2008.h` & `winloop-0.0.6/winloop/vendor/include/uv/stdint-msvc2008.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/sunos.h` & `winloop-0.0.6/winloop/vendor/include/uv/sunos.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/threadpool.h` & `winloop-0.0.6/winloop/vendor/include/uv/threadpool.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/tree.h` & `winloop-0.0.6/winloop/vendor/include/uv/tree.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/unix.h` & `winloop-0.0.6/winloop/vendor/include/uv/unix.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/version.h` & `winloop-0.0.6/winloop/vendor/include/uv/version.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv/win.h` & `winloop-0.0.6/winloop/vendor/include/uv/win.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/include/uv.h` & `winloop-0.0.6/winloop/vendor/include/uv.h`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/vendor/uv_a.lib` & `winloop-0.0.6/winloop/vendor/uv_a.lib`

 * *Files identical despite different names*

### Comparing `winloop-0.0.5/winloop/winloop.egg-info/PKG-INFO` & `winloop-0.0.6/winloop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: winloop
-Version: 0.0.4
+Version: 0.0.6
 Summary: An Alternative library for uvloop compatability with windows
+Home-page: https://github.com/vizonex/winloop
 Author: Vizonex
 License: MIT
 Keywords: winloop,libuv,windows,cython,fast-asyncio,uvloop-alternative
 Platform: Microsoft Windows
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `winloop-0.0.5/winloop/winloop.egg-info/SOURCES.txt` & `winloop-0.0.6/winloop.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE-APACHE
 LICENSE-MIT
 MANIFEST.in
+pyproject.toml
 setup.py
 winloop/__init__.py
 winloop/_noop.py
-winloop/_testbase.py
 winloop/cbhandles.pxd
 winloop/cbhandles.pyx
 winloop/dns.pyx
 winloop/errors.pyx
 winloop/loop.c
 winloop/loop.cp39-win_amd64.pyd
 winloop/loop.pxd
@@ -18,17 +18,19 @@
 winloop/pseudosock.pyx
 winloop/request.pxd
 winloop/request.pyx
 winloop/server.pxd
 winloop/server.pyx
 winloop/sslproto.pxd
 winloop/sslproto.pyx
-winloop/__pycache__/__init__.cpython-39.pyc
-winloop/__pycache__/_noop.cpython-39.pyc
-winloop/__pycache__/_testbase.cpython-39.pyc
+winloop.egg-info/PKG-INFO
+winloop.egg-info/SOURCES.txt
+winloop.egg-info/dependency_links.txt
+winloop.egg-info/requires.txt
+winloop.egg-info/top_level.txt
 winloop/handles/async_.pxd
 winloop/handles/async_.pyx
 winloop/handles/basetransport.pxd
 winloop/handles/basetransport.pyx
 winloop/handles/check.pxd
 winloop/handles/check.pyx
 winloop/handles/fsevent.pxd
@@ -51,28 +53,25 @@
 winloop/handles/tcp.pyx
 winloop/handles/timer.pxd
 winloop/handles/timer.pyx
 winloop/handles/udp.pxd
 winloop/handles/udp.pyx
 winloop/includes/__init__.py
 winloop/includes/_python.pxd
-winloop/includes/_stdlib.html
 winloop/includes/_stdlib.pxi
-winloop/includes/consts.html
 winloop/includes/consts.pxi
 winloop/includes/context.h
 winloop/includes/debug.h
 winloop/includes/debug.pxd
 winloop/includes/flowcontrol.pxd
 winloop/includes/nfork_handler.h
 winloop/includes/socketpair.h
 winloop/includes/system.pxd
 winloop/includes/tcp.h
 winloop/includes/uv.pxd
-winloop/includes/__pycache__/__init__.cpython-39.pyc
 winloop/vendor/uv_a.lib
 winloop/vendor/include/uv.h
 winloop/vendor/include/uv/aix.h
 winloop/vendor/include/uv/bsd.h
 winloop/vendor/include/uv/darwin.h
 winloop/vendor/include/uv/errno.h
 winloop/vendor/include/uv/linux.h
@@ -80,13 +79,8 @@
 winloop/vendor/include/uv/posix.h
 winloop/vendor/include/uv/stdint-msvc2008.h
 winloop/vendor/include/uv/sunos.h
 winloop/vendor/include/uv/threadpool.h
 winloop/vendor/include/uv/tree.h
 winloop/vendor/include/uv/unix.h
 winloop/vendor/include/uv/version.h
-winloop/vendor/include/uv/win.h
-winloop/winloop.egg-info/PKG-INFO
-winloop/winloop.egg-info/SOURCES.txt
-winloop/winloop.egg-info/dependency_links.txt
-winloop/winloop.egg-info/requires.txt
-winloop/winloop.egg-info/top_level.txt
+winloop/vendor/include/uv/win.h
```

