# Comparing `tmp/pure_ocean_breeze-3.9.6.tar.gz` & `tmp/pure_ocean_breeze-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_ocean_breeze-3.9.6.tar", last modified: Fri Jun  9 08:54:34 2023, max compression
+gzip compressed data, was "pure_ocean_breeze-3.9.7.tar", last modified: Wed Jun 14 02:31:01 2023, max compression
```

## Comparing `pure_ocean_breeze-3.9.6.tar` & `pure_ocean_breeze-3.9.7.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.108399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29570 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    65150 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    49382 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   227673 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.112399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.116399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/homeplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:54:34.108399 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 08:54:34.000000 pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:54:34.120399 pure_ocean_breeze-3.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-09 08:54:22.000000 pure_ocean_breeze-3.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31004 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67375 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49382 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   228266 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192825 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85655 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)   314704 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.341446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29395 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43178 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138094 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.345445 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29805 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   193541 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/homeplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.349446 pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 02:31:01.337445 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-14 02:31:01.000000 pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 02:31:01.353446 pure_ocean_breeze-3.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-14 02:30:51.000000 pure_ocean_breeze-3.9.7/setup.py
```

### Comparing `pure_ocean_breeze-3.9.6/LICENSE` & `pure_ocean_breeze-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/PKG-INFO` & `pure_ocean_breeze-3.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure_ocean_breeze
-Version: 3.9.6
+Version: 3.9.7
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.6/README.md` & `pure_ocean_breeze-3.9.7/README.md`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/__init__.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 一个量化多因子研究的框架，包含数据、回测、因子加工等方面的功能
 """
 
-__updated__ = "2023-05-18 18:47:05"
-__version__ = "3.9.6"
+__updated__ = "2023-06-10 21:02:21"
+__version__ = "3.9.7"
 __author__ = "chenzongwei"
 __author_email__ = "winterwinter999@163.com"
 __url__ = "https://github.com/chen-001/pure_ocean_breeze"
 __all__ = [
     "data",
     "labor",
     "state",
```

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/database.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/dicts.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/read_data.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/read_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-05-09 15:39:34"
+__updated__ = "2023-06-14 09:06:36"
 
 import os
 import numpy as np
 import pandas as pd
 import datetime
 from typing import Union, Dict, Tuple
 from loguru import logger
@@ -56,15 +56,15 @@
     stop_down: bool = 0,
     zxindustry_dummy_code: bool = 0,
     zxindustry_dummy_name: bool = 0,
     swindustry_dummy: bool = 0,
     hs300_member_weight: bool = 0,
     zz500_member_weight: bool = 0,
     zz1000_member_weight: bool = 0,
-    start: Union[int,str] = STATES["START"],
+    start: Union[int, str] = STATES["START"],
 ) -> pd.DataFrame:
     """直接读取常用的量价读取日频数据，默认为复权价格，
     在 open,close,high,low,tr,sharenum,volume 中选择一个参数指定为1
 
     Parameters
     ----------
     path : str, optional
@@ -163,121 +163,159 @@
         open,close,high,low,tr,sharenum,volume 都为0时，将报错
     """
 
     if not unadjust:
         if path:
             return pd.read_parquet(homeplace.daily_data_file + path)
         elif open:
-            opens = pd.read_parquet(homeplace.daily_data_file + "opens.parquet")
+            opens = pd.read_parquet(
+                homeplace.daily_data_file + "opens.parquet"
+            ) * read_daily(state=1)
             df = opens
         elif close:
-            closes = pd.read_parquet(homeplace.daily_data_file + "closes.parquet")
+            closes = pd.read_parquet(
+                homeplace.daily_data_file + "closes.parquet"
+            ) * read_daily(state=1)
             df = closes
         elif high:
-            highs = pd.read_parquet(homeplace.daily_data_file + "highs.parquet")
+            highs = pd.read_parquet(
+                homeplace.daily_data_file + "highs.parquet"
+            ) * read_daily(state=1)
             df = highs
         elif low:
-            lows = pd.read_parquet(homeplace.daily_data_file + "lows.parquet")
+            lows = pd.read_parquet(
+                homeplace.daily_data_file + "lows.parquet"
+            ) * read_daily(state=1)
             df = lows
         elif vwap:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "vwaps.parquet"
-            ) * read_daily(adjfactor=1, start=start)
+            df = (
+                pd.read_parquet(homeplace.daily_data_file + "vwaps.parquet")
+                * read_daily(adjfactor=1, start=start)
+                * read_daily(state=1)
+            )
         elif tr:
-            trs = pd.read_parquet(homeplace.daily_data_file + "trs.parquet").replace(0,np.nan)
+            trs = pd.read_parquet(homeplace.daily_data_file + "trs.parquet").replace(
+                0, np.nan
+            ) * read_daily(state=1)
             df = trs
         elif sharenum:
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             df = sharenums
         elif total_sharenum:
             df = pd.read_parquet(homeplace.daily_data_file + "total_sharenums.parquet")
         elif amount:
-            volumes = pd.read_parquet(homeplace.daily_data_file + "amounts.parquet")
+            volumes = pd.read_parquet(
+                homeplace.daily_data_file + "amounts.parquet"
+            ) * read_daily(state=1)
             df = volumes
         elif money:
             df = pd.read_parquet(
                 homeplace.factor_data_file + "日频数据-每日成交额/每日成交额.parquet"
             )
         elif age:
             age = pd.read_parquet(homeplace.daily_data_file + "ages.parquet")
             df = age
         elif flow_cap:
-            closes = pd.read_parquet(homeplace.daily_data_file + "closes_unadj.parquet")
+            closes = pd.read_parquet(
+                homeplace.daily_data_file + "closes_unadj.parquet"
+            ) * read_daily(state=1)
             sharenums = pd.read_parquet(homeplace.daily_data_file + "sharenums.parquet")
             flow_cap = closes * sharenums
             df = flow_cap
         elif total_cap:
-            closes = pd.read_parquet(homeplace.daily_data_file + "closes_unadj.parquet")
+            closes = pd.read_parquet(
+                homeplace.daily_data_file + "closes_unadj.parquet"
+            ) * read_daily(state=1)
             sharenums = pd.read_parquet(
                 homeplace.daily_data_file + "total_sharenums.parquet"
             )
             flow_cap = closes * sharenums
             df = flow_cap
         elif adjfactor:
             # df=pd.read_parquet(homeplace.daily_data_file+'adjfactors.parquet')
-            df = read_daily(close=1, start=start) / read_daily(
-                close=1, start=start, unadjust=1
+            df = (
+                read_daily(close=1, start=start)
+                * read_daily(state=1)
+                / read_daily(close=1, start=start, unadjust=1)
+                * read_daily(state=1)
             )
         elif st:
             st = pd.read_parquet(homeplace.daily_data_file + "sts.parquet")
             df = st
         elif state:
             state = pd.read_parquet(homeplace.daily_data_file + "states.parquet")
+            state = state.where(state == 1, np.nan)
             df = state
         elif ret:
             df = read_daily(close=1, start=start)
             df = df / df.shift(1) - 1
         elif ret_inday:
             df = read_daily(close=1, start=start) / read_daily(open=1, start=start) - 1
         elif ret_night:
             df = (
                 read_daily(open=1, start=start)
                 / read_daily(close=1, start=start).shift(1)
                 - 1
             )
         elif vol_daily:
-            df = pd.read_parquet(homeplace.factor_data_file + "草木皆兵/草木皆兵_初级.parquet")
+            df = pd.read_parquet(
+                homeplace.factor_data_file + "草木皆兵/草木皆兵_初级.parquet"
+            ) * read_daily(state=1)
         elif vol:
             df = read_daily(ret=1, start=start)
             df = df.rolling(20, min_periods=10).std()
         elif vol_inday:
             df = read_daily(ret_inday=1, start=start)
             df = df.rolling(20, min_periods=10).std()
         elif vol_night:
             df = read_daily(ret_night=1, start=start)
             df = df.rolling(20, min_periods=10).std()
         elif swing:
             df = (
                 read_daily(high=1, start=start) - read_daily(low=1, start=start)
             ) / read_daily(close=1, start=start)
         elif pb:
-            df = pd.read_parquet(homeplace.daily_data_file + "pb.parquet")
+            df = pd.read_parquet(homeplace.daily_data_file + "pb.parquet") * read_daily(
+                state=1
+            )
         elif pe:
-            df = pd.read_parquet(homeplace.daily_data_file + "pe.parquet")
+            df = pd.read_parquet(homeplace.daily_data_file + "pe.parquet") * read_daily(
+                state=1
+            )
         elif iret:
             df = pd.read_parquet(
                 homeplace.daily_data_file + "idiosyncratic_ret.parquet"
-            )
+            ) * read_daily(state=1)
         elif ivol:
             df = read_daily(iret=1, start=start)
             df = df.rolling(20, min_periods=10).std()
         elif illiquidity:
-            df = pd.read_parquet(homeplace.daily_data_file + "illiquidity.parquet")
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "illiquidity.parquet"
+            ) * read_daily(state=1)
         elif swindustry_ret:
-            df = pd.read_parquet(homeplace.daily_data_file + "股票对应申万一级行业每日收益率.parquet")
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "股票对应申万一级行业每日收益率.parquet"
+            ) * read_daily(state=1)
         elif zxindustry_ret:
-            df = pd.read_parquet(homeplace.daily_data_file + "股票对应中信一级行业每日收益率.parquet")
-        elif stop_up:
             df = pd.read_parquet(
-                homeplace.daily_data_file + "stop_ups.parquet"
-            ) * read_daily(adjfactor=1, start=start)
+                homeplace.daily_data_file + "股票对应中信一级行业每日收益率.parquet"
+            ) * read_daily(state=1)
+        elif stop_up:
+            df = (
+                pd.read_parquet(homeplace.daily_data_file + "stop_ups.parquet")
+                * read_daily(adjfactor=1, start=start)
+                * read_daily(state=1)
+            )
         elif stop_down:
-            df = pd.read_parquet(
-                homeplace.daily_data_file + "stop_downs.parquet"
-            ) * read_daily(adjfactor=1, start=start)
+            df = (
+                pd.read_parquet(homeplace.daily_data_file + "stop_downs.parquet")
+                * read_daily(adjfactor=1, start=start)
+                * read_daily(state=1)
+            )
         elif zxindustry_dummy_code:
             df = pd.read_parquet(homeplace.daily_data_file + "中信一级行业哑变量代码版.parquet")
         elif zxindustry_dummy_name:
             df = pd.read_parquet(homeplace.daily_data_file + "中信一级行业哑变量名称版.parquet")
         elif swindustry_dummy:
             df = pd.read_parquet(homeplace.daily_data_file + "申万行业2021版哑变量.parquet")
         elif hs300_member_weight:
@@ -298,31 +336,45 @@
                 .resample("M")
                 .last()
             )
         else:
             raise IOError("阁下总得读点什么吧？🤒")
     else:
         if open:
-            opens = pd.read_parquet(homeplace.daily_data_file + "opens_unadj.parquet")
+            opens = pd.read_parquet(
+                homeplace.daily_data_file + "opens_unadj.parquet"
+            ) * read_daily(state=1)
             df = opens
         elif close:
-            closes = pd.read_parquet(homeplace.daily_data_file + "closes_unadj.parquet")
+            closes = pd.read_parquet(
+                homeplace.daily_data_file + "closes_unadj.parquet"
+            ) * read_daily(state=1)
             df = closes
         elif high:
-            highs = pd.read_parquet(homeplace.daily_data_file + "highs_unadj.parquet")
+            highs = pd.read_parquet(
+                homeplace.daily_data_file + "highs_unadj.parquet"
+            ) * read_daily(state=1)
             df = highs
         elif low:
-            lows = pd.read_parquet(homeplace.daily_data_file + "lows_unadj.parquet")
+            lows = pd.read_parquet(
+                homeplace.daily_data_file + "lows_unadj.parquet"
+            ) * read_daily(state=1)
             df = lows
         elif vwap:
-            df = pd.read_parquet(homeplace.daily_data_file + "vwaps.parquet")
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "vwaps.parquet"
+            ) * read_daily(state=1)
         elif stop_up:
-            df = pd.read_parquet(homeplace.daily_data_file + "stop_ups.parquet")
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "stop_ups.parquet"
+            ) * read_daily(state=1)
         elif stop_down:
-            df = pd.read_parquet(homeplace.daily_data_file + "stop_downs.parquet")
+            df = pd.read_parquet(
+                homeplace.daily_data_file + "stop_downs.parquet"
+            ) * read_daily(state=1)
         else:
             raise IOError("阁下总得读点什么吧？🤒")
     if "date" not in df.columns:
         df = df[df.index >= pd.Timestamp(str(start))]
     return df.dropna(how="all")
 
 
@@ -330,15 +382,15 @@
     open: bool = 0,
     close: bool = 0,
     high: bool = 0,
     low: bool = 0,
     start: int = STATES["START"],
     every_stock: bool = 1,
     market_code: str = "000985.SH",
-    questdb_host: str = '127.0.0.1',
+    questdb_host: str = "127.0.0.1",
 ) -> Union[pd.DataFrame, pd.Series]:
     """读取中证全指日行情数据
 
     Parameters
     ----------
     open : bool, optional
         读取开盘点数, by default 0
@@ -378,15 +430,15 @@
     except Exception:
         try:
             qdb = Questdb(host=questdb_host)
             df = qdb.get_data(
                 f"select date,num,close,high,low from minute_data_index where code='{market_code}' and cast(date as int)>={start}"
             )
         except Exception:
-            qdb = Questdb(host='192.168.1.3')
+            qdb = Questdb(host="192.168.1.3")
             df = qdb.get_data(
                 f"select date,num,close,high,low from minute_data_index where code='{market_code}' and cast(date as int)>={start}"
             )
         df.num = df.num.astype(int)
     df = df.set_index("date")
     df.index = pd.to_datetime(df.index.astype(str), format="%Y%m%d")
     if open:
@@ -492,15 +544,15 @@
                 "sell_value_small",
             ]
         ]
         dfs = sum(dfs)
         return dfs
 
 
-def read_index_single(code: str,questdb_host:str='127.0.0.1') -> pd.Series:
+def read_index_single(code: str, questdb_host: str = "127.0.0.1") -> pd.Series:
     """读取某个指数的日行情收盘价数据
 
     Parameters
     ----------
     code : str
         指数的wind代码
     questdb_host: str, optional
@@ -531,15 +583,15 @@
     except Exception:
         try:
             qdb = Questdb(host=questdb_host)
             hs300 = qdb.get_data(
                 f"select date,num,close FROM 'minute_data_index' WHERE code='{code}'"
             )
         except Exception:
-            qdb = Questdb(host='192.168.1.3')
+            qdb = Questdb(host="192.168.1.3")
             hs300 = qdb.get_data(
                 f"select date,num,close FROM 'minute_data_index' WHERE code='{code}'"
             )
         hs300.date = pd.to_datetime(hs300.date, format="%Y%m%d")
         hs300.num = hs300.num.astype(int)
         hs300 = (
             hs300.sort_values(["date", "num"])
```

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/tools.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 针对一些不常见的文件格式，读取数据文件的一些工具函数，以及其他数据工具
 """
 
-__updated__ = "2023-06-09 16:44:30"
+__updated__ = "2023-06-14 00:08:18"
 
 import os
 import pandas as pd
 import tqdm.auto
 import datetime
 import scipy.io as scio
 import numpy as np
@@ -23,14 +23,15 @@
     rqdatac.init()
 except Exception:
     print("暂时未连接米筐")
 from pure_ocean_breeze.state.homeplace import HomePlace
 import deprecation
 from pure_ocean_breeze import __version__
 from pure_ocean_breeze.state.decorators import do_on_dfs
+
 try:
     homeplace = HomePlace()
 except Exception:
     print("您暂未初始化，功能将受限")
 
 
 def is_notebook() -> bool:
@@ -576,17 +577,21 @@
                         fac = self.fac[self.fac.date > new_date]
                         iter_item = [i for i in iter_item if i > new_date]
                         if whole_cross:
                             for end_date in tqdm.auto.tqdm(iter_item):
                                 start_date = self.find_begin(
                                     self.tradedays, end_date, self.backsee
                                 )
-                                df = fac[
-                                    (fac.date >= start_date) & (fac.date <= end_date)
-                                ]
+                                if start_date < end_date:
+                                    df = self.fac[
+                                        (self.fac.date >= start_date)
+                                        & (self.fac.date <= end_date)
+                                    ]
+                                else:
+                                    df = self.fac[self.fac.date <= end_date]
                                 df = func(df)
                                 df = df.to_frame().T
                                 df.index = [end_date]
                                 res.append(df)
                             fac = pd.concat(res).resample("M").last()
                             self.fac = pd.concat([old, fac])
                         else:
@@ -614,17 +619,21 @@
             else:
                 logger.info("第一次计算，请耐心等待……")
                 if whole_cross:
                     for end_date in tqdm.auto.tqdm(iter_item):
                         start_date = self.find_begin(
                             self.tradedays, end_date, self.backsee
                         )
-                        df = self.fac[
-                            (self.fac.date >= start_date) & (self.fac.date <= end_date)
-                        ]
+                        if start_date < end_date:
+                            df = self.fac[
+                                (self.fac.date >= start_date)
+                                & (self.fac.date <= end_date)
+                            ]
+                        else:
+                            df = self.fac[self.fac.date <= end_date]
                         df = func(df)
                         df = df.to_frame().T
                         df.index = [end_date]
                         res.append(df)
                     self.fac = pd.concat(res).resample("M").last()
                 else:
                     tqdm.auto.tqdm.pandas(
@@ -648,17 +657,20 @@
         else:
             logger.warning("您本次计算没有指定任何本地文件路径，这很可能会导致大量的重复计算和不必要的时间浪费，请注意！")
             if daily:
                 logger.warning("您指定的是日频计算，非月频计算，因此强烈建议您指定history_file参数！！")
             if whole_cross:
                 for end_date in tqdm.auto.tqdm(iter_item):
                     start_date = self.find_begin(self.tradedays, end_date, self.backsee)
-                    df = self.fac[
-                        (self.fac.date >= start_date) & (self.fac.date <= end_date)
-                    ]
+                    if start_date < end_date:
+                        df = self.fac[
+                            (self.fac.date >= start_date) & (self.fac.date <= end_date)
+                        ]
+                    else:
+                        df = self.fac[self.fac.date <= end_date]
                     df = func(df)
                     df = df.to_frame().T
                     df.index = [end_date]
                     res.append(df)
                 self.fac = pd.concat(res).resample("M").last()
             else:
                 tqdm.auto.tqdm.pandas(
@@ -705,22 +717,23 @@
         self.backsee = backsee
         self.get_fac_long_and_tradedays()
         self.get_month_starts_and_ends(backsee=backsee)
         self.get_monthly_factor(
             func, whole_cross=whole_cross, daily=daily, history_file=history_file
         )
 
+
 def corr_two_daily(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     history: str = None,
     rolling_window: int = 20,
     n_jobs: int = 1,
     daily: bool = 1,
-    method: str = 'pearson',
+    method: str = "pearson",
 ) -> pd.DataFrame:
     """求两个因子，在相同股票上，时序上滚动窗口下的相关系数
 
     Parameters
     ----------
     df1 : pd.DataFrame
         第一个因子，index为时间，columns为股票代码
@@ -739,57 +752,63 @@
 
     Returns
     -------
     pd.DataFrame
         相关系数后的结果，index为时间，columns为股票代码
     """
     if daily:
-        if method=='pearson':
+        if method == "pearson":
+
             def corr_in(a, b, c):
                 return c.iloc[-1], np.corrcoef(a, b)[0, 1]
 
             return func_two_daily(
                 df1=df1,
                 df2=df2,
                 func=corr_in,
                 history=history,
                 rolling_window=rolling_window,
                 n_jobs=n_jobs,
             )
-        elif method=='spearman':
+        elif method == "spearman":
+
             def corr_in(a, b, c):
                 return c.iloc[-1], np.corrcoef(np.argsort(a), np.argsort(b))[0, 1]
 
             return func_two_daily(
                 df1=df1,
                 df2=df2,
                 func=corr_in,
                 history=history,
                 rolling_window=rolling_window,
                 n_jobs=n_jobs,
             )
         else:
-            raise ValueError('您输入的方法暂不支持')
+            raise ValueError("您输入的方法暂不支持")
     else:
-        if method=='pearson':
+        if method == "pearson":
+
             class Cut(pure_dawn):
-                def cut(self,df:pd.DataFrame):
-                    return df[['fac1','fac2']].corr().iloc[0,1]
-            cut=Cut(df1,df2)
-            cut.run(cut.cut,backsee=rolling_window,history_file=history)
+                def cut(self, df: pd.DataFrame):
+                    return df[["fac1", "fac2"]].corr().iloc[0, 1]
+
+            cut = Cut(df1, df2)
+            cut.run(cut.cut, backsee=rolling_window, history_file=history)
             return cut()
-        elif method=='spearman':
+        elif method == "spearman":
+
             class Cut(pure_dawn):
-                def cut(self,df:pd.DataFrame):
-                    return df[['fac1','fac2']].rank().corr().iloc[0,1]
-            cut=Cut(df1,df2)
-            cut.run(cut.cut,backsee=rolling_window,history_file=history)
+                def cut(self, df: pd.DataFrame):
+                    return df[["fac1", "fac2"]].rank().corr().iloc[0, 1]
+
+            cut = Cut(df1, df2)
+            cut.run(cut.cut, backsee=rolling_window, history_file=history)
             return cut()
         else:
-            raise ValueError('您输入的方法暂不支持')
+            raise ValueError("您输入的方法暂不支持")
 
 
 def cov_two_daily(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     history: str = None,
     rolling_window: int = 20,
@@ -815,31 +834,34 @@
 
     Returns
     -------
     pd.DataFrame
         求协方差后的结果，index为时间，columns为股票代码
     """
     if daily:
+
         def cov_in(a, b, c):
             return c.iloc[-1], np.cov(a, b)[0, 1]
 
         return func_two_daily(
             df1=df1,
             df2=df2,
             func=cov_in,
             history=history,
             rolling_window=rolling_window,
             n_jobs=n_jobs,
         )
     else:
+
         class Cut(pure_dawn):
-            def cut(self,df:pd.DataFrame):
-                return df[['fac1','fac2']].cov().iloc[0,1]
-        cut=Cut(df1,df2)
-        cut.run(cut.cut,backsee=rolling_window,history_file=history)
+            def cut(self, df: pd.DataFrame):
+                return df[["fac1", "fac2"]].cov().iloc[0, 1]
+
+        cut = Cut(df1, df2)
+        cut.run(cut.cut, backsee=rolling_window, history_file=history)
         return cut()
 
 
 def func_two_daily(
     df1: pd.DataFrame,
     df2: pd.DataFrame,
     func: Callable,
@@ -1853,25 +1875,65 @@
     pd.DataFrame
         变化后非负的因子值
     """
     return (df.T - df.T.min()).T
 
 
 @do_on_dfs
-def clip_mad(df: pd.DataFrame, n: float = 3, replace: bool = 1) -> pd.DataFrame:
-    def clip_sing(x: pd.Series, n: float = 3):
-        median = x.quantile(0.5)
-        diff_median = ((x - median).abs()).quantile(0.5)
-        max_range = median + n * diff_median
-        min_range = median - n * diff_median
-        x = x.where(x < max_range, max_range)
-        x = x.where(x > min_range, min_range)
-        return x
+def clip_mad(
+    df: pd.DataFrame, n: float = 3, replace: bool = 1, keep_trend: bool = 1
+) -> pd.DataFrame:
+    if keep_trend:
+        df = df.stack().reset_index()
+        df.columns = ["date", "code", "fac"]
+
+        def clip_sing(x: pd.DataFrame, n: float = 3):
+            median = x.fac.quantile(0.5)
+            diff_median = ((x.fac - median).abs()).quantile(0.5)
+            max_range1 = median + n * diff_median
+            min_range1 = median - n * diff_median
+            max_range2 = median + (n + 0.5) * diff_median
+            min_range2 = median - (n + 0.5) * diff_median
+            x = x.sort_values(["fac"])
+            x_min = x[x.fac <= min_range1]
+            x_max = x[x.fac >= max_range1]
+            x_middle = x[(x.fac > min_range1) & (x.fac < max_range1)]
+            x_min.fac = np.nan
+            x_max.fac = np.nan
+            if x_min.shape[0] >= 1:
+                x_min.fac.iloc[-1] = min_range1
+                if x_min.shape[0] >= 2:
+                    x_min.fac.iloc[0] = min_range2
+                    x_min.fac = x_min.fac.interpolate()
+            if x_max.shape[0] >= 1:
+                x_max.fac.iloc[-1] = max_range2
+                if x_max.shape[0] >= 2:
+                    x_max.fac.iloc[0] = max_range1
+                    x_max.fac = x_max.fac.interpolate()
+            x = pd.concat([x_min, x_middle, x_max]).sort_values(["code"])
+            return x
+
+        df = df.groupby(["date"]).apply(lambda x: clip_sing(x, n))
+        try:
+            df = df.reset_index()
+        except Exception:
+            ...
+        df = df.pivot(index="date", columns="code", values="fac")
+        return df
+    elif replace:
+
+        def clip_sing(x: pd.Series, n: float = 3):
+            median = x.quantile(0.5)
+            diff_median = ((x - median).abs()).quantile(0.5)
+            max_range = median + n * diff_median
+            min_range = median - n * diff_median
+            x = x.where(x < max_range, max_range)
+            x = x.where(x > min_range, min_range)
+            return x
 
-    if replace:
         df1 = df.T.apply(lambda x: clip_sing(x, n)).T
         df = np.abs(np.sign(df)) * df1
         return df
     else:
         df0 = df.T
         median = df0.quantile(0.5)
         diff_median = ((df0 - median).abs()).quantile(0.5)
```

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/data/write_data.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/half_way.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/initialize/initialize.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/comment.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/labor/process.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/labor/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__updated__ = "2023-06-04 12:44:48"
+__updated__ = "2023-06-14 09:29:34"
 
 import warnings
 
 warnings.filterwarnings("ignore")
 import numpy as np
 import pandas as pd
 import knockknock as kk
@@ -1399,14 +1399,16 @@
         "__factors_out",
         "ics",
         "rankics",
         "factor_turnover_rates",
         "factor_turnover_rate",
         "group_rets_std",
         "group_rets_stds",
+        "group_rets_skews",
+        "group_rets_skew",
         "wind_out",
         "swindustry_dummy",
         "zxindustry_dummy",
         "closes2_monthly",
         "rets_monthly_last",
         "freq_ctrl",
         "freq",
@@ -1945,18 +1947,22 @@
             self.rets_all = self.data.groupby(["date"]).apply(in_g)
             self.group_rets_std = "市值加权暂未设置该功能，敬请期待🌙"
         else:
             self.group_rets = self.data.groupby(["date", "group"]).apply(
                 lambda x: x.ret.mean()
             )
             self.rets_all = self.data.groupby(["date"]).apply(lambda x: x.ret.mean())
-            self.group_rets_stds = self.data.groupby(["date", "group"]).apply(
-                lambda x: x.ret.std()
+            self.group_rets_stds = self.data.groupby(["date", "group"]).ret.std()
+            self.group_rets_std = (
+                self.group_rets_stds.reset_index().groupby("group").mean()
+            )
+            self.group_rets_skews = self.data.groupby(["date", "group"]).ret.skew()
+            self.group_rets_skew = (
+                self.group_rets_skews.reset_index().groupby("group").mean()
             )
-            self.group_rets_std = self.group_rets_stds.groupby("group").mean()
         # dropna是因为如果股票行情数据比因子数据的截止日期晚，而最后一个月发生月初跌停时，会造成最后某组多出一个月的数据
         self.group_rets = self.group_rets.unstack()
         self.group_rets = self.group_rets[
             self.group_rets.index <= self.factors.date.max()
         ]
         self.group_rets.columns = list(map(str, list(self.group_rets.columns)))
         self.group_rets = self.group_rets.add_prefix("group")
@@ -2816,15 +2822,15 @@
         """对回测的每年表现给出评价
 
         Returns
         -------
         pd.DataFrame
             各年度的收益率
         """
-        df = self.shen.group_net_values.resample("M").last().pct_change()
+        df = self.shen.group_net_values.resample("Y").last().pct_change()
         df.index = df.index.year
         return df
 
 
 class pure_week(pure_moon):
     ...
 
@@ -3530,14 +3536,20 @@
 
         def full_run(df, *args, **kwargs):
             res = func(df, *args, **kwargs)
             if isinstance(res, pd.Series):
                 res = res.reset_index()
                 res.columns = ["code", "fac"]
                 return res
+            elif isinstance(res, pd.DataFrame):
+                res.columns = [f"fac{i}" for i in range(len(res.columns))]
+                res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
+                res = res[["fac"]].reset_index()
+                res.columns = ["code", "fac"]
+                return res
             else:
                 res = pd.concat(res, axis=1)
                 res.columns = [f"fac{i}" for i in range(len(res.columns))]
                 res = res.assign(fac=list(zip(*[res[i] for i in list(res.columns)])))
                 res = res[["fac"]].reset_index()
                 res.columns = ["code", "fac"]
                 return res
@@ -3964,15 +3976,14 @@
         -------
         `pd.DataFrame`
             每个组的年化收益率
         """
         return self.square_rets.copy()
 
 
-
 @do_on_dfs
 def follow_tests(
     fac: pd.DataFrame,
     trade_cost_double_side_list: float = [0.001, 0.002, 0.003, 0.004, 0.005],
     index_member_value_weighted: bool = 1,
     comments_writer: pd.ExcelWriter = None,
     net_values_writer: pd.ExcelWriter = None,
```

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/initialize.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/initialize.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v1p10/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/initialize.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v2/pure_ocean_breeze.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/__init__.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/database.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/tools.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/labor/process.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/mail/email.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p1/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/__init__.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/database.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/database.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/dicts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/read_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/tools.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/tools.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/data/write_data.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/half_way.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/future_version/in_thoughts.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/comment.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/labor/process.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/labor/process.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/mail/email.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/state/states.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/legacy_version/v3p4/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/mail/email.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/mail/email.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/decorators.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/decorators.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/homeplace.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/homeplace.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/state/states.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/state/states.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze/withs/requires.py` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze/withs/requires.py`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/PKG-INFO` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-ocean-breeze
-Version: 3.9.6
+Version: 3.9.7
 Summary: stock factor test
 Home-page: https://github.com/chen-001/pure_ocean_breeze.git
 Author: chenzongwei
 Author-email: winterwinter999@163.com
 License: MIT
 Project-URL: Documentation, https://chen-001.github.io/pure_ocean_breeze/
 Requires-Python: >=3
```

### Comparing `pure_ocean_breeze-3.9.6/pure_ocean_breeze.egg-info/SOURCES.txt` & `pure_ocean_breeze-3.9.7/pure_ocean_breeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pure_ocean_breeze-3.9.6/setup.py` & `pure_ocean_breeze-3.9.7/setup.py`

 * *Files identical despite different names*

