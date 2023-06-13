# Comparing `tmp/aiomqtt-0.1.3.tar.gz` & `tmp/aiomqtt-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomqtt-0.1.3.tar", last modified: Sat May 22 19:14:41 2021, max compression
+gzip compressed data, was "aiomqtt-0.17.0.tar", max compression
```

## Comparing `aiomqtt-0.1.3.tar` & `aiomqtt-0.17.0.tar`

### file list

```diff
@@ -1,15 +1,9 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-05-22 19:14:41.232931 aiomqtt-0.1.3/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      736 2021-05-22 19:14:41.232931 aiomqtt-0.1.3/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2595 2021-03-07 09:45:58.000000 aiomqtt-0.1.3/README.md
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-05-22 19:14:41.232931 aiomqtt-0.1.3/aiomqtt/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      150 2017-07-13 06:33:33.000000 aiomqtt-0.1.3/aiomqtt/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3971 2017-07-13 06:38:01.000000 aiomqtt-0.1.3/aiomqtt/client.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       22 2021-05-22 19:13:30.000000 aiomqtt-0.1.3/aiomqtt/version.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-05-22 19:14:41.232931 aiomqtt-0.1.3/aiomqtt.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      736 2021-05-22 19:14:41.000000 aiomqtt-0.1.3/aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      229 2021-05-22 19:14:41.000000 aiomqtt-0.1.3/aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2021-05-22 19:14:41.000000 aiomqtt-0.1.3/aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       17 2021-05-22 19:14:41.000000 aiomqtt-0.1.3/aiomqtt.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        8 2021-05-22 19:14:41.000000 aiomqtt-0.1.3/aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2021-05-22 19:14:41.232931 aiomqtt-0.1.3/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      981 2018-07-22 15:47:58.000000 aiomqtt-0.1.3/setup.py
+-rw-r--r--   0        0        0     1464 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/LICENSE
+-rw-r--r--   0        0        0     7163 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/README.md
+-rw-r--r--   0        0        0      529 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/__init__.py
+-rw-r--r--   0        0        0    35189 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/client.py
+-rw-r--r--   0        0        0     1686 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/error.py
+-rw-r--r--   0        0        0        0 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/py.typed
+-rw-r--r--   0        0        0      245 2023-06-13 23:44:58.901558 aiomqtt-0.17.0/aiomqtt/types.py
+-rw-r--r--   0        0        0     4801 2023-06-13 23:45:22.397765 aiomqtt-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     8370 1970-01-01 00:00:00.000000 aiomqtt-0.17.0/PKG-INFO
```

