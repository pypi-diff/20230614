# Comparing `tmp/computex_cli-0.1.0.tar.gz` & `tmp/computex_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.0.tar", max compression
+gzip compressed data, was "computex_cli-0.1.1.tar", max compression
```

## Comparing `computex_cli-0.1.0.tar` & `computex_cli-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0      392 2023-06-08 18:28:28.160718 computex_cli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-08 18:28:28.160718 computex_cli-0.1.0/cxcli/__init__.py
--rw-r--r--   0        0        0      767 2023-06-08 18:28:28.160718 computex_cli-0.1.0/cxcli/cli.py
--rw-r--r--   0        0        0      757 2023-06-08 18:28:28.164718 computex_cli-0.1.0/cxcli/config.py
--rw-r--r--   0        0        0      416 2023-06-08 18:28:28.164718 computex_cli-0.1.0/cxcli/service.py
--rw-r--r--   0        0        0      579 2023-06-08 18:28:28.164718 computex_cli-0.1.0/cxcli/users.py
--rw-r--r--   0        0        0      446 2023-06-08 18:48:40.820391 computex_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 computex_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      613 2023-06-13 21:08:54.631293 computex_cli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 13:32:24.984013 computex_cli-0.1.1/cxcli/__init__.py
+-rw-r--r--   0        0        0     6202 2023-06-14 13:56:13.757403 computex_cli-0.1.1/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-06-13 21:08:54.632830 computex_cli-0.1.1/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-06-13 21:08:54.633286 computex_cli-0.1.1/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:08:54.633381 computex_cli-0.1.1/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-13 21:08:54.634140 computex_cli-0.1.1/cxcli/services/auth.py
+-rw-r--r--   0        0        0     1485 2023-06-13 21:08:54.634576 computex_cli-0.1.1/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-06-13 21:08:54.635101 computex_cli-0.1.1/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-06-13 21:08:54.635947 computex_cli-0.1.1/cxcli/services/users.py
+-rw-r--r--   0        0        0      727 2023-06-14 13:58:16.104380 computex_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 computex_cli-0.1.1/PKG-INFO
```

