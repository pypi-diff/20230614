# Comparing `tmp/m-abac-test-1.0.8.tar.gz` & `tmp/m-abac-test-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-test-1.0.8.tar", last modified: Tue Jun 13 08:41:52 2023, max compression
+gzip compressed data, was "m-abac-test-1.0.9.tar", last modified: Wed Jun 14 06:37:25 2023, max compression
```

## Comparing `m-abac-test-1.0.8.tar` & `m-abac-test-1.0.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.124431 m-abac-test-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-13 08:41:52.123431 m-abac-test-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.067430 m-abac-test-1.0.8/m_abac_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3851 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.056429 m-abac-test-1.0.8/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.057429 m-abac-test-1.0.8/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.071430 m-abac-test-1.0.8/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.073430 m-abac-test-1.0.8/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7967 2023-06-13 08:40:33.000000 m-abac-test-1.0.8/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.8/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    16098 2023-06-13 08:40:33.000000 m-abac-test-1.0.8/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.076430 m-abac-test-1.0.8/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.077430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.079430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.086430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      418 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_contains.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.092430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.097431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.100431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.105431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.108431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.121431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6055 2023-06-12 11:10:01.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-06-12 11:10:01.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-06-12 11:10:01.000000 m-abac-test-1.0.8/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 08:41:52.124431 m-abac-test-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9779 2023-06-13 08:41:50.000000 m-abac-test-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.840135 m-abac-test-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-06-14 06:37:25.839136 m-abac-test-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.783134 m-abac-test-1.0.9/m_abac_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-06-14 06:37:25.000000 m-abac-test-1.0.9/m_abac_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-14 06:37:25.000000 m-abac-test-1.0.9/m_abac_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 06:37:25.000000 m-abac-test-1.0.9/m_abac_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-14 06:37:25.000000 m-abac-test-1.0.9/m_abac_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-14 06:37:25.000000 m-abac-test-1.0.9/m_abac_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.772134 m-abac-test-1.0.9/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.773134 m-abac-test-1.0.9/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.787134 m-abac-test-1.0.9/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.788134 m-abac-test-1.0.9/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-06-14 05:04:55.000000 m-abac-test-1.0.9/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-06-14 05:04:55.000000 m-abac-test-1.0.9/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-06-14 05:04:55.000000 m-abac-test-1.0.9/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.791134 m-abac-test-1.0.9/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.793134 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.795134 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.803135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.810135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.817135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.820135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.825135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.828135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 06:37:25.838135 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-06-12 07:41:39.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-06-12 11:10:01.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2023-06-14 05:04:55.000000 m-abac-test-1.0.9/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-06-14 05:04:55.000000 m-abac-test-1.0.9/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 06:37:25.840135 m-abac-test-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9779 2023-06-14 06:37:25.000000 m-abac-test-1.0.9/setup.py
```

### Comparing `m-abac-test-1.0.8/PKG-INFO` & `m-abac-test-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ### ABAC Engine
-        Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install m-abac
-         ```
-        
-        ### Sử dụng:
-        
-        ##### Kiểm tra user có quyền thao tác hay không:
-           ```python
-            from mobio.libs.abac import PolicyDecisionPoint
-            resource = "deal"
-            # action = "UpdateFromSale"
-            action = "ListFromSale"
-        
-            pdb = PolicyDecisionPoint(resource=resource, action=action)
-            result = pdb.is_allowed()
-            if not result.get_allow_access():
-                # trả về lỗi không có quyền truy cập 
-           ```
-        #### Log - 1.0.0
-            - release sdk
-            
 Keywords: mobio,mobio-engine,m-abac
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+### ABAC Engine
+Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
+
+
+### Cài đặt:
+```bash
+ $ pip3 install m-abac
+ ```
+
+### Sử dụng:
+
+##### Kiểm tra user có quyền thao tác hay không:
+   ```python
+    from mobio.libs.abac import PolicyDecisionPoint
+    resource = "deal"
+    # action = "UpdateFromSale"
+    action = "ListFromSale"
+
+    pdb = PolicyDecisionPoint(resource=resource, action=action)
+    result = pdb.is_allowed()
+    if not result.get_allow_access():
+        # trả về lỗi không có quyền truy cập 
+   ```
+#### Log - 1.0.0
+    - release sdk
+
```

### Comparing `m-abac-test-1.0.8/README.md` & `m-abac-test-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/m_abac_test.egg-info/PKG-INFO` & `m-abac-test-1.0.9/m_abac_test.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.8
+Version: 1.0.9
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
-Description: ### ABAC Engine
-        Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
-        
-        
-        ### Cài đặt:
-        ```bash
-         $ pip3 install m-abac
-         ```
-        
-        ### Sử dụng:
-        
-        ##### Kiểm tra user có quyền thao tác hay không:
-           ```python
-            from mobio.libs.abac import PolicyDecisionPoint
-            resource = "deal"
-            # action = "UpdateFromSale"
-            action = "ListFromSale"
-        
-            pdb = PolicyDecisionPoint(resource=resource, action=action)
-            result = pdb.is_allowed()
-            if not result.get_allow_access():
-                # trả về lỗi không có quyền truy cập 
-           ```
-        #### Log - 1.0.0
-            - release sdk
-            
 Keywords: mobio,mobio-engine,m-abac
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+
+### ABAC Engine
+Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control).
+
+
+### Cài đặt:
+```bash
+ $ pip3 install m-abac
+ ```
+
+### Sử dụng:
+
+##### Kiểm tra user có quyền thao tác hay không:
+   ```python
+    from mobio.libs.abac import PolicyDecisionPoint
+    resource = "deal"
+    # action = "UpdateFromSale"
+    action = "ListFromSale"
+
+    pdb = PolicyDecisionPoint(resource=resource, action=action)
+    result = pdb.is_allowed()
+    if not result.get_allow_access():
+        # trả về lỗi không có quyền truy cập 
+   ```
+#### Log - 1.0.0
+    - release sdk
+
```

### Comparing `m-abac-test-1.0.8/m_abac_test.egg-info/SOURCES.txt` & `m-abac-test-1.0.9/m_abac_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-test-1.0.9/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/call_api.py` & `m-abac-test-1.0.9/mobio/libs/abac/call_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,16 @@
                 },
                 timeout=APIRequest.TimeOut,
             )
             data = None
             if data_res.status_code == 200:
                 if data_res.json().get("statements"):
                     data = data_res.json().get("statements")
-            # print("abac_sdk admin_get_list_statement: {}".format(data))
+            # TODO: comment log khi len prod
+            print("abac_sdk admin_get_list_statement: {}".format(data))
             return data
 
             # return [
             #     {
             #         "effect": "allow",
             #         "action": [
             #             "ListFromSale"
```

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/config.py` & `m-abac-test-1.0.9/mobio/libs/abac/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import redis
-
 from mobio.libs.Singleton import Singleton
 from mobio.libs.caching import LruCache
+# from mobio.libs.logging import MobioLogging
 
 
 class StoreCacheType:
     LOCAL = 1
     REDIS = 2
 
 
@@ -17,14 +17,15 @@
 
 lru_cache_redis = LruCache(
     store_type=StoreCacheType.REDIS,
     redis_uri=Cache.REDIS_URI,
     cache_prefix=Cache.PREFIX,
 )
 
+# mobio_log = MobioLogging()
 
 class Mobio:
     ADMIN_HOST = os.environ.get("ADMIN_HOST")
     MOBIO_TOKEN = "Basic {}".format(os.environ.get('YEK_REWOP', ''))
 
 
 @Singleton
```

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/pdp.py` & `m-abac-test-1.0.9/mobio/libs/abac/pdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,18 @@
     # TODO: bo su dung ham nay tren production
     @classmethod
     def check_merchant_use_abac(cls, merchant_id):
         use_abac = False
         data_cache = RedisClient().get_value(RedisClient.KeyCache.MERCHANT_USE_ABAC)
         if data_cache:
             data_merchant = str(data_cache.decode("utf-8")).split(";")
-            if merchant_id in data_merchant:
-                use_abac = True
+        else:
+            data_merchant = ["972e6e1d-8891-4fdb-9d02-8a7855393298", "87d9e1f3-6da0-415f-b418-9ba9f4fe5523"]
+        if merchant_id in data_merchant:
+            use_abac = True
         return use_abac
 
     def get_policy_statement_for_target(self):
         list_statement = CallAPI.admin_get_list_statement(self.merchant_id, self.account_id,
                                                 self.resource, self.action, self.service)
         if not list_statement:
             print("abac_sdk list_statement not found merchant_id: {} , account_id: {} , "
@@ -230,16 +232,20 @@
                                 "effect": statement.get("effect"),
                                 "fields": statement.get("fields"),
                             })
                             continue
                     else:
                         # nếu ko có field nào ở cấu hình policy nằm trong dữ liệu gửi lên thì cho qua
                         if statement.get("check_field") and statement.get("fields"):
-                            if not Utils.field_in_body_request(statement.get("fields"), self.data_after):
-                                continue
+                            if self.access_level == PolicyDecisionPoint.AccessLevel.ADD:
+                                if not Utils.add_field_in_body_request(statement.get("fields"), self.data_after):
+                                    continue
+                            else:
+                                if not Utils.field_in_body_request(statement.get("fields"), self.data_after):
+                                    continue
                     self.result_access.add_log_deny(statement)
                     result_deny = True
                     break
         except Exception as err:
             msg_err = "abac_sdk check_list_statement_is_deny err: {}".format(err)
             print(msg_err)
             self.result_access.add_log_error(msg_err)
@@ -270,15 +276,21 @@
                                 {"effect": statement.get("effect"),
                                  "condition": statement.get("condition_filter")})
                             continue
                     else:
                         # kiểm tra thông tin field dữ liệu gửi lên với cấu hình field trong policy,
                         # nếu field gửi lên ko nằm trong tập con của cấu hình field thì reject statement
                         if statement.get("check_field") and statement.get("fields"):
-                            list_field_data_after = list(self.data_after.keys())
+                            list_field_data_after = []
+                            if self.access_level == PolicyDecisionPoint.AccessLevel.ADD:
+                                for k, v in self.data_after.items():
+                                    if v is not None:
+                                        list_field_data_after.append(k)
+                            else:
+                                list_field_data_after = list(self.data_after.keys())
                             if not set(list_field_data_after).issubset(statement.get("fields")):
                                 result_allow = False
                                 continue
                         break
 
         except Exception as err:
             msg_err = "abac_sdk check_list_statement_is_allow err: {}".format(err)
```

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_contains.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_contains.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/exceptions.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/policy.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/policy/utils.py` & `m-abac-test-1.0.9/mobio/libs/abac/policy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,22 @@
         if list_field and body_request:
             for field in list_field:
                 if field in body_request:
                     return True
         return False
 
     @staticmethod
+    def add_field_in_body_request(list_field, body_request):
+        if list_field and body_request:
+            for field in list_field:
+                if field in body_request and body_request.get(field) is not None:
+                    return True
+        return False
+
+    @staticmethod
     def base64_encode(data):
         try:
             byte_string = data.encode('utf-8')
             encoded_data = base64.b64encode(byte_string)
             return encoded_data.decode(encoding='UTF-8')
         except:
             return ""
```

### Comparing `m-abac-test-1.0.8/mobio/libs/abac/result_access.py` & `m-abac-test-1.0.9/mobio/libs/abac/result_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,22 +51,23 @@
             "operator": items[1],
             "field": items[2],
             "qualifier": items[3],
         }
 
     @classmethod
     def convert_data_save_log(cls, value):
-        return {
-            'merchant_id': value.get('merchant_id'),
-            'policy_code': value.get('policy_code'),
-            'statement_id': value.get('statement_id'),
-            'effect': value.get('effect'),
-            'action': value.get('action'),
-            'resource': value.get('resource'),
-        }
+        # return {
+        #     'merchant_id': value.get('merchant_id'),
+        #     'policy_code': value.get('policy_code'),
+        #     'statement_id': value.get('statement_id'),
+        #     'effect': value.get('effect'),
+        #     'action': value.get('action'),
+        #     'resource': value.get('resource'),
+        # }
+        return value
 
     def add_log_deny(self, value):
         self.log_statement_deny.append(self.convert_data_save_log(value))
 
     def add_log_allow(self, value):
         self.log_statement_allow.append(self.convert_data_save_log(value))
```

### Comparing `m-abac-test-1.0.8/setup.py` & `m-abac-test-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.8'
+version_dev='1.0.9'
 version_prod='1.0.0'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.8',  # Required
+    version='1.0.9',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

