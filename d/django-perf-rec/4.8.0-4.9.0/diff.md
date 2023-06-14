# Comparing `tmp/django-perf-rec-4.8.0.tar.gz` & `tmp/django-perf-rec-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/chainz/Documents/Projects/django-perf-rec/dist/tmpzdjmby2k/django-perf-rec-4.8.0.tar", last modified: Sat Oct 10 14:40:12 2020, max compression
+gzip compressed data, was "/Users/chainz/Documents/Projects/django-perf-rec/dist/tmphaig8nsh/django-perf-rec-4.9.0.tar", last modified: Wed Nov  4 22:14:44 2020, max compression
```

## Comparing `django-perf-rec-4.8.0.tar` & `django-perf-rec-4.9.0.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.752989 django-perf-rec-4.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     4946 2020-10-10 14:39:26.000000 django-perf-rec-4.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1081 2020-09-21 19:14:47.000000 django-perf-rec-4.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      241 2020-07-22 15:00:03.000000 django-perf-rec-4.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)    10809 2020-10-10 14:40:12.753201 django-perf-rec-4.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     7829 2020-10-04 11:21:56.000000 django-perf-rec-4.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      172 2020-09-14 10:09:29.000000 django-perf-rec-4.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1485 2020-10-10 14:40:12.753880 django-perf-rec-4.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2020-07-11 12:16:51.000000 django-perf-rec-4.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.544907 django-perf-rec-4.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.560579 django-perf-rec-4.8.0/src/django_perf_rec/
--rw-r--r--   0 chainz     (501) staff       (20)      383 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/src/django_perf_rec/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)     4339 2020-08-24 19:21:42.000000 django-perf-rec-4.8.0/src/django_perf_rec/api.py
--rw-r--r--   0 chainz     (501) staff       (20)     4009 2020-08-24 19:21:42.000000 django-perf-rec-4.8.0/src/django_perf_rec/cache.py
--rw-r--r--   0 chainz     (501) staff       (20)     2558 2020-08-24 19:21:42.000000 django-perf-rec-4.8.0/src/django_perf_rec/db.py
--rw-r--r--   0 chainz     (501) staff       (20)     1049 2020-08-24 19:21:42.000000 django-perf-rec-4.8.0/src/django_perf_rec/operation.py
--rw-r--r--   0 chainz     (501) staff       (20)     1781 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/src/django_perf_rec/orm.py
--rw-r--r--   0 chainz     (501) staff       (20)       92 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/src/django_perf_rec/pytest_plugin.py
--rw-r--r--   0 chainz     (501) staff       (20)      484 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/src/django_perf_rec/settings.py
--rw-r--r--   0 chainz     (501) staff       (20)     4796 2020-10-10 14:29:00.000000 django-perf-rec-4.8.0/src/django_perf_rec/sql.py
--rw-r--r--   0 chainz     (501) staff       (20)     2585 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/src/django_perf_rec/utils.py
--rw-r--r--   0 chainz     (501) staff       (20)     1832 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/src/django_perf_rec/yaml.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.562624 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)    10809 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)     9031 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)       60 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/entry_points.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       42 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       16 2020-10-10 14:40:12.000000 django-perf-rec-4.8.0/src/django_perf_rec.egg-info/top_level.txt
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.567193 django-perf-rec-4.8.0/tests/
--rw-r--r--   0 chainz     (501) staff       (20)        0 2020-02-24 16:30:45.000000 django-perf-rec-4.8.0/tests/__init__.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.746479 django-perf-rec-4.8.0/tests/__pycache__/
--rw-r--r--   0 chainz     (501) staff       (20)      149 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      149 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      153 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      157 2020-05-20 13:19:39.000000 django-perf-rec-4.8.0/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      157 2020-10-10 12:57:19.000000 django-perf-rec-4.8.0/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1571 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-35.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1497 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-36.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1461 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1479 2020-05-20 13:19:39.000000 django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1467 2020-10-10 12:57:19.000000 django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    19813 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    17652 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    21661 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)    21661 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)    21661 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    17294 2019-12-21 18:35:19.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    17294 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    17882 2019-11-11 21:45:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    15493 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    15973 2020-10-10 12:57:19.000000 django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    13768 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    12052 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    15334 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)    15334 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)    15334 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    11654 2019-12-21 18:35:19.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    11654 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    11915 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    10037 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     9817 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     7174 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6311 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     7815 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)     7815 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)     7815 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6153 2019-12-21 18:49:45.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6153 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     6641 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     5636 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     5610 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1265 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1209 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)      877 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)      877 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)     1341 2019-11-25 10:46:56.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1341 2019-12-21 18:35:19.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1215 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)      889 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1231 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      885 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      621 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      588 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)      593 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)      593 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)      593 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      594 2019-12-21 18:49:06.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      594 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)      601 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      602 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      618 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      789 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      741 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)      746 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)      746 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)      746 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      747 2019-12-21 18:49:06.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      747 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)      756 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      757 2020-05-21 11:30:39.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      773 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1633 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1539 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     1544 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)     1544 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)     1544 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1545 2019-12-21 18:48:38.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1545 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     1542 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1543 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1599 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1560 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1444 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     2029 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)     2029 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)     2029 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1433 2019-12-21 18:48:15.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1433 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     1899 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1442 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1440 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    27075 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    23843 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    28742 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)    28742 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)    28742 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    20220 2019-12-21 18:35:20.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    23075 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    18677 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    17313 2020-05-21 11:25:45.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    16682 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     7224 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6290 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     8464 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)     8464 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)     8464 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6071 2019-12-21 18:35:20.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     6071 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     6723 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     5367 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     5189 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)    10311 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-35-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     9009 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-36-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)    11243 2019-10-21 08:39:17.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.1.pyc
--rw-------   0 chainz     (501) staff       (20)    11243 2019-10-27 19:16:29.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.2.pyc
--rw-------   0 chainz     (501) staff       (20)    11243 2019-11-25 10:43:43.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.4.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     8807 2019-12-21 18:35:20.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.3.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     8784 2020-05-20 13:50:12.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.4.2.pyc
--rw-------   0 chainz     (501) staff       (20)     9446 2019-11-11 21:45:52.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.2.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     7947 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.4.2.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     7885 2020-10-10 14:28:51.000000 django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-39-pytest-6.1.1.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1226 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-35.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1144 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1148 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1174 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1202 2020-10-10 12:57:19.000000 django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1670 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/settings.py
--rw-r--r--   0 chainz     (501) staff       (20)       71 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_api.file_name.perf.yml
--rw-r--r--   0 chainz     (501) staff       (20)     1550 2020-10-10 14:38:46.000000 django-perf-rec-4.8.0/tests/test_api.perf.yml
--rw-r--r--   0 chainz     (501) staff       (20)     7602 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_api.py
--rw-r--r--   0 chainz     (501) staff       (20)     3182 2020-08-24 19:21:42.000000 django-perf-rec-4.8.0/tests/test_cache.py
--rw-r--r--   0 chainz     (501) staff       (20)     2157 2020-08-24 19:21:42.000000 django-perf-rec-4.8.0/tests/test_db.py
--rw-r--r--   0 chainz     (501) staff       (20)      301 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_orm.py
--rw-r--r--   0 chainz     (501) staff       (20)       38 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_duplicate.perf.yml
--rw-r--r--   0 chainz     (501) staff       (20)      214 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_duplicate.py
--rw-r--r--   0 chainz     (501) staff       (20)       72 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_duplicate_other.perf.yml
--rw-r--r--   0 chainz     (501) staff       (20)      396 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_duplicate_other.py
--rw-r--r--   0 chainz     (501) staff       (20)      113 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_fixture_usage.perf.yml
--rw-r--r--   0 chainz     (501) staff       (20)      932 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_fixture_usage.py
--rw-r--r--   0 chainz     (501) staff       (20)      465 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_pytest_plugin.py
--rw-r--r--   0 chainz     (501) staff       (20)     8202 2020-10-10 14:38:46.000000 django-perf-rec-4.8.0/tests/test_sql.py
--rw-r--r--   0 chainz     (501) staff       (20)     1212 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_utils.py
--rw-r--r--   0 chainz     (501) staff       (20)     2543 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/test_yaml.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.747261 django-perf-rec-4.8.0/tests/testapp/
--rw-r--r--   0 chainz     (501) staff       (20)        0 2020-02-24 16:30:45.000000 django-perf-rec-4.8.0/tests/testapp/__init__.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-10-10 14:40:12.752312 django-perf-rec-4.8.0/tests/testapp/__pycache__/
--rw-r--r--   0 chainz     (501) staff       (20)      157 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      157 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      161 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      165 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      165 2020-10-10 12:57:19.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1187 2020-05-20 13:46:43.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-35.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1098 2020-05-20 13:48:01.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1102 2020-05-20 13:50:11.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-37.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1118 2020-05-20 13:19:40.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 chainz     (501) staff       (20)     1118 2020-10-10 12:57:19.000000 django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 chainz     (501) staff       (20)      534 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/testapp/models.py
--rw-r--r--   0 chainz     (501) staff       (20)      864 2020-06-20 17:45:51.000000 django-perf-rec-4.8.0/tests/utils.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.794286 django-perf-rec-4.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     5165 2020-11-04 22:14:25.000000 django-perf-rec-4.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1081 2020-11-04 21:49:14.000000 django-perf-rec-4.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      241 2020-07-22 15:00:03.000000 django-perf-rec-4.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)    12364 2020-11-04 22:14:44.794598 django-perf-rec-4.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     9176 2020-11-04 22:14:21.000000 django-perf-rec-4.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      172 2020-11-04 21:49:14.000000 django-perf-rec-4.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1485 2020-11-04 22:14:44.795343 django-perf-rec-4.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       38 2020-07-11 12:16:51.000000 django-perf-rec-4.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.682390 django-perf-rec-4.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.692720 django-perf-rec-4.9.0/src/django_perf_rec/
+-rw-r--r--   0 chainz     (501) staff       (20)      383 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/src/django_perf_rec/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)     4680 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/src/django_perf_rec/api.py
+-rw-r--r--   0 chainz     (501) staff       (20)     4186 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/src/django_perf_rec/cache.py
+-rw-r--r--   0 chainz     (501) staff       (20)     2534 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/src/django_perf_rec/db.py
+-rw-r--r--   0 chainz     (501) staff       (20)     1145 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/src/django_perf_rec/operation.py
+-rw-r--r--   0 chainz     (501) staff       (20)     1781 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/src/django_perf_rec/orm.py
+-rw-r--r--   0 chainz     (501) staff       (20)       92 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/src/django_perf_rec/pytest_plugin.py
+-rw-r--r--   0 chainz     (501) staff       (20)      484 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/src/django_perf_rec/settings.py
+-rw-r--r--   0 chainz     (501) staff       (20)     4796 2020-10-10 14:29:00.000000 django-perf-rec-4.9.0/src/django_perf_rec/sql.py
+-rw-r--r--   0 chainz     (501) staff       (20)     2585 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/src/django_perf_rec/utils.py
+-rw-r--r--   0 chainz     (501) staff       (20)     1832 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/src/django_perf_rec/yaml.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.695094 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)    12364 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     9031 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       60 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/entry_points.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       42 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       16 2020-11-04 22:14:44.000000 django-perf-rec-4.9.0/src/django_perf_rec.egg-info/top_level.txt
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.703582 django-perf-rec-4.9.0/tests/
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2020-02-24 16:30:45.000000 django-perf-rec-4.9.0/tests/__init__.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.787592 django-perf-rec-4.9.0/tests/__pycache__/
+-rw-r--r--   0 chainz     (501) staff       (20)      149 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      149 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      153 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      157 2020-05-20 13:19:39.000000 django-perf-rec-4.9.0/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      157 2020-10-10 12:57:19.000000 django-perf-rec-4.9.0/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1571 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-35.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1497 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-36.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1461 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1479 2020-05-20 13:19:39.000000 django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1467 2020-10-10 12:57:19.000000 django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    19813 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    17652 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    21661 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)    21661 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    21661 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    17294 2019-12-21 18:35:19.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    17294 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    17882 2019-11-11 21:45:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    15493 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    18093 2020-11-04 21:53:48.000000 django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    13768 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    12052 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    15334 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)    15334 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    15334 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    11654 2019-12-21 18:35:19.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    11654 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    11915 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    10037 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    11637 2020-11-04 21:55:44.000000 django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     7174 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     6311 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     7815 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)     7815 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     7815 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     6153 2019-12-21 18:49:45.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     6153 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     6641 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     5636 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     7556 2020-11-04 21:55:44.000000 django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1265 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1209 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      877 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)      877 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     1341 2019-11-25 10:46:56.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1341 2019-12-21 18:35:19.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1215 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      889 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1231 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      885 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      621 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      588 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      593 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)      593 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      593 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      594 2019-12-21 18:49:06.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      594 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      601 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      602 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      618 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      789 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      741 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      746 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)      746 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      746 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      747 2019-12-21 18:49:06.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      747 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)      756 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      757 2020-05-21 11:30:39.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      773 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1633 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1539 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     1544 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)     1544 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     1544 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1545 2019-12-21 18:48:38.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1545 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     1542 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1543 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1599 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1560 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1444 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     2029 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)     2029 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     2029 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1433 2019-12-21 18:48:15.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1433 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     1899 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1442 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1440 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    27075 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    23843 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    28742 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)    28742 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    28742 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    20220 2019-12-21 18:35:20.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    23075 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    18677 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    17313 2020-05-21 11:25:45.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    16682 2020-11-04 21:53:48.000000 django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     7224 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     6290 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     8464 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)     8464 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     8464 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     6071 2019-12-21 18:35:20.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     6071 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     6723 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     5367 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     5189 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)    10311 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-35-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     9009 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-36-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    11243 2019-10-21 08:39:17.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.1.pyc
+-rw-------   0 chainz     (501) staff       (20)    11243 2019-10-27 19:16:29.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.2.pyc
+-rw-------   0 chainz     (501) staff       (20)    11243 2019-11-25 10:43:43.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.4.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     8807 2019-12-21 18:35:20.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.3.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     8784 2020-05-20 13:50:12.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.4.2.pyc
+-rw-------   0 chainz     (501) staff       (20)     9446 2019-11-11 21:45:52.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.2.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     7947 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.4.2.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     7885 2020-10-10 14:28:51.000000 django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-39-pytest-6.1.1.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1226 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-35.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1144 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1148 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1174 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1345 2020-11-04 21:55:44.000000 django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1670 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/settings.py
+-rw-r--r--   0 chainz     (501) staff       (20)       71 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_api.file_name.perf.yml
+-rw-r--r--   0 chainz     (501) staff       (20)     1550 2020-11-04 21:49:14.000000 django-perf-rec-4.9.0/tests/test_api.perf.yml
+-rw-r--r--   0 chainz     (501) staff       (20)     8963 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/tests/test_api.py
+-rw-r--r--   0 chainz     (501) staff       (20)     3899 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/tests/test_cache.py
+-rw-r--r--   0 chainz     (501) staff       (20)     2845 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/tests/test_db.py
+-rw-r--r--   0 chainz     (501) staff       (20)      301 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_orm.py
+-rw-r--r--   0 chainz     (501) staff       (20)       38 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_duplicate.perf.yml
+-rw-r--r--   0 chainz     (501) staff       (20)      214 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_duplicate.py
+-rw-r--r--   0 chainz     (501) staff       (20)       72 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_duplicate_other.perf.yml
+-rw-r--r--   0 chainz     (501) staff       (20)      396 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_duplicate_other.py
+-rw-r--r--   0 chainz     (501) staff       (20)      113 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_fixture_usage.perf.yml
+-rw-r--r--   0 chainz     (501) staff       (20)      932 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_fixture_usage.py
+-rw-r--r--   0 chainz     (501) staff       (20)      465 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 chainz     (501) staff       (20)     8202 2020-11-04 21:49:14.000000 django-perf-rec-4.9.0/tests/test_sql.py
+-rw-r--r--   0 chainz     (501) staff       (20)     1212 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_utils.py
+-rw-r--r--   0 chainz     (501) staff       (20)     2543 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/test_yaml.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.788423 django-perf-rec-4.9.0/tests/testapp/
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2020-02-24 16:30:45.000000 django-perf-rec-4.9.0/tests/testapp/__init__.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2020-11-04 22:14:44.793678 django-perf-rec-4.9.0/tests/testapp/__pycache__/
+-rw-r--r--   0 chainz     (501) staff       (20)      157 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      157 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      161 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      165 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      165 2020-10-10 12:57:19.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1187 2020-05-20 13:46:43.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-35.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1098 2020-05-20 13:48:01.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1102 2020-05-20 13:50:11.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-37.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1118 2020-05-20 13:19:40.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)     1118 2020-10-10 12:57:19.000000 django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 chainz     (501) staff       (20)      534 2020-06-20 17:45:51.000000 django-perf-rec-4.9.0/tests/testapp/models.py
+-rw-r--r--   0 chainz     (501) staff       (20)      994 2020-11-04 22:03:17.000000 django-perf-rec-4.9.0/tests/utils.py
```

### Comparing `django-perf-rec-4.8.0/HISTORY.rst` & `django-perf-rec-4.9.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+=======
 History
 =======
 
+4.9.0 (2020-11-04)
+------------------
+
+* Support Python 3.9.
+* Allow recording of tracebacks alongside db queries or cache operations,
+  selected via a function passed as ``capture_traceback`` to ``record()``.
+
 4.8.0 (2020-10-10)
 ------------------
 
 * Drop Django 2.0 and 2.1 support.
 * Upgrade for sqlparse 0.4.0+. This required changing how SQL lists of one
   element are simplified, e.g. ``IN (1)`` will now be simplified to ``IN (#)``
   instead of ``IN (...)``. You should regenerate your performance record files
```

### Comparing `django-perf-rec-4.8.0/LICENSE` & `django-perf-rec-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/PKG-INFO` & `django-perf-rec-4.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: django-perf-rec
-Version: 4.8.0
+Version: 4.9.0
 Summary: Keep detailed records of the performance of your Django code.
 Home-page: https://github.com/adamchainz/django-perf-rec
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-perf-rec/blob/master/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Description: ===============
         django-perf-rec
         ===============
         
-        .. image:: https://github.com/adamchainz/django-perf-rec/workflows/CI/badge.svg?branch=master
+        .. image:: https://img.shields.io/github/workflow/status/adamchainz/django-perf-rec/CI/master?style=for-the-badge
            :target: https://github.com/adamchainz/django-perf-rec/actions?workflow=CI
         
-        .. image:: https://img.shields.io/pypi/v/django-perf-rec.svg
+        .. image:: https://img.shields.io/pypi/v/django-perf-rec.svg?style=for-the-badge
            :target: https://pypi.org/project/django-perf-rec/
         
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/python/black
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
+           :target: https://github.com/psf/black
+        
+        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
+           :target: https://github.com/pre-commit/pre-commit
+           :alt: pre-commit
         
         "Keep detailed records of the performance of your Django code."
         
         **django-perf-rec** is like Django's ``assertNumQueries`` on steroids. It lets
         you track the individual queries and cache operations that occur in your code.
         Use it in your tests like so:
         
@@ -69,30 +73,30 @@
         .. code-block:: bash
         
             python -m pip install django-perf-rec
         
         Requirements
         ============
         
-        Python 3.5 to 3.8 supported.
+        Python 3.5 to 3.9 supported.
         
         Django 2.2 to 3.1 suppported.
         
         ----
         
         **Are your tests slow?**
         Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
         
         ----
         
         API
         ===
         
-        ``record(record_name=None, path=None)``
-        ---------------------------------------
+        ``record(record_name=None, path=None, capture_traceback=None)``
+        ---------------------------------------------------------------
         
         Return a context manager that will be used for a single performance test.
         
         The arguments must be passed as keyword arguments.
         
         ``path`` is the path to a directory or file in which to store the record. If it
         ends with ``'/'``, or is left as ``None``, the filename will be automatically
@@ -130,14 +134,37 @@
             class AuthorPerformanceTests(TestCase):
         
                 def test_special_method(self):
                     with django_perf_rec.record():
                         list(Author.objects.special_method())
         
         
+        ``capture_traceback``, if not ``None``, should be a function that takes one
+        argument, the given DB or cache operation, and returns a ``bool`` indiciating
+        if a traceback should be captured for the operation (by default, they are not).
+        Capturing tracebacks allows fine-grained debugging of code paths causing the
+        operations. Be aware that records differing only by the presence of tracebacks
+        will not match and cause an ``AssertionError`` to be raised, so it's not
+        normally suitable to permanently record the tracebacks.
+        
+        For example, if you wanted to know what code paths query the table
+        ``my_table``, you could use a ``capture_traceback`` function like so:
+        
+        .. code-block:: python
+        
+            def debug_sql_query(operation):
+                return "my_tables" in operation.query
+        
+            def test_special_method(self):
+                with django_perf_rec.record(capture_traceback=debug_sql_query):
+                    list(Author.objects.special_method())
+        
+        The performance record herer would include a standard Python traceback attached
+        to each SQL query containing "my_table".
+        
         ``TestCaseMixin``
         -----------------
         
         A mixin class to be added to your custom ``TestCase`` subclass so you can use
         **django-perf-rec** across your codebase without needing to import it in each
         individual test file. It adds one method, ``record_performance()``, whose
         signature is the same as ``record()`` above.
@@ -216,15 +243,14 @@
         
         * ``'once'`` (default) creates missing records silently.
         * ``'none'`` raises ``AssertionError`` when a record does not exist. You
           probably want to use this mode in CI, to ensure new tests fail if their
           corresponding performance records were not committed.
         * ``'all'`` creates missing records and then raises ``AssertionError``.
         
-        
         Usage in Pytest
         ===============
         
         If you're using Pytest, you might want to call ``record()`` from within a
         Pytest fixture and have it automatically apply to all your tests. We have an
         example of this, see the file `test_pytest_fixture_usage.py
         <https://github.com/adamchainz/django-perf-rec/blob/master/tests/test_pytest_fixture_usage.py>`_
```

### Comparing `django-perf-rec-4.8.0/README.rst` & `django-perf-rec-4.9.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 ===============
 django-perf-rec
 ===============
 
-.. image:: https://github.com/adamchainz/django-perf-rec/workflows/CI/badge.svg?branch=master
+.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-perf-rec/CI/master?style=for-the-badge
    :target: https://github.com/adamchainz/django-perf-rec/actions?workflow=CI
 
-.. image:: https://img.shields.io/pypi/v/django-perf-rec.svg
+.. image:: https://img.shields.io/pypi/v/django-perf-rec.svg?style=for-the-badge
    :target: https://pypi.org/project/django-perf-rec/
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/python/black
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
+   :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
+   :target: https://github.com/pre-commit/pre-commit
+   :alt: pre-commit
 
 "Keep detailed records of the performance of your Django code."
 
 **django-perf-rec** is like Django's ``assertNumQueries`` on steroids. It lets
 you track the individual queries and cache operations that occur in your code.
 Use it in your tests like so:
 
@@ -59,30 +63,30 @@
 .. code-block:: bash
 
     python -m pip install django-perf-rec
 
 Requirements
 ============
 
-Python 3.5 to 3.8 supported.
+Python 3.5 to 3.9 supported.
 
 Django 2.2 to 3.1 suppported.
 
 ----
 
 **Are your tests slow?**
 Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
 
 ----
 
 API
 ===
 
-``record(record_name=None, path=None)``
----------------------------------------
+``record(record_name=None, path=None, capture_traceback=None)``
+---------------------------------------------------------------
 
 Return a context manager that will be used for a single performance test.
 
 The arguments must be passed as keyword arguments.
 
 ``path`` is the path to a directory or file in which to store the record. If it
 ends with ``'/'``, or is left as ``None``, the filename will be automatically
@@ -120,14 +124,37 @@
     class AuthorPerformanceTests(TestCase):
 
         def test_special_method(self):
             with django_perf_rec.record():
                 list(Author.objects.special_method())
 
 
+``capture_traceback``, if not ``None``, should be a function that takes one
+argument, the given DB or cache operation, and returns a ``bool`` indiciating
+if a traceback should be captured for the operation (by default, they are not).
+Capturing tracebacks allows fine-grained debugging of code paths causing the
+operations. Be aware that records differing only by the presence of tracebacks
+will not match and cause an ``AssertionError`` to be raised, so it's not
+normally suitable to permanently record the tracebacks.
+
+For example, if you wanted to know what code paths query the table
+``my_table``, you could use a ``capture_traceback`` function like so:
+
+.. code-block:: python
+
+    def debug_sql_query(operation):
+        return "my_tables" in operation.query
+
+    def test_special_method(self):
+        with django_perf_rec.record(capture_traceback=debug_sql_query):
+            list(Author.objects.special_method())
+
+The performance record herer would include a standard Python traceback attached
+to each SQL query containing "my_table".
+
 ``TestCaseMixin``
 -----------------
 
 A mixin class to be added to your custom ``TestCase`` subclass so you can use
 **django-perf-rec** across your codebase without needing to import it in each
 individual test file. It adds one method, ``record_performance()``, whose
 signature is the same as ``record()`` above.
@@ -206,15 +233,14 @@
 
 * ``'once'`` (default) creates missing records silently.
 * ``'none'`` raises ``AssertionError`` when a record does not exist. You
   probably want to use this mode in CI, to ensure new tests fail if their
   corresponding performance records were not committed.
 * ``'all'`` creates missing records and then raises ``AssertionError``.
 
-
 Usage in Pytest
 ===============
 
 If you're using Pytest, you might want to call ``record()`` from within a
 Pytest fixture and have it automatically apply to all your tests. We have an
 example of this, see the file `test_pytest_fixture_usage.py
 <https://github.com/adamchainz/django-perf-rec/blob/master/tests/test_pytest_fixture_usage.py>`_
```

### Comparing `django-perf-rec-4.8.0/setup.cfg` & `django-perf-rec-4.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-perf-rec
-version = 4.8.0
+version = 4.9.0
 description = Keep detailed records of the performance of your Django code.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/django-perf-rec
 project_urls =
```

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/api.py` & `django-perf-rec-4.9.0/src/django_perf_rec/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
+import traceback
 from threading import local
 
 from django.utils.functional import SimpleLazyObject
 
 from django_perf_rec import pytest_plugin
 from django_perf_rec.cache import AllCacheRecorder
 from django_perf_rec.db import AllDBRecorder
 from django_perf_rec.settings import perf_rec_settings
 from django_perf_rec.utils import current_test, record_diff
 from django_perf_rec.yaml import KVFile
 
 record_current = local()
 
 
-def record(*, record_name=None, path=None):
+def record(*, record_name=None, path=None, capture_traceback=None):
     # Lazy since we may not need this to determine record_name or path,
     # depending on logic below
     test_details = SimpleLazyObject(current_test)
 
     if path is None or path.endswith("/"):
         file_name = get_perf_path(test_details.file_path)
     else:
@@ -36,15 +37,15 @@
     if record_name is None:
         record_name = get_record_name(
             test_name=test_details.test_name,
             class_name=test_details.class_name,
             file_name=file_name,
         )
 
-    return PerformanceRecorder(file_name, record_name)
+    return PerformanceRecorder(file_name, record_name, capture_traceback)
 
 
 def get_perf_path(file_path):
     if file_path.endswith(".py"):
         perf_path = file_path[: -len(".py")] + ".perf.yml"
     elif file_path.endswith(".pyc"):
         perf_path = file_path[: -len(".pyc")] + ".perf.yml"
@@ -68,43 +69,50 @@
         record_current.record_spec = record_spec
         record_current.counter = 1
 
     return record_name
 
 
 class PerformanceRecorder:
-    def __init__(self, file_name, record_name):
+    def __init__(self, file_name, record_name, capture_traceback):
         self.file_name = file_name
         self.record_name = record_name
 
         self.record = []
         self.db_recorder = AllDBRecorder(self.on_op)
         self.cache_recorder = AllCacheRecorder(self.on_op)
+        self.capture_traceback = capture_traceback
 
     def __enter__(self):
         self.db_recorder.__enter__()
         self.cache_recorder.__enter__()
         self.load_recordings()
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.cache_recorder.__exit__(exc_type, exc_value, exc_traceback)
         self.db_recorder.__exit__(exc_type, exc_value, exc_traceback)
 
         if exc_type is None:
             self.save_or_assert()
 
     def on_op(self, op):
-        self.record.append({op.name: op.query})
+        record = {op.name: op.query}
+
+        if self.capture_traceback and self.capture_traceback(op):
+            record["traceback"] = traceback.StackSummary.from_list(
+                op.traceback
+            ).format()
+
+        self.record.append(record)
 
     def load_recordings(self):
         self.records_file = KVFile(self.file_name)
 
     def save_or_assert(self):
         orig_record = self.records_file.get(self.record_name, None)
-
         if perf_rec_settings.MODE == "none":
             assert (
                 orig_record is not None
             ), "Original performance record does not exist for {}".format(
                 self.record_name
             )
```

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/cache.py` & `django-perf-rec-4.9.0/src/django_perf_rec/cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import inspect
 import re
+import traceback
 from collections.abc import Mapping, Sequence
 from functools import wraps
 from types import MethodType
 
 from django.core.cache import DEFAULT_CACHE_ALIAS, caches
 
 from django_perf_rec.operation import AllSourceRecorder, Operation
 
 
 class CacheOp(Operation):
-    def __init__(self, alias, operation, key_or_keys):
+    def __init__(self, alias, operation, key_or_keys, traceback):
+        self.alias = alias
         self.operation = operation
         if isinstance(key_or_keys, str):
             cleaned_key_or_keys = self.clean_key(key_or_keys)
         elif isinstance(key_or_keys, (Mapping, Sequence)):
             cleaned_key_or_keys = sorted(self.clean_key(k) for k in key_or_keys)
         else:
             raise ValueError("key_or_keys must be a string, mapping, or sequence")
 
-        super().__init__(alias, cleaned_key_or_keys)
+        super().__init__(alias, cleaned_key_or_keys, traceback)
 
     @classmethod
     def clean_key(cls, key):
         """
         Replace things that look like variables with a '#' so tests aren't
         affected by random variables
         """
@@ -82,19 +84,21 @@
                     frame = frame.f_back
                     is_internal_call = frame.f_locals.get("self", None) is self
                 finally:
                     # Always delete frame references to help garbage collector
                     del frame
 
                 if not is_internal_call:
+                    key_or_keys = args[0]
                     callback(
                         CacheOp(
                             alias=alias,
                             operation=str(func.__name__),
-                            key_or_keys=args[0],
+                            key_or_keys=key_or_keys,
+                            traceback=traceback.extract_stack(),
                         )
                     )
 
                 return func(*args, **kwargs)
 
             return inner
```

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/db.py` & `django-perf-rec-4.9.0/src/django_perf_rec/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
+import traceback
 from functools import wraps
 from types import MethodType
 
 from django.db import DEFAULT_DB_ALIAS, connections
 
 from django_perf_rec.operation import AllSourceRecorder, Operation
 from django_perf_rec.orm import patch_ORM_to_be_deterministic
 from django_perf_rec.settings import perf_rec_settings
 from django_perf_rec.sql import sql_fingerprint
 
 
 class DBOp(Operation):
-    def __repr__(self):
-        return "DBOp({!r}, {!r})".format(repr(self.alias), repr(self.query))
-
     @property
     def name(self):
         name_parts = ["db"]
         if self.alias != DEFAULT_DB_ALIAS:
             name_parts.append(self.alias)
         return "|".join(name_parts)
 
@@ -52,14 +50,15 @@
             def inner(self, *args, **kwargs):
                 sql = func(*args, **kwargs)
                 hide_columns = perf_rec_settings.HIDE_COLUMNS
                 callback(
                     DBOp(
                         alias=alias,
                         query=sql_fingerprint(sql, hide_columns=hide_columns),
+                        traceback=traceback.extract_stack(),
                     )
                 )
                 return sql
 
             return inner
 
         self.orig_last_executed_query = connection.ops.last_executed_query
```

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/operation.py` & `django-perf-rec-4.9.0/src/django_perf_rec/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from django.conf import settings
 
 from django_perf_rec.utils import sorted_names
 
 
 class Operation:
-    def __init__(self, alias, query):
+    def __init__(self, alias, query, traceback):
         self.alias = alias
         self.query = query
+        self.traceback = traceback
 
     def __eq__(self, other):
         return (
             isinstance(other, type(self))
             and self.alias == other.alias
             and self.query == other.query
+            and self.traceback == other.traceback
         )
 
 
 class AllSourceRecorder:
     """
     Launches Recorders on all the active sources
     """
```

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/orm.py` & `django-perf-rec-4.9.0/src/django_perf_rec/orm.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/sql.py` & `django-perf-rec-4.9.0/src/django_perf_rec/sql.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/utils.py` & `django-perf-rec-4.9.0/src/django_perf_rec/utils.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec/yaml.py` & `django-perf-rec-4.9.0/src/django_perf_rec/yaml.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec.egg-info/PKG-INFO` & `django-perf-rec-4.9.0/src/django_perf_rec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: django-perf-rec
-Version: 4.8.0
+Version: 4.9.0
 Summary: Keep detailed records of the performance of your Django code.
 Home-page: https://github.com/adamchainz/django-perf-rec
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/django-perf-rec/blob/master/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
 Description: ===============
         django-perf-rec
         ===============
         
-        .. image:: https://github.com/adamchainz/django-perf-rec/workflows/CI/badge.svg?branch=master
+        .. image:: https://img.shields.io/github/workflow/status/adamchainz/django-perf-rec/CI/master?style=for-the-badge
            :target: https://github.com/adamchainz/django-perf-rec/actions?workflow=CI
         
-        .. image:: https://img.shields.io/pypi/v/django-perf-rec.svg
+        .. image:: https://img.shields.io/pypi/v/django-perf-rec.svg?style=for-the-badge
            :target: https://pypi.org/project/django-perf-rec/
         
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-           :target: https://github.com/python/black
+        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
+           :target: https://github.com/psf/black
+        
+        .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge
+           :target: https://github.com/pre-commit/pre-commit
+           :alt: pre-commit
         
         "Keep detailed records of the performance of your Django code."
         
         **django-perf-rec** is like Django's ``assertNumQueries`` on steroids. It lets
         you track the individual queries and cache operations that occur in your code.
         Use it in your tests like so:
         
@@ -69,30 +73,30 @@
         .. code-block:: bash
         
             python -m pip install django-perf-rec
         
         Requirements
         ============
         
-        Python 3.5 to 3.8 supported.
+        Python 3.5 to 3.9 supported.
         
         Django 2.2 to 3.1 suppported.
         
         ----
         
         **Are your tests slow?**
         Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
         
         ----
         
         API
         ===
         
-        ``record(record_name=None, path=None)``
-        ---------------------------------------
+        ``record(record_name=None, path=None, capture_traceback=None)``
+        ---------------------------------------------------------------
         
         Return a context manager that will be used for a single performance test.
         
         The arguments must be passed as keyword arguments.
         
         ``path`` is the path to a directory or file in which to store the record. If it
         ends with ``'/'``, or is left as ``None``, the filename will be automatically
@@ -130,14 +134,37 @@
             class AuthorPerformanceTests(TestCase):
         
                 def test_special_method(self):
                     with django_perf_rec.record():
                         list(Author.objects.special_method())
         
         
+        ``capture_traceback``, if not ``None``, should be a function that takes one
+        argument, the given DB or cache operation, and returns a ``bool`` indiciating
+        if a traceback should be captured for the operation (by default, they are not).
+        Capturing tracebacks allows fine-grained debugging of code paths causing the
+        operations. Be aware that records differing only by the presence of tracebacks
+        will not match and cause an ``AssertionError`` to be raised, so it's not
+        normally suitable to permanently record the tracebacks.
+        
+        For example, if you wanted to know what code paths query the table
+        ``my_table``, you could use a ``capture_traceback`` function like so:
+        
+        .. code-block:: python
+        
+            def debug_sql_query(operation):
+                return "my_tables" in operation.query
+        
+            def test_special_method(self):
+                with django_perf_rec.record(capture_traceback=debug_sql_query):
+                    list(Author.objects.special_method())
+        
+        The performance record herer would include a standard Python traceback attached
+        to each SQL query containing "my_table".
+        
         ``TestCaseMixin``
         -----------------
         
         A mixin class to be added to your custom ``TestCase`` subclass so you can use
         **django-perf-rec** across your codebase without needing to import it in each
         individual test file. It adds one method, ``record_performance()``, whose
         signature is the same as ``record()`` above.
@@ -216,15 +243,14 @@
         
         * ``'once'`` (default) creates missing records silently.
         * ``'none'`` raises ``AssertionError`` when a record does not exist. You
           probably want to use this mode in CI, to ensure new tests fail if their
           corresponding performance records were not committed.
         * ``'all'`` creates missing records and then raises ``AssertionError``.
         
-        
         Usage in Pytest
         ===============
         
         If you're using Pytest, you might want to call ``record()`` from within a
         Pytest fixture and have it automatically apply to all your tests. We have an
         example of this, see the file `test_pytest_fixture_usage.py
         <https://github.com/adamchainz/django-perf-rec/blob/master/tests/test_pytest_fixture_usage.py>`_
```

### Comparing `django-perf-rec-4.8.0/src/django_perf_rec.egg-info/SOURCES.txt` & `django-perf-rec-4.9.0/src/django_perf_rec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-35.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-36.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-37.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-38.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/settings.cpython-39.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/settings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_api.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_api.cpython-39-pytest-6.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 4f4b ee5e b21d 0000 e300 0000  a...OK.^........
+00000000: 610d 0d0a da21 a35f 0323 0000 e300 0000  a....!._.#......
 00000010: 0000 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0040 0000 0073 ec00 0000 6400 6401 6c00  .@...s....d.d.l.
 00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
 00000040: 5a05 0100 6400 6401 6c06 5a06 6400 6401  Z...d.d.l.Z.d.d.
 00000050: 6c07 5a07 6400 6402 6c08 6d09 5a09 0100  l.Z.d.d.l.m.Z...
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6400 6405 6c0e 6d0f  l.m.Z...d.d.l.m.
@@ -25,975 +25,1107 @@
 00000180: 5f70 6174 68da 0f67 6574 5f72 6563 6f72  _path..get_recor
 00000190: 645f 6e61 6d65 da06 7265 636f 7264 2901  d_name..record).
 000001a0: da06 4175 7468 6f72 2903 da18 7072 6574  ..Author)...pret
 000001b0: 656e 645f 6e6f 745f 756e 6465 725f 7079  end_not_under_py
 000001c0: 7465 7374 da09 7275 6e5f 7175 6572 79da  test..run_query.
 000001d0: 0e74 656d 706f 7261 7279 5f70 6174 6863  .temporary_pathc
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 0300 0000 4000 0000 73ec 0000 0065 005a  ....@...s....e.Z
+000001f0: 0300 0000 4000 0000 73fc 0000 0065 005a  ....@...s....e.Z
 00000200: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-00000210: 0484 005a 0465 0564 0564 0669 0164 078d  ...Z.e.d.d.i.d..
-00000220: 0164 0864 0984 0083 015a 0664 0a64 0b84  .d.d.....Z.d.d..
-00000230: 005a 0764 0c64 0d84 005a 0864 0e64 0f84  .Z.d.d...Z.d.d..
+00000210: 0484 005a 0464 0564 0684 005a 0565 0664  ...Z.d.d...Z.e.d
+00000220: 0764 0869 0164 098d 0164 0a64 0b84 0083  .d.i.d...d.d....
+00000230: 015a 0764 0c64 0d84 005a 0864 0e64 0f84  .Z.d.d...Z.d.d..
 00000240: 005a 0964 1064 1184 005a 0a64 1264 1384  .Z.d.d...Z.d.d..
 00000250: 005a 0b64 1464 1584 005a 0c64 1664 1784  .Z.d.d...Z.d.d..
 00000260: 005a 0d64 1864 1984 005a 0e64 1a64 1b84  .Z.d.d...Z.d.d..
 00000270: 005a 0f64 1c64 1d84 005a 1064 1e64 1f84  .Z.d.d...Z.d.d..
 00000280: 005a 1164 2064 2184 005a 1264 2264 2384  .Z.d d!..Z.d"d#.
-00000290: 005a 1364 2464 2584 005a 1465 0564 2664  .Z.d$d%..Z.e.d&d
-000002a0: 2769 0164 078d 0164 2864 2984 0083 015a  'i.d...d(d)....Z
-000002b0: 1565 0564 2664 2a69 0164 078d 0164 2b64  .e.d&d*i.d...d+d
-000002c0: 2c84 0083 015a 1665 0564 2664 2d69 0164  ,....Z.e.d&d-i.d
-000002d0: 078d 0164 2e64 2f84 0083 015a 1764 3064  ...d.d/....Z.d0d
-000002e0: 3184 005a 1864 3253 0029 33da 0b52 6563  1..Z.d2S.)3..Rec
-000002f0: 6f72 6454 6573 7473 6301 0000 0000 0000  ordTestsc.......
-00000300: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
-00000310: 0073 3400 0000 7400 8300 8f1a 0100 7401  .s4...t.......t.
-00000320: 6401 6402 8302 0100 5700 6400 0400 0400  d.d.....W.d.....
-00000330: 8303 0100 6e10 3100 7326 3000 0100 0100  ....n.1.s&0.....
-00000340: 0100 5900 0100 6400 5300 2903 4eda 0764  ..Y...d.S.).N..d
-00000350: 6566 6175 6c74 fa0b 5345 4c45 4354 2031  efault..SELECT 1
-00000360: 3333 37a9 0272 0b00 0000 720e 0000 00a9  337..r....r.....
-00000370: 01da 0473 656c 66a9 0072 1600 0000 fa42  ...self..r.....B
-00000380: 2f55 7365 7273 2f63 6861 696e 7a2f 446f  /Users/chainz/Do
-00000390: 6375 6d65 6e74 732f 5072 6f6a 6563 7473  cuments/Projects
-000003a0: 2f64 6a61 6e67 6f2d 7065 7266 2d72 6563  /django-perf-rec
-000003b0: 2f74 6573 7473 2f74 6573 745f 6170 692e  /tests/test_api.
-000003c0: 7079 da14 7465 7374 5f73 696e 676c 655f  py..test_single_
-000003d0: 6462 5f71 7565 7279 1100 0000 7304 0000  db_query....s...
-000003e0: 0000 0108 017a 2052 6563 6f72 6454 6573  .....z RecordTes
-000003f0: 7473 2e74 6573 745f 7369 6e67 6c65 5f64  ts.test_single_d
-00000400: 625f 7175 6572 7963 0100 0000 0000 0000  b_queryc........
-00000410: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-00000420: 7338 0000 0074 0083 008f 1e01 0074 0174  s8...t.......t.t
-00000430: 026a 03a0 04a1 0083 0101 0057 0064 0004  .j.........W.d..
-00000440: 0004 0083 0301 006e 1031 0073 2a30 0001  .......n.1.s*0..
-00000450: 0001 0001 0059 0001 0064 0053 00a9 014e  .....Y...d.S...N
-00000460: a905 720b 0000 00da 046c 6973 7472 0c00  ..r......listr..
-00000470: 0000 da07 6f62 6a65 6374 73da 0361 6c6c  ....objects..all
-00000480: 7214 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000490: 1700 0000 da1a 7465 7374 5f73 696e 676c  ......test_singl
-000004a0: 655f 6462 5f71 7565 7279 5f6d 6f64 656c  e_db_query_model
-000004b0: 1500 0000 7304 0000 0000 0108 017a 2652  ....s........z&R
-000004c0: 6563 6f72 6454 6573 7473 2e74 6573 745f  ecordTests.test_
-000004d0: 7369 6e67 6c65 5f64 625f 7175 6572 795f  single_db_query_
-000004e0: 6d6f 6465 6cda 0c48 4944 455f 434f 4c55  model..HIDE_COLU
-000004f0: 4d4e 5346 2901 da08 5045 5246 5f52 4543  MNSF)...PERF_REC
-00000500: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000510: 0008 0000 0043 0000 0073 3800 0000 7400  .....C...s8...t.
-00000520: 8300 8f1e 0100 7401 7402 6a03 a004 a100  ......t.t.j.....
-00000530: 8301 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000540: 6e10 3100 732a 3000 0100 0100 0100 5900  n.1.s*0.......Y.
-00000550: 0100 6400 5300 7219 0000 0072 1a00 0000  ..d.S.r....r....
-00000560: 7214 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000570: 1700 0000 da27 7465 7374 5f73 696e 676c  .....'test_singl
-00000580: 655f 6462 5f71 7565 7279 5f6d 6f64 656c  e_db_query_model
-00000590: 5f77 6974 685f 636f 6c75 6d6e 7319 0000  _with_columns...
-000005a0: 0073 0400 0000 0002 0801 7a33 5265 636f  .s........z3Reco
-000005b0: 7264 5465 7374 732e 7465 7374 5f73 696e  rdTests.test_sin
-000005c0: 676c 655f 6462 5f71 7565 7279 5f6d 6f64  gle_db_query_mod
-000005d0: 656c 5f77 6974 685f 636f 6c75 6d6e 7363  el_with_columnsc
-000005e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000005f0: 0800 0000 4300 0000 733e 0000 0074 0083  ....C...s>...t..
-00000600: 008f 2401 0074 0164 0164 0283 0201 0074  ..$..t.d.d.....t
-00000610: 0164 0164 0383 0201 0057 0064 0004 0004  .d.d.....W.d....
-00000620: 0083 0301 006e 1031 0073 3030 0001 0001  .....n.1.s00....
-00000630: 0001 0059 0001 0064 0053 0029 044e 7211  ...Y...d.S.).Nr.
-00000640: 0000 0072 1200 0000 7a0b 5345 4c45 4354  ...r....z.SELECT
-00000650: 2034 3934 3972 1300 0000 7214 0000 0072   4949r....r....r
-00000660: 1600 0000 7216 0000 0072 1700 0000 da18  ....r....r......
-00000670: 7465 7374 5f6d 756c 7469 706c 655f 6462  test_multiple_db
-00000680: 5f71 7565 7269 6573 1e00 0000 7306 0000  _queries....s...
-00000690: 0000 0108 010a 017a 2452 6563 6f72 6454  .......z$RecordT
-000006a0: 6573 7473 2e74 6573 745f 6d75 6c74 6970  ests.test_multip
-000006b0: 6c65 5f64 625f 7175 6572 6965 7363 0100  le_db_queriesc..
-000006c0: 0000 0000 0000 0000 0000 0100 0000 0800  ................
-000006d0: 0000 4300 0000 7346 0000 0074 0083 008f  ..C...sF...t....
-000006e0: 2c01 0074 0174 026a 036a 0474 0564 0183  ,..t.t.j.j.t.d..
-000006f0: 0174 0564 0183 0164 028d 0283 0101 0057  .t.d...d.......W
-00000700: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-00000710: 3830 0001 0001 0001 0059 0001 0064 0053  80.......Y...d.S
-00000720: 0029 034e da04 6e61 6d65 a902 da01 78da  .).N..name....x.
-00000730: 0179 2906 720b 0000 0072 1b00 0000 720c  .y).r....r....r.
-00000740: 0000 0072 1c00 0000 da08 616e 6e6f 7461  ...r......annota
-00000750: 7465 7204 0000 0072 1400 0000 7216 0000  ter....r....r...
-00000760: 0072 1600 0000 7217 0000 00da 2874 6573  .r....r.....(tes
-00000770: 745f 6e6f 6e5f 6465 7465 726d 696e 6973  t_non_determinis
-00000780: 7469 635f 5175 6572 7953 6574 5f61 6e6e  tic_QuerySet_ann
-00000790: 6f74 6174 6523 0000 0073 0400 0000 0001  otate#...s......
-000007a0: 0801 7a34 5265 636f 7264 5465 7374 732e  ..z4RecordTests.
-000007b0: 7465 7374 5f6e 6f6e 5f64 6574 6572 6d69  test_non_determi
-000007c0: 6e69 7374 6963 5f51 7565 7279 5365 745f  nistic_QuerySet_
-000007d0: 616e 6e6f 7461 7465 6301 0000 0000 0000  annotatec.......
-000007e0: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
-000007f0: 0073 4200 0000 7400 8300 8f28 0100 7401  .sB...t....(..t.
-00000800: 7402 6a03 6a04 6401 6401 6402 9c02 6403  t.j.j.d.d.d...d.
-00000810: 8d01 8301 0100 5700 6400 0400 0400 8303  ......W.d.......
-00000820: 0100 6e10 3100 7334 3000 0100 0100 0100  ..n.1.s40.......
-00000830: 5900 0100 6400 5300 2904 4eda 0131 7224  Y...d.S.).N..1r$
-00000840: 0000 0029 01da 0673 656c 6563 7429 0572  ...)...select).r
-00000850: 0b00 0000 721b 0000 0072 0c00 0000 721c  ....r....r....r.
-00000860: 0000 00da 0565 7874 7261 7214 0000 0072  .....extrar....r
-00000870: 1600 0000 7216 0000 0072 1700 0000 da25  ....r....r.....%
-00000880: 7465 7374 5f6e 6f6e 5f64 6574 6572 6d69  test_non_determi
-00000890: 6e69 7374 6963 5f51 7565 7279 5365 745f  nistic_QuerySet_
-000008a0: 6578 7472 6127 0000 0073 0400 0000 0001  extra'...s......
-000008b0: 0801 7a31 5265 636f 7264 5465 7374 732e  ..z1RecordTests.
-000008c0: 7465 7374 5f6e 6f6e 5f64 6574 6572 6d69  test_non_determi
-000008d0: 6e69 7374 6963 5f51 7565 7279 5365 745f  nistic_QuerySet_
-000008e0: 6578 7472 6163 0100 0000 0000 0000 0000  extrac..........
-000008f0: 0000 0100 0000 0800 0000 4300 0000 7342  ..........C...sB
-00000900: 0000 0074 0083 008f 2801 0074 0174 026a  ...t....(..t.t.j
-00000910: 03a0 0474 0564 0164 0264 038d 02a1 0183  ...t.d.d.d......
-00000920: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000930: 1031 0073 3430 0001 0001 0001 0059 0001  .1.s40.......Y..
-00000940: 0064 0053 0029 044e da03 666f 6fe9 0100  .d.S.).N..foo...
-00000950: 0000 a902 7223 0000 00da 0361 6765 2906  ....r#.....age).
-00000960: 720b 0000 0072 1b00 0000 720c 0000 0072  r....r....r....r
-00000970: 1c00 0000 da06 6669 6c74 6572 7203 0000  ......filterr...
-00000980: 0072 1400 0000 7216 0000 0072 1600 0000  .r....r....r....
-00000990: 7217 0000 00da 1e74 6573 745f 6e6f 6e5f  r......test_non_
-000009a0: 6465 7465 726d 696e 6973 7469 635f 515f  deterministic_Q_
-000009b0: 7175 6572 792b 0000 0073 0400 0000 0001  query+...s......
-000009c0: 0801 7a2a 5265 636f 7264 5465 7374 732e  ..z*RecordTests.
-000009d0: 7465 7374 5f6e 6f6e 5f64 6574 6572 6d69  test_non_determi
-000009e0: 6e69 7374 6963 5f51 5f71 7565 7279 6301  nistic_Q_queryc.
-000009f0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
-00000a00: 0000 0043 0000 0073 3800 0000 7400 8300  ...C...s8...t...
-00000a10: 8f1e 0100 7401 6401 1900 a002 6402 a101  ....t.d.....d...
-00000a20: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
-00000a30: 3100 732a 3000 0100 0100 0100 5900 0100  1.s*0.......Y...
-00000a40: 6400 5300 a903 4e72 1100 0000 722d 0000  d.S...Nr....r-..
-00000a50: 00a9 0372 0b00 0000 7202 0000 00da 0367  ...r....r......g
-00000a60: 6574 7214 0000 0072 1600 0000 7216 0000  etr....r....r...
-00000a70: 0072 1700 0000 da14 7465 7374 5f73 696e  .r......test_sin
-00000a80: 676c 655f 6361 6368 655f 6f70 2f00 0000  gle_cache_op/...
-00000a90: 7304 0000 0000 0108 017a 2052 6563 6f72  s........z Recor
-00000aa0: 6454 6573 7473 2e74 6573 745f 7369 6e67  dTests.test_sing
-00000ab0: 6c65 5f63 6163 6865 5f6f 7063 0100 0000  le_cache_opc....
-00000ac0: 0000 0000 0000 0000 0100 0000 0800 0000  ................
-00000ad0: 4300 0000 735a 0000 0074 0083 008f 4001  C...sZ...t....@.
-00000ae0: 0074 0164 0119 00a0 0264 0264 03a1 0201  .t.d.....d.d....
-00000af0: 0074 0164 0419 00a0 0364 0264 0367 02a1  .t.d.....d.d.g..
-00000b00: 0101 0074 0164 0119 00a0 0464 02a1 0101  ...t.d.....d....
-00000b10: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00000b20: 0073 4c30 0001 0001 0001 0059 0001 0064  .sL0.......Y...d
-00000b30: 0053 0029 054e 7211 0000 0072 2d00 0000  .S.).Nr....r-...
-00000b40: da03 6261 72da 0673 6563 6f6e 6429 0572  ..bar..second).r
-00000b50: 0b00 0000 7202 0000 00da 0373 6574 da08  ....r......set..
-00000b60: 6765 745f 6d61 6e79 da06 6465 6c65 7465  get_many..delete
-00000b70: 7214 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000b80: 1700 0000 da17 7465 7374 5f6d 756c 7469  ......test_multi
-00000b90: 706c 655f 6361 6368 655f 6f70 7333 0000  ple_cache_ops3..
-00000ba0: 0073 0800 0000 0001 0801 1001 1201 7a23  .s............z#
-00000bb0: 5265 636f 7264 5465 7374 732e 7465 7374  RecordTests.test
-00000bc0: 5f6d 756c 7469 706c 655f 6361 6368 655f  _multiple_cache_
-00000bd0: 6f70 7363 0100 0000 0000 0000 0000 0000  opsc............
-00000be0: 0100 0000 0800 0000 4300 0000 736c 0000  ........C...sl..
-00000bf0: 0074 0083 008f 1e01 0074 0164 0119 00a0  .t.......t.d....
-00000c00: 0264 02a1 0101 0057 0064 0004 0004 0083  .d.....W.d......
-00000c10: 0301 006e 1031 0073 2a30 0001 0001 0001  ...n.1.s*0......
-00000c20: 0059 0001 0074 0083 008f 1e01 0074 0164  .Y...t.......t.d
-00000c30: 0119 00a0 0264 03a1 0101 0057 0064 0004  .....d.....W.d..
-00000c40: 0004 0083 0301 006e 1031 0073 5e30 0001  .......n.1.s^0..
-00000c50: 0001 0001 0059 0001 0064 0053 0029 044e  .....Y...d.S.).N
-00000c60: 7211 0000 0072 2d00 0000 7237 0000 0072  r....r-...r7...r
-00000c70: 3400 0000 7214 0000 0072 1600 0000 7216  4...r....r....r.
-00000c80: 0000 0072 1700 0000 da3a 7465 7374 5f6d  ...r.....:test_m
-00000c90: 756c 7469 706c 655f 6361 6c6c 735f 696e  ultiple_calls_in
-00000ca0: 5f73 616d 655f 6675 6e63 7469 6f6e 5f61  _same_function_a
-00000cb0: 7265 5f64 6966 6665 7265 6e74 5f72 6563  re_different_rec
-00000cc0: 6f72 6473 3900 0000 7308 0000 0000 0108  ords9...s.......
-00000cd0: 012c 0208 017a 4652 6563 6f72 6454 6573  .,...zFRecordTes
-00000ce0: 7473 2e74 6573 745f 6d75 6c74 6970 6c65  ts.test_multiple
-00000cf0: 5f63 616c 6c73 5f69 6e5f 7361 6d65 5f66  _calls_in_same_f
-00000d00: 756e 6374 696f 6e5f 6172 655f 6469 6666  unction_are_diff
-00000d10: 6572 656e 745f 7265 636f 7264 7363 0100  erent_recordsc..
-00000d20: 0000 0000 0000 0000 0000 0100 0000 0800  ................
-00000d30: 0000 4300 0000 733c 0000 0074 0064 0164  ..C...s<...t.d.d
-00000d40: 028d 018f 1e01 0074 0164 0319 00a0 0264  .......t.d.....d
-00000d50: 04a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00000d60: 006e 1031 0073 2e30 0001 0001 0001 0059  .n.1.s.0.......Y
-00000d70: 0001 0064 0053 0029 054e da06 6375 7374  ...d.S.).N..cust
-00000d80: 6f6d a901 da0b 7265 636f 7264 5f6e 616d  om....record_nam
-00000d90: 6572 1100 0000 722d 0000 0072 3400 0000  er....r-...r4...
-00000da0: 7214 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-00000db0: 1700 0000 da10 7465 7374 5f63 7573 746f  ......test_custo
-00000dc0: 6d5f 6e61 6d65 4000 0000 7304 0000 0000  m_name@...s.....
-00000dd0: 010c 017a 1c52 6563 6f72 6454 6573 7473  ...z.RecordTests
-00000de0: 2e74 6573 745f 6375 7374 6f6d 5f6e 616d  .test_custom_nam
-00000df0: 6563 0100 0000 0000 0000 0000 0000 0800  ec..............
-00000e00: 0000 0900 0000 4300 0000 7364 0100 0074  ......C...sd...t
-00000e10: 0064 0164 028d 018f 1e01 0074 0164 0319  .d.d.......t.d..
-00000e20: 00a0 0264 04a1 0101 0057 0064 0004 0004  ...d.....W.d....
-00000e30: 0083 0301 006e 1031 0073 2e30 0001 0001  .....n.1.s.0....
-00000e40: 0001 0059 0001 0074 03a0 0474 05a1 018f  ...Y...t...t....
-00000e50: 487d 0174 0064 0164 028d 018f 1e01 0074  H}.t.d.d.......t
-00000e60: 0164 0319 00a0 0264 05a1 0101 0057 0064  .d.....d.....W.d
-00000e70: 0004 0004 0083 0301 006e 1031 0073 7230  .........n.1.sr0
-00000e80: 0001 0001 0001 0059 0001 0057 0064 0004  .......Y...W.d..
-00000e90: 0004 0083 0301 006e 1031 0073 9030 0001  .......n.1.s.0..
-00000ea0: 0001 0001 0059 0001 0064 067d 027c 016a  .....Y...d.}.|.j
-00000eb0: 067d 0374 077c 0383 017d 047c 027c 0476  .}.t.|...}.|.|.v
-00000ec0: 007d 057c 0590 0173 5074 08a0 0964 077c  .}.|...sPt...d.|
-00000ed0: 0566 0164 087c 027c 0466 02a1 0474 08a0  .f.d.|.|.f...t..
-00000ee0: 0a7c 02a1 0164 0974 0ba0 0ca1 0076 0073  .|...d.t.....v.s
-00000ef0: ec74 08a0 0d74 07a1 0172 f674 08a0 0a74  .t...t...r.t...t
-00000f00: 07a1 016e 0264 0964 0a74 0ba0 0ca1 0076  ...n.d.d.t.....v
-00000f10: 0090 0173 1274 08a0 0d7c 01a1 0190 0172  ...s.t...|.....r
-00000f20: 1c74 08a0 0a7c 01a1 016e 0264 0a74 08a0  .t...|...n.d.t..
-00000f30: 0a7c 03a1 0174 08a0 0a7c 04a1 0164 0b9c  .|...t...|...d..
-00000f40: 0516 007d 0664 0c64 0d7c 0669 0116 007d  ...}.d.d.|.i...}
-00000f50: 0774 0574 08a0 0e7c 07a1 0183 0182 0164  .t.t...|.......d
-00000f60: 0004 007d 0204 007d 0504 007d 037d 0464  ...}...}...}.}.d
-00000f70: 0053 0029 0e4e 723e 0000 0072 3f00 0000  .S.).Nr>...r?...
-00000f80: 7211 0000 0072 2d00 0000 7237 0000 007a  r....r-...r7...z
-00000f90: 2050 6572 666f 726d 616e 6365 2072 6563   Performance rec
-00000fa0: 6f72 6420 6469 6420 6e6f 7420 6d61 7463  ord did not matc
-00000fb0: 68a9 01da 0269 6ea9 017a 4b25 2870 7931  h....in..zK%(py1
-00000fc0: 2973 2069 6e20 2528 7079 3829 730a 7b25  )s in %(py8)s.{%
-00000fd0: 2870 7938 2973 203d 2025 2870 7933 2973  (py8)s = %(py3)s
-00000fe0: 2825 2870 7936 2973 0a7b 2528 7079 3629  (%(py6)s.{%(py6)
-00000ff0: 7320 3d20 2528 7079 3429 732e 7661 6c75  s = %(py4)s.valu
-00001000: 650a 7d29 0a7d da03 7374 72da 0765 7863  e.}).}..str..exc
-00001010: 696e 666f a905 da03 7079 31da 0370 7933  info....py1..py3
-00001020: da03 7079 34da 0370 7936 da03 7079 38fa  ..py4..py6..py8.
-00001030: 0f61 7373 6572 7420 2528 7079 3130 2973  .assert %(py10)s
-00001040: da04 7079 3130 290f 720b 0000 0072 0200  ..py10).r....r..
-00001050: 0000 7235 0000 00da 0670 7974 6573 74da  ..r5.....pytest.
-00001060: 0672 6169 7365 73da 0e41 7373 6572 7469  .raises..Asserti
-00001070: 6f6e 4572 726f 72da 0576 616c 7565 7245  onError..valuerE
-00001080: 0000 00da 0a40 7079 7465 7374 5f61 72da  .....@pytest_ar.
-00001090: 115f 6361 6c6c 5f72 6570 7263 6f6d 7061  ._call_reprcompa
-000010a0: 7265 da09 5f73 6166 6572 6570 72da 0c40  re.._saferepr..@
-000010b0: 7079 5f62 7569 6c74 696e 73da 066c 6f63  py_builtins..loc
-000010c0: 616c 73da 185f 7368 6f75 6c64 5f72 6570  als.._should_rep
-000010d0: 725f 676c 6f62 616c 5f6e 616d 65da 135f  r_global_name.._
-000010e0: 666f 726d 6174 5f65 7870 6c61 6e61 7469  format_explanati
-000010f0: 6f6e 2908 7215 0000 0072 4600 0000 da0b  on).r....rF.....
-00001100: 4070 795f 6173 7365 7274 30da 0b40 7079  @py_assert0..@py
-00001110: 5f61 7373 6572 7435 da0b 4070 795f 6173  _assert5..@py_as
-00001120: 7365 7274 37da 0b40 7079 5f61 7373 6572  sert7..@py_asser
-00001130: 7432 da0b 4070 795f 666f 726d 6174 39da  t2..@py_format9.
-00001140: 0c40 7079 5f66 6f72 6d61 7431 3172 1600  .@py_format11r..
-00001150: 0000 7216 0000 0072 1700 0000 da1f 7465  ..r....r......te
-00001160: 7374 5f63 7573 746f 6d5f 6e61 6d65 5f6d  st_custom_name_m
-00001170: 756c 7469 706c 655f 6361 6c6c 7344 0000  ultiple_callsD..
-00001180: 0073 0c00 0000 0001 0c01 2c02 0c01 0c01  .s........,.....
-00001190: 4a02 7a2b 5265 636f 7264 5465 7374 732e  J.z+RecordTests.
-000011a0: 7465 7374 5f63 7573 746f 6d5f 6e61 6d65  test_custom_name
-000011b0: 5f6d 756c 7469 706c 655f 6361 6c6c 7363  _multiple_callsc
-000011c0: 0100 0000 0000 0000 0000 0000 0700 0000  ................
-000011d0: 0a00 0000 4300 0000 73ca 0100 0074 0083  ....C...s....t..
-000011e0: 0090 018f ac01 0074 0164 0164 028d 018f  .......t.d.d....
-000011f0: 1e01 0074 0264 0319 00a0 0364 04a1 0101  ...t.d.....d....
-00001200: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00001210: 0073 3830 0001 0001 0001 0059 0001 0074  .s80.......Y...t
-00001220: 04a0 0574 06a1 018f 487d 0174 0164 0164  ...t....H}.t.d.d
-00001230: 028d 018f 1e01 0074 0264 0319 00a0 0364  .......t.d.....d
-00001240: 05a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00001250: 006e 1031 0073 7c30 0001 0001 0001 0059  .n.1.s|0.......Y
-00001260: 0001 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00001270: 1031 0073 9a30 0001 0001 0001 0059 0001  .1.s.0.......Y..
-00001280: 0074 077c 016a 0883 017d 0264 067d 037c  .t.|.j...}.d.}.|
-00001290: 037c 0276 007d 047c 0490 0173 2074 09a0  .|.v.}.|...s t..
-000012a0: 0a64 077c 0466 0164 087c 037c 0266 02a1  .d.|.f.d.|.|.f..
-000012b0: 0474 09a0 0b7c 03a1 0164 0974 0ca0 0da1  .t...|...d.t....
-000012c0: 0076 0073 f274 09a0 0e7c 02a1 0172 fc74  .v.s.t...|...r.t
-000012d0: 09a0 0b7c 02a1 016e 0264 0964 0a9c 0216  ...|...n.d.d....
-000012e0: 007d 0564 0b64 0c7c 0569 0116 007d 0674  .}.d.d.|.i...}.t
-000012f0: 0674 09a0 0f7c 06a1 0183 0182 0164 0004  .t...|.......d..
-00001300: 007d 037d 0464 0d7d 037c 037c 0276 007d  .}.}.d.}.|.|.v.}
-00001310: 047c 0490 0173 9e74 09a0 0a64 077c 0466  .|...s.t...d.|.f
-00001320: 0164 087c 037c 0266 02a1 0474 09a0 0b7c  .d.|.|.f...t...|
-00001330: 03a1 0164 0974 0ca0 0da1 0076 0090 0173  ...d.t.....v...s
-00001340: 7074 09a0 0e7c 02a1 0190 0172 7a74 09a0  pt...|.....rzt..
-00001350: 0b7c 02a1 016e 0264 0964 0a9c 0216 007d  .|...n.d.d.....}
-00001360: 0564 0b64 0c7c 0569 0116 007d 0674 0674  .d.d.|.i...}.t.t
-00001370: 09a0 0f7c 06a1 0183 0182 0164 0004 007d  ...|.......d...}
-00001380: 037d 0457 0064 0004 0004 0083 0301 006e  .}.W.d.........n
-00001390: 1231 0090 0173 bc30 0001 0001 0001 0059  .1...s.0.......Y
-000013a0: 0001 0064 0053 0029 0e4e da09 7465 7374  ...d.S.).N..test
-000013b0: 5f64 6966 6672 3f00 0000 7211 0000 0072  _diffr?...r....r
-000013c0: 2d00 0000 7237 0000 007a 112d 2063 6163  -...r7...z.- cac
-000013d0: 6865 7c67 6574 3a20 666f 6f0a 7242 0000  he|get: foo.rB..
-000013e0: 0029 017a 1225 2870 7931 2973 2069 6e20  .).z.%(py1)s in 
-000013f0: 2528 7079 3329 73da 036d 7367 2902 7248  %(py3)s..msg).rH
-00001400: 0000 0072 4900 0000 7a0e 6173 7365 7274  ...rI...z.assert
-00001410: 2025 2870 7935 2973 da03 7079 357a 112b   %(py5)s..py5z.+
-00001420: 2063 6163 6865 7c67 6574 3a20 6261 720a   cache|get: bar.
-00001430: 2910 720d 0000 0072 0b00 0000 7202 0000  ).r....r....r...
-00001440: 0072 3500 0000 724f 0000 0072 5000 0000  .r5...rO...rP...
-00001450: 7251 0000 0072 4500 0000 7252 0000 0072  rQ...rE...rR...r
-00001460: 5300 0000 7254 0000 0072 5500 0000 7256  S...rT...rU...rV
-00001470: 0000 0072 5700 0000 7258 0000 0072 5900  ...rW...rX...rY.
-00001480: 0000 2907 7215 0000 0072 4600 0000 7262  ..).r....rF...rb
-00001490: 0000 0072 5a00 0000 725d 0000 00da 0b40  ...rZ...r].....@
-000014a0: 7079 5f66 6f72 6d61 7434 da0b 4070 795f  py_format4..@py_
-000014b0: 666f 726d 6174 3672 1600 0000 7216 0000  format6r....r...
-000014c0: 0072 1700 0000 7261 0000 004e 0000 0073  .r....ra...N...s
-000014d0: 1200 0000 0001 0a01 0c01 2c02 0c01 0c01  ..........,.....
-000014e0: 4a02 0a01 7a01 7a15 5265 636f 7264 5465  J...z.z.RecordTe
-000014f0: 7374 732e 7465 7374 5f64 6966 6663 0100  sts.test_diffc..
-00001500: 0000 0000 0000 0000 0000 0600 0000 0900  ................
-00001510: 0000 4300 0000 73ea 0000 0074 0064 0183  ..C...s....t.d..
-00001520: 018f ce01 0074 0164 0164 028d 018f 1e01  .....t.d.d......
-00001530: 0074 0264 0319 00a0 0364 04a1 0101 0057  .t.d.....d.....W
-00001540: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-00001550: 3830 0001 0001 0001 0059 0001 0074 046a  80.......Y...t.j
-00001560: 057d 017c 016a 067d 0264 017d 037c 027c  .}.|.j.}.d.}.|.|
-00001570: 0383 017d 047c 0473 b864 0564 0674 07a0  ...}.|.s.d.d.t..
-00001580: 08a1 0076 0073 7674 09a0 0a74 04a1 0172  ...v.svt...t...r
-00001590: 8074 09a0 0b74 04a1 016e 0264 0674 09a0  .t...t...n.d.t..
-000015a0: 0b7c 01a1 0174 09a0 0b7c 02a1 0174 09a0  .|...t...|...t..
-000015b0: 0b7c 03a1 0174 09a0 0b7c 04a1 0164 079c  .|...t...|...d..
-000015c0: 0516 007d 0574 0c74 09a0 0d7c 05a1 0183  ...}.t.t...|....
-000015d0: 0182 0164 0004 007d 0104 007d 0204 007d  ...d...}...}...}
-000015e0: 037d 0457 0064 0004 0004 0083 0301 006e  .}.W.d.........n
-000015f0: 1031 0073 dc30 0001 0001 0001 0059 0001  .1.s.0.......Y..
-00001600: 0064 0053 0029 084e fa0f 6375 7374 6f6d  .d.S.).N..custom
-00001610: 2e70 6572 662e 796d 6ca9 01da 0470 6174  .perf.yml....pat
-00001620: 6872 1100 0000 722d 0000 007a 6261 7373  hr....r-...zbass
-00001630: 6572 7420 2528 7079 3829 730a 7b25 2870  ert %(py8)s.{%(p
-00001640: 7938 2973 203d 2025 2870 7934 2973 0a7b  y8)s = %(py4)s.{
-00001650: 2528 7079 3429 7320 3d20 2528 7079 3229  %(py4)s = %(py2)
-00001660: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
-00001670: 7930 2973 2e70 6174 680a 7d2e 6578 6973  y0)s.path.}.exis
-00001680: 7473 0a7d 2825 2870 7936 2973 290a 7dda  ts.}(%(py6)s).}.
-00001690: 026f 7329 05da 0370 7930 da03 7079 3272  .os)...py0..py2r
-000016a0: 4a00 0000 724b 0000 0072 4c00 0000 290e  J...rK...rL...).
-000016b0: 720f 0000 0072 0b00 0000 7202 0000 0072  r....r....r....r
-000016c0: 3500 0000 7269 0000 0072 6800 0000 da06  5...ri...rh.....
-000016d0: 6578 6973 7473 7256 0000 0072 5700 0000  existsrV...rW...
-000016e0: 7253 0000 0072 5800 0000 7255 0000 0072  rS...rX...rU...r
-000016f0: 5100 0000 7259 0000 0029 0672 1500 0000  Q...rY...).r....
-00001700: da0b 4070 795f 6173 7365 7274 31da 0b40  ..@py_assert1..@
-00001710: 7079 5f61 7373 6572 7433 725b 0000 0072  py_assert3r[...r
-00001720: 5c00 0000 725e 0000 0072 1600 0000 7216  \...r^...r....r.
-00001730: 0000 0072 1700 0000 da1e 7465 7374 5f70  ...r......test_p
-00001740: 6174 685f 706f 696e 7469 6e67 5f74 6f5f  ath_pointing_to_
-00001750: 6669 6c65 6e61 6d65 5b00 0000 7308 0000  filename[...s...
-00001760: 0000 010a 020c 012c 027a 2a52 6563 6f72  .......,.z*Recor
-00001770: 6454 6573 7473 2e74 6573 745f 7061 7468  dTests.test_path
-00001780: 5f70 6f69 6e74 696e 675f 746f 5f66 696c  _pointing_to_fil
-00001790: 656e 616d 6563 0100 0000 0000 0000 0000  enamec..........
-000017a0: 0000 0100 0000 0900 0000 4300 0000 739c  ..........C...s.
-000017b0: 0000 0074 0064 0183 018f 8001 0074 0164  ...t.d.......t.d
-000017c0: 0164 028d 018f 1e01 0074 0264 0319 00a0  .d.......t.d....
-000017d0: 0364 04a1 0101 0057 0064 0004 0004 0083  .d.....W.d......
-000017e0: 0301 006e 1031 0073 3830 0001 0001 0001  ...n.1.s80......
-000017f0: 0059 0001 0074 0164 0164 028d 018f 1e01  .Y...t.d.d......
-00001800: 0074 0264 0319 00a0 0364 04a1 0101 0057  .t.d.....d.....W
-00001810: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-00001820: 7030 0001 0001 0001 0059 0001 0057 0064  p0.......Y...W.d
-00001830: 0004 0004 0083 0301 006e 1031 0073 8e30  .........n.1.s.0
-00001840: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00001850: 054e 7266 0000 0072 6700 0000 7211 0000  .Nrf...rg...r...
-00001860: 0072 2d00 0000 2904 720f 0000 0072 0b00  .r-...).r....r..
-00001870: 0000 7202 0000 0072 3500 0000 7214 0000  ..r....r5...r...
-00001880: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00001890: da2b 7465 7374 5f70 6174 685f 706f 696e  .+test_path_poin
-000018a0: 7469 6e67 5f74 6f5f 6669 6c65 6e61 6d65  ting_to_filename
-000018b0: 5f72 6563 6f72 645f 7477 6963 6563 0000  _record_twicec..
-000018c0: 0073 0a00 0000 0001 0a02 0c01 2c02 0c01  .s..........,...
-000018d0: 7a37 5265 636f 7264 5465 7374 732e 7465  z7RecordTests.te
-000018e0: 7374 5f70 6174 685f 706f 696e 7469 6e67  st_path_pointing
-000018f0: 5f74 6f5f 6669 6c65 6e61 6d65 5f72 6563  _to_filename_rec
-00001900: 6f72 645f 7477 6963 6563 0100 0000 0000  ord_twicec......
-00001910: 0000 0000 0000 0700 0000 0900 0000 4300  ..............C.
-00001920: 0000 731c 0100 0074 006a 01a0 0274 0364  ..s....t.j...t.d
-00001930: 01a1 027d 0174 047c 0183 018f f001 0074  ...}.t.|.......t
-00001940: 0564 0164 028d 018f 1e01 0074 0664 0319  .d.d.......t.d..
-00001950: 00a0 0764 04a1 0101 0057 0064 0004 0004  ...d.....W.d....
-00001960: 0083 0301 006e 1031 0073 4630 0001 0001  .....n.1.sF0....
-00001970: 0001 0059 0001 0074 006a 01a0 0274 0364  ...Y...t.j...t.d
-00001980: 0564 06a1 037d 0274 006a 017d 037c 036a  .d...}.t.j.}.|.j
-00001990: 087d 047c 047c 0283 017d 057c 0573 ec64  .}.|.|...}.|.s.d
-000019a0: 0764 0874 09a0 0aa1 0076 0073 9074 0ba0  .d.t.....v.s.t..
-000019b0: 0c74 00a1 0172 9a74 0ba0 0d74 00a1 016e  .t...r.t...t...n
-000019c0: 0264 0874 0ba0 0d7c 03a1 0174 0ba0 0d7c  .d.t...|...t...|
-000019d0: 04a1 0164 0974 09a0 0aa1 0076 0073 c274  ...d.t.....v.s.t
-000019e0: 0ba0 0c7c 02a1 0172 cc74 0ba0 0d7c 02a1  ...|...r.t...|..
-000019f0: 016e 0264 0974 0ba0 0d7c 05a1 0164 0a9c  .n.d.t...|...d..
-00001a00: 0516 007d 0674 0e74 0ba0 0f7c 06a1 0183  ...}.t.t...|....
-00001a10: 0182 0164 0004 007d 0304 007d 047d 0557  ...d...}...}.}.W
-00001a20: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
-00001a30: 0173 0e30 0001 0001 0001 0059 0001 0064  .s.0.......Y...d
-00001a40: 0053 0029 0b4e fa0b 7065 7266 5f66 696c  .S.).N..perf_fil
-00001a50: 6573 2f72 6700 0000 7211 0000 0072 2d00  es/rg...r....r-.
-00001a60: 0000 da0a 7065 7266 5f66 696c 6573 fa11  ....perf_files..
-00001a70: 7465 7374 5f61 7069 2e70 6572 662e 796d  test_api.perf.ym
-00001a80: 6cfa 6261 7373 6572 7420 2528 7079 3729  l.bassert %(py7)
-00001a90: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
-00001aa0: 7934 2973 0a7b 2528 7079 3429 7320 3d20  y4)s.{%(py4)s = 
-00001ab0: 2528 7079 3229 730a 7b25 2870 7932 2973  %(py2)s.{%(py2)s
-00001ac0: 203d 2025 2870 7930 2973 2e70 6174 680a   = %(py0)s.path.
-00001ad0: 7d2e 6578 6973 7473 0a7d 2825 2870 7935  }.exists.}(%(py5
-00001ae0: 2973 290a 7d72 6900 0000 da09 6675 6c6c  )s).}ri.....full
-00001af0: 5f70 6174 68a9 0572 6a00 0000 726b 0000  _path..rj...rk..
-00001b00: 0072 4a00 0000 7263 0000 00da 0370 7937  .rJ...rc.....py7
-00001b10: a910 7269 0000 0072 6800 0000 da04 6a6f  ..ri...rh.....jo
-00001b20: 696e da08 4649 4c45 5f44 4952 720f 0000  in..FILE_DIRr...
-00001b30: 0072 0b00 0000 7202 0000 0072 3500 0000  .r....r....r5...
-00001b40: 726c 0000 0072 5600 0000 7257 0000 0072  rl...rV...rW...r
-00001b50: 5300 0000 7258 0000 0072 5500 0000 7251  S...rX...rU...rQ
-00001b60: 0000 0072 5900 0000 a907 7215 0000 00da  ...rY.....r.....
-00001b70: 0874 656d 705f 6469 7272 7500 0000 726d  .temp_dirru...rm
-00001b80: 0000 0072 6e00 0000 da0b 4070 795f 6173  ...rn.....@py_as
-00001b90: 7365 7274 36da 0b40 7079 5f66 6f72 6d61  sert6..@py_forma
-00001ba0: 7438 7216 0000 0072 1600 0000 7217 0000  t8r....r....r...
-00001bb0: 00da 1974 6573 745f 7061 7468 5f70 6f69  ...test_path_poi
-00001bc0: 6e74 696e 675f 746f 5f64 6972 6c00 0000  nting_to_dirl...
-00001bd0: 730c 0000 0000 010e 010a 020c 012c 0210  s............,..
-00001be0: 017a 2552 6563 6f72 6454 6573 7473 2e74  .z%RecordTests.t
-00001bf0: 6573 745f 7061 7468 5f70 6f69 6e74 696e  est_path_pointin
-00001c00: 675f 746f 5f64 6972 6301 0000 0000 0000  g_to_dirc.......
-00001c10: 0000 0000 0007 0000 0009 0000 0043 0000  .............C..
-00001c20: 0073 1e01 0000 7400 6a01 a002 7403 6401  .s....t.j...t.d.
-00001c30: a102 7d01 7404 7c01 8301 8ff2 0100 7405  ..}.t.|.......t.
-00001c40: 6402 6403 8d01 8f1e 0100 7406 6404 1900  d.d.......t.d...
-00001c50: a007 6405 a101 0100 5700 6400 0400 0400  ..d.....W.d.....
-00001c60: 8303 0100 6e10 3100 7346 3000 0100 0100  ....n.1.sF0.....
-00001c70: 0100 5900 0100 7400 6a01 a002 7403 6406  ..Y...t.j...t.d.
-00001c80: 6407 6408 a104 7d02 7400 6a01 7d03 7c03  d.d...}.t.j.}.|.
-00001c90: 6a08 7d04 7c04 7c02 8301 7d05 7c05 73ee  j.}.|.|...}.|.s.
-00001ca0: 6409 640a 7409 a00a a100 7600 7392 740b  d.d.t.....v.s.t.
-00001cb0: a00c 7400 a101 729c 740b a00d 7400 a101  ..t...r.t...t...
-00001cc0: 6e02 640a 740b a00d 7c03 a101 740b a00d  n.d.t...|...t...
-00001cd0: 7c04 a101 640b 7409 a00a a100 7600 73c4  |...d.t.....v.s.
-00001ce0: 740b a00c 7c02 a101 72ce 740b a00d 7c02  t...|...r.t...|.
-00001cf0: a101 6e02 640b 740b a00d 7c05 a101 640c  ..n.d.t...|...d.
-00001d00: 9c05 1600 7d06 740e 740b a00f 7c06 a101  ....}.t.t...|...
-00001d10: 8301 8201 6400 0400 7d03 0400 7d04 7d05  ....d...}...}.}.
-00001d20: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
-00001d30: 9001 7310 3000 0100 0100 0100 5900 0100  ..s.0.......Y...
-00001d40: 6400 5300 a90d 4e72 7100 0000 fa0f 7065  d.S...Nrq.....pe
-00001d50: 7266 5f66 696c 6573 2f61 7069 2f72 6700  rf_files/api/rg.
-00001d60: 0000 7211 0000 0072 2d00 0000 7272 0000  ..r....r-...rr..
-00001d70: 00da 0361 7069 7273 0000 0072 7400 0000  ...apirs...rt...
-00001d80: 7269 0000 0072 7500 0000 7276 0000 0072  ri...ru...rv...r
-00001d90: 7800 0000 727b 0000 0072 1600 0000 7216  x...r{...r....r.
-00001da0: 0000 0072 1700 0000 da17 7465 7374 5f63  ...r......test_c
-00001db0: 7573 746f 6d5f 6e65 7374 6564 5f70 6174  ustom_nested_pat
-00001dc0: 6876 0000 0073 0c00 0000 0001 0e01 0a02  hv...s..........
-00001dd0: 0c01 2c02 1201 7a23 5265 636f 7264 5465  ..,...z#RecordTe
-00001de0: 7374 732e 7465 7374 5f63 7573 746f 6d5f  sts.test_custom_
-00001df0: 6e65 7374 6564 5f70 6174 68da 044d 4f44  nested_path..MOD
-00001e00: 45da 046f 6e63 6563 0100 0000 0000 0000  E..oncec........
-00001e10: 0000 0000 0700 0000 0900 0000 4300 0000  ............C...
-00001e20: 731e 0100 0074 006a 01a0 0274 0364 01a1  s....t.j...t.d..
-00001e30: 027d 0174 047c 0183 018f f201 0074 0564  .}.t.|.......t.d
-00001e40: 0264 038d 018f 1e01 0074 0664 0419 00a0  .d.......t.d....
-00001e50: 0764 05a1 0101 0057 0064 0004 0004 0083  .d.....W.d......
-00001e60: 0301 006e 1031 0073 4630 0001 0001 0001  ...n.1.sF0......
-00001e70: 0059 0001 0074 006a 01a0 0274 0364 0664  .Y...t.j...t.d.d
-00001e80: 0764 08a1 047d 0274 006a 017d 037c 036a  .d...}.t.j.}.|.j
-00001e90: 087d 047c 047c 0283 017d 057c 0573 ee64  .}.|.|...}.|.s.d
-00001ea0: 0964 0a74 09a0 0aa1 0076 0073 9274 0ba0  .d.t.....v.s.t..
-00001eb0: 0c74 00a1 0172 9c74 0ba0 0d74 00a1 016e  .t...r.t...t...n
-00001ec0: 0264 0a74 0ba0 0d7c 03a1 0174 0ba0 0d7c  .d.t...|...t...|
-00001ed0: 04a1 0164 0b74 09a0 0aa1 0076 0073 c474  ...d.t.....v.s.t
-00001ee0: 0ba0 0c7c 02a1 0172 ce74 0ba0 0d7c 02a1  ...|...r.t...|..
-00001ef0: 016e 0264 0b74 0ba0 0d7c 05a1 0164 0c9c  .n.d.t...|...d..
-00001f00: 0516 007d 0674 0e74 0ba0 0f7c 06a1 0183  ...}.t.t...|....
-00001f10: 0182 0164 0004 007d 0304 007d 047d 0557  ...d...}...}.}.W
-00001f20: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
-00001f30: 0173 1030 0001 0001 0001 0059 0001 0064  .s.0.......Y...d
-00001f40: 0053 0072 8000 0000 7278 0000 0072 7b00  .S.r....rx...r{.
-00001f50: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001f60: 00da 0e74 6573 745f 6d6f 6465 5f6f 6e63  ...test_mode_onc
-00001f70: 6580 0000 0073 0c00 0000 0002 0e01 0a02  e....s..........
-00001f80: 0c01 2c02 1201 7a1a 5265 636f 7264 5465  ..,...z.RecordTe
-00001f90: 7374 732e 7465 7374 5f6d 6f64 655f 6f6e  sts.test_mode_on
-00001fa0: 6365 da04 6e6f 6e65 6301 0000 0000 0000  ce..nonec.......
-00001fb0: 0000 0000 000e 0000 000a 0000 0043 0000  .............C..
-00001fc0: 0073 2002 0000 7400 6a01 a002 7403 6401  .s ...t.j...t.d.
-00001fd0: a102 7d01 7404 7c01 8301 9001 8ff2 0100  ..}.t.|.........
-00001fe0: 7405 a006 7407 a101 8f48 7d02 7408 6402  t...t....H}.t.d.
-00001ff0: 6403 8d01 8f1e 0100 7409 6404 1900 a00a  d.......t.d.....
-00002000: 6405 a101 0100 5700 6400 0400 0400 8303  d.....W.d.......
-00002010: 0100 6e10 3100 7354 3000 0100 0100 0100  ..n.1.sT0.......
-00002020: 5900 0100 5700 6400 0400 0400 8303 0100  Y...W.d.........
-00002030: 6e10 3100 7372 3000 0100 0100 0100 5900  n.1.sr0.......Y.
-00002040: 0100 6406 7d03 7c02 6a0b 7d04 740c 7c04  ..d.}.|.j.}.t.|.
-00002050: 8301 7d05 7c03 7c05 7600 7d06 7c06 9001  ..}.|.|.v.}.|...
-00002060: 732e 740d a00e 6407 7c06 6601 6408 7c03  s.t...d.|.f.d.|.
-00002070: 7c05 6602 a104 740d a00f 7c03 a101 6409  |.f...t...|...d.
-00002080: 7410 a011 a100 7600 73ce 740d a012 740c  t.....v.s.t...t.
-00002090: a101 72d8 740d a00f 740c a101 6e02 6409  ..r.t...t...n.d.
-000020a0: 640a 7410 a011 a100 7600 73f0 740d a012  d.t.....v.s.t...
-000020b0: 7c02 a101 72fa 740d a00f 7c02 a101 6e02  |...r.t...|...n.
-000020c0: 640a 740d a00f 7c04 a101 740d a00f 7c05  d.t...|...t...|.
-000020d0: a101 640b 9c05 1600 7d07 640c 640d 7c07  ..d.....}.d.d.|.
-000020e0: 6901 1600 7d08 7407 740d a013 7c08 a101  i...}.t.t...|...
-000020f0: 8301 8201 6400 0400 7d03 0400 7d06 0400  ....d...}...}...
-00002100: 7d04 7d05 7400 6a01 a002 7403 640e 640f  }.}.t.j...t.d.d.
-00002110: 6410 a104 7d09 7400 6a01 7d0a 7c0a 6a14  d...}.t.j.}.|.j.
-00002120: 7d0b 7c0b 7c09 8301 7d0c 7c0c 0c00 7d0d  }.|.|...}.|...}.
-00002130: 7c0d 9001 73ec 6411 6412 7410 a011 a100  |...s.d.d.t.....
-00002140: 7600 9001 738c 740d a012 7400 a101 9001  v...s.t...t.....
-00002150: 7296 740d a00f 7400 a101 6e02 6412 740d  r.t...t...n.d.t.
-00002160: a00f 7c0a a101 740d a00f 7c0b a101 6413  ..|...t...|...d.
-00002170: 7410 a011 a100 7600 9001 73c2 740d a012  t.....v...s.t...
-00002180: 7c09 a101 9001 72cc 740d a00f 7c09 a101  |.....r.t...|...
-00002190: 6e02 6413 740d a00f 7c0c a101 6414 9c05  n.d.t...|...d...
-000021a0: 1600 7d07 7407 740d a013 7c07 a101 8301  ..}.t.t...|.....
-000021b0: 8201 6400 0400 7d0a 0400 7d0b 0400 7d0c  ..d...}...}...}.
-000021c0: 7d0d 5700 6400 0400 0400 8303 0100 6e12  }.W.d.........n.
-000021d0: 3100 9002 7312 3000 0100 0100 0100 5900  1...s.0.......Y.
-000021e0: 0100 6400 5300 2915 4e72 7100 0000 7281  ..d.S.).Nrq...r.
-000021f0: 0000 0072 6700 0000 7211 0000 0072 2d00  ...rg...r....r-.
-00002200: 0000 7a2a 4f72 6967 696e 616c 2070 6572  ..z*Original per
-00002210: 666f 726d 616e 6365 2072 6563 6f72 6420  formance record 
-00002220: 646f 6573 206e 6f74 2065 7869 7374 7242  does not existrB
-00002230: 0000 0072 4400 0000 7245 0000 0072 4600  ...rD...rE...rF.
-00002240: 0000 7247 0000 0072 4d00 0000 724e 0000  ..rG...rM...rN..
-00002250: 0072 7200 0000 7282 0000 0072 7300 0000  .rr...r....rs...
-00002260: 7a66 6173 7365 7274 206e 6f74 2025 2870  zfassert not %(p
-00002270: 7937 2973 0a7b 2528 7079 3729 7320 3d20  y7)s.{%(py7)s = 
-00002280: 2528 7079 3429 730a 7b25 2870 7934 2973  %(py4)s.{%(py4)s
-00002290: 203d 2025 2870 7932 2973 0a7b 2528 7079   = %(py2)s.{%(py
-000022a0: 3229 7320 3d20 2528 7079 3029 732e 7061  2)s = %(py0)s.pa
-000022b0: 7468 0a7d 2e65 7869 7374 730a 7d28 2528  th.}.exists.}(%(
-000022c0: 7079 3529 7329 0a7d 7269 0000 0072 7500  py5)s).}ri...ru.
-000022d0: 0000 7276 0000 00a9 1572 6900 0000 7268  ..rv.....ri...rh
-000022e0: 0000 0072 7900 0000 727a 0000 0072 0f00  ...ry...rz...r..
-000022f0: 0000 724f 0000 0072 5000 0000 7251 0000  ..rO...rP...rQ..
-00002300: 0072 0b00 0000 7202 0000 0072 3500 0000  .r....r....r5...
-00002310: 7252 0000 0072 4500 0000 7253 0000 0072  rR...rE...rS...r
-00002320: 5400 0000 7255 0000 0072 5600 0000 7257  T...rU...rV...rW
-00002330: 0000 0072 5800 0000 7259 0000 0072 6c00  ...rX...rY...rl.
-00002340: 0000 290e 7215 0000 0072 7c00 0000 7246  ..).r....r|...rF
-00002350: 0000 0072 5a00 0000 725b 0000 0072 5c00  ...rZ...r[...r\.
-00002360: 0000 725d 0000 0072 5e00 0000 725f 0000  ..r]...r^...r_..
-00002370: 0072 7500 0000 726d 0000 0072 6e00 0000  .ru...rm...rn...
-00002380: 727d 0000 00da 0b40 7079 5f61 7373 6572  r}.....@py_asser
-00002390: 7438 7216 0000 0072 1600 0000 7217 0000  t8r....r....r...
-000023a0: 00da 0e74 6573 745f 6d6f 6465 5f6e 6f6e  ...test_mode_non
-000023b0: 658b 0000 0073 1000 0000 0002 0e01 0c02  e....s..........
-000023c0: 0c02 0c01 4a02 c202 1201 7a1a 5265 636f  ....J.....z.Reco
-000023d0: 7264 5465 7374 732e 7465 7374 5f6d 6f64  rdTests.test_mod
-000023e0: 655f 6e6f 6e65 721d 0000 0063 0100 0000  e_noner....c....
-000023f0: 0000 0000 0000 0000 0e00 0000 0a00 0000  ................
-00002400: 4300 0000 7316 0200 0074 006a 01a0 0274  C...s....t.j...t
-00002410: 0364 01a1 027d 0174 047c 0183 0190 018f  .d...}.t.|......
-00002420: e801 0074 05a0 0674 07a1 018f 487d 0274  ...t...t....H}.t
-00002430: 0864 0264 038d 018f 1e01 0074 0964 0419  .d.d.......t.d..
-00002440: 00a0 0a64 05a1 0101 0057 0064 0004 0004  ...d.....W.d....
-00002450: 0083 0301 006e 1031 0073 5430 0001 0001  .....n.1.sT0....
-00002460: 0001 0059 0001 0057 0064 0004 0004 0083  ...Y...W.d......
-00002470: 0301 006e 1031 0073 7230 0001 0001 0001  ...n.1.sr0......
-00002480: 0059 0001 0064 067d 037c 026a 0b7d 0474  .Y...d.}.|.j.}.t
-00002490: 0c7c 0483 017d 057c 037c 0576 007d 067c  .|...}.|.|.v.}.|
-000024a0: 0690 0173 2e74 0da0 0e64 077c 0666 0164  ...s.t...d.|.f.d
-000024b0: 087c 037c 0566 02a1 0474 0da0 0f7c 03a1  .|.|.f...t...|..
-000024c0: 0164 0974 10a0 11a1 0076 0073 ce74 0da0  .d.t.....v.s.t..
-000024d0: 1274 0ca1 0172 d874 0da0 0f74 0ca1 016e  .t...r.t...t...n
-000024e0: 0264 0964 0a74 10a0 11a1 0076 0073 f074  .d.d.t.....v.s.t
-000024f0: 0da0 127c 02a1 0172 fa74 0da0 0f7c 02a1  ...|...r.t...|..
-00002500: 016e 0264 0a74 0da0 0f7c 04a1 0174 0da0  .n.d.t...|...t..
-00002510: 0f7c 05a1 0164 0b9c 0516 007d 0764 0c64  .|...d.....}.d.d
-00002520: 0d7c 0769 0116 007d 0874 0774 0da0 137c  .|.i...}.t.t...|
-00002530: 08a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
-00002540: 0604 007d 047d 0574 006a 01a0 0274 0364  ...}.}.t.j...t.d
-00002550: 0e64 0f64 10a1 047d 0974 006a 017d 0a7c  .d.d...}.t.j.}.|
-00002560: 0a6a 147d 0b7c 0b7c 0983 017d 0c7c 0c90  .j.}.|.|...}.|..
-00002570: 0173 e664 1164 1274 10a0 11a1 0076 0090  .s.d.d.t.....v..
-00002580: 0173 8674 0da0 1274 00a1 0190 0172 9074  .s.t...t.....r.t
-00002590: 0da0 0f74 00a1 016e 0264 1274 0da0 0f7c  ...t...n.d.t...|
-000025a0: 0aa1 0174 0da0 0f7c 0ba1 0164 1374 10a0  ...t...|...d.t..
-000025b0: 11a1 0076 0090 0173 bc74 0da0 127c 09a1  ...v...s.t...|..
-000025c0: 0190 0172 c674 0da0 0f7c 09a1 016e 0264  ...r.t...|...n.d
-000025d0: 1374 0da0 0f7c 0ca1 0164 149c 0516 007d  .t...|...d.....}
-000025e0: 0d74 0774 0da0 137c 0da1 0183 0182 0164  .t.t...|.......d
-000025f0: 0004 007d 0a04 007d 0b7d 0c57 0064 0004  ...}...}.}.W.d..
-00002600: 0004 0083 0301 006e 1231 0090 0273 0830  .......n.1...s.0
-00002610: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
-00002620: 154e 7271 0000 0072 8100 0000 7267 0000  .Nrq...r....rg..
-00002630: 0072 1100 0000 722d 0000 007a 294f 7269  .r....r-...z)Ori
-00002640: 6769 6e61 6c20 7065 7266 6f72 6d61 6e63  ginal performanc
-00002650: 6520 7265 636f 7264 2064 6964 206e 6f74  e record did not
-00002660: 2065 7869 7374 7242 0000 0072 4400 0000   existrB...rD...
-00002670: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
-00002680: 4d00 0000 724e 0000 0072 7200 0000 7282  M...rN...rr...r.
-00002690: 0000 0072 7300 0000 7274 0000 0072 6900  ...rs...rt...ri.
-000026a0: 0000 7275 0000 0072 7600 0000 7288 0000  ..ru...rv...r...
-000026b0: 0029 0e72 1500 0000 727c 0000 0072 4600  .).r....r|...rF.
-000026c0: 0000 725a 0000 0072 5b00 0000 725c 0000  ..rZ...r[...r\..
-000026d0: 0072 5d00 0000 725e 0000 0072 5f00 0000  .r]...r^...r_...
-000026e0: 7275 0000 0072 6d00 0000 726e 0000 0072  ru...rm...rn...r
-000026f0: 7d00 0000 727e 0000 0072 1600 0000 7216  }...r~...r....r.
-00002700: 0000 0072 1700 0000 da0d 7465 7374 5f6d  ...r......test_m
-00002710: 6f64 655f 616c 6c9a 0000 0073 1000 0000  ode_all....s....
-00002720: 0002 0e01 0c02 0c02 0c01 4a02 c202 1201  ..........J.....
-00002730: 7a19 5265 636f 7264 5465 7374 732e 7465  z.RecordTests.te
-00002740: 7374 5f6d 6f64 655f 616c 6c63 0100 0000  st_mode_allc....
-00002750: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-00002760: 4300 0000 7342 0000 0074 006a 016a 0264  C...sB...t.j.j.d
-00002770: 0164 0264 038d 027d 0174 0383 008f 1801  .d.d...}.t......
-00002780: 007c 01a0 04a1 0001 0057 0064 0004 0004  .|.......W.d....
-00002790: 0083 0301 006e 1031 0073 3430 0001 0001  .....n.1.s40....
-000027a0: 0001 0059 0001 0064 0053 0029 044e 5a06  ...Y...d.S.).NZ.
-000027b0: 4172 7468 7572 e92a 0000 0072 2f00 0000  Arthur.*...r/...
-000027c0: 2905 720c 0000 0072 1c00 0000 da06 6372  ).r....r......cr
-000027d0: 6561 7465 720b 0000 0072 3b00 0000 2902  eater....r;...).
-000027e0: 7215 0000 005a 0661 7274 6875 7272 1600  r....Z.arthurr..
-000027f0: 0000 7216 0000 0072 1700 0000 da23 7465  ..r....r.....#te
-00002800: 7374 5f64 656c 6574 655f 6f6e 5f63 6173  st_delete_on_cas
-00002810: 6361 6465 5f63 616c 6c65 645f 7477 6963  cade_called_twic
-00002820: 65a9 0000 0073 0600 0000 0001 1001 0801  e....s..........
-00002830: 7a2f 5265 636f 7264 5465 7374 732e 7465  z/RecordTests.te
-00002840: 7374 5f64 656c 6574 655f 6f6e 5f63 6173  st_delete_on_cas
-00002850: 6361 6465 5f63 616c 6c65 645f 7477 6963  cade_called_twic
-00002860: 654e 2919 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
-00002870: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00002880: 616c 6e61 6d65 5f5f 7218 0000 0072 1e00  alname__r....r..
-00002890: 0000 7207 0000 0072 2100 0000 7222 0000  ..r....r!...r"..
-000028a0: 0072 2800 0000 722c 0000 0072 3200 0000  .r(...r,...r2...
-000028b0: 7236 0000 0072 3c00 0000 723d 0000 0072  r6...r<...r=...r
-000028c0: 4100 0000 7260 0000 0072 6100 0000 726f  A...r`...ra...ro
-000028d0: 0000 0072 7000 0000 727f 0000 0072 8300  ...rp...r....r..
-000028e0: 0000 7286 0000 0072 8a00 0000 728b 0000  ..r....r....r...
-000028f0: 0072 8e00 0000 7216 0000 0072 1600 0000  .r....r....r....
-00002900: 7216 0000 0072 1700 0000 7210 0000 0010  r....r....r.....
-00002910: 0000 0073 3200 0000 0801 0804 0804 0c01  ...s2...........
-00002920: 0a04 0805 0804 0804 0804 0804 0806 0807  ................
-00002930: 0804 080a 080d 0808 0809 080a 080a 0c01  ................
-00002940: 0a0a 0c01 0a0e 0c01 0a0e 7210 0000 0063  ..........r....c
-00002950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002960: 0200 0000 4000 0000 7324 0000 0065 005a  ....@...s$...e.Z
-00002970: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-00002980: 0484 005a 0464 0564 0684 005a 0564 0753  ...Z.d.d...Z.d.S
-00002990: 0029 08da 1047 6574 5065 7266 5061 7468  .)...GetPerfPath
-000029a0: 5465 7374 7363 0100 0000 0000 0000 0000  Testsc..........
-000029b0: 0000 0700 0000 0700 0000 4300 0000 73a0  ..........C...s.
-000029c0: 0000 0064 017d 0174 007c 0183 017d 0264  ...d.}.t.|...}.d
-000029d0: 027d 037c 027c 036b 027d 047c 0473 8c74  .}.|.|.k.}.|.s.t
-000029e0: 01a0 0264 037c 0466 0164 047c 027c 0366  ...d.|.f.d.|.|.f
-000029f0: 02a1 0464 0574 03a0 04a1 0076 0073 4674  ...d.t.....v.sFt
-00002a00: 01a0 0574 00a1 0172 5074 01a0 0674 00a1  ...t...rPt...t..
-00002a10: 016e 0264 0574 01a0 067c 01a1 0174 01a0  .n.d.t...|...t..
-00002a20: 067c 02a1 0174 01a0 067c 03a1 0164 069c  .|...t...|...d..
-00002a30: 0416 007d 0564 0764 087c 0569 0116 007d  ...}.d.d.|.i...}
-00002a40: 0674 0774 01a0 087c 06a1 0183 0182 0164  .t.t...|.......d
-00002a50: 0004 007d 0104 007d 0204 007d 047d 0364  ...}...}...}.}.d
-00002a60: 0053 0029 094e fa06 666f 6f2e 7079 fa0c  .S.).N..foo.py..
-00002a70: 666f 6f2e 7065 7266 2e79 6d6c a901 fa02  foo.perf.yml....
-00002a80: 3d3d a901 7a30 2528 7079 3429 730a 7b25  ==..z0%(py4)s.{%
-00002a90: 2870 7934 2973 203d 2025 2870 7930 2973  (py4)s = %(py0)s
-00002aa0: 2825 2870 7932 2973 290a 7d20 3d3d 2025  (%(py2)s).} == %
-00002ab0: 2870 7937 2973 7209 0000 00a9 0472 6a00  (py7)sr......rj.
-00002ac0: 0000 726b 0000 0072 4a00 0000 7277 0000  ..rk...rJ...rw..
-00002ad0: 00fa 0e61 7373 6572 7420 2528 7079 3929  ...assert %(py9)
-00002ae0: 73da 0370 7939 a909 7209 0000 0072 5300  s..py9..r....rS.
-00002af0: 0000 7254 0000 0072 5600 0000 7257 0000  ..rT...rV...rW..
-00002b00: 0072 5800 0000 7255 0000 0072 5100 0000  .rX...rU...rQ...
-00002b10: 7259 0000 00a9 0772 1500 0000 726d 0000  rY.....r....rm..
-00002b20: 0072 6e00 0000 727d 0000 0072 5b00 0000  .rn...r}...r[...
-00002b30: 727e 0000 00da 0c40 7079 5f66 6f72 6d61  r~.....@py_forma
-00002b40: 7431 3072 1600 0000 7216 0000 0072 1700  t10r....r....r..
-00002b50: 0000 da0c 7465 7374 5f70 795f 6669 6c65  ....test_py_file
-00002b60: b000 0000 7302 0000 0000 017a 1d47 6574  ....s......z.Get
-00002b70: 5065 7266 5061 7468 5465 7374 732e 7465  PerfPathTests.te
-00002b80: 7374 5f70 795f 6669 6c65 6301 0000 0000  st_py_filec.....
-00002b90: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
-00002ba0: 0000 0073 a000 0000 6401 7d01 7400 7c01  ...s....d.}.t.|.
-00002bb0: 8301 7d02 6402 7d03 7c02 7c03 6b02 7d04  ..}.d.}.|.|.k.}.
-00002bc0: 7c04 738c 7401 a002 6403 7c04 6601 6404  |.s.t...d.|.f.d.
-00002bd0: 7c02 7c03 6602 a104 6405 7403 a004 a100  |.|.f...d.t.....
-00002be0: 7600 7346 7401 a005 7400 a101 7250 7401  v.sFt...t...rPt.
-00002bf0: a006 7400 a101 6e02 6405 7401 a006 7c01  ..t...n.d.t...|.
-00002c00: a101 7401 a006 7c02 a101 7401 a006 7c03  ..t...|...t...|.
-00002c10: a101 6406 9c04 1600 7d05 6407 6408 7c05  ..d.....}.d.d.|.
-00002c20: 6901 1600 7d06 7407 7401 a008 7c06 a101  i...}.t.t...|...
-00002c30: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-00002c40: 7d04 7d03 6400 5300 2909 4e7a 0766 6f6f  }.}.d.S.).Nz.foo
-00002c50: 2e70 7963 7294 0000 0072 9500 0000 7297  .pycr....r....r.
-00002c60: 0000 0072 0900 0000 7298 0000 0072 9900  ...r....r....r..
-00002c70: 0000 729a 0000 0072 9b00 0000 729c 0000  ..r....r....r...
-00002c80: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00002c90: da0d 7465 7374 5f70 7963 5f66 696c 65b3  ..test_pyc_file.
-00002ca0: 0000 0073 0200 0000 0001 7a1e 4765 7450  ...s......z.GetP
-00002cb0: 6572 6650 6174 6854 6573 7473 2e74 6573  erfPathTests.tes
-00002cc0: 745f 7079 635f 6669 6c65 6301 0000 0000  t_pyc_filec.....
-00002cd0: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
-00002ce0: 0000 0073 a000 0000 6401 7d01 7400 7c01  ...s....d.}.t.|.
-00002cf0: 8301 7d02 6402 7d03 7c02 7c03 6b02 7d04  ..}.d.}.|.|.k.}.
-00002d00: 7c04 738c 7401 a002 6403 7c04 6601 6404  |.s.t...d.|.f.d.
-00002d10: 7c02 7c03 6602 a104 6405 7403 a004 a100  |.|.f...d.t.....
-00002d20: 7600 7346 7401 a005 7400 a101 7250 7401  v.sFt...t...rPt.
-00002d30: a006 7400 a101 6e02 6405 7401 a006 7c01  ..t...n.d.t...|.
-00002d40: a101 7401 a006 7c02 a101 7401 a006 7c03  ..t...|...t...|.
-00002d50: a101 6406 9c04 1600 7d05 6407 6408 7c05  ..d.....}.d.d.|.
-00002d60: 6901 1600 7d06 7407 7401 a008 7c06 a101  i...}.t.t...|...
-00002d70: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-00002d80: 7d04 7d03 6400 5300 2909 4e7a 0866 6f6f  }.}.d.S.).Nz.foo
-00002d90: 2e70 6c6f 627a 1166 6f6f 2e70 6c6f 622e  .plobz.foo.plob.
-00002da0: 7065 7266 2e79 6d6c 7295 0000 0072 9700  perf.ymlr....r..
-00002db0: 0000 7209 0000 0072 9800 0000 7299 0000  ..r....r....r...
-00002dc0: 0072 9a00 0000 729b 0000 0072 9c00 0000  .r....r....r....
-00002dd0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00002de0: 1174 6573 745f 756e 6b6e 6f77 6e5f 6669  .test_unknown_fi
-00002df0: 6c65 b600 0000 7302 0000 0000 017a 2247  le....s......z"G
-00002e00: 6574 5065 7266 5061 7468 5465 7374 732e  etPerfPathTests.
-00002e10: 7465 7374 5f75 6e6b 6e6f 776e 5f66 696c  test_unknown_fil
-00002e20: 654e 2906 728f 0000 0072 9000 0000 7291  eN).r....r....r.
-00002e30: 0000 0072 9e00 0000 729f 0000 0072 a000  ...r....r....r..
-00002e40: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00002e50: 0072 1700 0000 7292 0000 00af 0000 0073  .r....r........s
-00002e60: 0600 0000 0801 0803 0803 7292 0000 0063  ..........r....c
-00002e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002e80: 0200 0000 4000 0000 732c 0000 0065 005a  ....@...s,...e.Z
-00002e90: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-00002ea0: 0484 005a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00002eb0: 0884 005a 0664 0953 0029 0ada 1247 6574  ...Z.d.S.)...Get
-00002ec0: 5265 636f 7264 4e61 6d65 5465 7374 7363  RecordNameTestsc
-00002ed0: 0100 0000 0000 0000 0000 0000 0800 0000  ................
-00002ee0: 0800 0000 4300 0000 73b4 0000 0064 017d  ....C...s....d.}
-00002ef0: 0164 027d 0274 007c 017c 0264 038d 027d  .d.}.t.|.|.d...}
-00002f00: 0364 047d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
-00002f10: 9c74 01a0 0264 057c 0566 0164 067c 037c  .t...d.|.f.d.|.|
-00002f20: 0466 02a1 0464 0774 03a0 04a1 0076 0073  .f...d.t.....v.s
-00002f30: 4e74 01a0 0574 00a1 0172 5874 01a0 0674  Nt...t...rXt...t
-00002f40: 00a1 016e 0264 0774 01a0 067c 01a1 0174  ...n.d.t...|...t
-00002f50: 01a0 067c 02a1 0174 01a0 067c 03a1 0174  ...|...t...|...t
-00002f60: 01a0 067c 04a1 0164 089c 0516 007d 0664  ...|...d.....}.d
-00002f70: 0964 0a7c 0669 0116 007d 0774 0774 01a0  .d.|.i...}.t.t..
-00002f80: 087c 07a1 0183 0182 0164 0004 007d 0104  .|.......d...}..
-00002f90: 007d 0204 007d 0304 007d 057d 0464 0053  .}...}...}.}.d.S
-00002fa0: 0029 0b4e 5a08 466f 6f54 6573 7473 5a08  .).NZ.FooTestsZ.
-00002fb0: 7465 7374 5f62 6172 2902 da0a 636c 6173  test_bar)...clas
-00002fc0: 735f 6e61 6d65 da09 7465 7374 5f6e 616d  s_name..test_nam
-00002fd0: 657a 1146 6f6f 5465 7374 732e 7465 7374  ez.FooTests.test
-00002fe0: 5f62 6172 7295 0000 0029 017a 4e25 2870  _barr....).zN%(p
-00002ff0: 7936 2973 0a7b 2528 7079 3629 7320 3d20  y6)s.{%(py6)s = 
-00003000: 2528 7079 3029 7328 636c 6173 735f 6e61  %(py0)s(class_na
-00003010: 6d65 3d25 2870 7932 2973 2c20 7465 7374  me=%(py2)s, test
-00003020: 5f6e 616d 653d 2528 7079 3429 7329 0a7d  _name=%(py4)s).}
-00003030: 203d 3d20 2528 7079 3929 7372 0a00 0000   == %(py9)sr....
-00003040: a905 726a 0000 0072 6b00 0000 724a 0000  ..rj...rk...rJ..
-00003050: 0072 4b00 0000 729a 0000 00fa 0f61 7373  .rK...r......ass
-00003060: 6572 7420 2528 7079 3131 2973 da04 7079  ert %(py11)s..py
-00003070: 3131 a909 720a 0000 0072 5300 0000 7254  11..r....rS...rT
-00003080: 0000 0072 5600 0000 7257 0000 0072 5800  ...rV...rW...rX.
-00003090: 0000 7255 0000 0072 5100 0000 7259 0000  ..rU...rQ...rY..
-000030a0: 00a9 0872 1500 0000 726d 0000 0072 6e00  ...r....rm...rn.
-000030b0: 0000 725b 0000 0072 8900 0000 725c 0000  ..r[...r....r\..
-000030c0: 0072 9d00 0000 5a0c 4070 795f 666f 726d  .r....Z.@py_form
-000030d0: 6174 3132 7216 0000 0072 1600 0000 7217  at12r....r....r.
-000030e0: 0000 00da 1374 6573 745f 636c 6173 735f  .....test_class_
-000030f0: 616e 645f 7465 7374 bb00 0000 7302 0000  and_test....s...
-00003100: 0000 017a 2647 6574 5265 636f 7264 4e61  ...z&GetRecordNa
-00003110: 6d65 5465 7374 732e 7465 7374 5f63 6c61  meTests.test_cla
-00003120: 7373 5f61 6e64 5f74 6573 7463 0100 0000  ss_and_testc....
-00003130: 0000 0000 0000 0000 0700 0000 0700 0000  ................
-00003140: 4300 0000 73a2 0000 0064 017d 0174 007c  C...s....d.}.t.|
-00003150: 0164 028d 017d 0264 017d 037c 027c 036b  .d...}.d.}.|.|.k
-00003160: 027d 047c 0473 8e74 01a0 0264 037c 0466  .}.|.s.t...d.|.f
-00003170: 0164 047c 027c 0366 02a1 0464 0574 03a0  .d.|.|.f...d.t..
-00003180: 04a1 0076 0073 4874 01a0 0574 00a1 0172  ...v.sHt...t...r
-00003190: 5274 01a0 0674 00a1 016e 0264 0574 01a0  Rt...t...n.d.t..
-000031a0: 067c 01a1 0174 01a0 067c 02a1 0174 01a0  .|...t...|...t..
-000031b0: 067c 03a1 0164 069c 0416 007d 0564 0764  .|...d.....}.d.d
-000031c0: 087c 0569 0116 007d 0674 0774 01a0 087c  .|.i...}.t.t...|
-000031d0: 06a1 0183 0182 0164 0004 007d 0104 007d  .......d...}...}
-000031e0: 0204 007d 047d 0364 0053 0029 094e 5a08  ...}.}.d.S.).NZ.
-000031f0: 7465 7374 5f62 617a a901 72a3 0000 0072  test_baz..r....r
-00003200: 9500 0000 a901 7a3a 2528 7079 3429 730a  ......z:%(py4)s.
-00003210: 7b25 2870 7934 2973 203d 2025 2870 7930  {%(py4)s = %(py0
-00003220: 2973 2874 6573 745f 6e61 6d65 3d25 2870  )s(test_name=%(p
-00003230: 7932 2973 290a 7d20 3d3d 2025 2870 7937  y2)s).} == %(py7
-00003240: 2973 720a 0000 0072 9800 0000 7299 0000  )sr....r....r...
-00003250: 0072 9a00 0000 72a7 0000 0072 9c00 0000  .r....r....r....
-00003260: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00003270: 0e74 6573 745f 6a75 7374 5f74 6573 74c1  .test_just_test.
-00003280: 0000 0073 0200 0000 0001 7a21 4765 7452  ...s......z!GetR
-00003290: 6563 6f72 644e 616d 6554 6573 7473 2e74  ecordNameTests.t
-000032a0: 6573 745f 6a75 7374 5f74 6573 7463 0100  est_just_testc..
-000032b0: 0000 0000 0000 0000 0000 0700 0000 0700  ................
-000032c0: 0000 4300 0000 7342 0100 0064 017d 0174  ..C...sB...d.}.t
-000032d0: 007c 0164 028d 017d 0264 017d 037c 027c  .|.d...}.d.}.|.|
-000032e0: 036b 027d 047c 0473 8e74 01a0 0264 037c  .k.}.|.s.t...d.|
-000032f0: 0466 0164 047c 027c 0366 02a1 0464 0574  .f.d.|.|.f...d.t
-00003300: 03a0 04a1 0076 0073 4874 01a0 0574 00a1  .....v.sHt...t..
-00003310: 0172 5274 01a0 0674 00a1 016e 0264 0574  .rRt...t...n.d.t
-00003320: 01a0 067c 01a1 0174 01a0 067c 02a1 0174  ...|...t...|...t
-00003330: 01a0 067c 03a1 0164 069c 0416 007d 0564  ...|...d.....}.d
-00003340: 0764 087c 0569 0116 007d 0674 0774 01a0  .d.|.i...}.t.t..
-00003350: 087c 06a1 0183 0182 0164 0004 007d 0104  .|.......d...}..
-00003360: 007d 0204 007d 047d 0364 017d 0174 007c  .}...}.}.d.}.t.|
-00003370: 0164 028d 017d 0264 097d 037c 027c 036b  .d...}.d.}.|.|.k
-00003380: 027d 047c 0490 0173 2e74 01a0 0264 037c  .}.|...s.t...d.|
-00003390: 0466 0164 047c 027c 0366 02a1 0464 0574  .f.d.|.|.f...d.t
-000033a0: 03a0 04a1 0076 0073 e874 01a0 0574 00a1  .....v.s.t...t..
-000033b0: 0172 f274 01a0 0674 00a1 016e 0264 0574  .r.t...t...n.d.t
-000033c0: 01a0 067c 01a1 0174 01a0 067c 02a1 0174  ...|...t...|...t
-000033d0: 01a0 067c 03a1 0164 069c 0416 007d 0564  ...|...d.....}.d
-000033e0: 0764 087c 0569 0116 007d 0674 0774 01a0  .d.|.i...}.t.t..
-000033f0: 087c 06a1 0183 0182 0164 0004 007d 0104  .|.......d...}..
-00003400: 007d 0204 007d 047d 0364 0053 0029 0a4e  .}...}.}.d.S.).N
-00003410: da08 7465 7374 5f71 7578 72aa 0000 0072  ..test_quxr....r
-00003420: 9500 0000 72ab 0000 0072 0a00 0000 7298  ....r....r....r.
-00003430: 0000 0072 9900 0000 729a 0000 00fa 0a74  ...r....r......t
-00003440: 6573 745f 7175 782e 3272 a700 0000 729c  est_qux.2r....r.
-00003450: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00003460: 0000 da13 7465 7374 5f6d 756c 7469 706c  ....test_multipl
-00003470: 655f 6361 6c6c 73c4 0000 0073 0400 0000  e_calls....s....
-00003480: 0001 9e01 7a26 4765 7452 6563 6f72 644e  ....z&GetRecordN
-00003490: 616d 6554 6573 7473 2e74 6573 745f 6d75  ameTests.test_mu
-000034a0: 6c74 6970 6c65 5f63 616c 6c73 6301 0000  ltiple_callsc...
-000034b0: 0000 0000 0000 0000 0008 0000 0008 0000  ................
-000034c0: 0043 0000 0073 d602 0000 6401 7d01 6402  .C...s....d.}.d.
-000034d0: 7d02 7400 7c01 7c02 6403 8d02 7d03 6401  }.t.|.|.d...}.d.
-000034e0: 7d04 7c03 7c04 6b02 7d05 7c05 739c 7401  }.|.|.k.}.|.s.t.
-000034f0: a002 6404 7c05 6601 6405 7c03 7c04 6602  ..d.|.f.d.|.|.f.
-00003500: a104 6406 7403 a004 a100 7600 734e 7401  ..d.t.....v.sNt.
-00003510: a005 7400 a101 7258 7401 a006 7400 a101  ..t...rXt...t...
-00003520: 6e02 6406 7401 a006 7c01 a101 7401 a006  n.d.t...|...t...
-00003530: 7c02 a101 7401 a006 7c03 a101 7401 a006  |...t...|...t...
-00003540: 7c04 a101 6407 9c05 1600 7d06 6408 6409  |...d.....}.d.d.
-00003550: 7c06 6901 1600 7d07 7407 7401 a008 7c07  |.i...}.t.t...|.
-00003560: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
-00003570: 0400 7d03 0400 7d05 7d04 6401 7d01 640a  ..}...}.}.d.}.d.
-00003580: 7d02 7400 7c01 7c02 6403 8d02 7d03 6401  }.t.|.|.d...}.d.
-00003590: 7d04 7c03 7c04 6b02 7d05 7c05 9001 7352  }.|.|.k.}.|...sR
-000035a0: 7401 a002 6404 7c05 6601 6405 7c03 7c04  t...d.|.f.d.|.|.
-000035b0: 6602 a104 6406 7403 a004 a100 7600 9001  f...d.t.....v...
-000035c0: 7304 7401 a005 7400 a101 9001 720e 7401  s.t...t.....r.t.
-000035d0: a006 7400 a101 6e02 6406 7401 a006 7c01  ..t...n.d.t...|.
-000035e0: a101 7401 a006 7c02 a101 7401 a006 7c03  ..t...|...t...|.
-000035f0: a101 7401 a006 7c04 a101 6407 9c05 1600  ..t...|...d.....
-00003600: 7d06 6408 6409 7c06 6901 1600 7d07 7407  }.d.d.|.i...}.t.
-00003610: 7401 a008 7c07 a101 8301 8201 6400 0400  t...|.......d...
-00003620: 7d01 0400 7d02 0400 7d03 0400 7d05 7d04  }...}...}...}.}.
-00003630: 6401 7d01 6402 7d02 7400 7c01 7c02 6403  d.}.d.}.t.|.|.d.
-00003640: 8d02 7d03 6401 7d04 7c03 7c04 6b02 7d05  ..}.d.}.|.|.k.}.
-00003650: 7c05 9002 7308 7401 a002 6404 7c05 6601  |...s.t...d.|.f.
-00003660: 6405 7c03 7c04 6602 a104 6406 7403 a004  d.|.|.f...d.t...
-00003670: a100 7600 9001 73ba 7401 a005 7400 a101  ..v...s.t...t...
-00003680: 9001 72c4 7401 a006 7400 a101 6e02 6406  ..r.t...t...n.d.
-00003690: 7401 a006 7c01 a101 7401 a006 7c02 a101  t...|...t...|...
-000036a0: 7401 a006 7c03 a101 7401 a006 7c04 a101  t...|...t...|...
-000036b0: 6407 9c05 1600 7d06 6408 6409 7c06 6901  d.....}.d.d.|.i.
-000036c0: 1600 7d07 7407 7401 a008 7c07 a101 8301  ..}.t.t...|.....
-000036d0: 8201 6400 0400 7d01 0400 7d02 0400 7d03  ..d...}...}...}.
-000036e0: 0400 7d05 7d04 6401 7d01 6402 7d02 7400  ..}.}.d.}.d.}.t.
-000036f0: 7c01 7c02 6403 8d02 7d03 640b 7d04 7c03  |.|.d...}.d.}.|.
-00003700: 7c04 6b02 7d05 7c05 9002 73be 7401 a002  |.k.}.|...s.t...
-00003710: 6404 7c05 6601 6405 7c03 7c04 6602 a104  d.|.f.d.|.|.f...
-00003720: 6406 7403 a004 a100 7600 9002 7370 7401  d.t.....v...spt.
-00003730: a005 7400 a101 9002 727a 7401 a006 7400  ..t.....rzt...t.
-00003740: a101 6e02 6406 7401 a006 7c01 a101 7401  ..n.d.t...|...t.
-00003750: a006 7c02 a101 7401 a006 7c03 a101 7401  ..|...t...|...t.
-00003760: a006 7c04 a101 6407 9c05 1600 7d06 6408  ..|...d.....}.d.
-00003770: 6409 7c06 6901 1600 7d07 7407 7401 a008  d.|.i...}.t.t...
-00003780: 7c07 a101 8301 8201 6400 0400 7d01 0400  |.......d...}...
-00003790: 7d02 0400 7d03 0400 7d05 7d04 6400 5300  }...}...}.}.d.S.
-000037a0: 290c 4e72 ad00 0000 7293 0000 0029 0272  ).Nr....r....).r
-000037b0: a300 0000 da09 6669 6c65 5f6e 616d 6572  ......file_namer
-000037c0: 9500 0000 2901 7a4d 2528 7079 3629 730a  ....).zM%(py6)s.
-000037d0: 7b25 2870 7936 2973 203d 2025 2870 7930  {%(py6)s = %(py0
-000037e0: 2973 2874 6573 745f 6e61 6d65 3d25 2870  )s(test_name=%(p
-000037f0: 7932 2973 2c20 6669 6c65 5f6e 616d 653d  y2)s, file_name=
-00003800: 2528 7079 3429 7329 0a7d 203d 3d20 2528  %(py4)s).} == %(
-00003810: 7079 3929 7372 0a00 0000 72a4 0000 0072  py9)sr....r....r
-00003820: a500 0000 72a6 0000 007a 0766 6f6f 322e  ....r....z.foo2.
-00003830: 7079 72ae 0000 0072 a700 0000 72a8 0000  pyr....r....r...
-00003840: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-00003850: da28 7465 7374 5f6d 756c 7469 706c 655f  .(test_multiple_
-00003860: 6361 6c6c 735f 6672 6f6d 5f64 6966 6665  calls_from_diffe
-00003870: 7265 6e74 5f66 696c 6573 c800 0000 7308  rent_files....s.
-00003880: 0000 0000 01b0 02b6 02b6 027a 3b47 6574  ...........z;Get
-00003890: 5265 636f 7264 4e61 6d65 5465 7374 732e  RecordNameTests.
-000038a0: 7465 7374 5f6d 756c 7469 706c 655f 6361  test_multiple_ca
-000038b0: 6c6c 735f 6672 6f6d 5f64 6966 6665 7265  lls_from_differe
-000038c0: 6e74 5f66 696c 6573 4e29 0772 8f00 0000  nt_filesN).r....
-000038d0: 7290 0000 0072 9100 0000 72a9 0000 0072  r....r....r....r
-000038e0: ac00 0000 72af 0000 0072 b100 0000 7216  ....r....r....r.
-000038f0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00003900: 0000 72a1 0000 00ba 0000 0073 0800 0000  ..r........s....
-00003910: 0801 0806 0803 0804 72a1 0000 0063 0000  ........r....c..
-00003920: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00003930: 0000 4000 0000 7324 0000 0065 005a 0164  ..@...s$...e.Z.d
-00003940: 005a 0264 0164 0284 005a 0364 0364 0484  .Z.d.d...Z.d.d..
-00003950: 005a 0464 0564 0684 005a 0564 0753 0029  .Z.d.d...Z.d.S.)
-00003960: 08da 1254 6573 7443 6173 654d 6978 696e  ...TestCaseMixin
-00003970: 5465 7374 7363 0100 0000 0000 0000 0000  Testsc..........
-00003980: 0000 0100 0000 0800 0000 4300 0000 733a  ..........C...s:
-00003990: 0000 007c 00a0 00a1 008f 1e01 0074 0164  ...|.........t.d
-000039a0: 0119 00a0 0264 02a1 0101 0057 0064 0004  .....d.....W.d..
-000039b0: 0004 0083 0301 006e 1031 0073 2c30 0001  .......n.1.s,0..
-000039c0: 0001 0001 0059 0001 0064 0053 0072 3300  .....Y...d.S.r3.
-000039d0: 0000 a903 da12 7265 636f 7264 5f70 6572  ......record_per
-000039e0: 666f 726d 616e 6365 7202 0000 0072 3500  formancer....r5.
-000039f0: 0000 7214 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00003a00: 0072 1700 0000 da17 7465 7374 5f72 6563  .r......test_rec
-00003a10: 6f72 645f 7065 7266 6f72 6d61 6e63 65d3  ord_performance.
-00003a20: 0000 0073 0400 0000 0001 0a01 7a2a 5465  ...s........z*Te
-00003a30: 7374 4361 7365 4d69 7869 6e54 6573 7473  stCaseMixinTests
-00003a40: 2e74 6573 745f 7265 636f 7264 5f70 6572  .test_record_per
-00003a50: 666f 726d 616e 6365 6301 0000 0000 0000  formancec.......
-00003a60: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
-00003a70: 0073 3e00 0000 7c00 6a00 6401 6402 8d01  .s>...|.j.d.d...
-00003a80: 8f1e 0100 7401 6403 1900 a002 6404 a101  ....t.d.....d...
-00003a90: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
-00003aa0: 3100 7330 3000 0100 0100 0100 5900 0100  1.s00.......Y...
-00003ab0: 6400 5300 2905 4eda 056f 7468 6572 723f  d.S.).N..otherr?
-00003ac0: 0000 0072 1100 0000 722d 0000 0072 b300  ...r....r-...r..
-00003ad0: 0000 7214 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00003ae0: 0072 1700 0000 da23 7465 7374 5f72 6563  .r.....#test_rec
-00003af0: 6f72 645f 7065 7266 6f72 6d61 6e63 655f  ord_performance_
-00003b00: 7265 636f 7264 5f6e 616d 65d7 0000 0073  record_name....s
-00003b10: 0400 0000 0001 0e01 7a36 5465 7374 4361  ........z6TestCa
-00003b20: 7365 4d69 7869 6e54 6573 7473 2e74 6573  seMixinTests.tes
-00003b30: 745f 7265 636f 7264 5f70 6572 666f 726d  t_record_perform
-00003b40: 616e 6365 5f72 6563 6f72 645f 6e61 6d65  ance_record_name
-00003b50: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00003b60: 0008 0000 0043 0000 0073 4a00 0000 7400  .....C...sJ...t.
-00003b70: a001 6401 6402 a102 7d01 7c00 6a02 7c01  ..d.d...}.|.j.|.
-00003b80: 6403 8d01 8f1e 0100 7403 6404 1900 a004  d.......t.d.....
-00003b90: 6405 a101 0100 5700 6400 0400 0400 8303  d.....W.d.......
-00003ba0: 0100 6e10 3100 733c 3000 0100 0100 0100  ..n.1.s<0.......
-00003bb0: 5900 0100 6400 5300 2906 4e7a 032e 7079  Y...d.S.).Nz..py
-00003bc0: 7a13 2e66 696c 655f 6e61 6d65 2e70 6572  z..file_name.per
-00003bd0: 662e 796d 6c72 6700 0000 7211 0000 0072  f.ymlrg...r....r
-00003be0: 2d00 0000 2905 da08 5f5f 6669 6c65 5f5f  -...)...__file__
-00003bf0: da07 7265 706c 6163 6572 b400 0000 7202  ..replacer....r.
-00003c00: 0000 0072 3500 0000 2902 7215 0000 005a  ...r5...).r....Z
-00003c10: 0970 6572 665f 6e61 6d65 7216 0000 0072  .perf_namer....r
-00003c20: 1600 0000 7217 0000 00da 2174 6573 745f  ....r.....!test_
-00003c30: 7265 636f 7264 5f70 6572 666f 726d 616e  record_performan
-00003c40: 6365 5f66 696c 655f 6e61 6d65 db00 0000  ce_file_name....
-00003c50: 7306 0000 0000 010c 010e 017a 3454 6573  s..........z4Tes
-00003c60: 7443 6173 654d 6978 696e 5465 7374 732e  tCaseMixinTests.
-00003c70: 7465 7374 5f72 6563 6f72 645f 7065 7266  test_record_perf
-00003c80: 6f72 6d61 6e63 655f 6669 6c65 5f6e 616d  ormance_file_nam
-00003c90: 654e 2906 728f 0000 0072 9000 0000 7291  eN).r....r....r.
-00003ca0: 0000 0072 b500 0000 72b7 0000 0072 ba00  ...r....r....r..
-00003cb0: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00003cc0: 0072 1700 0000 72b2 0000 00d2 0000 0073  .r....r........s
-00003cd0: 0600 0000 0801 0804 0804 72b2 0000 0029  ..........r....)
-00003ce0: 25da 0862 7569 6c74 696e 7372 5600 0000  %..builtinsrV...
-00003cf0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00003d00: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00003d10: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00003d20: 5300 0000 7269 0000 0072 4f00 0000 da11  S...ri...rO.....
-00003d30: 646a 616e 676f 2e63 6f72 652e 6361 6368  django.core.cach
-00003d40: 6572 0200 0000 da10 646a 616e 676f 2e64  er......django.d
-00003d50: 622e 6d6f 6465 6c73 7203 0000 00da 1a64  b.modelsr......d
-00003d60: 6a61 6e67 6f2e 6462 2e6d 6f64 656c 732e  jango.db.models.
-00003d70: 6675 6e63 7469 6f6e 7372 0400 0000 da0b  functionsr......
-00003d80: 646a 616e 676f 2e74 6573 7472 0500 0000  django.testr....
-00003d90: 7206 0000 0072 0700 0000 5a0f 646a 616e  r....r....Z.djan
-00003da0: 676f 5f70 6572 665f 7265 6372 0800 0000  go_perf_recr....
-00003db0: 7209 0000 0072 0a00 0000 720b 0000 005a  r....r....r....Z
-00003dc0: 1474 6573 7473 2e74 6573 7461 7070 2e6d  .tests.testapp.m
-00003dd0: 6f64 656c 7372 0c00 0000 5a0b 7465 7374  odelsr....Z.test
-00003de0: 732e 7574 696c 7372 0d00 0000 720e 0000  s.utilsr....r...
-00003df0: 0072 0f00 0000 7268 0000 00da 0764 6972  .r....rh.....dir
-00003e00: 6e61 6d65 72b8 0000 0072 7a00 0000 7210  namer....rz...r.
-00003e10: 0000 0072 9200 0000 72a1 0000 0072 b200  ...r....r....r..
-00003e20: 0000 7216 0000 0072 1600 0000 7216 0000  ..r....r....r...
-00003e30: 0072 1700 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00003e40: 0100 0000 731c 0000 0022 0208 010c 010c  ....s...."......
-00003e50: 010c 0114 0218 010c 0114 020c 0310 7f00  ................
-00003e60: 2010 0b10 18                              ....
+00000290: 005a 1364 2464 2584 005a 1464 2664 2784  .Z.d$d%..Z.d&d'.
+000002a0: 005a 1564 2864 2984 005a 1665 0664 2a64  .Z.d(d)..Z.e.d*d
+000002b0: 2b69 0164 098d 0164 2c64 2d84 0083 015a  +i.d...d,d-....Z
+000002c0: 1765 0664 2a64 2e69 0164 098d 0164 2f64  .e.d*d.i.d...d/d
+000002d0: 3084 0083 015a 1865 0664 2a64 3169 0164  0....Z.e.d*d1i.d
+000002e0: 098d 0164 3264 3384 0083 015a 1964 3464  ...d2d3....Z.d4d
+000002f0: 3584 005a 1a64 3653 0029 37da 0b52 6563  5..Z.d6S.)7..Rec
+00000300: 6f72 6454 6573 7473 6301 0000 0000 0000  ordTestsc.......
+00000310: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
+00000320: 0073 3400 0000 7400 8300 8f1a 0100 7401  .s4...t.......t.
+00000330: 6401 6402 8302 0100 5700 6400 0400 0400  d.d.....W.d.....
+00000340: 8303 0100 6e10 3100 7326 3000 0100 0100  ....n.1.s&0.....
+00000350: 0100 5900 0100 6400 5300 2903 4eda 0764  ..Y...d.S.).N..d
+00000360: 6566 6175 6c74 fa0b 5345 4c45 4354 2031  efault..SELECT 1
+00000370: 3333 37a9 0272 0b00 0000 720e 0000 00a9  337..r....r.....
+00000380: 01da 0473 656c 66a9 0072 1600 0000 fa42  ...self..r.....B
+00000390: 2f55 7365 7273 2f63 6861 696e 7a2f 446f  /Users/chainz/Do
+000003a0: 6375 6d65 6e74 732f 5072 6f6a 6563 7473  cuments/Projects
+000003b0: 2f64 6a61 6e67 6f2d 7065 7266 2d72 6563  /django-perf-rec
+000003c0: 2f74 6573 7473 2f74 6573 745f 6170 692e  /tests/test_api.
+000003d0: 7079 da14 7465 7374 5f73 696e 676c 655f  py..test_single_
+000003e0: 6462 5f71 7565 7279 1100 0000 7304 0000  db_query....s...
+000003f0: 0000 0108 01fa 2052 6563 6f72 6454 6573  ...... RecordTes
+00000400: 7473 2e74 6573 745f 7369 6e67 6c65 5f64  ts.test_single_d
+00000410: 625f 7175 6572 7963 0100 0000 0000 0000  b_queryc........
+00000420: 0000 0000 0800 0000 0a00 0000 4300 0000  ............C...
+00000430: 7314 0200 0074 0083 0090 018f f601 0074  s....t.........t
+00000440: 01a0 0274 03a1 018f 4e7d 0164 0164 0284  ...t....N}.d.d..
+00000450: 007d 0274 0464 037c 0264 048d 028f 1a01  .}.t.d.|.d......
+00000460: 0074 0564 0564 0683 0201 0057 0064 0004  .t.d.d.....W.d..
+00000470: 0004 0083 0301 006e 1031 0073 4a30 0001  .......n.1.sJ0..
+00000480: 0001 0001 0059 0001 0057 0064 0004 0004  .....Y...W.d....
+00000490: 0083 0301 006e 1031 0073 6830 0001 0001  .....n.1.sh0....
+000004a0: 0001 0059 0001 0074 067c 016a 0783 017d  ...Y...t.|.j...}
+000004b0: 0364 077d 047c 047c 0376 007d 057c 0573  .d.}.|.|.v.}.|.s
+000004c0: ec74 08a0 0964 087c 0566 0164 097c 047c  .t...d.|.f.d.|.|
+000004d0: 0366 02a1 0474 08a0 0a7c 04a1 0164 0a74  .f...t...|...d.t
+000004e0: 0ba0 0ca1 0076 0073 be74 08a0 0d7c 03a1  .....v.s.t...|..
+000004f0: 0172 c874 08a0 0a7c 03a1 016e 0264 0a64  .r.t...|...n.d.d
+00000500: 0b9c 0216 007d 0664 0c64 0d7c 0669 0116  .....}.d.d.|.i..
+00000510: 007d 0774 0374 08a0 0e7c 07a1 0183 0182  .}.t.t...|......
+00000520: 0164 0004 007d 047d 0564 0e7d 047c 047c  .d...}.}.d.}.|.|
+00000530: 0376 007d 057c 0590 0173 6a74 08a0 0964  .v.}.|...sjt...d
+00000540: 087c 0566 0164 097c 047c 0366 02a1 0474  .|.f.d.|.|.f...t
+00000550: 08a0 0a7c 04a1 0164 0a74 0ba0 0ca1 0076  ...|...d.t.....v
+00000560: 0090 0173 3c74 08a0 0d7c 03a1 0190 0172  ...s<t...|.....r
+00000570: 4674 08a0 0a7c 03a1 016e 0264 0a64 0b9c  Ft...|...n.d.d..
+00000580: 0216 007d 0664 0c64 0d7c 0669 0116 007d  ...}.d.d.|.i...}
+00000590: 0774 0374 08a0 0e7c 07a1 0183 0182 0164  .t.t...|.......d
+000005a0: 0004 007d 047d 0564 0f7d 047c 047c 0376  ...}.}.d.}.|.|.v
+000005b0: 007d 057c 0590 0173 e874 08a0 0964 087c  .}.|...s.t...d.|
+000005c0: 0566 0164 097c 047c 0366 02a1 0474 08a0  .f.d.|.|.f...t..
+000005d0: 0a7c 04a1 0164 0a74 0ba0 0ca1 0076 0090  .|...d.t.....v..
+000005e0: 0173 ba74 08a0 0d7c 03a1 0190 0172 c474  .s.t...|.....r.t
+000005f0: 08a0 0a7c 03a1 016e 0264 0a64 0b9c 0216  ...|...n.d.d....
+00000600: 007d 0664 0c64 0d7c 0669 0116 007d 0774  .}.d.d.|.i...}.t
+00000610: 0374 08a0 0e7c 07a1 0183 0182 0164 0004  .t...|.......d..
+00000620: 007d 047d 0557 0064 0004 0004 0083 0301  .}.}.W.d........
+00000630: 006e 1231 0090 0273 0630 0001 0001 0001  .n.1...s.0......
+00000640: 0059 0001 0064 0053 0029 104e 6301 0000  .Y...d.S.).Nc...
+00000650: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000660: 0053 0000 0073 0400 0000 6401 5300 a902  .S...s....d.S...
+00000670: 4e54 7216 0000 00a9 01da 096f 7065 7261  NTr........opera
+00000680: 7469 6f6e 7216 0000 0072 1600 0000 7217  tionr....r....r.
+00000690: 0000 00da 1163 6170 7475 7265 5f74 7261  .....capture_tra
+000006a0: 6365 6261 636b 1900 0000 7302 0000 0000  ceback....s.....
+000006b0: 017a 4a52 6563 6f72 6454 6573 7473 2e74  .zJRecordTests.t
+000006c0: 6573 745f 7369 6e67 6c65 5f64 625f 7175  est_single_db_qu
+000006d0: 6572 795f 7769 7468 5f74 7261 6365 6261  ery_with_traceba
+000006e0: 636b 2e3c 6c6f 6361 6c73 3e2e 6361 7074  ck.<locals>.capt
+000006f0: 7572 655f 7472 6163 6562 6163 6b72 1900  ure_tracebackr..
+00000700: 0000 a902 da0b 7265 636f 7264 5f6e 616d  ......record_nam
+00000710: 6572 1d00 0000 7211 0000 0072 1200 0000  er....r....r....
+00000720: 7a45 5065 7266 6f72 6d61 6e63 6520 7265  zEPerformance re
+00000730: 636f 7264 2064 6964 206e 6f74 206d 6174  cord did not mat
+00000740: 6368 2066 6f72 2052 6563 6f72 6454 6573  ch for RecordTes
+00000750: 7473 2e74 6573 745f 7369 6e67 6c65 5f64  ts.test_single_d
+00000760: 625f 7175 6572 79a9 01da 0269 6ea9 017a  b_query....in..z
+00000770: 1225 2870 7931 2973 2069 6e20 2528 7079  .%(py1)s in %(py
+00000780: 3329 73da 036d 7367 a902 da03 7079 31da  3)s..msg....py1.
+00000790: 0370 7933 fa0e 6173 7365 7274 2025 2870  .py3..assert %(p
+000007a0: 7935 2973 da03 7079 35fa 0c2b 2074 7261  y5)s..py5..+ tra
+000007b0: 6365 6261 636b 3a7a 2669 6e20 7465 7374  ceback:z&in test
+000007c0: 5f73 696e 676c 655f 6462 5f71 7565 7279  _single_db_query
+000007d0: 5f77 6974 685f 7472 6163 6562 6163 6b29  _with_traceback)
+000007e0: 0f72 0d00 0000 da06 7079 7465 7374 da06  .r......pytest..
+000007f0: 7261 6973 6573 da0e 4173 7365 7274 696f  raises..Assertio
+00000800: 6e45 7272 6f72 720b 0000 0072 0e00 0000  nErrorr....r....
+00000810: da03 7374 72da 0576 616c 7565 da0a 4070  ..str..value..@p
+00000820: 7974 6573 745f 6172 da11 5f63 616c 6c5f  ytest_ar.._call_
+00000830: 7265 7072 636f 6d70 6172 65da 095f 7361  reprcompare.._sa
+00000840: 6665 7265 7072 da0c 4070 795f 6275 696c  ferepr..@py_buil
+00000850: 7469 6e73 da06 6c6f 6361 6c73 da18 5f73  tins..locals.._s
+00000860: 686f 756c 645f 7265 7072 5f67 6c6f 6261  hould_repr_globa
+00000870: 6c5f 6e61 6d65 da13 5f66 6f72 6d61 745f  l_name.._format_
+00000880: 6578 706c 616e 6174 696f 6ea9 0872 1500  explanation..r..
+00000890: 0000 da07 6578 6369 6e66 6f72 1d00 0000  ....excinfor....
+000008a0: 7223 0000 00da 0b40 7079 5f61 7373 6572  r#.....@py_asser
+000008b0: 7430 da0b 4070 795f 6173 7365 7274 32da  t0..@py_assert2.
+000008c0: 0b40 7079 5f66 6f72 6d61 7434 da0b 4070  .@py_format4..@p
+000008d0: 795f 666f 726d 6174 3672 1600 0000 7216  y_format6r....r.
+000008e0: 0000 0072 1700 0000 da23 7465 7374 5f73  ...r.....#test_s
+000008f0: 696e 676c 655f 6462 5f71 7565 7279 5f77  ingle_db_query_w
+00000900: 6974 685f 7472 6163 6562 6163 6b15 0000  ith_traceback...
+00000910: 0073 1800 0000 0001 0a01 0c02 0803 0201  .s..............
+00000920: 0201 02fe 0804 4602 0a01 7804 7e01 7a2f  ......F...x.~.z/
+00000930: 5265 636f 7264 5465 7374 732e 7465 7374  RecordTests.test
+00000940: 5f73 696e 676c 655f 6462 5f71 7565 7279  _single_db_query
+00000950: 5f77 6974 685f 7472 6163 6562 6163 6b63  _with_tracebackc
+00000960: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000970: 0800 0000 4300 0000 7338 0000 0074 0083  ....C...s8...t..
+00000980: 008f 1e01 0074 0174 026a 03a0 04a1 0083  .....t.t.j......
+00000990: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+000009a0: 1031 0073 2a30 0001 0001 0001 0059 0001  .1.s*0.......Y..
+000009b0: 0064 0053 00a9 014e a905 720b 0000 00da  .d.S...N..r.....
+000009c0: 046c 6973 7472 0c00 0000 da07 6f62 6a65  .listr......obje
+000009d0: 6374 73da 0361 6c6c 7214 0000 0072 1600  cts..allr....r..
+000009e0: 0000 7216 0000 0072 1700 0000 da1a 7465  ..r....r......te
+000009f0: 7374 5f73 696e 676c 655f 6462 5f71 7565  st_single_db_que
+00000a00: 7279 5f6d 6f64 656c 2a00 0000 7304 0000  ry_model*...s...
+00000a10: 0000 0108 017a 2652 6563 6f72 6454 6573  .....z&RecordTes
+00000a20: 7473 2e74 6573 745f 7369 6e67 6c65 5f64  ts.test_single_d
+00000a30: 625f 7175 6572 795f 6d6f 6465 6cda 0c48  b_query_model..H
+00000a40: 4944 455f 434f 4c55 4d4e 5346 2901 da08  IDE_COLUMNSF)...
+00000a50: 5045 5246 5f52 4543 6301 0000 0000 0000  PERF_RECc.......
+00000a60: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
+00000a70: 0073 3800 0000 7400 8300 8f1e 0100 7401  .s8...t.......t.
+00000a80: 7402 6a03 a004 a100 8301 0100 5700 6400  t.j.........W.d.
+00000a90: 0400 0400 8303 0100 6e10 3100 732a 3000  ........n.1.s*0.
+00000aa0: 0100 0100 0100 5900 0100 6400 5300 723d  ......Y...d.S.r=
+00000ab0: 0000 0072 3e00 0000 7214 0000 0072 1600  ...r>...r....r..
+00000ac0: 0000 7216 0000 0072 1700 0000 da27 7465  ..r....r.....'te
+00000ad0: 7374 5f73 696e 676c 655f 6462 5f71 7565  st_single_db_que
+00000ae0: 7279 5f6d 6f64 656c 5f77 6974 685f 636f  ry_model_with_co
+00000af0: 6c75 6d6e 732e 0000 0073 0400 0000 0002  lumns....s......
+00000b00: 0801 7a33 5265 636f 7264 5465 7374 732e  ..z3RecordTests.
+00000b10: 7465 7374 5f73 696e 676c 655f 6462 5f71  test_single_db_q
+00000b20: 7565 7279 5f6d 6f64 656c 5f77 6974 685f  uery_model_with_
+00000b30: 636f 6c75 6d6e 7363 0100 0000 0000 0000  columnsc........
+00000b40: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
+00000b50: 733e 0000 0074 0083 008f 2401 0074 0164  s>...t....$..t.d
+00000b60: 0164 0283 0201 0074 0164 0164 0383 0201  .d.....t.d.d....
+00000b70: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00000b80: 0073 3030 0001 0001 0001 0059 0001 0064  .s00.......Y...d
+00000b90: 0053 0029 044e 7211 0000 0072 1200 0000  .S.).Nr....r....
+00000ba0: 7a0b 5345 4c45 4354 2034 3934 3972 1300  z.SELECT 4949r..
+00000bb0: 0000 7214 0000 0072 1600 0000 7216 0000  ..r....r....r...
+00000bc0: 0072 1700 0000 da18 7465 7374 5f6d 756c  .r......test_mul
+00000bd0: 7469 706c 655f 6462 5f71 7565 7269 6573  tiple_db_queries
+00000be0: 3300 0000 7306 0000 0000 0108 010a 017a  3...s..........z
+00000bf0: 2452 6563 6f72 6454 6573 7473 2e74 6573  $RecordTests.tes
+00000c00: 745f 6d75 6c74 6970 6c65 5f64 625f 7175  t_multiple_db_qu
+00000c10: 6572 6965 7363 0100 0000 0000 0000 0000  eriesc..........
+00000c20: 0000 0100 0000 0800 0000 4300 0000 7346  ..........C...sF
+00000c30: 0000 0074 0083 008f 2c01 0074 0174 026a  ...t....,..t.t.j
+00000c40: 036a 0474 0564 0183 0174 0564 0183 0164  .j.t.d...t.d...d
+00000c50: 028d 0283 0101 0057 0064 0004 0004 0083  .......W.d......
+00000c60: 0301 006e 1031 0073 3830 0001 0001 0001  ...n.1.s80......
+00000c70: 0059 0001 0064 0053 0029 034e da04 6e61  .Y...d.S.).N..na
+00000c80: 6d65 a902 da01 78da 0179 2906 720b 0000  me....x..y).r...
+00000c90: 0072 3f00 0000 720c 0000 0072 4000 0000  .r?...r....r@...
+00000ca0: da08 616e 6e6f 7461 7465 7204 0000 0072  ..annotater....r
+00000cb0: 1400 0000 7216 0000 0072 1600 0000 7217  ....r....r....r.
+00000cc0: 0000 00da 2874 6573 745f 6e6f 6e5f 6465  ....(test_non_de
+00000cd0: 7465 726d 696e 6973 7469 635f 5175 6572  terministic_Quer
+00000ce0: 7953 6574 5f61 6e6e 6f74 6174 6538 0000  ySet_annotate8..
+00000cf0: 0073 0400 0000 0001 0801 7a34 5265 636f  .s........z4Reco
+00000d00: 7264 5465 7374 732e 7465 7374 5f6e 6f6e  rdTests.test_non
+00000d10: 5f64 6574 6572 6d69 6e69 7374 6963 5f51  _deterministic_Q
+00000d20: 7565 7279 5365 745f 616e 6e6f 7461 7465  uerySet_annotate
+00000d30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000d40: 0008 0000 0043 0000 0073 4200 0000 7400  .....C...sB...t.
+00000d50: 8300 8f28 0100 7401 7402 6a03 6a04 6401  ...(..t.t.j.j.d.
+00000d60: 6401 6402 9c02 6403 8d01 8301 0100 5700  d.d...d.......W.
+00000d70: 6400 0400 0400 8303 0100 6e10 3100 7334  d.........n.1.s4
+00000d80: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00000d90: 2904 4eda 0131 7248 0000 0029 01da 0673  ).N..1rH...)...s
+00000da0: 656c 6563 7429 0572 0b00 0000 723f 0000  elect).r....r?..
+00000db0: 0072 0c00 0000 7240 0000 00da 0565 7874  .r....r@.....ext
+00000dc0: 7261 7214 0000 0072 1600 0000 7216 0000  rar....r....r...
+00000dd0: 0072 1700 0000 da25 7465 7374 5f6e 6f6e  .r.....%test_non
+00000de0: 5f64 6574 6572 6d69 6e69 7374 6963 5f51  _deterministic_Q
+00000df0: 7565 7279 5365 745f 6578 7472 613c 0000  uerySet_extra<..
+00000e00: 0073 0400 0000 0001 0801 7a31 5265 636f  .s........z1Reco
+00000e10: 7264 5465 7374 732e 7465 7374 5f6e 6f6e  rdTests.test_non
+00000e20: 5f64 6574 6572 6d69 6e69 7374 6963 5f51  _deterministic_Q
+00000e30: 7565 7279 5365 745f 6578 7472 6163 0100  uerySet_extrac..
+00000e40: 0000 0000 0000 0000 0000 0100 0000 0800  ................
+00000e50: 0000 4300 0000 7342 0000 0074 0083 008f  ..C...sB...t....
+00000e60: 2801 0074 0174 026a 03a0 0474 0564 0164  (..t.t.j...t.d.d
+00000e70: 0264 038d 02a1 0183 0101 0057 0064 0004  .d.........W.d..
+00000e80: 0004 0083 0301 006e 1031 0073 3430 0001  .......n.1.s40..
+00000e90: 0001 0001 0059 0001 0064 0053 0029 044e  .....Y...d.S.).N
+00000ea0: da03 666f 6fe9 0100 0000 a902 7247 0000  ..foo.......rG..
+00000eb0: 00da 0361 6765 2906 720b 0000 0072 3f00  ...age).r....r?.
+00000ec0: 0000 720c 0000 0072 4000 0000 da06 6669  ..r....r@.....fi
+00000ed0: 6c74 6572 7203 0000 0072 1400 0000 7216  lterr....r....r.
+00000ee0: 0000 0072 1600 0000 7217 0000 00da 1e74  ...r....r......t
+00000ef0: 6573 745f 6e6f 6e5f 6465 7465 726d 696e  est_non_determin
+00000f00: 6973 7469 635f 515f 7175 6572 7940 0000  istic_Q_query@..
+00000f10: 0073 0400 0000 0001 0801 7a2a 5265 636f  .s........z*Reco
+00000f20: 7264 5465 7374 732e 7465 7374 5f6e 6f6e  rdTests.test_non
+00000f30: 5f64 6574 6572 6d69 6e69 7374 6963 5f51  _deterministic_Q
+00000f40: 5f71 7565 7279 6301 0000 0000 0000 0000  _queryc.........
+00000f50: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
+00000f60: 3800 0000 7400 8300 8f1e 0100 7401 6401  8...t.......t.d.
+00000f70: 1900 a002 6402 a101 0100 5700 6400 0400  ....d.....W.d...
+00000f80: 0400 8303 0100 6e10 3100 732a 3000 0100  ......n.1.s*0...
+00000f90: 0100 0100 5900 0100 6400 5300 a903 4e72  ....Y...d.S...Nr
+00000fa0: 1100 0000 7251 0000 00a9 0372 0b00 0000  ....rQ.....r....
+00000fb0: 7202 0000 00da 0367 6574 7214 0000 0072  r......getr....r
+00000fc0: 1600 0000 7216 0000 0072 1700 0000 da14  ....r....r......
+00000fd0: 7465 7374 5f73 696e 676c 655f 6361 6368  test_single_cach
+00000fe0: 655f 6f70 4400 0000 7304 0000 0000 0108  e_opD...s.......
+00000ff0: 01fa 2052 6563 6f72 6454 6573 7473 2e74  .. RecordTests.t
+00001000: 6573 745f 7369 6e67 6c65 5f63 6163 6865  est_single_cache
+00001010: 5f6f 7063 0100 0000 0000 0000 0000 0000  _opc............
+00001020: 0800 0000 0a00 0000 4300 0000 739a 0100  ........C...s...
+00001030: 0074 0083 0090 018f 7c01 0074 01a0 0274  .t......|..t...t
+00001040: 03a1 018f 527d 0164 0164 0284 007d 0274  ....R}.d.d...}.t
+00001050: 0464 037c 0264 048d 028f 1e01 0074 0564  .d.|.d.......t.d
+00001060: 0519 00a0 0664 06a1 0101 0057 0064 0004  .....d.....W.d..
+00001070: 0004 0083 0301 006e 1031 0073 4e30 0001  .......n.1.sN0..
+00001080: 0001 0001 0059 0001 0057 0064 0004 0004  .....Y...W.d....
+00001090: 0083 0301 006e 1031 0073 6c30 0001 0001  .....n.1.sl0....
+000010a0: 0001 0059 0001 0074 077c 016a 0883 017d  ...Y...t.|.j...}
+000010b0: 0364 077d 047c 047c 0376 007d 057c 0573  .d.}.|.|.v.}.|.s
+000010c0: f074 09a0 0a64 087c 0566 0164 097c 047c  .t...d.|.f.d.|.|
+000010d0: 0366 02a1 0474 09a0 0b7c 04a1 0164 0a74  .f...t...|...d.t
+000010e0: 0ca0 0da1 0076 0073 c274 09a0 0e7c 03a1  .....v.s.t...|..
+000010f0: 0172 cc74 09a0 0b7c 03a1 016e 0264 0a64  .r.t...|...n.d.d
+00001100: 0b9c 0216 007d 0664 0c64 0d7c 0669 0116  .....}.d.d.|.i..
+00001110: 007d 0774 0374 09a0 0f7c 07a1 0183 0182  .}.t.t...|......
+00001120: 0164 0004 007d 047d 0564 0e7d 047c 047c  .d...}.}.d.}.|.|
+00001130: 0376 007d 057c 0590 0173 6e74 09a0 0a64  .v.}.|...snt...d
+00001140: 087c 0566 0164 097c 047c 0366 02a1 0474  .|.f.d.|.|.f...t
+00001150: 09a0 0b7c 04a1 0164 0a74 0ca0 0da1 0076  ...|...d.t.....v
+00001160: 0090 0173 4074 09a0 0e7c 03a1 0190 0172  ...s@t...|.....r
+00001170: 4a74 09a0 0b7c 03a1 016e 0264 0a64 0b9c  Jt...|...n.d.d..
+00001180: 0216 007d 0664 0c64 0d7c 0669 0116 007d  ...}.d.d.|.i...}
+00001190: 0774 0374 09a0 0f7c 07a1 0183 0182 0164  .t.t...|.......d
+000011a0: 0004 007d 047d 0557 0064 0004 0004 0083  ...}.}.W.d......
+000011b0: 0301 006e 1231 0090 0173 8c30 0001 0001  ...n.1...s.0....
+000011c0: 0001 0059 0001 0064 0053 0029 0f4e 6301  ...Y...d.S.).Nc.
+000011d0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+000011e0: 0000 0053 0000 0073 0400 0000 6401 5300  ...S...s....d.S.
+000011f0: 721a 0000 0072 1600 0000 721b 0000 0072  r....r....r....r
+00001200: 1600 0000 7216 0000 0072 1700 0000 721d  ....r....r....r.
+00001210: 0000 004c 0000 0073 0200 0000 0001 7a4a  ...L...s......zJ
+00001220: 5265 636f 7264 5465 7374 732e 7465 7374  RecordTests.test
+00001230: 5f73 696e 676c 655f 6361 6368 655f 6f70  _single_cache_op
+00001240: 5f77 6974 685f 7472 6163 6562 6163 6b2e  _with_traceback.
+00001250: 3c6c 6f63 616c 733e 2e63 6170 7475 7265  <locals>.capture
+00001260: 5f74 7261 6365 6261 636b 725b 0000 0072  _tracebackr[...r
+00001270: 1e00 0000 7211 0000 0072 5100 0000 7229  ....r....rQ...r)
+00001280: 0000 0072 2000 0000 7222 0000 0072 2300  ...r ...r"...r#.
+00001290: 0000 7224 0000 0072 2700 0000 7228 0000  ..r$...r'...r(..
+000012a0: 007a 2669 6e20 7465 7374 5f73 696e 676c  .z&in test_singl
+000012b0: 655f 6361 6368 655f 6f70 5f77 6974 685f  e_cache_op_with_
+000012c0: 7472 6163 6562 6163 6b29 1072 0d00 0000  traceback).r....
+000012d0: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+000012e0: 0b00 0000 7202 0000 0072 5900 0000 722d  ....r....rY...r-
+000012f0: 0000 0072 2e00 0000 722f 0000 0072 3000  ...r....r/...r0.
+00001300: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
+00001310: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
+00001320: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
+00001330: 2374 6573 745f 7369 6e67 6c65 5f63 6163  #test_single_cac
+00001340: 6865 5f6f 705f 7769 7468 5f74 7261 6365  he_op_with_trace
+00001350: 6261 636b 4800 0000 7316 0000 0000 010a  backH...s.......
+00001360: 010c 0208 0302 0102 0102 fe08 044a 020a  .............J..
+00001370: 0178 017a 2f52 6563 6f72 6454 6573 7473  .x.z/RecordTests
+00001380: 2e74 6573 745f 7369 6e67 6c65 5f63 6163  .test_single_cac
+00001390: 6865 5f6f 705f 7769 7468 5f74 7261 6365  he_op_with_trace
+000013a0: 6261 636b 6301 0000 0000 0000 0000 0000  backc...........
+000013b0: 0001 0000 0008 0000 0043 0000 0073 5a00  .........C...sZ.
+000013c0: 0000 7400 8300 8f40 0100 7401 6401 1900  ..t....@..t.d...
+000013d0: a002 6402 6403 a102 0100 7401 6404 1900  ..d.d.....t.d...
+000013e0: a003 6402 6403 6702 a101 0100 7401 6401  ..d.d.g.....t.d.
+000013f0: 1900 a004 6402 a101 0100 5700 6400 0400  ....d.....W.d...
+00001400: 0400 8303 0100 6e10 3100 734c 3000 0100  ......n.1.sL0...
+00001410: 0100 0100 5900 0100 6400 5300 2905 4e72  ....Y...d.S.).Nr
+00001420: 1100 0000 7251 0000 00da 0362 6172 da06  ....rQ.....bar..
+00001430: 7365 636f 6e64 2905 720b 0000 0072 0200  second).r....r..
+00001440: 0000 da03 7365 74da 0867 6574 5f6d 616e  ....set..get_man
+00001450: 79da 0664 656c 6574 6572 1400 0000 7216  y..deleter....r.
+00001460: 0000 0072 1600 0000 7217 0000 00da 1774  ...r....r......t
+00001470: 6573 745f 6d75 6c74 6970 6c65 5f63 6163  est_multiple_cac
+00001480: 6865 5f6f 7073 5900 0000 7308 0000 0000  he_opsY...s.....
+00001490: 0108 0110 0112 017a 2352 6563 6f72 6454  .......z#RecordT
+000014a0: 6573 7473 2e74 6573 745f 6d75 6c74 6970  ests.test_multip
+000014b0: 6c65 5f63 6163 6865 5f6f 7073 6301 0000  le_cache_opsc...
+000014c0: 0000 0000 0000 0000 0001 0000 0008 0000  ................
+000014d0: 0043 0000 0073 6c00 0000 7400 8300 8f1e  .C...sl...t.....
+000014e0: 0100 7401 6401 1900 a002 6402 a101 0100  ..t.d.....d.....
+000014f0: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
+00001500: 732a 3000 0100 0100 0100 5900 0100 7400  s*0.......Y...t.
+00001510: 8300 8f1e 0100 7401 6401 1900 a002 6403  ......t.d.....d.
+00001520: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00001530: 6e10 3100 735e 3000 0100 0100 0100 5900  n.1.s^0.......Y.
+00001540: 0100 6400 5300 2904 4e72 1100 0000 7251  ..d.S.).Nr....rQ
+00001550: 0000 0072 5d00 0000 7258 0000 0072 1400  ...r]...rX...r..
+00001560: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001570: 00da 3a74 6573 745f 6d75 6c74 6970 6c65  ..:test_multiple
+00001580: 5f63 616c 6c73 5f69 6e5f 7361 6d65 5f66  _calls_in_same_f
+00001590: 756e 6374 696f 6e5f 6172 655f 6469 6666  unction_are_diff
+000015a0: 6572 656e 745f 7265 636f 7264 735f 0000  erent_records_..
+000015b0: 0073 0800 0000 0001 0801 2c02 0801 7a46  .s........,...zF
+000015c0: 5265 636f 7264 5465 7374 732e 7465 7374  RecordTests.test
+000015d0: 5f6d 756c 7469 706c 655f 6361 6c6c 735f  _multiple_calls_
+000015e0: 696e 5f73 616d 655f 6675 6e63 7469 6f6e  in_same_function
+000015f0: 5f61 7265 5f64 6966 6665 7265 6e74 5f72  _are_different_r
+00001600: 6563 6f72 6473 6301 0000 0000 0000 0000  ecordsc.........
+00001610: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
+00001620: 3c00 0000 7400 6401 6402 8d01 8f1e 0100  <...t.d.d.......
+00001630: 7401 6403 1900 a002 6404 a101 0100 5700  t.d.....d.....W.
+00001640: 6400 0400 0400 8303 0100 6e10 3100 732e  d.........n.1.s.
+00001650: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00001660: 2905 4eda 0663 7573 746f 6da9 0172 1f00  ).N..custom..r..
+00001670: 0000 7211 0000 0072 5100 0000 7258 0000  ..r....rQ...rX..
+00001680: 0072 1400 0000 7216 0000 0072 1600 0000  .r....r....r....
+00001690: 7217 0000 00da 1074 6573 745f 6375 7374  r......test_cust
+000016a0: 6f6d 5f6e 616d 6566 0000 0073 0400 0000  om_namef...s....
+000016b0: 0001 0c01 7a1c 5265 636f 7264 5465 7374  ....z.RecordTest
+000016c0: 732e 7465 7374 5f63 7573 746f 6d5f 6e61  s.test_custom_na
+000016d0: 6d65 6301 0000 0000 0000 0000 0000 0008  mec.............
+000016e0: 0000 0009 0000 0043 0000 0073 6401 0000  .......C...sd...
+000016f0: 7400 6401 6402 8d01 8f1e 0100 7401 6403  t.d.d.......t.d.
+00001700: 1900 a002 6404 a101 0100 5700 6400 0400  ....d.....W.d...
+00001710: 0400 8303 0100 6e10 3100 732e 3000 0100  ......n.1.s.0...
+00001720: 0100 0100 5900 0100 7403 a004 7405 a101  ....Y...t...t...
+00001730: 8f48 7d01 7400 6401 6402 8d01 8f1e 0100  .H}.t.d.d.......
+00001740: 7401 6403 1900 a002 6405 a101 0100 5700  t.d.....d.....W.
+00001750: 6400 0400 0400 8303 0100 6e10 3100 7372  d.........n.1.sr
+00001760: 3000 0100 0100 0100 5900 0100 5700 6400  0.......Y...W.d.
+00001770: 0400 0400 8303 0100 6e10 3100 7390 3000  ........n.1.s.0.
+00001780: 0100 0100 0100 5900 0100 6406 7d02 7c01  ......Y...d.}.|.
+00001790: 6a06 7d03 7407 7c03 8301 7d04 7c02 7c04  j.}.t.|...}.|.|.
+000017a0: 7600 7d05 7c05 9001 7350 7408 a009 6407  v.}.|...sPt...d.
+000017b0: 7c05 6601 6408 7c02 7c04 6602 a104 7408  |.f.d.|.|.f...t.
+000017c0: a00a 7c02 a101 6409 740b a00c a100 7600  ..|...d.t.....v.
+000017d0: 73ec 7408 a00d 7407 a101 72f6 7408 a00a  s.t...t...r.t...
+000017e0: 7407 a101 6e02 6409 640a 740b a00c a100  t...n.d.d.t.....
+000017f0: 7600 9001 7312 7408 a00d 7c01 a101 9001  v...s.t...|.....
+00001800: 721c 7408 a00a 7c01 a101 6e02 640a 7408  r.t...|...n.d.t.
+00001810: a00a 7c03 a101 7408 a00a 7c04 a101 640b  ..|...t...|...d.
+00001820: 9c05 1600 7d06 640c 640d 7c06 6901 1600  ....}.d.d.|.i...
+00001830: 7d07 7405 7408 a00e 7c07 a101 8301 8201  }.t.t...|.......
+00001840: 6400 0400 7d02 0400 7d05 0400 7d03 7d04  d...}...}...}.}.
+00001850: 6400 5300 290e 4e72 6400 0000 7265 0000  d.S.).Nrd...re..
+00001860: 0072 1100 0000 7251 0000 0072 5d00 0000  .r....rQ...r]...
+00001870: 7a20 5065 7266 6f72 6d61 6e63 6520 7265  z Performance re
+00001880: 636f 7264 2064 6964 206e 6f74 206d 6174  cord did not mat
+00001890: 6368 7220 0000 00a9 017a 4b25 2870 7931  chr .....zK%(py1
+000018a0: 2973 2069 6e20 2528 7079 3829 730a 7b25  )s in %(py8)s.{%
+000018b0: 2870 7938 2973 203d 2025 2870 7933 2973  (py8)s = %(py3)s
+000018c0: 2825 2870 7936 2973 0a7b 2528 7079 3629  (%(py6)s.{%(py6)
+000018d0: 7320 3d20 2528 7079 3429 732e 7661 6c75  s = %(py4)s.valu
+000018e0: 650a 7d29 0a7d 722d 0000 0072 3700 0000  e.}).}r-...r7...
+000018f0: a905 7225 0000 0072 2600 0000 da03 7079  ..r%...r&.....py
+00001900: 34da 0370 7936 da03 7079 38fa 0f61 7373  4..py6..py8..ass
+00001910: 6572 7420 2528 7079 3130 2973 da04 7079  ert %(py10)s..py
+00001920: 3130 290f 720b 0000 0072 0200 0000 7259  10).r....r....rY
+00001930: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
+00001940: 0000 722e 0000 0072 2d00 0000 722f 0000  ..r....r-...r/..
+00001950: 0072 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
+00001960: 7233 0000 0072 3400 0000 7235 0000 0029  r3...r4...r5...)
+00001970: 0872 1500 0000 7237 0000 0072 3800 0000  .r....r7...r8...
+00001980: da0b 4070 795f 6173 7365 7274 35da 0b40  ..@py_assert5..@
+00001990: 7079 5f61 7373 6572 7437 7239 0000 00da  py_assert7r9....
+000019a0: 0b40 7079 5f66 6f72 6d61 7439 da0c 4070  .@py_format9..@p
+000019b0: 795f 666f 726d 6174 3131 7216 0000 0072  y_format11r....r
+000019c0: 1600 0000 7217 0000 00da 1f74 6573 745f  ....r......test_
+000019d0: 6375 7374 6f6d 5f6e 616d 655f 6d75 6c74  custom_name_mult
+000019e0: 6970 6c65 5f63 616c 6c73 6a00 0000 730c  iple_callsj...s.
+000019f0: 0000 0000 010c 012c 020c 010c 014a 027a  .......,.....J.z
+00001a00: 2b52 6563 6f72 6454 6573 7473 2e74 6573  +RecordTests.tes
+00001a10: 745f 6375 7374 6f6d 5f6e 616d 655f 6d75  t_custom_name_mu
+00001a20: 6c74 6970 6c65 5f63 616c 6c73 6301 0000  ltiple_callsc...
+00001a30: 0000 0000 0000 0000 0007 0000 000a 0000  ................
+00001a40: 0043 0000 0073 ca01 0000 7400 8300 9001  .C...s....t.....
+00001a50: 8fac 0100 7401 6401 6402 8d01 8f1e 0100  ....t.d.d.......
+00001a60: 7402 6403 1900 a003 6404 a101 0100 5700  t.d.....d.....W.
+00001a70: 6400 0400 0400 8303 0100 6e10 3100 7338  d.........n.1.s8
+00001a80: 3000 0100 0100 0100 5900 0100 7404 a005  0.......Y...t...
+00001a90: 7406 a101 8f48 7d01 7401 6401 6402 8d01  t....H}.t.d.d...
+00001aa0: 8f1e 0100 7402 6403 1900 a003 6405 a101  ....t.d.....d...
+00001ab0: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
+00001ac0: 3100 737c 3000 0100 0100 0100 5900 0100  1.s|0.......Y...
+00001ad0: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
+00001ae0: 739a 3000 0100 0100 0100 5900 0100 7407  s.0.......Y...t.
+00001af0: 7c01 6a08 8301 7d02 6406 7d03 7c03 7c02  |.j...}.d.}.|.|.
+00001b00: 7600 7d04 7c04 9001 7320 7409 a00a 6407  v.}.|...s t...d.
+00001b10: 7c04 6601 6408 7c03 7c02 6602 a104 7409  |.f.d.|.|.f...t.
+00001b20: a00b 7c03 a101 6409 740c a00d a100 7600  ..|...d.t.....v.
+00001b30: 73f2 7409 a00e 7c02 a101 72fc 7409 a00b  s.t...|...r.t...
+00001b40: 7c02 a101 6e02 6409 640a 9c02 1600 7d05  |...n.d.d.....}.
+00001b50: 640b 640c 7c05 6901 1600 7d06 7406 7409  d.d.|.i...}.t.t.
+00001b60: a00f 7c06 a101 8301 8201 6400 0400 7d03  ..|.......d...}.
+00001b70: 7d04 640d 7d03 7c03 7c02 7600 7d04 7c04  }.d.}.|.|.v.}.|.
+00001b80: 9001 739e 7409 a00a 6407 7c04 6601 6408  ..s.t...d.|.f.d.
+00001b90: 7c03 7c02 6602 a104 7409 a00b 7c03 a101  |.|.f...t...|...
+00001ba0: 6409 740c a00d a100 7600 9001 7370 7409  d.t.....v...spt.
+00001bb0: a00e 7c02 a101 9001 727a 7409 a00b 7c02  ..|.....rzt...|.
+00001bc0: a101 6e02 6409 640a 9c02 1600 7d05 640b  ..n.d.d.....}.d.
+00001bd0: 640c 7c05 6901 1600 7d06 7406 7409 a00f  d.|.i...}.t.t...
+00001be0: 7c06 a101 8301 8201 6400 0400 7d03 7d04  |.......d...}.}.
+00001bf0: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
+00001c00: 9001 73bc 3000 0100 0100 0100 5900 0100  ..s.0.......Y...
+00001c10: 6400 5300 290e 4eda 0974 6573 745f 6469  d.S.).N..test_di
+00001c20: 6666 7265 0000 0072 1100 0000 7251 0000  ffre...r....rQ..
+00001c30: 0072 5d00 0000 7a11 2d20 6361 6368 657c  .r]...z.- cache|
+00001c40: 6765 743a 2066 6f6f 0a72 2000 0000 7222  get: foo.r ...r"
+00001c50: 0000 0072 2300 0000 7224 0000 0072 2700  ...r#...r$...r'.
+00001c60: 0000 7228 0000 007a 112b 2063 6163 6865  ..r(...z.+ cache
+00001c70: 7c67 6574 3a20 6261 720a 2910 720d 0000  |get: bar.).r...
+00001c80: 0072 0b00 0000 7202 0000 0072 5900 0000  .r....r....rY...
+00001c90: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+00001ca0: 2d00 0000 722e 0000 0072 2f00 0000 7230  -...r....r/...r0
+00001cb0: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
+00001cc0: 0000 7234 0000 0072 3500 0000 2907 7215  ..r4...r5...).r.
+00001cd0: 0000 0072 3700 0000 7223 0000 0072 3800  ...r7...r#...r8.
+00001ce0: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
+00001cf0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001d00: 7273 0000 0074 0000 0073 1200 0000 0001  rs...t...s......
+00001d10: 0a01 0c01 2c02 0c01 0c01 4a02 0a01 7a01  ....,.....J...z.
+00001d20: 7a15 5265 636f 7264 5465 7374 732e 7465  z.RecordTests.te
+00001d30: 7374 5f64 6966 6663 0100 0000 0000 0000  st_diffc........
+00001d40: 0000 0000 0600 0000 0900 0000 4300 0000  ............C...
+00001d50: 73ea 0000 0074 0064 0183 018f ce01 0074  s....t.d.......t
+00001d60: 0164 0164 028d 018f 1e01 0074 0264 0319  .d.d.......t.d..
+00001d70: 00a0 0364 04a1 0101 0057 0064 0004 0004  ...d.....W.d....
+00001d80: 0083 0301 006e 1031 0073 3830 0001 0001  .....n.1.s80....
+00001d90: 0001 0059 0001 0074 046a 057d 017c 016a  ...Y...t.j.}.|.j
+00001da0: 067d 0264 017d 037c 027c 0383 017d 047c  .}.d.}.|.|...}.|
+00001db0: 0473 b864 0564 0674 07a0 08a1 0076 0073  .s.d.d.t.....v.s
+00001dc0: 7674 09a0 0a74 04a1 0172 8074 09a0 0b74  vt...t...r.t...t
+00001dd0: 04a1 016e 0264 0674 09a0 0b7c 01a1 0174  ...n.d.t...|...t
+00001de0: 09a0 0b7c 02a1 0174 09a0 0b7c 03a1 0174  ...|...t...|...t
+00001df0: 09a0 0b7c 04a1 0164 079c 0516 007d 0574  ...|...d.....}.t
+00001e00: 0c74 09a0 0d7c 05a1 0183 0182 0164 0004  .t...|.......d..
+00001e10: 007d 0104 007d 0204 007d 037d 0457 0064  .}...}...}.}.W.d
+00001e20: 0004 0004 0083 0301 006e 1031 0073 dc30  .........n.1.s.0
+00001e30: 0001 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00001e40: 084e fa0f 6375 7374 6f6d 2e70 6572 662e  .N..custom.perf.
+00001e50: 796d 6ca9 01da 0470 6174 6872 1100 0000  yml....pathr....
+00001e60: 7251 0000 007a 6261 7373 6572 7420 2528  rQ...zbassert %(
+00001e70: 7079 3829 730a 7b25 2870 7938 2973 203d  py8)s.{%(py8)s =
+00001e80: 2025 2870 7934 2973 0a7b 2528 7079 3429   %(py4)s.{%(py4)
+00001e90: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
+00001ea0: 7932 2973 203d 2025 2870 7930 2973 2e70  y2)s = %(py0)s.p
+00001eb0: 6174 680a 7d2e 6578 6973 7473 0a7d 2825  ath.}.exists.}(%
+00001ec0: 2870 7936 2973 290a 7dda 026f 7329 05da  (py6)s).}..os)..
+00001ed0: 0370 7930 da03 7079 3272 6900 0000 726a  .py0..py2ri...rj
+00001ee0: 0000 0072 6b00 0000 290e 720f 0000 0072  ...rk...).r....r
+00001ef0: 0b00 0000 7202 0000 0072 5900 0000 7277  ....r....rY...rw
+00001f00: 0000 0072 7600 0000 da06 6578 6973 7473  ...rv.....exists
+00001f10: 7232 0000 0072 3300 0000 722f 0000 0072  r2...r3...r/...r
+00001f20: 3400 0000 7231 0000 0072 2c00 0000 7235  4...r1...r,...r5
+00001f30: 0000 0029 0672 1500 0000 da0b 4070 795f  ...).r......@py_
+00001f40: 6173 7365 7274 31da 0b40 7079 5f61 7373  assert1..@py_ass
+00001f50: 6572 7433 726e 0000 0072 6f00 0000 7270  ert3rn...ro...rp
+00001f60: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00001f70: 0000 da1e 7465 7374 5f70 6174 685f 706f  ....test_path_po
+00001f80: 696e 7469 6e67 5f74 6f5f 6669 6c65 6e61  inting_to_filena
+00001f90: 6d65 8100 0000 7308 0000 0000 010a 020c  me....s.........
+00001fa0: 012c 027a 2a52 6563 6f72 6454 6573 7473  .,.z*RecordTests
+00001fb0: 2e74 6573 745f 7061 7468 5f70 6f69 6e74  .test_path_point
+00001fc0: 696e 675f 746f 5f66 696c 656e 616d 6563  ing_to_filenamec
+00001fd0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001fe0: 0900 0000 4300 0000 739c 0000 0074 0064  ....C...s....t.d
+00001ff0: 0183 018f 8001 0074 0164 0164 028d 018f  .......t.d.d....
+00002000: 1e01 0074 0264 0319 00a0 0364 04a1 0101  ...t.d.....d....
+00002010: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00002020: 0073 3830 0001 0001 0001 0059 0001 0074  .s80.......Y...t
+00002030: 0164 0164 028d 018f 1e01 0074 0264 0319  .d.d.......t.d..
+00002040: 00a0 0364 04a1 0101 0057 0064 0004 0004  ...d.....W.d....
+00002050: 0083 0301 006e 1031 0073 7030 0001 0001  .....n.1.sp0....
+00002060: 0001 0059 0001 0057 0064 0004 0004 0083  ...Y...W.d......
+00002070: 0301 006e 1031 0073 8e30 0001 0001 0001  ...n.1.s.0......
+00002080: 0059 0001 0064 0053 0029 054e 7274 0000  .Y...d.S.).Nrt..
+00002090: 0072 7500 0000 7211 0000 0072 5100 0000  .ru...r....rQ...
+000020a0: 2904 720f 0000 0072 0b00 0000 7202 0000  ).r....r....r...
+000020b0: 0072 5900 0000 7214 0000 0072 1600 0000  .rY...r....r....
+000020c0: 7216 0000 0072 1700 0000 da2b 7465 7374  r....r.....+test
+000020d0: 5f70 6174 685f 706f 696e 7469 6e67 5f74  _path_pointing_t
+000020e0: 6f5f 6669 6c65 6e61 6d65 5f72 6563 6f72  o_filename_recor
+000020f0: 645f 7477 6963 6589 0000 0073 0a00 0000  d_twice....s....
+00002100: 0001 0a02 0c01 2c02 0c01 7a37 5265 636f  ......,...z7Reco
+00002110: 7264 5465 7374 732e 7465 7374 5f70 6174  rdTests.test_pat
+00002120: 685f 706f 696e 7469 6e67 5f74 6f5f 6669  h_pointing_to_fi
+00002130: 6c65 6e61 6d65 5f72 6563 6f72 645f 7477  lename_record_tw
+00002140: 6963 6563 0100 0000 0000 0000 0000 0000  icec............
+00002150: 0700 0000 0900 0000 4300 0000 731c 0100  ........C...s...
+00002160: 0074 006a 01a0 0274 0364 01a1 027d 0174  .t.j...t.d...}.t
+00002170: 047c 0183 018f f001 0074 0564 0164 028d  .|.......t.d.d..
+00002180: 018f 1e01 0074 0664 0319 00a0 0764 04a1  .....t.d.....d..
+00002190: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+000021a0: 1031 0073 4630 0001 0001 0001 0059 0001  .1.sF0.......Y..
+000021b0: 0074 006a 01a0 0274 0364 0564 06a1 037d  .t.j...t.d.d...}
+000021c0: 0274 006a 017d 037c 036a 087d 047c 047c  .t.j.}.|.j.}.|.|
+000021d0: 0283 017d 057c 0573 ec64 0764 0874 09a0  ...}.|.s.d.d.t..
+000021e0: 0aa1 0076 0073 9074 0ba0 0c74 00a1 0172  ...v.s.t...t...r
+000021f0: 9a74 0ba0 0d74 00a1 016e 0264 0874 0ba0  .t...t...n.d.t..
+00002200: 0d7c 03a1 0174 0ba0 0d7c 04a1 0164 0974  .|...t...|...d.t
+00002210: 09a0 0aa1 0076 0073 c274 0ba0 0c7c 02a1  .....v.s.t...|..
+00002220: 0172 cc74 0ba0 0d7c 02a1 016e 0264 0974  .r.t...|...n.d.t
+00002230: 0ba0 0d7c 05a1 0164 0a9c 0516 007d 0674  ...|...d.....}.t
+00002240: 0e74 0ba0 0f7c 06a1 0183 0182 0164 0004  .t...|.......d..
+00002250: 007d 0304 007d 047d 0557 0064 0004 0004  .}...}.}.W.d....
+00002260: 0083 0301 006e 1231 0090 0173 0e30 0001  .....n.1...s.0..
+00002270: 0001 0001 0059 0001 0064 0053 0029 0b4e  .....Y...d.S.).N
+00002280: fa0b 7065 7266 5f66 696c 6573 2f72 7500  ..perf_files/ru.
+00002290: 0000 7211 0000 0072 5100 0000 da0a 7065  ..r....rQ.....pe
+000022a0: 7266 5f66 696c 6573 fa11 7465 7374 5f61  rf_files..test_a
+000022b0: 7069 2e70 6572 662e 796d 6cfa 6261 7373  pi.perf.yml.bass
+000022c0: 6572 7420 2528 7079 3729 730a 7b25 2870  ert %(py7)s.{%(p
+000022d0: 7937 2973 203d 2025 2870 7934 2973 0a7b  y7)s = %(py4)s.{
+000022e0: 2528 7079 3429 7320 3d20 2528 7079 3229  %(py4)s = %(py2)
+000022f0: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
+00002300: 7930 2973 2e70 6174 680a 7d2e 6578 6973  y0)s.path.}.exis
+00002310: 7473 0a7d 2825 2870 7935 2973 290a 7d72  ts.}(%(py5)s).}r
+00002320: 7700 0000 da09 6675 6c6c 5f70 6174 68a9  w.....full_path.
+00002330: 0572 7800 0000 7279 0000 0072 6900 0000  .rx...ry...ri...
+00002340: 7228 0000 00da 0370 7937 a910 7277 0000  r(.....py7..rw..
+00002350: 0072 7600 0000 da04 6a6f 696e da08 4649  .rv.....join..FI
+00002360: 4c45 5f44 4952 720f 0000 0072 0b00 0000  LE_DIRr....r....
+00002370: 7202 0000 0072 5900 0000 727a 0000 0072  r....rY...rz...r
+00002380: 3200 0000 7233 0000 0072 2f00 0000 7234  2...r3...r/...r4
+00002390: 0000 0072 3100 0000 722c 0000 0072 3500  ...r1...r,...r5.
+000023a0: 0000 a907 7215 0000 00da 0874 656d 705f  ....r......temp_
+000023b0: 6469 7272 8300 0000 727b 0000 0072 7c00  dirr....r{...r|.
+000023c0: 0000 da0b 4070 795f 6173 7365 7274 36da  ....@py_assert6.
+000023d0: 0b40 7079 5f66 6f72 6d61 7438 7216 0000  .@py_format8r...
+000023e0: 0072 1600 0000 7217 0000 00da 1974 6573  .r....r......tes
+000023f0: 745f 7061 7468 5f70 6f69 6e74 696e 675f  t_path_pointing_
+00002400: 746f 5f64 6972 9200 0000 730c 0000 0000  to_dir....s.....
+00002410: 010e 010a 020c 012c 0210 017a 2552 6563  .......,...z%Rec
+00002420: 6f72 6454 6573 7473 2e74 6573 745f 7061  ordTests.test_pa
+00002430: 7468 5f70 6f69 6e74 696e 675f 746f 5f64  th_pointing_to_d
+00002440: 6972 6301 0000 0000 0000 0000 0000 0007  irc.............
+00002450: 0000 0009 0000 0043 0000 0073 1e01 0000  .......C...s....
+00002460: 7400 6a01 a002 7403 6401 a102 7d01 7404  t.j...t.d...}.t.
+00002470: 7c01 8301 8ff2 0100 7405 6402 6403 8d01  |.......t.d.d...
+00002480: 8f1e 0100 7406 6404 1900 a007 6405 a101  ....t.d.....d...
+00002490: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
+000024a0: 3100 7346 3000 0100 0100 0100 5900 0100  1.sF0.......Y...
+000024b0: 7400 6a01 a002 7403 6406 6407 6408 a104  t.j...t.d.d.d...
+000024c0: 7d02 7400 6a01 7d03 7c03 6a08 7d04 7c04  }.t.j.}.|.j.}.|.
+000024d0: 7c02 8301 7d05 7c05 73ee 6409 640a 7409  |...}.|.s.d.d.t.
+000024e0: a00a a100 7600 7392 740b a00c 7400 a101  ....v.s.t...t...
+000024f0: 729c 740b a00d 7400 a101 6e02 640a 740b  r.t...t...n.d.t.
+00002500: a00d 7c03 a101 740b a00d 7c04 a101 640b  ..|...t...|...d.
+00002510: 7409 a00a a100 7600 73c4 740b a00c 7c02  t.....v.s.t...|.
+00002520: a101 72ce 740b a00d 7c02 a101 6e02 640b  ..r.t...|...n.d.
+00002530: 740b a00d 7c05 a101 640c 9c05 1600 7d06  t...|...d.....}.
+00002540: 740e 740b a00f 7c06 a101 8301 8201 6400  t.t...|.......d.
+00002550: 0400 7d03 0400 7d04 7d05 5700 6400 0400  ..}...}.}.W.d...
+00002560: 0400 8303 0100 6e12 3100 9001 7310 3000  ......n.1...s.0.
+00002570: 0100 0100 0100 5900 0100 6400 5300 a90d  ......Y...d.S...
+00002580: 4e72 7f00 0000 fa0f 7065 7266 5f66 696c  Nr......perf_fil
+00002590: 6573 2f61 7069 2f72 7500 0000 7211 0000  es/api/ru...r...
+000025a0: 0072 5100 0000 7280 0000 00da 0361 7069  .rQ...r......api
+000025b0: 7281 0000 0072 8200 0000 7277 0000 0072  r....r....rw...r
+000025c0: 8300 0000 7284 0000 0072 8600 0000 7289  ....r....r....r.
+000025d0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000025e0: 0000 da17 7465 7374 5f63 7573 746f 6d5f  ....test_custom_
+000025f0: 6e65 7374 6564 5f70 6174 689c 0000 0073  nested_path....s
+00002600: 0c00 0000 0001 0e01 0a02 0c01 2c02 1201  ............,...
+00002610: 7a23 5265 636f 7264 5465 7374 732e 7465  z#RecordTests.te
+00002620: 7374 5f63 7573 746f 6d5f 6e65 7374 6564  st_custom_nested
+00002630: 5f70 6174 68da 044d 4f44 45da 046f 6e63  _path..MODE..onc
+00002640: 6563 0100 0000 0000 0000 0000 0000 0700  ec..............
+00002650: 0000 0900 0000 4300 0000 731e 0100 0074  ......C...s....t
+00002660: 006a 01a0 0274 0364 01a1 027d 0174 047c  .j...t.d...}.t.|
+00002670: 0183 018f f201 0074 0564 0264 038d 018f  .......t.d.d....
+00002680: 1e01 0074 0664 0419 00a0 0764 05a1 0101  ...t.d.....d....
+00002690: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+000026a0: 0073 4630 0001 0001 0001 0059 0001 0074  .sF0.......Y...t
+000026b0: 006a 01a0 0274 0364 0664 0764 08a1 047d  .j...t.d.d.d...}
+000026c0: 0274 006a 017d 037c 036a 087d 047c 047c  .t.j.}.|.j.}.|.|
+000026d0: 0283 017d 057c 0573 ee64 0964 0a74 09a0  ...}.|.s.d.d.t..
+000026e0: 0aa1 0076 0073 9274 0ba0 0c74 00a1 0172  ...v.s.t...t...r
+000026f0: 9c74 0ba0 0d74 00a1 016e 0264 0a74 0ba0  .t...t...n.d.t..
+00002700: 0d7c 03a1 0174 0ba0 0d7c 04a1 0164 0b74  .|...t...|...d.t
+00002710: 09a0 0aa1 0076 0073 c474 0ba0 0c7c 02a1  .....v.s.t...|..
+00002720: 0172 ce74 0ba0 0d7c 02a1 016e 0264 0b74  .r.t...|...n.d.t
+00002730: 0ba0 0d7c 05a1 0164 0c9c 0516 007d 0674  ...|...d.....}.t
+00002740: 0e74 0ba0 0f7c 06a1 0183 0182 0164 0004  .t...|.......d..
+00002750: 007d 0304 007d 047d 0557 0064 0004 0004  .}...}.}.W.d....
+00002760: 0083 0301 006e 1231 0090 0173 1030 0001  .....n.1...s.0..
+00002770: 0001 0001 0059 0001 0064 0053 0072 8e00  .....Y...d.S.r..
+00002780: 0000 7286 0000 0072 8900 0000 7216 0000  ..r....r....r...
+00002790: 0072 1600 0000 7217 0000 00da 0e74 6573  .r....r......tes
+000027a0: 745f 6d6f 6465 5f6f 6e63 65a6 0000 0073  t_mode_once....s
+000027b0: 0c00 0000 0002 0e01 0a02 0c01 2c02 1201  ............,...
+000027c0: 7a1a 5265 636f 7264 5465 7374 732e 7465  z.RecordTests.te
+000027d0: 7374 5f6d 6f64 655f 6f6e 6365 da04 6e6f  st_mode_once..no
+000027e0: 6e65 6301 0000 0000 0000 0000 0000 000e  nec.............
+000027f0: 0000 000a 0000 0043 0000 0073 2002 0000  .......C...s ...
+00002800: 7400 6a01 a002 7403 6401 a102 7d01 7404  t.j...t.d...}.t.
+00002810: 7c01 8301 9001 8ff2 0100 7405 a006 7407  |.........t...t.
+00002820: a101 8f48 7d02 7408 6402 6403 8d01 8f1e  ...H}.t.d.d.....
+00002830: 0100 7409 6404 1900 a00a 6405 a101 0100  ..t.d.....d.....
+00002840: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
+00002850: 7354 3000 0100 0100 0100 5900 0100 5700  sT0.......Y...W.
+00002860: 6400 0400 0400 8303 0100 6e10 3100 7372  d.........n.1.sr
+00002870: 3000 0100 0100 0100 5900 0100 6406 7d03  0.......Y...d.}.
+00002880: 7c02 6a0b 7d04 740c 7c04 8301 7d05 7c03  |.j.}.t.|...}.|.
+00002890: 7c05 7600 7d06 7c06 9001 732e 740d a00e  |.v.}.|...s.t...
+000028a0: 6407 7c06 6601 6408 7c03 7c05 6602 a104  d.|.f.d.|.|.f...
+000028b0: 740d a00f 7c03 a101 6409 7410 a011 a100  t...|...d.t.....
+000028c0: 7600 73ce 740d a012 740c a101 72d8 740d  v.s.t...t...r.t.
+000028d0: a00f 740c a101 6e02 6409 640a 7410 a011  ..t...n.d.d.t...
+000028e0: a100 7600 73f0 740d a012 7c02 a101 72fa  ..v.s.t...|...r.
+000028f0: 740d a00f 7c02 a101 6e02 640a 740d a00f  t...|...n.d.t...
+00002900: 7c04 a101 740d a00f 7c05 a101 640b 9c05  |...t...|...d...
+00002910: 1600 7d07 640c 640d 7c07 6901 1600 7d08  ..}.d.d.|.i...}.
+00002920: 7407 740d a013 7c08 a101 8301 8201 6400  t.t...|.......d.
+00002930: 0400 7d03 0400 7d06 0400 7d04 7d05 7400  ..}...}...}.}.t.
+00002940: 6a01 a002 7403 640e 640f 6410 a104 7d09  j...t.d.d.d...}.
+00002950: 7400 6a01 7d0a 7c0a 6a14 7d0b 7c0b 7c09  t.j.}.|.j.}.|.|.
+00002960: 8301 7d0c 7c0c 0c00 7d0d 7c0d 9001 73ec  ..}.|...}.|...s.
+00002970: 6411 6412 7410 a011 a100 7600 9001 738c  d.d.t.....v...s.
+00002980: 740d a012 7400 a101 9001 7296 740d a00f  t...t.....r.t...
+00002990: 7400 a101 6e02 6412 740d a00f 7c0a a101  t...n.d.t...|...
+000029a0: 740d a00f 7c0b a101 6413 7410 a011 a100  t...|...d.t.....
+000029b0: 7600 9001 73c2 740d a012 7c09 a101 9001  v...s.t...|.....
+000029c0: 72cc 740d a00f 7c09 a101 6e02 6413 740d  r.t...|...n.d.t.
+000029d0: a00f 7c0c a101 6414 9c05 1600 7d07 7407  ..|...d.....}.t.
+000029e0: 740d a013 7c07 a101 8301 8201 6400 0400  t...|.......d...
+000029f0: 7d0a 0400 7d0b 0400 7d0c 7d0d 5700 6400  }...}...}.}.W.d.
+00002a00: 0400 0400 8303 0100 6e12 3100 9002 7312  ........n.1...s.
+00002a10: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00002a20: 2915 4e72 7f00 0000 728f 0000 0072 7500  ).Nr....r....ru.
+00002a30: 0000 7211 0000 0072 5100 0000 7a2a 4f72  ..r....rQ...z*Or
+00002a40: 6967 696e 616c 2070 6572 666f 726d 616e  iginal performan
+00002a50: 6365 2072 6563 6f72 6420 646f 6573 206e  ce record does n
+00002a60: 6f74 2065 7869 7374 7220 0000 0072 6700  ot existr ...rg.
+00002a70: 0000 722d 0000 0072 3700 0000 7268 0000  ..r-...r7...rh..
+00002a80: 0072 6c00 0000 726d 0000 0072 8000 0000  .rl...rm...r....
+00002a90: 7290 0000 0072 8100 0000 7a66 6173 7365  r....r....zfasse
+00002aa0: 7274 206e 6f74 2025 2870 7937 2973 0a7b  rt not %(py7)s.{
+00002ab0: 2528 7079 3729 7320 3d20 2528 7079 3429  %(py7)s = %(py4)
+00002ac0: 730a 7b25 2870 7934 2973 203d 2025 2870  s.{%(py4)s = %(p
+00002ad0: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
+00002ae0: 2528 7079 3029 732e 7061 7468 0a7d 2e65  %(py0)s.path.}.e
+00002af0: 7869 7374 730a 7d28 2528 7079 3529 7329  xists.}(%(py5)s)
+00002b00: 0a7d 7277 0000 0072 8300 0000 7284 0000  .}rw...r....r...
+00002b10: 00a9 1572 7700 0000 7276 0000 0072 8700  ...rw...rv...r..
+00002b20: 0000 7288 0000 0072 0f00 0000 722a 0000  ..r....r....r*..
+00002b30: 0072 2b00 0000 722c 0000 0072 0b00 0000  .r+...r,...r....
+00002b40: 7202 0000 0072 5900 0000 722e 0000 0072  r....rY...r....r
+00002b50: 2d00 0000 722f 0000 0072 3000 0000 7231  -...r/...r0...r1
+00002b60: 0000 0072 3200 0000 7233 0000 0072 3400  ...r2...r3...r4.
+00002b70: 0000 7235 0000 0072 7a00 0000 290e 7215  ..r5...rz...).r.
+00002b80: 0000 0072 8a00 0000 7237 0000 0072 3800  ...r....r7...r8.
+00002b90: 0000 726e 0000 0072 6f00 0000 7239 0000  ..rn...ro...r9..
+00002ba0: 0072 7000 0000 7271 0000 0072 8300 0000  .rp...rq...r....
+00002bb0: 727b 0000 0072 7c00 0000 728b 0000 00da  r{...r|...r.....
+00002bc0: 0b40 7079 5f61 7373 6572 7438 7216 0000  .@py_assert8r...
+00002bd0: 0072 1600 0000 7217 0000 00da 0e74 6573  .r....r......tes
+00002be0: 745f 6d6f 6465 5f6e 6f6e 65b1 0000 0073  t_mode_none....s
+00002bf0: 1000 0000 0002 0e01 0c02 0c02 0c01 4a02  ..............J.
+00002c00: c202 1201 7a1a 5265 636f 7264 5465 7374  ....z.RecordTest
+00002c10: 732e 7465 7374 5f6d 6f64 655f 6e6f 6e65  s.test_mode_none
+00002c20: 7241 0000 0063 0100 0000 0000 0000 0000  rA...c..........
+00002c30: 0000 0e00 0000 0a00 0000 4300 0000 7316  ..........C...s.
+00002c40: 0200 0074 006a 01a0 0274 0364 01a1 027d  ...t.j...t.d...}
+00002c50: 0174 047c 0183 0190 018f e801 0074 05a0  .t.|.........t..
+00002c60: 0674 07a1 018f 487d 0274 0864 0264 038d  .t....H}.t.d.d..
+00002c70: 018f 1e01 0074 0964 0419 00a0 0a64 05a1  .....t.d.....d..
+00002c80: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00002c90: 1031 0073 5430 0001 0001 0001 0059 0001  .1.sT0.......Y..
+00002ca0: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
+00002cb0: 0073 7230 0001 0001 0001 0059 0001 0064  .sr0.......Y...d
+00002cc0: 067d 037c 026a 0b7d 0474 0c7c 0483 017d  .}.|.j.}.t.|...}
+00002cd0: 057c 037c 0576 007d 067c 0690 0173 2e74  .|.|.v.}.|...s.t
+00002ce0: 0da0 0e64 077c 0666 0164 087c 037c 0566  ...d.|.f.d.|.|.f
+00002cf0: 02a1 0474 0da0 0f7c 03a1 0164 0974 10a0  ...t...|...d.t..
+00002d00: 11a1 0076 0073 ce74 0da0 1274 0ca1 0172  ...v.s.t...t...r
+00002d10: d874 0da0 0f74 0ca1 016e 0264 0964 0a74  .t...t...n.d.d.t
+00002d20: 10a0 11a1 0076 0073 f074 0da0 127c 02a1  .....v.s.t...|..
+00002d30: 0172 fa74 0da0 0f7c 02a1 016e 0264 0a74  .r.t...|...n.d.t
+00002d40: 0da0 0f7c 04a1 0174 0da0 0f7c 05a1 0164  ...|...t...|...d
+00002d50: 0b9c 0516 007d 0764 0c64 0d7c 0769 0116  .....}.d.d.|.i..
+00002d60: 007d 0874 0774 0da0 137c 08a1 0183 0182  .}.t.t...|......
+00002d70: 0164 0004 007d 0304 007d 0604 007d 047d  .d...}...}...}.}
+00002d80: 0574 006a 01a0 0274 0364 0e64 0f64 10a1  .t.j...t.d.d.d..
+00002d90: 047d 0974 006a 017d 0a7c 0a6a 147d 0b7c  .}.t.j.}.|.j.}.|
+00002da0: 0b7c 0983 017d 0c7c 0c90 0173 e664 1164  .|...}.|...s.d.d
+00002db0: 1274 10a0 11a1 0076 0090 0173 8674 0da0  .t.....v...s.t..
+00002dc0: 1274 00a1 0190 0172 9074 0da0 0f74 00a1  .t.....r.t...t..
+00002dd0: 016e 0264 1274 0da0 0f7c 0aa1 0174 0da0  .n.d.t...|...t..
+00002de0: 0f7c 0ba1 0164 1374 10a0 11a1 0076 0090  .|...d.t.....v..
+00002df0: 0173 bc74 0da0 127c 09a1 0190 0172 c674  .s.t...|.....r.t
+00002e00: 0da0 0f7c 09a1 016e 0264 1374 0da0 0f7c  ...|...n.d.t...|
+00002e10: 0ca1 0164 149c 0516 007d 0d74 0774 0da0  ...d.....}.t.t..
+00002e20: 137c 0da1 0183 0182 0164 0004 007d 0a04  .|.......d...}..
+00002e30: 007d 0b7d 0c57 0064 0004 0004 0083 0301  .}.}.W.d........
+00002e40: 006e 1231 0090 0273 0830 0001 0001 0001  .n.1...s.0......
+00002e50: 0059 0001 0064 0053 0029 154e 727f 0000  .Y...d.S.).Nr...
+00002e60: 0072 8f00 0000 7275 0000 0072 1100 0000  .r....ru...r....
+00002e70: 7251 0000 007a 294f 7269 6769 6e61 6c20  rQ...z)Original 
+00002e80: 7065 7266 6f72 6d61 6e63 6520 7265 636f  performance reco
+00002e90: 7264 2064 6964 206e 6f74 2065 7869 7374  rd did not exist
+00002ea0: 7220 0000 0072 6700 0000 722d 0000 0072  r ...rg...r-...r
+00002eb0: 3700 0000 7268 0000 0072 6c00 0000 726d  7...rh...rl...rm
+00002ec0: 0000 0072 8000 0000 7290 0000 0072 8100  ...r....r....r..
+00002ed0: 0000 7282 0000 0072 7700 0000 7283 0000  ..r....rw...r...
+00002ee0: 0072 8400 0000 7296 0000 0029 0e72 1500  .r....r....).r..
+00002ef0: 0000 728a 0000 0072 3700 0000 7238 0000  ..r....r7...r8..
+00002f00: 0072 6e00 0000 726f 0000 0072 3900 0000  .rn...ro...r9...
+00002f10: 7270 0000 0072 7100 0000 7283 0000 0072  rp...rq...r....r
+00002f20: 7b00 0000 727c 0000 0072 8b00 0000 728c  {...r|...r....r.
+00002f30: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+00002f40: 0000 da0d 7465 7374 5f6d 6f64 655f 616c  ....test_mode_al
+00002f50: 6cc0 0000 0073 1000 0000 0002 0e01 0c02  l....s..........
+00002f60: 0c02 0c01 4a02 c202 1201 7a19 5265 636f  ....J.....z.Reco
+00002f70: 7264 5465 7374 732e 7465 7374 5f6d 6f64  rdTests.test_mod
+00002f80: 655f 616c 6c63 0100 0000 0000 0000 0000  e_allc..........
+00002f90: 0000 0200 0000 0800 0000 4300 0000 7342  ..........C...sB
+00002fa0: 0000 0074 006a 016a 0264 0164 0264 038d  ...t.j.j.d.d.d..
+00002fb0: 027d 0174 0383 008f 1801 007c 01a0 04a1  .}.t.......|....
+00002fc0: 0001 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00002fd0: 1031 0073 3430 0001 0001 0001 0059 0001  .1.s40.......Y..
+00002fe0: 0064 0053 0029 044e 5a06 4172 7468 7572  .d.S.).NZ.Arthur
+00002ff0: e92a 0000 0072 5300 0000 2905 720c 0000  .*...rS...).r...
+00003000: 0072 4000 0000 da06 6372 6561 7465 720b  .r@.....creater.
+00003010: 0000 0072 6100 0000 2902 7215 0000 005a  ...ra...).r....Z
+00003020: 0661 7274 6875 7272 1600 0000 7216 0000  .arthurr....r...
+00003030: 0072 1700 0000 da23 7465 7374 5f64 656c  .r.....#test_del
+00003040: 6574 655f 6f6e 5f63 6173 6361 6465 5f63  ete_on_cascade_c
+00003050: 616c 6c65 645f 7477 6963 65cf 0000 0073  alled_twice....s
+00003060: 0600 0000 0001 1001 0801 7a2f 5265 636f  ..........z/Reco
+00003070: 7264 5465 7374 732e 7465 7374 5f64 656c  rdTests.test_del
+00003080: 6574 655f 6f6e 5f63 6173 6361 6465 5f63  ete_on_cascade_c
+00003090: 616c 6c65 645f 7477 6963 654e 291b da08  alled_twiceN)...
+000030a0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000030b0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000030c0: 5f5f 7218 0000 0072 3c00 0000 7242 0000  __r....r<...rB..
+000030d0: 0072 0700 0000 7245 0000 0072 4600 0000  .r....rE...rF...
+000030e0: 724c 0000 0072 5000 0000 7256 0000 0072  rL...rP...rV...r
+000030f0: 5a00 0000 725c 0000 0072 6200 0000 7263  Z...r\...rb...rc
+00003100: 0000 0072 6600 0000 7272 0000 0072 7300  ...rf...rr...rs.
+00003110: 0000 727d 0000 0072 7e00 0000 728d 0000  ..r}...r~...r...
+00003120: 0072 9100 0000 7294 0000 0072 9800 0000  .r....r....r....
+00003130: 7299 0000 0072 9c00 0000 7216 0000 0072  r....r....r....r
+00003140: 1600 0000 7216 0000 0072 1700 0000 7210  ....r....r....r.
+00003150: 0000 0010 0000 0073 3600 0000 0801 0804  .......s6.......
+00003160: 0815 0804 0c01 0a04 0805 0804 0804 0804  ................
+00003170: 0804 0811 0806 0807 0804 080a 080d 0808  ................
+00003180: 0809 080a 080a 0c01 0a0a 0c01 0a0e 0c01  ................
+00003190: 0a0e 7210 0000 0063 0000 0000 0000 0000  ..r....c........
+000031a0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+000031b0: 7324 0000 0065 005a 0164 005a 0264 0164  s$...e.Z.d.Z.d.d
+000031c0: 0284 005a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
+000031d0: 0684 005a 0564 0753 0029 08da 1047 6574  ...Z.d.S.)...Get
+000031e0: 5065 7266 5061 7468 5465 7374 7363 0100  PerfPathTestsc..
+000031f0: 0000 0000 0000 0000 0000 0700 0000 0700  ................
+00003200: 0000 4300 0000 73a0 0000 0064 017d 0174  ..C...s....d.}.t
+00003210: 007c 0183 017d 0264 027d 037c 027c 036b  .|...}.d.}.|.|.k
+00003220: 027d 047c 0473 8c74 01a0 0264 037c 0466  .}.|.s.t...d.|.f
+00003230: 0164 047c 027c 0366 02a1 0464 0574 03a0  .d.|.|.f...d.t..
+00003240: 04a1 0076 0073 4674 01a0 0574 00a1 0172  ...v.sFt...t...r
+00003250: 5074 01a0 0674 00a1 016e 0264 0574 01a0  Pt...t...n.d.t..
+00003260: 067c 01a1 0174 01a0 067c 02a1 0174 01a0  .|...t...|...t..
+00003270: 067c 03a1 0164 069c 0416 007d 0564 0764  .|...d.....}.d.d
+00003280: 087c 0569 0116 007d 0674 0774 01a0 087c  .|.i...}.t.t...|
+00003290: 06a1 0183 0182 0164 0004 007d 0104 007d  .......d...}...}
+000032a0: 0204 007d 047d 0364 0053 0029 094e fa06  ...}.}.d.S.).N..
+000032b0: 666f 6f2e 7079 fa0c 666f 6f2e 7065 7266  foo.py..foo.perf
+000032c0: 2e79 6d6c a901 fa02 3d3d a901 7a30 2528  .yml....==..z0%(
+000032d0: 7079 3429 730a 7b25 2870 7934 2973 203d  py4)s.{%(py4)s =
+000032e0: 2025 2870 7930 2973 2825 2870 7932 2973   %(py0)s(%(py2)s
+000032f0: 290a 7d20 3d3d 2025 2870 7937 2973 7209  ).} == %(py7)sr.
+00003300: 0000 00a9 0472 7800 0000 7279 0000 0072  .....rx...ry...r
+00003310: 6900 0000 7285 0000 00fa 0e61 7373 6572  i...r......asser
+00003320: 7420 2528 7079 3929 73da 0370 7939 a909  t %(py9)s..py9..
+00003330: 7209 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00003340: 3200 0000 7233 0000 0072 3400 0000 7231  2...r3...r4...r1
+00003350: 0000 0072 2c00 0000 7235 0000 00a9 0772  ...r,...r5.....r
+00003360: 1500 0000 727b 0000 0072 7c00 0000 728b  ....r{...r|...r.
+00003370: 0000 0072 6e00 0000 728c 0000 00da 0c40  ...rn...r......@
+00003380: 7079 5f66 6f72 6d61 7431 3072 1600 0000  py_format10r....
+00003390: 7216 0000 0072 1700 0000 da0c 7465 7374  r....r......test
+000033a0: 5f70 795f 6669 6c65 d600 0000 7302 0000  _py_file....s...
+000033b0: 0000 017a 1d47 6574 5065 7266 5061 7468  ...z.GetPerfPath
+000033c0: 5465 7374 732e 7465 7374 5f70 795f 6669  Tests.test_py_fi
+000033d0: 6c65 6301 0000 0000 0000 0000 0000 0007  lec.............
+000033e0: 0000 0007 0000 0043 0000 0073 a000 0000  .......C...s....
+000033f0: 6401 7d01 7400 7c01 8301 7d02 6402 7d03  d.}.t.|...}.d.}.
+00003400: 7c02 7c03 6b02 7d04 7c04 738c 7401 a002  |.|.k.}.|.s.t...
+00003410: 6403 7c04 6601 6404 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00003420: 6405 7403 a004 a100 7600 7346 7401 a005  d.t.....v.sFt...
+00003430: 7400 a101 7250 7401 a006 7400 a101 6e02  t...rPt...t...n.
+00003440: 6405 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
+00003450: a101 7401 a006 7c03 a101 6406 9c04 1600  ..t...|...d.....
+00003460: 7d05 6407 6408 7c05 6901 1600 7d06 7407  }.d.d.|.i...}.t.
+00003470: 7401 a008 7c06 a101 8301 8201 6400 0400  t...|.......d...
+00003480: 7d01 0400 7d02 0400 7d04 7d03 6400 5300  }...}...}.}.d.S.
+00003490: 2909 4e7a 0766 6f6f 2e70 7963 72a2 0000  ).Nz.foo.pycr...
+000034a0: 0072 a300 0000 72a5 0000 0072 0900 0000  .r....r....r....
+000034b0: 72a6 0000 0072 a700 0000 72a8 0000 0072  r....r....r....r
+000034c0: a900 0000 72aa 0000 0072 1600 0000 7216  ....r....r....r.
+000034d0: 0000 0072 1700 0000 da0d 7465 7374 5f70  ...r......test_p
+000034e0: 7963 5f66 696c 65d9 0000 0073 0200 0000  yc_file....s....
+000034f0: 0001 7a1e 4765 7450 6572 6650 6174 6854  ..z.GetPerfPathT
+00003500: 6573 7473 2e74 6573 745f 7079 635f 6669  ests.test_pyc_fi
+00003510: 6c65 6301 0000 0000 0000 0000 0000 0007  lec.............
+00003520: 0000 0007 0000 0043 0000 0073 a000 0000  .......C...s....
+00003530: 6401 7d01 7400 7c01 8301 7d02 6402 7d03  d.}.t.|...}.d.}.
+00003540: 7c02 7c03 6b02 7d04 7c04 738c 7401 a002  |.|.k.}.|.s.t...
+00003550: 6403 7c04 6601 6404 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00003560: 6405 7403 a004 a100 7600 7346 7401 a005  d.t.....v.sFt...
+00003570: 7400 a101 7250 7401 a006 7400 a101 6e02  t...rPt...t...n.
+00003580: 6405 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
+00003590: a101 7401 a006 7c03 a101 6406 9c04 1600  ..t...|...d.....
+000035a0: 7d05 6407 6408 7c05 6901 1600 7d06 7407  }.d.d.|.i...}.t.
+000035b0: 7401 a008 7c06 a101 8301 8201 6400 0400  t...|.......d...
+000035c0: 7d01 0400 7d02 0400 7d04 7d03 6400 5300  }...}...}.}.d.S.
+000035d0: 2909 4e7a 0866 6f6f 2e70 6c6f 627a 1166  ).Nz.foo.plobz.f
+000035e0: 6f6f 2e70 6c6f 622e 7065 7266 2e79 6d6c  oo.plob.perf.yml
+000035f0: 72a3 0000 0072 a500 0000 7209 0000 0072  r....r....r....r
+00003600: a600 0000 72a7 0000 0072 a800 0000 72a9  ....r....r....r.
+00003610: 0000 0072 aa00 0000 7216 0000 0072 1600  ...r....r....r..
+00003620: 0000 7217 0000 00da 1174 6573 745f 756e  ..r......test_un
+00003630: 6b6e 6f77 6e5f 6669 6c65 dc00 0000 7302  known_file....s.
+00003640: 0000 0000 017a 2247 6574 5065 7266 5061  .....z"GetPerfPa
+00003650: 7468 5465 7374 732e 7465 7374 5f75 6e6b  thTests.test_unk
+00003660: 6e6f 776e 5f66 696c 654e 2906 729d 0000  nown_fileN).r...
+00003670: 0072 9e00 0000 729f 0000 0072 ac00 0000  .r....r....r....
+00003680: 72ad 0000 0072 ae00 0000 7216 0000 0072  r....r....r....r
+00003690: 1600 0000 7216 0000 0072 1700 0000 72a0  ....r....r....r.
+000036a0: 0000 00d5 0000 0073 0600 0000 0801 0803  .......s........
+000036b0: 0803 72a0 0000 0063 0000 0000 0000 0000  ..r....c........
+000036c0: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+000036d0: 732c 0000 0065 005a 0164 005a 0264 0164  s,...e.Z.d.Z.d.d
+000036e0: 0284 005a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
+000036f0: 0684 005a 0564 0764 0884 005a 0664 0953  ...Z.d.d...Z.d.S
+00003700: 0029 0ada 1247 6574 5265 636f 7264 4e61  .)...GetRecordNa
+00003710: 6d65 5465 7374 7363 0100 0000 0000 0000  meTestsc........
+00003720: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
+00003730: 73b4 0000 0064 017d 0164 027d 0274 007c  s....d.}.d.}.t.|
+00003740: 017c 0264 038d 027d 0364 047d 047c 037c  .|.d...}.d.}.|.|
+00003750: 046b 027d 057c 0573 9c74 01a0 0264 057c  .k.}.|.s.t...d.|
+00003760: 0566 0164 067c 037c 0466 02a1 0464 0774  .f.d.|.|.f...d.t
+00003770: 03a0 04a1 0076 0073 4e74 01a0 0574 00a1  .....v.sNt...t..
+00003780: 0172 5874 01a0 0674 00a1 016e 0264 0774  .rXt...t...n.d.t
+00003790: 01a0 067c 01a1 0174 01a0 067c 02a1 0174  ...|...t...|...t
+000037a0: 01a0 067c 03a1 0174 01a0 067c 04a1 0164  ...|...t...|...d
+000037b0: 089c 0516 007d 0664 0964 0a7c 0669 0116  .....}.d.d.|.i..
+000037c0: 007d 0774 0774 01a0 087c 07a1 0183 0182  .}.t.t...|......
+000037d0: 0164 0004 007d 0104 007d 0204 007d 0304  .d...}...}...}..
+000037e0: 007d 057d 0464 0053 0029 0b4e 5a08 466f  .}.}.d.S.).NZ.Fo
+000037f0: 6f54 6573 7473 5a08 7465 7374 5f62 6172  oTestsZ.test_bar
+00003800: 2902 da0a 636c 6173 735f 6e61 6d65 da09  )...class_name..
+00003810: 7465 7374 5f6e 616d 657a 1146 6f6f 5465  test_namez.FooTe
+00003820: 7374 732e 7465 7374 5f62 6172 72a3 0000  sts.test_barr...
+00003830: 0029 017a 4e25 2870 7936 2973 0a7b 2528  .).zN%(py6)s.{%(
+00003840: 7079 3629 7320 3d20 2528 7079 3029 7328  py6)s = %(py0)s(
+00003850: 636c 6173 735f 6e61 6d65 3d25 2870 7932  class_name=%(py2
+00003860: 2973 2c20 7465 7374 5f6e 616d 653d 2528  )s, test_name=%(
+00003870: 7079 3429 7329 0a7d 203d 3d20 2528 7079  py4)s).} == %(py
+00003880: 3929 7372 0a00 0000 a905 7278 0000 0072  9)sr......rx...r
+00003890: 7900 0000 7269 0000 0072 6a00 0000 72a8  y...ri...rj...r.
+000038a0: 0000 00fa 0f61 7373 6572 7420 2528 7079  .....assert %(py
+000038b0: 3131 2973 da04 7079 3131 a909 720a 0000  11)s..py11..r...
+000038c0: 0072 2f00 0000 7230 0000 0072 3200 0000  .r/...r0...r2...
+000038d0: 7233 0000 0072 3400 0000 7231 0000 0072  r3...r4...r1...r
+000038e0: 2c00 0000 7235 0000 00a9 0872 1500 0000  ,...r5.....r....
+000038f0: 727b 0000 0072 7c00 0000 726e 0000 0072  r{...r|...rn...r
+00003900: 9700 0000 726f 0000 0072 ab00 0000 5a0c  ....ro...r....Z.
+00003910: 4070 795f 666f 726d 6174 3132 7216 0000  @py_format12r...
+00003920: 0072 1600 0000 7217 0000 00da 1374 6573  .r....r......tes
+00003930: 745f 636c 6173 735f 616e 645f 7465 7374  t_class_and_test
+00003940: e100 0000 7302 0000 0000 017a 2647 6574  ....s......z&Get
+00003950: 5265 636f 7264 4e61 6d65 5465 7374 732e  RecordNameTests.
+00003960: 7465 7374 5f63 6c61 7373 5f61 6e64 5f74  test_class_and_t
+00003970: 6573 7463 0100 0000 0000 0000 0000 0000  estc............
+00003980: 0700 0000 0700 0000 4300 0000 73a2 0000  ........C...s...
+00003990: 0064 017d 0174 007c 0164 028d 017d 0264  .d.}.t.|.d...}.d
+000039a0: 017d 037c 027c 036b 027d 047c 0473 8e74  .}.|.|.k.}.|.s.t
+000039b0: 01a0 0264 037c 0466 0164 047c 027c 0366  ...d.|.f.d.|.|.f
+000039c0: 02a1 0464 0574 03a0 04a1 0076 0073 4874  ...d.t.....v.sHt
+000039d0: 01a0 0574 00a1 0172 5274 01a0 0674 00a1  ...t...rRt...t..
+000039e0: 016e 0264 0574 01a0 067c 01a1 0174 01a0  .n.d.t...|...t..
+000039f0: 067c 02a1 0174 01a0 067c 03a1 0164 069c  .|...t...|...d..
+00003a00: 0416 007d 0564 0764 087c 0569 0116 007d  ...}.d.d.|.i...}
+00003a10: 0674 0774 01a0 087c 06a1 0183 0182 0164  .t.t...|.......d
+00003a20: 0004 007d 0104 007d 0204 007d 047d 0364  ...}...}...}.}.d
+00003a30: 0053 0029 094e 5a08 7465 7374 5f62 617a  .S.).NZ.test_baz
+00003a40: a901 72b1 0000 0072 a300 0000 a901 7a3a  ..r....r......z:
+00003a50: 2528 7079 3429 730a 7b25 2870 7934 2973  %(py4)s.{%(py4)s
+00003a60: 203d 2025 2870 7930 2973 2874 6573 745f   = %(py0)s(test_
+00003a70: 6e61 6d65 3d25 2870 7932 2973 290a 7d20  name=%(py2)s).} 
+00003a80: 3d3d 2025 2870 7937 2973 720a 0000 0072  == %(py7)sr....r
+00003a90: a600 0000 72a7 0000 0072 a800 0000 72b5  ....r....r....r.
+00003aa0: 0000 0072 aa00 0000 7216 0000 0072 1600  ...r....r....r..
+00003ab0: 0000 7217 0000 00da 0e74 6573 745f 6a75  ..r......test_ju
+00003ac0: 7374 5f74 6573 74e7 0000 0073 0200 0000  st_test....s....
+00003ad0: 0001 7a21 4765 7452 6563 6f72 644e 616d  ..z!GetRecordNam
+00003ae0: 6554 6573 7473 2e74 6573 745f 6a75 7374  eTests.test_just
+00003af0: 5f74 6573 7463 0100 0000 0000 0000 0000  _testc..........
+00003b00: 0000 0700 0000 0700 0000 4300 0000 7342  ..........C...sB
+00003b10: 0100 0064 017d 0174 007c 0164 028d 017d  ...d.}.t.|.d...}
+00003b20: 0264 017d 037c 027c 036b 027d 047c 0473  .d.}.|.|.k.}.|.s
+00003b30: 8e74 01a0 0264 037c 0466 0164 047c 027c  .t...d.|.f.d.|.|
+00003b40: 0366 02a1 0464 0574 03a0 04a1 0076 0073  .f...d.t.....v.s
+00003b50: 4874 01a0 0574 00a1 0172 5274 01a0 0674  Ht...t...rRt...t
+00003b60: 00a1 016e 0264 0574 01a0 067c 01a1 0174  ...n.d.t...|...t
+00003b70: 01a0 067c 02a1 0174 01a0 067c 03a1 0164  ...|...t...|...d
+00003b80: 069c 0416 007d 0564 0764 087c 0569 0116  .....}.d.d.|.i..
+00003b90: 007d 0674 0774 01a0 087c 06a1 0183 0182  .}.t.t...|......
+00003ba0: 0164 0004 007d 0104 007d 0204 007d 047d  .d...}...}...}.}
+00003bb0: 0364 017d 0174 007c 0164 028d 017d 0264  .d.}.t.|.d...}.d
+00003bc0: 097d 037c 027c 036b 027d 047c 0490 0173  .}.|.|.k.}.|...s
+00003bd0: 2e74 01a0 0264 037c 0466 0164 047c 027c  .t...d.|.f.d.|.|
+00003be0: 0366 02a1 0464 0574 03a0 04a1 0076 0073  .f...d.t.....v.s
+00003bf0: e874 01a0 0574 00a1 0172 f274 01a0 0674  .t...t...r.t...t
+00003c00: 00a1 016e 0264 0574 01a0 067c 01a1 0174  ...n.d.t...|...t
+00003c10: 01a0 067c 02a1 0174 01a0 067c 03a1 0164  ...|...t...|...d
+00003c20: 069c 0416 007d 0564 0764 087c 0569 0116  .....}.d.d.|.i..
+00003c30: 007d 0674 0774 01a0 087c 06a1 0183 0182  .}.t.t...|......
+00003c40: 0164 0004 007d 0104 007d 0204 007d 047d  .d...}...}...}.}
+00003c50: 0364 0053 0029 0a4e da08 7465 7374 5f71  .d.S.).N..test_q
+00003c60: 7578 72b8 0000 0072 a300 0000 72b9 0000  uxr....r....r...
+00003c70: 0072 0a00 0000 72a6 0000 0072 a700 0000  .r....r....r....
+00003c80: 72a8 0000 00fa 0a74 6573 745f 7175 782e  r......test_qux.
+00003c90: 3272 b500 0000 72aa 0000 0072 1600 0000  2r....r....r....
+00003ca0: 7216 0000 0072 1700 0000 da13 7465 7374  r....r......test
+00003cb0: 5f6d 756c 7469 706c 655f 6361 6c6c 73ea  _multiple_calls.
+00003cc0: 0000 0073 0400 0000 0001 9e01 7a26 4765  ...s........z&Ge
+00003cd0: 7452 6563 6f72 644e 616d 6554 6573 7473  tRecordNameTests
+00003ce0: 2e74 6573 745f 6d75 6c74 6970 6c65 5f63  .test_multiple_c
+00003cf0: 616c 6c73 6301 0000 0000 0000 0000 0000  allsc...........
+00003d00: 0008 0000 0008 0000 0043 0000 0073 d602  .........C...s..
+00003d10: 0000 6401 7d01 6402 7d02 7400 7c01 7c02  ..d.}.d.}.t.|.|.
+00003d20: 6403 8d02 7d03 6401 7d04 7c03 7c04 6b02  d...}.d.}.|.|.k.
+00003d30: 7d05 7c05 739c 7401 a002 6404 7c05 6601  }.|.s.t...d.|.f.
+00003d40: 6405 7c03 7c04 6602 a104 6406 7403 a004  d.|.|.f...d.t...
+00003d50: a100 7600 734e 7401 a005 7400 a101 7258  ..v.sNt...t...rX
+00003d60: 7401 a006 7400 a101 6e02 6406 7401 a006  t...t...n.d.t...
+00003d70: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
+00003d80: 7c03 a101 7401 a006 7c04 a101 6407 9c05  |...t...|...d...
+00003d90: 1600 7d06 6408 6409 7c06 6901 1600 7d07  ..}.d.d.|.i...}.
+00003da0: 7407 7401 a008 7c07 a101 8301 8201 6400  t.t...|.......d.
+00003db0: 0400 7d01 0400 7d02 0400 7d03 0400 7d05  ..}...}...}...}.
+00003dc0: 7d04 6401 7d01 640a 7d02 7400 7c01 7c02  }.d.}.d.}.t.|.|.
+00003dd0: 6403 8d02 7d03 6401 7d04 7c03 7c04 6b02  d...}.d.}.|.|.k.
+00003de0: 7d05 7c05 9001 7352 7401 a002 6404 7c05  }.|...sRt...d.|.
+00003df0: 6601 6405 7c03 7c04 6602 a104 6406 7403  f.d.|.|.f...d.t.
+00003e00: a004 a100 7600 9001 7304 7401 a005 7400  ....v...s.t...t.
+00003e10: a101 9001 720e 7401 a006 7400 a101 6e02  ....r.t...t...n.
+00003e20: 6406 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
+00003e30: a101 7401 a006 7c03 a101 7401 a006 7c04  ..t...|...t...|.
+00003e40: a101 6407 9c05 1600 7d06 6408 6409 7c06  ..d.....}.d.d.|.
+00003e50: 6901 1600 7d07 7407 7401 a008 7c07 a101  i...}.t.t...|...
+00003e60: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
+00003e70: 7d03 0400 7d05 7d04 6401 7d01 6402 7d02  }...}.}.d.}.d.}.
+00003e80: 7400 7c01 7c02 6403 8d02 7d03 6401 7d04  t.|.|.d...}.d.}.
+00003e90: 7c03 7c04 6b02 7d05 7c05 9002 7308 7401  |.|.k.}.|...s.t.
+00003ea0: a002 6404 7c05 6601 6405 7c03 7c04 6602  ..d.|.f.d.|.|.f.
+00003eb0: a104 6406 7403 a004 a100 7600 9001 73ba  ..d.t.....v...s.
+00003ec0: 7401 a005 7400 a101 9001 72c4 7401 a006  t...t.....r.t...
+00003ed0: 7400 a101 6e02 6406 7401 a006 7c01 a101  t...n.d.t...|...
+00003ee0: 7401 a006 7c02 a101 7401 a006 7c03 a101  t...|...t...|...
+00003ef0: 7401 a006 7c04 a101 6407 9c05 1600 7d06  t...|...d.....}.
+00003f00: 6408 6409 7c06 6901 1600 7d07 7407 7401  d.d.|.i...}.t.t.
+00003f10: a008 7c07 a101 8301 8201 6400 0400 7d01  ..|.......d...}.
+00003f20: 0400 7d02 0400 7d03 0400 7d05 7d04 6401  ..}...}...}.}.d.
+00003f30: 7d01 6402 7d02 7400 7c01 7c02 6403 8d02  }.d.}.t.|.|.d...
+00003f40: 7d03 640b 7d04 7c03 7c04 6b02 7d05 7c05  }.d.}.|.|.k.}.|.
+00003f50: 9002 73be 7401 a002 6404 7c05 6601 6405  ..s.t...d.|.f.d.
+00003f60: 7c03 7c04 6602 a104 6406 7403 a004 a100  |.|.f...d.t.....
+00003f70: 7600 9002 7370 7401 a005 7400 a101 9002  v...spt...t.....
+00003f80: 727a 7401 a006 7400 a101 6e02 6406 7401  rzt...t...n.d.t.
+00003f90: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
+00003fa0: a006 7c03 a101 7401 a006 7c04 a101 6407  ..|...t...|...d.
+00003fb0: 9c05 1600 7d06 6408 6409 7c06 6901 1600  ....}.d.d.|.i...
+00003fc0: 7d07 7407 7401 a008 7c07 a101 8301 8201  }.t.t...|.......
+00003fd0: 6400 0400 7d01 0400 7d02 0400 7d03 0400  d...}...}...}...
+00003fe0: 7d05 7d04 6400 5300 290c 4e72 bb00 0000  }.}.d.S.).Nr....
+00003ff0: 72a1 0000 0029 0272 b100 0000 da09 6669  r....).r......fi
+00004000: 6c65 5f6e 616d 6572 a300 0000 2901 7a4d  le_namer....).zM
+00004010: 2528 7079 3629 730a 7b25 2870 7936 2973  %(py6)s.{%(py6)s
+00004020: 203d 2025 2870 7930 2973 2874 6573 745f   = %(py0)s(test_
+00004030: 6e61 6d65 3d25 2870 7932 2973 2c20 6669  name=%(py2)s, fi
+00004040: 6c65 5f6e 616d 653d 2528 7079 3429 7329  le_name=%(py4)s)
+00004050: 0a7d 203d 3d20 2528 7079 3929 7372 0a00  .} == %(py9)sr..
+00004060: 0000 72b2 0000 0072 b300 0000 72b4 0000  ..r....r....r...
+00004070: 007a 0766 6f6f 322e 7079 72bc 0000 0072  .z.foo2.pyr....r
+00004080: b500 0000 72b6 0000 0072 1600 0000 7216  ....r....r....r.
+00004090: 0000 0072 1700 0000 da28 7465 7374 5f6d  ...r.....(test_m
+000040a0: 756c 7469 706c 655f 6361 6c6c 735f 6672  ultiple_calls_fr
+000040b0: 6f6d 5f64 6966 6665 7265 6e74 5f66 696c  om_different_fil
+000040c0: 6573 ee00 0000 7308 0000 0000 01b0 02b6  es....s.........
+000040d0: 02b6 027a 3b47 6574 5265 636f 7264 4e61  ...z;GetRecordNa
+000040e0: 6d65 5465 7374 732e 7465 7374 5f6d 756c  meTests.test_mul
+000040f0: 7469 706c 655f 6361 6c6c 735f 6672 6f6d  tiple_calls_from
+00004100: 5f64 6966 6665 7265 6e74 5f66 696c 6573  _different_files
+00004110: 4e29 0772 9d00 0000 729e 0000 0072 9f00  N).r....r....r..
+00004120: 0000 72b7 0000 0072 ba00 0000 72bd 0000  ..r....r....r...
+00004130: 0072 bf00 0000 7216 0000 0072 1600 0000  .r....r....r....
+00004140: 7216 0000 0072 1700 0000 72af 0000 00e0  r....r....r.....
+00004150: 0000 0073 0800 0000 0801 0806 0803 0804  ...s............
+00004160: 72af 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00004170: 0000 0000 0000 0200 0000 4000 0000 7324  ..........@...s$
+00004180: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00004190: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+000041a0: 005a 0564 0753 0029 08da 1254 6573 7443  .Z.d.S.)...TestC
+000041b0: 6173 654d 6978 696e 5465 7374 7363 0100  aseMixinTestsc..
+000041c0: 0000 0000 0000 0000 0000 0100 0000 0800  ................
+000041d0: 0000 4300 0000 733a 0000 007c 00a0 00a1  ..C...s:...|....
+000041e0: 008f 1e01 0074 0164 0119 00a0 0264 02a1  .....t.d.....d..
+000041f0: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
+00004200: 1031 0073 2c30 0001 0001 0001 0059 0001  .1.s,0.......Y..
+00004210: 0064 0053 0072 5700 0000 a903 da12 7265  .d.S.rW.......re
+00004220: 636f 7264 5f70 6572 666f 726d 616e 6365  cord_performance
+00004230: 7202 0000 0072 5900 0000 7214 0000 0072  r....rY...r....r
+00004240: 1600 0000 7216 0000 0072 1700 0000 da17  ....r....r......
+00004250: 7465 7374 5f72 6563 6f72 645f 7065 7266  test_record_perf
+00004260: 6f72 6d61 6e63 65f9 0000 0073 0400 0000  ormance....s....
+00004270: 0001 0a01 7a2a 5465 7374 4361 7365 4d69  ....z*TestCaseMi
+00004280: 7869 6e54 6573 7473 2e74 6573 745f 7265  xinTests.test_re
+00004290: 636f 7264 5f70 6572 666f 726d 616e 6365  cord_performance
+000042a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000042b0: 0008 0000 0043 0000 0073 3e00 0000 7c00  .....C...s>...|.
+000042c0: 6a00 6401 6402 8d01 8f1e 0100 7401 6403  j.d.d.......t.d.
+000042d0: 1900 a002 6404 a101 0100 5700 6400 0400  ....d.....W.d...
+000042e0: 0400 8303 0100 6e10 3100 7330 3000 0100  ......n.1.s00...
+000042f0: 0100 0100 5900 0100 6400 5300 2905 4eda  ....Y...d.S.).N.
+00004300: 056f 7468 6572 7265 0000 0072 1100 0000  .otherre...r....
+00004310: 7251 0000 0072 c100 0000 7214 0000 0072  rQ...r....r....r
+00004320: 1600 0000 7216 0000 0072 1700 0000 da23  ....r....r.....#
+00004330: 7465 7374 5f72 6563 6f72 645f 7065 7266  test_record_perf
+00004340: 6f72 6d61 6e63 655f 7265 636f 7264 5f6e  ormance_record_n
+00004350: 616d 65fd 0000 0073 0400 0000 0001 0e01  ame....s........
+00004360: 7a36 5465 7374 4361 7365 4d69 7869 6e54  z6TestCaseMixinT
+00004370: 6573 7473 2e74 6573 745f 7265 636f 7264  ests.test_record
+00004380: 5f70 6572 666f 726d 616e 6365 5f72 6563  _performance_rec
+00004390: 6f72 645f 6e61 6d65 6301 0000 0000 0000  ord_namec.......
+000043a0: 0000 0000 0002 0000 0008 0000 0043 0000  .............C..
+000043b0: 0073 4a00 0000 7400 a001 6401 6402 a102  .sJ...t...d.d...
+000043c0: 7d01 7c00 6a02 7c01 6403 8d01 8f1e 0100  }.|.j.|.d.......
+000043d0: 7403 6404 1900 a004 6405 a101 0100 5700  t.d.....d.....W.
+000043e0: 6400 0400 0400 8303 0100 6e10 3100 733c  d.........n.1.s<
+000043f0: 3000 0100 0100 0100 5900 0100 6400 5300  0.......Y...d.S.
+00004400: 2906 4e7a 032e 7079 7a13 2e66 696c 655f  ).Nz..pyz..file_
+00004410: 6e61 6d65 2e70 6572 662e 796d 6c72 7500  name.perf.ymlru.
+00004420: 0000 7211 0000 0072 5100 0000 2905 da08  ..r....rQ...)...
+00004430: 5f5f 6669 6c65 5f5f da07 7265 706c 6163  __file__..replac
+00004440: 6572 c200 0000 7202 0000 0072 5900 0000  er....r....rY...
+00004450: 2902 7215 0000 005a 0970 6572 665f 6e61  ).r....Z.perf_na
+00004460: 6d65 7216 0000 0072 1600 0000 7217 0000  mer....r....r...
+00004470: 00da 2174 6573 745f 7265 636f 7264 5f70  ..!test_record_p
+00004480: 6572 666f 726d 616e 6365 5f66 696c 655f  erformance_file_
+00004490: 6e61 6d65 0101 0000 7306 0000 0000 010c  name....s.......
+000044a0: 010e 017a 3454 6573 7443 6173 654d 6978  ...z4TestCaseMix
+000044b0: 696e 5465 7374 732e 7465 7374 5f72 6563  inTests.test_rec
+000044c0: 6f72 645f 7065 7266 6f72 6d61 6e63 655f  ord_performance_
+000044d0: 6669 6c65 5f6e 616d 654e 2906 729d 0000  file_nameN).r...
+000044e0: 0072 9e00 0000 729f 0000 0072 c300 0000  .r....r....r....
+000044f0: 72c5 0000 0072 c800 0000 7216 0000 0072  r....r....r....r
+00004500: 1600 0000 7216 0000 0072 1700 0000 72c0  ....r....r....r.
+00004510: 0000 00f8 0000 0073 0600 0000 0801 0804  .......s........
+00004520: 0804 72c0 0000 0029 25da 0862 7569 6c74  ..r....)%..built
+00004530: 696e 7372 3200 0000 da19 5f70 7974 6573  insr2....._pytes
+00004540: 742e 6173 7365 7274 696f 6e2e 7265 7772  t.assertion.rewr
+00004550: 6974 65da 0961 7373 6572 7469 6f6e da07  ite..assertion..
+00004560: 7265 7772 6974 6572 2f00 0000 7277 0000  rewriter/...rw..
+00004570: 0072 2a00 0000 da11 646a 616e 676f 2e63  .r*.....django.c
+00004580: 6f72 652e 6361 6368 6572 0200 0000 da10  ore.cacher......
+00004590: 646a 616e 676f 2e64 622e 6d6f 6465 6c73  django.db.models
+000045a0: 7203 0000 00da 1a64 6a61 6e67 6f2e 6462  r......django.db
+000045b0: 2e6d 6f64 656c 732e 6675 6e63 7469 6f6e  .models.function
+000045c0: 7372 0400 0000 da0b 646a 616e 676f 2e74  sr......django.t
+000045d0: 6573 7472 0500 0000 7206 0000 0072 0700  estr....r....r..
+000045e0: 0000 5a0f 646a 616e 676f 5f70 6572 665f  ..Z.django_perf_
+000045f0: 7265 6372 0800 0000 7209 0000 0072 0a00  recr....r....r..
+00004600: 0000 720b 0000 005a 1474 6573 7473 2e74  ..r....Z.tests.t
+00004610: 6573 7461 7070 2e6d 6f64 656c 7372 0c00  estapp.modelsr..
+00004620: 0000 5a0b 7465 7374 732e 7574 696c 7372  ..Z.tests.utilsr
+00004630: 0d00 0000 720e 0000 0072 0f00 0000 7276  ....r....r....rv
+00004640: 0000 00da 0764 6972 6e61 6d65 72c6 0000  .....dirnamer...
+00004650: 0072 8800 0000 7210 0000 0072 a000 0000  .r....r....r....
+00004660: 72af 0000 0072 c000 0000 7216 0000 0072  r....r....r....r
+00004670: 1600 0000 7216 0000 0072 1700 0000 da08  ....r....r......
+00004680: 3c6d 6f64 756c 653e 0100 0000 731c 0000  <module>....s...
+00004690: 0022 0208 010c 010c 010c 0114 0218 010c  ."..............
+000046a0: 0114 020c 0310 7f00 4610 0b10 18         ........F....
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_cache.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_cache.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.4.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,614 +1,549 @@
-00000000: 610d 0d0a 4613 445f 6e0c 0000 e300 0000  a...F.D_n.......
-00000010: 0000 0000 0000 0000 0000 0000 0008 0000  ................
-00000020: 0040 0000 0073 b200 0000 6400 6401 6c00  .@...s....d.d.l.
-00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
-00000040: 5a05 0100 6400 6401 6c06 5a06 6400 6402  Z...d.d.l.Z.d.d.
-00000050: 6c07 6d08 5a08 0100 6400 6403 6c09 6d0a  l.m.Z...d.d.l.m.
-00000060: 5a0a 6d0b 5a0b 0100 6400 6404 6c0c 6d0d  Z.m.Z...d.d.l.m.
-00000070: 5a0d 6d0e 5a0e 6d0f 5a0f 0100 7a10 6400  Z.m.Z.m.Z...z.d.
-00000080: 6405 6c10 6d11 5a11 0100 5700 6e1a 0400  d.l.m.Z...W.n...
-00000090: 6512 797c 0100 0100 0100 6400 6401 6c11  e.y|......d.d.l.
-000000a0: 5a11 5900 6e02 3000 4700 6406 6407 8400  Z.Y.n.0.G.d.d...
-000000b0: 6407 650a 8303 5a13 4700 6408 6409 8400  d.e...Z.G.d.d...
-000000c0: 6409 650b 8303 5a14 4700 640a 640b 8400  d.e...Z.G.d.d...
-000000d0: 640b 650b 8303 5a15 6401 5300 290c e900  d.e...Z.d.S.)...
-000000e0: 0000 004e 2901 da06 6361 6368 6573 2902  ...N)...caches).
-000000f0: da0e 5369 6d70 6c65 5465 7374 4361 7365  ..SimpleTestCase
-00000100: da08 5465 7374 4361 7365 2903 da10 416c  ..TestCase)...Al
-00000110: 6c43 6163 6865 5265 636f 7264 6572 da07  lCacheRecorder..
-00000120: 4361 6368 654f 70da 0d43 6163 6865 5265  CacheOp..CacheRe
-00000130: 636f 7264 6572 2901 da04 6d6f 636b 6300  corder)...mockc.
-00000140: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00000150: 0000 0040 0000 0073 6c00 0000 6500 5a01  ...@...sl...e.Z.
-00000160: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
-00000170: 8400 5a04 6405 6406 8400 5a05 6407 6408  ..Z.d.d...Z.d.d.
-00000180: 8400 5a06 6409 640a 8400 5a07 640b 640c  ..Z.d.d...Z.d.d.
-00000190: 8400 5a08 640d 640e 8400 5a09 640f 6410  ..Z.d.d...Z.d.d.
-000001a0: 8400 5a0a 6411 6412 8400 5a0b 6413 6414  ..Z.d.d...Z.d.d.
-000001b0: 8400 5a0c 6415 6416 8400 5a0d 6417 6418  ..Z.d.d...Z.d.d.
-000001c0: 8400 5a0e 6419 5300 291a da0c 4361 6368  ..Z.d.S.)...Cach
-000001d0: 654f 7054 6573 7473 6301 0000 0000 0000  eOpTestsc.......
-000001e0: 0000 0000 0008 0000 0008 0000 0043 0000  .............C..
-000001f0: 0073 b200 0000 7400 6a01 7d01 6401 7d02  .s....t.j.}.d.}.
-00000200: 7c01 7c02 8301 7d03 6402 7d04 7c03 7c04  |.|...}.d.}.|.|.
-00000210: 6b02 7d05 7c05 739a 7402 a003 6403 7c05  k.}.|.s.t...d.|.
-00000220: 6601 6404 7c03 7c04 6602 a104 6405 7404  f.d.|.|.f...d.t.
-00000230: a005 a100 7600 734c 7402 a006 7400 a101  ....v.sLt...t...
-00000240: 7256 7402 a007 7400 a101 6e02 6405 7402  rVt...t...n.d.t.
-00000250: a007 7c01 a101 7402 a007 7c02 a101 7402  ..|...t...|...t.
-00000260: a007 7c03 a101 7402 a007 7c04 a101 6406  ..|...t...|...d.
-00000270: 9c05 1600 7d06 6407 6408 7c06 6901 1600  ....}.d.d.|.i...
-00000280: 7d07 7408 7402 a009 7c07 a101 8301 8201  }.t.t...|.......
-00000290: 6400 0400 7d01 0400 7d02 0400 7d03 0400  d...}...}...}...
-000002a0: 7d05 7d04 6400 5300 2909 4e5a 0466 6f6f  }.}.d.S.).NZ.foo
-000002b0: 317a 0466 6f6f 23a9 01fa 023d 3da9 017a  1z.foo#....==..z
-000002c0: 4f25 2870 7936 2973 0a7b 2528 7079 3629  O%(py6)s.{%(py6)
-000002d0: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
-000002e0: 7932 2973 203d 2025 2870 7930 2973 2e63  y2)s = %(py0)s.c
-000002f0: 6c65 616e 5f6b 6579 0a7d 2825 2870 7934  lean_key.}(%(py4
-00000300: 2973 290a 7d20 3d3d 2025 2870 7939 2973  )s).} == %(py9)s
-00000310: 7206 0000 00a9 05da 0370 7930 da03 7079  r........py0..py
-00000320: 32da 0370 7934 da03 7079 36da 0370 7939  2..py4..py6..py9
-00000330: fa0f 6173 7365 7274 2025 2870 7931 3129  ..assert %(py11)
-00000340: 73da 0470 7931 31a9 0a72 0600 0000 da09  s..py11..r......
-00000350: 636c 6561 6e5f 6b65 79da 0a40 7079 7465  clean_key..@pyte
-00000360: 7374 5f61 72da 115f 6361 6c6c 5f72 6570  st_ar.._call_rep
-00000370: 7263 6f6d 7061 7265 da0c 4070 795f 6275  rcompare..@py_bu
-00000380: 696c 7469 6e73 da06 6c6f 6361 6c73 da18  iltins..locals..
-00000390: 5f73 686f 756c 645f 7265 7072 5f67 6c6f  _should_repr_glo
-000003a0: 6261 6c5f 6e61 6d65 da09 5f73 6166 6572  bal_name.._safer
-000003b0: 6570 72da 0e41 7373 6572 7469 6f6e 4572  epr..AssertionEr
-000003c0: 726f 72da 135f 666f 726d 6174 5f65 7870  ror.._format_exp
-000003d0: 6c61 6e61 7469 6f6e a908 da04 7365 6c66  lanation....self
-000003e0: da0b 4070 795f 6173 7365 7274 31da 0b40  ..@py_assert1..@
-000003f0: 7079 5f61 7373 6572 7433 da0b 4070 795f  py_assert3..@py_
-00000400: 6173 7365 7274 35da 0b40 7079 5f61 7373  assert5..@py_ass
-00000410: 6572 7438 da0b 4070 795f 6173 7365 7274  ert8..@py_assert
-00000420: 37da 0c40 7079 5f66 6f72 6d61 7431 30da  7..@py_format10.
-00000430: 0c40 7079 5f66 6f72 6d61 7431 32a9 0072  .@py_format12..r
-00000440: 2800 0000 fa44 2f55 7365 7273 2f63 6861  (....D/Users/cha
-00000450: 696e 7a2f 446f 6375 6d65 6e74 732f 5072  inz/Documents/Pr
-00000460: 6f6a 6563 7473 2f64 6a61 6e67 6f2d 7065  ojects/django-pe
-00000470: 7266 2d72 6563 2f74 6573 7473 2f74 6573  rf-rec/tests/tes
-00000480: 745f 6361 6368 652e 7079 da16 7465 7374  t_cache.py..test
-00000490: 5f63 6c65 616e 5f6b 6579 5f69 6e74 6567  _clean_key_integ
-000004a0: 6572 0e00 0000 7302 0000 0000 017a 2343  er....s......z#C
-000004b0: 6163 6865 4f70 5465 7374 732e 7465 7374  acheOpTests.test
-000004c0: 5f63 6c65 616e 5f6b 6579 5f69 6e74 6567  _clean_key_integ
-000004d0: 6572 6301 0000 0000 0000 0000 0000 0008  erc.............
-000004e0: 0000 0008 0000 0043 0000 0073 b200 0000  .......C...s....
-000004f0: 7400 6a01 7d01 6401 7d02 7c01 7c02 8301  t.j.}.d.}.|.|...
-00000500: 7d03 6402 7d04 7c03 7c04 6b02 7d05 7c05  }.d.}.|.|.k.}.|.
-00000510: 739a 7402 a003 6403 7c05 6601 6404 7c03  s.t...d.|.f.d.|.
-00000520: 7c04 6602 a104 6405 7404 a005 a100 7600  |.f...d.t.....v.
-00000530: 734c 7402 a006 7400 a101 7256 7402 a007  sLt...t...rVt...
-00000540: 7400 a101 6e02 6405 7402 a007 7c01 a101  t...n.d.t...|...
-00000550: 7402 a007 7c02 a101 7402 a007 7c03 a101  t...|...t...|...
-00000560: 7402 a007 7c04 a101 6406 9c05 1600 7d06  t...|...d.....}.
-00000570: 6407 6408 7c06 6901 1600 7d07 7408 7402  d.d.|.i...}.t.t.
-00000580: a009 7c07 a101 8301 8201 6400 0400 7d01  ..|.......d...}.
-00000590: 0400 7d02 0400 7d03 0400 7d05 7d04 6400  ..}...}...}.}.d.
-000005a0: 5300 2909 4e7a 2462 6466 6339 3938 362d  S.).Nz$bdfc9986-
-000005b0: 6434 3631 2d34 6135 652d 6266 3938 2d38  d461-4a5e-bf98-8
-000005c0: 3638 3839 3933 6162 6366 62fa 0123 720a  688993abcfb..#r.
-000005d0: 0000 0072 0c00 0000 7206 0000 0072 0d00  ...r....r....r..
-000005e0: 0000 7213 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000005f0: 0072 1f00 0000 7228 0000 0072 2800 0000  .r....r(...r(...
-00000600: 7229 0000 00da 1374 6573 745f 636c 6561  r).....test_clea
-00000610: 6e5f 6b65 795f 7575 6964 1100 0000 7302  n_key_uuid....s.
-00000620: 0000 0000 017a 2043 6163 6865 4f70 5465  .....z CacheOpTe
-00000630: 7374 732e 7465 7374 5f63 6c65 616e 5f6b  sts.test_clean_k
-00000640: 6579 5f75 7569 6463 0100 0000 0000 0000  ey_uuidc........
-00000650: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
-00000660: 73b2 0000 0074 006a 017d 0164 017d 027c  s....t.j.}.d.}.|
-00000670: 017c 0283 017d 0364 027d 047c 037c 046b  .|...}.d.}.|.|.k
-00000680: 027d 057c 0573 9a74 02a0 0364 037c 0566  .}.|.s.t...d.|.f
-00000690: 0164 047c 037c 0466 02a1 0464 0574 04a0  .d.|.|.f...d.t..
-000006a0: 05a1 0076 0073 4c74 02a0 0674 00a1 0172  ...v.sLt...t...r
-000006b0: 5674 02a0 0774 00a1 016e 0264 0574 02a0  Vt...t...n.d.t..
-000006c0: 077c 01a1 0174 02a0 077c 02a1 0174 02a0  .|...t...|...t..
-000006d0: 077c 03a1 0174 02a0 077c 04a1 0164 069c  .|...t...|...d..
-000006e0: 0516 007d 0664 0764 087c 0669 0116 007d  ...}.d.d.|.i...}
-000006f0: 0774 0874 02a0 097c 07a1 0183 0182 0164  .t.t...|.......d
-00000700: 0004 007d 0104 007d 0204 007d 0304 007d  ...}...}...}...}
-00000710: 057d 0464 0053 0029 094e 5a20 6162 6331  .}.d.S.).NZ abc1
-00000720: 3233 6162 6331 3233 6162 6331 3233 6162  23abc123abc123ab
-00000730: 6331 3233 6162 6331 3233 3435 722b 0000  c123abc12345r+..
-00000740: 0072 0a00 0000 720c 0000 0072 0600 0000  .r....r....r....
-00000750: 720d 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000760: 1500 0000 721f 0000 0072 2800 0000 7228  ....r....r(...r(
-00000770: 0000 0072 2900 0000 da1a 7465 7374 5f63  ...r).....test_c
-00000780: 6c65 616e 5f6b 6579 5f72 616e 646f 6d5f  lean_key_random_
-00000790: 6861 7368 1400 0000 7302 0000 0000 017a  hash....s......z
-000007a0: 2743 6163 6865 4f70 5465 7374 732e 7465  'CacheOpTests.te
-000007b0: 7374 5f63 6c65 616e 5f6b 6579 5f72 616e  st_clean_key_ran
-000007c0: 646f 6d5f 6861 7368 6301 0000 0000 0000  dom_hashc.......
-000007d0: 0000 0000 0008 0000 0008 0000 0043 0000  .............C..
-000007e0: 0073 c800 0000 6401 7d01 7400 6a01 7d02  .s....d.}.t.j.}.
-000007f0: 7c02 7c01 8301 7d03 6402 7d04 7c03 7c04  |.|...}.d.}.|.|.
-00000800: 6b02 7d05 7c05 73b4 7402 a003 6403 7c05  k.}.|.s.t...d.|.
-00000810: 6601 6404 7c03 7c04 6602 a104 6405 7404  f.d.|.|.f...d.t.
-00000820: a005 a100 7600 734c 7402 a006 7400 a101  ....v.sLt...t...
-00000830: 7256 7402 a007 7400 a101 6e02 6405 7402  rVt...t...n.d.t.
-00000840: a007 7c02 a101 6406 7404 a005 a100 7600  ..|...d.t.....v.
-00000850: 7376 7402 a006 7c01 a101 7280 7402 a007  svt...|...r.t...
-00000860: 7c01 a101 6e02 6406 7402 a007 7c03 a101  |...n.d.t...|...
-00000870: 7402 a007 7c04 a101 6407 9c05 1600 7d06  t...|...d.....}.
-00000880: 6408 6409 7c06 6901 1600 7d07 7408 7402  d.d.|.i...}.t.t.
-00000890: a009 7c07 a101 8301 8201 6400 0400 7d02  ..|.......d...}.
-000008a0: 0400 7d03 0400 7d05 7d04 6400 5300 290a  ..}...}.}.d.S.).
-000008b0: 4e7a 3d64 6a61 6e67 6f2e 636f 6e74 7269  Nz=django.contri
-000008c0: 622e 7365 7373 696f 6e73 2e63 6163 6865  b.sessions.cache
-000008d0: 6162 6364 6566 6768 696a 6b6c 6d6e 6f70  abcdefghijklmnop
-000008e0: 7172 7374 7576 7778 797a 3031 3233 3435  qrstuvwxyz012345
-000008f0: 7a1e 646a 616e 676f 2e63 6f6e 7472 6962  z.django.contrib
-00000900: 2e73 6573 7369 6f6e 732e 6361 6368 6523  .sessions.cache#
-00000910: 720a 0000 00a9 017a 4f25 2870 7935 2973  r......zO%(py5)s
-00000920: 0a7b 2528 7079 3529 7320 3d20 2528 7079  .{%(py5)s = %(py
-00000930: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
-00000940: 2870 7930 2973 2e63 6c65 616e 5f6b 6579  (py0)s.clean_key
-00000950: 0a7d 2825 2870 7933 2973 290a 7d20 3d3d  .}(%(py3)s).} ==
-00000960: 2025 2870 7938 2973 7206 0000 00da 036b   %(py8)sr......k
-00000970: 6579 a905 720e 0000 0072 0f00 0000 da03  ey..r....r......
-00000980: 7079 33da 0370 7935 da03 7079 38fa 0f61  py3..py5..py8..a
-00000990: 7373 6572 7420 2528 7079 3130 2973 da04  ssert %(py10)s..
-000009a0: 7079 3130 7215 0000 00a9 0872 2000 0000  py10r......r ...
-000009b0: 722f 0000 0072 2100 0000 da0b 4070 795f  r/...r!.....@py_
-000009c0: 6173 7365 7274 3472 2500 0000 da0b 4070  assert4r%.....@p
-000009d0: 795f 6173 7365 7274 36da 0b40 7079 5f66  y_assert6..@py_f
-000009e0: 6f72 6d61 7439 da0c 4070 795f 666f 726d  ormat9..@py_form
-000009f0: 6174 3131 7228 0000 0072 2800 0000 7229  at11r(...r(...r)
-00000a00: 0000 00da 2874 6573 745f 636c 6561 6e5f  ....(test_clean_
-00000a10: 6b65 795f 7365 7373 696f 6e5f 6b65 795f  key_session_key_
-00000a20: 6361 6368 655f 6261 636b 656e 6417 0000  cache_backend...
-00000a30: 0073 0400 0000 0001 0401 7a35 4361 6368  .s........z5Cach
-00000a40: 654f 7054 6573 7473 2e74 6573 745f 636c  eOpTests.test_cl
-00000a50: 6561 6e5f 6b65 795f 7365 7373 696f 6e5f  ean_key_session_
-00000a60: 6b65 795f 6361 6368 655f 6261 636b 656e  key_cache_backen
-00000a70: 6463 0100 0000 0000 0000 0000 0000 0800  dc..............
-00000a80: 0000 0800 0000 4300 0000 73c8 0000 0064  ......C...s....d
-00000a90: 017d 0174 006a 017d 027c 027c 0183 017d  .}.t.j.}.|.|...}
-00000aa0: 0364 027d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
-00000ab0: b474 02a0 0364 037c 0566 0164 047c 037c  .t...d.|.f.d.|.|
-00000ac0: 0466 02a1 0464 0574 04a0 05a1 0076 0073  .f...d.t.....v.s
-00000ad0: 4c74 02a0 0674 00a1 0172 5674 02a0 0774  Lt...t...rVt...t
-00000ae0: 00a1 016e 0264 0574 02a0 077c 02a1 0164  ...n.d.t...|...d
-00000af0: 0674 04a0 05a1 0076 0073 7674 02a0 067c  .t.....v.svt...|
-00000b00: 01a1 0172 8074 02a0 077c 01a1 016e 0264  ...r.t...|...n.d
-00000b10: 0674 02a0 077c 03a1 0174 02a0 077c 04a1  .t...|...t...|..
-00000b20: 0164 079c 0516 007d 0664 0864 097c 0669  .d.....}.d.d.|.i
-00000b30: 0116 007d 0774 0874 02a0 097c 07a1 0183  ...}.t.t...|....
-00000b40: 0182 0164 0004 007d 0204 007d 0304 007d  ...d...}...}...}
-00000b50: 057d 0464 0053 0029 0a4e 7a41 646a 616e  .}.d.S.).NzAdjan
-00000b60: 676f 2e63 6f6e 7472 6962 2e73 6573 7369  go.contrib.sessi
-00000b70: 6f6e 732e 6361 6368 6564 5f64 6261 6263  ons.cached_dbabc
-00000b80: 6465 6667 6869 6a6b 6c6d 6e6f 7071 7273  defghijklmnopqrs
-00000b90: 7475 7677 7879 7a30 3132 3334 357a 2264  tuvwxyz012345z"d
-00000ba0: 6a61 6e67 6f2e 636f 6e74 7269 622e 7365  jango.contrib.se
-00000bb0: 7373 696f 6e73 2e63 6163 6865 645f 6462  ssions.cached_db
-00000bc0: 2372 0a00 0000 722e 0000 0072 0600 0000  #r....r....r....
-00000bd0: 722f 0000 0072 3000 0000 7234 0000 0072  r/...r0...r4...r
-00000be0: 3500 0000 7215 0000 0072 3600 0000 7228  5...r....r6...r(
-00000bf0: 0000 0072 2800 0000 7229 0000 00da 2c74  ...r(...r)....,t
-00000c00: 6573 745f 636c 6561 6e5f 6b65 795f 7365  est_clean_key_se
-00000c10: 7373 696f 6e5f 6b65 795f 6361 6368 6564  ssion_key_cached
-00000c20: 5f64 625f 6261 636b 656e 641b 0000 0073  _db_backend....s
-00000c30: 0400 0000 0001 0401 7a39 4361 6368 654f  ........z9CacheO
-00000c40: 7054 6573 7473 2e74 6573 745f 636c 6561  pTests.test_clea
-00000c50: 6e5f 6b65 795f 7365 7373 696f 6e5f 6b65  n_key_session_ke
-00000c60: 795f 6361 6368 6564 5f64 625f 6261 636b  y_cached_db_back
-00000c70: 656e 6463 0100 0000 0000 0000 0000 0000  endc............
-00000c80: 0700 0000 0700 0000 4300 0000 73b6 0100  ........C...s...
-00000c90: 0074 0064 0164 0264 0383 037d 017c 016a  .t.d.d.d...}.|.j
-00000ca0: 017d 0264 017d 037c 027c 036b 027d 047c  .}.d.}.|.|.k.}.|
-00000cb0: 0473 8a74 02a0 0364 047c 0466 0164 057c  .s.t...d.|.f.d.|
-00000cc0: 027c 0366 02a1 0464 0674 04a0 05a1 0076  .|.f...d.t.....v
-00000cd0: 0073 4c74 02a0 067c 01a1 0172 5674 02a0  .sLt...|...rVt..
-00000ce0: 077c 01a1 016e 0264 0674 02a0 077c 02a1  .|...n.d.t...|..
-00000cf0: 0174 02a0 077c 03a1 0164 079c 0316 007d  .t...|...d.....}
-00000d00: 0564 0864 097c 0569 0116 007d 0674 0874  .d.d.|.i...}.t.t
-00000d10: 02a0 097c 06a1 0183 0182 0164 0004 007d  ...|.......d...}
-00000d20: 0204 007d 047d 037c 016a 0a7d 0264 027d  ...}.}.|.j.}.d.}
-00000d30: 037c 027c 036b 027d 047c 0490 0173 1674  .|.|.k.}.|...s.t
-00000d40: 02a0 0364 047c 0466 0164 0a7c 027c 0366  ...d.|.f.d.|.|.f
-00000d50: 02a1 0464 0674 04a0 05a1 0076 0073 d874  ...d.t.....v.s.t
-00000d60: 02a0 067c 01a1 0172 e274 02a0 077c 01a1  ...|...r.t...|..
-00000d70: 016e 0264 0674 02a0 077c 02a1 0174 02a0  .n.d.t...|...t..
-00000d80: 077c 03a1 0164 079c 0316 007d 0564 0864  .|...d.....}.d.d
-00000d90: 097c 0569 0116 007d 0674 0874 02a0 097c  .|.i...}.t.t...|
-00000da0: 06a1 0183 0182 0164 0004 007d 0204 007d  .......d...}...}
-00000db0: 047d 037c 016a 0b7d 0264 037d 037c 027c  .}.|.j.}.d.}.|.|
-00000dc0: 036b 027d 047c 0490 0173 a674 02a0 0364  .k.}.|...s.t...d
-00000dd0: 047c 0466 0164 0b7c 027c 0366 02a1 0464  .|.f.d.|.|.f...d
-00000de0: 0674 04a0 05a1 0076 0090 0173 6874 02a0  .t.....v...sht..
-00000df0: 067c 01a1 0190 0172 7274 02a0 077c 01a1  .|.....rrt...|..
-00000e00: 016e 0264 0674 02a0 077c 02a1 0174 02a0  .n.d.t...|...t..
-00000e10: 077c 03a1 0164 079c 0316 007d 0564 0864  .|...d.....}.d.d
-00000e20: 097c 0569 0116 007d 0674 0874 02a0 097c  .|.i...}.t.t...|
-00000e30: 06a1 0183 0182 0164 0004 007d 0204 007d  .......d...}...}
-00000e40: 047d 0364 0053 0029 0c4e da07 6465 6661  .}.d.S.).N..defa
-00000e50: 756c 74da 0366 6f6f da03 6261 7272 0a00  ult..foo..barr..
-00000e60: 0000 a901 7a2d 2528 7079 3229 730a 7b25  ....z-%(py2)s.{%
-00000e70: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
-00000e80: 2e61 6c69 6173 0a7d 203d 3d20 2528 7079  .alias.} == %(py
-00000e90: 3529 73da 026f 70a9 0372 0e00 0000 720f  5)s..op..r....r.
-00000ea0: 0000 0072 3200 0000 fa0e 6173 7365 7274  ...r2.....assert
-00000eb0: 2025 2870 7937 2973 da03 7079 37a9 017a   %(py7)s..py7..z
-00000ec0: 3125 2870 7932 2973 0a7b 2528 7079 3229  1%(py2)s.{%(py2)
-00000ed0: 7320 3d20 2528 7079 3029 732e 6f70 6572  s = %(py0)s.oper
-00000ee0: 6174 696f 6e0a 7d20 3d3d 2025 2870 7935  ation.} == %(py5
-00000ef0: 2973 a901 7a2d 2528 7079 3229 730a 7b25  )s..z-%(py2)s.{%
-00000f00: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
-00000f10: 2e71 7565 7279 0a7d 203d 3d20 2528 7079  .query.} == %(py
-00000f20: 3529 73a9 0c72 0600 0000 da05 616c 6961  5)s..r......alia
-00000f30: 7372 1700 0000 7218 0000 0072 1900 0000  sr....r....r....
-00000f40: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
-00000f50: 1d00 0000 721e 0000 00da 096f 7065 7261  ....r......opera
-00000f60: 7469 6f6e da05 7175 6572 79a9 0772 2000  tion..query..r .
-00000f70: 0000 7241 0000 0072 2100 0000 7237 0000  ..rA...r!...r7..
-00000f80: 0072 2200 0000 da0b 4070 795f 666f 726d  .r".....@py_form
-00000f90: 6174 36da 0b40 7079 5f66 6f72 6d61 7438  at6..@py_format8
-00000fa0: 7228 0000 0072 2800 0000 7229 0000 00da  r(...r(...r)....
-00000fb0: 0874 6573 745f 6b65 791f 0000 0073 0800  .test_key....s..
-00000fc0: 0000 0001 0c01 8a01 8c01 7a15 4361 6368  ..........z.Cach
-00000fd0: 654f 7054 6573 7473 2e74 6573 745f 6b65  eOpTests.test_ke
-00000fe0: 7963 0100 0000 0000 0000 0000 0000 0700  yc..............
-00000ff0: 0000 0700 0000 4300 0000 73be 0100 0074  ......C...s....t
-00001000: 0064 0164 0264 0364 0467 0283 037d 017c  .d.d.d.d.g...}.|
-00001010: 016a 017d 0264 017d 037c 027c 036b 027d  .j.}.d.}.|.|.k.}
-00001020: 047c 0473 8e74 02a0 0364 057c 0466 0164  .|.s.t...d.|.f.d
-00001030: 067c 027c 0366 02a1 0464 0774 04a0 05a1  .|.|.f...d.t....
-00001040: 0076 0073 5074 02a0 067c 01a1 0172 5a74  .v.sPt...|...rZt
-00001050: 02a0 077c 01a1 016e 0264 0774 02a0 077c  ...|...n.d.t...|
-00001060: 02a1 0174 02a0 077c 03a1 0164 089c 0316  ...t...|...d....
-00001070: 007d 0564 0964 0a7c 0569 0116 007d 0674  .}.d.d.|.i...}.t
-00001080: 0874 02a0 097c 06a1 0183 0182 0164 0004  .t...|.......d..
-00001090: 007d 0204 007d 047d 037c 016a 0a7d 0264  .}...}.}.|.j.}.d
-000010a0: 027d 037c 027c 036b 027d 047c 0490 0173  .}.|.|.k.}.|...s
-000010b0: 1a74 02a0 0364 057c 0466 0164 0b7c 027c  .t...d.|.f.d.|.|
-000010c0: 0366 02a1 0464 0774 04a0 05a1 0076 0073  .f...d.t.....v.s
-000010d0: dc74 02a0 067c 01a1 0172 e674 02a0 077c  .t...|...r.t...|
-000010e0: 01a1 016e 0264 0774 02a0 077c 02a1 0174  ...n.d.t...|...t
-000010f0: 02a0 077c 03a1 0164 089c 0316 007d 0564  ...|...d.....}.d
-00001100: 0964 0a7c 0569 0116 007d 0674 0874 02a0  .d.|.i...}.t.t..
-00001110: 097c 06a1 0183 0182 0164 0004 007d 0204  .|.......d...}..
-00001120: 007d 047d 037c 016a 0b7d 0264 0364 0467  .}.}.|.j.}.d.d.g
-00001130: 027d 037c 027c 036b 027d 047c 0490 0173  .}.|.|.k.}.|...s
-00001140: ae74 02a0 0364 057c 0466 0164 0c7c 027c  .t...d.|.f.d.|.|
-00001150: 0366 02a1 0464 0774 04a0 05a1 0076 0090  .f...d.t.....v..
-00001160: 0173 7074 02a0 067c 01a1 0190 0172 7a74  .spt...|.....rzt
-00001170: 02a0 077c 01a1 016e 0264 0774 02a0 077c  ...|...n.d.t...|
-00001180: 02a1 0174 02a0 077c 03a1 0164 089c 0316  ...t...|...d....
-00001190: 007d 0564 0964 0a7c 0569 0116 007d 0674  .}.d.d.|.i...}.t
-000011a0: 0874 02a0 097c 06a1 0183 0182 0164 0004  .t...|.......d..
-000011b0: 007d 0204 007d 047d 0364 0053 0029 0d4e  .}...}.}.d.S.).N
-000011c0: 723d 0000 0072 3e00 0000 723f 0000 00da  r=...r>...r?....
-000011d0: 0362 617a 720a 0000 0072 4000 0000 7241  .bazr....r@...rA
-000011e0: 0000 0072 4200 0000 7243 0000 0072 4400  ...rB...rC...rD.
-000011f0: 0000 7245 0000 0072 4600 0000 7247 0000  ..rE...rF...rG..
-00001200: 0072 4b00 0000 7228 0000 0072 2800 0000  .rK...r(...r(...
-00001210: 7229 0000 00da 0974 6573 745f 6b65 7973  r).....test_keys
-00001220: 2500 0000 7308 0000 0000 0110 018a 018c  %...s...........
-00001230: 017a 1643 6163 6865 4f70 5465 7374 732e  .z.CacheOpTests.
-00001240: 7465 7374 5f6b 6579 7363 0100 0000 0000  test_keysc......
-00001250: 0000 0000 0000 0100 0000 0800 0000 4300  ..............C.
-00001260: 0000 733c 0000 0074 00a0 0174 02a1 018f  ..s<...t...t....
-00001270: 1e01 0074 0364 0164 0274 0483 0083 0301  ...t.d.d.t......
-00001280: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00001290: 0073 2e30 0001 0001 0001 0059 0001 0064  .s.0.......Y...d
-000012a0: 0053 0029 034e da01 7872 3e00 0000 2905  .S.).N..xr>...).
-000012b0: da06 7079 7465 7374 da06 7261 6973 6573  ..pytest..raises
-000012c0: da0a 5661 6c75 6545 7272 6f72 7206 0000  ..ValueErrorr...
-000012d0: 00da 066f 626a 6563 7429 0172 2000 0000  ...object).r ...
-000012e0: 7228 0000 0072 2800 0000 7229 0000 00da  r(...r(...r)....
-000012f0: 0c74 6573 745f 696e 7661 6c69 642b 0000  .test_invalid+..
-00001300: 0073 0400 0000 0001 0c01 7a19 4361 6368  .s........z.Cach
-00001310: 654f 7054 6573 7473 2e74 6573 745f 696e  eOpTests.test_in
-00001320: 7661 6c69 6463 0100 0000 0000 0000 0000  validc..........
-00001330: 0000 0c00 0000 0d00 0000 4300 0000 731e  ..........C...s.
-00001340: 0100 0064 017d 0164 027d 0264 037d 0374  ...d.}.d.}.d.}.t
-00001350: 007c 017c 027c 0383 037d 0464 017d 0564  .|.|.|...}.d.}.d
-00001360: 027d 0664 037d 0774 007c 057c 067c 0783  .}.d.}.t.|.|.|..
-00001370: 037d 087c 047c 086b 027d 097c 0973 f674  .}.|.|.k.}.|.s.t
-00001380: 01a0 0264 047c 0966 0164 057c 047c 0866  ...d.|.f.d.|.|.f
-00001390: 02a1 0464 0674 03a0 04a1 0076 0073 6674  ...d.t.....v.sft
-000013a0: 01a0 0574 00a1 0172 7074 01a0 0674 00a1  ...t...rpt...t..
-000013b0: 016e 0264 0674 01a0 067c 01a1 0174 01a0  .n.d.t...|...t..
-000013c0: 067c 02a1 0174 01a0 067c 03a1 0174 01a0  .|...t...|...t..
-000013d0: 067c 04a1 0164 0674 03a0 04a1 0076 0073  .|...d.t.....v.s
-000013e0: a874 01a0 0574 00a1 0172 b274 01a0 0674  .t...t...r.t...t
-000013f0: 00a1 016e 0264 0674 01a0 067c 05a1 0174  ...n.d.t...|...t
-00001400: 01a0 067c 06a1 0174 01a0 067c 07a1 0174  ...|...t...|...t
-00001410: 01a0 067c 08a1 0164 079c 0a16 007d 0a64  ...|...d.....}.d
-00001420: 0864 097c 0a69 0116 007d 0b74 0774 01a0  .d.|.i...}.t.t..
-00001430: 087c 0ba1 0183 0182 0164 0004 007d 0104  .|.......d...}..
-00001440: 007d 0204 007d 0304 007d 0404 007d 0904  .}...}...}...}..
-00001450: 007d 0504 007d 0604 007d 077d 0864 0053  .}...}...}.}.d.S
-00001460: 0029 0a4e 7251 0000 0072 3e00 0000 723f  .).NrQ...r>...r?
-00001470: 0000 0072 0a00 0000 2901 7a78 2528 7079  ...r....).zx%(py
-00001480: 3829 730a 7b25 2870 7938 2973 203d 2025  8)s.{%(py8)s = %
-00001490: 2870 7930 2973 2825 2870 7932 2973 2c20  (py0)s(%(py2)s, 
-000014a0: 2528 7079 3429 732c 2025 2870 7936 2973  %(py4)s, %(py6)s
-000014b0: 290a 7d20 3d3d 2025 2870 7931 3829 730a  ).} == %(py18)s.
-000014c0: 7b25 2870 7931 3829 7320 3d20 2528 7079  {%(py18)s = %(py
-000014d0: 3130 2973 2825 2870 7931 3229 732c 2025  10)s(%(py12)s, %
-000014e0: 2870 7931 3429 732c 2025 2870 7931 3629  (py14)s, %(py16)
-000014f0: 7329 0a7d 7206 0000 00a9 0a72 0e00 0000  s).}r......r....
-00001500: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-00001510: 3300 0000 7235 0000 005a 0470 7931 325a  3...r5...Z.py12Z
-00001520: 0470 7931 345a 0470 7931 365a 0470 7931  .py14Z.py16Z.py1
-00001530: 38fa 0f61 7373 6572 7420 2528 7079 3230  8..assert %(py20
-00001540: 2973 da04 7079 3230 a909 7206 0000 0072  )s..py20..r....r
-00001550: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00001560: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00001570: 0000 721e 0000 00a9 0c72 2000 0000 7221  ..r......r ...r!
-00001580: 0000 0072 2200 0000 7223 0000 0072 2500  ...r"...r#...r%.
-00001590: 0000 5a0c 4070 795f 6173 7365 7274 3131  ..Z.@py_assert11
-000015a0: 5a0c 4070 795f 6173 7365 7274 3133 5a0c  Z.@py_assert13Z.
-000015b0: 4070 795f 6173 7365 7274 3135 5a0c 4070  @py_assert15Z.@p
-000015c0: 795f 6173 7365 7274 3137 5a0b 4070 795f  y_assert17Z.@py_
-000015d0: 6173 7365 7274 395a 0c40 7079 5f66 6f72  assert9Z.@py_for
-000015e0: 6d61 7431 395a 0c40 7079 5f66 6f72 6d61  mat19Z.@py_forma
-000015f0: 7432 3172 2800 0000 7228 0000 0072 2900  t21r(...r(...r).
-00001600: 0000 da0a 7465 7374 5f65 7175 616c 2f00  ....test_equal/.
-00001610: 0000 7302 0000 0000 017a 1743 6163 6865  ..s......z.Cache
-00001620: 4f70 5465 7374 732e 7465 7374 5f65 7175  OpTests.test_equ
-00001630: 616c 6301 0000 0000 0000 0000 0000 000c  alc.............
-00001640: 0000 000d 0000 0043 0000 0073 1e01 0000  .......C...s....
-00001650: 6401 7d01 6402 7d02 6403 7d03 7400 7c01  d.}.d.}.d.}.t.|.
-00001660: 7c02 7c03 8303 7d04 6404 7d05 6402 7d06  |.|...}.d.}.d.}.
-00001670: 6403 7d07 7400 7c05 7c06 7c07 8303 7d08  d.}.t.|.|.|...}.
-00001680: 7c04 7c08 6b03 7d09 7c09 73f6 7401 a002  |.|.k.}.|.s.t...
-00001690: 6405 7c09 6601 6406 7c04 7c08 6602 a104  d.|.f.d.|.|.f...
-000016a0: 6407 7403 a004 a100 7600 7366 7401 a005  d.t.....v.sft...
-000016b0: 7400 a101 7270 7401 a006 7400 a101 6e02  t...rpt...t...n.
-000016c0: 6407 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
-000016d0: a101 7401 a006 7c03 a101 7401 a006 7c04  ..t...|...t...|.
-000016e0: a101 6407 7403 a004 a100 7600 73a8 7401  ..d.t.....v.s.t.
-000016f0: a005 7400 a101 72b2 7401 a006 7400 a101  ..t...r.t...t...
-00001700: 6e02 6407 7401 a006 7c05 a101 7401 a006  n.d.t...|...t...
-00001710: 7c06 a101 7401 a006 7c07 a101 7401 a006  |...t...|...t...
-00001720: 7c08 a101 6408 9c0a 1600 7d0a 6409 640a  |...d.....}.d.d.
-00001730: 7c0a 6901 1600 7d0b 7407 7401 a008 7c0b  |.i...}.t.t...|.
-00001740: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
-00001750: 0400 7d03 0400 7d04 0400 7d09 0400 7d05  ..}...}...}...}.
-00001760: 0400 7d06 0400 7d07 7d08 6400 5300 290b  ..}...}.}.d.S.).
-00001770: 4e72 5100 0000 723e 0000 0072 3f00 0000  NrQ...r>...r?...
-00001780: da01 79a9 01fa 0221 3da9 017a 7825 2870  ..y....!=..zx%(p
-00001790: 7938 2973 0a7b 2528 7079 3829 7320 3d20  y8)s.{%(py8)s = 
-000017a0: 2528 7079 3029 7328 2528 7079 3229 732c  %(py0)s(%(py2)s,
-000017b0: 2025 2870 7934 2973 2c20 2528 7079 3629   %(py4)s, %(py6)
-000017c0: 7329 0a7d 2021 3d20 2528 7079 3138 2973  s).} != %(py18)s
-000017d0: 0a7b 2528 7079 3138 2973 203d 2025 2870  .{%(py18)s = %(p
-000017e0: 7931 3029 7328 2528 7079 3132 2973 2c20  y10)s(%(py12)s, 
-000017f0: 2528 7079 3134 2973 2c20 2528 7079 3136  %(py14)s, %(py16
-00001800: 2973 290a 7d72 0600 0000 7257 0000 0072  )s).}r....rW...r
-00001810: 5800 0000 7259 0000 0072 5a00 0000 725b  X...rY...rZ...r[
-00001820: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00001830: 0000 da14 7465 7374 5f6e 6f74 5f65 7175  ....test_not_equ
-00001840: 616c 5f61 6c69 6173 3200 0000 7302 0000  al_alias2...s...
-00001850: 0000 017a 2143 6163 6865 4f70 5465 7374  ...z!CacheOpTest
-00001860: 732e 7465 7374 5f6e 6f74 5f65 7175 616c  s.test_not_equal
-00001870: 5f61 6c69 6173 6301 0000 0000 0000 0000  _aliasc.........
-00001880: 0000 000c 0000 000d 0000 0043 0000 0073  ...........C...s
-00001890: 1e01 0000 6401 7d01 6402 7d02 6403 7d03  ....d.}.d.}.d.}.
-000018a0: 7400 7c01 7c02 7c03 8303 7d04 6401 7d05  t.|.|.|...}.d.}.
-000018b0: 6403 7d06 6403 7d07 7400 7c05 7c06 7c07  d.}.d.}.t.|.|.|.
-000018c0: 8303 7d08 7c04 7c08 6b03 7d09 7c09 73f6  ..}.|.|.k.}.|.s.
-000018d0: 7401 a002 6404 7c09 6601 6405 7c04 7c08  t...d.|.f.d.|.|.
-000018e0: 6602 a104 6406 7403 a004 a100 7600 7366  f...d.t.....v.sf
-000018f0: 7401 a005 7400 a101 7270 7401 a006 7400  t...t...rpt...t.
-00001900: a101 6e02 6406 7401 a006 7c01 a101 7401  ..n.d.t...|...t.
-00001910: a006 7c02 a101 7401 a006 7c03 a101 7401  ..|...t...|...t.
-00001920: a006 7c04 a101 6406 7403 a004 a100 7600  ..|...d.t.....v.
-00001930: 73a8 7401 a005 7400 a101 72b2 7401 a006  s.t...t...r.t...
-00001940: 7400 a101 6e02 6406 7401 a006 7c05 a101  t...n.d.t...|...
-00001950: 7401 a006 7c06 a101 7401 a006 7c07 a101  t...|...t...|...
-00001960: 7401 a006 7c08 a101 6407 9c0a 1600 7d0a  t...|...d.....}.
-00001970: 6408 6409 7c0a 6901 1600 7d0b 7407 7401  d.d.|.i...}.t.t.
-00001980: a008 7c0b a101 8301 8201 6400 0400 7d01  ..|.......d...}.
-00001990: 0400 7d02 0400 7d03 0400 7d04 0400 7d09  ..}...}...}...}.
-000019a0: 0400 7d05 0400 7d06 0400 7d07 7d08 6400  ..}...}...}.}.d.
-000019b0: 5300 290a 4e72 5100 0000 723e 0000 0072  S.).NrQ...r>...r
-000019c0: 3f00 0000 725e 0000 0072 6000 0000 7206  ?...r^...r`...r.
-000019d0: 0000 0072 5700 0000 7258 0000 0072 5900  ...rW...rX...rY.
-000019e0: 0000 725a 0000 0072 5b00 0000 7228 0000  ..rZ...r[...r(..
-000019f0: 0072 2800 0000 7229 0000 00da 1874 6573  .r(...r).....tes
-00001a00: 745f 6e6f 745f 6571 7561 6c5f 6f70 6572  t_not_equal_oper
-00001a10: 6174 696f 6e35 0000 0073 0200 0000 0001  ation5...s......
-00001a20: 7a25 4361 6368 654f 7054 6573 7473 2e74  z%CacheOpTests.t
-00001a30: 6573 745f 6e6f 745f 6571 7561 6c5f 6f70  est_not_equal_op
-00001a40: 6572 6174 696f 6e63 0100 0000 0000 0000  erationc........
-00001a50: 0000 0000 0c00 0000 0d00 0000 4300 0000  ............C...
-00001a60: 7322 0100 0064 017d 0164 027d 0264 0367  s"...d.}.d.}.d.g
-00001a70: 017d 0374 007c 017c 027c 0383 037d 0464  .}.t.|.|.|...}.d
-00001a80: 017d 0564 027d 0664 0467 017d 0774 007c  .}.d.}.d.g.}.t.|
-00001a90: 057c 067c 0783 037d 087c 047c 086b 037d  .|.|...}.|.|.k.}
-00001aa0: 097c 0973 fa74 01a0 0264 057c 0966 0164  .|.s.t...d.|.f.d
-00001ab0: 067c 047c 0866 02a1 0464 0774 03a0 04a1  .|.|.f...d.t....
-00001ac0: 0076 0073 6a74 01a0 0574 00a1 0172 7474  .v.sjt...t...rtt
-00001ad0: 01a0 0674 00a1 016e 0264 0774 01a0 067c  ...t...n.d.t...|
-00001ae0: 01a1 0174 01a0 067c 02a1 0174 01a0 067c  ...t...|...t...|
-00001af0: 03a1 0174 01a0 067c 04a1 0164 0774 03a0  ...t...|...d.t..
-00001b00: 04a1 0076 0073 ac74 01a0 0574 00a1 0172  ...v.s.t...t...r
-00001b10: b674 01a0 0674 00a1 016e 0264 0774 01a0  .t...t...n.d.t..
-00001b20: 067c 05a1 0174 01a0 067c 06a1 0174 01a0  .|...t...|...t..
-00001b30: 067c 07a1 0174 01a0 067c 08a1 0164 089c  .|...t...|...d..
-00001b40: 0a16 007d 0a64 0964 0a7c 0a69 0116 007d  ...}.d.d.|.i...}
-00001b50: 0b74 0774 01a0 087c 0ba1 0183 0182 0164  .t.t...|.......d
-00001b60: 0004 007d 0104 007d 0204 007d 0304 007d  ...}...}...}...}
-00001b70: 0404 007d 0904 007d 0504 007d 0604 007d  ...}...}...}...}
-00001b80: 077d 0864 0053 0029 0b4e 7251 0000 0072  .}.d.S.).NrQ...r
-00001b90: 3e00 0000 723f 0000 0072 4f00 0000 725e  >...r?...rO...r^
-00001ba0: 0000 0072 6000 0000 7206 0000 0072 5700  ...r`...r....rW.
-00001bb0: 0000 7258 0000 0072 5900 0000 725a 0000  ..rX...rY...rZ..
-00001bc0: 0072 5b00 0000 7228 0000 0072 2800 0000  .r[...r(...r(...
-00001bd0: 7229 0000 00da 1374 6573 745f 6e6f 745f  r).....test_not_
-00001be0: 6571 7561 6c5f 6b65 7973 3800 0000 7302  equal_keys8...s.
-00001bf0: 0000 0000 017a 2043 6163 6865 4f70 5465  .....z CacheOpTe
-00001c00: 7374 732e 7465 7374 5f6e 6f74 5f65 7175  sts.test_not_equ
-00001c10: 616c 5f6b 6579 734e 290f da08 5f5f 6e61  al_keysN)...__na
-00001c20: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00001c30: da0c 5f5f 7175 616c 6e61 6d65 5f5f 722a  ..__qualname__r*
-00001c40: 0000 0072 2c00 0000 722d 0000 0072 3b00  ...r,...r-...r;.
-00001c50: 0000 723c 0000 0072 4e00 0000 7250 0000  ..r<...rN...rP..
-00001c60: 0072 5600 0000 725c 0000 0072 6100 0000  .rV...r\...ra...
-00001c70: 7262 0000 0072 6300 0000 7228 0000 0072  rb...rc...r(...r
-00001c80: 2800 0000 7228 0000 0072 2900 0000 7209  (...r(...r)...r.
-00001c90: 0000 000d 0000 0073 1800 0000 0801 0803  .......s........
-00001ca0: 0803 0803 0804 0804 0806 0806 0804 0803  ................
-00001cb0: 0803 0803 7209 0000 0063 0000 0000 0000  ....r....c......
-00001cc0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00001cd0: 0000 7324 0000 0065 005a 0164 005a 0264  ..s$...e.Z.d.Z.d
-00001ce0: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
-00001cf0: 0564 0684 005a 0564 0753 0029 08da 1243  .d...Z.d.S.)...C
-00001d00: 6163 6865 5265 636f 7264 6572 5465 7374  acheRecorderTest
-00001d10: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
-00001d20: 0000 0800 0000 4300 0000 7356 0000 0074  ......C...sV...t
-00001d30: 00a0 01a1 007d 0174 0264 017c 0183 028f  .....}.t.d.|....
-00001d40: 1e01 0074 0364 0119 00a0 0464 02a1 0101  ...t.d.....d....
-00001d50: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00001d60: 0073 3630 0001 0001 0001 0059 0001 007c  .s60.......Y...|
-00001d70: 01a0 0574 0664 0164 0364 0283 03a1 0101  ...t.d.d.d......
-00001d80: 0064 0053 0029 044e 723d 0000 0072 3e00  .d.S.).Nr=...r>.
-00001d90: 0000 da03 6765 74a9 0772 0800 0000 da04  ....get..r......
-00001da0: 4d6f 636b 7207 0000 0072 0200 0000 7268  Mockr....r....rh
-00001db0: 0000 005a 1761 7373 6572 745f 6361 6c6c  ...Z.assert_call
-00001dc0: 6564 5f6f 6e63 655f 7769 7468 7206 0000  ed_once_withr...
-00001dd0: 00a9 0272 2000 0000 da08 6361 6c6c 6261  ...r .....callba
-00001de0: 636b 7228 0000 0072 2800 0000 7229 0000  ckr(...r(...r)..
-00001df0: 00da 0c74 6573 745f 6465 6661 756c 743d  ...test_default=
-00001e00: 0000 0073 0800 0000 0001 0801 0c01 2c01  ...s..........,.
-00001e10: 7a1f 4361 6368 6552 6563 6f72 6465 7254  z.CacheRecorderT
-00001e20: 6573 7473 2e74 6573 745f 6465 6661 756c  ests.test_defaul
-00001e30: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-00001e40: 0000 0800 0000 4300 0000 7356 0000 0074  ......C...sV...t
-00001e50: 00a0 01a1 007d 0174 0264 017c 0183 028f  .....}.t.d.|....
-00001e60: 1e01 0074 0364 0119 00a0 0464 02a1 0101  ...t.d.....d....
-00001e70: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00001e80: 0073 3630 0001 0001 0001 0059 0001 007c  .s60.......Y...|
-00001e90: 01a0 0574 0664 0164 0364 0283 03a1 0101  ...t.d.d.d......
-00001ea0: 0064 0053 0029 044e da06 7365 636f 6e64  .d.S.).N..second
-00001eb0: 723e 0000 0072 6800 0000 7269 0000 0072  r>...rh...ri...r
-00001ec0: 6b00 0000 7228 0000 0072 2800 0000 7229  k...r(...r(...r)
-00001ed0: 0000 00da 0e74 6573 745f 7365 636f 6e64  .....test_second
-00001ee0: 6172 7943 0000 0073 0800 0000 0001 0801  aryC...s........
-00001ef0: 0c01 2c01 7a21 4361 6368 6552 6563 6f72  ..,.z!CacheRecor
-00001f00: 6465 7254 6573 7473 2e74 6573 745f 7365  derTests.test_se
-00001f10: 636f 6e64 6172 7963 0100 0000 0000 0000  condaryc........
-00001f20: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
-00001f30: 7304 0100 0074 00a0 01a1 007d 0174 0264  s....t.....}.t.d
-00001f40: 017c 0183 028f 1e01 0074 0364 0219 00a0  .|.......t.d....
-00001f50: 0464 03a1 0101 0057 0064 0004 0004 0083  .d.....W.d......
-00001f60: 0301 006e 1031 0073 3630 0001 0001 0001  ...n.1.s60......
-00001f70: 0059 0001 007c 016a 057d 0274 067c 0283  .Y...|.j.}.t.|..
-00001f80: 017d 0364 047d 047c 037c 046b 027d 057c  .}.d.}.|.|.k.}.|
-00001f90: 0573 f074 07a0 0864 057c 0566 0164 067c  .s.t...d.|.f.d.|
-00001fa0: 037c 0466 02a1 0464 0774 09a0 0aa1 0076  .|.f...d.t.....v
-00001fb0: 0073 8874 07a0 0b74 06a1 0172 9274 07a0  .s.t...t...r.t..
-00001fc0: 0c74 06a1 016e 0264 0764 0874 09a0 0aa1  .t...n.d.d.t....
-00001fd0: 0076 0073 aa74 07a0 0b7c 01a1 0172 b474  .v.s.t...|...r.t
-00001fe0: 07a0 0c7c 01a1 016e 0264 0874 07a0 0c7c  ...|...n.d.t...|
-00001ff0: 02a1 0174 07a0 0c7c 03a1 0174 07a0 0c7c  ...t...|...t...|
-00002000: 04a1 0164 099c 0516 007d 0664 0a64 0b7c  ...d.....}.d.d.|
-00002010: 0669 0116 007d 0774 0d74 07a0 0e7c 07a1  .i...}.t.t...|..
-00002020: 0183 0182 0164 0004 007d 0204 007d 0304  .....d...}...}..
-00002030: 007d 057d 0464 0053 0029 0c4e 726e 0000  .}.}.d.S.).Nrn..
-00002040: 0072 3d00 0000 723e 0000 0072 0100 0000  .r=...r>...r....
-00002050: 720a 0000 0029 017a 5025 2870 7935 2973  r....).zP%(py5)s
-00002060: 0a7b 2528 7079 3529 7320 3d20 2528 7079  .{%(py5)s = %(py
-00002070: 3029 7328 2528 7079 3329 730a 7b25 2870  0)s(%(py3)s.{%(p
-00002080: 7933 2973 203d 2025 2870 7931 2973 2e6d  y3)s = %(py1)s.m
-00002090: 6f63 6b5f 6361 6c6c 730a 7d29 0a7d 203d  ock_calls.}).} =
-000020a0: 3d20 2528 7079 3829 73da 036c 656e 726c  = %(py8)s..lenrl
-000020b0: 0000 0029 0572 0e00 0000 da03 7079 3172  ...).r......py1r
-000020c0: 3100 0000 7232 0000 0072 3300 0000 7234  1...r2...r3...r4
-000020d0: 0000 0072 3500 0000 290f 7208 0000 0072  ...r5...).r....r
-000020e0: 6a00 0000 7207 0000 0072 0200 0000 7268  j...r....r....rh
-000020f0: 0000 00da 0a6d 6f63 6b5f 6361 6c6c 7372  .....mock_callsr
-00002100: 7000 0000 7217 0000 0072 1800 0000 7219  p...r....r....r.
-00002110: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00002120: 0000 721d 0000 0072 1e00 0000 2908 7220  ..r....r....).r 
-00002130: 0000 0072 6c00 0000 da0b 4070 795f 6173  ...rl.....@py_as
-00002140: 7365 7274 3272 3700 0000 7225 0000 0072  sert2r7...r%...r
-00002150: 3800 0000 7239 0000 0072 3a00 0000 7228  8...r9...r:...r(
-00002160: 0000 0072 2800 0000 7229 0000 00da 2374  ...r(...r)....#t
-00002170: 6573 745f 7365 636f 6e64 6172 795f 6465  est_secondary_de
-00002180: 6661 756c 745f 6e6f 745f 7265 636f 7264  fault_not_record
-00002190: 6564 4900 0000 7308 0000 0000 0108 010c  edI...s.........
-000021a0: 012c 017a 3643 6163 6865 5265 636f 7264  .,.z6CacheRecord
-000021b0: 6572 5465 7374 732e 7465 7374 5f73 6563  erTests.test_sec
-000021c0: 6f6e 6461 7279 5f64 6566 6175 6c74 5f6e  ondary_default_n
-000021d0: 6f74 5f72 6563 6f72 6465 644e 2906 7264  ot_recordedN).rd
-000021e0: 0000 0072 6500 0000 7266 0000 0072 6d00  ...re...rf...rm.
-000021f0: 0000 726f 0000 0072 7400 0000 7228 0000  ..ro...rt...r(..
-00002200: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
-00002210: 7267 0000 003c 0000 0073 0600 0000 0801  rg...<...s......
-00002220: 0806 0806 7267 0000 0063 0000 0000 0000  ....rg...c......
-00002230: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00002240: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00002250: 0164 0284 005a 0364 0353 0029 04da 1541  .d...Z.d.S.)...A
-00002260: 6c6c 4361 6368 6552 6563 6f72 6465 7254  llCacheRecorderT
-00002270: 6573 7473 6301 0000 0000 0000 0000 0000  estsc...........
-00002280: 0007 0000 0008 0000 0043 0000 0073 2001  .........C...s .
-00002290: 0000 7400 a001 a100 7d01 7402 7c01 8301  ..t.....}.t.|...
-000022a0: 8f3e 0100 7403 6401 1900 a004 6402 a101  .>..t.d.....d...
-000022b0: 0100 7403 6403 1900 a005 6404 6405 a102  ..t.d.....d.d...
-000022c0: 0100 7403 6401 1900 a006 6402 6701 a101  ..t.d.....d.g...
-000022d0: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
-000022e0: 3100 7354 3000 0100 0100 0100 5900 0100  1.sT0.......Y...
-000022f0: 7c01 6a07 7d02 7400 a008 7409 6401 6406  |.j.}.t...t.d.d.
-00002300: 6402 8303 a101 7400 a008 7409 6403 6407  d.....t...t.d.d.
-00002310: 6404 8303 a101 7400 a008 7409 6401 6408  d.....t...t.d.d.
-00002320: 6402 6701 8303 a101 6703 7d03 7c02 7c03  d.g.....g.}.|.|.
-00002330: 6b02 7d04 7c04 9001 7310 740a a00b 6409  k.}.|...s.t...d.
-00002340: 7c04 6601 640a 7c02 7c03 6602 a104 640b  |.f.d.|.|.f...d.
-00002350: 740c a00d a100 7600 73d2 740a a00e 7c01  t.....v.s.t...|.
-00002360: a101 72dc 740a a00f 7c01 a101 6e02 640b  ..r.t...|...n.d.
-00002370: 740a a00f 7c02 a101 740a a00f 7c03 a101  t...|...t...|...
-00002380: 640c 9c03 1600 7d05 640d 640e 7c05 6901  d.....}.d.d.|.i.
-00002390: 1600 7d06 7410 740a a011 7c06 a101 8301  ..}.t.t...|.....
-000023a0: 8201 6400 0400 7d02 0400 7d04 7d03 6400  ..d...}...}.}.d.
-000023b0: 5300 290f 4e72 3d00 0000 723e 0000 0072  S.).Nr=...r>...r
-000023c0: 6e00 0000 723f 0000 0072 4f00 0000 7268  n...r?...rO...rh
-000023d0: 0000 00da 0373 6574 da0b 6465 6c65 7465  .....set..delete
-000023e0: 5f6d 616e 7972 0a00 0000 2901 7a32 2528  _manyr....).z2%(
-000023f0: 7079 3229 730a 7b25 2870 7932 2973 203d  py2)s.{%(py2)s =
-00002400: 2025 2870 7930 2973 2e6d 6f63 6b5f 6361   %(py0)s.mock_ca
-00002410: 6c6c 730a 7d20 3d3d 2025 2870 7935 2973  lls.} == %(py5)s
-00002420: 726c 0000 0072 4200 0000 7243 0000 0072  rl...rB...rC...r
-00002430: 4400 0000 2912 7208 0000 0072 6a00 0000  D...).r....rj...
-00002440: 7205 0000 0072 0200 0000 7268 0000 0072  r....r....rh...r
-00002450: 7600 0000 7277 0000 0072 7200 0000 da04  v...rw...rr.....
-00002460: 6361 6c6c 7206 0000 0072 1700 0000 7218  callr....r....r.
-00002470: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00002480: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
-00002490: 0029 0772 2000 0000 726c 0000 0072 2100  .).r ...rl...r!.
-000024a0: 0000 7237 0000 0072 2200 0000 724c 0000  ..r7...r"...rL..
-000024b0: 0072 4d00 0000 7228 0000 0072 2800 0000  .rM...r(...r(...
-000024c0: 7229 0000 00da 1074 6573 745f 7265 636f  r).....test_reco
-000024d0: 7264 735f 616c 6c51 0000 0073 0c00 0000  rds_allQ...s....
-000024e0: 0001 0801 0a01 0e01 1001 2e02 7a26 416c  ............z&Al
-000024f0: 6c43 6163 6865 5265 636f 7264 6572 5465  lCacheRecorderTe
-00002500: 7374 732e 7465 7374 5f72 6563 6f72 6473  sts.test_records
-00002510: 5f61 6c6c 4e29 0472 6400 0000 7265 0000  _allN).rd...re..
-00002520: 0072 6600 0000 7279 0000 0072 2800 0000  .rf...ry...r(...
-00002530: 7228 0000 0072 2800 0000 7229 0000 0072  r(...r(...r)...r
-00002540: 7500 0000 5000 0000 7302 0000 0008 0172  u...P...s......r
-00002550: 7500 0000 2916 da08 6275 696c 7469 6e73  u...)...builtins
-00002560: 7219 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
-00002570: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
-00002580: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
-00002590: 7269 7465 7217 0000 0072 5200 0000 da11  riter....rR.....
-000025a0: 646a 616e 676f 2e63 6f72 652e 6361 6368  django.core.cach
-000025b0: 6572 0200 0000 da0b 646a 616e 676f 2e74  er......django.t
-000025c0: 6573 7472 0300 0000 7204 0000 00da 1564  estr....r......d
-000025d0: 6a61 6e67 6f5f 7065 7266 5f72 6563 2e63  jango_perf_rec.c
-000025e0: 6163 6865 7205 0000 0072 0600 0000 7207  acher....r....r.
-000025f0: 0000 00da 0875 6e69 7474 6573 7472 0800  .....unittestr..
-00002600: 0000 da0b 496d 706f 7274 4572 726f 7272  ....ImportErrorr
-00002610: 0900 0000 7267 0000 0072 7500 0000 7228  ....rg...ru...r(
-00002620: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00002630: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002640: 7314 0000 0022 010c 0110 0214 0202 0110  s...."..........
-00002650: 010c 010e 0310 2f10 14                   ....../..
+00000000: 420d 0d0a 7d79 7c5e ef09 0000 e300 0000  B...}y|^........
+00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000020: 0073 6a00 0000 6400 6401 6c00 5a01 6400  .sj...d.d.l.Z.d.
+00000030: 6401 6c02 6d03 0200 0100 6d04 5a05 0100  d.l.m.....m.Z...
+00000040: 6400 6401 6c06 5a06 6400 6402 6c07 6d08  d.d.l.Z.d.d.l.m.
+00000050: 5a08 0100 6400 6401 6c09 5a09 6400 6401  Z...d.d.l.Z.d.d.
+00000060: 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c 0100  l.Z.d.d.l.m.Z...
+00000070: 6400 6404 6c0d 6d0e 5a0e 0100 4700 6405  d.d.l.m.Z...G.d.
+00000080: 6406 8400 6406 650c 8303 5a0f 6401 5300  d...d.e...Z.d.S.
+00000090: 2907 e900 0000 004e 2901 da07 6d6b 6474  )......N)...mkdt
+000000a0: 656d 7029 01da 0e53 696d 706c 6554 6573  emp)...SimpleTes
+000000b0: 7443 6173 6529 01da 064b 5646 696c 6563  tCase)...KVFilec
+000000c0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000000d0: 0000 0000 7370 0000 0065 005a 0164 005a  ....sp...e.Z.d.Z
+000000e0: 0287 0066 0164 0164 0284 085a 0387 0066  ...f.d.d...Z...f
+000000f0: 0164 0364 0484 085a 0464 0564 0684 005a  .d.d...Z.d.d...Z
+00000100: 0564 0764 0884 005a 0664 0964 0a84 005a  .d.d...Z.d.d...Z
+00000110: 0764 0b64 0c84 005a 0864 0d64 0e84 005a  .d.d...Z.d.d...Z
+00000120: 0964 0f64 1084 005a 0a64 1164 1284 005a  .d.d...Z.d.d...Z
+00000130: 0b64 1364 1484 005a 0c64 1564 1684 005a  .d.d...Z.d.d...Z
+00000140: 0d87 0004 005a 0e53 0029 17da 0b4b 5646  .....Z.S.)...KVF
+00000150: 696c 6554 6573 7473 6301 0000 0000 0000  ileTestsc.......
+00000160: 0001 0000 0002 0000 0003 0000 0073 1e00  .............s..
+00000170: 0000 7400 8300 a001 a100 0100 7402 a003  ..t.........t...
+00000180: a100 0100 7404 8300 7c00 5f05 6400 5300  ....t...|._.d.S.
+00000190: 2901 4e29 06da 0573 7570 6572 da05 7365  ).N)...super..se
+000001a0: 7455 7072 0400 0000 da11 5f63 6c65 6172  tUpr......_clear
+000001b0: 5f6c 6f61 645f 6361 6368 6572 0200 0000  _load_cacher....
+000001c0: da08 7465 6d70 5f64 6972 2901 da04 7365  ..temp_dir)...se
+000001d0: 6c66 2901 da09 5f5f 636c 6173 735f 5fa9  lf)...__class__.
+000001e0: 00fa 432f 5573 6572 732f 6368 6169 6e7a  ..C/Users/chainz
+000001f0: 2f44 6f63 756d 656e 7473 2f50 726f 6a65  /Documents/Proje
+00000200: 6374 732f 646a 616e 676f 2d70 6572 662d  cts/django-perf-
+00000210: 7265 632f 7465 7374 732f 7465 7374 5f79  rec/tests/test_y
+00000220: 616d 6c2e 7079 7207 0000 000c 0000 0073  aml.pyr........s
+00000230: 0600 0000 0001 0a01 0801 7a11 4b56 4669  ..........z.KVFi
+00000240: 6c65 5465 7374 732e 7365 7455 7063 0100  leTests.setUpc..
+00000250: 0000 0000 0000 0100 0000 0300 0000 0300  ................
+00000260: 0000 731a 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
+00000270: 0101 0074 0383 00a0 04a1 0001 0064 0053  ...t.........d.S
+00000280: 0029 014e 2905 da06 7368 7574 696c da06  .).N)...shutil..
+00000290: 726d 7472 6565 7209 0000 0072 0600 0000  rmtreer....r....
+000002a0: da08 7465 6172 446f 776e 2901 720a 0000  ..tearDown).r...
+000002b0: 0029 0172 0b00 0000 720c 0000 0072 0d00  .).r....r....r..
+000002c0: 0000 7210 0000 0011 0000 0073 0400 0000  ..r........s....
+000002d0: 0001 0c01 7a14 4b56 4669 6c65 5465 7374  ....z.KVFileTest
+000002e0: 732e 7465 6172 446f 776e 6301 0000 0000  s.tearDownc.....
+000002f0: 0000 0001 0000 0009 0000 0043 0000 0073  ...........C...s
+00000300: 2200 0000 7400 a001 7402 a101 8f0e 0100  "...t...t.......
+00000310: 7403 6401 8301 0100 5700 6400 5100 5200  t.d.....W.d.Q.R.
+00000320: 5800 6400 5300 2902 4efa 012f 2904 da06  X.d.S.).N../)...
+00000330: 7079 7465 7374 da06 7261 6973 6573 da07  pytest..raises..
+00000340: 494f 4572 726f 7272 0400 0000 2901 720a  IOErrorr....).r.
+00000350: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
+00000360: 0000 da18 7465 7374 5f6c 6f61 645f 6e6f  ....test_load_no
+00000370: 5f70 6572 6d69 7373 696f 6e73 1500 0000  _permissions....
+00000380: 7304 0000 0000 010c 017a 244b 5646 696c  s........z$KVFil
+00000390: 6554 6573 7473 2e74 6573 745f 6c6f 6164  eTests.test_load
+000003a0: 5f6e 6f5f 7065 726d 6973 7369 6f6e 7363  _no_permissionsc
+000003b0: 0100 0000 0000 0000 0e00 0000 0900 0000  ................
+000003c0: 4300 0000 73b8 0100 0074 007c 006a 0164  C...s....t.|.j.d
+000003d0: 0117 0083 017d 0174 027c 0183 017d 0264  .....}.t.|...}.d
+000003e0: 027d 037c 027c 036b 027d 047c 0473 b074  .}.|.|.k.}.|.s.t
+000003f0: 03a0 0464 037c 0466 0164 047c 027c 0366  ...d.|.f.d.|.|.f
+00000400: 02a1 0464 0574 05a0 06a1 006b 0673 5074  ...d.t.....k.sPt
+00000410: 03a0 0774 02a1 0172 5a74 03a0 0874 02a1  ...t...rZt...t..
+00000420: 016e 0264 0564 0674 05a0 06a1 006b 0673  .n.d.d.t.....k.s
+00000430: 7274 03a0 077c 01a1 0172 7c74 03a0 087c  rt...|...r|t...|
+00000440: 01a1 016e 0264 0674 03a0 087c 02a1 0174  ...n.d.t...|...t
+00000450: 03a0 087c 03a1 0164 079c 0416 007d 0564  ...|...d.....}.d
+00000460: 0864 097c 0569 0116 007d 0674 0974 03a0  .d.|.i...}.t.t..
+00000470: 0a7c 06a1 0183 0182 0164 0004 007d 0204  .|.......d...}..
+00000480: 007d 047d 0374 0b83 007d 077c 016a 0c7d  .}.}.t...}.|.j.}
+00000490: 0864 0a7d 097c 087c 097c 0783 027d 0a7c  .d.}.|.|.|...}.|
+000004a0: 0a7c 076b 087d 0b7c 0b90 0173 a474 03a0  .|.k.}.|...s.t..
+000004b0: 0464 0b7c 0b66 0164 0c7c 0a7c 0766 02a1  .d.|.f.d.|.|.f..
+000004c0: 0464 0674 05a0 06a1 006b 0690 0173 1274  .d.t.....k...s.t
+000004d0: 03a0 077c 01a1 0190 0172 1c74 03a0 087c  ...|.....r.t...|
+000004e0: 01a1 016e 0264 0674 03a0 087c 08a1 0174  ...n.d.t...|...t
+000004f0: 03a0 087c 09a1 0164 0d74 05a0 06a1 006b  ...|...d.t.....k
+00000500: 0690 0173 4874 03a0 077c 07a1 0190 0172  ...sHt...|.....r
+00000510: 5274 03a0 087c 07a1 016e 0264 0d74 03a0  Rt...|...n.d.t..
+00000520: 087c 0aa1 0164 0d74 05a0 06a1 006b 0690  .|...d.t.....k..
+00000530: 0173 7674 03a0 077c 07a1 0190 0172 8074  .svt...|.....r.t
+00000540: 03a0 087c 07a1 016e 0264 0d64 0e9c 0616  ...|...n.d.d....
+00000550: 007d 0c64 0f64 107c 0c69 0116 007d 0d74  .}.d.d.|.i...}.t
+00000560: 0974 03a0 0a7c 0da1 0183 0182 0164 0004  .t...|.......d..
+00000570: 007d 0804 007d 0904 007d 0a7d 0b64 0053  .}...}...}.}.d.S
+00000580: 0029 114e 7a08 2f66 6f6f 2e79 6d6c 7201  .).Nz./foo.ymlr.
+00000590: 0000 0029 01fa 023d 3d29 017a 3025 2870  ...)...==).z0%(p
+000005a0: 7933 2973 0a7b 2528 7079 3329 7320 3d20  y3)s.{%(py3)s = 
+000005b0: 2528 7079 3029 7328 2528 7079 3129 7329  %(py0)s(%(py1)s)
+000005c0: 0a7d 203d 3d20 2528 7079 3629 73da 036c  .} == %(py6)s..l
+000005d0: 656e da03 6b76 6629 04da 0370 7930 da03  en..kvf)...py0..
+000005e0: 7079 31da 0370 7933 da03 7079 367a 0e61  py1..py3..py6z.a
+000005f0: 7373 6572 7420 2528 7079 3829 73da 0370  ssert %(py8)s..p
+00000600: 7938 da03 666f 6f29 01da 0269 7329 017a  y8..foo)...is).z
+00000610: 5225 2870 7937 2973 0a7b 2528 7079 3729  R%(py7)s.{%(py7)
+00000620: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
+00000630: 7932 2973 203d 2025 2870 7930 2973 2e67  y2)s = %(py0)s.g
+00000640: 6574 0a7d 2825 2870 7934 2973 2c20 2528  et.}(%(py4)s, %(
+00000650: 7079 3529 7329 0a7d 2069 7320 2528 7079  py5)s).} is %(py
+00000660: 3929 73da 0764 6566 6175 6c74 2906 7219  9)s..default).r.
+00000670: 0000 00da 0370 7932 da03 7079 34da 0370  .....py2..py4..p
+00000680: 7935 da03 7079 37da 0370 7939 7a0f 6173  y5..py7..py9z.as
+00000690: 7365 7274 2025 2870 7931 3129 73da 0470  sert %(py11)s..p
+000006a0: 7931 3129 0d72 0400 0000 7209 0000 0072  y11).r....r....r
+000006b0: 1700 0000 da0a 4070 7974 6573 745f 6172  ......@pytest_ar
+000006c0: da11 5f63 616c 6c5f 7265 7072 636f 6d70  .._call_reprcomp
+000006d0: 6172 65da 0c40 7079 5f62 7569 6c74 696e  are..@py_builtin
+000006e0: 73da 066c 6f63 616c 73da 185f 7368 6f75  s..locals.._shou
+000006f0: 6c64 5f72 6570 725f 676c 6f62 616c 5f6e  ld_repr_global_n
+00000700: 616d 65da 095f 7361 6665 7265 7072 da0e  ame.._saferepr..
+00000710: 4173 7365 7274 696f 6e45 7272 6f72 da13  AssertionError..
+00000720: 5f66 6f72 6d61 745f 6578 706c 616e 6174  _format_explanat
+00000730: 696f 6eda 066f 626a 6563 74da 0367 6574  ion..object..get
+00000740: 290e 720a 0000 0072 1800 0000 da0b 4070  ).r....r......@p
+00000750: 795f 6173 7365 7274 32da 0b40 7079 5f61  y_assert2..@py_a
+00000760: 7373 6572 7435 da0b 4070 795f 6173 7365  ssert5..@py_asse
+00000770: 7274 34da 0b40 7079 5f66 6f72 6d61 7437  rt4..@py_format7
+00000780: da0b 4070 795f 666f 726d 6174 3972 2000  ..@py_format9r .
+00000790: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
+000007a0: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
+000007b0: 795f 6173 7365 7274 36da 0b40 7079 5f61  y_assert6..@py_a
+000007c0: 7373 6572 7438 da0c 4070 795f 666f 726d  ssert8..@py_form
+000007d0: 6174 3130 da0c 4070 795f 666f 726d 6174  at10..@py_format
+000007e0: 3132 720c 0000 0072 0c00 0000 720d 0000  12r....r....r...
+000007f0: 00da 1f74 6573 745f 6c6f 6164 5f6e 6f6e  ...test_load_non
+00000800: 5f65 7869 7374 656e 745f 6973 5f65 6d70  _existent_is_emp
+00000810: 7479 1900 0000 7326 0000 0000 010e 0108  ty....s&........
+00000820: 0004 0008 0004 0070 000c 000e 000c 0106  .......p........
+00000830: 0106 0004 000a 0008 0006 00a6 000c 000e  ................
+00000840: 007a 2b4b 5646 696c 6554 6573 7473 2e74  .z+KVFileTests.t
+00000850: 6573 745f 6c6f 6164 5f6e 6f6e 5f65 7869  est_load_non_exi
+00000860: 7374 656e 745f 6973 5f65 6d70 7479 6301  stent_is_emptyc.
+00000870: 0000 0000 0000 0010 0000 0009 0000 0043  ...............C
+00000880: 0000 0073 aa01 0000 7c00 6a00 6401 1700  ...s....|.j.d...
+00000890: 7d01 7401 7c01 6402 8302 8f10 7d02 7c02  }.t.|.d.....}.|.
+000008a0: a002 6403 a101 0100 5700 6400 5100 5200  ..d.....W.d.Q.R.
+000008b0: 5800 7403 7c01 8301 7d03 7404 7c03 8301  X.t.|...}.t.|...
+000008c0: 7d04 6404 7d05 7c04 7c05 6b02 7d06 7c06  }.d.}.|.|.k.}.|.
+000008d0: 73d4 7405 a006 6405 7c06 6601 6406 7c04  s.t...d.|.f.d.|.
+000008e0: 7c05 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
+000008f0: 7374 7405 a009 7404 a101 727e 7405 a00a  stt...t...r~t...
+00000900: 7404 a101 6e02 6407 6408 7407 a008 a100  t...n.d.d.t.....
+00000910: 6b06 7396 7405 a009 7c03 a101 72a0 7405  k.s.t...|...r.t.
+00000920: a00a 7c03 a101 6e02 6408 7405 a00a 7c04  ..|...n.d.t...|.
+00000930: a101 7405 a00a 7c05 a101 6409 9c04 1600  ..t...|...d.....
+00000940: 7d07 640a 640b 7c07 6901 1600 7d08 740b  }.d.d.|.i...}.t.
+00000950: 7405 a00c 7c08 a101 8301 8201 6400 0400  t...|.......d...
+00000960: 7d04 0400 7d06 7d05 7c03 6a0d 7d09 640c  }...}.}.|.j.}.d.
+00000970: 7d0a 640d 7d05 7c09 7c0a 7c05 8302 7d0b  }.d.}.|.|.|...}.
+00000980: 640e 7d0c 7c0b 7c0c 6b02 7d0d 7c0d 9001  d.}.|.|.k.}.|...
+00000990: 738e 7405 a006 6405 7c0d 6601 640f 7c0b  s.t...d.|.f.d.|.
+000009a0: 7c0c 6602 a104 6408 7407 a008 a100 6b06  |.f...d.t.....k.
+000009b0: 9001 7338 7405 a009 7c03 a101 9001 7242  ..s8t...|.....rB
+000009c0: 7405 a00a 7c03 a101 6e02 6408 7405 a00a  t...|...n.d.t...
+000009d0: 7c09 a101 7405 a00a 7c0a a101 7405 a00a  |...t...|...t...
+000009e0: 7c05 a101 7405 a00a 7c0b a101 7405 a00a  |...t...|...t...
+000009f0: 7c0c a101 6410 9c06 1600 7d0e 6411 6412  |...d.....}.d.d.
+00000a00: 7c0e 6901 1600 7d0f 740b 7405 a00c 7c0f  |.i...}.t.t...|.
+00000a10: a101 8301 8201 6400 0400 7d09 0400 7d0a  ......d...}...}.
+00000a20: 0400 7d05 0400 7d0b 0400 7d0d 7d0c 6400  ..}...}...}.}.d.
+00000a30: 5300 2913 4e7a 082f 666f 6f2e 796d 6cda  S.).Nz./foo.yml.
+00000a40: 0177 7a08 666f 6f3a 2062 6172 e901 0000  .wz.foo: bar....
+00000a50: 0029 0172 1600 0000 2901 7a30 2528 7079  .).r....).z0%(py
+00000a60: 3329 730a 7b25 2870 7933 2973 203d 2025  3)s.{%(py3)s = %
+00000a70: 2870 7930 2973 2825 2870 7931 2973 290a  (py0)s(%(py1)s).
+00000a80: 7d20 3d3d 2025 2870 7936 2973 7217 0000  } == %(py6)sr...
+00000a90: 0072 1800 0000 2904 7219 0000 0072 1a00  .r....).r....r..
+00000aa0: 0000 721b 0000 0072 1c00 0000 7a0e 6173  ..r....r....z.as
+00000ab0: 7365 7274 2025 2870 7938 2973 721d 0000  sert %(py8)sr...
+00000ac0: 0072 1e00 0000 da00 da03 6261 7229 017a  .r........bar).z
+00000ad0: 5325 2870 7938 2973 0a7b 2528 7079 3829  S%(py8)s.{%(py8)
+00000ae0: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
+00000af0: 7932 2973 203d 2025 2870 7930 2973 2e67  y2)s = %(py0)s.g
+00000b00: 6574 0a7d 2825 2870 7934 2973 2c20 2528  et.}(%(py4)s, %(
+00000b10: 7079 3629 7329 0a7d 203d 3d20 2528 7079  py6)s).} == %(py
+00000b20: 3131 2973 2906 7219 0000 0072 2100 0000  11)s).r....r!...
+00000b30: 7222 0000 0072 1c00 0000 721d 0000 0072  r"...r....r....r
+00000b40: 2600 0000 7a0f 6173 7365 7274 2025 2870  &...z.assert %(p
+00000b50: 7931 3329 73da 0470 7931 3329 0e72 0900  y13)s..py13).r..
+00000b60: 0000 da04 6f70 656e da05 7772 6974 6572  ....open..writer
+00000b70: 0400 0000 7217 0000 0072 2700 0000 7228  ....r....r'...r(
+00000b80: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
+00000b90: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
+00000ba0: 0072 3000 0000 2910 720a 0000 00da 0966  .r0...).r......f
+00000bb0: 696c 655f 6e61 6d65 da02 6670 7218 0000  ile_name..fpr...
+00000bc0: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
+00000bd0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
+00000be0: 3700 0000 da0b 4070 795f 6173 7365 7274  7.....@py_assert
+00000bf0: 37da 0c40 7079 5f61 7373 6572 7431 30da  7..@py_assert10.
+00000c00: 0b40 7079 5f61 7373 6572 7439 723b 0000  .@py_assert9r;..
+00000c10: 00da 0c40 7079 5f66 6f72 6d61 7431 3472  ...@py_format14r
+00000c20: 0c00 0000 720c 0000 0072 0d00 0000 da12  ....r....r......
+00000c30: 7465 7374 5f6c 6f61 645f 6578 6973 7465  test_load_existe
+00000c40: 6e74 1f00 0000 732e 0000 0000 010a 010c  nt....s.........
+00000c50: 0114 0208 0108 0004 0008 0004 0070 000c  .............p..
+00000c60: 000e 000c 0106 0004 0004 000a 0004 0008  ................
+00000c70: 0006 006a 000c 000e 007a 1e4b 5646 696c  ...j.....z.KVFil
+00000c80: 6554 6573 7473 2e74 6573 745f 6c6f 6164  eTests.test_load
+00000c90: 5f65 7869 7374 656e 7463 0100 0000 0000  _existentc......
+00000ca0: 0000 0900 0000 0900 0000 4300 0000 7312  ..........C...s.
+00000cb0: 0100 007c 006a 0064 0117 007d 0174 017c  ...|.j.d...}.t.|
+00000cc0: 0164 0283 028f 107d 027c 02a0 0264 03a1  .d.....}.|...d..
+00000cd0: 0101 0057 0064 0051 0052 0058 0074 037c  ...W.d.Q.R.X.t.|
+00000ce0: 0183 017d 0374 047c 0383 017d 0464 047d  ...}.t.|...}.d.}
+00000cf0: 057c 047c 056b 027d 067c 0673 fe74 05a0  .|.|.k.}.|.s.t..
+00000d00: 0664 057c 0666 0164 067c 047c 0566 02a1  .d.|.f.d.|.|.f..
+00000d10: 0464 0774 07a0 08a1 006b 0673 7474 05a0  .d.t.....k.stt..
+00000d20: 0974 04a1 0172 7e74 05a0 0a74 04a1 016e  .t...r~t...t...n
+00000d30: 0264 0764 0874 07a0 08a1 006b 0673 9674  .d.d.t.....k.s.t
+00000d40: 05a0 0974 03a1 0172 a074 05a0 0a74 03a1  ...t...r.t...t..
+00000d50: 016e 0264 0864 0974 07a0 08a1 006b 0673  .n.d.d.t.....k.s
+00000d60: b874 05a0 097c 01a1 0172 c274 05a0 0a7c  .t...|...r.t...|
+00000d70: 01a1 016e 0264 0974 05a0 0a7c 03a1 0174  ...n.d.t...|...t
+00000d80: 05a0 0a7c 04a1 0174 05a0 0a7c 05a1 0164  ...|...t...|...d
+00000d90: 0a9c 0616 007d 0764 0b64 0c7c 0769 0116  .....}.d.d.|.i..
+00000da0: 007d 0874 0b74 05a0 0c7c 08a1 0183 0182  .}.t.t...|......
+00000db0: 0164 0004 007d 0304 007d 0404 007d 067d  .d...}...}...}.}
+00000dc0: 0564 0053 0029 0d4e 7a08 2f66 6f6f 2e79  .d.S.).Nz./foo.y
+00000dd0: 6d6c 723d 0000 0072 3f00 0000 7201 0000  mlr=...r?...r...
+00000de0: 0029 0172 1600 0000 2901 7a4e 2528 7079  .).r....).zN%(py
+00000df0: 3629 730a 7b25 2870 7936 2973 203d 2025  6)s.{%(py6)s = %
+00000e00: 2870 7930 2973 2825 2870 7934 2973 0a7b  (py0)s(%(py4)s.{
+00000e10: 2528 7079 3429 7320 3d20 2528 7079 3129  %(py4)s = %(py1)
+00000e20: 7328 2528 7079 3229 7329 0a7d 290a 7d20  s(%(py2)s).}).} 
+00000e30: 3d3d 2025 2870 7939 2973 7217 0000 0072  == %(py9)sr....r
+00000e40: 0400 0000 7244 0000 0029 0672 1900 0000  ....rD...).r....
+00000e50: 721a 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
+00000e60: 1c00 0000 7225 0000 007a 0f61 7373 6572  ....r%...z.asser
+00000e70: 7420 2528 7079 3131 2973 7226 0000 0029  t %(py11)sr&...)
+00000e80: 0d72 0900 0000 7242 0000 0072 4300 0000  .r....rB...rC...
+00000e90: 7204 0000 0072 1700 0000 7227 0000 0072  r....r....r'...r
+00000ea0: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
+00000eb0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+00000ec0: 0000 2909 720a 0000 0072 4400 0000 7245  ..).r....rD...rE
+00000ed0: 0000 0072 3700 0000 7232 0000 0072 3900  ...r7...r2...r9.
+00000ee0: 0000 7246 0000 0072 3a00 0000 723b 0000  ..rF...r:...r;..
+00000ef0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
+00000f00: da0f 7465 7374 5f6c 6f61 645f 656d 7074  ..test_load_empt
+00000f10: 7928 0000 0073 1800 0000 0001 0a01 0c01  y(...s..........
+00000f20: 1402 0800 0800 0400 0800 0400 9a00 0c00  ................
+00000f30: 0e00 7a1b 4b56 4669 6c65 5465 7374 732e  ..z.KVFileTests.
+00000f40: 7465 7374 5f6c 6f61 645f 656d 7074 7963  test_load_emptyc
+00000f50: 0100 0000 0000 0000 0900 0000 0900 0000  ................
+00000f60: 4300 0000 7312 0100 007c 006a 0064 0117  C...s....|.j.d..
+00000f70: 007d 0174 017c 0164 0283 028f 107d 027c  .}.t.|.d.....}.|
+00000f80: 02a0 0264 03a1 0101 0057 0064 0051 0052  ...d.....W.d.Q.R
+00000f90: 0058 0074 037c 0183 017d 0374 047c 0383  .X.t.|...}.t.|..
+00000fa0: 017d 0464 047d 057c 047c 056b 027d 067c  .}.d.}.|.|.k.}.|
+00000fb0: 0673 fe74 05a0 0664 057c 0666 0164 067c  .s.t...d.|.f.d.|
+00000fc0: 047c 0566 02a1 0464 0774 07a0 08a1 006b  .|.f...d.t.....k
+00000fd0: 0673 7474 05a0 0974 04a1 0172 7e74 05a0  .stt...t...r~t..
+00000fe0: 0a74 04a1 016e 0264 0764 0874 07a0 08a1  .t...n.d.d.t....
+00000ff0: 006b 0673 9674 05a0 0974 03a1 0172 a074  .k.s.t...t...r.t
+00001000: 05a0 0a74 03a1 016e 0264 0864 0974 07a0  ...t...n.d.d.t..
+00001010: 08a1 006b 0673 b874 05a0 097c 01a1 0172  ...k.s.t...|...r
+00001020: c274 05a0 0a7c 01a1 016e 0264 0974 05a0  .t...|...n.d.t..
+00001030: 0a7c 03a1 0174 05a0 0a7c 04a1 0174 05a0  .|...t...|...t..
+00001040: 0a7c 05a1 0164 0a9c 0616 007d 0764 0b64  .|...d.....}.d.d
+00001050: 0c7c 0769 0116 007d 0874 0b74 05a0 0c7c  .|.i...}.t.t...|
+00001060: 08a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
+00001070: 0404 007d 067d 0564 0053 0029 0d4e 7a08  ...}.}.d.S.).Nz.
+00001080: 2f66 6f6f 2e79 6d6c 723d 0000 007a 0220  /foo.ymlr=...z. 
+00001090: 0a72 0100 0000 2901 7216 0000 0029 017a  .r....).r....).z
+000010a0: 4e25 2870 7936 2973 0a7b 2528 7079 3629  N%(py6)s.{%(py6)
+000010b0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
+000010c0: 3429 730a 7b25 2870 7934 2973 203d 2025  4)s.{%(py4)s = %
+000010d0: 2870 7931 2973 2825 2870 7932 2973 290a  (py1)s(%(py2)s).
+000010e0: 7d29 0a7d 203d 3d20 2528 7079 3929 7372  }).} == %(py9)sr
+000010f0: 1700 0000 7204 0000 0072 4400 0000 2906  ....r....rD...).
+00001100: 7219 0000 0072 1a00 0000 7221 0000 0072  r....r....r!...r
+00001110: 2200 0000 721c 0000 0072 2500 0000 7a0f  "...r....r%...z.
+00001120: 6173 7365 7274 2025 2870 7931 3129 7372  assert %(py11)sr
+00001130: 2600 0000 290d 7209 0000 0072 4200 0000  &...).r....rB...
+00001140: 7243 0000 0072 0400 0000 7217 0000 0072  rC...r....r....r
+00001150: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
+00001160: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00001170: 0000 722e 0000 0029 0972 0a00 0000 7244  ..r....).r....rD
+00001180: 0000 0072 4500 0000 7237 0000 0072 3200  ...rE...r7...r2.
+00001190: 0000 7239 0000 0072 4600 0000 723a 0000  ..r9...rF...r:..
+000011a0: 0072 3b00 0000 720c 0000 0072 0c00 0000  .r;...r....r....
+000011b0: 720d 0000 00da 1a74 6573 745f 6c6f 6164  r......test_load
+000011c0: 5f77 6869 7465 7370 6163 655f 656d 7074  _whitespace_empt
+000011d0: 792f 0000 0073 1800 0000 0001 0a01 0c01  y/...s..........
+000011e0: 1402 0800 0800 0400 0800 0400 9a00 0c00  ................
+000011f0: 0e00 7a26 4b56 4669 6c65 5465 7374 732e  ..z&KVFileTests.
+00001200: 7465 7374 5f6c 6f61 645f 7768 6974 6573  test_load_whites
+00001210: 7061 6365 5f65 6d70 7479 6301 0000 0000  pace_emptyc.....
+00001220: 0000 000a 0000 0009 0000 0043 0000 0073  ...........C...s
+00001230: 0c01 0000 7c00 6a00 6401 1700 7d01 7401  ....|.j.d...}.t.
+00001240: 7c01 6402 8302 8f10 7d02 7c02 a002 6403  |.d.....}.|...d.
+00001250: a101 0100 5700 6400 5100 5200 5800 7403  ....W.d.Q.R.X.t.
+00001260: a004 7405 a101 8f0e 7d03 7406 7c01 8301  ..t.....}.t.|...
+00001270: 0100 5700 6400 5100 5200 5800 6404 7d04  ..W.d.Q.R.X.d.}.
+00001280: 7c03 6a07 7d05 7408 7c05 8301 7d06 7c04  |.j.}.t.|...}.|.
+00001290: 7c06 6b06 7d07 7c07 73f8 7409 a00a 6405  |.k.}.|.s.t...d.
+000012a0: 7c07 6601 6406 7c04 7c06 6602 a104 7409  |.f.d.|.|.f...t.
+000012b0: a00b 7c04 a101 6407 740c a00d a100 6b06  ..|...d.t.....k.
+000012c0: 7398 7409 a00e 7408 a101 72a2 7409 a00b  s.t...t...r.t...
+000012d0: 7408 a101 6e02 6407 6408 740c a00d a100  t...n.d.d.t.....
+000012e0: 6b06 73ba 7409 a00e 7c03 a101 72c4 7409  k.s.t...|...r.t.
+000012f0: a00b 7c03 a101 6e02 6408 7409 a00b 7c05  ..|...n.d.t...|.
+00001300: a101 7409 a00b 7c06 a101 6409 9c05 1600  ..t...|...d.....
+00001310: 7d08 640a 640b 7c08 6901 1600 7d09 740f  }.d.d.|.i...}.t.
+00001320: 7409 a010 7c09 a101 8301 8201 6400 0400  t...|.......d...
+00001330: 7d04 0400 7d07 0400 7d05 7d06 6400 5300  }...}...}.}.d.S.
+00001340: 290c 4e7a 082f 666f 6f2e 796d 6c72 3d00  ).Nz./foo.ymlr=.
+00001350: 0000 7a14 5b6e 6f74 2c20 612c 2064 6963  ..z.[not, a, dic
+00001360: 7469 6f6e 6172 795d 7a10 6e6f 7420 6120  tionary]z.not a 
+00001370: 6469 6374 696f 6e61 7279 2901 da02 696e  dictionary)...in
+00001380: 2901 7a4b 2528 7079 3129 7320 696e 2025  ).zK%(py1)s in %
+00001390: 2870 7938 2973 0a7b 2528 7079 3829 7320  (py8)s.{%(py8)s 
+000013a0: 3d20 2528 7079 3329 7328 2528 7079 3629  = %(py3)s(%(py6)
+000013b0: 730a 7b25 2870 7936 2973 203d 2025 2870  s.{%(py6)s = %(p
+000013c0: 7934 2973 2e76 616c 7565 0a7d 290a 7dda  y4)s.value.}).}.
+000013d0: 0373 7472 da07 6578 6369 6e66 6f29 0572  .str..excinfo).r
+000013e0: 1a00 0000 721b 0000 0072 2200 0000 721c  ....r....r"...r.
+000013f0: 0000 0072 1d00 0000 7a0f 6173 7365 7274  ...r....z.assert
+00001400: 2025 2870 7931 3029 73da 0470 7931 3029   %(py10)s..py10)
+00001410: 1172 0900 0000 7242 0000 0072 4300 0000  .r....rB...rC...
+00001420: 7212 0000 0072 1300 0000 da09 5479 7065  r....r......Type
+00001430: 4572 726f 7272 0400 0000 da05 7661 6c75  Errorr......valu
+00001440: 6572 4e00 0000 7227 0000 0072 2800 0000  erN...r'...r(...
+00001450: 722c 0000 0072 2900 0000 722a 0000 0072  r,...r)...r*...r
+00001460: 2b00 0000 722d 0000 0072 2e00 0000 290a  +...r-...r....).
+00001470: 720a 0000 0072 4400 0000 7245 0000 0072  r....rD...rE...r
+00001480: 4f00 0000 da0b 4070 795f 6173 7365 7274  O.....@py_assert
+00001490: 3072 3200 0000 7246 0000 0072 3100 0000  0r2...rF...r1...
+000014a0: 7235 0000 00da 0c40 7079 5f66 6f72 6d61  r5.....@py_forma
+000014b0: 7431 3172 0c00 0000 720c 0000 0072 0d00  t11r....r....r..
+000014c0: 0000 da18 7465 7374 5f6c 6f61 645f 6e6f  ....test_load_no
+000014d0: 6e5f 6469 6374 696f 6e61 7279 3600 0000  n_dictionary6...
+000014e0: 731c 0000 0000 010a 010c 0114 020c 0112  s...............
+000014f0: 0104 0006 0008 0008 0004 0078 000c 000e  ...........x....
+00001500: 007a 244b 5646 696c 6554 6573 7473 2e74  .z$KVFileTests.t
+00001510: 6573 745f 6c6f 6164 5f6e 6f6e 5f64 6963  est_load_non_dic
+00001520: 7469 6f6e 6172 7963 0100 0000 0000 0000  tionaryc........
+00001530: 0e00 0000 0900 0000 4300 0000 7392 0100  ........C...s...
+00001540: 0074 007c 006a 0164 0117 0083 017d 017c  .t.|.j.d.....}.|
+00001550: 01a0 0264 0264 03a1 0201 0074 037c 0183  ...d.d.....t.|..
+00001560: 017d 0264 047d 037c 027c 036b 027d 047c  .}.d.}.|.|.k.}.|
+00001570: 0473 bc74 04a0 0564 057c 0466 0164 067c  .s.t...d.|.f.d.|
+00001580: 027c 0366 02a1 0464 0774 06a0 07a1 006b  .|.f...d.t.....k
+00001590: 0673 5c74 04a0 0874 03a1 0172 6674 04a0  .s\t...t...rft..
+000015a0: 0974 03a1 016e 0264 0764 0874 06a0 07a1  .t...n.d.d.t....
+000015b0: 006b 0673 7e74 04a0 087c 01a1 0172 8874  .k.s~t...|...r.t
+000015c0: 04a0 097c 01a1 016e 0264 0874 04a0 097c  ...|...n.d.t...|
+000015d0: 02a1 0174 04a0 097c 03a1 0164 099c 0416  ...t...|...d....
+000015e0: 007d 0564 0a64 0b7c 0569 0116 007d 0674  .}.d.d.|.i...}.t
+000015f0: 0a74 04a0 0b7c 06a1 0183 0182 0164 0004  .t...|.......d..
+00001600: 007d 0204 007d 047d 037c 016a 0c7d 0764  .}...}.}.|.j.}.d
+00001610: 027d 0864 0c7d 037c 077c 087c 0383 027d  .}.d.}.|.|.|...}
+00001620: 0964 037d 0a7c 097c 0a6b 027d 0b7c 0b90  .d.}.|.|.k.}.|..
+00001630: 0173 7674 04a0 0564 057c 0b66 0164 0d7c  .svt...d.|.f.d.|
+00001640: 097c 0a66 02a1 0464 0874 06a0 07a1 006b  .|.f...d.t.....k
+00001650: 0690 0173 2074 04a0 087c 01a1 0190 0172  ...s t...|.....r
+00001660: 2a74 04a0 097c 01a1 016e 0264 0874 04a0  *t...|...n.d.t..
+00001670: 097c 07a1 0174 04a0 097c 08a1 0174 04a0  .|...t...|...t..
+00001680: 097c 03a1 0174 04a0 097c 09a1 0174 04a0  .|...t...|...t..
+00001690: 097c 0aa1 0164 0e9c 0616 007d 0c64 0f64  .|...d.....}.d.d
+000016a0: 107c 0c69 0116 007d 0d74 0a74 04a0 0b7c  .|.i...}.t.t...|
+000016b0: 0da1 0183 0182 0164 0004 007d 0704 007d  .......d...}...}
+000016c0: 0804 007d 0304 007d 0904 007d 0b7d 0a64  ...}...}...}.}.d
+000016d0: 0053 0029 114e 7a08 2f66 6f6f 2e79 6d6c  .S.).Nz./foo.yml
+000016e0: 721e 0000 0072 4000 0000 723e 0000 0029  r....r@...r>...)
+000016f0: 0172 1600 0000 2901 7a30 2528 7079 3329  .r....).z0%(py3)
+00001700: 730a 7b25 2870 7933 2973 203d 2025 2870  s.{%(py3)s = %(p
+00001710: 7930 2973 2825 2870 7931 2973 290a 7d20  y0)s(%(py1)s).} 
+00001720: 3d3d 2025 2870 7936 2973 7217 0000 0072  == %(py6)sr....r
+00001730: 1800 0000 2904 7219 0000 0072 1a00 0000  ....).r....r....
+00001740: 721b 0000 0072 1c00 0000 7a0e 6173 7365  r....r....z.asse
+00001750: 7274 2025 2870 7938 2973 721d 0000 0072  rt %(py8)sr....r
+00001760: 3f00 0000 2901 7a53 2528 7079 3829 730a  ?...).zS%(py8)s.
+00001770: 7b25 2870 7938 2973 203d 2025 2870 7932  {%(py8)s = %(py2
+00001780: 2973 0a7b 2528 7079 3229 7320 3d20 2528  )s.{%(py2)s = %(
+00001790: 7079 3029 732e 6765 740a 7d28 2528 7079  py0)s.get.}(%(py
+000017a0: 3429 732c 2025 2870 7936 2973 290a 7d20  4)s, %(py6)s).} 
+000017b0: 3d3d 2025 2870 7931 3129 7329 0672 1900  == %(py11)s).r..
+000017c0: 0000 7221 0000 0072 2200 0000 721c 0000  ..r!...r"...r...
+000017d0: 0072 1d00 0000 7226 0000 007a 0f61 7373  .r....r&...z.ass
+000017e0: 6572 7420 2528 7079 3133 2973 7241 0000  ert %(py13)srA..
+000017f0: 0029 0d72 0400 0000 7209 0000 00da 0c73  .).r....r......s
+00001800: 6574 5f61 6e64 5f73 6176 6572 1700 0000  et_and_saver....
+00001810: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
+00001820: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
+00001830: 0000 0072 2e00 0000 7230 0000 0029 0e72  ...r....r0...).r
+00001840: 0a00 0000 7218 0000 0072 3100 0000 7232  ....r....r1...r2
+00001850: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
+00001860: 0000 7236 0000 0072 3700 0000 7246 0000  ..r6...r7...rF..
+00001870: 0072 4700 0000 7248 0000 0072 3b00 0000  .rG...rH...r;...
+00001880: 7249 0000 0072 0c00 0000 720c 0000 0072  rI...r....r....r
+00001890: 0d00 0000 da17 7465 7374 5f67 6574 5f61  ......test_get_a
+000018a0: 6674 6572 5f73 6574 5f73 616d 653f 0000  fter_set_same?..
+000018b0: 0073 2a00 0000 0001 0e01 0c02 0800 0400  .s*.............
+000018c0: 0800 0400 7000 0c00 0e00 0c01 0600 0400  ....p...........
+000018d0: 0400 0a00 0400 0800 0600 6a00 0c00 0e00  ..........j.....
+000018e0: 7a23 4b56 4669 6c65 5465 7374 732e 7465  z#KVFileTests.te
+000018f0: 7374 5f67 6574 5f61 6674 6572 5f73 6574  st_get_after_set
+00001900: 5f73 616d 6563 0100 0000 0000 0000 0f00  _samec..........
+00001910: 0000 0900 0000 4300 0000 73a0 0100 0074  ......C...s....t
+00001920: 007c 006a 0164 0117 0083 017d 017c 01a0  .|.j.d.....}.|..
+00001930: 0264 0264 03a1 0201 0074 007c 006a 0164  .d.d.....t.|.j.d
+00001940: 0117 0083 017d 0274 037c 0283 017d 0364  .....}.t.|...}.d
+00001950: 047d 047c 037c 046b 027d 057c 0573 ca74  .}.|.|.k.}.|.s.t
+00001960: 04a0 0564 057c 0566 0164 067c 037c 0466  ...d.|.f.d.|.|.f
+00001970: 02a1 0464 0774 06a0 07a1 006b 0673 6a74  ...d.t.....k.sjt
+00001980: 04a0 0874 03a1 0172 7474 04a0 0974 03a1  ...t...rtt...t..
+00001990: 016e 0264 0764 0874 06a0 07a1 006b 0673  .n.d.d.t.....k.s
+000019a0: 8c74 04a0 087c 02a1 0172 9674 04a0 097c  .t...|...r.t...|
+000019b0: 02a1 016e 0264 0874 04a0 097c 03a1 0174  ...n.d.t...|...t
+000019c0: 04a0 097c 04a1 0164 099c 0416 007d 0664  ...|...d.....}.d
+000019d0: 0a64 0b7c 0669 0116 007d 0774 0a74 04a0  .d.|.i...}.t.t..
+000019e0: 0b7c 07a1 0183 0182 0164 0004 007d 0304  .|.......d...}..
+000019f0: 007d 057d 047c 026a 0c7d 0864 027d 0964  .}.}.|.j.}.d.}.d
+00001a00: 0c7d 047c 087c 097c 0483 027d 0a64 037d  .}.|.|.|...}.d.}
+00001a10: 0b7c 0a7c 0b6b 027d 0c7c 0c90 0173 8474  .|.|.k.}.|...s.t
+00001a20: 04a0 0564 057c 0c66 0164 0d7c 0a7c 0b66  ...d.|.f.d.|.|.f
+00001a30: 02a1 0464 0874 06a0 07a1 006b 0690 0173  ...d.t.....k...s
+00001a40: 2e74 04a0 087c 02a1 0190 0172 3874 04a0  .t...|.....r8t..
+00001a50: 097c 02a1 016e 0264 0874 04a0 097c 08a1  .|...n.d.t...|..
+00001a60: 0174 04a0 097c 09a1 0174 04a0 097c 04a1  .t...|...t...|..
+00001a70: 0174 04a0 097c 0aa1 0174 04a0 097c 0ba1  .t...|...t...|..
+00001a80: 0164 0e9c 0616 007d 0d64 0f64 107c 0d69  .d.....}.d.d.|.i
+00001a90: 0116 007d 0e74 0a74 04a0 0b7c 0ea1 0183  ...}.t.t...|....
+00001aa0: 0182 0164 0004 007d 0804 007d 0904 007d  ...d...}...}...}
+00001ab0: 0404 007d 0a04 007d 0c7d 0b64 0053 0029  ...}...}.}.d.S.)
+00001ac0: 114e 7a08 2f66 6f6f 2e79 6d6c 721e 0000  .Nz./foo.ymlr...
+00001ad0: 0072 4000 0000 723e 0000 0029 0172 1600  .r@...r>...).r..
+00001ae0: 0000 2901 7a30 2528 7079 3329 730a 7b25  ..).z0%(py3)s.{%
+00001af0: 2870 7933 2973 203d 2025 2870 7930 2973  (py3)s = %(py0)s
+00001b00: 2825 2870 7931 2973 290a 7d20 3d3d 2025  (%(py1)s).} == %
+00001b10: 2870 7936 2973 7217 0000 00da 046b 7666  (py6)sr......kvf
+00001b20: 3229 0472 1900 0000 721a 0000 0072 1b00  2).r....r....r..
+00001b30: 0000 721c 0000 007a 0e61 7373 6572 7420  ..r....z.assert 
+00001b40: 2528 7079 3829 7372 1d00 0000 723f 0000  %(py8)sr....r?..
+00001b50: 0029 017a 5325 2870 7938 2973 0a7b 2528  .).zS%(py8)s.{%(
+00001b60: 7079 3829 7320 3d20 2528 7079 3229 730a  py8)s = %(py2)s.
+00001b70: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
+00001b80: 2973 2e67 6574 0a7d 2825 2870 7934 2973  )s.get.}(%(py4)s
+00001b90: 2c20 2528 7079 3629 7329 0a7d 203d 3d20  , %(py6)s).} == 
+00001ba0: 2528 7079 3131 2973 2906 7219 0000 0072  %(py11)s).r....r
+00001bb0: 2100 0000 7222 0000 0072 1c00 0000 721d  !...r"...r....r.
+00001bc0: 0000 0072 2600 0000 7a0f 6173 7365 7274  ...r&...z.assert
+00001bd0: 2025 2870 7931 3329 7372 4100 0000 290d   %(py13)srA...).
+00001be0: 7204 0000 0072 0900 0000 7256 0000 0072  r....r....rV...r
+00001bf0: 1700 0000 7227 0000 0072 2800 0000 7229  ....r'...r(...r)
+00001c00: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
+00001c10: 0000 722d 0000 0072 2e00 0000 7230 0000  ..r-...r....r0..
+00001c20: 0029 0f72 0a00 0000 7218 0000 0072 5800  .).r....r....rX.
+00001c30: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
+00001c40: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
+00001c50: 7237 0000 0072 4600 0000 7247 0000 0072  r7...rF...rG...r
+00001c60: 4800 0000 723b 0000 0072 4900 0000 720c  H...r;...rI...r.
+00001c70: 0000 0072 0c00 0000 720d 0000 00da 1574  ...r....r......t
+00001c80: 6573 745f 6c6f 6164 5f73 6563 6f6e 645f  est_load_second_
+00001c90: 7361 6d65 4600 0000 732c 0000 0000 010e  sameF...s,......
+00001ca0: 010c 010e 0208 0004 0008 0004 0070 000c  .............p..
+00001cb0: 000e 000c 0106 0004 0004 000a 0004 0008  ................
+00001cc0: 0006 006a 000c 000e 007a 214b 5646 696c  ...j.....z!KVFil
+00001cd0: 6554 6573 7473 2e74 6573 745f 6c6f 6164  eTests.test_load
+00001ce0: 5f73 6563 6f6e 645f 7361 6d65 6301 0000  _second_samec...
+00001cf0: 0000 0000 000e 0000 0009 0000 0043 0000  .............C..
+00001d00: 0073 9001 0000 7c00 6a00 6401 1700 7d01  .s....|.j.d...}.
+00001d10: 7401 7c01 8301 7d02 7c02 a002 6402 6403  t.|...}.|...d.d.
+00001d20: a102 0100 7c02 a002 6404 6403 a102 0100  ....|...d.d.....
+00001d30: 7403 7c01 8301 8f22 7d03 7c03 a004 a100  t.|...."}.|.....
+00001d40: 7d04 7c03 a005 6405 a101 0100 7406 a007  }.|...d.....t...
+00001d50: 7c03 a101 7d05 5700 6400 5100 5200 5800  |...}.W.d.Q.R.X.
+00001d60: 7408 7c04 8301 7d06 6406 7d07 7c06 7c07  t.|...}.d.}.|.|.
+00001d70: 6b02 7d08 7c08 73fc 7409 a00a 6407 7c08  k.}.|.s.t...d.|.
+00001d80: 6601 6408 7c06 7c07 6602 a104 6409 740b  f.d.|.|.f...d.t.
+00001d90: a00c a100 6b06 739c 7409 a00d 7408 a101  ....k.s.t...t...
+00001da0: 72a6 7409 a00e 7408 a101 6e02 6409 640a  r.t...t...n.d.d.
+00001db0: 740b a00c a100 6b06 73be 7409 a00d 7c04  t.....k.s.t...|.
+00001dc0: a101 72c8 7409 a00e 7c04 a101 6e02 640a  ..r.t...|...n.d.
+00001dd0: 7409 a00e 7c06 a101 7409 a00e 7c07 a101  t...|...t...|...
+00001de0: 640b 9c04 1600 7d09 640c 640d 7c09 6901  d.....}.d.d.|.i.
+00001df0: 1600 7d0a 740f 7409 a010 7c0a a101 8301  ..}.t.t...|.....
+00001e00: 8201 6400 0400 7d06 0400 7d08 7d07 6403  ..d...}...}.}.d.
+00001e10: 6403 640e 9c02 7d06 7c05 7c06 6b02 7d0b  d.d...}.|.|.k.}.
+00001e20: 7c0b 9001 7384 7409 a00a 6407 7c0b 6601  |...s.t...d.|.f.
+00001e30: 640f 7c05 7c06 6602 a104 6410 740b a00c  d.|.|.f...d.t...
+00001e40: a100 6b06 9001 734e 7409 a00d 7c05 a101  ..k...sNt...|...
+00001e50: 9001 7258 7409 a00e 7c05 a101 6e02 6410  ..rXt...|...n.d.
+00001e60: 7409 a00e 7c06 a101 6411 9c02 1600 7d0c  t...|...d.....}.
+00001e70: 6412 6413 7c0c 6901 1600 7d0d 740f 7409  d.d.|.i...}.t.t.
+00001e80: a010 7c0d a101 8301 8201 6400 0400 7d0b  ..|.......d...}.
+00001e90: 7d06 6400 5300 2914 4e7a 082f 666f 6f2e  }.d.S.).Nz./foo.
+00001ea0: 796d 6c72 1e00 0000 7240 0000 00da 0466  ymlr....r@.....f
+00001eb0: 6f6f 3272 0100 0000 e902 0000 0029 0172  oo2r.........).r
+00001ec0: 1600 0000 2901 7a30 2528 7079 3329 730a  ....).z0%(py3)s.
+00001ed0: 7b25 2870 7933 2973 203d 2025 2870 7930  {%(py3)s = %(py0
+00001ee0: 2973 2825 2870 7931 2973 290a 7d20 3d3d  )s(%(py1)s).} ==
+00001ef0: 2025 2870 7936 2973 7217 0000 00da 056c   %(py6)sr......l
+00001f00: 696e 6573 2904 7219 0000 0072 1a00 0000  ines).r....r....
+00001f10: 721b 0000 0072 1c00 0000 7a0e 6173 7365  r....r....z.asse
+00001f20: 7274 2025 2870 7938 2973 721d 0000 0029  rt %(py8)sr....)
+00001f30: 0272 1e00 0000 725a 0000 0029 017a 1225  .r....rZ...).z.%
+00001f40: 2870 7930 2973 203d 3d20 2528 7079 3329  (py0)s == %(py3)
+00001f50: 73da 0464 6174 6129 0272 1900 0000 721b  s..data).r....r.
+00001f60: 0000 007a 0e61 7373 6572 7420 2528 7079  ...z.assert %(py
+00001f70: 3529 7372 2300 0000 2911 7209 0000 0072  5)sr#...).r....r
+00001f80: 0400 0000 7256 0000 0072 4200 0000 da09  ....rV...rB.....
+00001f90: 7265 6164 6c69 6e65 73da 0473 6565 6bda  readlines..seek.
+00001fa0: 0479 616d 6cda 0973 6166 655f 6c6f 6164  .yaml..safe_load
+00001fb0: 7217 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
+00001fc0: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
+00001fd0: 0000 0072 2d00 0000 722e 0000 0029 0e72  ...r-...r....).r
+00001fe0: 0a00 0000 7244 0000 0072 1800 0000 7245  ....rD...r....rE
+00001ff0: 0000 0072 5c00 0000 725d 0000 0072 3100  ...r\...r]...r1.
+00002000: 0000 7232 0000 0072 3300 0000 7234 0000  ..r2...r3...r4..
+00002010: 0072 3500 0000 7236 0000 00da 0b40 7079  .r5...r6.....@py
+00002020: 5f66 6f72 6d61 7434 da0b 4070 795f 666f  _format4..@py_fo
+00002030: 726d 6174 3672 0c00 0000 720c 0000 0072  rmat6r....r....r
+00002040: 0d00 0000 da27 7465 7374 5f73 6574 735f  .....'test_sets_
+00002050: 646f 6e74 5f63 6175 7365 5f61 7070 656e  dont_cause_appen
+00002060: 645f 6475 706c 6963 6174 696f 6e4e 0000  d_duplicationN..
+00002070: 0073 2e00 0000 0001 0a01 0801 0c01 0c02  .s..............
+00002080: 0a01 0801 0a01 1402 0800 0400 0800 0400  ................
+00002090: 7000 0c00 0e00 0c01 0a00 0800 0600 4a00  p.............J.
+000020a0: 0c00 0e00 7a33 4b56 4669 6c65 5465 7374  ....z3KVFileTest
+000020b0: 732e 7465 7374 5f73 6574 735f 646f 6e74  s.test_sets_dont
+000020c0: 5f63 6175 7365 5f61 7070 656e 645f 6475  _cause_append_du
+000020d0: 706c 6963 6174 696f 6e29 0fda 085f 5f6e  plication)...__n
+000020e0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+000020f0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00002100: 0700 0000 7210 0000 0072 1500 0000 723c  ....r....r....r<
+00002110: 0000 0072 4a00 0000 724b 0000 0072 4c00  ...rJ...rK...rL.
+00002120: 0000 7255 0000 0072 5700 0000 7259 0000  ..rU...rW...rY..
+00002130: 0072 6400 0000 da0d 5f5f 636c 6173 7363  .rd.....__classc
+00002140: 656c 6c5f 5f72 0c00 0000 720c 0000 0029  ell__r....r....)
+00002150: 0172 0b00 0000 720d 0000 0072 0500 0000  .r....r....r....
+00002160: 0b00 0000 7316 0000 0008 010c 050c 0408  ....s...........
+00002170: 0408 0608 0908 0708 0708 0908 0708 0872  ...............r
+00002180: 0500 0000 2910 da08 6275 696c 7469 6e73  ....)...builtins
+00002190: 7229 0000 00da 195f 7079 7465 7374 2e61  r)....._pytest.a
+000021a0: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+000021b0: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+000021c0: 7269 7465 7227 0000 0072 0e00 0000 da08  riter'...r......
+000021d0: 7465 6d70 6669 6c65 7202 0000 0072 1200  tempfiler....r..
+000021e0: 0000 7260 0000 00da 0b64 6a61 6e67 6f2e  ..r`.....django.
+000021f0: 7465 7374 7203 0000 00da 1464 6a61 6e67  testr......djang
+00002200: 6f5f 7065 7266 5f72 6563 2e79 616d 6c72  o_perf_rec.yamlr
+00002210: 0400 0000 7205 0000 0072 0c00 0000 720c  ....r....r....r.
+00002220: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+00002230: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
+00002240: 0800 1200 0801 0c02 0801 0801 0c02 0c03  ................
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_db.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_db.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.3.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,351 +1,380 @@
-00000000: 610d 0d0a 4613 445f 6d08 0000 e300 0000  a...F.D_m.......
-00000010: 0000 0000 0000 0000 0000 0000 0008 0000  ................
-00000020: 0040 0000 0073 aa00 0000 6400 6401 6c00  .@...s....d.d.l.
-00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
-00000040: 5a05 0100 6400 6402 6c06 6d07 5a07 6d08  Z...d.d.l.m.Z.m.
-00000050: 5a08 0100 6400 6403 6c09 6d0a 5a0a 6d0b  Z...d.d.l.m.Z.m.
-00000060: 5a0b 6d0c 5a0c 0100 6400 6404 6c0d 6d0e  Z.m.Z...d.d.l.m.
-00000070: 5a0e 0100 7a10 6400 6405 6c0f 6d10 5a10  Z...z.d.d.l.m.Z.
-00000080: 0100 5700 6e1a 0400 6511 7974 0100 0100  ..W.n...e.yt....
-00000090: 0100 6400 6401 6c10 5a10 5900 6e02 3000  ..d.d.l.Z.Y.n.0.
-000000a0: 4700 6406 6407 8400 6407 6507 8303 5a12  G.d.d...d.e...Z.
-000000b0: 4700 6408 6409 8400 6409 6508 8303 5a13  G.d.d...d.e...Z.
-000000c0: 4700 640a 640b 8400 640b 6508 8303 5a14  G.d.d...d.e...Z.
-000000d0: 6401 5300 290c e900 0000 004e 2902 da0e  d.S.)......N)...
-000000e0: 5369 6d70 6c65 5465 7374 4361 7365 da08  SimpleTestCase..
-000000f0: 5465 7374 4361 7365 2903 da0d 416c 6c44  TestCase)...AllD
-00000100: 4252 6563 6f72 6465 72da 0444 424f 70da  BRecorder..DBOp.
-00000110: 0a44 4252 6563 6f72 6465 7229 01da 0972  .DBRecorder)...r
-00000120: 756e 5f71 7565 7279 2901 da04 6d6f 636b  un_query)...mock
-00000130: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000140: 0002 0000 0040 0000 0073 2c00 0000 6500  .....@...s,...e.
-00000150: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000160: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-00000170: 6408 8400 5a06 6409 5300 290a da09 4442  d...Z.d.S.)...DB
-00000180: 4f70 5465 7374 7363 0100 0000 0000 0000  OpTestsc........
-00000190: 0000 0000 0700 0000 0700 0000 4300 0000  ............C...
-000001a0: 7324 0100 0074 0064 0164 0283 027d 017c  s$...t.d.d...}.|
-000001b0: 016a 017d 0264 017d 037c 027c 036b 027d  .j.}.d.}.|.|.k.}
-000001c0: 047c 0473 8874 02a0 0364 037c 0466 0164  .|.s.t...d.|.f.d
-000001d0: 047c 027c 0366 02a1 0464 0574 04a0 05a1  .|.|.f...d.t....
-000001e0: 0076 0073 4a74 02a0 067c 01a1 0172 5474  .v.sJt...|...rTt
-000001f0: 02a0 077c 01a1 016e 0264 0574 02a0 077c  ...|...n.d.t...|
-00000200: 02a1 0174 02a0 077c 03a1 0164 069c 0316  ...t...|...d....
-00000210: 007d 0564 0764 087c 0569 0116 007d 0674  .}.d.d.|.i...}.t
-00000220: 0874 02a0 097c 06a1 0183 0182 0164 0004  .t...|.......d..
-00000230: 007d 0204 007d 047d 037c 016a 0a7d 0264  .}...}.}.|.j.}.d
-00000240: 027d 037c 027c 036b 027d 047c 0490 0173  .}.|.|.k.}.|...s
-00000250: 1474 02a0 0364 037c 0466 0164 097c 027c  .t...d.|.f.d.|.|
-00000260: 0366 02a1 0464 0574 04a0 05a1 0076 0073  .f...d.t.....v.s
-00000270: d674 02a0 067c 01a1 0172 e074 02a0 077c  .t...|...r.t...|
-00000280: 01a1 016e 0264 0574 02a0 077c 02a1 0174  ...n.d.t...|...t
-00000290: 02a0 077c 03a1 0164 069c 0316 007d 0564  ...|...d.....}.d
-000002a0: 0764 087c 0569 0116 007d 0674 0874 02a0  .d.|.i...}.t.t..
-000002b0: 097c 06a1 0183 0182 0164 0004 007d 0204  .|.......d...}..
-000002c0: 007d 047d 0364 0053 0029 0a4e 5a07 6d79  .}.}.d.S.).NZ.my
-000002d0: 616c 6961 73fa 0853 454c 4543 5420 31a9  alias..SELECT 1.
-000002e0: 01fa 023d 3d29 017a 2d25 2870 7932 2973  ...==).z-%(py2)s
-000002f0: 0a7b 2528 7079 3229 7320 3d20 2528 7079  .{%(py2)s = %(py
-00000300: 3029 732e 616c 6961 730a 7d20 3d3d 2025  0)s.alias.} == %
-00000310: 2870 7935 2973 da02 6f70 a903 da03 7079  (py5)s..op....py
-00000320: 30da 0370 7932 da03 7079 35fa 0e61 7373  0..py2..py5..ass
-00000330: 6572 7420 2528 7079 3729 73da 0370 7937  ert %(py7)s..py7
-00000340: 2901 7a2d 2528 7079 3229 730a 7b25 2870  ).z-%(py2)s.{%(p
-00000350: 7932 2973 203d 2025 2870 7930 2973 2e71  y2)s = %(py0)s.q
-00000360: 7565 7279 0a7d 203d 3d20 2528 7079 3529  uery.} == %(py5)
-00000370: 7329 0b72 0500 0000 da05 616c 6961 73da  s).r......alias.
-00000380: 0a40 7079 7465 7374 5f61 72da 115f 6361  .@pytest_ar.._ca
-00000390: 6c6c 5f72 6570 7263 6f6d 7061 7265 da0c  ll_reprcompare..
-000003a0: 4070 795f 6275 696c 7469 6e73 da06 6c6f  @py_builtins..lo
-000003b0: 6361 6c73 da18 5f73 686f 756c 645f 7265  cals.._should_re
-000003c0: 7072 5f67 6c6f 6261 6c5f 6e61 6d65 da09  pr_global_name..
-000003d0: 5f73 6166 6572 6570 72da 0e41 7373 6572  _saferepr..Asser
-000003e0: 7469 6f6e 4572 726f 72da 135f 666f 726d  tionError.._form
-000003f0: 6174 5f65 7870 6c61 6e61 7469 6f6e da05  at_explanation..
-00000400: 7175 6572 7929 07da 0473 656c 6672 0d00  query)...selfr..
-00000410: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
-00000420: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
-00000430: 795f 6173 7365 7274 33da 0b40 7079 5f66  y_assert3..@py_f
-00000440: 6f72 6d61 7436 da0b 4070 795f 666f 726d  ormat6..@py_form
-00000450: 6174 38a9 0072 2400 0000 fa41 2f55 7365  at8..r$....A/Use
-00000460: 7273 2f63 6861 696e 7a2f 446f 6375 6d65  rs/chainz/Docume
-00000470: 6e74 732f 5072 6f6a 6563 7473 2f64 6a61  nts/Projects/dja
-00000480: 6e67 6f2d 7065 7266 2d72 6563 2f74 6573  ngo-perf-rec/tes
-00000490: 7473 2f74 6573 745f 6462 2e70 79da 0b74  ts/test_db.py..t
-000004a0: 6573 745f 6372 6561 7465 0d00 0000 7306  est_create....s.
-000004b0: 0000 0000 010a 018a 017a 1544 424f 7054  .........z.DBOpT
-000004c0: 6573 7473 2e74 6573 745f 6372 6561 7465  ests.test_create
-000004d0: 6301 0000 0000 0000 0000 0000 000a 0000  c...............
-000004e0: 000b 0000 0043 0000 0073 fa00 0000 6401  .....C...s....d.
-000004f0: 7d01 6402 7d02 7400 7c01 7c02 8302 7d03  }.d.}.t.|.|...}.
-00000500: 6401 7d04 6402 7d05 7400 7c04 7c05 8302  d.}.d.}.t.|.|...
-00000510: 7d06 7c03 7c06 6b02 7d07 7c07 73da 7401  }.|.|.k.}.|.s.t.
-00000520: a002 6403 7c07 6601 6404 7c03 7c06 6602  ..d.|.f.d.|.|.f.
-00000530: a104 6405 7403 a004 a100 7600 735a 7401  ..d.t.....v.sZt.
-00000540: a005 7400 a101 7264 7401 a006 7400 a101  ..t...rdt...t...
-00000550: 6e02 6405 7401 a006 7c01 a101 7401 a006  n.d.t...|...t...
-00000560: 7c02 a101 7401 a006 7c03 a101 6405 7403  |...t...|...d.t.
-00000570: a004 a100 7600 7394 7401 a005 7400 a101  ....v.s.t...t...
-00000580: 729e 7401 a006 7400 a101 6e02 6405 7401  r.t...t...n.d.t.
-00000590: a006 7c04 a101 7401 a006 7c05 a101 7401  ..|...t...|...t.
-000005a0: a006 7c06 a101 6406 9c08 1600 7d08 6407  ..|...d.....}.d.
-000005b0: 6408 7c08 6901 1600 7d09 7407 7401 a008  d.|.i...}.t.t...
-000005c0: 7c09 a101 8301 8201 6400 0400 7d01 0400  |.......d...}...
-000005d0: 7d02 0400 7d03 0400 7d07 0400 7d04 0400  }...}...}...}...
-000005e0: 7d05 7d06 6400 5300 2909 4eda 0366 6f6f  }.}.d.S.).N..foo
-000005f0: da03 6261 7272 0b00 0000 2901 7a64 2528  ..barr....).zd%(
-00000600: 7079 3629 730a 7b25 2870 7936 2973 203d  py6)s.{%(py6)s =
-00000610: 2025 2870 7930 2973 2825 2870 7932 2973   %(py0)s(%(py2)s
-00000620: 2c20 2528 7079 3429 7329 0a7d 203d 3d20  , %(py4)s).} == 
-00000630: 2528 7079 3134 2973 0a7b 2528 7079 3134  %(py14)s.{%(py14
-00000640: 2973 203d 2025 2870 7938 2973 2825 2870  )s = %(py8)s(%(p
-00000650: 7931 3029 732c 2025 2870 7931 3229 7329  y10)s, %(py12)s)
-00000660: 0a7d 7205 0000 00a9 0872 0f00 0000 7210  .}r......r....r.
-00000670: 0000 00da 0370 7934 da03 7079 36da 0370  .....py4..py6..p
-00000680: 7938 da04 7079 3130 da04 7079 3132 da04  y8..py10..py12..
-00000690: 7079 3134 fa0f 6173 7365 7274 2025 2870  py14..assert %(p
-000006a0: 7931 3629 73da 0470 7931 36a9 0972 0500  y16)s..py16..r..
-000006b0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-000006c0: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-000006d0: 721b 0000 0072 1c00 0000 a90a 721e 0000  r....r......r...
-000006e0: 0072 1f00 0000 7221 0000 00da 0b40 7079  .r....r!.....@py
-000006f0: 5f61 7373 6572 7435 da0b 4070 795f 6173  _assert5..@py_as
-00000700: 7365 7274 39da 0c40 7079 5f61 7373 6572  sert9..@py_asser
-00000710: 7431 31da 0c40 7079 5f61 7373 6572 7431  t11..@py_assert1
-00000720: 33da 0b40 7079 5f61 7373 6572 7437 5a0c  3..@py_assert7Z.
-00000730: 4070 795f 666f 726d 6174 3135 5a0c 4070  @py_format15Z.@p
-00000740: 795f 666f 726d 6174 3137 7224 0000 0072  y_format17r$...r
-00000750: 2400 0000 7225 0000 00da 0a74 6573 745f  $...r%.....test_
-00000760: 6571 7561 6c12 0000 0073 0200 0000 0001  equal....s......
-00000770: 7a14 4442 4f70 5465 7374 732e 7465 7374  z.DBOpTests.test
-00000780: 5f65 7175 616c 6301 0000 0000 0000 0000  _equalc.........
-00000790: 0000 000a 0000 000b 0000 0043 0000 0073  ...........C...s
-000007a0: fa00 0000 6401 7d01 6402 7d02 7400 7c01  ....d.}.d.}.t.|.
-000007b0: 7c02 8302 7d03 6403 7d04 6402 7d05 7400  |...}.d.}.d.}.t.
-000007c0: 7c04 7c05 8302 7d06 7c03 7c06 6b03 7d07  |.|...}.|.|.k.}.
-000007d0: 7c07 73da 7401 a002 6404 7c07 6601 6405  |.s.t...d.|.f.d.
-000007e0: 7c03 7c06 6602 a104 6406 7403 a004 a100  |.|.f...d.t.....
-000007f0: 7600 735a 7401 a005 7400 a101 7264 7401  v.sZt...t...rdt.
-00000800: a006 7400 a101 6e02 6406 7401 a006 7c01  ..t...n.d.t...|.
-00000810: a101 7401 a006 7c02 a101 7401 a006 7c03  ..t...|...t...|.
-00000820: a101 6406 7403 a004 a100 7600 7394 7401  ..d.t.....v.s.t.
-00000830: a005 7400 a101 729e 7401 a006 7400 a101  ..t...r.t...t...
-00000840: 6e02 6406 7401 a006 7c04 a101 7401 a006  n.d.t...|...t...
-00000850: 7c05 a101 7401 a006 7c06 a101 6407 9c08  |...t...|...d...
-00000860: 1600 7d08 6408 6409 7c08 6901 1600 7d09  ..}.d.d.|.i...}.
-00000870: 7407 7401 a008 7c09 a101 8301 8201 6400  t.t...|.......d.
-00000880: 0400 7d01 0400 7d02 0400 7d03 0400 7d07  ..}...}...}...}.
-00000890: 0400 7d04 0400 7d05 7d06 6400 5300 a90a  ..}...}.}.d.S...
-000008a0: 4e72 2700 0000 7228 0000 00da 0362 617a  Nr'...r(.....baz
-000008b0: 2901 fa02 213d 2901 7a64 2528 7079 3629  )...!=).zd%(py6)
-000008c0: 730a 7b25 2870 7936 2973 203d 2025 2870  s.{%(py6)s = %(p
-000008d0: 7930 2973 2825 2870 7932 2973 2c20 2528  y0)s(%(py2)s, %(
-000008e0: 7079 3429 7329 0a7d 2021 3d20 2528 7079  py4)s).} != %(py
-000008f0: 3134 2973 0a7b 2528 7079 3134 2973 203d  14)s.{%(py14)s =
-00000900: 2025 2870 7938 2973 2825 2870 7931 3029   %(py8)s(%(py10)
-00000910: 732c 2025 2870 7931 3229 7329 0a7d 7205  s, %(py12)s).}r.
-00000920: 0000 0072 2900 0000 7230 0000 0072 3100  ...r)...r0...r1.
-00000930: 0000 7232 0000 0072 3300 0000 7224 0000  ..r2...r3...r$..
-00000940: 0072 2400 0000 7225 0000 00da 1474 6573  .r$...r%.....tes
-00000950: 745f 6e6f 745f 6571 7561 6c5f 616c 6961  t_not_equal_alia
-00000960: 7315 0000 0073 0200 0000 0001 7a1e 4442  s....s......z.DB
-00000970: 4f70 5465 7374 732e 7465 7374 5f6e 6f74  OpTests.test_not
-00000980: 5f65 7175 616c 5f61 6c69 6173 6301 0000  _equal_aliasc...
-00000990: 0000 0000 0000 0000 000a 0000 000b 0000  ................
-000009a0: 0043 0000 0073 fa00 0000 6401 7d01 6402  .C...s....d.}.d.
-000009b0: 7d02 7400 7c01 7c02 8302 7d03 6401 7d04  }.t.|.|...}.d.}.
-000009c0: 6403 7d05 7400 7c04 7c05 8302 7d06 7c03  d.}.t.|.|...}.|.
-000009d0: 7c06 6b03 7d07 7c07 73da 7401 a002 6404  |.k.}.|.s.t...d.
-000009e0: 7c07 6601 6405 7c03 7c06 6602 a104 6406  |.f.d.|.|.f...d.
-000009f0: 7403 a004 a100 7600 735a 7401 a005 7400  t.....v.sZt...t.
-00000a00: a101 7264 7401 a006 7400 a101 6e02 6406  ..rdt...t...n.d.
-00000a10: 7401 a006 7c01 a101 7401 a006 7c02 a101  t...|...t...|...
-00000a20: 7401 a006 7c03 a101 6406 7403 a004 a100  t...|...d.t.....
-00000a30: 7600 7394 7401 a005 7400 a101 729e 7401  v.s.t...t...r.t.
-00000a40: a006 7400 a101 6e02 6406 7401 a006 7c04  ..t...n.d.t...|.
-00000a50: a101 7401 a006 7c05 a101 7401 a006 7c06  ..t...|...t...|.
-00000a60: a101 6407 9c08 1600 7d08 6408 6409 7c08  ..d.....}.d.d.|.
-00000a70: 6901 1600 7d09 7407 7401 a008 7c09 a101  i...}.t.t...|...
-00000a80: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-00000a90: 7d03 0400 7d07 0400 7d04 0400 7d05 7d06  }...}...}...}.}.
-00000aa0: 6400 5300 723a 0000 0072 3200 0000 7233  d.S.r:...r2...r3
-00000ab0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00000ac0: 0000 da12 7465 7374 5f6e 6f74 5f65 7175  ....test_not_equ
-00000ad0: 616c 5f73 716c 1800 0000 7302 0000 0000  al_sql....s.....
-00000ae0: 017a 1c44 424f 7054 6573 7473 2e74 6573  .z.DBOpTests.tes
-00000af0: 745f 6e6f 745f 6571 7561 6c5f 7371 6c4e  t_not_equal_sqlN
-00000b00: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000b10: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000b20: 6e61 6d65 5f5f 7226 0000 0072 3900 0000  name__r&...r9...
-00000b30: 723d 0000 0072 3e00 0000 7224 0000 0072  r=...r>...r$...r
-00000b40: 2400 0000 7224 0000 0072 2500 0000 7209  $...r$...r%...r.
-00000b50: 0000 000c 0000 0073 0800 0000 0801 0805  .......s........
-00000b60: 0803 0803 7209 0000 0063 0000 0000 0000  ....r....c......
-00000b70: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00000b80: 0000 7330 0000 0065 005a 0164 005a 0264  ..s0...e.Z.d.Z.d
-00000b90: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
-00000ba0: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-00000bb0: 005a 0764 0a53 0029 0bda 0f44 4252 6563  .Z.d.S.)...DBRec
-00000bc0: 6f72 6465 7254 6573 7473 a903 da07 6465  orderTests....de
-00000bd0: 6661 756c 74da 0673 6563 6f6e 64da 0772  fault..second..r
-00000be0: 6570 6c69 6361 6301 0000 0000 0000 0000  eplicac.........
-00000bf0: 0000 0002 0000 0008 0000 0043 0000 0073  ...........C...s
-00000c00: 5000 0000 7400 a001 a100 7d01 7402 6401  P...t.....}.t.d.
-00000c10: 7c01 8302 8f1a 0100 7403 6401 6402 8302  |.......t.d.d...
-00000c20: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
-00000c30: 3100 7332 3000 0100 0100 0100 5900 0100  1.s20.......Y...
-00000c40: 7c01 a004 7405 6401 6403 8302 a101 0100  |...t.d.d.......
-00000c50: 6400 5300 2904 4e72 4400 0000 720a 0000  d.S.).NrD...r...
-00000c60: 00fa 0853 454c 4543 5420 23a9 0672 0800  ...SELECT #..r..
-00000c70: 0000 da04 4d6f 636b 7206 0000 0072 0700  ....Mockr....r..
-00000c80: 0000 da17 6173 7365 7274 5f63 616c 6c65  ....assert_calle
-00000c90: 645f 6f6e 6365 5f77 6974 6872 0500 0000  d_once_withr....
-00000ca0: a902 721e 0000 00da 0863 616c 6c62 6163  ..r......callbac
-00000cb0: 6b72 2400 0000 7224 0000 0072 2500 0000  kr$...r$...r%...
-00000cc0: da0c 7465 7374 5f64 6566 6175 6c74 1f00  ..test_default..
-00000cd0: 0000 7308 0000 0000 0108 010c 0128 017a  ..s..........(.z
-00000ce0: 1c44 4252 6563 6f72 6465 7254 6573 7473  .DBRecorderTests
-00000cf0: 2e74 6573 745f 6465 6661 756c 7463 0100  .test_defaultc..
-00000d00: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00000d10: 0000 4300 0000 7350 0000 0074 00a0 01a1  ..C...sP...t....
-00000d20: 007d 0174 0264 017c 0183 028f 1a01 0074  .}.t.d.|.......t
-00000d30: 0364 0164 0283 0201 0057 0064 0004 0004  .d.d.....W.d....
-00000d40: 0083 0301 006e 1031 0073 3230 0001 0001  .....n.1.s20....
-00000d50: 0001 0059 0001 007c 01a0 0474 0564 0164  ...Y...|...t.d.d
-00000d60: 0383 02a1 0101 0064 0053 0029 044e 7245  .......d.S.).NrE
-00000d70: 0000 0072 0a00 0000 7247 0000 0072 4800  ...r....rG...rH.
-00000d80: 0000 724b 0000 0072 2400 0000 7224 0000  ..rK...r$...r$..
-00000d90: 0072 2500 0000 da0e 7465 7374 5f73 6563  .r%.....test_sec
-00000da0: 6f6e 6461 7279 2500 0000 7308 0000 0000  ondary%...s.....
-00000db0: 0108 010c 0128 017a 1e44 4252 6563 6f72  .....(.z.DBRecor
-00000dc0: 6465 7254 6573 7473 2e74 6573 745f 7365  derTests.test_se
-00000dd0: 636f 6e64 6172 7963 0100 0000 0000 0000  condaryc........
-00000de0: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
-00000df0: 7350 0000 0074 00a0 01a1 007d 0174 0264  sP...t.....}.t.d
-00000e00: 017c 0183 028f 1a01 0074 0364 0164 0283  .|.......t.d.d..
-00000e10: 0201 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000e20: 1031 0073 3230 0001 0001 0001 0059 0001  .1.s20.......Y..
-00000e30: 007c 01a0 0474 0564 0164 0383 02a1 0101  .|...t.d.d......
-00000e40: 0064 0053 0029 044e 7246 0000 0072 0a00  .d.S.).NrF...r..
-00000e50: 0000 7247 0000 0072 4800 0000 724b 0000  ..rG...rH...rK..
-00000e60: 0072 2400 0000 7224 0000 0072 2500 0000  .r$...r$...r%...
-00000e70: da0c 7465 7374 5f72 6570 6c69 6361 2b00  ..test_replica+.
-00000e80: 0000 7308 0000 0000 0108 010c 0128 017a  ..s..........(.z
-00000e90: 1c44 4252 6563 6f72 6465 7254 6573 7473  .DBRecorderTests
-00000ea0: 2e74 6573 745f 7265 706c 6963 6163 0100  .test_replicac..
-00000eb0: 0000 0000 0000 0000 0000 0800 0000 0800  ................
-00000ec0: 0000 4300 0000 7300 0100 0074 00a0 01a1  ..C...s....t....
-00000ed0: 007d 0174 0264 017c 0183 028f 1a01 0074  .}.t.d.|.......t
-00000ee0: 0364 0264 0383 0201 0057 0064 0004 0004  .d.d.....W.d....
-00000ef0: 0083 0301 006e 1031 0073 3230 0001 0001  .....n.1.s20....
-00000f00: 0001 0059 0001 007c 016a 047d 0274 057c  ...Y...|.j.}.t.|
-00000f10: 0283 017d 0364 047d 047c 037c 046b 027d  ...}.d.}.|.|.k.}
-00000f20: 057c 0573 ec74 06a0 0764 057c 0566 0164  .|.s.t...d.|.f.d
-00000f30: 067c 037c 0466 02a1 0464 0774 08a0 09a1  .|.|.f...d.t....
-00000f40: 0076 0073 8474 06a0 0a74 05a1 0172 8e74  .v.s.t...t...r.t
-00000f50: 06a0 0b74 05a1 016e 0264 0764 0874 08a0  ...t...n.d.d.t..
-00000f60: 09a1 0076 0073 a674 06a0 0a7c 01a1 0172  ...v.s.t...|...r
-00000f70: b074 06a0 0b7c 01a1 016e 0264 0874 06a0  .t...|...n.d.t..
-00000f80: 0b7c 02a1 0174 06a0 0b7c 03a1 0174 06a0  .|...t...|...t..
-00000f90: 0b7c 04a1 0164 099c 0516 007d 0664 0a64  .|...d.....}.d.d
-00000fa0: 0b7c 0669 0116 007d 0774 0c74 06a0 0d7c  .|.i...}.t.t...|
-00000fb0: 07a1 0183 0182 0164 0004 007d 0204 007d  .......d...}...}
-00000fc0: 0304 007d 057d 0464 0053 0029 0c4e 7245  ...}.}.d.S.).NrE
-00000fd0: 0000 0072 4400 0000 720a 0000 0072 0100  ...rD...r....r..
-00000fe0: 0000 720b 0000 0029 017a 5025 2870 7935  ..r....).zP%(py5
-00000ff0: 2973 0a7b 2528 7079 3529 7320 3d20 2528  )s.{%(py5)s = %(
-00001000: 7079 3029 7328 2528 7079 3329 730a 7b25  py0)s(%(py3)s.{%
-00001010: 2870 7933 2973 203d 2025 2870 7931 2973  (py3)s = %(py1)s
-00001020: 2e6d 6f63 6b5f 6361 6c6c 730a 7d29 0a7d  .mock_calls.}).}
-00001030: 203d 3d20 2528 7079 3829 73da 036c 656e   == %(py8)s..len
-00001040: 724c 0000 0029 0572 0f00 0000 da03 7079  rL...).r......py
-00001050: 31da 0370 7933 7211 0000 0072 2c00 0000  1..py3r....r,...
-00001060: 7a0f 6173 7365 7274 2025 2870 7931 3029  z.assert %(py10)
-00001070: 7372 2d00 0000 290e 7208 0000 0072 4900  sr-...).r....rI.
-00001080: 0000 7206 0000 0072 0700 0000 da0a 6d6f  ..r....r......mo
-00001090: 636b 5f63 616c 6c73 7250 0000 0072 1500  ck_callsrP...r..
-000010a0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-000010b0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000010c0: 721c 0000 0029 0872 1e00 0000 724c 0000  r....).r....rL..
-000010d0: 00da 0b40 7079 5f61 7373 6572 7432 7220  ...@py_assert2r 
-000010e0: 0000 0072 3800 0000 da0b 4070 795f 6173  ...r8.....@py_as
-000010f0: 7365 7274 36da 0b40 7079 5f66 6f72 6d61  sert6..@py_forma
-00001100: 7439 da0c 4070 795f 666f 726d 6174 3131  t9..@py_format11
-00001110: 7224 0000 0072 2400 0000 7225 0000 00da  r$...r$...r%....
-00001120: 2374 6573 745f 7365 636f 6e64 6172 795f  #test_secondary_
-00001130: 6465 6661 756c 745f 6e6f 745f 7265 636f  default_not_reco
-00001140: 7264 6564 3100 0000 7308 0000 0000 0108  rded1...s.......
-00001150: 010c 0128 017a 3344 4252 6563 6f72 6465  ...(.z3DBRecorde
-00001160: 7254 6573 7473 2e74 6573 745f 7365 636f  rTests.test_seco
-00001170: 6e64 6172 795f 6465 6661 756c 745f 6e6f  ndary_default_no
-00001180: 745f 7265 636f 7264 6564 4e29 0872 3f00  t_recordedN).r?.
-00001190: 0000 7240 0000 0072 4100 0000 da09 6461  ..r@...rA.....da
-000011a0: 7461 6261 7365 7372 4d00 0000 724e 0000  tabasesrM...rN..
-000011b0: 0072 4f00 0000 7258 0000 0072 2400 0000  .rO...rX...r$...
-000011c0: 7224 0000 0072 2400 0000 7225 0000 0072  r$...r$...r%...r
-000011d0: 4200 0000 1c00 0000 730a 0000 0008 0104  B.......s.......
-000011e0: 0208 0608 0608 0672 4200 0000 6300 0000  .......rB...c...
-000011f0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00001200: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00001210: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
-00001220: 5300 2905 da12 416c 6c44 4252 6563 6f72  S.)...AllDBRecor
-00001230: 6465 7254 6573 7473 7243 0000 0063 0100  derTestsrC...c..
-00001240: 0000 0000 0000 0000 0000 0700 0000 0800  ................
-00001250: 0000 4300 0000 7306 0100 0074 00a0 01a1  ..C...s....t....
-00001260: 007d 0174 027c 0183 018f 2e01 0074 0364  .}.t.|.......t.d
-00001270: 0164 0283 0201 0074 0364 0364 0483 0201  .d.....t.d.d....
-00001280: 0074 0364 0564 0683 0201 0057 0064 0004  .t.d.d.....W.d..
-00001290: 0004 0083 0301 006e 1031 0073 4430 0001  .......n.1.sD0..
-000012a0: 0001 0001 0059 0001 007c 016a 047d 0274  .....Y...|.j.}.t
-000012b0: 00a0 0574 0664 0164 0783 02a1 0174 00a0  ...t.d.d.....t..
-000012c0: 0574 0664 0364 0783 02a1 0174 00a0 0574  .t.d.d.....t...t
-000012d0: 0664 0564 0783 02a1 0167 037d 037c 027c  .d.d.....g.}.|.|
-000012e0: 036b 027d 047c 0473 f674 07a0 0864 087c  .k.}.|.s.t...d.|
-000012f0: 0466 0164 097c 027c 0366 02a1 0464 0a74  .f.d.|.|.f...d.t
-00001300: 09a0 0aa1 0076 0073 b874 07a0 0b7c 01a1  .....v.s.t...|..
-00001310: 0172 c274 07a0 0c7c 01a1 016e 0264 0a74  .r.t...|...n.d.t
-00001320: 07a0 0c7c 02a1 0174 07a0 0c7c 03a1 0164  ...|...t...|...d
-00001330: 0b9c 0316 007d 0564 0c64 0d7c 0569 0116  .....}.d.d.|.i..
-00001340: 007d 0674 0d74 07a0 0e7c 06a1 0183 0182  .}.t.t...|......
-00001350: 0164 0004 007d 0204 007d 047d 0364 0053  .d...}...}.}.d.S
-00001360: 0029 0e4e 7246 0000 0072 0a00 0000 7244  .).NrF...r....rD
-00001370: 0000 007a 0853 454c 4543 5420 3272 4500  ...z.SELECT 2rE.
-00001380: 0000 7a08 5345 4c45 4354 2033 7247 0000  ..z.SELECT 3rG..
-00001390: 0072 0b00 0000 2901 7a32 2528 7079 3229  .r....).z2%(py2)
-000013a0: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
-000013b0: 7930 2973 2e6d 6f63 6b5f 6361 6c6c 730a  y0)s.mock_calls.
-000013c0: 7d20 3d3d 2025 2870 7935 2973 724c 0000  } == %(py5)srL..
-000013d0: 0072 0e00 0000 7212 0000 0072 1300 0000  .r....r....r....
-000013e0: 290f 7208 0000 0072 4900 0000 7204 0000  ).r....rI...r...
-000013f0: 0072 0700 0000 7253 0000 00da 0463 616c  .r....rS.....cal
-00001400: 6c72 0500 0000 7215 0000 0072 1600 0000  lr....r....r....
-00001410: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00001420: 1a00 0000 721b 0000 0072 1c00 0000 2907  ....r....r....).
-00001430: 721e 0000 0072 4c00 0000 721f 0000 0072  r....rL...r....r
-00001440: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-00001450: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
-00001460: 0000 da10 7465 7374 5f72 6563 6f72 6473  ....test_records
-00001470: 5f61 6c6c 3b00 0000 730c 0000 0000 0108  _all;...s.......
-00001480: 010a 010a 010a 0128 027a 2341 6c6c 4442  .......(.z#AllDB
-00001490: 5265 636f 7264 6572 5465 7374 732e 7465  RecorderTests.te
-000014a0: 7374 5f72 6563 6f72 6473 5f61 6c6c 4e29  st_records_allN)
-000014b0: 0572 3f00 0000 7240 0000 0072 4100 0000  .r?...r@...rA...
-000014c0: 7259 0000 0072 5c00 0000 7224 0000 0072  rY...r\...r$...r
-000014d0: 2400 0000 7224 0000 0072 2500 0000 725a  $...r$...r%...rZ
-000014e0: 0000 0038 0000 0073 0400 0000 0801 0402  ...8...s........
-000014f0: 725a 0000 0029 15da 0862 7569 6c74 696e  rZ...)...builtin
-00001500: 7372 1700 0000 da19 5f70 7974 6573 742e  sr......_pytest.
-00001510: 6173 7365 7274 696f 6e2e 7265 7772 6974  assertion.rewrit
-00001520: 65da 0961 7373 6572 7469 6f6e da07 7265  e..assertion..re
-00001530: 7772 6974 6572 1500 0000 da0b 646a 616e  writer......djan
-00001540: 676f 2e74 6573 7472 0200 0000 7203 0000  go.testr....r...
-00001550: 00da 1264 6a61 6e67 6f5f 7065 7266 5f72  ...django_perf_r
-00001560: 6563 2e64 6272 0400 0000 7205 0000 0072  ec.dbr....r....r
-00001570: 0600 0000 da0b 7465 7374 732e 7574 696c  ......tests.util
-00001580: 7372 0700 0000 da08 756e 6974 7465 7374  sr......unittest
-00001590: 7208 0000 00da 0b49 6d70 6f72 7445 7272  r......ImportErr
-000015a0: 6f72 7209 0000 0072 4200 0000 725a 0000  orr....rB...rZ..
-000015b0: 0072 2400 0000 7224 0000 0072 2400 0000  .r$...r$...r$...
-000015c0: 7225 0000 00da 083c 6d6f 6475 6c65 3e01  r%.....<module>.
-000015d0: 0000 0073 1200 0000 2a02 1401 0c02 0201  ...s....*.......
-000015e0: 1001 0c01 0e03 1010 101c                 ..........
+00000000: 420d 0d0a 914c 075d bc04 0000 e300 0000  B....L.]........
+00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+00000020: 0073 5a00 0000 6400 6401 6c00 5a01 6400  .sZ...d.d.l.Z.d.
+00000030: 6401 6c02 6d03 0200 0100 6d04 5a05 0100  d.l.m.....m.Z...
+00000040: 6400 6402 6c06 6d07 5a07 0100 6400 6403  d.d.l.m.Z...d.d.
+00000050: 6c08 6d09 5a09 6d0a 5a0a 0100 4700 6404  l.m.Z.m.Z...G.d.
+00000060: 6405 8400 6405 6507 8303 5a0b 4700 6406  d...d.e...Z.G.d.
+00000070: 6407 8400 6407 6507 8303 5a0c 6401 5300  d...d.e...Z.d.S.
+00000080: 2908 e900 0000 004e 2901 da0e 5369 6d70  )......N)...Simp
+00000090: 6c65 5465 7374 4361 7365 2902 da0c 6375  leTestCase)...cu
+000000a0: 7272 656e 745f 7465 7374 da0c 736f 7274  rrent_test..sort
+000000b0: 6564 5f6e 616d 6573 6300 0000 0000 0000  ed_namesc.......
+000000c0: 0000 0000 0002 0000 0040 0000 0073 2400  .........@...s$.
+000000d0: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
+000000e0: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
+000000f0: 5a05 6407 5300 2908 da10 4375 7272 656e  Z.d.S.)...Curren
+00000100: 7454 6573 7454 6573 7473 6301 0000 0000  tTestTestsc.....
+00000110: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
+00000120: c201 0000 7400 8300 7d01 7c01 6a01 7d02  ....t...}.|.j.}.
+00000130: 7c02 7402 6b02 7d03 7c03 739a 7403 a004  |.t.k.}.|.s.t...
+00000140: 6401 7c03 6601 6402 7c02 7402 6602 a104  d.|.f.d.|.t.f...
+00000150: 6403 7405 a006 a100 6b06 7342 7403 a007  d.t.....k.sBt...
+00000160: 7c01 a101 724c 7403 a008 7c01 a101 6e02  |...rLt...|...n.
+00000170: 6403 7403 a008 7c02 a101 6404 7405 a006  d.t...|...d.t...
+00000180: a100 6b06 736c 7403 a007 7402 a101 7276  ..k.slt...t...rv
+00000190: 7403 a008 7402 a101 6e02 6404 6405 9c03  t...t...n.d.d...
+000001a0: 1600 7d04 6406 6407 7c04 6901 1600 7d05  ..}.d.d.|.i...}.
+000001b0: 7409 7403 a00a 7c05 a101 8301 8201 6400  t.t...|.......d.
+000001c0: 0400 7d02 7d03 7c01 6a0b 7d02 6408 7d06  ..}.}.|.j.}.d.}.
+000001d0: 7c02 7c06 6b02 7d03 7c03 9001 7322 7403  |.|.k.}.|...s"t.
+000001e0: a004 6401 7c03 6601 6409 7c02 7c06 6602  ..d.|.f.d.|.|.f.
+000001f0: a104 6403 7405 a006 a100 6b06 73e4 7403  ..d.t.....k.s.t.
+00000200: a007 7c01 a101 72ee 7403 a008 7c01 a101  ..|...r.t...|...
+00000210: 6e02 6403 7403 a008 7c02 a101 7403 a008  n.d.t...|...t...
+00000220: 7c06 a101 640a 9c03 1600 7d07 640b 640c  |...d.....}.d.d.
+00000230: 7c07 6901 1600 7d08 7409 7403 a00a 7c08  |.i...}.t.t...|.
+00000240: a101 8301 8201 6400 0400 7d02 0400 7d03  ......d...}...}.
+00000250: 7d06 7c01 6a0c 7d02 640d 7d06 7c02 7c06  }.|.j.}.d.}.|.|.
+00000260: 6b02 7d03 7c03 9001 73b2 7403 a004 6401  k.}.|...s.t...d.
+00000270: 7c03 6601 640e 7c02 7c06 6602 a104 6403  |.f.d.|.|.f...d.
+00000280: 7405 a006 a100 6b06 9001 7374 7403 a007  t.....k...stt...
+00000290: 7c01 a101 9001 727e 7403 a008 7c01 a101  |.....r~t...|...
+000002a0: 6e02 6403 7403 a008 7c02 a101 7403 a008  n.d.t...|...t...
+000002b0: 7c06 a101 640a 9c03 1600 7d07 640b 640c  |...d.....}.d.d.
+000002c0: 7c07 6901 1600 7d08 7409 7403 a00a 7c08  |.i...}.t.t...|.
+000002d0: a101 8301 8201 6400 0400 7d02 0400 7d03  ......d...}...}.
+000002e0: 7d06 6400 5300 290f 4e29 01fa 023d 3d29  }.d.S.).N)...==)
+000002f0: 017a 3125 2870 7932 2973 0a7b 2528 7079  .z1%(py2)s.{%(py
+00000300: 3229 7320 3d20 2528 7079 3029 732e 6669  2)s = %(py0)s.fi
+00000310: 6c65 5f70 6174 680a 7d20 3d3d 2025 2870  le_path.} == %(p
+00000320: 7934 2973 da07 6465 7461 696c 73da 085f  y4)s..details.._
+00000330: 5f66 696c 655f 5f29 03da 0370 7930 da03  _file__)...py0..
+00000340: 7079 32da 0370 7934 7a0e 6173 7365 7274  py2..py4z.assert
+00000350: 2025 2870 7936 2973 da03 7079 3672 0500   %(py6)s..py6r..
+00000360: 0000 2901 7a32 2528 7079 3229 730a 7b25  ..).z2%(py2)s.{%
+00000370: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
+00000380: 2e63 6c61 7373 5f6e 616d 650a 7d20 3d3d  .class_name.} ==
+00000390: 2025 2870 7935 2973 2903 7209 0000 0072   %(py5)s).r....r
+000003a0: 0a00 0000 da03 7079 357a 0e61 7373 6572  ......py5z.asser
+000003b0: 7420 2528 7079 3729 73da 0370 7937 da09  t %(py7)s..py7..
+000003c0: 7465 7374 5f68 6572 6529 017a 3125 2870  test_here).z1%(p
+000003d0: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
+000003e0: 2528 7079 3029 732e 7465 7374 5f6e 616d  %(py0)s.test_nam
+000003f0: 650a 7d20 3d3d 2025 2870 7935 2973 290d  e.} == %(py5)s).
+00000400: 7203 0000 00da 0966 696c 655f 7061 7468  r......file_path
+00000410: 7208 0000 00da 0a40 7079 7465 7374 5f61  r......@pytest_a
+00000420: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
+00000430: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
+00000440: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
+00000450: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
+00000460: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
+00000470: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
+00000480: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
+00000490: 7469 6f6e da0a 636c 6173 735f 6e61 6d65  tion..class_name
+000004a0: da09 7465 7374 5f6e 616d 6529 09da 0473  ..test_name)...s
+000004b0: 656c 6672 0700 0000 da0b 4070 795f 6173  elfr......@py_as
+000004c0: 7365 7274 31da 0b40 7079 5f61 7373 6572  sert1..@py_asser
+000004d0: 7433 da0b 4070 795f 666f 726d 6174 35da  t3..@py_format5.
+000004e0: 0b40 7079 5f66 6f72 6d61 7437 da0b 4070  .@py_format7..@p
+000004f0: 795f 6173 7365 7274 34da 0b40 7079 5f66  y_assert4..@py_f
+00000500: 6f72 6d61 7436 da0b 4070 795f 666f 726d  ormat6..@py_form
+00000510: 6174 38a9 0072 2300 0000 fa44 2f55 7365  at8..r#....D/Use
+00000520: 7273 2f63 6861 696e 7a2f 446f 6375 6d65  rs/chainz/Docume
+00000530: 6e74 732f 5072 6f6a 6563 7473 2f64 6a61  nts/Projects/dja
+00000540: 6e67 6f2d 7065 7266 2d72 6563 2f74 6573  ngo-perf-rec/tes
+00000550: 7473 2f74 6573 745f 7574 696c 732e 7079  ts/test_utils.py
+00000560: 720f 0000 0007 0000 0073 3000 0000 0001  r........s0.....
+00000570: 0601 0600 0800 0400 6800 0c00 0e00 0801  ........h.......
+00000580: 0600 0400 0800 0600 4e00 0c00 0e00 0c01  ........N.......
+00000590: 0600 0400 0800 0600 5200 0c00 0e00 7a1a  ........R.....z.
+000005a0: 4375 7272 656e 7454 6573 7454 6573 7473  CurrentTestTests
+000005b0: 2e74 6573 745f 6865 7265 6301 0000 0000  .test_herec.....
+000005c0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
+000005d0: b200 0000 7400 8300 7d01 7400 8300 7d02  ....t...}.t...}.
+000005e0: 7c01 7c02 6b02 7d03 7c03 73a2 7401 a002  |.|.k.}.|.s.t...
+000005f0: 6401 7c03 6601 6402 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
+00000600: 6403 7403 a004 a100 6b06 7342 7401 a005  d.t.....k.sBt...
+00000610: 7400 a101 724c 7401 a006 7400 a101 6e02  t...rLt...t...n.
+00000620: 6403 7401 a006 7c01 a101 6403 7403 a004  d.t...|...d.t...
+00000630: a100 6b06 736c 7401 a005 7400 a101 7276  ..k.slt...t...rv
+00000640: 7401 a006 7400 a101 6e02 6403 7401 a006  t...t...n.d.t...
+00000650: 7c02 a101 6404 9c04 1600 7d04 6405 6406  |...d.....}.d.d.
+00000660: 7c04 6901 1600 7d05 7407 7401 a008 7c05  |.i...}.t.t...|.
+00000670: a101 8301 8201 6400 0400 7d01 0400 7d03  ......d...}...}.
+00000680: 7d02 6400 5300 2907 4e29 0172 0600 0000  }.d.S.).N).r....
+00000690: 2901 7a40 2528 7079 3229 730a 7b25 2870  ).z@%(py2)s.{%(p
+000006a0: 7932 2973 203d 2025 2870 7930 2973 2829  y2)s = %(py0)s()
+000006b0: 0a7d 203d 3d20 2528 7079 3629 730a 7b25  .} == %(py6)s.{%
+000006c0: 2870 7936 2973 203d 2025 2870 7934 2973  (py6)s = %(py4)s
+000006d0: 2829 0a7d 7203 0000 0029 0472 0900 0000  ().}r....).r....
+000006e0: 720a 0000 0072 0b00 0000 720c 0000 007a  r....r....r....z
+000006f0: 0e61 7373 6572 7420 2528 7079 3829 73da  .assert %(py8)s.
+00000700: 0370 7938 2909 7203 0000 0072 1100 0000  .py8).r....r....
+00000710: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000720: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00000730: 0000 0029 0672 1b00 0000 721c 0000 00da  ...).r....r.....
+00000740: 0b40 7079 5f61 7373 6572 7435 721d 0000  .@py_assert5r...
+00000750: 0072 1f00 0000 da0b 4070 795f 666f 726d  .r......@py_form
+00000760: 6174 3972 2300 0000 7223 0000 0072 2400  at9r#...r#...r$.
+00000770: 0000 da0f 7465 7374 5f74 7769 6365 5f73  ....test_twice_s
+00000780: 616d 650d 0000 0073 1000 0000 0001 0600  ame....s........
+00000790: 0600 0800 0400 7000 0c00 0e00 7a20 4375  ......p.....z Cu
+000007a0: 7272 656e 7454 6573 7454 6573 7473 2e74  rrentTestTests.t
+000007b0: 6573 745f 7477 6963 655f 7361 6d65 6301  est_twice_samec.
+000007c0: 0000 0000 0000 000a 0000 0007 0000 0043  ...............C
+000007d0: 0000 0073 ca01 0000 6401 6402 8400 7d01  ...s....d.d...}.
+000007e0: 7c01 8300 7d02 7c02 6a00 7d03 7c03 7401  |...}.|.j.}.|.t.
+000007f0: 6b02 7d04 7c04 73a2 7402 a003 6403 7c04  k.}.|.s.t...d.|.
+00000800: 6601 6404 7c03 7401 6602 a104 6405 7404  f.d.|.t.f...d.t.
+00000810: a005 a100 6b06 734a 7402 a006 7c02 a101  ....k.sJt...|...
+00000820: 7254 7402 a007 7c02 a101 6e02 6405 7402  rTt...|...n.d.t.
+00000830: a007 7c03 a101 6406 7404 a005 a100 6b06  ..|...d.t.....k.
+00000840: 7374 7402 a006 7401 a101 727e 7402 a007  stt...t...r~t...
+00000850: 7401 a101 6e02 6406 6407 9c03 1600 7d05  t...n.d.d.....}.
+00000860: 6408 6409 7c05 6901 1600 7d06 7408 7402  d.d.|.i...}.t.t.
+00000870: a009 7c06 a101 8301 8201 6400 0400 7d03  ..|.......d...}.
+00000880: 7d04 7c02 6a0a 7d03 6400 7d07 7c03 7c07  }.|.j.}.d.}.|.|.
+00000890: 6b08 7d04 7c04 9001 732a 7402 a003 640a  k.}.|...s*t...d.
+000008a0: 7c04 6601 640b 7c03 7c07 6602 a104 6405  |.f.d.|.|.f...d.
+000008b0: 7404 a005 a100 6b06 73ec 7402 a006 7c02  t.....k.s.t...|.
+000008c0: a101 72f6 7402 a007 7c02 a101 6e02 6405  ..r.t...|...n.d.
+000008d0: 7402 a007 7c03 a101 7402 a007 7c07 a101  t...|...t...|...
+000008e0: 640c 9c03 1600 7d08 640d 640e 7c08 6901  d.....}.d.d.|.i.
+000008f0: 1600 7d09 7408 7402 a009 7c09 a101 8301  ..}.t.t...|.....
+00000900: 8201 6400 0400 7d03 0400 7d04 7d07 7c02  ..d...}...}.}.|.
+00000910: 6a0b 7d03 640f 7d07 7c03 7c07 6b02 7d04  j.}.d.}.|.|.k.}.
+00000920: 7c04 9001 73ba 7402 a003 6403 7c04 6601  |...s.t...d.|.f.
+00000930: 6410 7c03 7c07 6602 a104 6405 7404 a005  d.|.|.f...d.t...
+00000940: a100 6b06 9001 737c 7402 a006 7c02 a101  ..k...s|t...|...
+00000950: 9001 7286 7402 a007 7c02 a101 6e02 6405  ..r.t...|...n.d.
+00000960: 7402 a007 7c03 a101 7402 a007 7c07 a101  t...|...t...|...
+00000970: 640c 9c03 1600 7d08 640d 640e 7c08 6901  d.....}.d.d.|.i.
+00000980: 1600 7d09 7408 7402 a009 7c09 a101 8301  ..}.t.t...|.....
+00000990: 8201 6400 0400 7d03 0400 7d04 7d07 6400  ..d...}...}.}.d.
+000009a0: 5300 2911 4e63 0000 0000 0000 0000 0000  S.).Nc..........
+000009b0: 0000 0100 0000 5300 0000 7306 0000 0074  ......S...s....t
+000009c0: 0083 0053 0029 014e 2901 7203 0000 0072  ...S.).N).r....r
+000009d0: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
+000009e0: 0000 00da 1574 6573 745f 7468 6174 735f  .....test_thats_
+000009f0: 6675 6e63 7469 6f6e 616c 1100 0000 7302  functional....s.
+00000a00: 0000 0000 017a 3f43 7572 7265 6e74 5465  .....z?CurrentTe
+00000a10: 7374 5465 7374 732e 7465 7374 5f66 756e  stTests.test_fun
+00000a20: 6374 696f 6e61 6c2e 3c6c 6f63 616c 733e  ctional.<locals>
+00000a30: 2e74 6573 745f 7468 6174 735f 6675 6e63  .test_thats_func
+00000a40: 7469 6f6e 616c 2901 7206 0000 0029 017a  tional).r....).z
+00000a50: 3125 2870 7932 2973 0a7b 2528 7079 3229  1%(py2)s.{%(py2)
+00000a60: 7320 3d20 2528 7079 3029 732e 6669 6c65  s = %(py0)s.file
+00000a70: 5f70 6174 680a 7d20 3d3d 2025 2870 7934  _path.} == %(py4
+00000a80: 2973 7207 0000 0072 0800 0000 2903 7209  )sr....r....).r.
+00000a90: 0000 0072 0a00 0000 720b 0000 007a 0e61  ...r....r....z.a
+00000aa0: 7373 6572 7420 2528 7079 3629 7372 0c00  ssert %(py6)sr..
+00000ab0: 0000 2901 da02 6973 2901 7a32 2528 7079  ..)...is).z2%(py
+00000ac0: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
+00000ad0: 2870 7930 2973 2e63 6c61 7373 5f6e 616d  (py0)s.class_nam
+00000ae0: 650a 7d20 6973 2025 2870 7935 2973 2903  e.} is %(py5)s).
+00000af0: 7209 0000 0072 0a00 0000 720d 0000 007a  r....r....r....z
+00000b00: 0e61 7373 6572 7420 2528 7079 3729 7372  .assert %(py7)sr
+00000b10: 0e00 0000 7229 0000 0029 017a 3125 2870  ....r)...).z1%(p
+00000b20: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
+00000b30: 2528 7079 3029 732e 7465 7374 5f6e 616d  %(py0)s.test_nam
+00000b40: 650a 7d20 3d3d 2025 2870 7935 2973 290c  e.} == %(py5)s).
+00000b50: 7210 0000 0072 0800 0000 7211 0000 0072  r....r....r....r
+00000b60: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
+00000b70: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
+00000b80: 0000 7219 0000 0072 1a00 0000 290a 721b  ..r....r....).r.
+00000b90: 0000 0072 2900 0000 7207 0000 0072 1c00  ...r)...r....r..
+00000ba0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000bb0: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000bc0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
+00000bd0: 0f74 6573 745f 6675 6e63 7469 6f6e 616c  .test_functional
+00000be0: 1000 0000 7332 0000 0000 0108 0306 0106  ....s2..........
+00000bf0: 0008 0004 0068 000c 000e 0008 0106 0004  .....h..........
+00000c00: 0008 0006 004e 000c 000e 000c 0106 0004  .....N..........
+00000c10: 0008 0006 0052 000c 000e 007a 2043 7572  .....R.....z Cur
+00000c20: 7265 6e74 5465 7374 5465 7374 732e 7465  rentTestTests.te
+00000c30: 7374 5f66 756e 6374 696f 6e61 6c4e 2906  st_functionalN).
+00000c40: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000c50: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000c60: 6d65 5f5f 720f 0000 0072 2800 0000 722b  me__r....r(...r+
+00000c70: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
+00000c80: 0000 7224 0000 0072 0500 0000 0600 0000  ..r$...r........
+00000c90: 7306 0000 0008 0108 0608 0372 0500 0000  s..........r....
+00000ca0: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
+00000cb0: 0040 0000 0073 3400 0000 6500 5a01 6400  .@...s4...e.Z.d.
+00000cc0: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
+00000cd0: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
+00000ce0: 5a06 6409 640a 8400 5a07 640b 5300 290c  Z.d.d...Z.d.S.).
+00000cf0: da10 536f 7274 6564 4e61 6d65 7354 6573  ..SortedNamesTes
+00000d00: 7473 6301 0000 0000 0000 0007 0000 0007  tsc.............
+00000d10: 0000 0043 0000 0073 a000 0000 6700 7d01  ...C...s....g.}.
+00000d20: 7400 7c01 8301 7d02 6700 7d03 7c02 7c03  t.|...}.g.}.|.|.
+00000d30: 6b02 7d04 7c04 738c 7401 a002 6401 7c04  k.}.|.s.t...d.|.
+00000d40: 6601 6402 7c02 7c03 6602 a104 6403 7403  f.d.|.|.f...d.t.
+00000d50: a004 a100 6b06 7346 7401 a005 7400 a101  ....k.sFt...t...
+00000d60: 7250 7401 a006 7400 a101 6e02 6403 7401  rPt...t...n.d.t.
+00000d70: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
+00000d80: a006 7c03 a101 6404 9c04 1600 7d05 6405  ..|...d.....}.d.
+00000d90: 6406 7c05 6901 1600 7d06 7407 7401 a008  d.|.i...}.t.t...
+00000da0: 7c06 a101 8301 8201 6400 0400 7d01 0400  |.......d...}...
+00000db0: 7d02 0400 7d04 7d03 6400 5300 2907 4e29  }...}.}.d.S.).N)
+00000dc0: 0172 0600 0000 2901 7a30 2528 7079 3429  .r....).z0%(py4)
+00000dd0: 730a 7b25 2870 7934 2973 203d 2025 2870  s.{%(py4)s = %(p
+00000de0: 7930 2973 2825 2870 7932 2973 290a 7d20  y0)s(%(py2)s).} 
+00000df0: 3d3d 2025 2870 7937 2973 7204 0000 0029  == %(py7)sr....)
+00000e00: 0472 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000e10: 720e 0000 007a 0e61 7373 6572 7420 2528  r....z.assert %(
+00000e20: 7079 3929 73da 0370 7939 2909 7204 0000  py9)s..py9).r...
+00000e30: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000e40: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000e50: 1700 0000 7218 0000 0029 0772 1b00 0000  ....r....).r....
+00000e60: 721c 0000 0072 1d00 0000 da0b 4070 795f  r....r......@py_
+00000e70: 6173 7365 7274 3672 2600 0000 7222 0000  assert6r&...r"..
+00000e80: 00da 0c40 7079 5f66 6f72 6d61 7431 3072  ...@py_format10r
+00000e90: 2300 0000 7223 0000 0072 2400 0000 da0a  #...r#...r$.....
+00000ea0: 7465 7374 5f65 6d70 7479 1b00 0000 7312  test_empty....s.
+00000eb0: 0000 0000 0104 0008 0004 0008 0004 0056  ...............V
+00000ec0: 000c 000e 007a 1b53 6f72 7465 644e 616d  .....z.SortedNam
+00000ed0: 6573 5465 7374 732e 7465 7374 5f65 6d70  esTests.test_emp
+00000ee0: 7479 6301 0000 0000 0000 0007 0000 0007  tyc.............
+00000ef0: 0000 0043 0000 0073 a400 0000 6401 6701  ...C...s....d.g.
+00000f00: 7d01 7400 7c01 8301 7d02 6401 6701 7d03  }.t.|...}.d.g.}.
+00000f10: 7c02 7c03 6b02 7d04 7c04 7390 7401 a002  |.|.k.}.|.s.t...
+00000f20: 6402 7c04 6601 6403 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00000f30: 6404 7403 a004 a100 6b06 734a 7401 a005  d.t.....k.sJt...
+00000f40: 7400 a101 7254 7401 a006 7400 a101 6e02  t...rTt...t...n.
+00000f50: 6404 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
+00000f60: a101 7401 a006 7c03 a101 6405 9c04 1600  ..t...|...d.....
+00000f70: 7d05 6406 6407 7c05 6901 1600 7d06 7407  }.d.d.|.i...}.t.
+00000f80: 7401 a008 7c06 a101 8301 8201 6400 0400  t...|.......d...
+00000f90: 7d01 0400 7d02 0400 7d04 7d03 6400 5300  }...}...}.}.d.S.
+00000fa0: 2908 4eda 0764 6566 6175 6c74 2901 7206  ).N..default).r.
+00000fb0: 0000 0029 017a 3025 2870 7934 2973 0a7b  ...).z0%(py4)s.{
+00000fc0: 2528 7079 3429 7320 3d20 2528 7079 3029  %(py4)s = %(py0)
+00000fd0: 7328 2528 7079 3229 7329 0a7d 203d 3d20  s(%(py2)s).} == 
+00000fe0: 2528 7079 3729 7372 0400 0000 2904 7209  %(py7)sr....).r.
+00000ff0: 0000 0072 0a00 0000 720b 0000 0072 0e00  ...r....r....r..
+00001000: 0000 7a0e 6173 7365 7274 2025 2870 7939  ..z.assert %(py9
+00001010: 2973 7230 0000 0029 0972 0400 0000 7211  )sr0...).r....r.
+00001020: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
+00001030: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00001040: 0072 1800 0000 2907 721b 0000 0072 1c00  .r....).r....r..
+00001050: 0000 721d 0000 0072 3100 0000 7226 0000  ..r....r1...r&..
+00001060: 0072 2200 0000 7232 0000 0072 2300 0000  .r"...r2...r#...
+00001070: 7223 0000 0072 2400 0000 da11 7465 7374  r#...r$.....test
+00001080: 5f6a 7573 745f 6465 6661 756c 741e 0000  _just_default...
+00001090: 0073 1200 0000 0001 0600 0800 0600 0800  .s..............
+000010a0: 0400 5600 0c00 0e00 7a22 536f 7274 6564  ..V.....z"Sorted
+000010b0: 4e61 6d65 7354 6573 7473 2e74 6573 745f  NamesTests.test_
+000010c0: 6a75 7374 5f64 6566 6175 6c74 6301 0000  just_defaultc...
+000010d0: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
+000010e0: 0073 a400 0000 6401 6701 7d01 7400 7c01  .s....d.g.}.t.|.
+000010f0: 8301 7d02 6401 6701 7d03 7c02 7c03 6b02  ..}.d.g.}.|.|.k.
+00001100: 7d04 7c04 7390 7401 a002 6402 7c04 6601  }.|.s.t...d.|.f.
+00001110: 6403 7c02 7c03 6602 a104 6404 7403 a004  d.|.|.f...d.t...
+00001120: a100 6b06 734a 7401 a005 7400 a101 7254  ..k.sJt...t...rT
+00001130: 7401 a006 7400 a101 6e02 6404 7401 a006  t...t...n.d.t...
+00001140: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
+00001150: 7c03 a101 6405 9c04 1600 7d05 6406 6407  |...d.....}.d.d.
+00001160: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
+00001170: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
+00001180: 0400 7d04 7d03 6400 5300 2908 4e5a 0973  ..}.}.d.S.).NZ.s
+00001190: 6f6d 6574 6869 6e67 2901 7206 0000 0029  omething).r....)
+000011a0: 017a 3025 2870 7934 2973 0a7b 2528 7079  .z0%(py4)s.{%(py
+000011b0: 3429 7320 3d20 2528 7079 3029 7328 2528  4)s = %(py0)s(%(
+000011c0: 7079 3229 7329 0a7d 203d 3d20 2528 7079  py2)s).} == %(py
+000011d0: 3729 7372 0400 0000 2904 7209 0000 0072  7)sr....).r....r
+000011e0: 0a00 0000 720b 0000 0072 0e00 0000 7a0e  ....r....r....z.
+000011f0: 6173 7365 7274 2025 2870 7939 2973 7230  assert %(py9)sr0
+00001200: 0000 0029 0972 0400 0000 7211 0000 0072  ...).r....r....r
+00001210: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
+00001220: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
+00001230: 0000 2907 721b 0000 0072 1c00 0000 721d  ..).r....r....r.
+00001240: 0000 0072 3100 0000 7226 0000 0072 2200  ...r1...r&...r".
+00001250: 0000 7232 0000 0072 2300 0000 7223 0000  ..r2...r#...r#..
+00001260: 0072 2400 0000 da13 7465 7374 5f6a 7573  .r$.....test_jus
+00001270: 745f 736f 6d65 7468 696e 6721 0000 0073  t_something!...s
+00001280: 1200 0000 0001 0600 0800 0600 0800 0400  ................
+00001290: 5600 0c00 0e00 7a24 536f 7274 6564 4e61  V.....z$SortedNa
+000012a0: 6d65 7354 6573 7473 2e74 6573 745f 6a75  mesTests.test_ju
+000012b0: 7374 5f73 6f6d 6574 6869 6e67 6301 0000  st_somethingc...
+000012c0: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
+000012d0: 0073 a800 0000 6401 6402 6702 7d01 7400  .s....d.d.g.}.t.
+000012e0: 7c01 8301 7d02 6402 6401 6702 7d03 7c02  |...}.d.d.g.}.|.
+000012f0: 7c03 6b02 7d04 7c04 7394 7401 a002 6403  |.k.}.|.s.t...d.
+00001300: 7c04 6601 6404 7c02 7c03 6602 a104 6405  |.f.d.|.|.f...d.
+00001310: 7403 a004 a100 6b06 734e 7401 a005 7400  t.....k.sNt...t.
+00001320: a101 7258 7401 a006 7400 a101 6e02 6405  ..rXt...t...n.d.
+00001330: 7401 a006 7c01 a101 7401 a006 7c02 a101  t...|...t...|...
+00001340: 7401 a006 7c03 a101 6406 9c04 1600 7d05  t...|...d.....}.
+00001350: 6407 6408 7c05 6901 1600 7d06 7407 7401  d.d.|.i...}.t.t.
+00001360: a008 7c06 a101 8301 8201 6400 0400 7d01  ..|.......d...}.
+00001370: 0400 7d02 0400 7d04 7d03 6400 5300 2909  ..}...}.}.d.S.).
+00001380: 4eda 0162 da01 6129 0172 0600 0000 2901  N..b..a).r....).
+00001390: 7a30 2528 7079 3429 730a 7b25 2870 7934  z0%(py4)s.{%(py4
+000013a0: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
+000013b0: 7932 2973 290a 7d20 3d3d 2025 2870 7937  y2)s).} == %(py7
+000013c0: 2973 7204 0000 0029 0472 0900 0000 720a  )sr....).r....r.
+000013d0: 0000 0072 0b00 0000 720e 0000 007a 0e61  ...r....r....z.a
+000013e0: 7373 6572 7420 2528 7079 3929 7372 3000  ssert %(py9)sr0.
+000013f0: 0000 2909 7204 0000 0072 1100 0000 7212  ..).r....r....r.
+00001400: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
+00001410: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00001420: 0029 0772 1b00 0000 721c 0000 0072 1d00  .).r....r....r..
+00001430: 0000 7231 0000 0072 2600 0000 7222 0000  ..r1...r&...r"..
+00001440: 0072 3200 0000 7223 0000 0072 2300 0000  .r2...r#...r#...
+00001450: 7224 0000 00da 0e74 6573 745f 646f 6573  r$.....test_does
+00001460: 5f73 6f72 7424 0000 0073 1200 0000 0001  _sort$...s......
+00001470: 0800 0800 0800 0800 0400 5600 0c00 0e00  ..........V.....
+00001480: 7a1f 536f 7274 6564 4e61 6d65 7354 6573  z.SortedNamesTes
+00001490: 7473 2e74 6573 745f 646f 6573 5f73 6f72  ts.test_does_sor
+000014a0: 7463 0100 0000 0000 0000 0700 0000 0700  tc..............
+000014b0: 0000 4300 0000 73a8 0000 0064 0164 0267  ..C...s....d.d.g
+000014c0: 027d 0174 007c 0183 017d 0264 0264 0167  .}.t.|...}.d.d.g
+000014d0: 027d 037c 027c 036b 027d 047c 0473 9474  .}.|.|.k.}.|.s.t
+000014e0: 01a0 0264 037c 0466 0164 047c 027c 0366  ...d.|.f.d.|.|.f
+000014f0: 02a1 0464 0574 03a0 04a1 006b 0673 4e74  ...d.t.....k.sNt
+00001500: 01a0 0574 00a1 0172 5874 01a0 0674 00a1  ...t...rXt...t..
+00001510: 016e 0264 0574 01a0 067c 01a1 0174 01a0  .n.d.t...|...t..
+00001520: 067c 02a1 0174 01a0 067c 03a1 0164 069c  .|...t...|...d..
+00001530: 0416 007d 0564 0764 087c 0569 0116 007d  ...}.d.d.|.i...}
+00001540: 0674 0774 01a0 087c 06a1 0183 0182 0164  .t.t...|.......d
+00001550: 0004 007d 0104 007d 0204 007d 047d 0364  ...}...}...}.}.d
+00001560: 0053 0029 094e 7238 0000 0072 3400 0000  .S.).Nr8...r4...
+00001570: 2901 7206 0000 0029 017a 3025 2870 7934  ).r....).z0%(py4
+00001580: 2973 0a7b 2528 7079 3429 7320 3d20 2528  )s.{%(py4)s = %(
+00001590: 7079 3029 7328 2528 7079 3229 7329 0a7d  py0)s(%(py2)s).}
+000015a0: 203d 3d20 2528 7079 3729 7372 0400 0000   == %(py7)sr....
+000015b0: 2904 7209 0000 0072 0a00 0000 720b 0000  ).r....r....r...
+000015c0: 0072 0e00 0000 7a0e 6173 7365 7274 2025  .r....z.assert %
+000015d0: 2870 7939 2973 7230 0000 0029 0972 0400  (py9)sr0...).r..
+000015e0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000015f0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00001600: 7217 0000 0072 1800 0000 2907 721b 0000  r....r....).r...
+00001610: 0072 1c00 0000 721d 0000 0072 3100 0000  .r....r....r1...
+00001620: 7226 0000 0072 2200 0000 7232 0000 0072  r&...r"...r2...r
+00001630: 2300 0000 7223 0000 0072 2400 0000 da1d  #...r#...r$.....
+00001640: 7465 7374 5f73 6f72 745f 6b65 6570 735f  test_sort_keeps_
+00001650: 6465 6661 756c 745f 6669 7273 7427 0000  default_first'..
+00001660: 0073 1200 0000 0001 0800 0800 0800 0800  .s..............
+00001670: 0400 5600 0c00 0e00 7a2e 536f 7274 6564  ..V.....z.Sorted
+00001680: 4e61 6d65 7354 6573 7473 2e74 6573 745f  NamesTests.test_
+00001690: 736f 7274 5f6b 6565 7073 5f64 6566 6175  sort_keeps_defau
+000016a0: 6c74 5f66 6972 7374 4e29 0872 2c00 0000  lt_firstN).r,...
+000016b0: 722d 0000 0072 2e00 0000 7233 0000 0072  r-...r....r3...r
+000016c0: 3500 0000 7236 0000 0072 3900 0000 723a  5...r6...r9...r:
+000016d0: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
+000016e0: 0000 7224 0000 0072 2f00 0000 1a00 0000  ..r$...r/.......
+000016f0: 730a 0000 0008 0108 0308 0308 0308 0372  s..............r
+00001700: 2f00 0000 290d da08 6275 696c 7469 6e73  /...)...builtins
+00001710: 7213 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
+00001720: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+00001730: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+00001740: 7269 7465 7211 0000 00da 0b64 6a61 6e67  riter......djang
+00001750: 6f2e 7465 7374 7202 0000 005a 1564 6a61  o.testr....Z.dja
+00001760: 6e67 6f5f 7065 7266 5f72 6563 2e75 7469  ngo_perf_rec.uti
+00001770: 6c73 7203 0000 0072 0400 0000 7205 0000  lsr....r....r...
+00001780: 0072 2f00 0000 7223 0000 0072 2300 0000  .r/...r#...r#...
+00001790: 7223 0000 0072 2400 0000 da08 3c6d 6f64  r#...r$.....<mod
+000017a0: 756c 653e 0100 0000 730a 0000 0008 0012  ule>....s.......
+000017b0: 000c 0210 0310 14                        .......
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_orm.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_orm.cpython-39-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate.cpython-39-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_duplicate_other.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_duplicate_other.cpython-39-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_fixture_usage.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_fixture_usage.cpython-39-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_pytest_plugin.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_pytest_plugin.cpython-39-pytest-6.1.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-37-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_sql.cpython-39-pytest-6.1.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_sql.cpython-39-pytest-6.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 10c5 815f 0a20 0000 e300 0000  a......_. ......
+00000000: 610d 0d0a da21 a35f 0a20 0000 e300 0000  a....!._. ......
 00000010: 0000 0000 0000 0000 0000 0000 0002 0000  ................
 00000020: 0040 0000 0073 5a01 0000 6400 6401 6c00  .@...sZ...d.d.l.
 00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
 00000040: 5a05 0100 6400 6402 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000050: 6403 6404 8400 5a08 6405 6406 8400 5a09  d.d...Z.d.d...Z.
 00000060: 6407 6408 8400 5a0a 6409 640a 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 640b 640c 8400 5a0c 640d 640e 8400 5a0d  d.d...Z.d.d...Z.
@@ -185,19 +185,19 @@
 00000b80: 720d 0000 00da 0470 7931 327a 0f61 7373  r......py12z.ass
 00000b90: 6572 7420 2528 7079 3134 2973 da04 7079  ert %(py14)s..py
 00000ba0: 3134 720e 0000 0029 0a72 2b00 0000 7218  14r....).r+...r.
 00000bb0: 0000 0072 1900 0000 721b 0000 0072 1a00  ...r....r....r..
 00000bc0: 0000 722c 0000 00da 0c40 7079 5f61 7373  ..r,.....@py_ass
 00000bd0: 6572 7431 31da 0c40 7079 5f61 7373 6572  ert11..@py_asser
 00000be0: 7431 305a 0c40 7079 5f66 6f72 6d61 7431  t10Z.@py_format1
-00000bf0: 33da 0c40 7079 5f66 6f72 6d61 7431 3572  3..@py_format15r
+00000bf0: 335a 0c40 7079 5f66 6f72 6d61 7431 3572  3Z.@py_format15r
 00000c00: 1e00 0000 721e 0000 0072 1f00 0000 da21  ....r....r.....!
 00000c10: 7465 7374 5f73 656c 6563 745f 636f 616c  test_select_coal
 00000c20: 6573 6365 5f73 686f 775f 636f 6c75 6d6e  esce_show_column
-00000c30: 731b 0000 0073 0200 0000 0001 7237 0000  s....s......r7..
+00000c30: 731b 0000 0073 0200 0000 0001 7236 0000  s....s......r6..
 00000c40: 0063 0000 0000 0000 0000 0000 0000 0600  .c..............
 00000c50: 0000 0700 0000 4300 0000 73a0 0000 0064  ......C...s....d
 00000c60: 017d 0074 007c 0083 017d 0164 027d 027c  .}.t.|...}.d.}.|
 00000c70: 017c 026b 027d 037c 0373 8c74 01a0 0264  .|.k.}.|.s.t...d
 00000c80: 037c 0366 0164 047c 017c 0266 02a1 0464  .|.f.d.|.|.f...d
 00000c90: 0574 03a0 04a1 0076 0073 4674 01a0 0574  .t.....v.sFt...t
 00000ca0: 00a1 0172 5074 01a0 0674 00a1 016e 0264  ...rPt...t...n.d
@@ -216,35 +216,35 @@
 00000d70: 6162 6c65 6020 5748 4552 4520 6074 6162  able` WHERE `tab
 00000d80: 6c65 602e 6069 6460 203d 2023 7204 0000  le`.`id` = #r...
 00000d90: 0072 0600 0000 7202 0000 0072 0700 0000  .r....r....r....
 00000da0: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
 00000db0: 1700 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
 00000dc0: 0000 00da 1174 6573 745f 7365 6c65 6374  .....test_select
 00000dd0: 5f77 6865 7265 2800 0000 7302 0000 0000  _where(...s.....
-00000de0: 0172 3a00 0000 6301 0000 0000 0000 0000  .r:...c.........
+00000de0: 0172 3900 0000 6301 0000 0000 0000 0000  .r9...c.........
 00000df0: 0000 0008 0000 0008 0000 0043 0000 0073  ...........C...s
 00000e00: b400 0000 6401 7d01 6402 7d02 7400 7c01  ....d.}.d.}.t.|.
 00000e10: 7c02 6403 8d02 7d03 6404 7d04 7c03 7c04  |.d...}.d.}.|.|.
 00000e20: 6b02 7d05 7c05 739c 7401 a002 6405 7c05  k.}.|.s.t...d.|.
 00000e30: 6601 6406 7c03 7c04 6602 a104 6407 7403  f.d.|.|.f...d.t.
 00000e40: a004 a100 7600 734e 7401 a005 7400 a101  ....v.sNt...t...
 00000e50: 7258 7401 a006 7400 a101 6e02 6407 7401  rXt...t...n.d.t.
 00000e60: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
 00000e70: a006 7c03 a101 7401 a006 7c04 a101 6408  ..|...t...|...d.
 00000e80: 9c05 1600 7d06 6409 640a 7c06 6901 1600  ....}.d.d.|.i...
 00000e90: 7d07 7407 7401 a008 7c07 a101 8301 8201  }.t.t...|.......
 00000ea0: 6400 0400 7d01 0400 7d02 0400 7d03 0400  d...}...}...}...
-00000eb0: 7d05 7d04 6400 5300 290b 4e72 3800 0000  }.}.d.S.).Nr8...
-00000ec0: 4672 2300 0000 7239 0000 0072 0400 0000  Fr#...r9...r....
+00000eb0: 7d05 7d04 6400 5300 290b 4e72 3700 0000  }.}.d.S.).Nr7...
+00000ec0: 4672 2300 0000 7238 0000 0072 0400 0000  Fr#...r8...r....
 00000ed0: 7225 0000 0072 0200 0000 7226 0000 0072  r%...r....r&...r
 00000ee0: 2800 0000 7229 0000 0072 0e00 0000 722a  (...r)...r....r*
 00000ef0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
 00000f00: 0000 da1e 7465 7374 5f73 656c 6563 745f  ....test_select_
 00000f10: 7768 6572 655f 7368 6f77 5f63 6f6c 756d  where_show_colum
-00000f20: 6e73 3100 0000 7302 0000 0000 0172 3b00  ns1...s......r;.
+00000f20: 6e73 3100 0000 7302 0000 0000 0172 3a00  ns1...s......r:.
 00000f30: 0000 6300 0000 0000 0000 0000 0000 0006  ..c.............
 00000f40: 0000 0007 0000 0043 0000 0073 a000 0000  .......C...s....
 00000f50: 6401 7d00 7400 7c00 8301 7d01 6402 7d02  d.}.t.|...}.d.}.
 00000f60: 7c01 7c02 6b02 7d03 7c03 738c 7401 a002  |.|.k.}.|.s.t...
 00000f70: 6403 7c03 6601 6404 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
 00000f80: 6405 7403 a004 a100 7600 7346 7401 a005  d.t.....v.sFt...
 00000f90: 7400 a101 7250 7401 a006 7400 a101 6e02  t...rPt...t...n.
@@ -259,36 +259,36 @@
 00001020: 454c 4543 5420 2f2a 2063 6f6d 6d65 6e74  ELECT /* comment
 00001030: 202a 2f20 2e2e 2e20 4652 4f4d 2060 6260   */ ... FROM `b`
 00001040: 7204 0000 0072 0600 0000 7202 0000 0072  r....r....r....r
 00001050: 0700 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00001060: 0000 0072 1700 0000 721e 0000 0072 1e00  ...r....r....r..
 00001070: 0000 721f 0000 00da 1374 6573 745f 7365  ..r......test_se
 00001080: 6c65 6374 5f63 6f6d 6d65 6e74 3b00 0000  lect_comment;...
-00001090: 7302 0000 0000 0172 3d00 0000 6301 0000  s......r=...c...
+00001090: 7302 0000 0000 0172 3c00 0000 6301 0000  s......r<...c...
 000010a0: 0000 0000 0000 0000 0008 0000 0008 0000  ................
 000010b0: 0043 0000 0073 b400 0000 6401 7d01 6402  .C...s....d.}.d.
 000010c0: 7d02 7400 7c01 7c02 6403 8d02 7d03 6401  }.t.|.|.d...}.d.
 000010d0: 7d04 7c03 7c04 6b02 7d05 7c05 739c 7401  }.|.|.k.}.|.s.t.
 000010e0: a002 6404 7c05 6601 6405 7c03 7c04 6602  ..d.|.f.d.|.|.f.
 000010f0: a104 6406 7403 a004 a100 7600 734e 7401  ..d.t.....v.sNt.
 00001100: a005 7400 a101 7258 7401 a006 7400 a101  ..t...rXt...t...
 00001110: 6e02 6406 7401 a006 7c01 a101 7401 a006  n.d.t...|...t...
 00001120: 7c02 a101 7401 a006 7c03 a101 7401 a006  |...t...|...t...
 00001130: 7c04 a101 6407 9c05 1600 7d06 6408 6409  |...d.....}.d.d.
 00001140: 7c06 6901 1600 7d07 7407 7401 a008 7c07  |.i...}.t.t...|.
 00001150: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
 00001160: 0400 7d03 0400 7d05 7d04 6400 5300 290a  ..}...}.}.d.S.).
-00001170: 4e72 3c00 0000 4672 2300 0000 7204 0000  Nr<...Fr#...r...
+00001170: 4e72 3b00 0000 4672 2300 0000 7204 0000  Nr;...Fr#...r...
 00001180: 0072 2500 0000 7202 0000 0072 2600 0000  .r%...r....r&...
 00001190: 7228 0000 0072 2900 0000 720e 0000 0072  r(...r)...r....r
 000011a0: 2a00 0000 721e 0000 0072 1e00 0000 721f  *...r....r....r.
 000011b0: 0000 00da 2074 6573 745f 7365 6c65 6374  .... test_select
 000011c0: 5f63 6f6d 6d65 6e74 5f73 686f 775f 636f  _comment_show_co
 000011d0: 6c75 6d6e 7342 0000 0073 0200 0000 0001  lumnsB...s......
-000011e0: 723e 0000 0063 0000 0000 0000 0000 0000  r>...c..........
+000011e0: 723d 0000 0063 0000 0000 0000 0000 0000  r=...c..........
 000011f0: 0000 0600 0000 0700 0000 4300 0000 73a0  ..........C...s.
 00001200: 0000 0064 017d 0074 007c 0083 017d 0164  ...d.}.t.|...}.d
 00001210: 027d 027c 017c 026b 027d 037c 0373 8c74  .}.|.|.k.}.|.s.t
 00001220: 01a0 0264 037c 0366 0164 047c 017c 0266  ...d.|.f.d.|.|.f
 00001230: 02a1 0464 0574 03a0 04a1 0076 0073 4674  ...d.t.....v.sFt
 00001240: 01a0 0574 00a1 0172 5074 01a0 0674 00a1  ...t...rPt...t..
 00001250: 016e 0264 0574 01a0 067c 00a1 0174 01a0  .n.d.t...|...t..
@@ -306,39 +306,39 @@
 00001310: 612e 625f 6964 203d 2062 2e69 6429 2057  a.b_id = b.id) W
 00001320: 4845 5245 2061 2e66 3220 3d20 2372 0400  HERE a.f2 = #r..
 00001330: 0000 7206 0000 0072 0200 0000 7207 0000  ..r....r....r...
 00001340: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
 00001350: 7217 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
 00001360: 1f00 0000 da10 7465 7374 5f73 656c 6563  ......test_selec
 00001370: 745f 6a6f 696e 4900 0000 7302 0000 0000  t_joinI...s.....
-00001380: 0172 4000 0000 6301 0000 0000 0000 0000  .r@...c.........
+00001380: 0172 3f00 0000 6301 0000 0000 0000 0000  .r?...c.........
 00001390: 0000 0008 0000 0008 0000 0043 0000 0073  ...........C...s
 000013a0: b400 0000 6401 7d01 6402 7d02 7400 7c01  ....d.}.d.}.t.|.
 000013b0: 7c02 6403 8d02 7d03 6404 7d04 7c03 7c04  |.d...}.d.}.|.|.
 000013c0: 6b02 7d05 7c05 739c 7401 a002 6405 7c05  k.}.|.s.t...d.|.
 000013d0: 6601 6406 7c03 7c04 6602 a104 6407 7403  f.d.|.|.f...d.t.
 000013e0: a004 a100 7600 734e 7401 a005 7400 a101  ....v.sNt...t...
 000013f0: 7258 7401 a006 7400 a101 6e02 6407 7401  rXt...t...n.d.t.
 00001400: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
 00001410: a006 7c03 a101 7401 a006 7c04 a101 6408  ..|...t...|...d.
 00001420: 9c05 1600 7d06 6409 640a 7c06 6901 1600  ....}.d.d.|.i...
 00001430: 7d07 7407 7401 a008 7c07 a101 8301 8201  }.t.t...|.......
 00001440: 6400 0400 7d01 0400 7d02 0400 7d03 0400  d...}...}...}...
-00001450: 7d05 7d04 6400 5300 290b 4e72 3f00 0000  }.}.d.S.).Nr?...
+00001450: 7d05 7d04 6400 5300 290b 4e72 3e00 0000  }.}.d.S.).Nr>...
 00001460: 4672 2300 0000 7a43 5345 4c45 4354 2066  Fr#...zCSELECT f
 00001470: 312c 2066 3220 4652 4f4d 2061 2049 4e4e  1, f2 FROM a INN
 00001480: 4552 204a 4f49 4e20 6220 4f4e 2028 612e  ER JOIN b ON (a.
 00001490: 625f 6964 203d 2062 2e69 6429 2057 4845  b_id = b.id) WHE
 000014a0: 5245 2061 2e66 3220 3d20 2372 0400 0000  RE a.f2 = #r....
 000014b0: 7225 0000 0072 0200 0000 7226 0000 0072  r%...r....r&...r
 000014c0: 2800 0000 7229 0000 0072 0e00 0000 722a  (...r)...r....r*
 000014d0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
 000014e0: 0000 da1d 7465 7374 5f73 656c 6563 745f  ....test_select_
 000014f0: 6a6f 696e 5f73 686f 775f 636f 6c75 6d6e  join_show_column
-00001500: 7352 0000 0073 0200 0000 0001 7241 0000  sR...s......rA..
+00001500: 7352 0000 0073 0200 0000 0001 7240 0000  sR...s......r@..
 00001510: 0063 0000 0000 0000 0000 0000 0000 0600  .c..............
 00001520: 0000 0700 0000 4300 0000 73a0 0000 0064  ......C...s....d
 00001530: 017d 0074 007c 0083 017d 0164 027d 027c  .}.t.|...}.d.}.|
 00001540: 017c 026b 027d 037c 0373 8c74 01a0 0264  .|.k.}.|.s.t...d
 00001550: 037c 0366 0164 047c 017c 0266 02a1 0464  .|.f.d.|.|.f...d
 00001560: 0574 03a0 04a1 0076 0073 4674 01a0 0574  .t.....v.sFt...t
 00001570: 00a1 0172 5074 01a0 0674 00a1 016e 0264  ...rPt...t...n.d
@@ -352,15 +352,15 @@
 000015f0: 5920 6633 7a1d 5345 4c45 4354 202e 2e2e  Y f3z.SELECT ...
 00001600: 2046 524f 4d20 6120 4f52 4445 5220 4259   FROM a ORDER BY
 00001610: 2066 3372 0400 0000 7206 0000 0072 0200   f3r....r....r..
 00001620: 0000 7207 0000 0072 0c00 0000 720d 0000  ..r....r....r...
 00001630: 0072 0e00 0000 7217 0000 0072 1e00 0000  .r....r....r....
 00001640: 721e 0000 0072 1f00 0000 da14 7465 7374  r....r......test
 00001650: 5f73 656c 6563 745f 6f72 6465 725f 6279  _select_order_by
-00001660: 5c00 0000 7302 0000 0000 0172 4300 0000  \...s......rC...
+00001660: 5c00 0000 7302 0000 0000 0172 4200 0000  \...s......rB...
 00001670: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
 00001680: 0007 0000 0043 0000 0073 a000 0000 6401  .....C...s....d.
 00001690: 7d00 7400 7c00 8301 7d01 6402 7d02 7c01  }.t.|...}.d.}.|.
 000016a0: 7c02 6b02 7d03 7c03 738c 7401 a002 6403  |.k.}.|.s.t...d.
 000016b0: 7c03 6601 6404 7c01 7c02 6602 a104 6405  |.f.d.|.|.f...d.
 000016c0: 7403 a004 a100 7600 7346 7401 a005 7400  t.....v.sFt...t.
 000016d0: a101 7250 7401 a006 7400 a101 6e02 6405  ..rPt...t...n.d.
@@ -376,35 +376,35 @@
 00001770: 4f52 4445 5220 4259 2066 3320 4c49 4d49  ORDER BY f3 LIMI
 00001780: 5420 2372 0400 0000 7206 0000 0072 0200  T #r....r....r..
 00001790: 0000 7207 0000 0072 0c00 0000 720d 0000  ..r....r....r...
 000017a0: 0072 0e00 0000 7217 0000 0072 1e00 0000  .r....r....r....
 000017b0: 721e 0000 0072 1f00 0000 da1a 7465 7374  r....r......test
 000017c0: 5f73 656c 6563 745f 6f72 6465 725f 6279  _select_order_by
 000017d0: 5f6c 696d 6974 6300 0000 7302 0000 0000  _limitc...s.....
-000017e0: 0172 4400 0000 6301 0000 0000 0000 0000  .rD...c.........
+000017e0: 0172 4300 0000 6301 0000 0000 0000 0000  .rC...c.........
 000017f0: 0000 0008 0000 0008 0000 0043 0000 0073  ...........C...s
 00001800: b400 0000 6401 7d01 6402 7d02 7400 7c01  ....d.}.d.}.t.|.
 00001810: 7c02 6403 8d02 7d03 6401 7d04 7c03 7c04  |.d...}.d.}.|.|.
 00001820: 6b02 7d05 7c05 739c 7401 a002 6404 7c05  k.}.|.s.t...d.|.
 00001830: 6601 6405 7c03 7c04 6602 a104 6406 7403  f.d.|.|.f...d.t.
 00001840: a004 a100 7600 734e 7401 a005 7400 a101  ....v.sNt...t...
 00001850: 7258 7401 a006 7400 a101 6e02 6406 7401  rXt...t...n.d.t.
 00001860: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
 00001870: a006 7c03 a101 7401 a006 7c04 a101 6407  ..|...t...|...d.
 00001880: 9c05 1600 7d06 6408 6409 7c06 6901 1600  ....}.d.d.|.i...
 00001890: 7d07 7407 7401 a008 7c07 a101 8301 8201  }.t.t...|.......
 000018a0: 6400 0400 7d01 0400 7d02 0400 7d03 0400  d...}...}...}...
-000018b0: 7d05 7d04 6400 5300 290a 4e72 4200 0000  }.}.d.S.).NrB...
+000018b0: 7d05 7d04 6400 5300 290a 4e72 4100 0000  }.}.d.S.).NrA...
 000018c0: 4672 2300 0000 7204 0000 0072 2500 0000  Fr#...r....r%...
 000018d0: 7202 0000 0072 2600 0000 7228 0000 0072  r....r&...r(...r
 000018e0: 2900 0000 720e 0000 0072 2a00 0000 721e  )...r....r*...r.
 000018f0: 0000 0072 1e00 0000 721f 0000 00da 2174  ...r....r.....!t
 00001900: 6573 745f 7365 6c65 6374 5f6f 7264 6572  est_select_order
 00001910: 5f62 795f 7368 6f77 5f63 6f6c 756d 6e73  _by_show_columns
-00001920: 6a00 0000 7302 0000 0000 0172 4500 0000  j...s......rE...
+00001920: 6a00 0000 7302 0000 0000 0172 4400 0000  j...s......rD...
 00001930: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
 00001940: 0007 0000 0043 0000 0073 a000 0000 6401  .....C...s....d.
 00001950: 7d00 7400 7c00 8301 7d01 6402 7d02 7c01  }.t.|...}.d.}.|.
 00001960: 7c02 6b02 7d03 7c03 738c 7401 a002 6403  |.k.}.|.s.t...d.
 00001970: 7c03 6601 6404 7c01 7c02 6602 a104 6405  |.f.d.|.|.f...d.
 00001980: 7403 a004 a100 7600 7346 7401 a005 7400  t.....v.sFt...t.
 00001990: a101 7250 7401 a006 7400 a101 6e02 6405  ..rPt...t...n.d.
@@ -419,15 +419,15 @@
 00001a20: 2e2e 2e20 4652 4f4d 2061 204f 5244 4552  ... FROM a ORDER
 00001a30: 2042 5920 6633 2c20 6634 7204 0000 0072   BY f3, f4r....r
 00001a40: 0600 0000 7202 0000 0072 0700 0000 720c  ....r....r....r.
 00001a50: 0000 0072 0d00 0000 720e 0000 0072 1700  ...r....r....r..
 00001a60: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
 00001a70: 00da 1d74 6573 745f 7365 6c65 6374 5f6f  ...test_select_o
 00001a80: 7264 6572 5f62 795f 6d75 6c74 6970 6c65  rder_by_multiple
-00001a90: 7100 0000 7302 0000 0000 0172 4600 0000  q...s......rF...
+00001a90: 7100 0000 7302 0000 0000 0172 4500 0000  q...s......rE...
 00001aa0: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
 00001ab0: 0007 0000 0043 0000 0073 a000 0000 6401  .....C...s....d.
 00001ac0: 7d00 7400 7c00 8301 7d01 6402 7d02 7c01  }.t.|...}.d.}.|.
 00001ad0: 7c02 6b02 7d03 7c03 738c 7401 a002 6403  |.k.}.|.s.t...d.
 00001ae0: 7c03 6601 6404 7c01 7c02 6602 a104 6405  |.f.d.|.|.f...d.
 00001af0: 7403 a004 a100 7600 7346 7401 a005 7400  t.....v.sFt...t.
 00001b00: a101 7250 7401 a006 7400 a101 6e02 6405  ..rPt...t...n.d.
@@ -441,36 +441,36 @@
 00001b80: 2066 317a 1d53 454c 4543 5420 2e2e 2e20   f1z.SELECT ... 
 00001b90: 4652 4f4d 2061 2047 524f 5550 2042 5920  FROM a GROUP BY 
 00001ba0: 6631 7204 0000 0072 0600 0000 7202 0000  f1r....r....r...
 00001bb0: 0072 0700 0000 720c 0000 0072 0d00 0000  .r....r....r....
 00001bc0: 720e 0000 0072 1700 0000 721e 0000 0072  r....r....r....r
 00001bd0: 1e00 0000 721f 0000 00da 1474 6573 745f  ....r......test_
 00001be0: 7365 6c65 6374 5f67 726f 7570 5f62 7978  select_group_byx
-00001bf0: 0000 0073 0200 0000 0001 7248 0000 0063  ...s......rH...c
+00001bf0: 0000 0073 0200 0000 0001 7247 0000 0063  ...s......rG...c
 00001c00: 0100 0000 0000 0000 0000 0000 0800 0000  ................
 00001c10: 0800 0000 4300 0000 73b4 0000 0064 017d  ....C...s....d.}
 00001c20: 0164 027d 0274 007c 017c 0264 038d 027d  .d.}.t.|.|.d...}
 00001c30: 0364 017d 047c 037c 046b 027d 057c 0573  .d.}.|.|.k.}.|.s
 00001c40: 9c74 01a0 0264 047c 0566 0164 057c 037c  .t...d.|.f.d.|.|
 00001c50: 0466 02a1 0464 0674 03a0 04a1 0076 0073  .f...d.t.....v.s
 00001c60: 4e74 01a0 0574 00a1 0172 5874 01a0 0674  Nt...t...rXt...t
 00001c70: 00a1 016e 0264 0674 01a0 067c 01a1 0174  ...n.d.t...|...t
 00001c80: 01a0 067c 02a1 0174 01a0 067c 03a1 0174  ...|...t...|...t
 00001c90: 01a0 067c 04a1 0164 079c 0516 007d 0664  ...|...d.....}.d
 00001ca0: 0864 097c 0669 0116 007d 0774 0774 01a0  .d.|.i...}.t.t..
 00001cb0: 087c 07a1 0183 0182 0164 0004 007d 0104  .|.......d...}..
 00001cc0: 007d 0204 007d 0304 007d 057d 0464 0053  .}...}...}.}.d.S
-00001cd0: 0029 0a4e 7247 0000 0046 7223 0000 0072  .).NrG...Fr#...r
+00001cd0: 0029 0a4e 7246 0000 0046 7223 0000 0072  .).NrF...Fr#...r
 00001ce0: 0400 0000 7225 0000 0072 0200 0000 7226  ....r%...r....r&
 00001cf0: 0000 0072 2800 0000 7229 0000 0072 0e00  ...r(...r)...r..
 00001d00: 0000 722a 0000 0072 1e00 0000 721e 0000  ..r*...r....r...
 00001d10: 0072 1f00 0000 da21 7465 7374 5f73 656c  .r.....!test_sel
 00001d20: 6563 745f 6772 6f75 705f 6279 5f73 686f  ect_group_by_sho
 00001d30: 775f 636f 6c75 6d6e 737f 0000 0073 0200  w_columns....s..
-00001d40: 0000 0001 7249 0000 0063 0000 0000 0000  ....rI...c......
+00001d40: 0000 0001 7248 0000 0063 0000 0000 0000  ....rH...c......
 00001d50: 0000 0000 0000 0600 0000 0700 0000 4300  ..............C.
 00001d60: 0000 73a0 0000 0064 017d 0074 007c 0083  ..s....d.}.t.|..
 00001d70: 017d 0164 027d 027c 017c 026b 027d 037c  .}.d.}.|.|.k.}.|
 00001d80: 0373 8c74 01a0 0264 037c 0366 0164 047c  .s.t...d.|.f.d.|
 00001d90: 017c 0266 02a1 0464 0574 03a0 04a1 0076  .|.f...d.t.....v
 00001da0: 0073 4674 01a0 0574 00a1 0172 5074 01a0  .sFt...t...rPt..
 00001db0: 0674 00a1 016e 0264 0574 01a0 067c 00a1  .t...n.d.t...|..
@@ -485,15 +485,15 @@
 00001e40: 4d20 6120 4752 4f55 5020 4259 2066 312c  M a GROUP BY f1,
 00001e50: 2066 3272 0400 0000 7206 0000 0072 0200   f2r....r....r..
 00001e60: 0000 7207 0000 0072 0c00 0000 720d 0000  ..r....r....r...
 00001e70: 0072 0e00 0000 7217 0000 0072 1e00 0000  .r....r....r....
 00001e80: 721e 0000 0072 1f00 0000 da1d 7465 7374  r....r......test
 00001e90: 5f73 656c 6563 745f 6772 6f75 705f 6279  _select_group_by
 00001ea0: 5f6d 756c 7469 706c 6586 0000 0073 0200  _multiple....s..
-00001eb0: 0000 0001 724a 0000 0063 0000 0000 0000  ....rJ...c......
+00001eb0: 0000 0001 7249 0000 0063 0000 0000 0000  ....rI...c......
 00001ec0: 0000 0000 0000 0600 0000 0700 0000 4300  ..............C.
 00001ed0: 0000 73a0 0000 0064 017d 0074 007c 0083  ..s....d.}.t.|..
 00001ee0: 017d 0164 027d 027c 017c 026b 027d 037c  .}.d.}.|.|.k.}.|
 00001ef0: 0373 8c74 01a0 0264 037c 0366 0164 047c  .s.t...d.|.f.d.|
 00001f00: 017c 0266 02a1 0464 0574 03a0 04a1 0076  .|.f...d.t.....v
 00001f10: 0073 4674 01a0 0574 00a1 0172 5074 01a0  .sFt...t...rPt..
 00001f20: 0674 00a1 016e 0264 0574 01a0 067c 00a1  .t...n.d.t...|..
@@ -509,39 +509,39 @@
 00001fc0: 524f 5550 2042 5920 6631 2048 4156 494e  ROUP BY f1 HAVIN
 00001fd0: 4720 6631 203e 2023 7204 0000 0072 0600  G f1 > #r....r..
 00001fe0: 0000 7202 0000 0072 0700 0000 720c 0000  ..r....r....r...
 00001ff0: 0072 0d00 0000 720e 0000 0072 1700 0000  .r....r....r....
 00002000: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
 00002010: 1b74 6573 745f 7365 6c65 6374 5f67 726f  .test_select_gro
 00002020: 7570 5f62 795f 6861 7669 6e67 8d00 0000  up_by_having....
-00002030: 7302 0000 0000 0172 4c00 0000 6301 0000  s......rL...c...
+00002030: 7302 0000 0000 0172 4b00 0000 6301 0000  s......rK...c...
 00002040: 0000 0000 0000 0000 0008 0000 0008 0000  ................
 00002050: 0043 0000 0073 b400 0000 6401 7d01 6402  .C...s....d.}.d.
 00002060: 7d02 7400 7c01 7c02 6403 8d02 7d03 6404  }.t.|.|.d...}.d.
 00002070: 7d04 7c03 7c04 6b02 7d05 7c05 739c 7401  }.|.|.k.}.|.s.t.
 00002080: a002 6405 7c05 6601 6406 7c03 7c04 6602  ..d.|.f.d.|.|.f.
 00002090: a104 6407 7403 a004 a100 7600 734e 7401  ..d.t.....v.sNt.
 000020a0: a005 7400 a101 7258 7401 a006 7400 a101  ..t...rXt...t...
 000020b0: 6e02 6407 7401 a006 7c01 a101 7401 a006  n.d.t...|...t...
 000020c0: 7c02 a101 7401 a006 7c03 a101 7401 a006  |...t...|...t...
 000020d0: 7c04 a101 6408 9c05 1600 7d06 6409 640a  |...d.....}.d.d.
 000020e0: 7c06 6901 1600 7d07 7407 7401 a008 7c07  |.i...}.t.t...|.
 000020f0: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
 00002100: 0400 7d03 0400 7d05 7d04 6400 5300 290b  ..}...}.}.d.S.).
-00002110: 4e72 4b00 0000 4672 2300 0000 7a2e 5345  NrK...Fr#...z.SE
+00002110: 4e72 4a00 0000 4672 2300 0000 7a2e 5345  NrJ...Fr#...z.SE
 00002120: 4c45 4354 2066 312c 2066 3220 4652 4f4d  LECT f1, f2 FROM
 00002130: 2061 2047 524f 5550 2042 5920 6631 2048   a GROUP BY f1 H
 00002140: 4156 494e 4720 6631 203e 2023 7204 0000  AVING f1 > #r...
 00002150: 0072 2500 0000 7202 0000 0072 2600 0000  .r%...r....r&...
 00002160: 7228 0000 0072 2900 0000 720e 0000 0072  r(...r)...r....r
 00002170: 2a00 0000 721e 0000 0072 1e00 0000 721f  *...r....r....r.
 00002180: 0000 00da 2874 6573 745f 7365 6c65 6374  ....(test_select
 00002190: 5f67 726f 7570 5f62 795f 6861 7669 6e67  _group_by_having
 000021a0: 5f73 686f 775f 636f 6c75 6d6e 7394 0000  _show_columns...
-000021b0: 0073 0200 0000 0001 724d 0000 0063 0000  .s......rM...c..
+000021b0: 0073 0200 0000 0001 724c 0000 0063 0000  .s......rL...c..
 000021c0: 0000 0000 0000 0000 0000 0600 0000 0700  ................
 000021d0: 0000 4300 0000 73a0 0000 0064 017d 0074  ..C...s....d.}.t
 000021e0: 007c 0083 017d 0164 027d 027c 017c 026b  .|...}.d.}.|.|.k
 000021f0: 027d 037c 0373 8c74 01a0 0264 037c 0366  .}.|.s.t...d.|.f
 00002200: 0164 047c 017c 0266 02a1 0464 0574 03a0  .d.|.|.f...d.t..
 00002210: 04a1 0076 0073 4674 01a0 0574 00a1 0172  ...v.sFt...t...r
 00002220: 5074 01a0 0674 00a1 016e 0264 0574 01a0  Pt...t...n.d.t..
@@ -559,15 +559,15 @@
 000022e0: 3120 3e20 232c 2066 3220 3c20 2372 0400  1 > #, f2 < #r..
 000022f0: 0000 7206 0000 0072 0200 0000 7207 0000  ..r....r....r...
 00002300: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
 00002310: 7217 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
 00002320: 1f00 0000 da24 7465 7374 5f73 656c 6563  .....$test_selec
 00002330: 745f 6772 6f75 705f 6279 5f68 6176 696e  t_group_by_havin
 00002340: 675f 6d75 6c74 6970 6c65 9d00 0000 7302  g_multiple....s.
-00002350: 0000 0000 0172 4e00 0000 6300 0000 0000  .....rN...c.....
+00002350: 0000 0000 0172 4d00 0000 6300 0000 0000  .....rM...c.....
 00002360: 0000 0000 0000 0006 0000 0007 0000 0043  ...............C
 00002370: 0000 0073 a000 0000 6401 7d00 7400 7c00  ...s....d.}.t.|.
 00002380: 8301 7d01 6402 7d02 7c01 7c02 6b02 7d03  ..}.d.}.|.|.k.}.
 00002390: 7c03 738c 7401 a002 6403 7c03 6601 6404  |.s.t...d.|.f.d.
 000023a0: 7c01 7c02 6602 a104 6405 7403 a004 a100  |.|.f...d.t.....
 000023b0: 7600 7346 7401 a005 7400 a101 7250 7401  v.sFt...t...rPt.
 000023c0: a006 7400 a101 6e02 6405 7401 a006 7c00  ..t...n.d.t...|.
@@ -582,38 +582,38 @@
 00002450: 494e 5345 5254 2049 4e54 4f20 6074 6162  INSERT INTO `tab
 00002460: 6c65 6020 282e 2e2e 2920 5641 4c55 4553  le` (...) VALUES
 00002470: 2028 2e2e 2e29 7204 0000 0072 0600 0000   (...)r....r....
 00002480: 7202 0000 0072 0700 0000 720c 0000 0072  r....r....r....r
 00002490: 0d00 0000 720e 0000 0072 1700 0000 721e  ....r....r....r.
 000024a0: 0000 0072 1e00 0000 721f 0000 00da 0b74  ...r....r......t
 000024b0: 6573 745f 696e 7365 7274 a400 0000 7302  est_insert....s.
-000024c0: 0000 0000 0172 5000 0000 6301 0000 0000  .....rP...c.....
+000024c0: 0000 0000 0172 4f00 0000 6301 0000 0000  .....rO...c.....
 000024d0: 0000 0000 0000 0008 0000 0008 0000 0043  ...............C
 000024e0: 0000 0073 b400 0000 6401 7d01 6402 7d02  ...s....d.}.d.}.
 000024f0: 7400 7c01 7c02 6403 8d02 7d03 6404 7d04  t.|.|.d...}.d.}.
 00002500: 7c03 7c04 6b02 7d05 7c05 739c 7401 a002  |.|.k.}.|.s.t...
 00002510: 6405 7c05 6601 6406 7c03 7c04 6602 a104  d.|.f.d.|.|.f...
 00002520: 6407 7403 a004 a100 7600 734e 7401 a005  d.t.....v.sNt...
 00002530: 7400 a101 7258 7401 a006 7400 a101 6e02  t...rXt...t...n.
 00002540: 6407 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
 00002550: a101 7401 a006 7c03 a101 7401 a006 7c04  ..t...|...t...|.
 00002560: a101 6408 9c05 1600 7d06 6409 640a 7c06  ..d.....}.d.d.|.
 00002570: 6901 1600 7d07 7407 7401 a008 7c07 a101  i...}.t.t...|...
 00002580: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
 00002590: 7d03 0400 7d05 7d04 6400 5300 290b 4e72  }...}.}.d.S.).Nr
-000025a0: 4f00 0000 4672 2300 0000 7a2e 494e 5345  O...Fr#...z.INSE
+000025a0: 4e00 0000 4672 2300 0000 7a2e 494e 5345  N...Fr#...z.INSE
 000025b0: 5254 2049 4e54 4f20 6074 6162 6c65 6020  RT INTO `table` 
 000025c0: 2860 6631 602c 2060 6632 6029 2056 414c  (`f1`, `f2`) VAL
 000025d0: 5545 5320 2823 2c20 2329 7204 0000 0072  UES (#, #)r....r
 000025e0: 2500 0000 7202 0000 0072 2600 0000 7228  %...r....r&...r(
 000025f0: 0000 0072 2900 0000 720e 0000 0072 2a00  ...r)...r....r*.
 00002600: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
 00002610: 00da 1874 6573 745f 696e 7365 7274 5f73  ...test_insert_s
 00002620: 686f 775f 636f 6c75 6d6e 73ab 0000 0073  how_columns....s
-00002630: 0200 0000 0001 7251 0000 0063 0000 0000  ......rQ...c....
+00002630: 0200 0000 0001 7250 0000 0063 0000 0000  ......rP...c....
 00002640: 0000 0000 0000 0000 0600 0000 0700 0000  ................
 00002650: 4300 0000 73a0 0000 0064 017d 0074 007c  C...s....d.}.t.|
 00002660: 0083 017d 0164 027d 027c 017c 026b 027d  ...}.d.}.|.|.k.}
 00002670: 037c 0373 8c74 01a0 0264 037c 0366 0164  .|.s.t...d.|.f.d
 00002680: 047c 017c 0266 02a1 0464 0574 03a0 04a1  .|.|.f...d.t....
 00002690: 0076 0073 4674 01a0 0574 00a1 0172 5074  .v.sFt...t...rPt
 000026a0: 01a0 0674 00a1 016e 0264 0574 01a0 067c  ...t...n.d.t...|
@@ -629,15 +629,15 @@
 00002740: 6162 6c65 6020 5345 5420 2e2e 2e20 5748  able` SET ... WH
 00002750: 4552 4520 6074 6162 6c65 602e 6069 6460  ERE `table`.`id`
 00002760: 203d 2023 7204 0000 0072 0600 0000 7202   = #r....r....r.
 00002770: 0000 0072 0700 0000 720c 0000 0072 0d00  ...r....r....r..
 00002780: 0000 720e 0000 0072 1700 0000 721e 0000  ..r....r....r...
 00002790: 0072 1e00 0000 721f 0000 00da 0b74 6573  .r....r......tes
 000027a0: 745f 7570 6461 7465 b400 0000 7302 0000  t_update....s...
-000027b0: 0000 0172 5200 0000 6300 0000 0000 0000  ...rR...c.......
+000027b0: 0000 0172 5100 0000 6300 0000 0000 0000  ...rQ...c.......
 000027c0: 0000 0000 0006 0000 0007 0000 0043 0000  .............C..
 000027d0: 0073 a000 0000 6401 7d00 7400 7c00 8301  .s....d.}.t.|...
 000027e0: 7d01 6402 7d02 7c01 7c02 6b02 7d03 7c03  }.d.}.|.|.k.}.|.
 000027f0: 738c 7401 a002 6403 7c03 6601 6404 7c01  s.t...d.|.f.d.|.
 00002800: 7c02 6602 a104 6405 7403 a004 a100 7600  |.f...d.t.....v.
 00002810: 7346 7401 a005 7400 a101 7250 7401 a006  sFt...t...rPt...
 00002820: 7400 a101 6e02 6405 7401 a006 7c00 a101  t...n.d.t...|...
@@ -654,15 +654,15 @@
 000028d0: 6f5f 6375 7273 5f23 2220 4e4f 2053 4352  o_curs_#" NO SCR
 000028e0: 4f4c 4c20 4355 5253 4f52 2057 4954 484f  OLL CURSOR WITHO
 000028f0: 5554 7204 0000 0072 0600 0000 7202 0000  UTr....r....r...
 00002900: 0072 0700 0000 720c 0000 0072 0d00 0000  .r....r....r....
 00002910: 720e 0000 0072 1700 0000 721e 0000 0072  r....r....r....r
 00002920: 1e00 0000 721f 0000 00da 1374 6573 745f  ....r......test_
 00002930: 6465 636c 6172 655f 6375 7273 6f72 bb00  declare_cursor..
-00002940: 0000 7302 0000 0000 0172 5300 0000 6300  ..s......rS...c.
+00002940: 0000 7302 0000 0000 0172 5200 0000 6300  ..s......rR...c.
 00002950: 0000 0000 0000 0000 0000 0006 0000 0007  ................
 00002960: 0000 0043 0000 0073 a000 0000 6401 7d00  ...C...s....d.}.
 00002970: 7400 7c00 8301 7d01 6402 7d02 7c01 7c02  t.|...}.d.}.|.|.
 00002980: 6b02 7d03 7c03 738c 7401 a002 6403 7c03  k.}.|.s.t...d.|.
 00002990: 6601 6404 7c01 7c02 6602 a104 6405 7403  f.d.|.|.f...d.t.
 000029a0: a004 a100 7600 7346 7401 a005 7400 a101  ....v.sFt...t...
 000029b0: 7250 7401 a006 7400 a101 6e02 6405 7401  rPt...t...n.d.t.
@@ -675,15 +675,15 @@
 00002a20: 3332 3338 3039 3636 3237 3834 5f78 3534  323809662784_x54
 00002a30: 607a 0d53 4156 4550 4f49 4e54 2060 2360  `z.SAVEPOINT `#`
 00002a40: 7204 0000 0072 0600 0000 7202 0000 0072  r....r....r....r
 00002a50: 0700 0000 720c 0000 0072 0d00 0000 720e  ....r....r....r.
 00002a60: 0000 0072 1700 0000 721e 0000 0072 1e00  ...r....r....r..
 00002a70: 0000 721f 0000 00da 0e74 6573 745f 7361  ..r......test_sa
 00002a80: 7665 706f 696e 74c4 0000 0073 0200 0000  vepoint....s....
-00002a90: 0001 7254 0000 0063 0000 0000 0000 0000  ..rT...c........
+00002a90: 0001 7253 0000 0063 0000 0000 0000 0000  ..rS...c........
 00002aa0: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
 00002ab0: 73a0 0000 0064 017d 0074 007c 0083 017d  s....d.}.t.|...}
 00002ac0: 0164 027d 027c 017c 026b 027d 037c 0373  .d.}.|.|.k.}.|.s
 00002ad0: 8c74 01a0 0264 037c 0366 0164 047c 017c  .t...d.|.f.d.|.|
 00002ae0: 0266 02a1 0464 0574 03a0 04a1 0076 0073  .f...d.t.....v.s
 00002af0: 4674 01a0 0574 00a1 0172 5074 01a0 0674  Ft...t...rPt...t
 00002b00: 00a1 016e 0264 0574 01a0 067c 00a1 0174  ...n.d.t...|...t
@@ -698,15 +698,15 @@
 00002b90: 2054 4f20 5341 5645 504f 494e 5420 6023   TO SAVEPOINT `#
 00002ba0: 6072 0400 0000 7206 0000 0072 0200 0000  `r....r....r....
 00002bb0: 7207 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
 00002bc0: 0e00 0000 7217 0000 0072 1e00 0000 721e  ....r....r....r.
 00002bd0: 0000 0072 1f00 0000 da1a 7465 7374 5f72  ...r......test_r
 00002be0: 6f6c 6c62 6163 6b5f 746f 5f73 6176 6570  ollback_to_savep
 00002bf0: 6f69 6e74 c800 0000 7302 0000 0000 0172  oint....s......r
-00002c00: 5500 0000 6300 0000 0000 0000 0000 0000  U...c...........
+00002c00: 5400 0000 6300 0000 0000 0000 0000 0000  T...c...........
 00002c10: 0006 0000 0007 0000 0043 0000 0073 a000  .........C...s..
 00002c20: 0000 6401 7d00 7400 7c00 8301 7d01 6402  ..d.}.t.|...}.d.
 00002c30: 7d02 7c01 7c02 6b02 7d03 7c03 738c 7401  }.|.|.k.}.|.s.t.
 00002c40: a002 6403 7c03 6601 6404 7c01 7c02 6602  ..d.|.f.d.|.|.f.
 00002c50: a104 6405 7403 a004 a100 7600 7346 7401  ..d.t.....v.sFt.
 00002c60: a005 7400 a101 7250 7401 a006 7400 a101  ..t...rPt...t...
 00002c70: 6e02 6405 7401 a006 7c00 a101 7401 a006  n.d.t...|...t...
@@ -720,15 +720,15 @@
 00002cf0: 1552 454c 4541 5345 2053 4156 4550 4f49  .RELEASE SAVEPOI
 00002d00: 4e54 2060 2360 7204 0000 0072 0600 0000  NT `#`r....r....
 00002d10: 7202 0000 0072 0700 0000 720c 0000 0072  r....r....r....r
 00002d20: 0d00 0000 720e 0000 0072 1700 0000 721e  ....r....r....r.
 00002d30: 0000 0072 1e00 0000 721f 0000 00da 1674  ...r....r......t
 00002d40: 6573 745f 7265 6c65 6173 655f 7361 7665  est_release_save
 00002d50: 706f 696e 74cf 0000 0073 0200 0000 0001  point....s......
-00002d60: 7256 0000 0063 0000 0000 0000 0000 0000  rV...c..........
+00002d60: 7255 0000 0063 0000 0000 0000 0000 0000  rU...c..........
 00002d70: 0000 0700 0000 0800 0000 4300 0000 73b4  ..........C...s.
 00002d80: 0000 0064 017d 0064 027d 0174 007c 007c  ...d.}.d.}.t.|.|
 00002d90: 0164 038d 027d 0264 047d 037c 027c 036b  .d...}.d.}.|.|.k
 00002da0: 027d 047c 0473 9c74 01a0 0264 057c 0466  .}.|.s.t...d.|.f
 00002db0: 0164 067c 027c 0366 02a1 0464 0774 03a0  .d.|.|.f...d.t..
 00002dc0: 04a1 0076 0073 4e74 01a0 0574 00a1 0172  ...v.sNt...t...r
 00002dd0: 5874 01a0 0674 00a1 016e 0264 0774 01a0  Xt...t...n.d.t..
@@ -747,15 +747,15 @@
 00002ea0: 6560 2049 5320 2372 0400 0000 7225 0000  e` IS #r....r%..
 00002eb0: 0072 0200 0000 7226 0000 0072 2800 0000  .r....r&...r(...
 00002ec0: 7229 0000 0072 0e00 0000 a907 7218 0000  r)...r......r...
 00002ed0: 0072 1900 0000 721b 0000 0072 2c00 0000  .r....r....r,...
 00002ee0: 722d 0000 0072 1d00 0000 722e 0000 0072  r-...r....r....r
 00002ef0: 1e00 0000 721e 0000 0072 1f00 0000 da0f  ....r....r......
 00002f00: 7465 7374 5f6e 756c 6c5f 7661 6c75 65d6  test_null_value.
-00002f10: 0000 0073 0200 0000 0001 7258 0000 0063  ...s......rX...c
+00002f10: 0000 0073 0200 0000 0001 7257 0000 0063  ...s......rW...c
 00002f20: 0000 0000 0000 0000 0000 0000 0600 0000  ................
 00002f30: 0700 0000 4300 0000 73a0 0000 0064 017d  ....C...s....d.}
 00002f40: 0074 007c 0083 017d 0164 027d 027c 017c  .t.|...}.d.}.|.|
 00002f50: 026b 027d 037c 0373 8c74 01a0 0264 037c  .k.}.|.s.t...d.|
 00002f60: 0366 0164 047c 017c 0266 02a1 0464 0574  .f.d.|.|.f...d.t
 00002f70: 03a0 04a1 0076 0073 4674 01a0 0574 00a1  .....v.sFt...t..
 00002f80: 0172 5074 01a0 0674 00a1 016e 0264 0574  .rPt...t...n.d.t
@@ -773,15 +773,15 @@
 00003040: 4520 6062 602e 6066 3160 2049 5320 2320  E `b`.`f1` IS # 
 00003050: 4c49 4d49 5420 2372 0400 0000 7206 0000  LIMIT #r....r...
 00003060: 0072 0200 0000 7207 0000 0072 0c00 0000  .r....r....r....
 00003070: 720d 0000 0072 0e00 0000 7217 0000 0072  r....r....r....r
 00003080: 1e00 0000 721e 0000 0072 1f00 0000 da20  ....r....r..... 
 00003090: 7465 7374 5f73 7472 6970 5f64 7570 6c69  test_strip_dupli
 000030a0: 6361 7465 5f77 6869 7465 7370 6163 6573  cate_whitespaces
-000030b0: df00 0000 7302 0000 0000 0172 5900 0000  ....s......rY...
+000030b0: df00 0000 7302 0000 0000 0172 5800 0000  ....s......rX...
 000030c0: 6300 0000 0000 0000 0000 0000 0007 0000  c...............
 000030d0: 0008 0000 0043 0000 0073 b400 0000 6401  .....C...s....d.
 000030e0: 7d00 6402 7d01 7400 7c00 7c01 6403 8d02  }.d.}.t.|.|.d...
 000030f0: 7d02 6404 7d03 7c02 7c03 6b02 7d04 7c04  }.d.}.|.|.k.}.|.
 00003100: 739c 7401 a002 6405 7c04 6601 6406 7c02  s.t...d.|.f.d.|.
 00003110: 7c03 6602 a104 6407 7403 a004 a100 7600  |.f...d.t.....v.
 00003120: 734e 7401 a005 7400 a101 7258 7401 a006  sNt...t...rXt...
@@ -806,19 +806,19 @@
 00003250: 3e23 2c20 622e 6633 2d3e 3e23 2c20 2329  >#, b.f3->>#, #)
 00003260: 2920 4652 4f4d 2060 6260 2057 4845 5245  ) FROM `b` WHERE
 00003270: 2028 6062 602e 6066 3160 2049 5320 2320   (`b`.`f1` IS # 
 00003280: 4f52 2028 4558 4953 5453 2043 4f55 4e54  OR (EXISTS COUNT
 00003290: 2823 2929 2920 4c49 4d49 5420 2372 0400  (#))) LIMIT #r..
 000032a0: 0000 7225 0000 0072 0200 0000 7226 0000  ..r%...r....r&..
 000032b0: 0072 2800 0000 7229 0000 0072 0e00 0000  .r(...r)...r....
-000032c0: 7257 0000 0072 1e00 0000 721e 0000 0072  rW...r....r....r
+000032c0: 7256 0000 0072 1e00 0000 721e 0000 0072  rV...r....r....r
 000032d0: 1f00 0000 da2a 7465 7374 5f73 7472 6970  .....*test_strip
 000032e0: 5f64 7570 6c69 6361 7465 5f77 6869 7465  _duplicate_white
 000032f0: 7370 6163 6573 5f72 6563 7572 7369 7665  spaces_recursive
-00003300: e800 0000 7302 0000 0000 0172 5a00 0000  ....s......rZ...
+00003300: e800 0000 7302 0000 0000 0172 5900 0000  ....s......rY...
 00003310: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
 00003320: 0007 0000 0043 0000 0073 a000 0000 6401  .....C...s....d.
 00003330: 7d00 7400 7c00 8301 7d01 6402 7d02 7c01  }.t.|...}.d.}.|.
 00003340: 7c02 6b02 7d03 7c03 738c 7401 a002 6403  |.k.}.|.s.t...d.
 00003350: 7c03 6601 6404 7c01 7c02 6602 a104 6405  |.f.d.|.|.f...d.
 00003360: 7403 a004 a100 7600 7346 7401 a005 7400  t.....v.sFt...t.
 00003370: a101 7250 7401 a006 7400 a101 6e02 6405  ..rPt...t...n.d.
@@ -832,15 +832,15 @@
 000033f0: 494d 4954 2031 320a 0a7a 1b53 454c 4543  IMIT 12..z.SELEC
 00003400: 5420 2e2e 2e20 4652 4f4d 2060 6260 204c  T ... FROM `b` L
 00003410: 494d 4954 2023 7204 0000 0072 0600 0000  IMIT #r....r....
 00003420: 7202 0000 0072 0700 0000 720c 0000 0072  r....r....r....r
 00003430: 0d00 0000 720e 0000 0072 1700 0000 721e  ....r....r....r.
 00003440: 0000 0072 1e00 0000 721f 0000 00da 1374  ...r....r......t
 00003450: 6573 745f 7374 7269 705f 6e65 776c 696e  est_strip_newlin
-00003460: 6573 f400 0000 7302 0000 0000 0172 5b00  es....s......r[.
+00003460: 6573 f400 0000 7302 0000 0000 0172 5a00  es....s......rZ.
 00003470: 0000 6300 0000 0000 0000 0000 0000 000a  ..c.............
 00003480: 0000 0009 0000 0043 0000 0073 d800 0000  .......C...s....
 00003490: 6401 7d00 7400 7c00 8301 7d01 6402 7d02  d.}.t.|...}.d.}.
 000034a0: 6403 7d03 7c02 7c03 1700 7d04 6404 7d05  d.}.|.|...}.d.}.
 000034b0: 7c04 7c05 1700 7d06 7c01 7c06 6b02 7d07  |.|...}.|.|.k.}.
 000034c0: 7c07 73b4 7401 a002 6405 7c07 6601 6406  |.s.t...d.|.f.d.
 000034d0: 7c01 7c06 6602 a104 6407 7403 a004 a100  |.|.f...d.t.....
@@ -887,15 +887,15 @@
 00003760: 0000 0072 2c00 0000 7235 0000 0072 3400  ...r,...r5...r4.
 00003770: 0000 da0c 4070 795f 6173 7365 7274 3133  ....@py_assert13
 00003780: 721b 0000 005a 0c40 7079 5f66 6f72 6d61  r....Z.@py_forma
 00003790: 7431 345a 0c40 7079 5f66 6f72 6d61 7431  t14Z.@py_format1
 000037a0: 3672 1e00 0000 721e 0000 0072 1f00 0000  6r....r....r....
 000037b0: da14 7465 7374 5f73 7472 6970 5f72 6177  ..test_strip_raw
 000037c0: 5f71 7565 7279 fb00 0000 7302 0000 0000  _query....s.....
-000037d0: 0172 5d00 0000 6300 0000 0000 0000 0000  .r]...c.........
+000037d0: 0172 5c00 0000 6300 0000 0000 0000 0000  .r\...c.........
 000037e0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
 000037f0: a000 0000 6401 7d00 7400 7c00 8301 7d01  ....d.}.t.|...}.
 00003800: 6402 7d02 7c01 7c02 6b02 7d03 7c03 738c  d.}.|.|.k.}.|.s.
 00003810: 7401 a002 6403 7c03 6601 6404 7c01 7c02  t...d.|.f.d.|.|.
 00003820: 6602 a104 6405 7403 a004 a100 7600 7346  f...d.t.....v.sF
 00003830: 7401 a005 7400 a101 7250 7401 a006 7400  t...t...rPt...t.
 00003840: a101 6e02 6405 7401 a006 7c00 a101 7401  ..n.d.t...|...t.
@@ -910,15 +910,15 @@
 000038d0: 2046 524f 4d20 6062 6020 5748 4552 4520   FROM `b` WHERE 
 000038e0: 6078 6020 494e 2028 2329 7204 0000 0072  `x` IN (#)r....r
 000038f0: 0600 0000 7202 0000 0072 0700 0000 720c  ....r....r....r.
 00003900: 0000 0072 0d00 0000 720e 0000 0072 1700  ...r....r....r..
 00003910: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
 00003920: 00da 1474 6573 745f 696e 5f73 696e 676c  ...test_in_singl
 00003930: 655f 7661 6c75 6513 0100 0073 0200 0000  e_value....s....
-00003940: 0001 725e 0000 0063 0000 0000 0000 0000  ..r^...c........
+00003940: 0001 725d 0000 0063 0000 0000 0000 0000  ..r]...c........
 00003950: 0000 0000 0600 0000 0700 0000 4300 0000  ............C...
 00003960: 73a0 0000 0064 017d 0074 007c 0083 017d  s....d.}.t.|...}
 00003970: 0164 027d 027c 017c 026b 027d 037c 0373  .d.}.|.|.k.}.|.s
 00003980: 8c74 01a0 0264 037c 0366 0164 047c 017c  .t...d.|.f.d.|.|
 00003990: 0266 02a1 0464 0574 03a0 04a1 0076 0073  .f...d.t.....v.s
 000039a0: 4674 01a0 0574 00a1 0172 5074 01a0 0674  Ft...t...rPt...t
 000039b0: 00a1 016e 0264 0574 01a0 067c 00a1 0174  ...n.d.t...|...t
@@ -933,15 +933,15 @@
 00003a40: 4543 5420 2e2e 2e20 4652 4f4d 2060 6260  ECT ... FROM `b`
 00003a50: 2057 4845 5245 2060 7860 2049 4e20 282e   WHERE `x` IN (.
 00003a60: 2e2e 2972 0400 0000 7206 0000 0072 0200  ..)r....r....r..
 00003a70: 0000 7207 0000 0072 0c00 0000 720d 0000  ..r....r....r...
 00003a80: 0072 0e00 0000 7217 0000 0072 1e00 0000  .r....r....r....
 00003a90: 721e 0000 0072 1f00 0000 da17 7465 7374  r....r......test
 00003aa0: 5f69 6e5f 6d75 6c74 6970 6c65 5f76 616c  _in_multiple_val
-00003ab0: 7565 731a 0100 0073 0200 0000 0001 725f  ues....s......r_
+00003ab0: 7565 731a 0100 0073 0200 0000 0001 725e  ues....s......r^
 00003ac0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00003ad0: 0600 0000 0700 0000 4300 0000 73a0 0000  ........C...s...
 00003ae0: 0064 017d 0074 007c 0083 017d 0164 027d  .d.}.t.|...}.d.}
 00003af0: 027c 017c 026b 027d 037c 0373 8c74 01a0  .|.|.k.}.|.s.t..
 00003b00: 0264 037c 0366 0164 047c 017c 0266 02a1  .d.|.f.d.|.|.f..
 00003b10: 0464 0574 03a0 04a1 0076 0073 4674 01a0  .d.t.....v.sFt..
 00003b20: 0574 00a1 0172 5074 01a0 0674 00a1 016e  .t...rPt...t...n
@@ -960,15 +960,15 @@
 00003bf0: 2e2e 2e29 2041 4e44 2060 7960 2049 4e20  ...) AND `y` IN 
 00003c00: 282e 2e2e 2972 0400 0000 7206 0000 0072  (...)r....r....r
 00003c10: 0200 0000 7207 0000 0072 0c00 0000 720d  ....r....r....r.
 00003c20: 0000 0072 0e00 0000 7217 0000 0072 1e00  ...r....r....r..
 00003c30: 0000 721e 0000 0072 1f00 0000 da18 7465  ..r....r......te
 00003c40: 7374 5f69 6e5f 6d75 6c74 6970 6c65 5f63  st_in_multiple_c
 00003c50: 6c61 7573 6573 2101 0000 7302 0000 0000  lauses!...s.....
-00003c60: 0172 6000 0000 6300 0000 0000 0000 0000  .r`...c.........
+00003c60: 0172 5f00 0000 6300 0000 0000 0000 0000  .r_...c.........
 00003c70: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
 00003c80: a000 0000 6401 7d00 7400 7c00 8301 7d01  ....d.}.t.|...}.
 00003c90: 6402 7d02 7c01 7c02 6b02 7d03 7c03 738c  d.}.|.|.k.}.|.s.
 00003ca0: 7401 a002 6403 7c03 6601 6404 7c01 7c02  t...d.|.f.d.|.|.
 00003cb0: 6602 a104 6405 7403 a004 a100 7600 7346  f...d.t.....v.sF
 00003cc0: 7401 a005 7400 a101 7250 7401 a006 7400  t...t...rPt...t.
 00003cd0: a101 6e02 6405 7401 a006 7c00 a101 7401  ..n.d.t...|...t.
@@ -987,15 +987,15 @@
 00003da0: 2860 7960 203d 2023 204f 5220 6079 6020  (`y` = # OR `y` 
 00003db0: 3d20 2329 7204 0000 0072 0600 0000 7202  = #)r....r....r.
 00003dc0: 0000 0072 0700 0000 720c 0000 0072 0d00  ...r....r....r..
 00003dd0: 0000 720e 0000 0072 1700 0000 721e 0000  ..r....r....r...
 00003de0: 0072 1e00 0000 721f 0000 00da 2274 6573  .r....r....."tes
 00003df0: 745f 696e 5f6d 756c 7469 706c 655f 7661  t_in_multiple_va
 00003e00: 6c75 6573 5f61 6e64 5f63 6c61 7573 652a  lues_and_clause*
-00003e10: 0100 0073 0200 0000 0001 7261 0000 0063  ...s......ra...c
+00003e10: 0100 0073 0200 0000 0001 7260 0000 0063  ...s......r`...c
 00003e20: 0000 0000 0000 0000 0000 0000 0600 0000  ................
 00003e30: 0700 0000 4300 0000 73a0 0000 0064 017d  ....C...s....d.}
 00003e40: 0074 007c 0083 017d 0164 027d 027c 017c  .t.|...}.d.}.|.|
 00003e50: 026b 027d 037c 0373 8c74 01a0 0264 037c  .k.}.|.s.t...d.|
 00003e60: 0366 0164 047c 017c 0266 02a1 0464 0574  .f.d.|.|.f...d.t
 00003e70: 03a0 04a1 0076 0073 4674 01a0 0574 00a1  .....v.sFt...t..
 00003e80: 0172 5074 01a0 0674 00a1 016e 0264 0574  .rPt...t...n.d.t
@@ -1011,33 +1011,33 @@
 00003f20: 2046 524f 4d20 6062 6020 5748 4552 4520   FROM `b` WHERE 
 00003f30: 6078 6020 494e 2028 5345 4c45 4354 2023  `x` IN (SELECT #
 00003f40: 2972 0400 0000 7206 0000 0072 0200 0000  )r....r....r....
 00003f50: 7207 0000 0072 0c00 0000 720d 0000 0072  r....r....r....r
 00003f60: 0e00 0000 7217 0000 0072 1e00 0000 721e  ....r....r....r.
 00003f70: 0000 0072 1f00 0000 da10 7465 7374 5f69  ...r......test_i
 00003f80: 6e5f 7375 6271 7565 7279 3301 0000 7302  n_subquery3...s.
-00003f90: 0000 0000 0172 6200 0000 292e da08 6275  .....rb...)...bu
+00003f90: 0000 0000 0172 6100 0000 292e da08 6275  .....ra...)...bu
 00003fa0: 696c 7469 6e73 7211 0000 00da 195f 7079  iltinsr......_py
 00003fb0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
 00003fc0: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
 00003fd0: 6eda 0772 6577 7269 7465 720f 0000 00da  n..rewriter.....
 00003fe0: 1364 6a61 6e67 6f5f 7065 7266 5f72 6563  .django_perf_rec
 00003ff0: 2e73 716c 7202 0000 0072 2000 0000 7222  .sqlr....r ...r"
-00004000: 0000 0072 2f00 0000 7230 0000 0072 3700  ...r/...r0...r7.
-00004010: 0000 723a 0000 0072 3b00 0000 723d 0000  ..r:...r;...r=..
-00004020: 0072 3e00 0000 7240 0000 0072 4100 0000  .r>...r@...rA...
-00004030: 7243 0000 0072 4400 0000 7245 0000 0072  rC...rD...rE...r
-00004040: 4600 0000 7248 0000 0072 4900 0000 724a  F...rH...rI...rJ
-00004050: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
-00004060: 0000 7250 0000 0072 5100 0000 7252 0000  ..rP...rQ...rR..
-00004070: 0072 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
-00004080: 7256 0000 0072 5800 0000 7259 0000 0072  rV...rX...rY...r
-00004090: 5a00 0000 725b 0000 0072 5d00 0000 725e  Z...r[...r]...r^
-000040a0: 0000 0072 5f00 0000 7260 0000 0072 6100  ...r_...r`...ra.
-000040b0: 0000 7262 0000 0072 1e00 0000 721e 0000  ..rb...r....r...
+00004000: 0000 0072 2f00 0000 7230 0000 0072 3600  ...r/...r0...r6.
+00004010: 0000 7239 0000 0072 3a00 0000 723c 0000  ..r9...r:...r<..
+00004020: 0072 3d00 0000 723f 0000 0072 4000 0000  .r=...r?...r@...
+00004030: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
+00004040: 4500 0000 7247 0000 0072 4800 0000 7249  E...rG...rH...rI
+00004050: 0000 0072 4b00 0000 724c 0000 0072 4d00  ...rK...rL...rM.
+00004060: 0000 724f 0000 0072 5000 0000 7251 0000  ..rO...rP...rQ..
+00004070: 0072 5200 0000 7253 0000 0072 5400 0000  .rR...rS...rT...
+00004080: 7255 0000 0072 5700 0000 7258 0000 0072  rU...rW...rX...r
+00004090: 5900 0000 725a 0000 0072 5c00 0000 725d  Y...rZ...r\...r]
+000040a0: 0000 0072 5e00 0000 725f 0000 0072 6000  ...r^...r_...r`.
+000040b0: 0000 7261 0000 0072 1e00 0000 721e 0000  ..ra...r....r...
 000040c0: 0072 1e00 0000 721f 0000 00da 083c 6d6f  .r....r......<mo
 000040d0: 6475 6c65 3e01 0000 0073 4c00 0000 2603  dule>....sL...&.
 000040e0: 0805 0804 0807 0807 080d 0809 080a 0807  ................
 000040f0: 0807 0809 080a 0807 0807 0807 0807 0807  ................
 00004100: 0807 0807 0807 0809 0807 0807 0809 0807  ................
 00004110: 0809 0804 0807 0807 0809 0809 080c 0807  ................
 00004120: 0818 0807 0807 0809 0809                 ..........
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-37-pytest-5.4.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 420d 0d0a 914c 075d bc04 0000 e300 0000  B....L.]........
+00000000: 420d 0d0a 35fa 535e bc04 0000 e300 0000  B...5.S^........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 5a00 0000 6400 6401 6c00 5a01 6400  .sZ...d.d.l.Z.d.
 00000030: 6401 6c02 6d03 0200 0100 6d04 5a05 0100  d.l.m.....m.Z...
 00000040: 6400 6402 6c06 6d07 5a07 0100 6400 6403  d.d.l.m.Z...d.d.
 00000050: 6c08 6d09 5a09 6d0a 5a0a 0100 4700 6404  l.m.Z.m.Z...G.d.
 00000060: 6405 8400 6405 6507 8303 5a0b 4700 6406  d...d.e...Z.G.d.
 00000070: 6407 8400 6407 6507 8303 5a0c 6401 5300  d...d.e...Z.d.S.
@@ -367,14 +367,14 @@
 000016e0: 0000 7224 0000 0072 2f00 0000 1a00 0000  ..r$...r/.......
 000016f0: 730a 0000 0008 0108 0308 0308 0308 0372  s..............r
 00001700: 2f00 0000 290d da08 6275 696c 7469 6e73  /...)...builtins
 00001710: 7213 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
 00001720: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
 00001730: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
 00001740: 7269 7465 7211 0000 00da 0b64 6a61 6e67  riter......djang
-00001750: 6f2e 7465 7374 7202 0000 005a 1564 6a61  o.testr....Z.dja
+00001750: 6f2e 7465 7374 7202 0000 00da 1564 6a61  o.testr......dja
 00001760: 6e67 6f5f 7065 7266 5f72 6563 2e75 7469  ngo_perf_rec.uti
 00001770: 6c73 7203 0000 0072 0400 0000 7205 0000  lsr....r....r...
 00001780: 0072 2f00 0000 7223 0000 0072 2300 0000  .r/...r#...r#...
 00001790: 7223 0000 0072 2400 0000 da08 3c6d 6f64  r#...r$.....<mod
 000017a0: 756c 653e 0100 0000 730a 0000 0008 0012  ule>....s.......
 000017b0: 000c 0210 0310 14                        .......
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-38-pytest-5.4.2.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,380 +1,336 @@
-00000000: 420d 0d0a 35fa 535e bc04 0000 e300 0000  B...5.S^........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 5a00 0000 6400 6401 6c00 5a01 6400  .sZ...d.d.l.Z.d.
-00000030: 6401 6c02 6d03 0200 0100 6d04 5a05 0100  d.l.m.....m.Z...
-00000040: 6400 6402 6c06 6d07 5a07 0100 6400 6403  d.d.l.m.Z...d.d.
-00000050: 6c08 6d09 5a09 6d0a 5a0a 0100 4700 6404  l.m.Z.m.Z...G.d.
-00000060: 6405 8400 6405 6507 8303 5a0b 4700 6406  d...d.e...Z.G.d.
-00000070: 6407 8400 6407 6507 8303 5a0c 6401 5300  d...d.e...Z.d.S.
-00000080: 2908 e900 0000 004e 2901 da0e 5369 6d70  )......N)...Simp
-00000090: 6c65 5465 7374 4361 7365 2902 da0c 6375  leTestCase)...cu
-000000a0: 7272 656e 745f 7465 7374 da0c 736f 7274  rrent_test..sort
-000000b0: 6564 5f6e 616d 6573 6300 0000 0000 0000  ed_namesc.......
-000000c0: 0000 0000 0002 0000 0040 0000 0073 2400  .........@...s$.
-000000d0: 0000 6500 5a01 6400 5a02 6401 6402 8400  ..e.Z.d.Z.d.d...
-000000e0: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
-000000f0: 5a05 6407 5300 2908 da10 4375 7272 656e  Z.d.S.)...Curren
-00000100: 7454 6573 7454 6573 7473 6301 0000 0000  tTestTestsc.....
-00000110: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
-00000120: c201 0000 7400 8300 7d01 7c01 6a01 7d02  ....t...}.|.j.}.
-00000130: 7c02 7402 6b02 7d03 7c03 739a 7403 a004  |.t.k.}.|.s.t...
-00000140: 6401 7c03 6601 6402 7c02 7402 6602 a104  d.|.f.d.|.t.f...
-00000150: 6403 7405 a006 a100 6b06 7342 7403 a007  d.t.....k.sBt...
-00000160: 7c01 a101 724c 7403 a008 7c01 a101 6e02  |...rLt...|...n.
-00000170: 6403 7403 a008 7c02 a101 6404 7405 a006  d.t...|...d.t...
-00000180: a100 6b06 736c 7403 a007 7402 a101 7276  ..k.slt...t...rv
-00000190: 7403 a008 7402 a101 6e02 6404 6405 9c03  t...t...n.d.d...
-000001a0: 1600 7d04 6406 6407 7c04 6901 1600 7d05  ..}.d.d.|.i...}.
-000001b0: 7409 7403 a00a 7c05 a101 8301 8201 6400  t.t...|.......d.
-000001c0: 0400 7d02 7d03 7c01 6a0b 7d02 6408 7d06  ..}.}.|.j.}.d.}.
-000001d0: 7c02 7c06 6b02 7d03 7c03 9001 7322 7403  |.|.k.}.|...s"t.
-000001e0: a004 6401 7c03 6601 6409 7c02 7c06 6602  ..d.|.f.d.|.|.f.
-000001f0: a104 6403 7405 a006 a100 6b06 73e4 7403  ..d.t.....k.s.t.
-00000200: a007 7c01 a101 72ee 7403 a008 7c01 a101  ..|...r.t...|...
-00000210: 6e02 6403 7403 a008 7c02 a101 7403 a008  n.d.t...|...t...
-00000220: 7c06 a101 640a 9c03 1600 7d07 640b 640c  |...d.....}.d.d.
-00000230: 7c07 6901 1600 7d08 7409 7403 a00a 7c08  |.i...}.t.t...|.
-00000240: a101 8301 8201 6400 0400 7d02 0400 7d03  ......d...}...}.
-00000250: 7d06 7c01 6a0c 7d02 640d 7d06 7c02 7c06  }.|.j.}.d.}.|.|.
-00000260: 6b02 7d03 7c03 9001 73b2 7403 a004 6401  k.}.|...s.t...d.
-00000270: 7c03 6601 640e 7c02 7c06 6602 a104 6403  |.f.d.|.|.f...d.
-00000280: 7405 a006 a100 6b06 9001 7374 7403 a007  t.....k...stt...
-00000290: 7c01 a101 9001 727e 7403 a008 7c01 a101  |.....r~t...|...
-000002a0: 6e02 6403 7403 a008 7c02 a101 7403 a008  n.d.t...|...t...
-000002b0: 7c06 a101 640a 9c03 1600 7d07 640b 640c  |...d.....}.d.d.
-000002c0: 7c07 6901 1600 7d08 7409 7403 a00a 7c08  |.i...}.t.t...|.
-000002d0: a101 8301 8201 6400 0400 7d02 0400 7d03  ......d...}...}.
-000002e0: 7d06 6400 5300 290f 4e29 01fa 023d 3d29  }.d.S.).N)...==)
-000002f0: 017a 3125 2870 7932 2973 0a7b 2528 7079  .z1%(py2)s.{%(py
-00000300: 3229 7320 3d20 2528 7079 3029 732e 6669  2)s = %(py0)s.fi
-00000310: 6c65 5f70 6174 680a 7d20 3d3d 2025 2870  le_path.} == %(p
-00000320: 7934 2973 da07 6465 7461 696c 73da 085f  y4)s..details.._
-00000330: 5f66 696c 655f 5f29 03da 0370 7930 da03  _file__)...py0..
-00000340: 7079 32da 0370 7934 7a0e 6173 7365 7274  py2..py4z.assert
-00000350: 2025 2870 7936 2973 da03 7079 3672 0500   %(py6)s..py6r..
-00000360: 0000 2901 7a32 2528 7079 3229 730a 7b25  ..).z2%(py2)s.{%
-00000370: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
-00000380: 2e63 6c61 7373 5f6e 616d 650a 7d20 3d3d  .class_name.} ==
-00000390: 2025 2870 7935 2973 2903 7209 0000 0072   %(py5)s).r....r
-000003a0: 0a00 0000 da03 7079 357a 0e61 7373 6572  ......py5z.asser
-000003b0: 7420 2528 7079 3729 73da 0370 7937 da09  t %(py7)s..py7..
-000003c0: 7465 7374 5f68 6572 6529 017a 3125 2870  test_here).z1%(p
-000003d0: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
-000003e0: 2528 7079 3029 732e 7465 7374 5f6e 616d  %(py0)s.test_nam
-000003f0: 650a 7d20 3d3d 2025 2870 7935 2973 290d  e.} == %(py5)s).
-00000400: 7203 0000 00da 0966 696c 655f 7061 7468  r......file_path
-00000410: 7208 0000 00da 0a40 7079 7465 7374 5f61  r......@pytest_a
-00000420: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
-00000430: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
-00000440: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
-00000450: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
-00000460: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
-00000470: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000480: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000490: 7469 6f6e da0a 636c 6173 735f 6e61 6d65  tion..class_name
-000004a0: da09 7465 7374 5f6e 616d 6529 09da 0473  ..test_name)...s
-000004b0: 656c 6672 0700 0000 da0b 4070 795f 6173  elfr......@py_as
-000004c0: 7365 7274 31da 0b40 7079 5f61 7373 6572  sert1..@py_asser
-000004d0: 7433 da0b 4070 795f 666f 726d 6174 35da  t3..@py_format5.
-000004e0: 0b40 7079 5f66 6f72 6d61 7437 da0b 4070  .@py_format7..@p
-000004f0: 795f 6173 7365 7274 34da 0b40 7079 5f66  y_assert4..@py_f
-00000500: 6f72 6d61 7436 da0b 4070 795f 666f 726d  ormat6..@py_form
-00000510: 6174 38a9 0072 2300 0000 fa44 2f55 7365  at8..r#....D/Use
-00000520: 7273 2f63 6861 696e 7a2f 446f 6375 6d65  rs/chainz/Docume
-00000530: 6e74 732f 5072 6f6a 6563 7473 2f64 6a61  nts/Projects/dja
-00000540: 6e67 6f2d 7065 7266 2d72 6563 2f74 6573  ngo-perf-rec/tes
-00000550: 7473 2f74 6573 745f 7574 696c 732e 7079  ts/test_utils.py
-00000560: 720f 0000 0007 0000 0073 3000 0000 0001  r........s0.....
-00000570: 0601 0600 0800 0400 6800 0c00 0e00 0801  ........h.......
-00000580: 0600 0400 0800 0600 4e00 0c00 0e00 0c01  ........N.......
-00000590: 0600 0400 0800 0600 5200 0c00 0e00 7a1a  ........R.....z.
-000005a0: 4375 7272 656e 7454 6573 7454 6573 7473  CurrentTestTests
-000005b0: 2e74 6573 745f 6865 7265 6301 0000 0000  .test_herec.....
-000005c0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
-000005d0: b200 0000 7400 8300 7d01 7400 8300 7d02  ....t...}.t...}.
-000005e0: 7c01 7c02 6b02 7d03 7c03 73a2 7401 a002  |.|.k.}.|.s.t...
-000005f0: 6401 7c03 6601 6402 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
-00000600: 6403 7403 a004 a100 6b06 7342 7401 a005  d.t.....k.sBt...
-00000610: 7400 a101 724c 7401 a006 7400 a101 6e02  t...rLt...t...n.
-00000620: 6403 7401 a006 7c01 a101 6403 7403 a004  d.t...|...d.t...
-00000630: a100 6b06 736c 7401 a005 7400 a101 7276  ..k.slt...t...rv
-00000640: 7401 a006 7400 a101 6e02 6403 7401 a006  t...t...n.d.t...
-00000650: 7c02 a101 6404 9c04 1600 7d04 6405 6406  |...d.....}.d.d.
-00000660: 7c04 6901 1600 7d05 7407 7401 a008 7c05  |.i...}.t.t...|.
-00000670: a101 8301 8201 6400 0400 7d01 0400 7d03  ......d...}...}.
-00000680: 7d02 6400 5300 2907 4e29 0172 0600 0000  }.d.S.).N).r....
-00000690: 2901 7a40 2528 7079 3229 730a 7b25 2870  ).z@%(py2)s.{%(p
-000006a0: 7932 2973 203d 2025 2870 7930 2973 2829  y2)s = %(py0)s()
-000006b0: 0a7d 203d 3d20 2528 7079 3629 730a 7b25  .} == %(py6)s.{%
-000006c0: 2870 7936 2973 203d 2025 2870 7934 2973  (py6)s = %(py4)s
-000006d0: 2829 0a7d 7203 0000 0029 0472 0900 0000  ().}r....).r....
-000006e0: 720a 0000 0072 0b00 0000 720c 0000 007a  r....r....r....z
-000006f0: 0e61 7373 6572 7420 2528 7079 3829 73da  .assert %(py8)s.
-00000700: 0370 7938 2909 7203 0000 0072 1100 0000  .py8).r....r....
-00000710: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000720: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00000730: 0000 0029 0672 1b00 0000 721c 0000 00da  ...).r....r.....
-00000740: 0b40 7079 5f61 7373 6572 7435 721d 0000  .@py_assert5r...
-00000750: 0072 1f00 0000 da0b 4070 795f 666f 726d  .r......@py_form
-00000760: 6174 3972 2300 0000 7223 0000 0072 2400  at9r#...r#...r$.
-00000770: 0000 da0f 7465 7374 5f74 7769 6365 5f73  ....test_twice_s
-00000780: 616d 650d 0000 0073 1000 0000 0001 0600  ame....s........
-00000790: 0600 0800 0400 7000 0c00 0e00 7a20 4375  ......p.....z Cu
-000007a0: 7272 656e 7454 6573 7454 6573 7473 2e74  rrentTestTests.t
-000007b0: 6573 745f 7477 6963 655f 7361 6d65 6301  est_twice_samec.
-000007c0: 0000 0000 0000 000a 0000 0007 0000 0043  ...............C
-000007d0: 0000 0073 ca01 0000 6401 6402 8400 7d01  ...s....d.d...}.
-000007e0: 7c01 8300 7d02 7c02 6a00 7d03 7c03 7401  |...}.|.j.}.|.t.
-000007f0: 6b02 7d04 7c04 73a2 7402 a003 6403 7c04  k.}.|.s.t...d.|.
-00000800: 6601 6404 7c03 7401 6602 a104 6405 7404  f.d.|.t.f...d.t.
-00000810: a005 a100 6b06 734a 7402 a006 7c02 a101  ....k.sJt...|...
-00000820: 7254 7402 a007 7c02 a101 6e02 6405 7402  rTt...|...n.d.t.
-00000830: a007 7c03 a101 6406 7404 a005 a100 6b06  ..|...d.t.....k.
-00000840: 7374 7402 a006 7401 a101 727e 7402 a007  stt...t...r~t...
-00000850: 7401 a101 6e02 6406 6407 9c03 1600 7d05  t...n.d.d.....}.
-00000860: 6408 6409 7c05 6901 1600 7d06 7408 7402  d.d.|.i...}.t.t.
-00000870: a009 7c06 a101 8301 8201 6400 0400 7d03  ..|.......d...}.
-00000880: 7d04 7c02 6a0a 7d03 6400 7d07 7c03 7c07  }.|.j.}.d.}.|.|.
-00000890: 6b08 7d04 7c04 9001 732a 7402 a003 640a  k.}.|...s*t...d.
-000008a0: 7c04 6601 640b 7c03 7c07 6602 a104 6405  |.f.d.|.|.f...d.
-000008b0: 7404 a005 a100 6b06 73ec 7402 a006 7c02  t.....k.s.t...|.
-000008c0: a101 72f6 7402 a007 7c02 a101 6e02 6405  ..r.t...|...n.d.
-000008d0: 7402 a007 7c03 a101 7402 a007 7c07 a101  t...|...t...|...
-000008e0: 640c 9c03 1600 7d08 640d 640e 7c08 6901  d.....}.d.d.|.i.
-000008f0: 1600 7d09 7408 7402 a009 7c09 a101 8301  ..}.t.t...|.....
-00000900: 8201 6400 0400 7d03 0400 7d04 7d07 7c02  ..d...}...}.}.|.
-00000910: 6a0b 7d03 640f 7d07 7c03 7c07 6b02 7d04  j.}.d.}.|.|.k.}.
-00000920: 7c04 9001 73ba 7402 a003 6403 7c04 6601  |...s.t...d.|.f.
-00000930: 6410 7c03 7c07 6602 a104 6405 7404 a005  d.|.|.f...d.t...
-00000940: a100 6b06 9001 737c 7402 a006 7c02 a101  ..k...s|t...|...
-00000950: 9001 7286 7402 a007 7c02 a101 6e02 6405  ..r.t...|...n.d.
-00000960: 7402 a007 7c03 a101 7402 a007 7c07 a101  t...|...t...|...
-00000970: 640c 9c03 1600 7d08 640d 640e 7c08 6901  d.....}.d.d.|.i.
-00000980: 1600 7d09 7408 7402 a009 7c09 a101 8301  ..}.t.t...|.....
-00000990: 8201 6400 0400 7d03 0400 7d04 7d07 6400  ..d...}...}.}.d.
-000009a0: 5300 2911 4e63 0000 0000 0000 0000 0000  S.).Nc..........
-000009b0: 0000 0100 0000 5300 0000 7306 0000 0074  ......S...s....t
-000009c0: 0083 0053 0029 014e 2901 7203 0000 0072  ...S.).N).r....r
-000009d0: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
-000009e0: 0000 00da 1574 6573 745f 7468 6174 735f  .....test_thats_
-000009f0: 6675 6e63 7469 6f6e 616c 1100 0000 7302  functional....s.
-00000a00: 0000 0000 017a 3f43 7572 7265 6e74 5465  .....z?CurrentTe
-00000a10: 7374 5465 7374 732e 7465 7374 5f66 756e  stTests.test_fun
-00000a20: 6374 696f 6e61 6c2e 3c6c 6f63 616c 733e  ctional.<locals>
-00000a30: 2e74 6573 745f 7468 6174 735f 6675 6e63  .test_thats_func
-00000a40: 7469 6f6e 616c 2901 7206 0000 0029 017a  tional).r....).z
-00000a50: 3125 2870 7932 2973 0a7b 2528 7079 3229  1%(py2)s.{%(py2)
-00000a60: 7320 3d20 2528 7079 3029 732e 6669 6c65  s = %(py0)s.file
-00000a70: 5f70 6174 680a 7d20 3d3d 2025 2870 7934  _path.} == %(py4
-00000a80: 2973 7207 0000 0072 0800 0000 2903 7209  )sr....r....).r.
-00000a90: 0000 0072 0a00 0000 720b 0000 007a 0e61  ...r....r....z.a
-00000aa0: 7373 6572 7420 2528 7079 3629 7372 0c00  ssert %(py6)sr..
-00000ab0: 0000 2901 da02 6973 2901 7a32 2528 7079  ..)...is).z2%(py
-00000ac0: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
-00000ad0: 2870 7930 2973 2e63 6c61 7373 5f6e 616d  (py0)s.class_nam
-00000ae0: 650a 7d20 6973 2025 2870 7935 2973 2903  e.} is %(py5)s).
-00000af0: 7209 0000 0072 0a00 0000 720d 0000 007a  r....r....r....z
-00000b00: 0e61 7373 6572 7420 2528 7079 3729 7372  .assert %(py7)sr
-00000b10: 0e00 0000 7229 0000 0029 017a 3125 2870  ....r)...).z1%(p
-00000b20: 7932 2973 0a7b 2528 7079 3229 7320 3d20  y2)s.{%(py2)s = 
-00000b30: 2528 7079 3029 732e 7465 7374 5f6e 616d  %(py0)s.test_nam
-00000b40: 650a 7d20 3d3d 2025 2870 7935 2973 290c  e.} == %(py5)s).
-00000b50: 7210 0000 0072 0800 0000 7211 0000 0072  r....r....r....r
-00000b60: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
-00000b70: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
-00000b80: 0000 7219 0000 0072 1a00 0000 290a 721b  ..r....r....).r.
-00000b90: 0000 0072 2900 0000 7207 0000 0072 1c00  ...r)...r....r..
-00000ba0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000bb0: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
-00000bc0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00000bd0: 0f74 6573 745f 6675 6e63 7469 6f6e 616c  .test_functional
-00000be0: 1000 0000 7332 0000 0000 0108 0306 0106  ....s2..........
-00000bf0: 0008 0004 0068 000c 000e 0008 0106 0004  .....h..........
-00000c00: 0008 0006 004e 000c 000e 000c 0106 0004  .....N..........
-00000c10: 0008 0006 0052 000c 000e 007a 2043 7572  .....R.....z Cur
-00000c20: 7265 6e74 5465 7374 5465 7374 732e 7465  rentTestTests.te
-00000c30: 7374 5f66 756e 6374 696f 6e61 6c4e 2906  st_functionalN).
-00000c40: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000c50: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000c60: 6d65 5f5f 720f 0000 0072 2800 0000 722b  me__r....r(...r+
-00000c70: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
-00000c80: 0000 7224 0000 0072 0500 0000 0600 0000  ..r$...r........
-00000c90: 7306 0000 0008 0108 0608 0372 0500 0000  s..........r....
-00000ca0: 6300 0000 0000 0000 0000 0000 0002 0000  c...............
-00000cb0: 0040 0000 0073 3400 0000 6500 5a01 6400  .@...s4...e.Z.d.
-00000cc0: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
-00000cd0: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
-00000ce0: 5a06 6409 640a 8400 5a07 640b 5300 290c  Z.d.d...Z.d.S.).
-00000cf0: da10 536f 7274 6564 4e61 6d65 7354 6573  ..SortedNamesTes
-00000d00: 7473 6301 0000 0000 0000 0007 0000 0007  tsc.............
-00000d10: 0000 0043 0000 0073 a000 0000 6700 7d01  ...C...s....g.}.
-00000d20: 7400 7c01 8301 7d02 6700 7d03 7c02 7c03  t.|...}.g.}.|.|.
-00000d30: 6b02 7d04 7c04 738c 7401 a002 6401 7c04  k.}.|.s.t...d.|.
-00000d40: 6601 6402 7c02 7c03 6602 a104 6403 7403  f.d.|.|.f...d.t.
-00000d50: a004 a100 6b06 7346 7401 a005 7400 a101  ....k.sFt...t...
-00000d60: 7250 7401 a006 7400 a101 6e02 6403 7401  rPt...t...n.d.t.
-00000d70: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
-00000d80: a006 7c03 a101 6404 9c04 1600 7d05 6405  ..|...d.....}.d.
-00000d90: 6406 7c05 6901 1600 7d06 7407 7401 a008  d.|.i...}.t.t...
-00000da0: 7c06 a101 8301 8201 6400 0400 7d01 0400  |.......d...}...
-00000db0: 7d02 0400 7d04 7d03 6400 5300 2907 4e29  }...}.}.d.S.).N)
-00000dc0: 0172 0600 0000 2901 7a30 2528 7079 3429  .r....).z0%(py4)
-00000dd0: 730a 7b25 2870 7934 2973 203d 2025 2870  s.{%(py4)s = %(p
-00000de0: 7930 2973 2825 2870 7932 2973 290a 7d20  y0)s(%(py2)s).} 
-00000df0: 3d3d 2025 2870 7937 2973 7204 0000 0029  == %(py7)sr....)
-00000e00: 0472 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000e10: 720e 0000 007a 0e61 7373 6572 7420 2528  r....z.assert %(
-00000e20: 7079 3929 73da 0370 7939 2909 7204 0000  py9)s..py9).r...
-00000e30: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
-00000e40: 7214 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000e50: 1700 0000 7218 0000 0029 0772 1b00 0000  ....r....).r....
-00000e60: 721c 0000 0072 1d00 0000 da0b 4070 795f  r....r......@py_
-00000e70: 6173 7365 7274 3672 2600 0000 7222 0000  assert6r&...r"..
-00000e80: 00da 0c40 7079 5f66 6f72 6d61 7431 3072  ...@py_format10r
-00000e90: 2300 0000 7223 0000 0072 2400 0000 da0a  #...r#...r$.....
-00000ea0: 7465 7374 5f65 6d70 7479 1b00 0000 7312  test_empty....s.
-00000eb0: 0000 0000 0104 0008 0004 0008 0004 0056  ...............V
-00000ec0: 000c 000e 007a 1b53 6f72 7465 644e 616d  .....z.SortedNam
-00000ed0: 6573 5465 7374 732e 7465 7374 5f65 6d70  esTests.test_emp
-00000ee0: 7479 6301 0000 0000 0000 0007 0000 0007  tyc.............
-00000ef0: 0000 0043 0000 0073 a400 0000 6401 6701  ...C...s....d.g.
-00000f00: 7d01 7400 7c01 8301 7d02 6401 6701 7d03  }.t.|...}.d.g.}.
-00000f10: 7c02 7c03 6b02 7d04 7c04 7390 7401 a002  |.|.k.}.|.s.t...
-00000f20: 6402 7c04 6601 6403 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
-00000f30: 6404 7403 a004 a100 6b06 734a 7401 a005  d.t.....k.sJt...
-00000f40: 7400 a101 7254 7401 a006 7400 a101 6e02  t...rTt...t...n.
-00000f50: 6404 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
-00000f60: a101 7401 a006 7c03 a101 6405 9c04 1600  ..t...|...d.....
-00000f70: 7d05 6406 6407 7c05 6901 1600 7d06 7407  }.d.d.|.i...}.t.
-00000f80: 7401 a008 7c06 a101 8301 8201 6400 0400  t...|.......d...
-00000f90: 7d01 0400 7d02 0400 7d04 7d03 6400 5300  }...}...}.}.d.S.
-00000fa0: 2908 4eda 0764 6566 6175 6c74 2901 7206  ).N..default).r.
-00000fb0: 0000 0029 017a 3025 2870 7934 2973 0a7b  ...).z0%(py4)s.{
-00000fc0: 2528 7079 3429 7320 3d20 2528 7079 3029  %(py4)s = %(py0)
-00000fd0: 7328 2528 7079 3229 7329 0a7d 203d 3d20  s(%(py2)s).} == 
-00000fe0: 2528 7079 3729 7372 0400 0000 2904 7209  %(py7)sr....).r.
-00000ff0: 0000 0072 0a00 0000 720b 0000 0072 0e00  ...r....r....r..
-00001000: 0000 7a0e 6173 7365 7274 2025 2870 7939  ..z.assert %(py9
-00001010: 2973 7230 0000 0029 0972 0400 0000 7211  )sr0...).r....r.
-00001020: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
-00001030: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001040: 0072 1800 0000 2907 721b 0000 0072 1c00  .r....).r....r..
-00001050: 0000 721d 0000 0072 3100 0000 7226 0000  ..r....r1...r&..
-00001060: 0072 2200 0000 7232 0000 0072 2300 0000  .r"...r2...r#...
-00001070: 7223 0000 0072 2400 0000 da11 7465 7374  r#...r$.....test
-00001080: 5f6a 7573 745f 6465 6661 756c 741e 0000  _just_default...
-00001090: 0073 1200 0000 0001 0600 0800 0600 0800  .s..............
-000010a0: 0400 5600 0c00 0e00 7a22 536f 7274 6564  ..V.....z"Sorted
-000010b0: 4e61 6d65 7354 6573 7473 2e74 6573 745f  NamesTests.test_
-000010c0: 6a75 7374 5f64 6566 6175 6c74 6301 0000  just_defaultc...
-000010d0: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
-000010e0: 0073 a400 0000 6401 6701 7d01 7400 7c01  .s....d.g.}.t.|.
-000010f0: 8301 7d02 6401 6701 7d03 7c02 7c03 6b02  ..}.d.g.}.|.|.k.
-00001100: 7d04 7c04 7390 7401 a002 6402 7c04 6601  }.|.s.t...d.|.f.
-00001110: 6403 7c02 7c03 6602 a104 6404 7403 a004  d.|.|.f...d.t...
-00001120: a100 6b06 734a 7401 a005 7400 a101 7254  ..k.sJt...t...rT
-00001130: 7401 a006 7400 a101 6e02 6404 7401 a006  t...t...n.d.t...
-00001140: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
-00001150: 7c03 a101 6405 9c04 1600 7d05 6406 6407  |...d.....}.d.d.
-00001160: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
-00001170: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
-00001180: 0400 7d04 7d03 6400 5300 2908 4e5a 0973  ..}.}.d.S.).NZ.s
-00001190: 6f6d 6574 6869 6e67 2901 7206 0000 0029  omething).r....)
-000011a0: 017a 3025 2870 7934 2973 0a7b 2528 7079  .z0%(py4)s.{%(py
-000011b0: 3429 7320 3d20 2528 7079 3029 7328 2528  4)s = %(py0)s(%(
-000011c0: 7079 3229 7329 0a7d 203d 3d20 2528 7079  py2)s).} == %(py
-000011d0: 3729 7372 0400 0000 2904 7209 0000 0072  7)sr....).r....r
-000011e0: 0a00 0000 720b 0000 0072 0e00 0000 7a0e  ....r....r....z.
-000011f0: 6173 7365 7274 2025 2870 7939 2973 7230  assert %(py9)sr0
-00001200: 0000 0029 0972 0400 0000 7211 0000 0072  ...).r....r....r
-00001210: 1200 0000 7213 0000 0072 1400 0000 7215  ....r....r....r.
-00001220: 0000 0072 1600 0000 7217 0000 0072 1800  ...r....r....r..
-00001230: 0000 2907 721b 0000 0072 1c00 0000 721d  ..).r....r....r.
-00001240: 0000 0072 3100 0000 7226 0000 0072 2200  ...r1...r&...r".
-00001250: 0000 7232 0000 0072 2300 0000 7223 0000  ..r2...r#...r#..
-00001260: 0072 2400 0000 da13 7465 7374 5f6a 7573  .r$.....test_jus
-00001270: 745f 736f 6d65 7468 696e 6721 0000 0073  t_something!...s
-00001280: 1200 0000 0001 0600 0800 0600 0800 0400  ................
-00001290: 5600 0c00 0e00 7a24 536f 7274 6564 4e61  V.....z$SortedNa
-000012a0: 6d65 7354 6573 7473 2e74 6573 745f 6a75  mesTests.test_ju
-000012b0: 7374 5f73 6f6d 6574 6869 6e67 6301 0000  st_somethingc...
-000012c0: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
-000012d0: 0073 a800 0000 6401 6402 6702 7d01 7400  .s....d.d.g.}.t.
-000012e0: 7c01 8301 7d02 6402 6401 6702 7d03 7c02  |...}.d.d.g.}.|.
-000012f0: 7c03 6b02 7d04 7c04 7394 7401 a002 6403  |.k.}.|.s.t...d.
-00001300: 7c04 6601 6404 7c02 7c03 6602 a104 6405  |.f.d.|.|.f...d.
-00001310: 7403 a004 a100 6b06 734e 7401 a005 7400  t.....k.sNt...t.
-00001320: a101 7258 7401 a006 7400 a101 6e02 6405  ..rXt...t...n.d.
-00001330: 7401 a006 7c01 a101 7401 a006 7c02 a101  t...|...t...|...
-00001340: 7401 a006 7c03 a101 6406 9c04 1600 7d05  t...|...d.....}.
-00001350: 6407 6408 7c05 6901 1600 7d06 7407 7401  d.d.|.i...}.t.t.
-00001360: a008 7c06 a101 8301 8201 6400 0400 7d01  ..|.......d...}.
-00001370: 0400 7d02 0400 7d04 7d03 6400 5300 2909  ..}...}.}.d.S.).
-00001380: 4eda 0162 da01 6129 0172 0600 0000 2901  N..b..a).r....).
-00001390: 7a30 2528 7079 3429 730a 7b25 2870 7934  z0%(py4)s.{%(py4
-000013a0: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
-000013b0: 7932 2973 290a 7d20 3d3d 2025 2870 7937  y2)s).} == %(py7
-000013c0: 2973 7204 0000 0029 0472 0900 0000 720a  )sr....).r....r.
-000013d0: 0000 0072 0b00 0000 720e 0000 007a 0e61  ...r....r....z.a
-000013e0: 7373 6572 7420 2528 7079 3929 7372 3000  ssert %(py9)sr0.
-000013f0: 0000 2909 7204 0000 0072 1100 0000 7212  ..).r....r....r.
-00001400: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-00001410: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00001420: 0029 0772 1b00 0000 721c 0000 0072 1d00  .).r....r....r..
-00001430: 0000 7231 0000 0072 2600 0000 7222 0000  ..r1...r&...r"..
-00001440: 0072 3200 0000 7223 0000 0072 2300 0000  .r2...r#...r#...
-00001450: 7224 0000 00da 0e74 6573 745f 646f 6573  r$.....test_does
-00001460: 5f73 6f72 7424 0000 0073 1200 0000 0001  _sort$...s......
-00001470: 0800 0800 0800 0800 0400 5600 0c00 0e00  ..........V.....
-00001480: 7a1f 536f 7274 6564 4e61 6d65 7354 6573  z.SortedNamesTes
-00001490: 7473 2e74 6573 745f 646f 6573 5f73 6f72  ts.test_does_sor
-000014a0: 7463 0100 0000 0000 0000 0700 0000 0700  tc..............
-000014b0: 0000 4300 0000 73a8 0000 0064 0164 0267  ..C...s....d.d.g
-000014c0: 027d 0174 007c 0183 017d 0264 0264 0167  .}.t.|...}.d.d.g
-000014d0: 027d 037c 027c 036b 027d 047c 0473 9474  .}.|.|.k.}.|.s.t
-000014e0: 01a0 0264 037c 0466 0164 047c 027c 0366  ...d.|.f.d.|.|.f
-000014f0: 02a1 0464 0574 03a0 04a1 006b 0673 4e74  ...d.t.....k.sNt
-00001500: 01a0 0574 00a1 0172 5874 01a0 0674 00a1  ...t...rXt...t..
-00001510: 016e 0264 0574 01a0 067c 01a1 0174 01a0  .n.d.t...|...t..
-00001520: 067c 02a1 0174 01a0 067c 03a1 0164 069c  .|...t...|...d..
-00001530: 0416 007d 0564 0764 087c 0569 0116 007d  ...}.d.d.|.i...}
-00001540: 0674 0774 01a0 087c 06a1 0183 0182 0164  .t.t...|.......d
-00001550: 0004 007d 0104 007d 0204 007d 047d 0364  ...}...}...}.}.d
-00001560: 0053 0029 094e 7238 0000 0072 3400 0000  .S.).Nr8...r4...
-00001570: 2901 7206 0000 0029 017a 3025 2870 7934  ).r....).z0%(py4
-00001580: 2973 0a7b 2528 7079 3429 7320 3d20 2528  )s.{%(py4)s = %(
-00001590: 7079 3029 7328 2528 7079 3229 7329 0a7d  py0)s(%(py2)s).}
-000015a0: 203d 3d20 2528 7079 3729 7372 0400 0000   == %(py7)sr....
-000015b0: 2904 7209 0000 0072 0a00 0000 720b 0000  ).r....r....r...
-000015c0: 0072 0e00 0000 7a0e 6173 7365 7274 2025  .r....z.assert %
-000015d0: 2870 7939 2973 7230 0000 0029 0972 0400  (py9)sr0...).r..
-000015e0: 0000 7211 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000015f0: 0072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001600: 7217 0000 0072 1800 0000 2907 721b 0000  r....r....).r...
-00001610: 0072 1c00 0000 721d 0000 0072 3100 0000  .r....r....r1...
-00001620: 7226 0000 0072 2200 0000 7232 0000 0072  r&...r"...r2...r
-00001630: 2300 0000 7223 0000 0072 2400 0000 da1d  #...r#...r$.....
-00001640: 7465 7374 5f73 6f72 745f 6b65 6570 735f  test_sort_keeps_
-00001650: 6465 6661 756c 745f 6669 7273 7427 0000  default_first'..
-00001660: 0073 1200 0000 0001 0800 0800 0800 0800  .s..............
-00001670: 0400 5600 0c00 0e00 7a2e 536f 7274 6564  ..V.....z.Sorted
-00001680: 4e61 6d65 7354 6573 7473 2e74 6573 745f  NamesTests.test_
-00001690: 736f 7274 5f6b 6565 7073 5f64 6566 6175  sort_keeps_defau
-000016a0: 6c74 5f66 6972 7374 4e29 0872 2c00 0000  lt_firstN).r,...
-000016b0: 722d 0000 0072 2e00 0000 7233 0000 0072  r-...r....r3...r
-000016c0: 3500 0000 7236 0000 0072 3900 0000 723a  5...r6...r9...r:
-000016d0: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
-000016e0: 0000 7224 0000 0072 2f00 0000 1a00 0000  ..r$...r/.......
-000016f0: 730a 0000 0008 0108 0308 0308 0308 0372  s..............r
-00001700: 2f00 0000 290d da08 6275 696c 7469 6e73  /...)...builtins
-00001710: 7213 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
-00001720: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
-00001730: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
-00001740: 7269 7465 7211 0000 00da 0b64 6a61 6e67  riter......djang
-00001750: 6f2e 7465 7374 7202 0000 00da 1564 6a61  o.testr......dja
-00001760: 6e67 6f5f 7065 7266 5f72 6563 2e75 7469  ngo_perf_rec.uti
-00001770: 6c73 7203 0000 0072 0400 0000 7205 0000  lsr....r....r...
-00001780: 0072 2f00 0000 7223 0000 0072 2300 0000  .r/...r#...r#...
-00001790: 7223 0000 0072 2400 0000 da08 3c6d 6f64  r#...r$.....<mod
-000017a0: 756c 653e 0100 0000 730a 0000 0008 0012  ule>....s.......
-000017b0: 000c 0210 0310 14                        .......
+00000000: 550d 0d0a 35fa 535e bc04 0000 e300 0000  U...5.S^........
+00000010: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 5a00 0000 6400 6401 6c00  .@...sZ...d.d.l.
+00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
+00000040: 5a05 0100 6400 6402 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
+00000050: 6400 6403 6c08 6d09 5a09 6d0a 5a0a 0100  d.d.l.m.Z.m.Z...
+00000060: 4700 6404 6405 8400 6405 6507 8303 5a0b  G.d.d...d.e...Z.
+00000070: 4700 6406 6407 8400 6407 6507 8303 5a0c  G.d.d...d.e...Z.
+00000080: 6401 5300 2908 e900 0000 004e 2901 da0e  d.S.)......N)...
+00000090: 5369 6d70 6c65 5465 7374 4361 7365 2902  SimpleTestCase).
+000000a0: da0c 6375 7272 656e 745f 7465 7374 da0c  ..current_test..
+000000b0: 736f 7274 6564 5f6e 616d 6573 6300 0000  sorted_namesc...
+000000c0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+000000d0: 0040 0000 0073 2400 0000 6500 5a01 6400  .@...s$...e.Z.d.
+000000e0: 5a02 6401 6402 8400 5a03 6403 6404 8400  Z.d.d...Z.d.d...
+000000f0: 5a04 6405 6406 8400 5a05 6407 5300 2908  Z.d.d...Z.d.S.).
+00000100: da10 4375 7272 656e 7454 6573 7454 6573  ..CurrentTestTes
+00000110: 7473 6301 0000 0000 0000 0000 0000 0009  tsc.............
+00000120: 0000 0007 0000 0043 0000 0073 c201 0000  .......C...s....
+00000130: 7400 8300 7d01 7c01 6a01 7d02 7c02 7402  t...}.|.j.}.|.t.
+00000140: 6b02 7d03 7c03 739a 7403 a004 6401 7c03  k.}.|.s.t...d.|.
+00000150: 6601 6402 7c02 7402 6602 a104 6403 7405  f.d.|.t.f...d.t.
+00000160: a006 a100 6b06 7342 7403 a007 7c01 a101  ....k.sBt...|...
+00000170: 724c 7403 a008 7c01 a101 6e02 6403 7403  rLt...|...n.d.t.
+00000180: a008 7c02 a101 6404 7405 a006 a100 6b06  ..|...d.t.....k.
+00000190: 736c 7403 a007 7402 a101 7276 7403 a008  slt...t...rvt...
+000001a0: 7402 a101 6e02 6404 6405 9c03 1600 7d04  t...n.d.d.....}.
+000001b0: 6406 6407 7c04 6901 1600 7d05 7409 7403  d.d.|.i...}.t.t.
+000001c0: a00a 7c05 a101 8301 8201 6400 0400 7d02  ..|.......d...}.
+000001d0: 7d03 7c01 6a0b 7d02 6408 7d06 7c02 7c06  }.|.j.}.d.}.|.|.
+000001e0: 6b02 7d03 7c03 9001 7322 7403 a004 6401  k.}.|...s"t...d.
+000001f0: 7c03 6601 6409 7c02 7c06 6602 a104 6403  |.f.d.|.|.f...d.
+00000200: 7405 a006 a100 6b06 73e4 7403 a007 7c01  t.....k.s.t...|.
+00000210: a101 72ee 7403 a008 7c01 a101 6e02 6403  ..r.t...|...n.d.
+00000220: 7403 a008 7c02 a101 7403 a008 7c06 a101  t...|...t...|...
+00000230: 640a 9c03 1600 7d07 640b 640c 7c07 6901  d.....}.d.d.|.i.
+00000240: 1600 7d08 7409 7403 a00a 7c08 a101 8301  ..}.t.t...|.....
+00000250: 8201 6400 0400 7d02 0400 7d03 7d06 7c01  ..d...}...}.}.|.
+00000260: 6a0c 7d02 640d 7d06 7c02 7c06 6b02 7d03  j.}.d.}.|.|.k.}.
+00000270: 7c03 9001 73b2 7403 a004 6401 7c03 6601  |...s.t...d.|.f.
+00000280: 640e 7c02 7c06 6602 a104 6403 7405 a006  d.|.|.f...d.t...
+00000290: a100 6b06 9001 7374 7403 a007 7c01 a101  ..k...stt...|...
+000002a0: 9001 727e 7403 a008 7c01 a101 6e02 6403  ..r~t...|...n.d.
+000002b0: 7403 a008 7c02 a101 7403 a008 7c06 a101  t...|...t...|...
+000002c0: 640a 9c03 1600 7d07 640b 640c 7c07 6901  d.....}.d.d.|.i.
+000002d0: 1600 7d08 7409 7403 a00a 7c08 a101 8301  ..}.t.t...|.....
+000002e0: 8201 6400 0400 7d02 0400 7d03 7d06 6400  ..d...}...}.}.d.
+000002f0: 5300 290f 4ea9 01fa 023d 3da9 017a 3125  S.).N....==..z1%
+00000300: 2870 7932 2973 0a7b 2528 7079 3229 7320  (py2)s.{%(py2)s 
+00000310: 3d20 2528 7079 3029 732e 6669 6c65 5f70  = %(py0)s.file_p
+00000320: 6174 680a 7d20 3d3d 2025 2870 7934 2973  ath.} == %(py4)s
+00000330: da07 6465 7461 696c 73da 085f 5f66 696c  ..details..__fil
+00000340: 655f 5fa9 03da 0370 7930 da03 7079 32da  e__....py0..py2.
+00000350: 0370 7934 fa0e 6173 7365 7274 2025 2870  .py4..assert %(p
+00000360: 7936 2973 da03 7079 3672 0500 0000 2901  y6)s..py6r....).
+00000370: 7a32 2528 7079 3229 730a 7b25 2870 7932  z2%(py2)s.{%(py2
+00000380: 2973 203d 2025 2870 7930 2973 2e63 6c61  )s = %(py0)s.cla
+00000390: 7373 5f6e 616d 650a 7d20 3d3d 2025 2870  ss_name.} == %(p
+000003a0: 7935 2973 a903 720c 0000 0072 0d00 0000  y5)s..r....r....
+000003b0: da03 7079 35fa 0e61 7373 6572 7420 2528  ..py5..assert %(
+000003c0: 7079 3729 73da 0370 7937 da09 7465 7374  py7)s..py7..test
+000003d0: 5f68 6572 65a9 017a 3125 2870 7932 2973  _here..z1%(py2)s
+000003e0: 0a7b 2528 7079 3229 7320 3d20 2528 7079  .{%(py2)s = %(py
+000003f0: 3029 732e 7465 7374 5f6e 616d 650a 7d20  0)s.test_name.} 
+00000400: 3d3d 2025 2870 7935 2973 290d 7203 0000  == %(py5)s).r...
+00000410: 00da 0966 696c 655f 7061 7468 720a 0000  ...file_pathr...
+00000420: 00da 0a40 7079 7465 7374 5f61 72da 115f  ...@pytest_ar.._
+00000430: 6361 6c6c 5f72 6570 7263 6f6d 7061 7265  call_reprcompare
+00000440: da0c 4070 795f 6275 696c 7469 6e73 da06  ..@py_builtins..
+00000450: 6c6f 6361 6c73 da18 5f73 686f 756c 645f  locals.._should_
+00000460: 7265 7072 5f67 6c6f 6261 6c5f 6e61 6d65  repr_global_name
+00000470: da09 5f73 6166 6572 6570 72da 0e41 7373  .._saferepr..Ass
+00000480: 6572 7469 6f6e 4572 726f 72da 135f 666f  ertionError.._fo
+00000490: 726d 6174 5f65 7870 6c61 6e61 7469 6f6e  rmat_explanation
+000004a0: da0a 636c 6173 735f 6e61 6d65 da09 7465  ..class_name..te
+000004b0: 7374 5f6e 616d 6529 09da 0473 656c 6672  st_name)...selfr
+000004c0: 0900 0000 da0b 4070 795f 6173 7365 7274  ......@py_assert
+000004d0: 31da 0b40 7079 5f61 7373 6572 7433 da0b  1..@py_assert3..
+000004e0: 4070 795f 666f 726d 6174 35da 0b40 7079  @py_format5..@py
+000004f0: 5f66 6f72 6d61 7437 da0b 4070 795f 6173  _format7..@py_as
+00000500: 7365 7274 34da 0b40 7079 5f66 6f72 6d61  sert4..@py_forma
+00000510: 7436 da0b 4070 795f 666f 726d 6174 38a9  t6..@py_format8.
+00000520: 0072 2a00 0000 fa44 2f55 7365 7273 2f63  .r*....D/Users/c
+00000530: 6861 696e 7a2f 446f 6375 6d65 6e74 732f  hainz/Documents/
+00000540: 5072 6f6a 6563 7473 2f64 6a61 6e67 6f2d  Projects/django-
+00000550: 7065 7266 2d72 6563 2f74 6573 7473 2f74  perf-rec/tests/t
+00000560: 6573 745f 7574 696c 732e 7079 7215 0000  est_utils.pyr...
+00000570: 0007 0000 0073 3000 0000 0001 0601 0600  .....s0.........
+00000580: 0800 0400 6800 0c00 0e00 0801 0600 0400  ....h...........
+00000590: 0800 0600 4e00 0c00 0e00 0c01 0600 0400  ....N...........
+000005a0: 0800 0600 5200 0c00 0e00 7a1a 4375 7272  ....R.....z.Curr
+000005b0: 656e 7454 6573 7454 6573 7473 2e74 6573  entTestTests.tes
+000005c0: 745f 6865 7265 6301 0000 0000 0000 0000  t_herec.........
+000005d0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
+000005e0: b200 0000 7400 8300 7d01 7400 8300 7d02  ....t...}.t...}.
+000005f0: 7c01 7c02 6b02 7d03 7c03 73a2 7401 a002  |.|.k.}.|.s.t...
+00000600: 6401 7c03 6601 6402 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
+00000610: 6403 7403 a004 a100 6b06 7342 7401 a005  d.t.....k.sBt...
+00000620: 7400 a101 724c 7401 a006 7400 a101 6e02  t...rLt...t...n.
+00000630: 6403 7401 a006 7c01 a101 6403 7403 a004  d.t...|...d.t...
+00000640: a100 6b06 736c 7401 a005 7400 a101 7276  ..k.slt...t...rv
+00000650: 7401 a006 7400 a101 6e02 6403 7401 a006  t...t...n.d.t...
+00000660: 7c02 a101 6404 9c04 1600 7d04 6405 6406  |...d.....}.d.d.
+00000670: 7c04 6901 1600 7d05 7407 7401 a008 7c05  |.i...}.t.t...|.
+00000680: a101 8301 8201 6400 0400 7d01 0400 7d03  ......d...}...}.
+00000690: 7d02 6400 5300 2907 4e72 0600 0000 2901  }.d.S.).Nr....).
+000006a0: 7a40 2528 7079 3229 730a 7b25 2870 7932  z@%(py2)s.{%(py2
+000006b0: 2973 203d 2025 2870 7930 2973 2829 0a7d  )s = %(py0)s().}
+000006c0: 203d 3d20 2528 7079 3629 730a 7b25 2870   == %(py6)s.{%(p
+000006d0: 7936 2973 203d 2025 2870 7934 2973 2829  y6)s = %(py4)s()
+000006e0: 0a7d 7203 0000 0029 0472 0c00 0000 720d  .}r....).r....r.
+000006f0: 0000 0072 0e00 0000 7210 0000 007a 0e61  ...r....r....z.a
+00000700: 7373 6572 7420 2528 7079 3829 73da 0370  ssert %(py8)s..p
+00000710: 7938 2909 7203 0000 0072 1800 0000 7219  y8).r....r....r.
+00000720: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000730: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000740: 0029 0672 2200 0000 7223 0000 00da 0b40  .).r"...r#.....@
+00000750: 7079 5f61 7373 6572 7435 7224 0000 0072  py_assert5r$...r
+00000760: 2600 0000 da0b 4070 795f 666f 726d 6174  &.....@py_format
+00000770: 3972 2a00 0000 722a 0000 0072 2b00 0000  9r*...r*...r+...
+00000780: da0f 7465 7374 5f74 7769 6365 5f73 616d  ..test_twice_sam
+00000790: 650d 0000 0073 1000 0000 0001 0600 0600  e....s..........
+000007a0: 0800 0400 7000 0c00 0e00 7a20 4375 7272  ....p.....z Curr
+000007b0: 656e 7454 6573 7454 6573 7473 2e74 6573  entTestTests.tes
+000007c0: 745f 7477 6963 655f 7361 6d65 6301 0000  t_twice_samec...
+000007d0: 0000 0000 0000 0000 000a 0000 0007 0000  ................
+000007e0: 0043 0000 0073 ca01 0000 6401 6402 8400  .C...s....d.d...
+000007f0: 7d01 7c01 8300 7d02 7c02 6a00 7d03 7c03  }.|...}.|.j.}.|.
+00000800: 7401 6b02 7d04 7c04 73a2 7402 a003 6403  t.k.}.|.s.t...d.
+00000810: 7c04 6601 6404 7c03 7401 6602 a104 6405  |.f.d.|.t.f...d.
+00000820: 7404 a005 a100 6b06 734a 7402 a006 7c02  t.....k.sJt...|.
+00000830: a101 7254 7402 a007 7c02 a101 6e02 6405  ..rTt...|...n.d.
+00000840: 7402 a007 7c03 a101 6406 7404 a005 a100  t...|...d.t.....
+00000850: 6b06 7374 7402 a006 7401 a101 727e 7402  k.stt...t...r~t.
+00000860: a007 7401 a101 6e02 6406 6407 9c03 1600  ..t...n.d.d.....
+00000870: 7d05 6408 6409 7c05 6901 1600 7d06 7408  }.d.d.|.i...}.t.
+00000880: 7402 a009 7c06 a101 8301 8201 6400 0400  t...|.......d...
+00000890: 7d03 7d04 7c02 6a0a 7d03 6400 7d07 7c03  }.}.|.j.}.d.}.|.
+000008a0: 7c07 6b08 7d04 7c04 9001 732a 7402 a003  |.k.}.|...s*t...
+000008b0: 640a 7c04 6601 640b 7c03 7c07 6602 a104  d.|.f.d.|.|.f...
+000008c0: 6405 7404 a005 a100 6b06 73ec 7402 a006  d.t.....k.s.t...
+000008d0: 7c02 a101 72f6 7402 a007 7c02 a101 6e02  |...r.t...|...n.
+000008e0: 6405 7402 a007 7c03 a101 7402 a007 7c07  d.t...|...t...|.
+000008f0: a101 640c 9c03 1600 7d08 640d 640e 7c08  ..d.....}.d.d.|.
+00000900: 6901 1600 7d09 7408 7402 a009 7c09 a101  i...}.t.t...|...
+00000910: 8301 8201 6400 0400 7d03 0400 7d04 7d07  ....d...}...}.}.
+00000920: 7c02 6a0b 7d03 640f 7d07 7c03 7c07 6b02  |.j.}.d.}.|.|.k.
+00000930: 7d04 7c04 9001 73ba 7402 a003 6403 7c04  }.|...s.t...d.|.
+00000940: 6601 6410 7c03 7c07 6602 a104 6405 7404  f.d.|.|.f...d.t.
+00000950: a005 a100 6b06 9001 737c 7402 a006 7c02  ....k...s|t...|.
+00000960: a101 9001 7286 7402 a007 7c02 a101 6e02  ....r.t...|...n.
+00000970: 6405 7402 a007 7c03 a101 7402 a007 7c07  d.t...|...t...|.
+00000980: a101 640c 9c03 1600 7d08 640d 640e 7c08  ..d.....}.d.d.|.
+00000990: 6901 1600 7d09 7408 7402 a009 7c09 a101  i...}.t.t...|...
+000009a0: 8301 8201 6400 0400 7d03 0400 7d04 7d07  ....d...}...}.}.
+000009b0: 6400 5300 2911 4e63 0000 0000 0000 0000  d.S.).Nc........
+000009c0: 0000 0000 0000 0000 0100 0000 5300 0000  ............S...
+000009d0: 7306 0000 0074 0083 0053 0029 014e 2901  s....t...S.).N).
+000009e0: 7203 0000 0072 2a00 0000 722a 0000 0072  r....r*...r*...r
+000009f0: 2a00 0000 722b 0000 00da 1574 6573 745f  *...r+.....test_
+00000a00: 7468 6174 735f 6675 6e63 7469 6f6e 616c  thats_functional
+00000a10: 1100 0000 7302 0000 0000 017a 3f43 7572  ....s......z?Cur
+00000a20: 7265 6e74 5465 7374 5465 7374 732e 7465  rentTestTests.te
+00000a30: 7374 5f66 756e 6374 696f 6e61 6c2e 3c6c  st_functional.<l
+00000a40: 6f63 616c 733e 2e74 6573 745f 7468 6174  ocals>.test_that
+00000a50: 735f 6675 6e63 7469 6f6e 616c 7206 0000  s_functionalr...
+00000a60: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000a70: 720b 0000 0072 0f00 0000 7210 0000 0029  r....r....r....)
+00000a80: 01da 0269 7329 017a 3225 2870 7932 2973  ...is).z2%(py2)s
+00000a90: 0a7b 2528 7079 3229 7320 3d20 2528 7079  .{%(py2)s = %(py
+00000aa0: 3029 732e 636c 6173 735f 6e61 6d65 0a7d  0)s.class_name.}
+00000ab0: 2069 7320 2528 7079 3529 7372 1100 0000   is %(py5)sr....
+00000ac0: 7213 0000 0072 1400 0000 7230 0000 0072  r....r....r0...r
+00000ad0: 1600 0000 290c 7217 0000 0072 0a00 0000  ....).r....r....
+00000ae0: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00000af0: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
+00000b00: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
+00000b10: 0000 290a 7222 0000 0072 3000 0000 7209  ..).r"...r0...r.
+00000b20: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00000b30: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
+00000b40: 0072 2900 0000 722a 0000 0072 2a00 0000  .r)...r*...r*...
+00000b50: 722b 0000 00da 0f74 6573 745f 6675 6e63  r+.....test_func
+00000b60: 7469 6f6e 616c 1000 0000 7332 0000 0000  tional....s2....
+00000b70: 0108 0306 0106 0008 0004 0068 000c 000e  ...........h....
+00000b80: 0008 0106 0004 0008 0006 004e 000c 000e  ...........N....
+00000b90: 000c 0106 0004 0008 0006 0052 000c 000e  ...........R....
+00000ba0: 007a 2043 7572 7265 6e74 5465 7374 5465  .z CurrentTestTe
+00000bb0: 7374 732e 7465 7374 5f66 756e 6374 696f  sts.test_functio
+00000bc0: 6e61 6c4e 2906 da08 5f5f 6e61 6d65 5f5f  nalN)...__name__
+00000bd0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000be0: 7175 616c 6e61 6d65 5f5f 7215 0000 0072  qualname__r....r
+00000bf0: 2f00 0000 7232 0000 0072 2a00 0000 722a  /...r2...r*...r*
+00000c00: 0000 0072 2a00 0000 722b 0000 0072 0500  ...r*...r+...r..
+00000c10: 0000 0600 0000 7306 0000 0008 0108 0608  ......s.........
+00000c20: 0372 0500 0000 6300 0000 0000 0000 0000  .r....c.........
+00000c30: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00000c40: 3400 0000 6500 5a01 6400 5a02 6401 6402  4...e.Z.d.Z.d.d.
+00000c50: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
+00000c60: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
+00000c70: 8400 5a07 640b 5300 290c da10 536f 7274  ..Z.d.S.)...Sort
+00000c80: 6564 4e61 6d65 7354 6573 7473 6301 0000  edNamesTestsc...
+00000c90: 0000 0000 0000 0000 0007 0000 0007 0000  ................
+00000ca0: 0043 0000 0073 a000 0000 6700 7d01 7400  .C...s....g.}.t.
+00000cb0: 7c01 8301 7d02 6700 7d03 7c02 7c03 6b02  |...}.g.}.|.|.k.
+00000cc0: 7d04 7c04 738c 7401 a002 6401 7c04 6601  }.|.s.t...d.|.f.
+00000cd0: 6402 7c02 7c03 6602 a104 6403 7403 a004  d.|.|.f...d.t...
+00000ce0: a100 6b06 7346 7401 a005 7400 a101 7250  ..k.sFt...t...rP
+00000cf0: 7401 a006 7400 a101 6e02 6403 7401 a006  t...t...n.d.t...
+00000d00: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
+00000d10: 7c03 a101 6404 9c04 1600 7d05 6405 6406  |...d.....}.d.d.
+00000d20: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
+00000d30: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
+00000d40: 0400 7d04 7d03 6400 5300 2907 4e72 0600  ..}.}.d.S.).Nr..
+00000d50: 0000 a901 7a30 2528 7079 3429 730a 7b25  ....z0%(py4)s.{%
+00000d60: 2870 7934 2973 203d 2025 2870 7930 2973  (py4)s = %(py0)s
+00000d70: 2825 2870 7932 2973 290a 7d20 3d3d 2025  (%(py2)s).} == %
+00000d80: 2870 7937 2973 7204 0000 00a9 0472 0c00  (py7)sr......r..
+00000d90: 0000 720d 0000 0072 0e00 0000 7214 0000  ..r....r....r...
+00000da0: 00fa 0e61 7373 6572 7420 2528 7079 3929  ...assert %(py9)
+00000db0: 73da 0370 7939 a909 7204 0000 0072 1800  s..py9..r....r..
+00000dc0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000dd0: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000de0: 721f 0000 00a9 0772 2200 0000 7223 0000  r......r"...r#..
+00000df0: 0072 2400 0000 da0b 4070 795f 6173 7365  .r$.....@py_asse
+00000e00: 7274 3672 2d00 0000 7229 0000 00da 0c40  rt6r-...r).....@
+00000e10: 7079 5f66 6f72 6d61 7431 3072 2a00 0000  py_format10r*...
+00000e20: 722a 0000 0072 2b00 0000 da0a 7465 7374  r*...r+.....test
+00000e30: 5f65 6d70 7479 1b00 0000 7312 0000 0000  _empty....s.....
+00000e40: 0104 0008 0004 0008 0004 0056 000c 000e  ...........V....
+00000e50: 007a 1b53 6f72 7465 644e 616d 6573 5465  .z.SortedNamesTe
+00000e60: 7374 732e 7465 7374 5f65 6d70 7479 6301  sts.test_emptyc.
+00000e70: 0000 0000 0000 0000 0000 0007 0000 0007  ................
+00000e80: 0000 0043 0000 0073 a400 0000 6401 6701  ...C...s....d.g.
+00000e90: 7d01 7400 7c01 8301 7d02 6401 6701 7d03  }.t.|...}.d.g.}.
+00000ea0: 7c02 7c03 6b02 7d04 7c04 7390 7401 a002  |.|.k.}.|.s.t...
+00000eb0: 6402 7c04 6601 6403 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00000ec0: 6404 7403 a004 a100 6b06 734a 7401 a005  d.t.....k.sJt...
+00000ed0: 7400 a101 7254 7401 a006 7400 a101 6e02  t...rTt...t...n.
+00000ee0: 6404 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
+00000ef0: a101 7401 a006 7c03 a101 6405 9c04 1600  ..t...|...d.....
+00000f00: 7d05 6406 6407 7c05 6901 1600 7d06 7407  }.d.d.|.i...}.t.
+00000f10: 7401 a008 7c06 a101 8301 8201 6400 0400  t...|.......d...
+00000f20: 7d01 0400 7d02 0400 7d04 7d03 6400 5300  }...}...}.}.d.S.
+00000f30: 2908 4eda 0764 6566 6175 6c74 7206 0000  ).N..defaultr...
+00000f40: 0072 3700 0000 7204 0000 0072 3800 0000  .r7...r....r8...
+00000f50: 7239 0000 0072 3a00 0000 723b 0000 0072  r9...r:...r;...r
+00000f60: 3c00 0000 722a 0000 0072 2a00 0000 722b  <...r*...r*...r+
+00000f70: 0000 00da 1174 6573 745f 6a75 7374 5f64  .....test_just_d
+00000f80: 6566 6175 6c74 1e00 0000 7312 0000 0000  efault....s.....
+00000f90: 0106 0008 0006 0008 0004 0056 000c 000e  ...........V....
+00000fa0: 007a 2253 6f72 7465 644e 616d 6573 5465  .z"SortedNamesTe
+00000fb0: 7374 732e 7465 7374 5f6a 7573 745f 6465  sts.test_just_de
+00000fc0: 6661 756c 7463 0100 0000 0000 0000 0000  faultc..........
+00000fd0: 0000 0700 0000 0700 0000 4300 0000 73a4  ..........C...s.
+00000fe0: 0000 0064 0167 017d 0174 007c 0183 017d  ...d.g.}.t.|...}
+00000ff0: 0264 0167 017d 037c 027c 036b 027d 047c  .d.g.}.|.|.k.}.|
+00001000: 0473 9074 01a0 0264 027c 0466 0164 037c  .s.t...d.|.f.d.|
+00001010: 027c 0366 02a1 0464 0474 03a0 04a1 006b  .|.f...d.t.....k
+00001020: 0673 4a74 01a0 0574 00a1 0172 5474 01a0  .sJt...t...rTt..
+00001030: 0674 00a1 016e 0264 0474 01a0 067c 01a1  .t...n.d.t...|..
+00001040: 0174 01a0 067c 02a1 0174 01a0 067c 03a1  .t...|...t...|..
+00001050: 0164 059c 0416 007d 0564 0664 077c 0569  .d.....}.d.d.|.i
+00001060: 0116 007d 0674 0774 01a0 087c 06a1 0183  ...}.t.t...|....
+00001070: 0182 0164 0004 007d 0104 007d 0204 007d  ...d...}...}...}
+00001080: 047d 0364 0053 0029 084e 5a09 736f 6d65  .}.d.S.).NZ.some
+00001090: 7468 696e 6772 0600 0000 7237 0000 0072  thingr....r7...r
+000010a0: 0400 0000 7238 0000 0072 3900 0000 723a  ....r8...r9...r:
+000010b0: 0000 0072 3b00 0000 723c 0000 0072 2a00  ...r;...r<...r*.
+000010c0: 0000 722a 0000 0072 2b00 0000 da13 7465  ..r*...r+.....te
+000010d0: 7374 5f6a 7573 745f 736f 6d65 7468 696e  st_just_somethin
+000010e0: 6721 0000 0073 1200 0000 0001 0600 0800  g!...s..........
+000010f0: 0600 0800 0400 5600 0c00 0e00 7a24 536f  ......V.....z$So
+00001100: 7274 6564 4e61 6d65 7354 6573 7473 2e74  rtedNamesTests.t
+00001110: 6573 745f 6a75 7374 5f73 6f6d 6574 6869  est_just_somethi
+00001120: 6e67 6301 0000 0000 0000 0000 0000 0007  ngc.............
+00001130: 0000 0007 0000 0043 0000 0073 a800 0000  .......C...s....
+00001140: 6401 6402 6702 7d01 7400 7c01 8301 7d02  d.d.g.}.t.|...}.
+00001150: 6402 6401 6702 7d03 7c02 7c03 6b02 7d04  d.d.g.}.|.|.k.}.
+00001160: 7c04 7394 7401 a002 6403 7c04 6601 6404  |.s.t...d.|.f.d.
+00001170: 7c02 7c03 6602 a104 6405 7403 a004 a100  |.|.f...d.t.....
+00001180: 6b06 734e 7401 a005 7400 a101 7258 7401  k.sNt...t...rXt.
+00001190: a006 7400 a101 6e02 6405 7401 a006 7c01  ..t...n.d.t...|.
+000011a0: a101 7401 a006 7c02 a101 7401 a006 7c03  ..t...|...t...|.
+000011b0: a101 6406 9c04 1600 7d05 6407 6408 7c05  ..d.....}.d.d.|.
+000011c0: 6901 1600 7d06 7407 7401 a008 7c06 a101  i...}.t.t...|...
+000011d0: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
+000011e0: 7d04 7d03 6400 5300 2909 4eda 0162 da01  }.}.d.S.).N..b..
+000011f0: 6172 0600 0000 7237 0000 0072 0400 0000  ar....r7...r....
+00001200: 7238 0000 0072 3900 0000 723a 0000 0072  r8...r9...r:...r
+00001210: 3b00 0000 723c 0000 0072 2a00 0000 722a  ;...r<...r*...r*
+00001220: 0000 0072 2b00 0000 da0e 7465 7374 5f64  ...r+.....test_d
+00001230: 6f65 735f 736f 7274 2400 0000 7312 0000  oes_sort$...s...
+00001240: 0000 0108 0008 0008 0008 0004 0056 000c  .............V..
+00001250: 000e 007a 1f53 6f72 7465 644e 616d 6573  ...z.SortedNames
+00001260: 5465 7374 732e 7465 7374 5f64 6f65 735f  Tests.test_does_
+00001270: 736f 7274 6301 0000 0000 0000 0000 0000  sortc...........
+00001280: 0007 0000 0007 0000 0043 0000 0073 a800  .........C...s..
+00001290: 0000 6401 6402 6702 7d01 7400 7c01 8301  ..d.d.g.}.t.|...
+000012a0: 7d02 6402 6401 6702 7d03 7c02 7c03 6b02  }.d.d.g.}.|.|.k.
+000012b0: 7d04 7c04 7394 7401 a002 6403 7c04 6601  }.|.s.t...d.|.f.
+000012c0: 6404 7c02 7c03 6602 a104 6405 7403 a004  d.|.|.f...d.t...
+000012d0: a100 6b06 734e 7401 a005 7400 a101 7258  ..k.sNt...t...rX
+000012e0: 7401 a006 7400 a101 6e02 6405 7401 a006  t...t...n.d.t...
+000012f0: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
+00001300: 7c03 a101 6406 9c04 1600 7d05 6407 6408  |...d.....}.d.d.
+00001310: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
+00001320: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
+00001330: 0400 7d04 7d03 6400 5300 2909 4e72 4400  ..}.}.d.S.).NrD.
+00001340: 0000 7240 0000 0072 0600 0000 7237 0000  ..r@...r....r7..
+00001350: 0072 0400 0000 7238 0000 0072 3900 0000  .r....r8...r9...
+00001360: 723a 0000 0072 3b00 0000 723c 0000 0072  r:...r;...r<...r
+00001370: 2a00 0000 722a 0000 0072 2b00 0000 da1d  *...r*...r+.....
+00001380: 7465 7374 5f73 6f72 745f 6b65 6570 735f  test_sort_keeps_
+00001390: 6465 6661 756c 745f 6669 7273 7427 0000  default_first'..
+000013a0: 0073 1200 0000 0001 0800 0800 0800 0800  .s..............
+000013b0: 0400 5600 0c00 0e00 7a2e 536f 7274 6564  ..V.....z.Sorted
+000013c0: 4e61 6d65 7354 6573 7473 2e74 6573 745f  NamesTests.test_
+000013d0: 736f 7274 5f6b 6565 7073 5f64 6566 6175  sort_keeps_defau
+000013e0: 6c74 5f66 6972 7374 4e29 0872 3300 0000  lt_firstN).r3...
+000013f0: 7234 0000 0072 3500 0000 723f 0000 0072  r4...r5...r?...r
+00001400: 4100 0000 7242 0000 0072 4500 0000 7246  A...rB...rE...rF
+00001410: 0000 0072 2a00 0000 722a 0000 0072 2a00  ...r*...r*...r*.
+00001420: 0000 722b 0000 0072 3600 0000 1a00 0000  ..r+...r6.......
+00001430: 730a 0000 0008 0108 0308 0308 0308 0372  s..............r
+00001440: 3600 0000 290d da08 6275 696c 7469 6e73  6...)...builtins
+00001450: 721a 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
+00001460: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+00001470: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+00001480: 7269 7465 7218 0000 00da 0b64 6a61 6e67  riter......djang
+00001490: 6f2e 7465 7374 7202 0000 00da 1564 6a61  o.testr......dja
+000014a0: 6e67 6f5f 7065 7266 5f72 6563 2e75 7469  ngo_perf_rec.uti
+000014b0: 6c73 7203 0000 0072 0400 0000 7205 0000  lsr....r....r...
+000014c0: 0072 3600 0000 722a 0000 0072 2a00 0000  .r6...r*...r*...
+000014d0: 722a 0000 0072 2b00 0000 da08 3c6d 6f64  r*...r+.....<mod
+000014e0: 756c 653e 0100 0000 730a 0000 0008 0012  ule>....s.......
+000014f0: 000c 0210 0310 14                        .......
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_utils.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_utils.cpython-39-pytest-6.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 35fa 535e bc04 0000 e300 0000  U...5.S^........
+00000000: 610d 0d0a 4f4b ee5e bc04 0000 e300 0000  a...OK.^........
 00000010: 0000 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0040 0000 0073 5a00 0000 6400 6401 6c00  .@...sZ...d.d.l.
 00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
 00000040: 5a05 0100 6400 6402 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
 00000050: 6400 6403 6c08 6d09 5a09 6d0a 5a0a 0100  d.d.l.m.Z.m.Z...
 00000060: 4700 6404 6405 8400 6405 6507 8303 5a0b  G.d.d...d.e...Z.
 00000070: 4700 6406 6407 8400 6407 6507 8303 5a0c  G.d.d...d.e...Z.
@@ -16,34 +16,34 @@
 000000f0: 5a04 6405 6406 8400 5a05 6407 5300 2908  Z.d.d...Z.d.S.).
 00000100: da10 4375 7272 656e 7454 6573 7454 6573  ..CurrentTestTes
 00000110: 7473 6301 0000 0000 0000 0000 0000 0009  tsc.............
 00000120: 0000 0007 0000 0043 0000 0073 c201 0000  .......C...s....
 00000130: 7400 8300 7d01 7c01 6a01 7d02 7c02 7402  t...}.|.j.}.|.t.
 00000140: 6b02 7d03 7c03 739a 7403 a004 6401 7c03  k.}.|.s.t...d.|.
 00000150: 6601 6402 7c02 7402 6602 a104 6403 7405  f.d.|.t.f...d.t.
-00000160: a006 a100 6b06 7342 7403 a007 7c01 a101  ....k.sBt...|...
+00000160: a006 a100 7600 7342 7403 a007 7c01 a101  ....v.sBt...|...
 00000170: 724c 7403 a008 7c01 a101 6e02 6403 7403  rLt...|...n.d.t.
-00000180: a008 7c02 a101 6404 7405 a006 a100 6b06  ..|...d.t.....k.
+00000180: a008 7c02 a101 6404 7405 a006 a100 7600  ..|...d.t.....v.
 00000190: 736c 7403 a007 7402 a101 7276 7403 a008  slt...t...rvt...
 000001a0: 7402 a101 6e02 6404 6405 9c03 1600 7d04  t...n.d.d.....}.
 000001b0: 6406 6407 7c04 6901 1600 7d05 7409 7403  d.d.|.i...}.t.t.
 000001c0: a00a 7c05 a101 8301 8201 6400 0400 7d02  ..|.......d...}.
 000001d0: 7d03 7c01 6a0b 7d02 6408 7d06 7c02 7c06  }.|.j.}.d.}.|.|.
 000001e0: 6b02 7d03 7c03 9001 7322 7403 a004 6401  k.}.|...s"t...d.
 000001f0: 7c03 6601 6409 7c02 7c06 6602 a104 6403  |.f.d.|.|.f...d.
-00000200: 7405 a006 a100 6b06 73e4 7403 a007 7c01  t.....k.s.t...|.
+00000200: 7405 a006 a100 7600 73e4 7403 a007 7c01  t.....v.s.t...|.
 00000210: a101 72ee 7403 a008 7c01 a101 6e02 6403  ..r.t...|...n.d.
 00000220: 7403 a008 7c02 a101 7403 a008 7c06 a101  t...|...t...|...
 00000230: 640a 9c03 1600 7d07 640b 640c 7c07 6901  d.....}.d.d.|.i.
 00000240: 1600 7d08 7409 7403 a00a 7c08 a101 8301  ..}.t.t...|.....
 00000250: 8201 6400 0400 7d02 0400 7d03 7d06 7c01  ..d...}...}.}.|.
 00000260: 6a0c 7d02 640d 7d06 7c02 7c06 6b02 7d03  j.}.d.}.|.|.k.}.
 00000270: 7c03 9001 73b2 7403 a004 6401 7c03 6601  |...s.t...d.|.f.
 00000280: 640e 7c02 7c06 6602 a104 6403 7405 a006  d.|.|.f...d.t...
-00000290: a100 6b06 9001 7374 7403 a007 7c01 a101  ..k...stt...|...
+00000290: a100 7600 9001 7374 7403 a007 7c01 a101  ..v...stt...|...
 000002a0: 9001 727e 7403 a008 7c01 a101 6e02 6403  ..r~t...|...n.d.
 000002b0: 7403 a008 7c02 a101 7403 a008 7c06 a101  t...|...t...|...
 000002c0: 640a 9c03 1600 7d07 640b 640c 7c07 6901  d.....}.d.d.|.i.
 000002d0: 1600 7d08 7409 7403 a00a 7c08 a101 8301  ..}.t.t...|.....
 000002e0: 8201 6400 0400 7d02 0400 7d03 7d06 6400  ..d...}...}.}.d.
 000002f0: 5300 290f 4ea9 01fa 023d 3da9 017a 3125  S.).N....==..z1%
 00000300: 2870 7932 2973 0a7b 2528 7079 3229 7320  (py2)s.{%(py2)s 
@@ -81,256 +81,245 @@
 00000500: 7365 7274 34da 0b40 7079 5f66 6f72 6d61  sert4..@py_forma
 00000510: 7436 da0b 4070 795f 666f 726d 6174 38a9  t6..@py_format8.
 00000520: 0072 2a00 0000 fa44 2f55 7365 7273 2f63  .r*....D/Users/c
 00000530: 6861 696e 7a2f 446f 6375 6d65 6e74 732f  hainz/Documents/
 00000540: 5072 6f6a 6563 7473 2f64 6a61 6e67 6f2d  Projects/django-
 00000550: 7065 7266 2d72 6563 2f74 6573 7473 2f74  perf-rec/tests/t
 00000560: 6573 745f 7574 696c 732e 7079 7215 0000  est_utils.pyr...
-00000570: 0007 0000 0073 3000 0000 0001 0601 0600  .....s0.........
-00000580: 0800 0400 6800 0c00 0e00 0801 0600 0400  ....h...........
-00000590: 0800 0600 4e00 0c00 0e00 0c01 0600 0400  ....N...........
-000005a0: 0800 0600 5200 0c00 0e00 7a1a 4375 7272  ....R.....z.Curr
-000005b0: 656e 7454 6573 7454 6573 7473 2e74 6573  entTestTests.tes
-000005c0: 745f 6865 7265 6301 0000 0000 0000 0000  t_herec.........
-000005d0: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
-000005e0: b200 0000 7400 8300 7d01 7400 8300 7d02  ....t...}.t...}.
-000005f0: 7c01 7c02 6b02 7d03 7c03 73a2 7401 a002  |.|.k.}.|.s.t...
-00000600: 6401 7c03 6601 6402 7c01 7c02 6602 a104  d.|.f.d.|.|.f...
-00000610: 6403 7403 a004 a100 6b06 7342 7401 a005  d.t.....k.sBt...
-00000620: 7400 a101 724c 7401 a006 7400 a101 6e02  t...rLt...t...n.
-00000630: 6403 7401 a006 7c01 a101 6403 7403 a004  d.t...|...d.t...
-00000640: a100 6b06 736c 7401 a005 7400 a101 7276  ..k.slt...t...rv
-00000650: 7401 a006 7400 a101 6e02 6403 7401 a006  t...t...n.d.t...
-00000660: 7c02 a101 6404 9c04 1600 7d04 6405 6406  |...d.....}.d.d.
-00000670: 7c04 6901 1600 7d05 7407 7401 a008 7c05  |.i...}.t.t...|.
-00000680: a101 8301 8201 6400 0400 7d01 0400 7d03  ......d...}...}.
-00000690: 7d02 6400 5300 2907 4e72 0600 0000 2901  }.d.S.).Nr....).
-000006a0: 7a40 2528 7079 3229 730a 7b25 2870 7932  z@%(py2)s.{%(py2
-000006b0: 2973 203d 2025 2870 7930 2973 2829 0a7d  )s = %(py0)s().}
-000006c0: 203d 3d20 2528 7079 3629 730a 7b25 2870   == %(py6)s.{%(p
-000006d0: 7936 2973 203d 2025 2870 7934 2973 2829  y6)s = %(py4)s()
-000006e0: 0a7d 7203 0000 0029 0472 0c00 0000 720d  .}r....).r....r.
-000006f0: 0000 0072 0e00 0000 7210 0000 007a 0e61  ...r....r....z.a
-00000700: 7373 6572 7420 2528 7079 3829 73da 0370  ssert %(py8)s..p
-00000710: 7938 2909 7203 0000 0072 1800 0000 7219  y8).r....r....r.
-00000720: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
-00000730: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00000740: 0029 0672 2200 0000 7223 0000 00da 0b40  .).r"...r#.....@
-00000750: 7079 5f61 7373 6572 7435 7224 0000 0072  py_assert5r$...r
-00000760: 2600 0000 da0b 4070 795f 666f 726d 6174  &.....@py_format
-00000770: 3972 2a00 0000 722a 0000 0072 2b00 0000  9r*...r*...r+...
-00000780: da0f 7465 7374 5f74 7769 6365 5f73 616d  ..test_twice_sam
-00000790: 650d 0000 0073 1000 0000 0001 0600 0600  e....s..........
-000007a0: 0800 0400 7000 0c00 0e00 7a20 4375 7272  ....p.....z Curr
-000007b0: 656e 7454 6573 7454 6573 7473 2e74 6573  entTestTests.tes
-000007c0: 745f 7477 6963 655f 7361 6d65 6301 0000  t_twice_samec...
-000007d0: 0000 0000 0000 0000 000a 0000 0007 0000  ................
-000007e0: 0043 0000 0073 ca01 0000 6401 6402 8400  .C...s....d.d...
-000007f0: 7d01 7c01 8300 7d02 7c02 6a00 7d03 7c03  }.|...}.|.j.}.|.
-00000800: 7401 6b02 7d04 7c04 73a2 7402 a003 6403  t.k.}.|.s.t...d.
-00000810: 7c04 6601 6404 7c03 7401 6602 a104 6405  |.f.d.|.t.f...d.
-00000820: 7404 a005 a100 6b06 734a 7402 a006 7c02  t.....k.sJt...|.
-00000830: a101 7254 7402 a007 7c02 a101 6e02 6405  ..rTt...|...n.d.
-00000840: 7402 a007 7c03 a101 6406 7404 a005 a100  t...|...d.t.....
-00000850: 6b06 7374 7402 a006 7401 a101 727e 7402  k.stt...t...r~t.
-00000860: a007 7401 a101 6e02 6406 6407 9c03 1600  ..t...n.d.d.....
-00000870: 7d05 6408 6409 7c05 6901 1600 7d06 7408  }.d.d.|.i...}.t.
-00000880: 7402 a009 7c06 a101 8301 8201 6400 0400  t...|.......d...
-00000890: 7d03 7d04 7c02 6a0a 7d03 6400 7d07 7c03  }.}.|.j.}.d.}.|.
-000008a0: 7c07 6b08 7d04 7c04 9001 732a 7402 a003  |.k.}.|...s*t...
-000008b0: 640a 7c04 6601 640b 7c03 7c07 6602 a104  d.|.f.d.|.|.f...
-000008c0: 6405 7404 a005 a100 6b06 73ec 7402 a006  d.t.....k.s.t...
-000008d0: 7c02 a101 72f6 7402 a007 7c02 a101 6e02  |...r.t...|...n.
-000008e0: 6405 7402 a007 7c03 a101 7402 a007 7c07  d.t...|...t...|.
-000008f0: a101 640c 9c03 1600 7d08 640d 640e 7c08  ..d.....}.d.d.|.
-00000900: 6901 1600 7d09 7408 7402 a009 7c09 a101  i...}.t.t...|...
-00000910: 8301 8201 6400 0400 7d03 0400 7d04 7d07  ....d...}...}.}.
-00000920: 7c02 6a0b 7d03 640f 7d07 7c03 7c07 6b02  |.j.}.d.}.|.|.k.
-00000930: 7d04 7c04 9001 73ba 7402 a003 6403 7c04  }.|...s.t...d.|.
-00000940: 6601 6410 7c03 7c07 6602 a104 6405 7404  f.d.|.|.f...d.t.
-00000950: a005 a100 6b06 9001 737c 7402 a006 7c02  ....k...s|t...|.
-00000960: a101 9001 7286 7402 a007 7c02 a101 6e02  ....r.t...|...n.
-00000970: 6405 7402 a007 7c03 a101 7402 a007 7c07  d.t...|...t...|.
-00000980: a101 640c 9c03 1600 7d08 640d 640e 7c08  ..d.....}.d.d.|.
-00000990: 6901 1600 7d09 7408 7402 a009 7c09 a101  i...}.t.t...|...
-000009a0: 8301 8201 6400 0400 7d03 0400 7d04 7d07  ....d...}...}.}.
-000009b0: 6400 5300 2911 4e63 0000 0000 0000 0000  d.S.).Nc........
-000009c0: 0000 0000 0000 0000 0100 0000 5300 0000  ............S...
-000009d0: 7306 0000 0074 0083 0053 0029 014e 2901  s....t...S.).N).
-000009e0: 7203 0000 0072 2a00 0000 722a 0000 0072  r....r*...r*...r
-000009f0: 2a00 0000 722b 0000 00da 1574 6573 745f  *...r+.....test_
-00000a00: 7468 6174 735f 6675 6e63 7469 6f6e 616c  thats_functional
-00000a10: 1100 0000 7302 0000 0000 017a 3f43 7572  ....s......z?Cur
-00000a20: 7265 6e74 5465 7374 5465 7374 732e 7465  rentTestTests.te
-00000a30: 7374 5f66 756e 6374 696f 6e61 6c2e 3c6c  st_functional.<l
-00000a40: 6f63 616c 733e 2e74 6573 745f 7468 6174  ocals>.test_that
-00000a50: 735f 6675 6e63 7469 6f6e 616c 7206 0000  s_functionalr...
-00000a60: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000a70: 720b 0000 0072 0f00 0000 7210 0000 0029  r....r....r....)
-00000a80: 01da 0269 7329 017a 3225 2870 7932 2973  ...is).z2%(py2)s
-00000a90: 0a7b 2528 7079 3229 7320 3d20 2528 7079  .{%(py2)s = %(py
-00000aa0: 3029 732e 636c 6173 735f 6e61 6d65 0a7d  0)s.class_name.}
-00000ab0: 2069 7320 2528 7079 3529 7372 1100 0000   is %(py5)sr....
-00000ac0: 7213 0000 0072 1400 0000 7230 0000 0072  r....r....r0...r
-00000ad0: 1600 0000 290c 7217 0000 0072 0a00 0000  ....).r....r....
-00000ae0: 7218 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00000af0: 1b00 0000 721c 0000 0072 1d00 0000 721e  ....r....r....r.
-00000b00: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00000b10: 0000 290a 7222 0000 0072 3000 0000 7209  ..).r"...r0...r.
-00000b20: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-00000b30: 0000 7226 0000 0072 2700 0000 7228 0000  ..r&...r'...r(..
-00000b40: 0072 2900 0000 722a 0000 0072 2a00 0000  .r)...r*...r*...
-00000b50: 722b 0000 00da 0f74 6573 745f 6675 6e63  r+.....test_func
-00000b60: 7469 6f6e 616c 1000 0000 7332 0000 0000  tional....s2....
-00000b70: 0108 0306 0106 0008 0004 0068 000c 000e  ...........h....
-00000b80: 0008 0106 0004 0008 0006 004e 000c 000e  ...........N....
-00000b90: 000c 0106 0004 0008 0006 0052 000c 000e  ...........R....
-00000ba0: 007a 2043 7572 7265 6e74 5465 7374 5465  .z CurrentTestTe
-00000bb0: 7374 732e 7465 7374 5f66 756e 6374 696f  sts.test_functio
-00000bc0: 6e61 6c4e 2906 da08 5f5f 6e61 6d65 5f5f  nalN)...__name__
-00000bd0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000be0: 7175 616c 6e61 6d65 5f5f 7215 0000 0072  qualname__r....r
-00000bf0: 2f00 0000 7232 0000 0072 2a00 0000 722a  /...r2...r*...r*
-00000c00: 0000 0072 2a00 0000 722b 0000 0072 0500  ...r*...r+...r..
-00000c10: 0000 0600 0000 7306 0000 0008 0108 0608  ......s.........
-00000c20: 0372 0500 0000 6300 0000 0000 0000 0000  .r....c.........
-00000c30: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00000c40: 3400 0000 6500 5a01 6400 5a02 6401 6402  4...e.Z.d.Z.d.d.
-00000c50: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-00000c60: 8400 5a05 6407 6408 8400 5a06 6409 640a  ..Z.d.d...Z.d.d.
-00000c70: 8400 5a07 640b 5300 290c da10 536f 7274  ..Z.d.S.)...Sort
-00000c80: 6564 4e61 6d65 7354 6573 7473 6301 0000  edNamesTestsc...
-00000c90: 0000 0000 0000 0000 0007 0000 0007 0000  ................
-00000ca0: 0043 0000 0073 a000 0000 6700 7d01 7400  .C...s....g.}.t.
-00000cb0: 7c01 8301 7d02 6700 7d03 7c02 7c03 6b02  |...}.g.}.|.|.k.
-00000cc0: 7d04 7c04 738c 7401 a002 6401 7c04 6601  }.|.s.t...d.|.f.
-00000cd0: 6402 7c02 7c03 6602 a104 6403 7403 a004  d.|.|.f...d.t...
-00000ce0: a100 6b06 7346 7401 a005 7400 a101 7250  ..k.sFt...t...rP
-00000cf0: 7401 a006 7400 a101 6e02 6403 7401 a006  t...t...n.d.t...
-00000d00: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
-00000d10: 7c03 a101 6404 9c04 1600 7d05 6405 6406  |...d.....}.d.d.
-00000d20: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
-00000d30: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
-00000d40: 0400 7d04 7d03 6400 5300 2907 4e72 0600  ..}.}.d.S.).Nr..
-00000d50: 0000 a901 7a30 2528 7079 3429 730a 7b25  ....z0%(py4)s.{%
-00000d60: 2870 7934 2973 203d 2025 2870 7930 2973  (py4)s = %(py0)s
-00000d70: 2825 2870 7932 2973 290a 7d20 3d3d 2025  (%(py2)s).} == %
-00000d80: 2870 7937 2973 7204 0000 00a9 0472 0c00  (py7)sr......r..
-00000d90: 0000 720d 0000 0072 0e00 0000 7214 0000  ..r....r....r...
-00000da0: 00fa 0e61 7373 6572 7420 2528 7079 3929  ...assert %(py9)
-00000db0: 73da 0370 7939 a909 7204 0000 0072 1800  s..py9..r....r..
-00000dc0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000dd0: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000de0: 721f 0000 00a9 0772 2200 0000 7223 0000  r......r"...r#..
-00000df0: 0072 2400 0000 da0b 4070 795f 6173 7365  .r$.....@py_asse
-00000e00: 7274 3672 2d00 0000 7229 0000 00da 0c40  rt6r-...r).....@
-00000e10: 7079 5f66 6f72 6d61 7431 3072 2a00 0000  py_format10r*...
-00000e20: 722a 0000 0072 2b00 0000 da0a 7465 7374  r*...r+.....test
-00000e30: 5f65 6d70 7479 1b00 0000 7312 0000 0000  _empty....s.....
-00000e40: 0104 0008 0004 0008 0004 0056 000c 000e  ...........V....
-00000e50: 007a 1b53 6f72 7465 644e 616d 6573 5465  .z.SortedNamesTe
-00000e60: 7374 732e 7465 7374 5f65 6d70 7479 6301  sts.test_emptyc.
-00000e70: 0000 0000 0000 0000 0000 0007 0000 0007  ................
-00000e80: 0000 0043 0000 0073 a400 0000 6401 6701  ...C...s....d.g.
-00000e90: 7d01 7400 7c01 8301 7d02 6401 6701 7d03  }.t.|...}.d.g.}.
-00000ea0: 7c02 7c03 6b02 7d04 7c04 7390 7401 a002  |.|.k.}.|.s.t...
-00000eb0: 6402 7c04 6601 6403 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
-00000ec0: 6404 7403 a004 a100 6b06 734a 7401 a005  d.t.....k.sJt...
-00000ed0: 7400 a101 7254 7401 a006 7400 a101 6e02  t...rTt...t...n.
-00000ee0: 6404 7401 a006 7c01 a101 7401 a006 7c02  d.t...|...t...|.
-00000ef0: a101 7401 a006 7c03 a101 6405 9c04 1600  ..t...|...d.....
-00000f00: 7d05 6406 6407 7c05 6901 1600 7d06 7407  }.d.d.|.i...}.t.
-00000f10: 7401 a008 7c06 a101 8301 8201 6400 0400  t...|.......d...
-00000f20: 7d01 0400 7d02 0400 7d04 7d03 6400 5300  }...}...}.}.d.S.
-00000f30: 2908 4eda 0764 6566 6175 6c74 7206 0000  ).N..defaultr...
-00000f40: 0072 3700 0000 7204 0000 0072 3800 0000  .r7...r....r8...
-00000f50: 7239 0000 0072 3a00 0000 723b 0000 0072  r9...r:...r;...r
-00000f60: 3c00 0000 722a 0000 0072 2a00 0000 722b  <...r*...r*...r+
-00000f70: 0000 00da 1174 6573 745f 6a75 7374 5f64  .....test_just_d
-00000f80: 6566 6175 6c74 1e00 0000 7312 0000 0000  efault....s.....
-00000f90: 0106 0008 0006 0008 0004 0056 000c 000e  ...........V....
-00000fa0: 007a 2253 6f72 7465 644e 616d 6573 5465  .z"SortedNamesTe
-00000fb0: 7374 732e 7465 7374 5f6a 7573 745f 6465  sts.test_just_de
-00000fc0: 6661 756c 7463 0100 0000 0000 0000 0000  faultc..........
-00000fd0: 0000 0700 0000 0700 0000 4300 0000 73a4  ..........C...s.
-00000fe0: 0000 0064 0167 017d 0174 007c 0183 017d  ...d.g.}.t.|...}
-00000ff0: 0264 0167 017d 037c 027c 036b 027d 047c  .d.g.}.|.|.k.}.|
-00001000: 0473 9074 01a0 0264 027c 0466 0164 037c  .s.t...d.|.f.d.|
-00001010: 027c 0366 02a1 0464 0474 03a0 04a1 006b  .|.f...d.t.....k
-00001020: 0673 4a74 01a0 0574 00a1 0172 5474 01a0  .sJt...t...rTt..
-00001030: 0674 00a1 016e 0264 0474 01a0 067c 01a1  .t...n.d.t...|..
-00001040: 0174 01a0 067c 02a1 0174 01a0 067c 03a1  .t...|...t...|..
-00001050: 0164 059c 0416 007d 0564 0664 077c 0569  .d.....}.d.d.|.i
-00001060: 0116 007d 0674 0774 01a0 087c 06a1 0183  ...}.t.t...|....
-00001070: 0182 0164 0004 007d 0104 007d 0204 007d  ...d...}...}...}
-00001080: 047d 0364 0053 0029 084e 5a09 736f 6d65  .}.d.S.).NZ.some
-00001090: 7468 696e 6772 0600 0000 7237 0000 0072  thingr....r7...r
-000010a0: 0400 0000 7238 0000 0072 3900 0000 723a  ....r8...r9...r:
-000010b0: 0000 0072 3b00 0000 723c 0000 0072 2a00  ...r;...r<...r*.
-000010c0: 0000 722a 0000 0072 2b00 0000 da13 7465  ..r*...r+.....te
-000010d0: 7374 5f6a 7573 745f 736f 6d65 7468 696e  st_just_somethin
-000010e0: 6721 0000 0073 1200 0000 0001 0600 0800  g!...s..........
-000010f0: 0600 0800 0400 5600 0c00 0e00 7a24 536f  ......V.....z$So
-00001100: 7274 6564 4e61 6d65 7354 6573 7473 2e74  rtedNamesTests.t
-00001110: 6573 745f 6a75 7374 5f73 6f6d 6574 6869  est_just_somethi
-00001120: 6e67 6301 0000 0000 0000 0000 0000 0007  ngc.............
-00001130: 0000 0007 0000 0043 0000 0073 a800 0000  .......C...s....
-00001140: 6401 6402 6702 7d01 7400 7c01 8301 7d02  d.d.g.}.t.|...}.
-00001150: 6402 6401 6702 7d03 7c02 7c03 6b02 7d04  d.d.g.}.|.|.k.}.
-00001160: 7c04 7394 7401 a002 6403 7c04 6601 6404  |.s.t...d.|.f.d.
-00001170: 7c02 7c03 6602 a104 6405 7403 a004 a100  |.|.f...d.t.....
-00001180: 6b06 734e 7401 a005 7400 a101 7258 7401  k.sNt...t...rXt.
-00001190: a006 7400 a101 6e02 6405 7401 a006 7c01  ..t...n.d.t...|.
-000011a0: a101 7401 a006 7c02 a101 7401 a006 7c03  ..t...|...t...|.
-000011b0: a101 6406 9c04 1600 7d05 6407 6408 7c05  ..d.....}.d.d.|.
-000011c0: 6901 1600 7d06 7407 7401 a008 7c06 a101  i...}.t.t...|...
-000011d0: 8301 8201 6400 0400 7d01 0400 7d02 0400  ....d...}...}...
-000011e0: 7d04 7d03 6400 5300 2909 4eda 0162 da01  }.}.d.S.).N..b..
-000011f0: 6172 0600 0000 7237 0000 0072 0400 0000  ar....r7...r....
-00001200: 7238 0000 0072 3900 0000 723a 0000 0072  r8...r9...r:...r
-00001210: 3b00 0000 723c 0000 0072 2a00 0000 722a  ;...r<...r*...r*
-00001220: 0000 0072 2b00 0000 da0e 7465 7374 5f64  ...r+.....test_d
-00001230: 6f65 735f 736f 7274 2400 0000 7312 0000  oes_sort$...s...
-00001240: 0000 0108 0008 0008 0008 0004 0056 000c  .............V..
-00001250: 000e 007a 1f53 6f72 7465 644e 616d 6573  ...z.SortedNames
-00001260: 5465 7374 732e 7465 7374 5f64 6f65 735f  Tests.test_does_
-00001270: 736f 7274 6301 0000 0000 0000 0000 0000  sortc...........
-00001280: 0007 0000 0007 0000 0043 0000 0073 a800  .........C...s..
-00001290: 0000 6401 6402 6702 7d01 7400 7c01 8301  ..d.d.g.}.t.|...
-000012a0: 7d02 6402 6401 6702 7d03 7c02 7c03 6b02  }.d.d.g.}.|.|.k.
-000012b0: 7d04 7c04 7394 7401 a002 6403 7c04 6601  }.|.s.t...d.|.f.
-000012c0: 6404 7c02 7c03 6602 a104 6405 7403 a004  d.|.|.f...d.t...
-000012d0: a100 6b06 734e 7401 a005 7400 a101 7258  ..k.sNt...t...rX
-000012e0: 7401 a006 7400 a101 6e02 6405 7401 a006  t...t...n.d.t...
-000012f0: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
-00001300: 7c03 a101 6406 9c04 1600 7d05 6407 6408  |...d.....}.d.d.
-00001310: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
-00001320: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
-00001330: 0400 7d04 7d03 6400 5300 2909 4e72 4400  ..}.}.d.S.).NrD.
-00001340: 0000 7240 0000 0072 0600 0000 7237 0000  ..r@...r....r7..
-00001350: 0072 0400 0000 7238 0000 0072 3900 0000  .r....r8...r9...
-00001360: 723a 0000 0072 3b00 0000 723c 0000 0072  r:...r;...r<...r
-00001370: 2a00 0000 722a 0000 0072 2b00 0000 da1d  *...r*...r+.....
-00001380: 7465 7374 5f73 6f72 745f 6b65 6570 735f  test_sort_keeps_
-00001390: 6465 6661 756c 745f 6669 7273 7427 0000  default_first'..
-000013a0: 0073 1200 0000 0001 0800 0800 0800 0800  .s..............
-000013b0: 0400 5600 0c00 0e00 7a2e 536f 7274 6564  ..V.....z.Sorted
-000013c0: 4e61 6d65 7354 6573 7473 2e74 6573 745f  NamesTests.test_
-000013d0: 736f 7274 5f6b 6565 7073 5f64 6566 6175  sort_keeps_defau
-000013e0: 6c74 5f66 6972 7374 4e29 0872 3300 0000  lt_firstN).r3...
-000013f0: 7234 0000 0072 3500 0000 723f 0000 0072  r4...r5...r?...r
-00001400: 4100 0000 7242 0000 0072 4500 0000 7246  A...rB...rE...rF
-00001410: 0000 0072 2a00 0000 722a 0000 0072 2a00  ...r*...r*...r*.
-00001420: 0000 722b 0000 0072 3600 0000 1a00 0000  ..r+...r6.......
-00001430: 730a 0000 0008 0108 0308 0308 0308 0372  s..............r
-00001440: 3600 0000 290d da08 6275 696c 7469 6e73  6...)...builtins
-00001450: 721a 0000 00da 195f 7079 7465 7374 2e61  r......_pytest.a
-00001460: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
-00001470: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
-00001480: 7269 7465 7218 0000 00da 0b64 6a61 6e67  riter......djang
-00001490: 6f2e 7465 7374 7202 0000 00da 1564 6a61  o.testr......dja
-000014a0: 6e67 6f5f 7065 7266 5f72 6563 2e75 7469  ngo_perf_rec.uti
-000014b0: 6c73 7203 0000 0072 0400 0000 7205 0000  lsr....r....r...
-000014c0: 0072 3600 0000 722a 0000 0072 2a00 0000  .r6...r*...r*...
-000014d0: 722a 0000 0072 2b00 0000 da08 3c6d 6f64  r*...r+.....<mod
-000014e0: 756c 653e 0100 0000 730a 0000 0008 0012  ule>....s.......
-000014f0: 000c 0210 0310 14                        .......
+00000570: 0007 0000 0073 0800 0000 0001 0601 9c01  .....s..........
+00000580: 8c01 7a1a 4375 7272 656e 7454 6573 7454  ..z.CurrentTestT
+00000590: 6573 7473 2e74 6573 745f 6865 7265 6301  ests.test_herec.
+000005a0: 0000 0000 0000 0000 0000 0006 0000 0007  ................
+000005b0: 0000 0043 0000 0073 b200 0000 7400 8300  ...C...s....t...
+000005c0: 7d01 7400 8300 7d02 7c01 7c02 6b02 7d03  }.t...}.|.|.k.}.
+000005d0: 7c03 73a2 7401 a002 6401 7c03 6601 6402  |.s.t...d.|.f.d.
+000005e0: 7c01 7c02 6602 a104 6403 7403 a004 a100  |.|.f...d.t.....
+000005f0: 7600 7342 7401 a005 7400 a101 724c 7401  v.sBt...t...rLt.
+00000600: a006 7400 a101 6e02 6403 7401 a006 7c01  ..t...n.d.t...|.
+00000610: a101 6403 7403 a004 a100 7600 736c 7401  ..d.t.....v.slt.
+00000620: a005 7400 a101 7276 7401 a006 7400 a101  ..t...rvt...t...
+00000630: 6e02 6403 7401 a006 7c02 a101 6404 9c04  n.d.t...|...d...
+00000640: 1600 7d04 6405 6406 7c04 6901 1600 7d05  ..}.d.d.|.i...}.
+00000650: 7407 7401 a008 7c05 a101 8301 8201 6400  t.t...|.......d.
+00000660: 0400 7d01 0400 7d03 7d02 6400 5300 2907  ..}...}.}.d.S.).
+00000670: 4e72 0600 0000 2901 7a40 2528 7079 3229  Nr....).z@%(py2)
+00000680: 730a 7b25 2870 7932 2973 203d 2025 2870  s.{%(py2)s = %(p
+00000690: 7930 2973 2829 0a7d 203d 3d20 2528 7079  y0)s().} == %(py
+000006a0: 3629 730a 7b25 2870 7936 2973 203d 2025  6)s.{%(py6)s = %
+000006b0: 2870 7934 2973 2829 0a7d 7203 0000 0029  (py4)s().}r....)
+000006c0: 0472 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+000006d0: 7210 0000 007a 0e61 7373 6572 7420 2528  r....z.assert %(
+000006e0: 7079 3829 73da 0370 7938 2909 7203 0000  py8)s..py8).r...
+000006f0: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00000700: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+00000710: 1e00 0000 721f 0000 0029 0672 2200 0000  ....r....).r"...
+00000720: 7223 0000 00da 0b40 7079 5f61 7373 6572  r#.....@py_asser
+00000730: 7435 7224 0000 0072 2600 0000 da0b 4070  t5r$...r&.....@p
+00000740: 795f 666f 726d 6174 3972 2a00 0000 722a  y_format9r*...r*
+00000750: 0000 0072 2b00 0000 da0f 7465 7374 5f74  ...r+.....test_t
+00000760: 7769 6365 5f73 616d 650d 0000 0073 0200  wice_same....s..
+00000770: 0000 0001 7a20 4375 7272 656e 7454 6573  ....z CurrentTes
+00000780: 7454 6573 7473 2e74 6573 745f 7477 6963  tTests.test_twic
+00000790: 655f 7361 6d65 6301 0000 0000 0000 0000  e_samec.........
+000007a0: 0000 000a 0000 0007 0000 0043 0000 0073  ...........C...s
+000007b0: ca01 0000 6401 6402 8400 7d01 7c01 8300  ....d.d...}.|...
+000007c0: 7d02 7c02 6a00 7d03 7c03 7401 6b02 7d04  }.|.j.}.|.t.k.}.
+000007d0: 7c04 73a2 7402 a003 6403 7c04 6601 6404  |.s.t...d.|.f.d.
+000007e0: 7c03 7401 6602 a104 6405 7404 a005 a100  |.t.f...d.t.....
+000007f0: 7600 734a 7402 a006 7c02 a101 7254 7402  v.sJt...|...rTt.
+00000800: a007 7c02 a101 6e02 6405 7402 a007 7c03  ..|...n.d.t...|.
+00000810: a101 6406 7404 a005 a100 7600 7374 7402  ..d.t.....v.stt.
+00000820: a006 7401 a101 727e 7402 a007 7401 a101  ..t...r~t...t...
+00000830: 6e02 6406 6407 9c03 1600 7d05 6408 6409  n.d.d.....}.d.d.
+00000840: 7c05 6901 1600 7d06 7408 7402 a009 7c06  |.i...}.t.t...|.
+00000850: a101 8301 8201 6400 0400 7d03 7d04 7c02  ......d...}.}.|.
+00000860: 6a0a 7d03 6400 7d07 7c03 7c07 7500 7d04  j.}.d.}.|.|.u.}.
+00000870: 7c04 9001 732a 7402 a003 640a 7c04 6601  |...s*t...d.|.f.
+00000880: 640b 7c03 7c07 6602 a104 6405 7404 a005  d.|.|.f...d.t...
+00000890: a100 7600 73ec 7402 a006 7c02 a101 72f6  ..v.s.t...|...r.
+000008a0: 7402 a007 7c02 a101 6e02 6405 7402 a007  t...|...n.d.t...
+000008b0: 7c03 a101 7402 a007 7c07 a101 640c 9c03  |...t...|...d...
+000008c0: 1600 7d08 640d 640e 7c08 6901 1600 7d09  ..}.d.d.|.i...}.
+000008d0: 7408 7402 a009 7c09 a101 8301 8201 6400  t.t...|.......d.
+000008e0: 0400 7d03 0400 7d04 7d07 7c02 6a0b 7d03  ..}...}.}.|.j.}.
+000008f0: 640f 7d07 7c03 7c07 6b02 7d04 7c04 9001  d.}.|.|.k.}.|...
+00000900: 73ba 7402 a003 6403 7c04 6601 6410 7c03  s.t...d.|.f.d.|.
+00000910: 7c07 6602 a104 6405 7404 a005 a100 7600  |.f...d.t.....v.
+00000920: 9001 737c 7402 a006 7c02 a101 9001 7286  ..s|t...|.....r.
+00000930: 7402 a007 7c02 a101 6e02 6405 7402 a007  t...|...n.d.t...
+00000940: 7c03 a101 7402 a007 7c07 a101 640c 9c03  |...t...|...d...
+00000950: 1600 7d08 640d 640e 7c08 6901 1600 7d09  ..}.d.d.|.i...}.
+00000960: 7408 7402 a009 7c09 a101 8301 8201 6400  t.t...|.......d.
+00000970: 0400 7d03 0400 7d04 7d07 6400 5300 2911  ..}...}.}.d.S.).
+00000980: 4e63 0000 0000 0000 0000 0000 0000 0000  Nc..............
+00000990: 0000 0100 0000 5300 0000 7306 0000 0074  ......S...s....t
+000009a0: 0083 0053 0029 014e 2901 7203 0000 0072  ...S.).N).r....r
+000009b0: 2a00 0000 722a 0000 0072 2a00 0000 722b  *...r*...r*...r+
+000009c0: 0000 00da 1574 6573 745f 7468 6174 735f  .....test_thats_
+000009d0: 6675 6e63 7469 6f6e 616c 1100 0000 7302  functional....s.
+000009e0: 0000 0000 017a 3f43 7572 7265 6e74 5465  .....z?CurrentTe
+000009f0: 7374 5465 7374 732e 7465 7374 5f66 756e  stTests.test_fun
+00000a00: 6374 696f 6e61 6c2e 3c6c 6f63 616c 733e  ctional.<locals>
+00000a10: 2e74 6573 745f 7468 6174 735f 6675 6e63  .test_thats_func
+00000a20: 7469 6f6e 616c 7206 0000 0072 0800 0000  tionalr....r....
+00000a30: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
+00000a40: 0f00 0000 7210 0000 0029 01da 0269 7329  ....r....)...is)
+00000a50: 017a 3225 2870 7932 2973 0a7b 2528 7079  .z2%(py2)s.{%(py
+00000a60: 3229 7320 3d20 2528 7079 3029 732e 636c  2)s = %(py0)s.cl
+00000a70: 6173 735f 6e61 6d65 0a7d 2069 7320 2528  ass_name.} is %(
+00000a80: 7079 3529 7372 1100 0000 7213 0000 0072  py5)sr....r....r
+00000a90: 1400 0000 7230 0000 0072 1600 0000 290c  ....r0...r....).
+00000aa0: 7217 0000 0072 0a00 0000 7218 0000 0072  r....r....r....r
+00000ab0: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00000ac0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+00000ad0: 0000 7220 0000 0072 2100 0000 290a 7222  ..r ...r!...).r"
+00000ae0: 0000 0072 3000 0000 7209 0000 0072 2300  ...r0...r....r#.
+00000af0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+00000b00: 0072 2700 0000 7228 0000 0072 2900 0000  .r'...r(...r)...
+00000b10: 722a 0000 0072 2a00 0000 722b 0000 00da  r*...r*...r+....
+00000b20: 0f74 6573 745f 6675 6e63 7469 6f6e 616c  .test_functional
+00000b30: 1000 0000 730a 0000 0000 0108 0306 019c  ....s...........
+00000b40: 018c 017a 2043 7572 7265 6e74 5465 7374  ...z CurrentTest
+00000b50: 5465 7374 732e 7465 7374 5f66 756e 6374  Tests.test_funct
+00000b60: 696f 6e61 6c4e 2906 da08 5f5f 6e61 6d65  ionalN)...__name
+00000b70: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000b80: 5f5f 7175 616c 6e61 6d65 5f5f 7215 0000  __qualname__r...
+00000b90: 0072 2f00 0000 7232 0000 0072 2a00 0000  .r/...r2...r*...
+00000ba0: 722a 0000 0072 2a00 0000 722b 0000 0072  r*...r*...r+...r
+00000bb0: 0500 0000 0600 0000 7306 0000 0008 0108  ........s.......
+00000bc0: 0608 0372 0500 0000 6300 0000 0000 0000  ...r....c.......
+00000bd0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
+00000be0: 0073 3400 0000 6500 5a01 6400 5a02 6401  .s4...e.Z.d.Z.d.
+00000bf0: 6402 8400 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+00000c00: 6406 8400 5a05 6407 6408 8400 5a06 6409  d...Z.d.d...Z.d.
+00000c10: 640a 8400 5a07 640b 5300 290c da10 536f  d...Z.d.S.)...So
+00000c20: 7274 6564 4e61 6d65 7354 6573 7473 6301  rtedNamesTestsc.
+00000c30: 0000 0000 0000 0000 0000 0007 0000 0007  ................
+00000c40: 0000 0043 0000 0073 a000 0000 6700 7d01  ...C...s....g.}.
+00000c50: 7400 7c01 8301 7d02 6700 7d03 7c02 7c03  t.|...}.g.}.|.|.
+00000c60: 6b02 7d04 7c04 738c 7401 a002 6401 7c04  k.}.|.s.t...d.|.
+00000c70: 6601 6402 7c02 7c03 6602 a104 6403 7403  f.d.|.|.f...d.t.
+00000c80: a004 a100 7600 7346 7401 a005 7400 a101  ....v.sFt...t...
+00000c90: 7250 7401 a006 7400 a101 6e02 6403 7401  rPt...t...n.d.t.
+00000ca0: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
+00000cb0: a006 7c03 a101 6404 9c04 1600 7d05 6405  ..|...d.....}.d.
+00000cc0: 6406 7c05 6901 1600 7d06 7407 7401 a008  d.|.i...}.t.t...
+00000cd0: 7c06 a101 8301 8201 6400 0400 7d01 0400  |.......d...}...
+00000ce0: 7d02 0400 7d04 7d03 6400 5300 2907 4e72  }...}.}.d.S.).Nr
+00000cf0: 0600 0000 a901 7a30 2528 7079 3429 730a  ......z0%(py4)s.
+00000d00: 7b25 2870 7934 2973 203d 2025 2870 7930  {%(py4)s = %(py0
+00000d10: 2973 2825 2870 7932 2973 290a 7d20 3d3d  )s(%(py2)s).} ==
+00000d20: 2025 2870 7937 2973 7204 0000 00a9 0472   %(py7)sr......r
+00000d30: 0c00 0000 720d 0000 0072 0e00 0000 7214  ....r....r....r.
+00000d40: 0000 00fa 0e61 7373 6572 7420 2528 7079  .....assert %(py
+00000d50: 3929 73da 0370 7939 a909 7204 0000 0072  9)s..py9..r....r
+00000d60: 1800 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
+00000d70: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000d80: 0000 721f 0000 00a9 0772 2200 0000 7223  ..r......r"...r#
+00000d90: 0000 0072 2400 0000 da0b 4070 795f 6173  ...r$.....@py_as
+00000da0: 7365 7274 3672 2d00 0000 7229 0000 00da  sert6r-...r)....
+00000db0: 0c40 7079 5f66 6f72 6d61 7431 3072 2a00  .@py_format10r*.
+00000dc0: 0000 722a 0000 0072 2b00 0000 da0a 7465  ..r*...r+.....te
+00000dd0: 7374 5f65 6d70 7479 1b00 0000 7302 0000  st_empty....s...
+00000de0: 0000 017a 1b53 6f72 7465 644e 616d 6573  ...z.SortedNames
+00000df0: 5465 7374 732e 7465 7374 5f65 6d70 7479  Tests.test_empty
+00000e00: 6301 0000 0000 0000 0000 0000 0007 0000  c...............
+00000e10: 0007 0000 0043 0000 0073 a400 0000 6401  .....C...s....d.
+00000e20: 6701 7d01 7400 7c01 8301 7d02 6401 6701  g.}.t.|...}.d.g.
+00000e30: 7d03 7c02 7c03 6b02 7d04 7c04 7390 7401  }.|.|.k.}.|.s.t.
+00000e40: a002 6402 7c04 6601 6403 7c02 7c03 6602  ..d.|.f.d.|.|.f.
+00000e50: a104 6404 7403 a004 a100 7600 734a 7401  ..d.t.....v.sJt.
+00000e60: a005 7400 a101 7254 7401 a006 7400 a101  ..t...rTt...t...
+00000e70: 6e02 6404 7401 a006 7c01 a101 7401 a006  n.d.t...|...t...
+00000e80: 7c02 a101 7401 a006 7c03 a101 6405 9c04  |...t...|...d...
+00000e90: 1600 7d05 6406 6407 7c05 6901 1600 7d06  ..}.d.d.|.i...}.
+00000ea0: 7407 7401 a008 7c06 a101 8301 8201 6400  t.t...|.......d.
+00000eb0: 0400 7d01 0400 7d02 0400 7d04 7d03 6400  ..}...}...}.}.d.
+00000ec0: 5300 2908 4eda 0764 6566 6175 6c74 7206  S.).N..defaultr.
+00000ed0: 0000 0072 3700 0000 7204 0000 0072 3800  ...r7...r....r8.
+00000ee0: 0000 7239 0000 0072 3a00 0000 723b 0000  ..r9...r:...r;..
+00000ef0: 0072 3c00 0000 722a 0000 0072 2a00 0000  .r<...r*...r*...
+00000f00: 722b 0000 00da 1174 6573 745f 6a75 7374  r+.....test_just
+00000f10: 5f64 6566 6175 6c74 1e00 0000 7302 0000  _default....s...
+00000f20: 0000 017a 2253 6f72 7465 644e 616d 6573  ...z"SortedNames
+00000f30: 5465 7374 732e 7465 7374 5f6a 7573 745f  Tests.test_just_
+00000f40: 6465 6661 756c 7463 0100 0000 0000 0000  defaultc........
+00000f50: 0000 0000 0700 0000 0700 0000 4300 0000  ............C...
+00000f60: 73a4 0000 0064 0167 017d 0174 007c 0183  s....d.g.}.t.|..
+00000f70: 017d 0264 0167 017d 037c 027c 036b 027d  .}.d.g.}.|.|.k.}
+00000f80: 047c 0473 9074 01a0 0264 027c 0466 0164  .|.s.t...d.|.f.d
+00000f90: 037c 027c 0366 02a1 0464 0474 03a0 04a1  .|.|.f...d.t....
+00000fa0: 0076 0073 4a74 01a0 0574 00a1 0172 5474  .v.sJt...t...rTt
+00000fb0: 01a0 0674 00a1 016e 0264 0474 01a0 067c  ...t...n.d.t...|
+00000fc0: 01a1 0174 01a0 067c 02a1 0174 01a0 067c  ...t...|...t...|
+00000fd0: 03a1 0164 059c 0416 007d 0564 0664 077c  ...d.....}.d.d.|
+00000fe0: 0569 0116 007d 0674 0774 01a0 087c 06a1  .i...}.t.t...|..
+00000ff0: 0183 0182 0164 0004 007d 0104 007d 0204  .....d...}...}..
+00001000: 007d 047d 0364 0053 0029 084e 5a09 736f  .}.}.d.S.).NZ.so
+00001010: 6d65 7468 696e 6772 0600 0000 7237 0000  methingr....r7..
+00001020: 0072 0400 0000 7238 0000 0072 3900 0000  .r....r8...r9...
+00001030: 723a 0000 0072 3b00 0000 723c 0000 0072  r:...r;...r<...r
+00001040: 2a00 0000 722a 0000 0072 2b00 0000 da13  *...r*...r+.....
+00001050: 7465 7374 5f6a 7573 745f 736f 6d65 7468  test_just_someth
+00001060: 696e 6721 0000 0073 0200 0000 0001 7a24  ing!...s......z$
+00001070: 536f 7274 6564 4e61 6d65 7354 6573 7473  SortedNamesTests
+00001080: 2e74 6573 745f 6a75 7374 5f73 6f6d 6574  .test_just_somet
+00001090: 6869 6e67 6301 0000 0000 0000 0000 0000  hingc...........
+000010a0: 0007 0000 0007 0000 0043 0000 0073 a800  .........C...s..
+000010b0: 0000 6401 6402 6702 7d01 7400 7c01 8301  ..d.d.g.}.t.|...
+000010c0: 7d02 6402 6401 6702 7d03 7c02 7c03 6b02  }.d.d.g.}.|.|.k.
+000010d0: 7d04 7c04 7394 7401 a002 6403 7c04 6601  }.|.s.t...d.|.f.
+000010e0: 6404 7c02 7c03 6602 a104 6405 7403 a004  d.|.|.f...d.t...
+000010f0: a100 7600 734e 7401 a005 7400 a101 7258  ..v.sNt...t...rX
+00001100: 7401 a006 7400 a101 6e02 6405 7401 a006  t...t...n.d.t...
+00001110: 7c01 a101 7401 a006 7c02 a101 7401 a006  |...t...|...t...
+00001120: 7c03 a101 6406 9c04 1600 7d05 6407 6408  |...d.....}.d.d.
+00001130: 7c05 6901 1600 7d06 7407 7401 a008 7c06  |.i...}.t.t...|.
+00001140: a101 8301 8201 6400 0400 7d01 0400 7d02  ......d...}...}.
+00001150: 0400 7d04 7d03 6400 5300 2909 4eda 0162  ..}.}.d.S.).N..b
+00001160: da01 6172 0600 0000 7237 0000 0072 0400  ..ar....r7...r..
+00001170: 0000 7238 0000 0072 3900 0000 723a 0000  ..r8...r9...r:..
+00001180: 0072 3b00 0000 723c 0000 0072 2a00 0000  .r;...r<...r*...
+00001190: 722a 0000 0072 2b00 0000 da0e 7465 7374  r*...r+.....test
+000011a0: 5f64 6f65 735f 736f 7274 2400 0000 7302  _does_sort$...s.
+000011b0: 0000 0000 017a 1f53 6f72 7465 644e 616d  .....z.SortedNam
+000011c0: 6573 5465 7374 732e 7465 7374 5f64 6f65  esTests.test_doe
+000011d0: 735f 736f 7274 6301 0000 0000 0000 0000  s_sortc.........
+000011e0: 0000 0007 0000 0007 0000 0043 0000 0073  ...........C...s
+000011f0: a800 0000 6401 6402 6702 7d01 7400 7c01  ....d.d.g.}.t.|.
+00001200: 8301 7d02 6402 6401 6702 7d03 7c02 7c03  ..}.d.d.g.}.|.|.
+00001210: 6b02 7d04 7c04 7394 7401 a002 6403 7c04  k.}.|.s.t...d.|.
+00001220: 6601 6404 7c02 7c03 6602 a104 6405 7403  f.d.|.|.f...d.t.
+00001230: a004 a100 7600 734e 7401 a005 7400 a101  ....v.sNt...t...
+00001240: 7258 7401 a006 7400 a101 6e02 6405 7401  rXt...t...n.d.t.
+00001250: a006 7c01 a101 7401 a006 7c02 a101 7401  ..|...t...|...t.
+00001260: a006 7c03 a101 6406 9c04 1600 7d05 6407  ..|...d.....}.d.
+00001270: 6408 7c05 6901 1600 7d06 7407 7401 a008  d.|.i...}.t.t...
+00001280: 7c06 a101 8301 8201 6400 0400 7d01 0400  |.......d...}...
+00001290: 7d02 0400 7d04 7d03 6400 5300 2909 4e72  }...}.}.d.S.).Nr
+000012a0: 4400 0000 7240 0000 0072 0600 0000 7237  D...r@...r....r7
+000012b0: 0000 0072 0400 0000 7238 0000 0072 3900  ...r....r8...r9.
+000012c0: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
+000012d0: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
+000012e0: da1d 7465 7374 5f73 6f72 745f 6b65 6570  ..test_sort_keep
+000012f0: 735f 6465 6661 756c 745f 6669 7273 7427  s_default_first'
+00001300: 0000 0073 0200 0000 0001 7a2e 536f 7274  ...s......z.Sort
+00001310: 6564 4e61 6d65 7354 6573 7473 2e74 6573  edNamesTests.tes
+00001320: 745f 736f 7274 5f6b 6565 7073 5f64 6566  t_sort_keeps_def
+00001330: 6175 6c74 5f66 6972 7374 4e29 0872 3300  ault_firstN).r3.
+00001340: 0000 7234 0000 0072 3500 0000 723f 0000  ..r4...r5...r?..
+00001350: 0072 4100 0000 7242 0000 0072 4500 0000  .rA...rB...rE...
+00001360: 7246 0000 0072 2a00 0000 722a 0000 0072  rF...r*...r*...r
+00001370: 2a00 0000 722b 0000 0072 3600 0000 1a00  *...r+...r6.....
+00001380: 0000 730a 0000 0008 0108 0308 0308 0308  ..s.............
+00001390: 0372 3600 0000 290d da08 6275 696c 7469  .r6...)...builti
+000013a0: 6e73 721a 0000 00da 195f 7079 7465 7374  nsr......_pytest
+000013b0: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
+000013c0: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
+000013d0: 6577 7269 7465 7218 0000 00da 0b64 6a61  ewriter......dja
+000013e0: 6e67 6f2e 7465 7374 7202 0000 00da 1564  ngo.testr......d
+000013f0: 6a61 6e67 6f5f 7065 7266 5f72 6563 2e75  jango_perf_rec.u
+00001400: 7469 6c73 7203 0000 0072 0400 0000 7205  tilsr....r....r.
+00001410: 0000 0072 3600 0000 722a 0000 0072 2a00  ...r6...r*...r*.
+00001420: 0000 722a 0000 0072 2b00 0000 da08 3c6d  ..r*...r+.....<m
+00001430: 6f64 756c 653e 0100 0000 7306 0000 0026  odule>....s....&
+00001440: 0210 0310 14                             .....
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-35-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-35-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-36-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-36-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.1.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.1.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.4.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.2.4.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.3.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.3.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-37-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-39-pytest-6.1.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff.*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,549 +1,493 @@
-00000000: 420d 0d0a 7d79 7c5e ef09 0000 e300 0000  B...}y|^........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 6a00 0000 6400 6401 6c00 5a01 6400  .sj...d.d.l.Z.d.
-00000030: 6401 6c02 6d03 0200 0100 6d04 5a05 0100  d.l.m.....m.Z...
-00000040: 6400 6401 6c06 5a06 6400 6402 6c07 6d08  d.d.l.Z.d.d.l.m.
-00000050: 5a08 0100 6400 6401 6c09 5a09 6400 6401  Z...d.d.l.Z.d.d.
-00000060: 6c0a 5a0a 6400 6403 6c0b 6d0c 5a0c 0100  l.Z.d.d.l.m.Z...
-00000070: 6400 6404 6c0d 6d0e 5a0e 0100 4700 6405  d.d.l.m.Z...G.d.
-00000080: 6406 8400 6406 650c 8303 5a0f 6401 5300  d...d.e...Z.d.S.
-00000090: 2907 e900 0000 004e 2901 da07 6d6b 6474  )......N)...mkdt
-000000a0: 656d 7029 01da 0e53 696d 706c 6554 6573  emp)...SimpleTes
-000000b0: 7443 6173 6529 01da 064b 5646 696c 6563  tCase)...KVFilec
-000000c0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-000000d0: 0000 0000 7370 0000 0065 005a 0164 005a  ....sp...e.Z.d.Z
-000000e0: 0287 0066 0164 0164 0284 085a 0387 0066  ...f.d.d...Z...f
-000000f0: 0164 0364 0484 085a 0464 0564 0684 005a  .d.d...Z.d.d...Z
-00000100: 0564 0764 0884 005a 0664 0964 0a84 005a  .d.d...Z.d.d...Z
-00000110: 0764 0b64 0c84 005a 0864 0d64 0e84 005a  .d.d...Z.d.d...Z
-00000120: 0964 0f64 1084 005a 0a64 1164 1284 005a  .d.d...Z.d.d...Z
-00000130: 0b64 1364 1484 005a 0c64 1564 1684 005a  .d.d...Z.d.d...Z
-00000140: 0d87 0004 005a 0e53 0029 17da 0b4b 5646  .....Z.S.)...KVF
-00000150: 696c 6554 6573 7473 6301 0000 0000 0000  ileTestsc.......
-00000160: 0001 0000 0002 0000 0003 0000 0073 1e00  .............s..
-00000170: 0000 7400 8300 a001 a100 0100 7402 a003  ..t.........t...
-00000180: a100 0100 7404 8300 7c00 5f05 6400 5300  ....t...|._.d.S.
-00000190: 2901 4e29 06da 0573 7570 6572 da05 7365  ).N)...super..se
-000001a0: 7455 7072 0400 0000 da11 5f63 6c65 6172  tUpr......_clear
-000001b0: 5f6c 6f61 645f 6361 6368 6572 0200 0000  _load_cacher....
-000001c0: da08 7465 6d70 5f64 6972 2901 da04 7365  ..temp_dir)...se
-000001d0: 6c66 2901 da09 5f5f 636c 6173 735f 5fa9  lf)...__class__.
-000001e0: 00fa 432f 5573 6572 732f 6368 6169 6e7a  ..C/Users/chainz
-000001f0: 2f44 6f63 756d 656e 7473 2f50 726f 6a65  /Documents/Proje
-00000200: 6374 732f 646a 616e 676f 2d70 6572 662d  cts/django-perf-
-00000210: 7265 632f 7465 7374 732f 7465 7374 5f79  rec/tests/test_y
-00000220: 616d 6c2e 7079 7207 0000 000c 0000 0073  aml.pyr........s
-00000230: 0600 0000 0001 0a01 0801 7a11 4b56 4669  ..........z.KVFi
-00000240: 6c65 5465 7374 732e 7365 7455 7063 0100  leTests.setUpc..
-00000250: 0000 0000 0000 0100 0000 0300 0000 0300  ................
-00000260: 0000 731a 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
-00000270: 0101 0074 0383 00a0 04a1 0001 0064 0053  ...t.........d.S
-00000280: 0029 014e 2905 da06 7368 7574 696c da06  .).N)...shutil..
-00000290: 726d 7472 6565 7209 0000 0072 0600 0000  rmtreer....r....
-000002a0: da08 7465 6172 446f 776e 2901 720a 0000  ..tearDown).r...
-000002b0: 0029 0172 0b00 0000 720c 0000 0072 0d00  .).r....r....r..
-000002c0: 0000 7210 0000 0011 0000 0073 0400 0000  ..r........s....
-000002d0: 0001 0c01 7a14 4b56 4669 6c65 5465 7374  ....z.KVFileTest
-000002e0: 732e 7465 6172 446f 776e 6301 0000 0000  s.tearDownc.....
-000002f0: 0000 0001 0000 0009 0000 0043 0000 0073  ...........C...s
-00000300: 2200 0000 7400 a001 7402 a101 8f0e 0100  "...t...t.......
-00000310: 7403 6401 8301 0100 5700 6400 5100 5200  t.d.....W.d.Q.R.
-00000320: 5800 6400 5300 2902 4efa 012f 2904 da06  X.d.S.).N../)...
-00000330: 7079 7465 7374 da06 7261 6973 6573 da07  pytest..raises..
-00000340: 494f 4572 726f 7272 0400 0000 2901 720a  IOErrorr....).r.
-00000350: 0000 0072 0c00 0000 720c 0000 0072 0d00  ...r....r....r..
-00000360: 0000 da18 7465 7374 5f6c 6f61 645f 6e6f  ....test_load_no
-00000370: 5f70 6572 6d69 7373 696f 6e73 1500 0000  _permissions....
-00000380: 7304 0000 0000 010c 017a 244b 5646 696c  s........z$KVFil
-00000390: 6554 6573 7473 2e74 6573 745f 6c6f 6164  eTests.test_load
-000003a0: 5f6e 6f5f 7065 726d 6973 7369 6f6e 7363  _no_permissionsc
-000003b0: 0100 0000 0000 0000 0e00 0000 0900 0000  ................
-000003c0: 4300 0000 73b8 0100 0074 007c 006a 0164  C...s....t.|.j.d
-000003d0: 0117 0083 017d 0174 027c 0183 017d 0264  .....}.t.|...}.d
-000003e0: 027d 037c 027c 036b 027d 047c 0473 b074  .}.|.|.k.}.|.s.t
-000003f0: 03a0 0464 037c 0466 0164 047c 027c 0366  ...d.|.f.d.|.|.f
-00000400: 02a1 0464 0574 05a0 06a1 006b 0673 5074  ...d.t.....k.sPt
-00000410: 03a0 0774 02a1 0172 5a74 03a0 0874 02a1  ...t...rZt...t..
-00000420: 016e 0264 0564 0674 05a0 06a1 006b 0673  .n.d.d.t.....k.s
-00000430: 7274 03a0 077c 01a1 0172 7c74 03a0 087c  rt...|...r|t...|
-00000440: 01a1 016e 0264 0674 03a0 087c 02a1 0174  ...n.d.t...|...t
-00000450: 03a0 087c 03a1 0164 079c 0416 007d 0564  ...|...d.....}.d
-00000460: 0864 097c 0569 0116 007d 0674 0974 03a0  .d.|.i...}.t.t..
-00000470: 0a7c 06a1 0183 0182 0164 0004 007d 0204  .|.......d...}..
-00000480: 007d 047d 0374 0b83 007d 077c 016a 0c7d  .}.}.t...}.|.j.}
-00000490: 0864 0a7d 097c 087c 097c 0783 027d 0a7c  .d.}.|.|.|...}.|
-000004a0: 0a7c 076b 087d 0b7c 0b90 0173 a474 03a0  .|.k.}.|...s.t..
-000004b0: 0464 0b7c 0b66 0164 0c7c 0a7c 0766 02a1  .d.|.f.d.|.|.f..
-000004c0: 0464 0674 05a0 06a1 006b 0690 0173 1274  .d.t.....k...s.t
-000004d0: 03a0 077c 01a1 0190 0172 1c74 03a0 087c  ...|.....r.t...|
-000004e0: 01a1 016e 0264 0674 03a0 087c 08a1 0174  ...n.d.t...|...t
-000004f0: 03a0 087c 09a1 0164 0d74 05a0 06a1 006b  ...|...d.t.....k
-00000500: 0690 0173 4874 03a0 077c 07a1 0190 0172  ...sHt...|.....r
-00000510: 5274 03a0 087c 07a1 016e 0264 0d74 03a0  Rt...|...n.d.t..
-00000520: 087c 0aa1 0164 0d74 05a0 06a1 006b 0690  .|...d.t.....k..
-00000530: 0173 7674 03a0 077c 07a1 0190 0172 8074  .svt...|.....r.t
-00000540: 03a0 087c 07a1 016e 0264 0d64 0e9c 0616  ...|...n.d.d....
-00000550: 007d 0c64 0f64 107c 0c69 0116 007d 0d74  .}.d.d.|.i...}.t
-00000560: 0974 03a0 0a7c 0da1 0183 0182 0164 0004  .t...|.......d..
-00000570: 007d 0804 007d 0904 007d 0a7d 0b64 0053  .}...}...}.}.d.S
-00000580: 0029 114e 7a08 2f66 6f6f 2e79 6d6c 7201  .).Nz./foo.ymlr.
-00000590: 0000 0029 01fa 023d 3d29 017a 3025 2870  ...)...==).z0%(p
-000005a0: 7933 2973 0a7b 2528 7079 3329 7320 3d20  y3)s.{%(py3)s = 
-000005b0: 2528 7079 3029 7328 2528 7079 3129 7329  %(py0)s(%(py1)s)
-000005c0: 0a7d 203d 3d20 2528 7079 3629 73da 036c  .} == %(py6)s..l
-000005d0: 656e da03 6b76 6629 04da 0370 7930 da03  en..kvf)...py0..
-000005e0: 7079 31da 0370 7933 da03 7079 367a 0e61  py1..py3..py6z.a
-000005f0: 7373 6572 7420 2528 7079 3829 73da 0370  ssert %(py8)s..p
-00000600: 7938 da03 666f 6f29 01da 0269 7329 017a  y8..foo)...is).z
-00000610: 5225 2870 7937 2973 0a7b 2528 7079 3729  R%(py7)s.{%(py7)
-00000620: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
-00000630: 7932 2973 203d 2025 2870 7930 2973 2e67  y2)s = %(py0)s.g
-00000640: 6574 0a7d 2825 2870 7934 2973 2c20 2528  et.}(%(py4)s, %(
-00000650: 7079 3529 7329 0a7d 2069 7320 2528 7079  py5)s).} is %(py
-00000660: 3929 73da 0764 6566 6175 6c74 2906 7219  9)s..default).r.
-00000670: 0000 00da 0370 7932 da03 7079 34da 0370  .....py2..py4..p
-00000680: 7935 da03 7079 37da 0370 7939 7a0f 6173  y5..py7..py9z.as
-00000690: 7365 7274 2025 2870 7931 3129 73da 0470  sert %(py11)s..p
-000006a0: 7931 3129 0d72 0400 0000 7209 0000 0072  y11).r....r....r
-000006b0: 1700 0000 da0a 4070 7974 6573 745f 6172  ......@pytest_ar
-000006c0: da11 5f63 616c 6c5f 7265 7072 636f 6d70  .._call_reprcomp
-000006d0: 6172 65da 0c40 7079 5f62 7569 6c74 696e  are..@py_builtin
-000006e0: 73da 066c 6f63 616c 73da 185f 7368 6f75  s..locals.._shou
-000006f0: 6c64 5f72 6570 725f 676c 6f62 616c 5f6e  ld_repr_global_n
-00000700: 616d 65da 095f 7361 6665 7265 7072 da0e  ame.._saferepr..
-00000710: 4173 7365 7274 696f 6e45 7272 6f72 da13  AssertionError..
-00000720: 5f66 6f72 6d61 745f 6578 706c 616e 6174  _format_explanat
-00000730: 696f 6eda 066f 626a 6563 74da 0367 6574  ion..object..get
-00000740: 290e 720a 0000 0072 1800 0000 da0b 4070  ).r....r......@p
-00000750: 795f 6173 7365 7274 32da 0b40 7079 5f61  y_assert2..@py_a
-00000760: 7373 6572 7435 da0b 4070 795f 6173 7365  ssert5..@py_asse
-00000770: 7274 34da 0b40 7079 5f66 6f72 6d61 7437  rt4..@py_format7
-00000780: da0b 4070 795f 666f 726d 6174 3972 2000  ..@py_format9r .
-00000790: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
-000007a0: 0b40 7079 5f61 7373 6572 7433 da0b 4070  .@py_assert3..@p
-000007b0: 795f 6173 7365 7274 36da 0b40 7079 5f61  y_assert6..@py_a
-000007c0: 7373 6572 7438 da0c 4070 795f 666f 726d  ssert8..@py_form
-000007d0: 6174 3130 da0c 4070 795f 666f 726d 6174  at10..@py_format
-000007e0: 3132 720c 0000 0072 0c00 0000 720d 0000  12r....r....r...
-000007f0: 00da 1f74 6573 745f 6c6f 6164 5f6e 6f6e  ...test_load_non
-00000800: 5f65 7869 7374 656e 745f 6973 5f65 6d70  _existent_is_emp
-00000810: 7479 1900 0000 7326 0000 0000 010e 0108  ty....s&........
-00000820: 0004 0008 0004 0070 000c 000e 000c 0106  .......p........
-00000830: 0106 0004 000a 0008 0006 00a6 000c 000e  ................
-00000840: 007a 2b4b 5646 696c 6554 6573 7473 2e74  .z+KVFileTests.t
-00000850: 6573 745f 6c6f 6164 5f6e 6f6e 5f65 7869  est_load_non_exi
-00000860: 7374 656e 745f 6973 5f65 6d70 7479 6301  stent_is_emptyc.
-00000870: 0000 0000 0000 0010 0000 0009 0000 0043  ...............C
-00000880: 0000 0073 aa01 0000 7c00 6a00 6401 1700  ...s....|.j.d...
-00000890: 7d01 7401 7c01 6402 8302 8f10 7d02 7c02  }.t.|.d.....}.|.
-000008a0: a002 6403 a101 0100 5700 6400 5100 5200  ..d.....W.d.Q.R.
-000008b0: 5800 7403 7c01 8301 7d03 7404 7c03 8301  X.t.|...}.t.|...
-000008c0: 7d04 6404 7d05 7c04 7c05 6b02 7d06 7c06  }.d.}.|.|.k.}.|.
-000008d0: 73d4 7405 a006 6405 7c06 6601 6406 7c04  s.t...d.|.f.d.|.
-000008e0: 7c05 6602 a104 6407 7407 a008 a100 6b06  |.f...d.t.....k.
-000008f0: 7374 7405 a009 7404 a101 727e 7405 a00a  stt...t...r~t...
-00000900: 7404 a101 6e02 6407 6408 7407 a008 a100  t...n.d.d.t.....
-00000910: 6b06 7396 7405 a009 7c03 a101 72a0 7405  k.s.t...|...r.t.
-00000920: a00a 7c03 a101 6e02 6408 7405 a00a 7c04  ..|...n.d.t...|.
-00000930: a101 7405 a00a 7c05 a101 6409 9c04 1600  ..t...|...d.....
-00000940: 7d07 640a 640b 7c07 6901 1600 7d08 740b  }.d.d.|.i...}.t.
-00000950: 7405 a00c 7c08 a101 8301 8201 6400 0400  t...|.......d...
-00000960: 7d04 0400 7d06 7d05 7c03 6a0d 7d09 640c  }...}.}.|.j.}.d.
-00000970: 7d0a 640d 7d05 7c09 7c0a 7c05 8302 7d0b  }.d.}.|.|.|...}.
-00000980: 640e 7d0c 7c0b 7c0c 6b02 7d0d 7c0d 9001  d.}.|.|.k.}.|...
-00000990: 738e 7405 a006 6405 7c0d 6601 640f 7c0b  s.t...d.|.f.d.|.
-000009a0: 7c0c 6602 a104 6408 7407 a008 a100 6b06  |.f...d.t.....k.
-000009b0: 9001 7338 7405 a009 7c03 a101 9001 7242  ..s8t...|.....rB
-000009c0: 7405 a00a 7c03 a101 6e02 6408 7405 a00a  t...|...n.d.t...
-000009d0: 7c09 a101 7405 a00a 7c0a a101 7405 a00a  |...t...|...t...
-000009e0: 7c05 a101 7405 a00a 7c0b a101 7405 a00a  |...t...|...t...
-000009f0: 7c0c a101 6410 9c06 1600 7d0e 6411 6412  |...d.....}.d.d.
-00000a00: 7c0e 6901 1600 7d0f 740b 7405 a00c 7c0f  |.i...}.t.t...|.
-00000a10: a101 8301 8201 6400 0400 7d09 0400 7d0a  ......d...}...}.
-00000a20: 0400 7d05 0400 7d0b 0400 7d0d 7d0c 6400  ..}...}...}.}.d.
-00000a30: 5300 2913 4e7a 082f 666f 6f2e 796d 6cda  S.).Nz./foo.yml.
-00000a40: 0177 7a08 666f 6f3a 2062 6172 e901 0000  .wz.foo: bar....
-00000a50: 0029 0172 1600 0000 2901 7a30 2528 7079  .).r....).z0%(py
-00000a60: 3329 730a 7b25 2870 7933 2973 203d 2025  3)s.{%(py3)s = %
-00000a70: 2870 7930 2973 2825 2870 7931 2973 290a  (py0)s(%(py1)s).
-00000a80: 7d20 3d3d 2025 2870 7936 2973 7217 0000  } == %(py6)sr...
-00000a90: 0072 1800 0000 2904 7219 0000 0072 1a00  .r....).r....r..
-00000aa0: 0000 721b 0000 0072 1c00 0000 7a0e 6173  ..r....r....z.as
-00000ab0: 7365 7274 2025 2870 7938 2973 721d 0000  sert %(py8)sr...
-00000ac0: 0072 1e00 0000 da00 da03 6261 7229 017a  .r........bar).z
-00000ad0: 5325 2870 7938 2973 0a7b 2528 7079 3829  S%(py8)s.{%(py8)
-00000ae0: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
-00000af0: 7932 2973 203d 2025 2870 7930 2973 2e67  y2)s = %(py0)s.g
-00000b00: 6574 0a7d 2825 2870 7934 2973 2c20 2528  et.}(%(py4)s, %(
-00000b10: 7079 3629 7329 0a7d 203d 3d20 2528 7079  py6)s).} == %(py
-00000b20: 3131 2973 2906 7219 0000 0072 2100 0000  11)s).r....r!...
-00000b30: 7222 0000 0072 1c00 0000 721d 0000 0072  r"...r....r....r
-00000b40: 2600 0000 7a0f 6173 7365 7274 2025 2870  &...z.assert %(p
-00000b50: 7931 3329 73da 0470 7931 3329 0e72 0900  y13)s..py13).r..
-00000b60: 0000 da04 6f70 656e da05 7772 6974 6572  ....open..writer
-00000b70: 0400 0000 7217 0000 0072 2700 0000 7228  ....r....r'...r(
-00000b80: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00000b90: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00000ba0: 0072 3000 0000 2910 720a 0000 00da 0966  .r0...).r......f
-00000bb0: 696c 655f 6e61 6d65 da02 6670 7218 0000  ile_name..fpr...
-00000bc0: 0072 3100 0000 7232 0000 0072 3300 0000  .r1...r2...r3...
-00000bd0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
-00000be0: 3700 0000 da0b 4070 795f 6173 7365 7274  7.....@py_assert
-00000bf0: 37da 0c40 7079 5f61 7373 6572 7431 30da  7..@py_assert10.
-00000c00: 0b40 7079 5f61 7373 6572 7439 723b 0000  .@py_assert9r;..
-00000c10: 00da 0c40 7079 5f66 6f72 6d61 7431 3472  ...@py_format14r
-00000c20: 0c00 0000 720c 0000 0072 0d00 0000 da12  ....r....r......
-00000c30: 7465 7374 5f6c 6f61 645f 6578 6973 7465  test_load_existe
-00000c40: 6e74 1f00 0000 732e 0000 0000 010a 010c  nt....s.........
-00000c50: 0114 0208 0108 0004 0008 0004 0070 000c  .............p..
-00000c60: 000e 000c 0106 0004 0004 000a 0004 0008  ................
-00000c70: 0006 006a 000c 000e 007a 1e4b 5646 696c  ...j.....z.KVFil
-00000c80: 6554 6573 7473 2e74 6573 745f 6c6f 6164  eTests.test_load
-00000c90: 5f65 7869 7374 656e 7463 0100 0000 0000  _existentc......
-00000ca0: 0000 0900 0000 0900 0000 4300 0000 7312  ..........C...s.
-00000cb0: 0100 007c 006a 0064 0117 007d 0174 017c  ...|.j.d...}.t.|
-00000cc0: 0164 0283 028f 107d 027c 02a0 0264 03a1  .d.....}.|...d..
-00000cd0: 0101 0057 0064 0051 0052 0058 0074 037c  ...W.d.Q.R.X.t.|
-00000ce0: 0183 017d 0374 047c 0383 017d 0464 047d  ...}.t.|...}.d.}
-00000cf0: 057c 047c 056b 027d 067c 0673 fe74 05a0  .|.|.k.}.|.s.t..
-00000d00: 0664 057c 0666 0164 067c 047c 0566 02a1  .d.|.f.d.|.|.f..
-00000d10: 0464 0774 07a0 08a1 006b 0673 7474 05a0  .d.t.....k.stt..
-00000d20: 0974 04a1 0172 7e74 05a0 0a74 04a1 016e  .t...r~t...t...n
-00000d30: 0264 0764 0874 07a0 08a1 006b 0673 9674  .d.d.t.....k.s.t
-00000d40: 05a0 0974 03a1 0172 a074 05a0 0a74 03a1  ...t...r.t...t..
-00000d50: 016e 0264 0864 0974 07a0 08a1 006b 0673  .n.d.d.t.....k.s
-00000d60: b874 05a0 097c 01a1 0172 c274 05a0 0a7c  .t...|...r.t...|
-00000d70: 01a1 016e 0264 0974 05a0 0a7c 03a1 0174  ...n.d.t...|...t
-00000d80: 05a0 0a7c 04a1 0174 05a0 0a7c 05a1 0164  ...|...t...|...d
-00000d90: 0a9c 0616 007d 0764 0b64 0c7c 0769 0116  .....}.d.d.|.i..
-00000da0: 007d 0874 0b74 05a0 0c7c 08a1 0183 0182  .}.t.t...|......
-00000db0: 0164 0004 007d 0304 007d 0404 007d 067d  .d...}...}...}.}
-00000dc0: 0564 0053 0029 0d4e 7a08 2f66 6f6f 2e79  .d.S.).Nz./foo.y
-00000dd0: 6d6c 723d 0000 0072 3f00 0000 7201 0000  mlr=...r?...r...
-00000de0: 0029 0172 1600 0000 2901 7a4e 2528 7079  .).r....).zN%(py
-00000df0: 3629 730a 7b25 2870 7936 2973 203d 2025  6)s.{%(py6)s = %
-00000e00: 2870 7930 2973 2825 2870 7934 2973 0a7b  (py0)s(%(py4)s.{
-00000e10: 2528 7079 3429 7320 3d20 2528 7079 3129  %(py4)s = %(py1)
-00000e20: 7328 2528 7079 3229 7329 0a7d 290a 7d20  s(%(py2)s).}).} 
-00000e30: 3d3d 2025 2870 7939 2973 7217 0000 0072  == %(py9)sr....r
-00000e40: 0400 0000 7244 0000 0029 0672 1900 0000  ....rD...).r....
-00000e50: 721a 0000 0072 2100 0000 7222 0000 0072  r....r!...r"...r
-00000e60: 1c00 0000 7225 0000 007a 0f61 7373 6572  ....r%...z.asser
-00000e70: 7420 2528 7079 3131 2973 7226 0000 0029  t %(py11)sr&...)
-00000e80: 0d72 0900 0000 7242 0000 0072 4300 0000  .r....rB...rC...
-00000e90: 7204 0000 0072 1700 0000 7227 0000 0072  r....r....r'...r
-00000ea0: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
-00000eb0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00000ec0: 0000 2909 720a 0000 0072 4400 0000 7245  ..).r....rD...rE
-00000ed0: 0000 0072 3700 0000 7232 0000 0072 3900  ...r7...r2...r9.
-00000ee0: 0000 7246 0000 0072 3a00 0000 723b 0000  ..rF...r:...r;..
-00000ef0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000f00: da0f 7465 7374 5f6c 6f61 645f 656d 7074  ..test_load_empt
-00000f10: 7928 0000 0073 1800 0000 0001 0a01 0c01  y(...s..........
-00000f20: 1402 0800 0800 0400 0800 0400 9a00 0c00  ................
-00000f30: 0e00 7a1b 4b56 4669 6c65 5465 7374 732e  ..z.KVFileTests.
-00000f40: 7465 7374 5f6c 6f61 645f 656d 7074 7963  test_load_emptyc
-00000f50: 0100 0000 0000 0000 0900 0000 0900 0000  ................
-00000f60: 4300 0000 7312 0100 007c 006a 0064 0117  C...s....|.j.d..
-00000f70: 007d 0174 017c 0164 0283 028f 107d 027c  .}.t.|.d.....}.|
-00000f80: 02a0 0264 03a1 0101 0057 0064 0051 0052  ...d.....W.d.Q.R
-00000f90: 0058 0074 037c 0183 017d 0374 047c 0383  .X.t.|...}.t.|..
-00000fa0: 017d 0464 047d 057c 047c 056b 027d 067c  .}.d.}.|.|.k.}.|
-00000fb0: 0673 fe74 05a0 0664 057c 0666 0164 067c  .s.t...d.|.f.d.|
-00000fc0: 047c 0566 02a1 0464 0774 07a0 08a1 006b  .|.f...d.t.....k
-00000fd0: 0673 7474 05a0 0974 04a1 0172 7e74 05a0  .stt...t...r~t..
-00000fe0: 0a74 04a1 016e 0264 0764 0874 07a0 08a1  .t...n.d.d.t....
-00000ff0: 006b 0673 9674 05a0 0974 03a1 0172 a074  .k.s.t...t...r.t
-00001000: 05a0 0a74 03a1 016e 0264 0864 0974 07a0  ...t...n.d.d.t..
-00001010: 08a1 006b 0673 b874 05a0 097c 01a1 0172  ...k.s.t...|...r
-00001020: c274 05a0 0a7c 01a1 016e 0264 0974 05a0  .t...|...n.d.t..
-00001030: 0a7c 03a1 0174 05a0 0a7c 04a1 0174 05a0  .|...t...|...t..
-00001040: 0a7c 05a1 0164 0a9c 0616 007d 0764 0b64  .|...d.....}.d.d
-00001050: 0c7c 0769 0116 007d 0874 0b74 05a0 0c7c  .|.i...}.t.t...|
-00001060: 08a1 0183 0182 0164 0004 007d 0304 007d  .......d...}...}
-00001070: 0404 007d 067d 0564 0053 0029 0d4e 7a08  ...}.}.d.S.).Nz.
-00001080: 2f66 6f6f 2e79 6d6c 723d 0000 007a 0220  /foo.ymlr=...z. 
-00001090: 0a72 0100 0000 2901 7216 0000 0029 017a  .r....).r....).z
-000010a0: 4e25 2870 7936 2973 0a7b 2528 7079 3629  N%(py6)s.{%(py6)
-000010b0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
-000010c0: 3429 730a 7b25 2870 7934 2973 203d 2025  4)s.{%(py4)s = %
-000010d0: 2870 7931 2973 2825 2870 7932 2973 290a  (py1)s(%(py2)s).
-000010e0: 7d29 0a7d 203d 3d20 2528 7079 3929 7372  }).} == %(py9)sr
-000010f0: 1700 0000 7204 0000 0072 4400 0000 2906  ....r....rD...).
-00001100: 7219 0000 0072 1a00 0000 7221 0000 0072  r....r....r!...r
-00001110: 2200 0000 721c 0000 0072 2500 0000 7a0f  "...r....r%...z.
-00001120: 6173 7365 7274 2025 2870 7931 3129 7372  assert %(py11)sr
-00001130: 2600 0000 290d 7209 0000 0072 4200 0000  &...).r....rB...
-00001140: 7243 0000 0072 0400 0000 7217 0000 0072  rC...r....r....r
-00001150: 2700 0000 7228 0000 0072 2900 0000 722a  '...r(...r)...r*
-00001160: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
-00001170: 0000 722e 0000 0029 0972 0a00 0000 7244  ..r....).r....rD
-00001180: 0000 0072 4500 0000 7237 0000 0072 3200  ...rE...r7...r2.
-00001190: 0000 7239 0000 0072 4600 0000 723a 0000  ..r9...rF...r:..
-000011a0: 0072 3b00 0000 720c 0000 0072 0c00 0000  .r;...r....r....
-000011b0: 720d 0000 00da 1a74 6573 745f 6c6f 6164  r......test_load
-000011c0: 5f77 6869 7465 7370 6163 655f 656d 7074  _whitespace_empt
-000011d0: 792f 0000 0073 1800 0000 0001 0a01 0c01  y/...s..........
-000011e0: 1402 0800 0800 0400 0800 0400 9a00 0c00  ................
-000011f0: 0e00 7a26 4b56 4669 6c65 5465 7374 732e  ..z&KVFileTests.
-00001200: 7465 7374 5f6c 6f61 645f 7768 6974 6573  test_load_whites
-00001210: 7061 6365 5f65 6d70 7479 6301 0000 0000  pace_emptyc.....
-00001220: 0000 000a 0000 0009 0000 0043 0000 0073  ...........C...s
-00001230: 0c01 0000 7c00 6a00 6401 1700 7d01 7401  ....|.j.d...}.t.
-00001240: 7c01 6402 8302 8f10 7d02 7c02 a002 6403  |.d.....}.|...d.
-00001250: a101 0100 5700 6400 5100 5200 5800 7403  ....W.d.Q.R.X.t.
-00001260: a004 7405 a101 8f0e 7d03 7406 7c01 8301  ..t.....}.t.|...
-00001270: 0100 5700 6400 5100 5200 5800 6404 7d04  ..W.d.Q.R.X.d.}.
-00001280: 7c03 6a07 7d05 7408 7c05 8301 7d06 7c04  |.j.}.t.|...}.|.
-00001290: 7c06 6b06 7d07 7c07 73f8 7409 a00a 6405  |.k.}.|.s.t...d.
-000012a0: 7c07 6601 6406 7c04 7c06 6602 a104 7409  |.f.d.|.|.f...t.
-000012b0: a00b 7c04 a101 6407 740c a00d a100 6b06  ..|...d.t.....k.
-000012c0: 7398 7409 a00e 7408 a101 72a2 7409 a00b  s.t...t...r.t...
-000012d0: 7408 a101 6e02 6407 6408 740c a00d a100  t...n.d.d.t.....
-000012e0: 6b06 73ba 7409 a00e 7c03 a101 72c4 7409  k.s.t...|...r.t.
-000012f0: a00b 7c03 a101 6e02 6408 7409 a00b 7c05  ..|...n.d.t...|.
-00001300: a101 7409 a00b 7c06 a101 6409 9c05 1600  ..t...|...d.....
-00001310: 7d08 640a 640b 7c08 6901 1600 7d09 740f  }.d.d.|.i...}.t.
-00001320: 7409 a010 7c09 a101 8301 8201 6400 0400  t...|.......d...
-00001330: 7d04 0400 7d07 0400 7d05 7d06 6400 5300  }...}...}.}.d.S.
-00001340: 290c 4e7a 082f 666f 6f2e 796d 6c72 3d00  ).Nz./foo.ymlr=.
-00001350: 0000 7a14 5b6e 6f74 2c20 612c 2064 6963  ..z.[not, a, dic
-00001360: 7469 6f6e 6172 795d 7a10 6e6f 7420 6120  tionary]z.not a 
-00001370: 6469 6374 696f 6e61 7279 2901 da02 696e  dictionary)...in
-00001380: 2901 7a4b 2528 7079 3129 7320 696e 2025  ).zK%(py1)s in %
-00001390: 2870 7938 2973 0a7b 2528 7079 3829 7320  (py8)s.{%(py8)s 
-000013a0: 3d20 2528 7079 3329 7328 2528 7079 3629  = %(py3)s(%(py6)
-000013b0: 730a 7b25 2870 7936 2973 203d 2025 2870  s.{%(py6)s = %(p
-000013c0: 7934 2973 2e76 616c 7565 0a7d 290a 7dda  y4)s.value.}).}.
-000013d0: 0373 7472 da07 6578 6369 6e66 6f29 0572  .str..excinfo).r
-000013e0: 1a00 0000 721b 0000 0072 2200 0000 721c  ....r....r"...r.
-000013f0: 0000 0072 1d00 0000 7a0f 6173 7365 7274  ...r....z.assert
-00001400: 2025 2870 7931 3029 73da 0470 7931 3029   %(py10)s..py10)
-00001410: 1172 0900 0000 7242 0000 0072 4300 0000  .r....rB...rC...
-00001420: 7212 0000 0072 1300 0000 da09 5479 7065  r....r......Type
-00001430: 4572 726f 7272 0400 0000 da05 7661 6c75  Errorr......valu
-00001440: 6572 4e00 0000 7227 0000 0072 2800 0000  erN...r'...r(...
-00001450: 722c 0000 0072 2900 0000 722a 0000 0072  r,...r)...r*...r
-00001460: 2b00 0000 722d 0000 0072 2e00 0000 290a  +...r-...r....).
-00001470: 720a 0000 0072 4400 0000 7245 0000 0072  r....rD...rE...r
-00001480: 4f00 0000 da0b 4070 795f 6173 7365 7274  O.....@py_assert
-00001490: 3072 3200 0000 7246 0000 0072 3100 0000  0r2...rF...r1...
-000014a0: 7235 0000 00da 0c40 7079 5f66 6f72 6d61  r5.....@py_forma
-000014b0: 7431 3172 0c00 0000 720c 0000 0072 0d00  t11r....r....r..
-000014c0: 0000 da18 7465 7374 5f6c 6f61 645f 6e6f  ....test_load_no
-000014d0: 6e5f 6469 6374 696f 6e61 7279 3600 0000  n_dictionary6...
-000014e0: 731c 0000 0000 010a 010c 0114 020c 0112  s...............
-000014f0: 0104 0006 0008 0008 0004 0078 000c 000e  ...........x....
-00001500: 007a 244b 5646 696c 6554 6573 7473 2e74  .z$KVFileTests.t
-00001510: 6573 745f 6c6f 6164 5f6e 6f6e 5f64 6963  est_load_non_dic
-00001520: 7469 6f6e 6172 7963 0100 0000 0000 0000  tionaryc........
-00001530: 0e00 0000 0900 0000 4300 0000 7392 0100  ........C...s...
-00001540: 0074 007c 006a 0164 0117 0083 017d 017c  .t.|.j.d.....}.|
-00001550: 01a0 0264 0264 03a1 0201 0074 037c 0183  ...d.d.....t.|..
-00001560: 017d 0264 047d 037c 027c 036b 027d 047c  .}.d.}.|.|.k.}.|
-00001570: 0473 bc74 04a0 0564 057c 0466 0164 067c  .s.t...d.|.f.d.|
-00001580: 027c 0366 02a1 0464 0774 06a0 07a1 006b  .|.f...d.t.....k
-00001590: 0673 5c74 04a0 0874 03a1 0172 6674 04a0  .s\t...t...rft..
-000015a0: 0974 03a1 016e 0264 0764 0874 06a0 07a1  .t...n.d.d.t....
-000015b0: 006b 0673 7e74 04a0 087c 01a1 0172 8874  .k.s~t...|...r.t
-000015c0: 04a0 097c 01a1 016e 0264 0874 04a0 097c  ...|...n.d.t...|
-000015d0: 02a1 0174 04a0 097c 03a1 0164 099c 0416  ...t...|...d....
-000015e0: 007d 0564 0a64 0b7c 0569 0116 007d 0674  .}.d.d.|.i...}.t
-000015f0: 0a74 04a0 0b7c 06a1 0183 0182 0164 0004  .t...|.......d..
-00001600: 007d 0204 007d 047d 037c 016a 0c7d 0764  .}...}.}.|.j.}.d
-00001610: 027d 0864 0c7d 037c 077c 087c 0383 027d  .}.d.}.|.|.|...}
-00001620: 0964 037d 0a7c 097c 0a6b 027d 0b7c 0b90  .d.}.|.|.k.}.|..
-00001630: 0173 7674 04a0 0564 057c 0b66 0164 0d7c  .svt...d.|.f.d.|
-00001640: 097c 0a66 02a1 0464 0874 06a0 07a1 006b  .|.f...d.t.....k
-00001650: 0690 0173 2074 04a0 087c 01a1 0190 0172  ...s t...|.....r
-00001660: 2a74 04a0 097c 01a1 016e 0264 0874 04a0  *t...|...n.d.t..
-00001670: 097c 07a1 0174 04a0 097c 08a1 0174 04a0  .|...t...|...t..
-00001680: 097c 03a1 0174 04a0 097c 09a1 0174 04a0  .|...t...|...t..
-00001690: 097c 0aa1 0164 0e9c 0616 007d 0c64 0f64  .|...d.....}.d.d
-000016a0: 107c 0c69 0116 007d 0d74 0a74 04a0 0b7c  .|.i...}.t.t...|
-000016b0: 0da1 0183 0182 0164 0004 007d 0704 007d  .......d...}...}
-000016c0: 0804 007d 0304 007d 0904 007d 0b7d 0a64  ...}...}...}.}.d
-000016d0: 0053 0029 114e 7a08 2f66 6f6f 2e79 6d6c  .S.).Nz./foo.yml
-000016e0: 721e 0000 0072 4000 0000 723e 0000 0029  r....r@...r>...)
-000016f0: 0172 1600 0000 2901 7a30 2528 7079 3329  .r....).z0%(py3)
-00001700: 730a 7b25 2870 7933 2973 203d 2025 2870  s.{%(py3)s = %(p
-00001710: 7930 2973 2825 2870 7931 2973 290a 7d20  y0)s(%(py1)s).} 
-00001720: 3d3d 2025 2870 7936 2973 7217 0000 0072  == %(py6)sr....r
-00001730: 1800 0000 2904 7219 0000 0072 1a00 0000  ....).r....r....
-00001740: 721b 0000 0072 1c00 0000 7a0e 6173 7365  r....r....z.asse
-00001750: 7274 2025 2870 7938 2973 721d 0000 0072  rt %(py8)sr....r
-00001760: 3f00 0000 2901 7a53 2528 7079 3829 730a  ?...).zS%(py8)s.
-00001770: 7b25 2870 7938 2973 203d 2025 2870 7932  {%(py8)s = %(py2
-00001780: 2973 0a7b 2528 7079 3229 7320 3d20 2528  )s.{%(py2)s = %(
-00001790: 7079 3029 732e 6765 740a 7d28 2528 7079  py0)s.get.}(%(py
-000017a0: 3429 732c 2025 2870 7936 2973 290a 7d20  4)s, %(py6)s).} 
-000017b0: 3d3d 2025 2870 7931 3129 7329 0672 1900  == %(py11)s).r..
-000017c0: 0000 7221 0000 0072 2200 0000 721c 0000  ..r!...r"...r...
-000017d0: 0072 1d00 0000 7226 0000 007a 0f61 7373  .r....r&...z.ass
-000017e0: 6572 7420 2528 7079 3133 2973 7241 0000  ert %(py13)srA..
-000017f0: 0029 0d72 0400 0000 7209 0000 00da 0c73  .).r....r......s
-00001800: 6574 5f61 6e64 5f73 6176 6572 1700 0000  et_and_saver....
-00001810: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
-00001820: 2a00 0000 722b 0000 0072 2c00 0000 722d  *...r+...r,...r-
-00001830: 0000 0072 2e00 0000 7230 0000 0029 0e72  ...r....r0...).r
-00001840: 0a00 0000 7218 0000 0072 3100 0000 7232  ....r....r1...r2
-00001850: 0000 0072 3300 0000 7234 0000 0072 3500  ...r3...r4...r5.
-00001860: 0000 7236 0000 0072 3700 0000 7246 0000  ..r6...r7...rF..
-00001870: 0072 4700 0000 7248 0000 0072 3b00 0000  .rG...rH...r;...
-00001880: 7249 0000 0072 0c00 0000 720c 0000 0072  rI...r....r....r
-00001890: 0d00 0000 da17 7465 7374 5f67 6574 5f61  ......test_get_a
-000018a0: 6674 6572 5f73 6574 5f73 616d 653f 0000  fter_set_same?..
-000018b0: 0073 2a00 0000 0001 0e01 0c02 0800 0400  .s*.............
-000018c0: 0800 0400 7000 0c00 0e00 0c01 0600 0400  ....p...........
-000018d0: 0400 0a00 0400 0800 0600 6a00 0c00 0e00  ..........j.....
-000018e0: 7a23 4b56 4669 6c65 5465 7374 732e 7465  z#KVFileTests.te
-000018f0: 7374 5f67 6574 5f61 6674 6572 5f73 6574  st_get_after_set
-00001900: 5f73 616d 6563 0100 0000 0000 0000 0f00  _samec..........
-00001910: 0000 0900 0000 4300 0000 73a0 0100 0074  ......C...s....t
-00001920: 007c 006a 0164 0117 0083 017d 017c 01a0  .|.j.d.....}.|..
-00001930: 0264 0264 03a1 0201 0074 007c 006a 0164  .d.d.....t.|.j.d
-00001940: 0117 0083 017d 0274 037c 0283 017d 0364  .....}.t.|...}.d
-00001950: 047d 047c 037c 046b 027d 057c 0573 ca74  .}.|.|.k.}.|.s.t
-00001960: 04a0 0564 057c 0566 0164 067c 037c 0466  ...d.|.f.d.|.|.f
-00001970: 02a1 0464 0774 06a0 07a1 006b 0673 6a74  ...d.t.....k.sjt
-00001980: 04a0 0874 03a1 0172 7474 04a0 0974 03a1  ...t...rtt...t..
-00001990: 016e 0264 0764 0874 06a0 07a1 006b 0673  .n.d.d.t.....k.s
-000019a0: 8c74 04a0 087c 02a1 0172 9674 04a0 097c  .t...|...r.t...|
-000019b0: 02a1 016e 0264 0874 04a0 097c 03a1 0174  ...n.d.t...|...t
-000019c0: 04a0 097c 04a1 0164 099c 0416 007d 0664  ...|...d.....}.d
-000019d0: 0a64 0b7c 0669 0116 007d 0774 0a74 04a0  .d.|.i...}.t.t..
-000019e0: 0b7c 07a1 0183 0182 0164 0004 007d 0304  .|.......d...}..
-000019f0: 007d 057d 047c 026a 0c7d 0864 027d 0964  .}.}.|.j.}.d.}.d
-00001a00: 0c7d 047c 087c 097c 0483 027d 0a64 037d  .}.|.|.|...}.d.}
-00001a10: 0b7c 0a7c 0b6b 027d 0c7c 0c90 0173 8474  .|.|.k.}.|...s.t
-00001a20: 04a0 0564 057c 0c66 0164 0d7c 0a7c 0b66  ...d.|.f.d.|.|.f
-00001a30: 02a1 0464 0874 06a0 07a1 006b 0690 0173  ...d.t.....k...s
-00001a40: 2e74 04a0 087c 02a1 0190 0172 3874 04a0  .t...|.....r8t..
-00001a50: 097c 02a1 016e 0264 0874 04a0 097c 08a1  .|...n.d.t...|..
-00001a60: 0174 04a0 097c 09a1 0174 04a0 097c 04a1  .t...|...t...|..
-00001a70: 0174 04a0 097c 0aa1 0174 04a0 097c 0ba1  .t...|...t...|..
-00001a80: 0164 0e9c 0616 007d 0d64 0f64 107c 0d69  .d.....}.d.d.|.i
-00001a90: 0116 007d 0e74 0a74 04a0 0b7c 0ea1 0183  ...}.t.t...|....
-00001aa0: 0182 0164 0004 007d 0804 007d 0904 007d  ...d...}...}...}
-00001ab0: 0404 007d 0a04 007d 0c7d 0b64 0053 0029  ...}...}.}.d.S.)
-00001ac0: 114e 7a08 2f66 6f6f 2e79 6d6c 721e 0000  .Nz./foo.ymlr...
-00001ad0: 0072 4000 0000 723e 0000 0029 0172 1600  .r@...r>...).r..
-00001ae0: 0000 2901 7a30 2528 7079 3329 730a 7b25  ..).z0%(py3)s.{%
-00001af0: 2870 7933 2973 203d 2025 2870 7930 2973  (py3)s = %(py0)s
-00001b00: 2825 2870 7931 2973 290a 7d20 3d3d 2025  (%(py1)s).} == %
-00001b10: 2870 7936 2973 7217 0000 00da 046b 7666  (py6)sr......kvf
-00001b20: 3229 0472 1900 0000 721a 0000 0072 1b00  2).r....r....r..
-00001b30: 0000 721c 0000 007a 0e61 7373 6572 7420  ..r....z.assert 
-00001b40: 2528 7079 3829 7372 1d00 0000 723f 0000  %(py8)sr....r?..
-00001b50: 0029 017a 5325 2870 7938 2973 0a7b 2528  .).zS%(py8)s.{%(
-00001b60: 7079 3829 7320 3d20 2528 7079 3229 730a  py8)s = %(py2)s.
-00001b70: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
-00001b80: 2973 2e67 6574 0a7d 2825 2870 7934 2973  )s.get.}(%(py4)s
-00001b90: 2c20 2528 7079 3629 7329 0a7d 203d 3d20  , %(py6)s).} == 
-00001ba0: 2528 7079 3131 2973 2906 7219 0000 0072  %(py11)s).r....r
-00001bb0: 2100 0000 7222 0000 0072 1c00 0000 721d  !...r"...r....r.
-00001bc0: 0000 0072 2600 0000 7a0f 6173 7365 7274  ...r&...z.assert
-00001bd0: 2025 2870 7931 3329 7372 4100 0000 290d   %(py13)srA...).
-00001be0: 7204 0000 0072 0900 0000 7256 0000 0072  r....r....rV...r
-00001bf0: 1700 0000 7227 0000 0072 2800 0000 7229  ....r'...r(...r)
-00001c00: 0000 0072 2a00 0000 722b 0000 0072 2c00  ...r*...r+...r,.
-00001c10: 0000 722d 0000 0072 2e00 0000 7230 0000  ..r-...r....r0..
-00001c20: 0029 0f72 0a00 0000 7218 0000 0072 5800  .).r....r....rX.
-00001c30: 0000 7231 0000 0072 3200 0000 7233 0000  ..r1...r2...r3..
-00001c40: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
-00001c50: 7237 0000 0072 4600 0000 7247 0000 0072  r7...rF...rG...r
-00001c60: 4800 0000 723b 0000 0072 4900 0000 720c  H...r;...rI...r.
-00001c70: 0000 0072 0c00 0000 720d 0000 00da 1574  ...r....r......t
-00001c80: 6573 745f 6c6f 6164 5f73 6563 6f6e 645f  est_load_second_
-00001c90: 7361 6d65 4600 0000 732c 0000 0000 010e  sameF...s,......
-00001ca0: 010c 010e 0208 0004 0008 0004 0070 000c  .............p..
-00001cb0: 000e 000c 0106 0004 0004 000a 0004 0008  ................
-00001cc0: 0006 006a 000c 000e 007a 214b 5646 696c  ...j.....z!KVFil
-00001cd0: 6554 6573 7473 2e74 6573 745f 6c6f 6164  eTests.test_load
-00001ce0: 5f73 6563 6f6e 645f 7361 6d65 6301 0000  _second_samec...
-00001cf0: 0000 0000 000e 0000 0009 0000 0043 0000  .............C..
-00001d00: 0073 9001 0000 7c00 6a00 6401 1700 7d01  .s....|.j.d...}.
-00001d10: 7401 7c01 8301 7d02 7c02 a002 6402 6403  t.|...}.|...d.d.
-00001d20: a102 0100 7c02 a002 6404 6403 a102 0100  ....|...d.d.....
-00001d30: 7403 7c01 8301 8f22 7d03 7c03 a004 a100  t.|...."}.|.....
-00001d40: 7d04 7c03 a005 6405 a101 0100 7406 a007  }.|...d.....t...
-00001d50: 7c03 a101 7d05 5700 6400 5100 5200 5800  |...}.W.d.Q.R.X.
-00001d60: 7408 7c04 8301 7d06 6406 7d07 7c06 7c07  t.|...}.d.}.|.|.
-00001d70: 6b02 7d08 7c08 73fc 7409 a00a 6407 7c08  k.}.|.s.t...d.|.
-00001d80: 6601 6408 7c06 7c07 6602 a104 6409 740b  f.d.|.|.f...d.t.
-00001d90: a00c a100 6b06 739c 7409 a00d 7408 a101  ....k.s.t...t...
-00001da0: 72a6 7409 a00e 7408 a101 6e02 6409 640a  r.t...t...n.d.d.
-00001db0: 740b a00c a100 6b06 73be 7409 a00d 7c04  t.....k.s.t...|.
-00001dc0: a101 72c8 7409 a00e 7c04 a101 6e02 640a  ..r.t...|...n.d.
-00001dd0: 7409 a00e 7c06 a101 7409 a00e 7c07 a101  t...|...t...|...
-00001de0: 640b 9c04 1600 7d09 640c 640d 7c09 6901  d.....}.d.d.|.i.
-00001df0: 1600 7d0a 740f 7409 a010 7c0a a101 8301  ..}.t.t...|.....
-00001e00: 8201 6400 0400 7d06 0400 7d08 7d07 6403  ..d...}...}.}.d.
-00001e10: 6403 640e 9c02 7d06 7c05 7c06 6b02 7d0b  d.d...}.|.|.k.}.
-00001e20: 7c0b 9001 7384 7409 a00a 6407 7c0b 6601  |...s.t...d.|.f.
-00001e30: 640f 7c05 7c06 6602 a104 6410 740b a00c  d.|.|.f...d.t...
-00001e40: a100 6b06 9001 734e 7409 a00d 7c05 a101  ..k...sNt...|...
-00001e50: 9001 7258 7409 a00e 7c05 a101 6e02 6410  ..rXt...|...n.d.
-00001e60: 7409 a00e 7c06 a101 6411 9c02 1600 7d0c  t...|...d.....}.
-00001e70: 6412 6413 7c0c 6901 1600 7d0d 740f 7409  d.d.|.i...}.t.t.
-00001e80: a010 7c0d a101 8301 8201 6400 0400 7d0b  ..|.......d...}.
-00001e90: 7d06 6400 5300 2914 4e7a 082f 666f 6f2e  }.d.S.).Nz./foo.
-00001ea0: 796d 6c72 1e00 0000 7240 0000 00da 0466  ymlr....r@.....f
-00001eb0: 6f6f 3272 0100 0000 e902 0000 0029 0172  oo2r.........).r
-00001ec0: 1600 0000 2901 7a30 2528 7079 3329 730a  ....).z0%(py3)s.
-00001ed0: 7b25 2870 7933 2973 203d 2025 2870 7930  {%(py3)s = %(py0
-00001ee0: 2973 2825 2870 7931 2973 290a 7d20 3d3d  )s(%(py1)s).} ==
-00001ef0: 2025 2870 7936 2973 7217 0000 00da 056c   %(py6)sr......l
-00001f00: 696e 6573 2904 7219 0000 0072 1a00 0000  ines).r....r....
-00001f10: 721b 0000 0072 1c00 0000 7a0e 6173 7365  r....r....z.asse
-00001f20: 7274 2025 2870 7938 2973 721d 0000 0029  rt %(py8)sr....)
-00001f30: 0272 1e00 0000 725a 0000 0029 017a 1225  .r....rZ...).z.%
-00001f40: 2870 7930 2973 203d 3d20 2528 7079 3329  (py0)s == %(py3)
-00001f50: 73da 0464 6174 6129 0272 1900 0000 721b  s..data).r....r.
-00001f60: 0000 007a 0e61 7373 6572 7420 2528 7079  ...z.assert %(py
-00001f70: 3529 7372 2300 0000 2911 7209 0000 0072  5)sr#...).r....r
-00001f80: 0400 0000 7256 0000 0072 4200 0000 da09  ....rV...rB.....
-00001f90: 7265 6164 6c69 6e65 73da 0473 6565 6bda  readlines..seek.
-00001fa0: 0479 616d 6cda 0973 6166 655f 6c6f 6164  .yaml..safe_load
-00001fb0: 7217 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
-00001fc0: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
-00001fd0: 0000 0072 2d00 0000 722e 0000 0029 0e72  ...r-...r....).r
-00001fe0: 0a00 0000 7244 0000 0072 1800 0000 7245  ....rD...r....rE
-00001ff0: 0000 0072 5c00 0000 725d 0000 0072 3100  ...r\...r]...r1.
-00002000: 0000 7232 0000 0072 3300 0000 7234 0000  ..r2...r3...r4..
-00002010: 0072 3500 0000 7236 0000 00da 0b40 7079  .r5...r6.....@py
-00002020: 5f66 6f72 6d61 7434 da0b 4070 795f 666f  _format4..@py_fo
-00002030: 726d 6174 3672 0c00 0000 720c 0000 0072  rmat6r....r....r
-00002040: 0d00 0000 da27 7465 7374 5f73 6574 735f  .....'test_sets_
-00002050: 646f 6e74 5f63 6175 7365 5f61 7070 656e  dont_cause_appen
-00002060: 645f 6475 706c 6963 6174 696f 6e4e 0000  d_duplicationN..
-00002070: 0073 2e00 0000 0001 0a01 0801 0c01 0c02  .s..............
-00002080: 0a01 0801 0a01 1402 0800 0400 0800 0400  ................
-00002090: 7000 0c00 0e00 0c01 0a00 0800 0600 4a00  p.............J.
-000020a0: 0c00 0e00 7a33 4b56 4669 6c65 5465 7374  ....z3KVFileTest
-000020b0: 732e 7465 7374 5f73 6574 735f 646f 6e74  s.test_sets_dont
-000020c0: 5f63 6175 7365 5f61 7070 656e 645f 6475  _cause_append_du
-000020d0: 706c 6963 6174 696f 6e29 0fda 085f 5f6e  plication)...__n
-000020e0: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000020f0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00002100: 0700 0000 7210 0000 0072 1500 0000 723c  ....r....r....r<
-00002110: 0000 0072 4a00 0000 724b 0000 0072 4c00  ...rJ...rK...rL.
-00002120: 0000 7255 0000 0072 5700 0000 7259 0000  ..rU...rW...rY..
-00002130: 0072 6400 0000 da0d 5f5f 636c 6173 7363  .rd.....__classc
-00002140: 656c 6c5f 5f72 0c00 0000 720c 0000 0029  ell__r....r....)
-00002150: 0172 0b00 0000 720d 0000 0072 0500 0000  .r....r....r....
-00002160: 0b00 0000 7316 0000 0008 010c 050c 0408  ....s...........
-00002170: 0408 0608 0908 0708 0708 0908 0708 0872  ...............r
-00002180: 0500 0000 2910 da08 6275 696c 7469 6e73  ....)...builtins
-00002190: 7229 0000 00da 195f 7079 7465 7374 2e61  r)....._pytest.a
-000021a0: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
-000021b0: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
-000021c0: 7269 7465 7227 0000 0072 0e00 0000 da08  riter'...r......
-000021d0: 7465 6d70 6669 6c65 7202 0000 0072 1200  tempfiler....r..
-000021e0: 0000 7260 0000 00da 0b64 6a61 6e67 6f2e  ..r`.....django.
-000021f0: 7465 7374 7203 0000 00da 1464 6a61 6e67  testr......djang
-00002200: 6f5f 7065 7266 5f72 6563 2e79 616d 6c72  o_perf_rec.yamlr
-00002210: 0400 0000 7205 0000 0072 0c00 0000 720c  ....r....r....r.
-00002220: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
-00002230: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
-00002240: 0800 1200 0801 0c02 0801 0801 0c02 0c03  ................
+00000000: 610d 0d0a 4f4b ee5e ef09 0000 e300 0000  a...OK.^........
+00000010: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00000020: 0040 0000 0073 6a00 0000 6400 6401 6c00  .@...sj...d.d.l.
+00000030: 5a01 6400 6401 6c02 6d03 0200 0100 6d04  Z.d.d.l.m.....m.
+00000040: 5a05 0100 6400 6401 6c06 5a06 6400 6402  Z...d.d.l.Z.d.d.
+00000050: 6c07 6d08 5a08 0100 6400 6401 6c09 5a09  l.m.Z...d.d.l.Z.
+00000060: 6400 6401 6c0a 5a0a 6400 6403 6c0b 6d0c  d.d.l.Z.d.d.l.m.
+00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 0100  Z...d.d.l.m.Z...
+00000080: 4700 6405 6406 8400 6406 650c 8303 5a0f  G.d.d...d.e...Z.
+00000090: 6401 5300 2907 e900 0000 004e 2901 da07  d.S.)......N)...
+000000a0: 6d6b 6474 656d 7029 01da 0e53 696d 706c  mkdtemp)...Simpl
+000000b0: 6554 6573 7443 6173 6529 01da 064b 5646  eTestCase)...KVF
+000000c0: 696c 6563 0000 0000 0000 0000 0000 0000  ilec............
+000000d0: 0000 0000 0300 0000 0000 0000 7370 0000  ............sp..
+000000e0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+000000f0: 0284 085a 0387 0066 0164 0364 0484 085a  ...Z...f.d.d...Z
+00000100: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
+00000110: 0664 0964 0a84 005a 0764 0b64 0c84 005a  .d.d...Z.d.d...Z
+00000120: 0864 0d64 0e84 005a 0964 0f64 1084 005a  .d.d...Z.d.d...Z
+00000130: 0a64 1164 1284 005a 0b64 1364 1484 005a  .d.d...Z.d.d...Z
+00000140: 0c64 1564 1684 005a 0d87 0004 005a 0e53  .d.d...Z.....Z.S
+00000150: 0029 17da 0b4b 5646 696c 6554 6573 7473  .)...KVFileTests
+00000160: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000170: 0002 0000 0003 0000 0073 1e00 0000 7400  .........s....t.
+00000180: 8300 a001 a100 0100 7402 a003 a100 0100  ........t.......
+00000190: 7404 8300 7c00 5f05 6400 5300 a901 4e29  t...|._.d.S...N)
+000001a0: 06da 0573 7570 6572 da05 7365 7455 7072  ...super..setUpr
+000001b0: 0400 0000 da11 5f63 6c65 6172 5f6c 6f61  ......_clear_loa
+000001c0: 645f 6361 6368 6572 0200 0000 da08 7465  d_cacher......te
+000001d0: 6d70 5f64 6972 a901 da04 7365 6c66 a901  mp_dir....self..
+000001e0: da09 5f5f 636c 6173 735f 5fa9 00fa 432f  ..__class__...C/
+000001f0: 5573 6572 732f 6368 6169 6e7a 2f44 6f63  Users/chainz/Doc
+00000200: 756d 656e 7473 2f50 726f 6a65 6374 732f  uments/Projects/
+00000210: 646a 616e 676f 2d70 6572 662d 7265 632f  django-perf-rec/
+00000220: 7465 7374 732f 7465 7374 5f79 616d 6c2e  tests/test_yaml.
+00000230: 7079 7208 0000 000c 0000 0073 0600 0000  pyr........s....
+00000240: 0001 0a01 0801 7a11 4b56 4669 6c65 5465  ......z.KVFileTe
+00000250: 7374 732e 7365 7455 7063 0100 0000 0000  sts.setUpc......
+00000260: 0000 0000 0000 0100 0000 0300 0000 0300  ................
+00000270: 0000 731a 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
+00000280: 0101 0074 0383 00a0 04a1 0001 0064 0053  ...t.........d.S
+00000290: 0072 0600 0000 2905 da06 7368 7574 696c  .r....)...shutil
+000002a0: da06 726d 7472 6565 720a 0000 0072 0700  ..rmtreer....r..
+000002b0: 0000 da08 7465 6172 446f 776e 720b 0000  ....tearDownr...
+000002c0: 0072 0d00 0000 720f 0000 0072 1000 0000  .r....r....r....
+000002d0: 7213 0000 0011 0000 0073 0400 0000 0001  r........s......
+000002e0: 0c01 7a14 4b56 4669 6c65 5465 7374 732e  ..z.KVFileTests.
+000002f0: 7465 6172 446f 776e 6301 0000 0000 0000  tearDownc.......
+00000300: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
+00000310: 0073 3600 0000 7400 a001 7402 a101 8f18  .s6...t...t.....
+00000320: 0100 7403 6401 8301 0100 5700 6400 0400  ..t.d.....W.d...
+00000330: 0400 8303 0100 6e10 3100 7328 3000 0100  ......n.1.s(0...
+00000340: 0100 0100 5900 0100 6400 5300 2902 4efa  ....Y...d.S.).N.
+00000350: 012f 2904 da06 7079 7465 7374 da06 7261  ./)...pytest..ra
+00000360: 6973 6573 da07 494f 4572 726f 7272 0400  ises..IOErrorr..
+00000370: 0000 720b 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00000380: 0072 1000 0000 da18 7465 7374 5f6c 6f61  .r......test_loa
+00000390: 645f 6e6f 5f70 6572 6d69 7373 696f 6e73  d_no_permissions
+000003a0: 1500 0000 7304 0000 0000 010c 017a 244b  ....s........z$K
+000003b0: 5646 696c 6554 6573 7473 2e74 6573 745f  VFileTests.test_
+000003c0: 6c6f 6164 5f6e 6f5f 7065 726d 6973 7369  load_no_permissi
+000003d0: 6f6e 7363 0100 0000 0000 0000 0000 0000  onsc............
+000003e0: 0e00 0000 0900 0000 4300 0000 73b8 0100  ........C...s...
+000003f0: 0074 007c 006a 0164 0117 0083 017d 0174  .t.|.j.d.....}.t
+00000400: 027c 0183 017d 0264 027d 037c 027c 036b  .|...}.d.}.|.|.k
+00000410: 027d 047c 0473 b074 03a0 0464 037c 0466  .}.|.s.t...d.|.f
+00000420: 0164 047c 027c 0366 02a1 0464 0574 05a0  .d.|.|.f...d.t..
+00000430: 06a1 0076 0073 5074 03a0 0774 02a1 0172  ...v.sPt...t...r
+00000440: 5a74 03a0 0874 02a1 016e 0264 0564 0674  Zt...t...n.d.d.t
+00000450: 05a0 06a1 0076 0073 7274 03a0 077c 01a1  .....v.srt...|..
+00000460: 0172 7c74 03a0 087c 01a1 016e 0264 0674  .r|t...|...n.d.t
+00000470: 03a0 087c 02a1 0174 03a0 087c 03a1 0164  ...|...t...|...d
+00000480: 079c 0416 007d 0564 0864 097c 0569 0116  .....}.d.d.|.i..
+00000490: 007d 0674 0974 03a0 0a7c 06a1 0183 0182  .}.t.t...|......
+000004a0: 0164 0004 007d 0204 007d 047d 0374 0b83  .d...}...}.}.t..
+000004b0: 007d 077c 016a 0c7d 0864 0a7d 097c 087c  .}.|.j.}.d.}.|.|
+000004c0: 097c 0783 027d 0a7c 0a7c 0775 007d 0b7c  .|...}.|.|.u.}.|
+000004d0: 0b90 0173 a474 03a0 0464 0b7c 0b66 0164  ...s.t...d.|.f.d
+000004e0: 0c7c 0a7c 0766 02a1 0464 0674 05a0 06a1  .|.|.f...d.t....
+000004f0: 0076 0090 0173 1274 03a0 077c 01a1 0190  .v...s.t...|....
+00000500: 0172 1c74 03a0 087c 01a1 016e 0264 0674  .r.t...|...n.d.t
+00000510: 03a0 087c 08a1 0174 03a0 087c 09a1 0164  ...|...t...|...d
+00000520: 0d74 05a0 06a1 0076 0090 0173 4874 03a0  .t.....v...sHt..
+00000530: 077c 07a1 0190 0172 5274 03a0 087c 07a1  .|.....rRt...|..
+00000540: 016e 0264 0d74 03a0 087c 0aa1 0164 0d74  .n.d.t...|...d.t
+00000550: 05a0 06a1 0076 0090 0173 7674 03a0 077c  .....v...svt...|
+00000560: 07a1 0190 0172 8074 03a0 087c 07a1 016e  .....r.t...|...n
+00000570: 0264 0d64 0e9c 0616 007d 0c64 0f64 107c  .d.d.....}.d.d.|
+00000580: 0c69 0116 007d 0d74 0974 03a0 0a7c 0da1  .i...}.t.t...|..
+00000590: 0183 0182 0164 0004 007d 0804 007d 0904  .....d...}...}..
+000005a0: 007d 0a7d 0b64 0053 0029 114e fa08 2f66  .}.}.d.S.).N../f
+000005b0: 6f6f 2e79 6d6c 7201 0000 00a9 01fa 023d  oo.ymlr........=
+000005c0: 3da9 017a 3025 2870 7933 2973 0a7b 2528  =..z0%(py3)s.{%(
+000005d0: 7079 3329 7320 3d20 2528 7079 3029 7328  py3)s = %(py0)s(
+000005e0: 2528 7079 3129 7329 0a7d 203d 3d20 2528  %(py1)s).} == %(
+000005f0: 7079 3629 73da 036c 656e da03 6b76 66a9  py6)s..len..kvf.
+00000600: 04da 0370 7930 da03 7079 31da 0370 7933  ...py0..py1..py3
+00000610: da03 7079 36fa 0e61 7373 6572 7420 2528  ..py6..assert %(
+00000620: 7079 3829 73da 0370 7938 da03 666f 6f29  py8)s..py8..foo)
+00000630: 01da 0269 7329 017a 5225 2870 7937 2973  ...is).zR%(py7)s
+00000640: 0a7b 2528 7079 3729 7320 3d20 2528 7079  .{%(py7)s = %(py
+00000650: 3229 730a 7b25 2870 7932 2973 203d 2025  2)s.{%(py2)s = %
+00000660: 2870 7930 2973 2e67 6574 0a7d 2825 2870  (py0)s.get.}(%(p
+00000670: 7934 2973 2c20 2528 7079 3529 7329 0a7d  y4)s, %(py5)s).}
+00000680: 2069 7320 2528 7079 3929 73da 0764 6566   is %(py9)s..def
+00000690: 6175 6c74 2906 7220 0000 00da 0370 7932  ault).r .....py2
+000006a0: da03 7079 34da 0370 7935 da03 7079 37da  ..py4..py5..py7.
+000006b0: 0370 7939 fa0f 6173 7365 7274 2025 2870  .py9..assert %(p
+000006c0: 7931 3129 73da 0470 7931 3129 0d72 0400  y11)s..py11).r..
+000006d0: 0000 720a 0000 0072 1d00 0000 da0a 4070  ..r....r......@p
+000006e0: 7974 6573 745f 6172 da11 5f63 616c 6c5f  ytest_ar.._call_
+000006f0: 7265 7072 636f 6d70 6172 65da 0c40 7079  reprcompare..@py
+00000700: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
+00000710: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
+00000720: 676c 6f62 616c 5f6e 616d 65da 095f 7361  global_name.._sa
+00000730: 6665 7265 7072 da0e 4173 7365 7274 696f  ferepr..Assertio
+00000740: 6e45 7272 6f72 da13 5f66 6f72 6d61 745f  nError.._format_
+00000750: 6578 706c 616e 6174 696f 6eda 066f 626a  explanation..obj
+00000760: 6563 74da 0367 6574 290e 720c 0000 0072  ect..get).r....r
+00000770: 1e00 0000 da0b 4070 795f 6173 7365 7274  ......@py_assert
+00000780: 32da 0b40 7079 5f61 7373 6572 7435 da0b  2..@py_assert5..
+00000790: 4070 795f 6173 7365 7274 34da 0b40 7079  @py_assert4..@py
+000007a0: 5f66 6f72 6d61 7437 da0b 4070 795f 666f  _format7..@py_fo
+000007b0: 726d 6174 3972 2800 0000 da0b 4070 795f  rmat9r(.....@py_
+000007c0: 6173 7365 7274 31da 0b40 7079 5f61 7373  assert1..@py_ass
+000007d0: 6572 7433 da0b 4070 795f 6173 7365 7274  ert3..@py_assert
+000007e0: 36da 0b40 7079 5f61 7373 6572 7438 da0c  6..@py_assert8..
+000007f0: 4070 795f 666f 726d 6174 3130 da0c 4070  @py_format10..@p
+00000800: 795f 666f 726d 6174 3132 720f 0000 0072  y_format12r....r
+00000810: 0f00 0000 7210 0000 00da 1f74 6573 745f  ....r......test_
+00000820: 6c6f 6164 5f6e 6f6e 5f65 7869 7374 656e  load_non_existen
+00000830: 745f 6973 5f65 6d70 7479 1900 0000 7308  t_is_empty....s.
+00000840: 0000 0000 010e 01ae 0106 017a 2b4b 5646  ...........z+KVF
+00000850: 696c 6554 6573 7473 2e74 6573 745f 6c6f  ileTests.test_lo
+00000860: 6164 5f6e 6f6e 5f65 7869 7374 656e 745f  ad_non_existent_
+00000870: 6973 5f65 6d70 7479 6301 0000 0000 0000  is_emptyc.......
+00000880: 0000 0000 0010 0000 0009 0000 0043 0000  .............C..
+00000890: 0073 be01 0000 7c00 6a00 6401 1700 7d01  .s....|.j.d...}.
+000008a0: 7401 7c01 6402 8302 8f1a 7d02 7c02 a002  t.|.d.....}.|...
+000008b0: 6403 a101 0100 5700 6400 0400 0400 8303  d.....W.d.......
+000008c0: 0100 6e10 3100 7334 3000 0100 0100 0100  ..n.1.s40.......
+000008d0: 5900 0100 7403 7c01 8301 7d03 7404 7c03  Y...t.|...}.t.|.
+000008e0: 8301 7d04 6404 7d05 7c04 7c05 6b02 7d06  ..}.d.}.|.|.k.}.
+000008f0: 7c06 73e8 7405 a006 6405 7c06 6601 6406  |.s.t...d.|.f.d.
+00000900: 7c04 7c05 6602 a104 6407 7407 a008 a100  |.|.f...d.t.....
+00000910: 7600 7388 7405 a009 7404 a101 7292 7405  v.s.t...t...r.t.
+00000920: a00a 7404 a101 6e02 6407 6408 7407 a008  ..t...n.d.d.t...
+00000930: a100 7600 73aa 7405 a009 7c03 a101 72b4  ..v.s.t...|...r.
+00000940: 7405 a00a 7c03 a101 6e02 6408 7405 a00a  t...|...n.d.t...
+00000950: 7c04 a101 7405 a00a 7c05 a101 6409 9c04  |...t...|...d...
+00000960: 1600 7d07 640a 640b 7c07 6901 1600 7d08  ..}.d.d.|.i...}.
+00000970: 740b 7405 a00c 7c08 a101 8301 8201 6400  t.t...|.......d.
+00000980: 0400 7d04 0400 7d06 7d05 7c03 6a0d 7d09  ..}...}.}.|.j.}.
+00000990: 640c 7d0a 640d 7d05 7c09 7c0a 7c05 8302  d.}.d.}.|.|.|...
+000009a0: 7d0b 640e 7d0c 7c0b 7c0c 6b02 7d0d 7c0d  }.d.}.|.|.k.}.|.
+000009b0: 9001 73a2 7405 a006 6405 7c0d 6601 640f  ..s.t...d.|.f.d.
+000009c0: 7c0b 7c0c 6602 a104 6408 7407 a008 a100  |.|.f...d.t.....
+000009d0: 7600 9001 734c 7405 a009 7c03 a101 9001  v...sLt...|.....
+000009e0: 7256 7405 a00a 7c03 a101 6e02 6408 7405  rVt...|...n.d.t.
+000009f0: a00a 7c09 a101 7405 a00a 7c0a a101 7405  ..|...t...|...t.
+00000a00: a00a 7c05 a101 7405 a00a 7c0b a101 7405  ..|...t...|...t.
+00000a10: a00a 7c0c a101 6410 9c06 1600 7d0e 6411  ..|...d.....}.d.
+00000a20: 6412 7c0e 6901 1600 7d0f 740b 7405 a00c  d.|.i...}.t.t...
+00000a30: 7c0f a101 8301 8201 6400 0400 7d09 0400  |.......d...}...
+00000a40: 7d0a 0400 7d05 0400 7d0b 0400 7d0d 7d0c  }...}...}...}.}.
+00000a50: 6400 5300 2913 4e72 1900 0000 da01 777a  d.S.).Nr......wz
+00000a60: 0866 6f6f 3a20 6261 72e9 0100 0000 721a  .foo: bar.....r.
+00000a70: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00000a80: 0000 721f 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
+00000a90: 0072 2600 0000 da00 da03 6261 72a9 017a  .r&.......bar..z
+00000aa0: 5325 2870 7938 2973 0a7b 2528 7079 3829  S%(py8)s.{%(py8)
+00000ab0: 7320 3d20 2528 7079 3229 730a 7b25 2870  s = %(py2)s.{%(p
+00000ac0: 7932 2973 203d 2025 2870 7930 2973 2e67  y2)s = %(py0)s.g
+00000ad0: 6574 0a7d 2825 2870 7934 2973 2c20 2528  et.}(%(py4)s, %(
+00000ae0: 7079 3629 7329 0a7d 203d 3d20 2528 7079  py6)s).} == %(py
+00000af0: 3131 2973 a906 7220 0000 0072 2900 0000  11)s..r ...r)...
+00000b00: 722a 0000 0072 2300 0000 7225 0000 0072  r*...r#...r%...r
+00000b10: 2f00 0000 fa0f 6173 7365 7274 2025 2870  /.....assert %(p
+00000b20: 7931 3329 73da 0470 7931 3329 0e72 0a00  y13)s..py13).r..
+00000b30: 0000 da04 6f70 656e da05 7772 6974 6572  ....open..writer
+00000b40: 0400 0000 721d 0000 0072 3000 0000 7231  ....r....r0...r1
+00000b50: 0000 0072 3200 0000 7233 0000 0072 3400  ...r2...r3...r4.
+00000b60: 0000 7235 0000 0072 3600 0000 7237 0000  ..r5...r6...r7..
+00000b70: 0072 3900 0000 2910 720c 0000 00da 0966  .r9...).r......f
+00000b80: 696c 655f 6e61 6d65 da02 6670 721e 0000  ile_name..fpr...
+00000b90: 0072 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
+00000ba0: 723d 0000 0072 3e00 0000 723f 0000 0072  r=...r>...r?...r
+00000bb0: 4000 0000 da0b 4070 795f 6173 7365 7274  @.....@py_assert
+00000bc0: 37da 0c40 7079 5f61 7373 6572 7431 30da  7..@py_assert10.
+00000bd0: 0b40 7079 5f61 7373 6572 7439 7244 0000  .@py_assert9rD..
+00000be0: 00da 0c40 7079 5f66 6f72 6d61 7431 3472  ...@py_format14r
+00000bf0: 0f00 0000 720f 0000 0072 1000 0000 da12  ....r....r......
+00000c00: 7465 7374 5f6c 6f61 645f 6578 6973 7465  test_load_existe
+00000c10: 6e74 1f00 0000 730c 0000 0000 010a 010c  nt....s.........
+00000c20: 0128 0208 01ae 017a 1e4b 5646 696c 6554  .(.....z.KVFileT
+00000c30: 6573 7473 2e74 6573 745f 6c6f 6164 5f65  ests.test_load_e
+00000c40: 7869 7374 656e 7463 0100 0000 0000 0000  xistentc........
+00000c50: 0000 0000 0900 0000 0900 0000 4300 0000  ............C...
+00000c60: 7328 0100 007c 006a 0064 0117 007d 0174  s(...|.j.d...}.t
+00000c70: 017c 0164 0283 028f 1a7d 027c 02a0 0264  .|.d.....}.|...d
+00000c80: 03a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+00000c90: 006e 1031 0073 3430 0001 0001 0001 0059  .n.1.s40.......Y
+00000ca0: 0001 0074 037c 0183 017d 0374 047c 0383  ...t.|...}.t.|..
+00000cb0: 017d 0464 047d 057c 047c 056b 027d 067c  .}.d.}.|.|.k.}.|
+00000cc0: 0690 0173 1474 05a0 0664 057c 0666 0164  ...s.t...d.|.f.d
+00000cd0: 067c 047c 0566 02a1 0464 0774 07a0 08a1  .|.|.f...d.t....
+00000ce0: 0076 0073 8a74 05a0 0974 04a1 0172 9474  .v.s.t...t...r.t
+00000cf0: 05a0 0a74 04a1 016e 0264 0764 0874 07a0  ...t...n.d.d.t..
+00000d00: 08a1 0076 0073 ac74 05a0 0974 03a1 0172  ...v.s.t...t...r
+00000d10: b674 05a0 0a74 03a1 016e 0264 0864 0974  .t...t...n.d.d.t
+00000d20: 07a0 08a1 0076 0073 ce74 05a0 097c 01a1  .....v.s.t...|..
+00000d30: 0172 d874 05a0 0a7c 01a1 016e 0264 0974  .r.t...|...n.d.t
+00000d40: 05a0 0a7c 03a1 0174 05a0 0a7c 04a1 0174  ...|...t...|...t
+00000d50: 05a0 0a7c 05a1 0164 0a9c 0616 007d 0764  ...|...d.....}.d
+00000d60: 0b64 0c7c 0769 0116 007d 0874 0b74 05a0  .d.|.i...}.t.t..
+00000d70: 0c7c 08a1 0183 0182 0164 0004 007d 0304  .|.......d...}..
+00000d80: 007d 0404 007d 067d 0564 0053 0029 0d4e  .}...}.}.d.S.).N
+00000d90: 7219 0000 0072 4600 0000 7248 0000 0072  r....rF...rH...r
+00000da0: 0100 0000 721a 0000 00a9 017a 4e25 2870  ....r......zN%(p
+00000db0: 7936 2973 0a7b 2528 7079 3629 7320 3d20  y6)s.{%(py6)s = 
+00000dc0: 2528 7079 3029 7328 2528 7079 3429 730a  %(py0)s(%(py4)s.
+00000dd0: 7b25 2870 7934 2973 203d 2025 2870 7931  {%(py4)s = %(py1
+00000de0: 2973 2825 2870 7932 2973 290a 7d29 0a7d  )s(%(py2)s).}).}
+00000df0: 203d 3d20 2528 7079 3929 7372 1d00 0000   == %(py9)sr....
+00000e00: 7204 0000 0072 5000 0000 a906 7220 0000  r....rP.....r ..
+00000e10: 0072 2100 0000 7229 0000 0072 2a00 0000  .r!...r)...r*...
+00000e20: 7223 0000 0072 2d00 0000 722e 0000 0072  r#...r-...r....r
+00000e30: 2f00 0000 a90d 720a 0000 0072 4e00 0000  /.....r....rN...
+00000e40: 724f 0000 0072 0400 0000 721d 0000 0072  rO...r....r....r
+00000e50: 3000 0000 7231 0000 0072 3200 0000 7233  0...r1...r2...r3
+00000e60: 0000 0072 3400 0000 7235 0000 0072 3600  ...r4...r5...r6.
+00000e70: 0000 7237 0000 00a9 0972 0c00 0000 7250  ..r7.....r....rP
+00000e80: 0000 0072 5100 0000 7240 0000 0072 3b00  ...rQ...r@...r;.
+00000e90: 0000 7242 0000 0072 5200 0000 7243 0000  ..rB...rR...rC..
+00000ea0: 0072 4400 0000 720f 0000 0072 0f00 0000  .rD...r....r....
+00000eb0: 7210 0000 00da 0f74 6573 745f 6c6f 6164  r......test_load
+00000ec0: 5f65 6d70 7479 2800 0000 7308 0000 0000  _empty(...s.....
+00000ed0: 010a 010c 0128 027a 1b4b 5646 696c 6554  .....(.z.KVFileT
+00000ee0: 6573 7473 2e74 6573 745f 6c6f 6164 5f65  ests.test_load_e
+00000ef0: 6d70 7479 6301 0000 0000 0000 0000 0000  mptyc...........
+00000f00: 0009 0000 0009 0000 0043 0000 0073 2801  .........C...s(.
+00000f10: 0000 7c00 6a00 6401 1700 7d01 7401 7c01  ..|.j.d...}.t.|.
+00000f20: 6402 8302 8f1a 7d02 7c02 a002 6403 a101  d.....}.|...d...
+00000f30: 0100 5700 6400 0400 0400 8303 0100 6e10  ..W.d.........n.
+00000f40: 3100 7334 3000 0100 0100 0100 5900 0100  1.s40.......Y...
+00000f50: 7403 7c01 8301 7d03 7404 7c03 8301 7d04  t.|...}.t.|...}.
+00000f60: 6404 7d05 7c04 7c05 6b02 7d06 7c06 9001  d.}.|.|.k.}.|...
+00000f70: 7314 7405 a006 6405 7c06 6601 6406 7c04  s.t...d.|.f.d.|.
+00000f80: 7c05 6602 a104 6407 7407 a008 a100 7600  |.f...d.t.....v.
+00000f90: 738a 7405 a009 7404 a101 7294 7405 a00a  s.t...t...r.t...
+00000fa0: 7404 a101 6e02 6407 6408 7407 a008 a100  t...n.d.d.t.....
+00000fb0: 7600 73ac 7405 a009 7403 a101 72b6 7405  v.s.t...t...r.t.
+00000fc0: a00a 7403 a101 6e02 6408 6409 7407 a008  ..t...n.d.d.t...
+00000fd0: a100 7600 73ce 7405 a009 7c01 a101 72d8  ..v.s.t...|...r.
+00000fe0: 7405 a00a 7c01 a101 6e02 6409 7405 a00a  t...|...n.d.t...
+00000ff0: 7c03 a101 7405 a00a 7c04 a101 7405 a00a  |...t...|...t...
+00001000: 7c05 a101 640a 9c06 1600 7d07 640b 640c  |...d.....}.d.d.
+00001010: 7c07 6901 1600 7d08 740b 7405 a00c 7c08  |.i...}.t.t...|.
+00001020: a101 8301 8201 6400 0400 7d03 0400 7d04  ......d...}...}.
+00001030: 0400 7d06 7d05 6400 5300 290d 4e72 1900  ..}.}.d.S.).Nr..
+00001040: 0000 7246 0000 007a 0220 0a72 0100 0000  ..rF...z. .r....
+00001050: 721a 0000 0072 5700 0000 721d 0000 0072  r....rW...r....r
+00001060: 0400 0000 7250 0000 0072 5800 0000 722e  ....rP...rX...r.
+00001070: 0000 0072 2f00 0000 7259 0000 0072 5a00  ...r/...rY...rZ.
+00001080: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00001090: 00da 1a74 6573 745f 6c6f 6164 5f77 6869  ...test_load_whi
+000010a0: 7465 7370 6163 655f 656d 7074 792f 0000  tespace_empty/..
+000010b0: 0073 0800 0000 0001 0a01 0c01 2802 7a26  .s..........(.z&
+000010c0: 4b56 4669 6c65 5465 7374 732e 7465 7374  KVFileTests.test
+000010d0: 5f6c 6f61 645f 7768 6974 6573 7061 6365  _load_whitespace
+000010e0: 5f65 6d70 7479 6301 0000 0000 0000 0000  _emptyc.........
+000010f0: 0000 000a 0000 0008 0000 0043 0000 0073  ...........C...s
+00001100: 3601 0000 7c00 6a00 6401 1700 7d01 7401  6...|.j.d...}.t.
+00001110: 7c01 6402 8302 8f1a 7d02 7c02 a002 6403  |.d.....}.|...d.
+00001120: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00001130: 6e10 3100 7334 3000 0100 0100 0100 5900  n.1.s40.......Y.
+00001140: 0100 7403 a004 7405 a101 8f18 7d03 7406  ..t...t.....}.t.
+00001150: 7c01 8301 0100 5700 6400 0400 0400 8303  |.....W.d.......
+00001160: 0100 6e10 3100 7366 3000 0100 0100 0100  ..n.1.sf0.......
+00001170: 5900 0100 6404 7d04 7c03 6a07 7d05 7408  Y...d.}.|.j.}.t.
+00001180: 7c05 8301 7d06 7c04 7c06 7600 7d07 7c07  |...}.|.|.v.}.|.
+00001190: 9001 7322 7409 a00a 6405 7c07 6601 6406  ..s"t...d.|.f.d.
+000011a0: 7c04 7c06 6602 a104 7409 a00b 7c04 a101  |.|.f...t...|...
+000011b0: 6407 740c a00d a100 7600 73c2 7409 a00e  d.t.....v.s.t...
+000011c0: 7408 a101 72cc 7409 a00b 7408 a101 6e02  t...r.t...t...n.
+000011d0: 6407 6408 740c a00d a100 7600 73e4 7409  d.d.t.....v.s.t.
+000011e0: a00e 7c03 a101 72ee 7409 a00b 7c03 a101  ..|...r.t...|...
+000011f0: 6e02 6408 7409 a00b 7c05 a101 7409 a00b  n.d.t...|...t...
+00001200: 7c06 a101 6409 9c05 1600 7d08 640a 640b  |...d.....}.d.d.
+00001210: 7c08 6901 1600 7d09 740f 7409 a010 7c09  |.i...}.t.t...|.
+00001220: a101 8301 8201 6400 0400 7d04 0400 7d07  ......d...}...}.
+00001230: 0400 7d05 7d06 6400 5300 290c 4e72 1900  ..}.}.d.S.).Nr..
+00001240: 0000 7246 0000 007a 145b 6e6f 742c 2061  ..rF...z.[not, a
+00001250: 2c20 6469 6374 696f 6e61 7279 5d7a 106e  , dictionary]z.n
+00001260: 6f74 2061 2064 6963 7469 6f6e 6172 7929  ot a dictionary)
+00001270: 01da 0269 6e29 017a 4b25 2870 7931 2973  ...in).zK%(py1)s
+00001280: 2069 6e20 2528 7079 3829 730a 7b25 2870   in %(py8)s.{%(p
+00001290: 7938 2973 203d 2025 2870 7933 2973 2825  y8)s = %(py3)s(%
+000012a0: 2870 7936 2973 0a7b 2528 7079 3629 7320  (py6)s.{%(py6)s 
+000012b0: 3d20 2528 7079 3429 732e 7661 6c75 650a  = %(py4)s.value.
+000012c0: 7d29 0a7d da03 7374 72da 0765 7863 696e  }).}..str..excin
+000012d0: 666f 2905 7221 0000 0072 2200 0000 722a  fo).r!...r"...r*
+000012e0: 0000 0072 2300 0000 7225 0000 007a 0f61  ...r#...r%...z.a
+000012f0: 7373 6572 7420 2528 7079 3130 2973 da04  ssert %(py10)s..
+00001300: 7079 3130 2911 720a 0000 0072 4e00 0000  py10).r....rN...
+00001310: 724f 0000 0072 1500 0000 7216 0000 00da  rO...r....r.....
+00001320: 0954 7970 6545 7272 6f72 7204 0000 00da  .TypeErrorr.....
+00001330: 0576 616c 7565 725e 0000 0072 3000 0000  .valuer^...r0...
+00001340: 7231 0000 0072 3500 0000 7232 0000 0072  r1...r5...r2...r
+00001350: 3300 0000 7234 0000 0072 3600 0000 7237  3...r4...r6...r7
+00001360: 0000 0029 0a72 0c00 0000 7250 0000 0072  ...).r....rP...r
+00001370: 5100 0000 725f 0000 00da 0b40 7079 5f61  Q...r_.....@py_a
+00001380: 7373 6572 7430 723b 0000 0072 5200 0000  ssert0r;...rR...
+00001390: 723a 0000 0072 3e00 0000 da0c 4070 795f  r:...r>.....@py_
+000013a0: 666f 726d 6174 3131 720f 0000 0072 0f00  format11r....r..
+000013b0: 0000 7210 0000 00da 1874 6573 745f 6c6f  ..r......test_lo
+000013c0: 6164 5f6e 6f6e 5f64 6963 7469 6f6e 6172  ad_non_dictionar
+000013d0: 7936 0000 0073 0c00 0000 0001 0a01 0c01  y6...s..........
+000013e0: 2802 0c01 2601 7a24 4b56 4669 6c65 5465  (...&.z$KVFileTe
+000013f0: 7374 732e 7465 7374 5f6c 6f61 645f 6e6f  sts.test_load_no
+00001400: 6e5f 6469 6374 696f 6e61 7279 6301 0000  n_dictionaryc...
+00001410: 0000 0000 0000 0000 000e 0000 0009 0000  ................
+00001420: 0043 0000 0073 9201 0000 7400 7c00 6a01  .C...s....t.|.j.
+00001430: 6401 1700 8301 7d01 7c01 a002 6402 6403  d.....}.|...d.d.
+00001440: a102 0100 7403 7c01 8301 7d02 6404 7d03  ....t.|...}.d.}.
+00001450: 7c02 7c03 6b02 7d04 7c04 73bc 7404 a005  |.|.k.}.|.s.t...
+00001460: 6405 7c04 6601 6406 7c02 7c03 6602 a104  d.|.f.d.|.|.f...
+00001470: 6407 7406 a007 a100 7600 735c 7404 a008  d.t.....v.s\t...
+00001480: 7403 a101 7266 7404 a009 7403 a101 6e02  t...rft...t...n.
+00001490: 6407 6408 7406 a007 a100 7600 737e 7404  d.d.t.....v.s~t.
+000014a0: a008 7c01 a101 7288 7404 a009 7c01 a101  ..|...r.t...|...
+000014b0: 6e02 6408 7404 a009 7c02 a101 7404 a009  n.d.t...|...t...
+000014c0: 7c03 a101 6409 9c04 1600 7d05 640a 640b  |...d.....}.d.d.
+000014d0: 7c05 6901 1600 7d06 740a 7404 a00b 7c06  |.i...}.t.t...|.
+000014e0: a101 8301 8201 6400 0400 7d02 0400 7d04  ......d...}...}.
+000014f0: 7d03 7c01 6a0c 7d07 6402 7d08 640c 7d03  }.|.j.}.d.}.d.}.
+00001500: 7c07 7c08 7c03 8302 7d09 6403 7d0a 7c09  |.|.|...}.d.}.|.
+00001510: 7c0a 6b02 7d0b 7c0b 9001 7376 7404 a005  |.k.}.|...svt...
+00001520: 6405 7c0b 6601 640d 7c09 7c0a 6602 a104  d.|.f.d.|.|.f...
+00001530: 6408 7406 a007 a100 7600 9001 7320 7404  d.t.....v...s t.
+00001540: a008 7c01 a101 9001 722a 7404 a009 7c01  ..|.....r*t...|.
+00001550: a101 6e02 6408 7404 a009 7c07 a101 7404  ..n.d.t...|...t.
+00001560: a009 7c08 a101 7404 a009 7c03 a101 7404  ..|...t...|...t.
+00001570: a009 7c09 a101 7404 a009 7c0a a101 640e  ..|...t...|...d.
+00001580: 9c06 1600 7d0c 640f 6410 7c0c 6901 1600  ....}.d.d.|.i...
+00001590: 7d0d 740a 7404 a00b 7c0d a101 8301 8201  }.t.t...|.......
+000015a0: 6400 0400 7d07 0400 7d08 0400 7d03 0400  d...}...}...}...
+000015b0: 7d09 0400 7d0b 7d0a 6400 5300 2911 4e72  }...}.}.d.S.).Nr
+000015c0: 1900 0000 7226 0000 0072 4900 0000 7247  ....r&...rI...rG
+000015d0: 0000 0072 1a00 0000 721c 0000 0072 1d00  ...r....r....r..
+000015e0: 0000 721e 0000 0072 1f00 0000 7224 0000  ..r....r....r$..
+000015f0: 0072 2500 0000 7248 0000 0072 4a00 0000  .r%...rH...rJ...
+00001600: 724b 0000 0072 4c00 0000 724d 0000 00a9  rK...rL...rM....
+00001610: 0d72 0400 0000 720a 0000 00da 0c73 6574  .r....r......set
+00001620: 5f61 6e64 5f73 6176 6572 1d00 0000 7230  _and_saver....r0
+00001630: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
+00001640: 0000 7234 0000 0072 3500 0000 7236 0000  ..r4...r5...r6..
+00001650: 0072 3700 0000 7239 0000 0029 0e72 0c00  .r7...r9...).r..
+00001660: 0000 721e 0000 0072 3a00 0000 723b 0000  ..r....r:...r;..
+00001670: 0072 3c00 0000 723d 0000 0072 3e00 0000  .r<...r=...r>...
+00001680: 723f 0000 0072 4000 0000 7252 0000 0072  r?...r@...rR...r
+00001690: 5300 0000 7254 0000 0072 4400 0000 7255  S...rT...rD...rU
+000016a0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
+000016b0: 0000 da17 7465 7374 5f67 6574 5f61 6674  ....test_get_aft
+000016c0: 6572 5f73 6574 5f73 616d 653f 0000 0073  er_set_same?...s
+000016d0: 0800 0000 0001 0e01 0c02 ae01 7a23 4b56  ............z#KV
+000016e0: 4669 6c65 5465 7374 732e 7465 7374 5f67  FileTests.test_g
+000016f0: 6574 5f61 6674 6572 5f73 6574 5f73 616d  et_after_set_sam
+00001700: 6563 0100 0000 0000 0000 0000 0000 0f00  ec..............
+00001710: 0000 0900 0000 4300 0000 73a0 0100 0074  ......C...s....t
+00001720: 007c 006a 0164 0117 0083 017d 017c 01a0  .|.j.d.....}.|..
+00001730: 0264 0264 03a1 0201 0074 007c 006a 0164  .d.d.....t.|.j.d
+00001740: 0117 0083 017d 0274 037c 0283 017d 0364  .....}.t.|...}.d
+00001750: 047d 047c 037c 046b 027d 057c 0573 ca74  .}.|.|.k.}.|.s.t
+00001760: 04a0 0564 057c 0566 0164 067c 037c 0466  ...d.|.f.d.|.|.f
+00001770: 02a1 0464 0774 06a0 07a1 0076 0073 6a74  ...d.t.....v.sjt
+00001780: 04a0 0874 03a1 0172 7474 04a0 0974 03a1  ...t...rtt...t..
+00001790: 016e 0264 0764 0874 06a0 07a1 0076 0073  .n.d.d.t.....v.s
+000017a0: 8c74 04a0 087c 02a1 0172 9674 04a0 097c  .t...|...r.t...|
+000017b0: 02a1 016e 0264 0874 04a0 097c 03a1 0174  ...n.d.t...|...t
+000017c0: 04a0 097c 04a1 0164 099c 0416 007d 0664  ...|...d.....}.d
+000017d0: 0a64 0b7c 0669 0116 007d 0774 0a74 04a0  .d.|.i...}.t.t..
+000017e0: 0b7c 07a1 0183 0182 0164 0004 007d 0304  .|.......d...}..
+000017f0: 007d 057d 047c 026a 0c7d 0864 027d 0964  .}.}.|.j.}.d.}.d
+00001800: 0c7d 047c 087c 097c 0483 027d 0a64 037d  .}.|.|.|...}.d.}
+00001810: 0b7c 0a7c 0b6b 027d 0c7c 0c90 0173 8474  .|.|.k.}.|...s.t
+00001820: 04a0 0564 057c 0c66 0164 0d7c 0a7c 0b66  ...d.|.f.d.|.|.f
+00001830: 02a1 0464 0874 06a0 07a1 0076 0090 0173  ...d.t.....v...s
+00001840: 2e74 04a0 087c 02a1 0190 0172 3874 04a0  .t...|.....r8t..
+00001850: 097c 02a1 016e 0264 0874 04a0 097c 08a1  .|...n.d.t...|..
+00001860: 0174 04a0 097c 09a1 0174 04a0 097c 04a1  .t...|...t...|..
+00001870: 0174 04a0 097c 0aa1 0174 04a0 097c 0ba1  .t...|...t...|..
+00001880: 0164 0e9c 0616 007d 0d64 0f64 107c 0d69  .d.....}.d.d.|.i
+00001890: 0116 007d 0e74 0a74 04a0 0b7c 0ea1 0183  ...}.t.t...|....
+000018a0: 0182 0164 0004 007d 0804 007d 0904 007d  ...d...}...}...}
+000018b0: 0404 007d 0a04 007d 0c7d 0b64 0053 0029  ...}...}.}.d.S.)
+000018c0: 114e 7219 0000 0072 2600 0000 7249 0000  .Nr....r&...rI..
+000018d0: 0072 4700 0000 721a 0000 0072 1c00 0000  .rG...r....r....
+000018e0: 721d 0000 00da 046b 7666 3272 1f00 0000  r......kvf2r....
+000018f0: 7224 0000 0072 2500 0000 7248 0000 0072  r$...r%...rH...r
+00001900: 4a00 0000 724b 0000 0072 4c00 0000 724d  J...rK...rL...rM
+00001910: 0000 0072 6600 0000 290f 720c 0000 0072  ...rf...).r....r
+00001920: 1e00 0000 7269 0000 0072 3a00 0000 723b  ....ri...r:...r;
+00001930: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
+00001940: 0000 723f 0000 0072 4000 0000 7252 0000  ..r?...r@...rR..
+00001950: 0072 5300 0000 7254 0000 0072 4400 0000  .rS...rT...rD...
+00001960: 7255 0000 0072 0f00 0000 720f 0000 0072  rU...r....r....r
+00001970: 1000 0000 da15 7465 7374 5f6c 6f61 645f  ......test_load_
+00001980: 7365 636f 6e64 5f73 616d 6546 0000 0073  second_sameF...s
+00001990: 0a00 0000 0001 0e01 0c01 0e02 ae01 7a21  ..............z!
+000019a0: 4b56 4669 6c65 5465 7374 732e 7465 7374  KVFileTests.test
+000019b0: 5f6c 6f61 645f 7365 636f 6e64 5f73 616d  _load_second_sam
+000019c0: 6563 0100 0000 0000 0000 0000 0000 0e00  ec..............
+000019d0: 0000 0800 0000 4300 0000 73a6 0100 007c  ......C...s....|
+000019e0: 006a 0064 0117 007d 0174 017c 0183 017d  .j.d...}.t.|...}
+000019f0: 027c 02a0 0264 0264 03a1 0201 007c 02a0  .|...d.d.....|..
+00001a00: 0264 0464 03a1 0201 0074 037c 0183 018f  .d.d.....t.|....
+00001a10: 2c7d 037c 03a0 04a1 007d 047c 03a0 0564  ,}.|.....}.|...d
+00001a20: 05a1 0101 0074 06a0 077c 03a1 017d 0557  .....t...|...}.W
+00001a30: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00001a40: 6430 0001 0001 0001 0059 0001 0074 087c  d0.......Y...t.|
+00001a50: 0483 017d 0664 067d 077c 067c 076b 027d  ...}.d.}.|.|.k.}
+00001a60: 087c 0890 0173 1274 09a0 0a64 077c 0866  .|...s.t...d.|.f
+00001a70: 0164 087c 067c 0766 02a1 0464 0974 0ba0  .d.|.|.f...d.t..
+00001a80: 0ca1 0076 0073 b274 09a0 0d74 08a1 0172  ...v.s.t...t...r
+00001a90: bc74 09a0 0e74 08a1 016e 0264 0964 0a74  .t...t...n.d.d.t
+00001aa0: 0ba0 0ca1 0076 0073 d474 09a0 0d7c 04a1  .....v.s.t...|..
+00001ab0: 0172 de74 09a0 0e7c 04a1 016e 0264 0a74  .r.t...|...n.d.t
+00001ac0: 09a0 0e7c 06a1 0174 09a0 0e7c 07a1 0164  ...|...t...|...d
+00001ad0: 0b9c 0416 007d 0964 0c64 0d7c 0969 0116  .....}.d.d.|.i..
+00001ae0: 007d 0a74 0f74 09a0 107c 0aa1 0183 0182  .}.t.t...|......
+00001af0: 0164 0004 007d 0604 007d 087d 0764 0364  .d...}...}.}.d.d
+00001b00: 0364 0e9c 027d 067c 057c 066b 027d 0b7c  .d...}.|.|.k.}.|
+00001b10: 0b90 0173 9a74 09a0 0a64 077c 0b66 0164  ...s.t...d.|.f.d
+00001b20: 0f7c 057c 0666 02a1 0464 1074 0ba0 0ca1  .|.|.f...d.t....
+00001b30: 0076 0090 0173 6474 09a0 0d7c 05a1 0190  .v...sdt...|....
+00001b40: 0172 6e74 09a0 0e7c 05a1 016e 0264 1074  .rnt...|...n.d.t
+00001b50: 09a0 0e7c 06a1 0164 119c 0216 007d 0c64  ...|...d.....}.d
+00001b60: 1264 137c 0c69 0116 007d 0d74 0f74 09a0  .d.|.i...}.t.t..
+00001b70: 107c 0da1 0183 0182 0164 0004 007d 0b7d  .|.......d...}.}
+00001b80: 0664 0053 0029 144e 7219 0000 0072 2600  .d.S.).Nr....r&.
+00001b90: 0000 7249 0000 00da 0466 6f6f 3272 0100  ..rI.....foo2r..
+00001ba0: 0000 e902 0000 0072 1a00 0000 721c 0000  .......r....r...
+00001bb0: 0072 1d00 0000 da05 6c69 6e65 7372 1f00  .r......linesr..
+00001bc0: 0000 7224 0000 0072 2500 0000 2902 7226  ..r$...r%...).r&
+00001bd0: 0000 0072 6b00 0000 2901 7a12 2528 7079  ...rk...).z.%(py
+00001be0: 3029 7320 3d3d 2025 2870 7933 2973 da04  0)s == %(py3)s..
+00001bf0: 6461 7461 2902 7220 0000 0072 2200 0000  data).r ...r"...
+00001c00: 7a0e 6173 7365 7274 2025 2870 7935 2973  z.assert %(py5)s
+00001c10: 722b 0000 0029 1172 0a00 0000 7204 0000  r+...).r....r...
+00001c20: 0072 6700 0000 724e 0000 00da 0972 6561  .rg...rN.....rea
+00001c30: 646c 696e 6573 da04 7365 656b da04 7961  dlines..seek..ya
+00001c40: 6d6c da09 7361 6665 5f6c 6f61 6472 1d00  ml..safe_loadr..
+00001c50: 0000 7230 0000 0072 3100 0000 7232 0000  ..r0...r1...r2..
+00001c60: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
+00001c70: 7236 0000 0072 3700 0000 290e 720c 0000  r6...r7...).r...
+00001c80: 0072 5000 0000 721e 0000 0072 5100 0000  .rP...r....rQ...
+00001c90: 726d 0000 0072 6e00 0000 723a 0000 0072  rm...rn...r:...r
+00001ca0: 3b00 0000 723c 0000 0072 3d00 0000 723e  ;...r<...r=...r>
+00001cb0: 0000 0072 3f00 0000 da0b 4070 795f 666f  ...r?.....@py_fo
+00001cc0: 726d 6174 34da 0b40 7079 5f66 6f72 6d61  rmat4..@py_forma
+00001cd0: 7436 720f 0000 0072 0f00 0000 7210 0000  t6r....r....r...
+00001ce0: 00da 2774 6573 745f 7365 7473 5f64 6f6e  ..'test_sets_don
+00001cf0: 745f 6361 7573 655f 6170 7065 6e64 5f64  t_cause_append_d
+00001d00: 7570 6c69 6361 7469 6f6e 4e00 0000 7314  uplicationN...s.
+00001d10: 0000 0000 010a 0108 010c 010c 020a 0108  ................
+00001d20: 010a 0128 02b0 017a 334b 5646 696c 6554  ...(...z3KVFileT
+00001d30: 6573 7473 2e74 6573 745f 7365 7473 5f64  ests.test_sets_d
+00001d40: 6f6e 745f 6361 7573 655f 6170 7065 6e64  ont_cause_append
+00001d50: 5f64 7570 6c69 6361 7469 6f6e 290f da08  _duplication)...
+00001d60: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00001d70: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00001d80: 5f5f 7208 0000 0072 1300 0000 7218 0000  __r....r....r...
+00001d90: 0072 4500 0000 7256 0000 0072 5b00 0000  .rE...rV...r[...
+00001da0: 725c 0000 0072 6500 0000 7268 0000 0072  r\...re...rh...r
+00001db0: 6a00 0000 7275 0000 00da 0d5f 5f63 6c61  j...ru.....__cla
+00001dc0: 7373 6365 6c6c 5f5f 720f 0000 0072 0f00  sscell__r....r..
+00001dd0: 0000 720d 0000 0072 1000 0000 7205 0000  ..r....r....r...
+00001de0: 000b 0000 0073 1600 0000 0801 0c05 0c04  .....s..........
+00001df0: 0804 0806 0809 0807 0807 0809 0807 0808  ................
+00001e00: 7205 0000 0029 10da 0862 7569 6c74 696e  r....)...builtin
+00001e10: 7372 3200 0000 da19 5f70 7974 6573 742e  sr2....._pytest.
+00001e20: 6173 7365 7274 696f 6e2e 7265 7772 6974  assertion.rewrit
+00001e30: 65da 0961 7373 6572 7469 6f6e da07 7265  e..assertion..re
+00001e40: 7772 6974 6572 3000 0000 7211 0000 00da  writer0...r.....
+00001e50: 0874 656d 7066 696c 6572 0200 0000 7215  .tempfiler....r.
+00001e60: 0000 0072 7100 0000 da0b 646a 616e 676f  ...rq.....django
+00001e70: 2e74 6573 7472 0300 0000 da14 646a 616e  .testr......djan
+00001e80: 676f 5f70 6572 665f 7265 632e 7961 6d6c  go_perf_rec.yaml
+00001e90: 7204 0000 0072 0500 0000 720f 0000 0072  r....r....r....r
+00001ea0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
+00001eb0: 3c6d 6f64 756c 653e 0100 0000 730c 0000  <module>....s...
+00001ec0: 0022 010c 0208 0108 010c 020c 03         ."...........
```

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.2.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.2.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.4.2.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/test_yaml.cpython-38-pytest-5.4.2.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-35.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-36.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-37.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/__pycache__/utils.cpython-38.pyc` & `django-perf-rec-4.9.0/tests/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/settings.py` & `django-perf-rec-4.9.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/test_api.perf.yml` & `django-perf-rec-4.9.0/tests/test_api.perf.yml`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/test_api.py` & `django-perf-rec-4.9.0/tests/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,35 @@
 
 
 class RecordTests(TestCase):
     def test_single_db_query(self):
         with record():
             run_query("default", "SELECT 1337")
 
+    def test_single_db_query_with_traceback(self):
+        with pretend_not_under_pytest():
+            with pytest.raises(AssertionError) as excinfo:
+
+                def capture_traceback(operation):
+                    return True
+
+                with record(
+                    record_name="RecordTests.test_single_db_query",
+                    capture_traceback=capture_traceback,
+                ):
+                    run_query("default", "SELECT 1337")
+
+            msg = str(excinfo.value)
+            assert (
+                "Performance record did not match for RecordTests.test_single_db_query"
+                in msg
+            )
+            assert "+ traceback:" in msg
+            assert "in test_single_db_query_with_traceback" in msg
+
     def test_single_db_query_model(self):
         with record():
             list(Author.objects.all())
 
     @override_settings(PERF_REC={"HIDE_COLUMNS": False})
     def test_single_db_query_model_with_columns(self):
         with record():
@@ -44,14 +65,31 @@
         with record():
             list(Author.objects.filter(Q(name="foo", age=1)))
 
     def test_single_cache_op(self):
         with record():
             caches["default"].get("foo")
 
+    def test_single_cache_op_with_traceback(self):
+        with pretend_not_under_pytest():
+            with pytest.raises(AssertionError) as excinfo:
+
+                def capture_traceback(operation):
+                    return True
+
+                with record(
+                    record_name="RecordTests.test_single_cache_op",
+                    capture_traceback=capture_traceback,
+                ):
+                    caches["default"].get("foo")
+
+            msg = str(excinfo.value)
+            assert "+ traceback:" in msg
+            assert "in test_single_cache_op_with_traceback" in msg
+
     def test_multiple_cache_ops(self):
         with record():
             caches["default"].set("foo", "bar")
             caches["second"].get_many(["foo", "bar"])
             caches["default"].delete("foo")
 
     def test_multiple_calls_in_same_function_are_different_records(self):
```

### Comparing `django-perf-rec-4.8.0/tests/test_cache.py` & `django-perf-rec-4.9.0/tests/test_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
+from unittest import mock
+
 import pytest
 from django.core.cache import caches
 from django.test import SimpleTestCase, TestCase
 
 from django_perf_rec.cache import AllCacheRecorder, CacheOp, CacheRecorder
-
-try:
-    from unittest import mock
-except ImportError:
-    import mock
+from tests.utils import disable_traceback
 
 
 class CacheOpTests(SimpleTestCase):
     def test_clean_key_integer(self):
         assert CacheOp.clean_key("foo1") == "foo#"
 
     def test_clean_key_uuid(self):
@@ -25,68 +23,88 @@
         assert CacheOp.clean_key(key) == "django.contrib.sessions.cache#"
 
     def test_clean_key_session_key_cached_db_backend(self):
         key = "django.contrib.sessions.cached_db" + "abcdefghijklmnopqrstuvwxyz012345"
         assert CacheOp.clean_key(key) == "django.contrib.sessions.cached_db#"
 
     def test_key(self):
-        op = CacheOp("default", "foo", "bar")
+        op = CacheOp("default", "foo", "bar", None)
         assert op.alias == "default"
         assert op.operation == "foo"
         assert op.query == "bar"
 
     def test_keys(self):
-        op = CacheOp("default", "foo", ["bar", "baz"])
+        op = CacheOp("default", "foo", ["bar", "baz"], None)
         assert op.alias == "default"
         assert op.operation == "foo"
         assert op.query == ["bar", "baz"]
 
     def test_invalid(self):
         with pytest.raises(ValueError):
-            CacheOp("x", "foo", object())
+            CacheOp("x", "foo", object(), None)
 
     def test_equal(self):
-        assert CacheOp("x", "foo", "bar") == CacheOp("x", "foo", "bar")
+        assert CacheOp("x", "foo", "bar", "traceback") == CacheOp(
+            "x", "foo", "bar", "traceback"
+        )
 
     def test_not_equal_alias(self):
-        assert CacheOp("x", "foo", "bar") != CacheOp("y", "foo", "bar")
+        assert CacheOp("x", "foo", "bar", None) != CacheOp("y", "foo", "bar", None)
 
     def test_not_equal_operation(self):
-        assert CacheOp("x", "foo", "bar") != CacheOp("x", "bar", "bar")
+        assert CacheOp("x", "foo", "bar", None) != CacheOp("x", "bar", "bar", None)
 
     def test_not_equal_keys(self):
-        assert CacheOp("x", "foo", ["bar"]) != CacheOp("x", "foo", ["baz"])
+        assert CacheOp("x", "foo", ["bar"], None) != CacheOp("x", "foo", ["baz"], None)
+
+    def test_not_equal_traceback(self):
+        assert CacheOp("x", "foo", "bar", "traceback") != CacheOp(
+            "x", "foo", "bar", None
+        )
 
 
 class CacheRecorderTests(TestCase):
-    def test_default(self):
+    @disable_traceback
+    def test_default(self, extract_stack):
         callback = mock.Mock()
         with CacheRecorder("default", callback):
             caches["default"].get("foo")
-        callback.assert_called_once_with(CacheOp("default", "get", "foo"))
+        callback.assert_called_once_with(CacheOp("default", "get", "foo", None))
 
-    def test_secondary(self):
+    @disable_traceback
+    def test_secondary(self, extract_stack):
         callback = mock.Mock()
         with CacheRecorder("second", callback):
             caches["second"].get("foo")
-        callback.assert_called_once_with(CacheOp("second", "get", "foo"))
+        callback.assert_called_once_with(CacheOp("second", "get", "foo", None))
 
     def test_secondary_default_not_recorded(self):
         callback = mock.Mock()
         with CacheRecorder("second", callback):
             caches["default"].get("foo")
         assert len(callback.mock_calls) == 0
 
+    def test_record_traceback(self):
+        callback = mock.Mock()
+        with CacheRecorder("default", callback):
+            caches["default"].get("foo")
+
+        assert len(callback.mock_calls) == 1
+        assert "django_perf_rec/cache.py" in str(
+            callback.call_args_list[0][0][0].traceback
+        )
+
 
 class AllCacheRecorderTests(TestCase):
-    def test_records_all(self):
+    @disable_traceback
+    def test_records_all(self, extract_stack):
         callback = mock.Mock()
         with AllCacheRecorder(callback):
             caches["default"].get("foo")
             caches["second"].set("bar", "baz")
             caches["default"].delete_many(["foo"])
 
         assert callback.mock_calls == [
-            mock.call(CacheOp("default", "get", "foo")),
-            mock.call(CacheOp("second", "set", "bar")),
-            mock.call(CacheOp("default", "delete_many", ["foo"])),
+            mock.call(CacheOp("default", "get", "foo", None)),
+            mock.call(CacheOp("second", "set", "bar", None)),
+            mock.call(CacheOp("default", "delete_many", ["foo"], None)),
         ]
```

### Comparing `django-perf-rec-4.8.0/tests/test_db.py` & `django-perf-rec-4.9.0/tests/test_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,85 @@
+from unittest import mock
+
 from django.test import SimpleTestCase, TestCase
 
 from django_perf_rec.db import AllDBRecorder, DBOp, DBRecorder
-from tests.utils import run_query
-
-try:
-    from unittest import mock
-except ImportError:
-    import mock
+from tests.utils import disable_traceback, run_query
 
 
 class DBOpTests(SimpleTestCase):
     def test_create(self):
-        op = DBOp("myalias", "SELECT 1")
+        op = DBOp("myalias", "SELECT 1", None)
         assert op.alias == "myalias"
         assert op.query == "SELECT 1"
+        assert op.traceback is None
 
     def test_equal(self):
-        assert DBOp("foo", "bar") == DBOp("foo", "bar")
+        assert DBOp("foo", "bar", "traceback") == DBOp("foo", "bar", "traceback")
 
     def test_not_equal_alias(self):
-        assert DBOp("foo", "bar") != DBOp("baz", "bar")
+        assert DBOp("foo", "bar", None) != DBOp("baz", "bar", None)
 
     def test_not_equal_sql(self):
-        assert DBOp("foo", "bar") != DBOp("foo", "baz")
+        assert DBOp("foo", "bar", None) != DBOp("foo", "baz", None)
+
+    def test_not_equal_traceback(self):
+        assert DBOp("foo", "bar", "traceback") != DBOp("foo", "baz", None)
 
 
 class DBRecorderTests(TestCase):
     databases = ("default", "second", "replica")
 
-    def test_default(self):
+    @disable_traceback
+    def test_default(self, extract_stack):
         callback = mock.Mock()
         with DBRecorder("default", callback):
             run_query("default", "SELECT 1")
-        callback.assert_called_once_with(DBOp("default", "SELECT #"))
+        callback.assert_called_once_with(DBOp("default", "SELECT #", None))
 
-    def test_secondary(self):
+    @disable_traceback
+    def test_secondary(self, extract_stack):
         callback = mock.Mock()
         with DBRecorder("second", callback):
             run_query("second", "SELECT 1")
-        callback.assert_called_once_with(DBOp("second", "SELECT #"))
+        callback.assert_called_once_with(DBOp("second", "SELECT #", None))
 
-    def test_replica(self):
+    @disable_traceback
+    def test_replica(self, extract_stack):
         callback = mock.Mock()
         with DBRecorder("replica", callback):
             run_query("replica", "SELECT 1")
-        callback.assert_called_once_with(DBOp("replica", "SELECT #"))
+        callback.assert_called_once_with(DBOp("replica", "SELECT #", None))
 
     def test_secondary_default_not_recorded(self):
         callback = mock.Mock()
         with DBRecorder("second", callback):
             run_query("default", "SELECT 1")
         assert len(callback.mock_calls) == 0
 
+    def test_record_traceback(self):
+        callback = mock.Mock()
+        with DBRecorder("default", callback):
+            run_query("default", "SELECT 1")
+
+        assert len(callback.mock_calls) == 1
+        assert "django_perf_rec/db.py" in str(
+            callback.call_args_list[0][0][0].traceback
+        )
+
 
 class AllDBRecorderTests(TestCase):
     databases = ("default", "second", "replica")
 
-    def test_records_all(self):
+    @disable_traceback
+    def test_records_all(self, extract_stack):
         callback = mock.Mock()
         with AllDBRecorder(callback):
             run_query("replica", "SELECT 1")
             run_query("default", "SELECT 2")
             run_query("second", "SELECT 3")
 
         assert callback.mock_calls == [
-            mock.call(DBOp("replica", "SELECT #")),
-            mock.call(DBOp("default", "SELECT #")),
-            mock.call(DBOp("second", "SELECT #")),
+            mock.call(DBOp("replica", "SELECT #", None)),
+            mock.call(DBOp("default", "SELECT #", None)),
+            mock.call(DBOp("second", "SELECT #", None)),
         ]
```

### Comparing `django-perf-rec-4.8.0/tests/test_pytest_fixture_usage.py` & `django-perf-rec-4.9.0/tests/test_pytest_fixture_usage.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/test_sql.py` & `django-perf-rec-4.9.0/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/test_utils.py` & `django-perf-rec-4.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/test_yaml.py` & `django-perf-rec-4.9.0/tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-35.pyc` & `django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-36.pyc` & `django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-37.pyc` & `django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-38.pyc` & `django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/testapp/__pycache__/models.cpython-39.pyc` & `django-perf-rec-4.9.0/tests/testapp/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/testapp/models.py` & `django-perf-rec-4.9.0/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-perf-rec-4.8.0/tests/utils.py` & `django-perf-rec-4.9.0/tests/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import errno
 import os
 import shutil
+import traceback
 from contextlib import contextmanager
+from unittest import mock
 
 from django.db import connections
 
 from django_perf_rec import pytest_plugin
 
 
 def run_query(alias, sql, params=None):
@@ -35,7 +37,10 @@
 def pretend_not_under_pytest():
     orig = pytest_plugin.in_pytest
     pytest_plugin.in_pytest = False
     try:
         yield
     finally:
         pytest_plugin.in_pytest = orig
+
+
+disable_traceback = mock.patch.object(traceback, "extract_stack", return_value=None)
```

