# Comparing `tmp/pyjls-0.7.1.tar.gz` & `tmp/pyjls-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.7.1.tar", last modified: Wed Jun  7 21:34:37 2023, max compression
+gzip compressed data, was "pyjls-0.7.2.tar", last modified: Wed Jun 14 09:28:24 2023, max compression
```

## Comparing `pyjls-0.7.1.tar` & `pyjls-0.7.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.906780 pyjls-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-07 21:34:22.000000 pyjls-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-07 21:34:22.000000 pyjls-0.7.1/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 21:34:22.000000 pyjls-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 21:34:22.000000 pyjls-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-07 21:34:37.906780 pyjls-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-07 21:34:22.000000 pyjls-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.894780 pyjls-0.7.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.898780 pyjls-0.7.1/include/jls/
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/backend.h
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/cmacro.h
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/crc32c.h
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/ec.h
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/format.h
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/log.h
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/raw.h
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/reader.h
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/statistics.h
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/threaded_writer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/time.h
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls/writer.h
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-07 21:34:22.000000 pyjls-0.7.1/include/jls.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.894780 pyjls-0.7.1/include_prv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.898780 pyjls-0.7.1/include_prv/jls/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/bit_shift.h
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/cdef.h
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/datatype.h
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/msg_ring_buffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/rd_fsr.h
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/util.h
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/wr_fsr.h
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/wr_prv.h
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-07 21:34:22.000000 pyjls-0.7.1/include_prv/jls/wr_ts.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.902780 pyjls-0.7.1/pyjls/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1639926 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.902780 pyjls-0.7.1/pyjls/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/entry_points/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/entry_points/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/entry_points/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/entry_points/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.902780 pyjls-0.7.1/pyjls/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/test/test_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.902780 pyjls-0.7.1/pyjls/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyjls/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.902780 pyjls-0.7.1/pyjls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 21:34:37.000000 pyjls-0.7.1/pyjls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-07 21:34:22.000000 pyjls-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:34:37.906780 pyjls-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-07 21:34:22.000000 pyjls-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:34:37.906780 pyjls-0.7.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/backend_posix.c
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/backend_win.c
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/bit_shift.c
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/crc32c.c
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/crc32c_arm_neon.c
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/crc32c_intel_sse4.c
--rw-r--r--   0 runner    (1001) docker     (123)    33131 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/crc32c_sw.c
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/datatype.c
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/ec.c
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/log.c
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/msg_ring_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/raw.c
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/rd_fsr.c
--rw-r--r--   0 runner    (1001) docker     (123)    53622 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/statistics.c
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/threaded_writer.c
--rw-r--r--   0 runner    (1001) docker     (123)    27409 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/wr_fsr.c
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/wr_ts.c
--rw-r--r--   0 runner    (1001) docker     (123)    29536 2023-06-07 21:34:22.000000 pyjls-0.7.1/src/writer.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.258803 pyjls-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-14 09:28:05.000000 pyjls-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-14 09:28:05.000000 pyjls-0.7.2/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 09:28:05.000000 pyjls-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-14 09:28:05.000000 pyjls-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-14 09:28:24.258803 pyjls-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-14 09:28:05.000000 pyjls-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.238803 pyjls-0.7.2/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.242803 pyjls-0.7.2/include/jls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/backend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/cmacro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/crc32c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/ec.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/format.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/raw.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/reader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/statistics.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/threaded_writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/time.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls/writer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-14 09:28:05.000000 pyjls-0.7.2/include/jls.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.234803 pyjls-0.7.2/include_prv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.246803 pyjls-0.7.2/include_prv/jls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/bit_shift.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/cdef.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/datatype.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/msg_ring_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/rd_fsr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/wr_fsr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/wr_prv.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-14 09:28:05.000000 pyjls-0.7.2/include_prv/jls/wr_ts.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.250803 pyjls-0.7.2/pyjls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1639926 2023-06-14 09:28:23.000000 pyjls-0.7.2/pyjls/binding.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.250803 pyjls-0.7.2/pyjls/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/entry_points/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/entry_points/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/entry_points/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/entry_points/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.254804 pyjls-0.7.2/pyjls/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/test/test_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.254804 pyjls-0.7.2/pyjls/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyjls/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.250803 pyjls-0.7.2/pyjls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-06-14 09:28:24.000000 pyjls-0.7.2/pyjls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-14 09:28:24.000000 pyjls-0.7.2/pyjls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:28:24.000000 pyjls-0.7.2/pyjls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 09:28:24.000000 pyjls-0.7.2/pyjls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 09:28:24.000000 pyjls-0.7.2/pyjls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 09:28:24.000000 pyjls-0.7.2/pyjls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-14 09:28:05.000000 pyjls-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 09:28:24.258803 pyjls-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-14 09:28:05.000000 pyjls-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:28:24.258803 pyjls-0.7.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/backend_posix.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/backend_win.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/bit_shift.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/crc32c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/crc32c_arm_neon.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/crc32c_intel_sse4.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33131 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/crc32c_sw.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/datatype.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/ec.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/msg_ring_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/raw.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/rd_fsr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53622 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/reader.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/statistics.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/threaded_writer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    27409 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/wr_fsr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/wr_ts.c
+-rw-r--r--   0 runner    (1001) docker     (123)    29536 2023-06-14 09:28:05.000000 pyjls-0.7.2/src/writer.c
```

### Comparing `pyjls-0.7.1/CHANGELOG.md` & `pyjls-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to the JLS project.
 
 
+## 0.7.2
+
+2023 Jun 14
+
+* Fixed build for Raspberry Pi.
+* Added JLS_OPTIMIZE_CRC cmake option.
+
+
 ## 0.7.1
 
 2023 Jun 7
 
 * Added Reader.signal_lookup.
 * Improved documentation.
 * Added Read The Docs integration.
```

### Comparing `pyjls-0.7.1/CREDITS.html` & `pyjls-0.7.2/CREDITS.html`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/LICENSE` & `pyjls-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/PKG-INFO` & `pyjls-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.7.1
+Version: 0.7.2
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.7.1/README.md` & `pyjls-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/backend.h` & `pyjls-0.7.2/include/jls/backend.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/cmacro.h` & `pyjls-0.7.2/include/jls/cmacro.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/crc32c.h` & `pyjls-0.7.2/include/jls/crc32c.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/ec.h` & `pyjls-0.7.2/include/jls/ec.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/format.h` & `pyjls-0.7.2/include/jls/format.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/log.h` & `pyjls-0.7.2/include/jls/log.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/raw.h` & `pyjls-0.7.2/include/jls/raw.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/reader.h` & `pyjls-0.7.2/include/jls/reader.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/statistics.h` & `pyjls-0.7.2/include/jls/statistics.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/threaded_writer.h` & `pyjls-0.7.2/include/jls/threaded_writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/time.h` & `pyjls-0.7.2/include/jls/time.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls/version.h` & `pyjls-0.7.2/include/jls/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  */
 
 JLS_CPP_GUARD_START
 
 // Use version_update.py to update.
 #define JLS_VERSION_MAJOR 0
 #define JLS_VERSION_MINOR 7
-#define JLS_VERSION_PATCH 1
+#define JLS_VERSION_PATCH 2
 
 /**
  * \brief Macro to encode version to uint32_t.
  *
  * \param major The major release number (0 to 255)
  * \param minor The minor release number (0 to 255)
  * \param patch The patch release number (0 to 65535)
```

### Comparing `pyjls-0.7.1/include/jls/writer.h` & `pyjls-0.7.2/include/jls/writer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include/jls.h` & `pyjls-0.7.2/include/jls.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/bit_shift.h` & `pyjls-0.7.2/include_prv/jls/bit_shift.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/cdef.h` & `pyjls-0.7.2/include_prv/jls/cdef.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/datatype.h` & `pyjls-0.7.2/include_prv/jls/datatype.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/msg_ring_buffer.h` & `pyjls-0.7.2/include_prv/jls/msg_ring_buffer.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/rd_fsr.h` & `pyjls-0.7.2/include_prv/jls/rd_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/util.h` & `pyjls-0.7.2/include_prv/jls/util.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/wr_fsr.h` & `pyjls-0.7.2/include_prv/jls/wr_fsr.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/wr_prv.h` & `pyjls-0.7.2/include_prv/jls/wr_prv.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/include_prv/jls/wr_ts.h` & `pyjls-0.7.2/include_prv/jls/wr_ts.h`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/__init__.py` & `pyjls-0.7.2/pyjls/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/__main__.py` & `pyjls-0.7.2/pyjls/__main__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/binding.c` & `pyjls-0.7.2/pyjls/binding.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-msse4.2"
         ],
         "include_dirs": [
             "include",
             "include_prv",
-            "/tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/core/include"
         ],
         "libraries": [
             "pthread",
             "m"
         ],
         "name": "pyjls.binding",
         "sources": [
@@ -1150,195 +1150,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1372,42 +1372,42 @@
 struct __pyx_obj_5pyjls_7binding_AnnotationCallback;
 struct __pyx_obj_5pyjls_7binding_Reader;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -14943,15 +14943,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -14960,29 +14960,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -14993,15 +14993,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15010,29 +15010,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -15043,15 +15043,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15060,29 +15060,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -15093,15 +15093,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15110,29 +15110,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -15143,15 +15143,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15160,29 +15160,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -15193,212 +15193,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15414,15 +15414,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -15430,53 +15430,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -15484,30 +15484,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -15522,15 +15522,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15546,15 +15546,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15562,53 +15562,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -15616,30 +15616,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15654,15 +15654,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15678,15 +15678,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -15694,53 +15694,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -15748,30 +15748,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -15786,176 +15786,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -30565,26 +30565,26 @@
   __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_self__rd_cannot_be_converted_to); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
   __pyx_tuple__13 = PyTuple_Pack(3, __pyx_int_3248624, __pyx_int_200305830, __pyx_int_134405936); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
-  /* "../../../../../tmp/build-env-pr837epv/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-hln9x_rt/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 950, __pyx_L1_error)
```

### Comparing `pyjls-0.7.1/pyjls/entry_points/__init__.py` & `pyjls-0.7.2/pyjls/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/entry_points/annotate.py` & `pyjls-0.7.2/pyjls/entry_points/annotate.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/entry_points/export.py` & `pyjls-0.7.2/pyjls/entry_points/export.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/entry_points/info.py` & `pyjls-0.7.2/pyjls/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/entry_points/plot.py` & `pyjls-0.7.2/pyjls/entry_points/plot.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/structs.py` & `pyjls-0.7.2/pyjls/structs.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/test/__init__.py` & `pyjls-0.7.2/pyjls/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/test/test_binding.py` & `pyjls-0.7.2/pyjls/test/test_binding.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/v1/__init__.py` & `pyjls-0.7.2/pyjls/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyjls/version.py` & `pyjls-0.7.2/pyjls/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
 __title__ = "pyjls"
 __description__ = 'Joulescope™ file format'
 __url__ = 'https://joulescope.readthedocs.io'
 __author__ = 'Jetperch LLC'
 __author_email__ = 'joulescope-dev@jetperch.com'
 __license__ = 'Apache 2.0'
```

### Comparing `pyjls-0.7.1/pyjls.egg-info/PKG-INFO` & `pyjls-0.7.2/pyjls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjls
-Version: 0.7.1
+Version: 0.7.2
 Summary: Joulescope™ file format
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/jls/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `pyjls-0.7.1/pyjls.egg-info/SOURCES.txt` & `pyjls-0.7.2/pyjls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/pyproject.toml` & `pyjls-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/setup.py` & `pyjls-0.7.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,21 +46,30 @@
     exec(f.read(), about)
 
 
 extra_compile_args = []
 if platform.system() == 'Windows':
     sources = ['src/backend_win.c']
     libraries = []
+    if platform.machine() in ['AMD64', 'x86_64']:
+        pass  # SSE supported by default
+    else:
+        print(f'Unknown windows machine: {platform.machine()}')
 else:
     sources = ['src/backend_posix.c']
     libraries = ['pthread', 'm']
-    if platform.system() == 'Linux':
-        extra_compile_args = ['-msse4.2']
-    elif platform.system() == 'Darwin':
-        extra_compile_args = ['-msse4.2', '-mcrc']
+    if platform.system() == 'Darwin':
+        extra_compile_args = ['-msse4.2', '-mcrc']  # universal2
+    elif platform.system() == 'Linux':
+        if platform.processor() == 'x86_64':
+            extra_compile_args = ['-msse4.2']
+        else:
+            # Raspberry Pi 4 does not support CRC acceleration
+            # While other non x86_64 platforms may, do not provide any compiler flags
+            print(f'CRC optimization likely disabled')
 
 
 ext = '.pyx' if USE_CYTHON else '.c'
 extensions = [
     setuptools.Extension('pyjls.binding',
         sources=[
             'pyjls/binding' + ext,
```

### Comparing `pyjls-0.7.1/src/backend_posix.c` & `pyjls-0.7.2/src/backend_posix.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/backend_win.c` & `pyjls-0.7.2/src/backend_win.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/bit_shift.c` & `pyjls-0.7.2/src/bit_shift.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/crc32c.c` & `pyjls-0.7.2/src/crc32c.c`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,40 @@
  *
  * We would prefer to use the build process to include the correct
  * implementation.  However, the variations with building
  * python wheels make this very challenging, especially considering
  * macOS universal2 builds.  Since the native compilation must know
  * compiler flags, we make the decision here.
  */
+
+#if defined(JLS_OPTIMIZE_CRC_DISABLE)
+#include "crc32c_sw.c"
+
+#elif defined(WIN32) || defined(_WIN32) || defined(__WIN32__) || defined(__NT__)
+#if defined(_M_X64) || defined(__x86_64__)
+#include "crc32c_intel_sse4.c"
+#else
+#include "crc32c_sw.c"
+#endif
+
+#elif defined(__APPLE__) && defined(__MACH__)
 #if defined(_M_ARM64) || defined(__aarch64__) || defined(__arm64__)
 #include "crc32c_arm_neon.c"
-#elif defined(_M_AMD64) || defined(__amd64__)
-#include "crc32c_intel_sse4.c"
 #elif defined(_M_X64) || defined(__x86_64__)
 #include "crc32c_intel_sse4.c"
 #else
 #include "crc32c_sw.c"
 #endif
+
+#elif defined(__linux__) && __linux__
+#if defined(_M_X64) || defined(__x86_64__)
+#include "crc32c_intel_sse4.c"
+#else
+// Raspberry Pi 4 does not support CRC optimization.
+// Other Linux platforms may, but disable for now.
+#include "crc32c_sw.c"
+#endif
+
+#else
+#include "crc32c_sw.c"
+
+#endif
```

### Comparing `pyjls-0.7.1/src/crc32c_arm_neon.c` & `pyjls-0.7.2/src/crc32c_arm_neon.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/crc32c_intel_sse4.c` & `pyjls-0.7.2/src/crc32c_intel_sse4.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/crc32c_sw.c` & `pyjls-0.7.2/src/crc32c_sw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/datatype.c` & `pyjls-0.7.2/src/datatype.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/ec.c` & `pyjls-0.7.2/src/ec.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/log.c` & `pyjls-0.7.2/src/log.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/msg_ring_buffer.c` & `pyjls-0.7.2/src/msg_ring_buffer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/raw.c` & `pyjls-0.7.2/src/raw.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/rd_fsr.c` & `pyjls-0.7.2/src/rd_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/reader.c` & `pyjls-0.7.2/src/reader.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/statistics.c` & `pyjls-0.7.2/src/statistics.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/threaded_writer.c` & `pyjls-0.7.2/src/threaded_writer.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/wr_fsr.c` & `pyjls-0.7.2/src/wr_fsr.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/wr_ts.c` & `pyjls-0.7.2/src/wr_ts.c`

 * *Files identical despite different names*

### Comparing `pyjls-0.7.1/src/writer.c` & `pyjls-0.7.2/src/writer.c`

 * *Files identical despite different names*

