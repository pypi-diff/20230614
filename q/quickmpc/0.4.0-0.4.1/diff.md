# Comparing `tmp/quickmpc-0.4.0.tar.gz` & `tmp/quickmpc-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-jwzx7ry0/quickmpc-0.4.0.tar", last modified: Thu Jun  8 06:09:02 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-alf_s202/quickmpc-0.4.1.tar", last modified: Wed Jun 14 04:09:09 2023, max compression
```

## Comparing `quickmpc-0.4.0.tar` & `quickmpc-0.4.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 06:08:46.000000 quickmpc-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 06:08:46.000000 quickmpc-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-08 06:08:46.000000 quickmpc-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 06:09:02.000000 quickmpc-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 06:08:46.000000 quickmpc-0.4.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-06-08 06:08:46.000000 quickmpc-0.4.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-08 06:08:46.000000 quickmpc-0.4.0/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 06:08:46.000000 quickmpc-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-08 06:08:46.000000 quickmpc-0.4.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 06:08:46.000000 quickmpc-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/qmpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/parse_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/utils/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 06:08:46.000000 quickmpc-0.4.0/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 06:09:02.000000 quickmpc-0.4.0/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 06:09:02.000000 quickmpc-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 06:08:46.000000 quickmpc-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/unit_tests/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server1.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server2.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server2.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server3.key
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/certificates/server3.pem
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:09:02.000000 quickmpc-0.4.0/tests/unit_tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tests/unit_tests/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-08 06:08:46.000000 quickmpc-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-14 04:08:49.000000 quickmpc-0.4.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-14 04:08:49.000000 quickmpc-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 04:08:49.000000 quickmpc-0.4.1/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-14 04:08:49.000000 quickmpc-0.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 04:08:49.000000 quickmpc-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 04:08:49.000000 quickmpc-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 04:09:09.000000 quickmpc-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-14 04:08:49.000000 quickmpc-0.4.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38604 2023-06-14 04:08:49.000000 quickmpc-0.4.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-14 04:08:49.000000 quickmpc-0.4.1/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-14 04:08:49.000000 quickmpc-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-14 04:08:49.000000 quickmpc-0.4.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-14 04:08:49.000000 quickmpc-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13392 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/qmpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/utils/parse_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-14 04:08:49.000000 quickmpc-0.4.1/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 04:09:09.000000 quickmpc-0.4.1/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-14 04:09:09.000000 quickmpc-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-14 04:08:49.000000 quickmpc-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/tests/unit_tests/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/certificates/server1.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/certificates/server1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/certificates/server2.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/certificates/server2.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/certificates/server3.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/certificates/server3.pem
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:09:09.000000 quickmpc-0.4.1/tests/unit_tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tests/unit_tests/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-14 04:08:49.000000 quickmpc-0.4.1/tox.ini
```

### Comparing `quickmpc-0.4.0/.vscode/settings.json` & `quickmpc-0.4.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/LICENSE` & `quickmpc-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/Pipfile.lock` & `quickmpc-0.4.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/README-ja.md` & `quickmpc-0.4.1/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/README.md` & `quickmpc-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/mypy.ini` & `quickmpc-0.4.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/README.md` & `quickmpc-0.4.1/quickmpc/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.py` & `quickmpc-0.4.1/quickmpc/proto/common_types/common_types_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-0.4.1/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.py` & `quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-0.4.1/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/qmpc.py` & `quickmpc-0.4.1/quickmpc/qmpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass, field, InitVar
 from typing import Dict, List, Optional, Tuple
 
 from .proto.common_types import common_types_pb2
 from .qmpc_server import QMPCServer
 from .share import Share
 from .utils.parse_csv import parse, parse_csv
-from .utils.restore import restore
+from .restore import restore
 
 logger = logging.getLogger(__name__)
 # qmpc.JobStatus でアクセスできるようにエイリアスを設定する
 JobStatus \
     = common_types_pb2.JobStatus
 ComputationMethod \
     = common_types_pb2.ComputationMethod
```

### Comparing `quickmpc-0.4.0/quickmpc/qmpc_server.py` & `quickmpc-0.4.1/quickmpc/qmpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     @staticmethod
     def __stream_result(stream: Iterable, job_uuid: str, party: int,
                         path: Optional[str]) -> Dict:
         """ エラーチェックしてstreamのresultを得る """
         is_ok: bool = True
         res_list = []
         for res in stream:
-            if path is not None:
+            if path and res.status == JobStatus.Value('COMPLETED'):
                 file_title = "dim1"
                 if res.HasField("is_dim2"):
                     file_title = "dim2"
                 elif res.HasField("is_schema"):
                     file_title = "schema"
 
                 file_path = f"{path}/" + \
```

### Comparing `quickmpc-0.4.0/quickmpc/share.py` & `quickmpc-0.4.1/quickmpc/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/utils/make_pieces.py` & `quickmpc-0.4.1/quickmpc/utils/make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/utils/overload_tools.py` & `quickmpc-0.4.1/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/utils/parse_csv.py` & `quickmpc-0.4.1/quickmpc/utils/parse_csv.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/utils/random.py` & `quickmpc-0.4.1/quickmpc/utils/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/quickmpc/utils/restore.py` & `quickmpc-0.4.1/quickmpc/restore.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import csv
 import glob
-from decimal import Decimal
 from typing import Any
 
 import numpy as np
 from natsort import natsorted
 
+import google.protobuf.json_format
+from .proto.common_types.common_types_pb2 import Schema
+from .share import Share
+from .utils.if_present import if_present
+
 
 def get_meta(job_uuid: str, path: str):
     file_name = glob.glob(f"{path}/dim?-{job_uuid}-*")[0]
     with open(file_name, 'r') as f:
         reader = csv.reader(f)
         # 1列目のデータを取得
         meta = next(reader)
@@ -24,34 +28,49 @@
             next(reader)
             for row in reader:
                 for val in row:
                     yield val
 
 
 def restore(job_uuid: str, path: str, party_size: int) -> Any:
-    schema = []
-    result: Any = []
-
     column_number = get_meta(job_uuid, path)
+
+    schema: Any = [None]*column_number
+    results: Any = []
+
+    is_schema = True if len(
+        glob.glob(f"{path}/schema-{job_uuid}-*")) != 0 else False
     is_dim2 = True if len(
         glob.glob(f"{path}/dim2-{job_uuid}-*")) != 0 else False
     if column_number == 0:
-        return [[]] if is_dim2 else []
+        if is_schema:
+            return {"schema": [], "table": [[]]}
+        elif is_dim2:
+            return [[]]
+        else:
+            return []
 
     for party in range(party_size):
         if party == 0:
-            for val in get_result(job_uuid, f"{path}/schema", party):
-                schema.append(val)
+            for i, val in enumerate(get_result(
+                                    job_uuid, f"{path}/schema", party)):
+                col_sch = google.protobuf.json_format.Parse(
+                    val, Schema())
+                schema[i] = col_sch
 
         itr = 0
         for val in get_result(job_uuid, f"{path}/dim?", party):
-            if itr >= len(result):
-                result.append(Decimal(val))
+            f = Share.get_pre_convert_func(schema[itr % column_number])
+            if itr >= len(results):
+                results.append(f(val))
             else:
-                result[itr] += Decimal(val)
+                results[itr] += f(val)
             itr += 1
-
-    result_float = np.vectorize(float)(result)
-    result = np.array(result_float)\
-        .reshape(-1, column_number).tolist() if is_dim2 else result_float
-    result = {"schema": schema, "table": result} if len(schema) else result
-    return result
+    results = np.array(results)\
+        .reshape(-1, column_number).tolist() if is_dim2 else results
+    if is_dim2 and len(results) == 0:
+        schema = []
+        results = [[]]
+
+    results = if_present(results, Share.convert_type, schema)
+    results = {"schema": schema, "table": results} if is_schema else results
+    return results
```

### Comparing `quickmpc-0.4.0/quickmpc.egg-info/SOURCES.txt` & `quickmpc-0.4.1/quickmpc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .vscode/settings.json
 quickmpc/README.md
 quickmpc/__init__.py
 quickmpc/_version.py
 quickmpc/exception.py
 quickmpc/qmpc.py
 quickmpc/qmpc_server.py
+quickmpc/restore.py
 quickmpc/share.py
 quickmpc/version.py
 quickmpc.egg-info/PKG-INFO
 quickmpc.egg-info/SOURCES.txt
 quickmpc.egg-info/dependency_links.txt
 quickmpc.egg-info/requires.txt
 quickmpc.egg-info/top_level.txt
@@ -37,15 +38,14 @@
 quickmpc/proto/common_types/common_types_pb2.pyi
 quickmpc/utils/__init__.py
 quickmpc/utils/if_present.py
 quickmpc/utils/make_pieces.py
 quickmpc/utils/overload_tools.py
 quickmpc/utils/parse_csv.py
 quickmpc/utils/random.py
-quickmpc/utils/restore.py
 tests/__init__.py
 tests/unit_tests/__init__.py
 tests/unit_tests/conftest.py
 tests/unit_tests/local_server.py
 tests/unit_tests/test_make_pieces.py
 tests/unit_tests/test_over_load.py
 tests/unit_tests/test_parse.py
```

### Comparing `quickmpc-0.4.0/tests/unit_tests/certificates/server1.key` & `quickmpc-0.4.1/tests/unit_tests/certificates/server1.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/certificates/server1.pem` & `quickmpc-0.4.1/tests/unit_tests/certificates/server1.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/certificates/server2.key` & `quickmpc-0.4.1/tests/unit_tests/certificates/server2.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/certificates/server2.pem` & `quickmpc-0.4.1/tests/unit_tests/certificates/server2.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/certificates/server3.key` & `quickmpc-0.4.1/tests/unit_tests/certificates/server3.key`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/certificates/server3.pem` & `quickmpc-0.4.1/tests/unit_tests/certificates/server3.pem`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/conftest.py` & `quickmpc-0.4.1/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/local_server.py` & `quickmpc-0.4.1/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_files/edge_data.csv` & `quickmpc-0.4.1/tests/unit_tests/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_files/string_data.csv` & `quickmpc-0.4.1/tests/unit_tests/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_make_pieces.py` & `quickmpc-0.4.1/tests/unit_tests/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_over_load.py` & `quickmpc-0.4.1/tests/unit_tests/test_over_load.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_parse.py` & `quickmpc-0.4.1/tests/unit_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_qmpc.py` & `quickmpc-0.4.1/tests/unit_tests/test_qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_random.py` & `quickmpc-0.4.1/tests/unit_tests/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_restore.py` & `quickmpc-0.4.1/tests/unit_tests/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_share_recons.py` & `quickmpc-0.4.1/tests/unit_tests/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.4.0/tests/unit_tests/test_share_sharize.py` & `quickmpc-0.4.1/tests/unit_tests/test_share_sharize.py`

 * *Files identical despite different names*

