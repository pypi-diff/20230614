# Comparing `tmp/obis-0.4.1.tar.gz` & `tmp/obis-0.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obis-0.4.1.tar", last modified: Wed Mar 29 13:53:08 2023, max compression
+gzip compressed data, was "obis-0.4.2rc1.tar", last modified: Fri Mar 31 13:08:19 2023, max compression
```

## Comparing `obis-0.4.1.tar` & `obis-0.4.2rc1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.761636 obis-0.4.1/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      475 2023-03-29 13:52:34.000000 obis-0.4.1/CHANGELOG.md
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.1/LICENSE
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.1/MANIFEST.in
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    29595 2023-03-29 13:53:08.761636 obis-0.4.1/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    29036 2023-03-07 14:12:15.000000 obis-0.4.1/README.md
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.717635 obis-0.4.1/man/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.729636 obis-0.4.1/man/man1/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-addref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-clone.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-collection.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-commit.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-config.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-data_set.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-download.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-init.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-init_analysis.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-move.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-object.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-removeref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-repository.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-settings.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-status.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis-sync.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.1/man/man1/obis.1
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.729636 obis-0.4.1/obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      754 2023-03-28 07:04:01.000000 obis-0.4.1/obis/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.733636 obis-0.4.1/obis/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      317 2023-03-29 13:31:31.000000 obis-0.4.1/obis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.1/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.1/obis/conftest.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.737636 obis-0.4.1/obis/dm/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.741636 obis-0.4.1/obis/dm/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.1/obis/dm/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.1/obis/dm/__pycache__/checksum.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.1/obis/dm/__pycache__/command_log.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.1/obis/dm/__pycache__/command_result.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.1/obis/dm/__pycache__/config.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    22942 2023-03-03 10:58:54.000000 obis-0.4.1/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-03-29 13:31:59.000000 obis-0.4.1/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6894 2023-02-23 08:54:08.000000 obis-0.4.1/obis/dm/__pycache__/git.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.1/obis/dm/__pycache__/repository_utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3132 2023-02-27 10:08:46.000000 obis-0.4.1/obis/dm/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.1/obis/dm/checksum.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/command_log.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/command_result.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.745636 obis-0.4.1/obis/dm/commands/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/commands/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.749636 obis-0.4.1/obis/dm/commands/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.1/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-02-21 12:13:21.000000 obis-0.4.1/obis/dm/commands/__pycache__/addref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.1/obis/dm/commands/__pycache__/clone.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.1/obis/dm/commands/__pycache__/collection.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.1/obis/dm/commands/__pycache__/download.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.1/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.1/obis/dm/commands/__pycache__/move.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.1/obis/dm/commands/__pycache__/object.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10914 2023-03-29 13:49:33.000000 obis-0.4.1/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.1/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.1/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2849 2023-03-03 10:58:54.000000 obis-0.4.1/obis/dm/commands/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.1/obis/dm/commands/__pycache__/upload.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/commands/addref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.1/obis/dm/commands/clone.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.1/obis/dm/commands/collection.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.1/obis/dm/commands/download.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.1/obis/dm/commands/download_physical.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/commands/move.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.1/obis/dm/commands/object.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12023 2023-03-29 13:49:21.000000 obis-0.4.1/obis/dm/commands/openbis_command.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/commands/openbis_command_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/commands/openbis_sync.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/commands/removeref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4366 2023-03-03 10:58:45.000000 obis-0.4.1/obis/dm/commands/search.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.1/obis/dm/commands/upload.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.1/obis/dm/config.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/config_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27633 2023-03-03 10:44:27.000000 obis-0.4.1/obis/dm/data_mgmt.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.1/obis/dm/data_mgmt_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.1/obis/dm/git-annex-attributes
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8138 2023-02-23 08:53:54.000000 obis-0.4.1/obis/dm/git.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/repository_utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3720 2023-02-27 10:08:42.000000 obis-0.4.1/obis/dm/utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.1/obis/dm/utils_test.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.749636 obis-0.4.1/obis/scripts/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.1/obis/scripts/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.749636 obis-0.4.1/obis/scripts/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.1/obis/scripts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    25500 2023-03-03 11:10:17.000000 obis-0.4.1/obis/scripts/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.1/obis/scripts/__pycache__/click_util.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-02-28 13:09:17.000000 obis-0.4.1/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31141 2023-03-03 11:10:13.000000 obis-0.4.1/obis/scripts/cli.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.1/obis/scripts/click_util.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-02-28 13:09:09.000000 obis-0.4.1/obis/scripts/data_mgmt_runner.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.757636 obis-0.4.1/obis/test-data/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.1/obis/test-data/snb-data.zip
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.1/obis/test-data/text-data-2.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.1/obis/test-data/text-data.txt
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.717635 obis-0.4.1/obis/test-data/user_config/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.761636 obis-0.4.1/obis/test-data/user_config/.obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.1/obis/test-data/user_config/.obis/config.json
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-29 13:53:08.733636 obis-0.4.1/obis.egg-info/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    29595 2023-03-29 13:53:08.000000 obis-0.4.1/obis.egg-info/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-03-29 13:53:08.000000 obis-0.4.1/obis.egg-info/SOURCES.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-03-29 13:53:08.000000 obis-0.4.1/obis.egg-info/dependency_links.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-03-29 13:53:08.000000 obis-0.4.1/obis.egg-info/entry_points.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.1/obis.egg-info/not-zip-safe
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-03-29 13:53:08.000000 obis-0.4.1/obis.egg-info/requires.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-03-29 13:53:08.000000 obis-0.4.1/obis.egg-info/top_level.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-03-29 13:53:08.761636 obis-0.4.1/setup.cfg
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1982 2023-03-28 07:04:01.000000 obis-0.4.1/setup.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.952626 obis-0.4.2rc1/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      680 2023-03-30 13:23:35.000000 obis-0.4.2rc1/CHANGELOG.md
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.2rc1/LICENSE
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.2rc1/MANIFEST.in
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30929 2023-03-31 13:08:19.952626 obis-0.4.2rc1/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30367 2023-03-31 13:07:05.000000 obis-0.4.2rc1/README.md
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.876625 obis-0.4.2rc1/man/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.900625 obis-0.4.2rc1/man/man1/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-addref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-clone.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-collection.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-commit.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-config.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-data_set.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-download.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-init.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-init_analysis.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-move.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-object.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-removeref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-repository.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-settings.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-status.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis-sync.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.2rc1/man/man1/obis.1
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.904626 obis-0.4.2rc1/obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-03-30 11:24:06.000000 obis-0.4.2rc1/obis/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.908625 obis-0.4.2rc1/obis/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      320 2023-03-30 11:28:49.000000 obis-0.4.2rc1/obis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.2rc1/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/conftest.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.920626 obis-0.4.2rc1/obis/dm/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.920626 obis-0.4.2rc1/obis/dm/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.2rc1/obis/dm/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.2rc1/obis/dm/__pycache__/checksum.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.2rc1/obis/dm/__pycache__/command_log.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.2rc1/obis/dm/__pycache__/command_result.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.2rc1/obis/dm/__pycache__/config.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-03-30 13:34:10.000000 obis-0.4.2rc1/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-03-29 13:31:59.000000 obis-0.4.2rc1/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.2rc1/obis/dm/__pycache__/git.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.2rc1/obis/dm/__pycache__/repository_utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.2rc1/obis/dm/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.2rc1/obis/dm/checksum.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/command_log.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/command_result.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.928626 obis-0.4.2rc1/obis/dm/commands/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/commands/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.932626 obis-0.4.2rc1/obis/dm/commands/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/addref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/clone.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/collection.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/download.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/move.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/object.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10941 2023-03-30 10:21:33.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4708 2023-03-31 12:20:58.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1589 2023-02-24 12:01:17.000000 obis-0.4.2rc1/obis/dm/commands/__pycache__/upload.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.2rc1/obis/dm/commands/addref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.2rc1/obis/dm/commands/clone.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.2rc1/obis/dm/commands/collection.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.2rc1/obis/dm/commands/download.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.2rc1/obis/dm/commands/download_physical.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/commands/move.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.2rc1/obis/dm/commands/object.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-03-30 10:21:12.000000 obis-0.4.2rc1/obis/dm/commands/openbis_command.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/commands/openbis_command_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/commands/openbis_sync.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/commands/removeref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6660 2023-03-31 12:39:08.000000 obis-0.4.2rc1/obis/dm/commands/search.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1801 2023-02-24 12:00:59.000000 obis-0.4.2rc1/obis/dm/commands/upload.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.2rc1/obis/dm/config.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/config_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-03-30 13:30:39.000000 obis-0.4.2rc1/obis/dm/data_mgmt.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.2rc1/obis/dm/data_mgmt_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.2rc1/obis/dm/git-annex-attributes
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.2rc1/obis/dm/git.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/repository_utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.2rc1/obis/dm/utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/dm/utils_test.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.932626 obis-0.4.2rc1/obis/scripts/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/scripts/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.936626 obis-0.4.2rc1/obis/scripts/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.2rc1/obis/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    28937 2023-03-31 10:16:28.000000 obis-0.4.2rc1/obis/scripts/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-21 12:13:22.000000 obis-0.4.2rc1/obis/scripts/__pycache__/click_util.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.2rc1/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    35475 2023-03-31 10:16:23.000000 obis-0.4.2rc1/obis/scripts/cli.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1126 2023-02-21 12:05:41.000000 obis-0.4.2rc1/obis/scripts/click_util.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.2rc1/obis/scripts/data_mgmt_runner.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.948626 obis-0.4.2rc1/obis/test-data/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.2rc1/obis/test-data/snb-data.zip
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.2rc1/obis/test-data/text-data-2.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.2rc1/obis/test-data/text-data.txt
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.876625 obis-0.4.2rc1/obis/test-data/user_config/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.948626 obis-0.4.2rc1/obis/test-data/user_config/.obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.2rc1/obis/test-data/user_config/.obis/config.json
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-03-31 13:08:19.904626 obis-0.4.2rc1/obis.egg-info/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30929 2023-03-31 13:08:19.000000 obis-0.4.2rc1/obis.egg-info/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-03-31 13:08:19.000000 obis-0.4.2rc1/obis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-03-31 13:08:19.000000 obis-0.4.2rc1/obis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-03-31 13:08:19.000000 obis-0.4.2rc1/obis.egg-info/entry_points.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.2rc1/obis.egg-info/not-zip-safe
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-03-31 13:08:19.000000 obis-0.4.2rc1/obis.egg-info/requires.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-03-31 13:08:19.000000 obis-0.4.2rc1/obis.egg-info/top_level.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-03-31 13:08:19.952626 obis-0.4.2rc1/setup.cfg
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1985 2023-03-30 11:24:06.000000 obis-0.4.2rc1/setup.py
```

### Comparing `obis-0.4.1/LICENSE` & `obis-0.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/PKG-INFO` & `obis-0.4.2rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: obis
-Version: 0.4.1
-Summary: Local data management with assistance from OpenBIS.
-Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
-Author: ID SIS • ETH Zürich
-Author-email: openbis-support@id.ethz.ch
-License: Apache Software License Version 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # openBIS Command Line Tool (oBIS)
 
 oBIS is a command-line tool that makes it possible to handle data sets tracked by OpenBIS,
 where users have complete freedom to structure and manipulate the data as they wish, while retaining
 the benefits of openBIS.
 
 With oBIS, it is possible not only to handle datasets stored in OpenBIS but also available to keep
@@ -33,17 +18,20 @@
     1. [Standard Data Store](#51-standard-data-store)
         1. [Commands](#511-commands)
         2. [Examples](#512-examples)
     2. [External Data Store](#52-external-data-store)
         1. [Settings](#521-settings)
         2. [Commands](#522-commands)
         3. [Examples](#523-examples)
-6. [Big Data Link Services](#6-big-data-link-services)
-7. [Rationale for obis](#7-rationale-for-obis)
-8. [Literature](#8-literature)
+6. [Authentication](#6-authentication)
+   1. [Login](#61-login)
+   2. [Personal Access Token](#62-personal-access-token)
+7. [Big Data Link Services](#7-big-data-link-services)
+8. [Rationale for obis](#8-rationale-for-obis)
+9. [Literature](#9-literature)
 
 ## 1. Prerequisites
 
 - python 3.6 or higher
 - git 2.11 or higher
 - git-annex 6 or higher [Installation guide](https://git-annex.branchable.com/install/)
 
@@ -177,15 +165,15 @@
 | repository set   |          ❌          |          ✅          |
 | repository clear |          ❌          |          ✅          |
 | settings get     |          ❌          |          ✅          |
 | settings set     |          ❌          |          ✅          |
 | settings clear   |          ❌          |          ✅          |
 | status           |          ❌          |          ✅          |
 | sync             |          ❌          |          ✅          |
-| token            |          ❌          |          ✅          |
+| token            |          ✅          |          ✅          |
 | upload           |          ✅          |          ❌          |
 
 **Login**
 
 Some commands like `download` or `upload` will connect to OpenBIS instance. At that time, oBIS will
 use username configured in `.obis/config.json` and will ask for password whenever session expires or
 username changes.
@@ -245,30 +233,35 @@
 
 Options:
   -object_type, --object_type TEXT              
                                   Object type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
   -experiment, --experiment TEXT  Full experiment code
+  -object, --object TEXT          Object identification information, it can be permId or identifier
   -type, --type TEXT              Type code
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -property TEXT                  Property code
   -property-value TEXT            Property value
   -save, --save TEXT              Directory name to save results
+  -r, --recursive                 Search data recursively
 ```
 
 With `data_set search` command, obis connects to a configured OpenBIS instance and searches for all
-data sets that fulfill given filtering criteria.
-At least one filtering criteria must be specified. Search results can be downloaded by
-using `save` option.
+data sets that fulfill given filtering criteria or by using object identification string.
+At least one search option must be specified. 
+
+Search results can be downloaded into a file by using `save` option.
+
+Recursive option enables searching for datasets of children samples or datasets
 
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **download**
 
 ```
@@ -317,29 +310,34 @@
 obis object search [OPTIONS]
 
 Options:
   -type, --type TEXT              Type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
   -experiment, --experiment TEXT  Full experiment 
+  -object, --object TEXT          Object identification information, it can be permId or identifier
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -property TEXT                  Property code
   -property-value TEXT            Property value
   -save, --save TEXT              File name to save results in csv format
+  -r, --recursive                 Search data recursively
 ```
 
 With `object search` command, obis connects to a configured OpenBIS instance and searches for all
-objects/samples that fulfill given filtering criteria.
-At least one filtering criteria must be specified. Search results can be downloaded int a file by
-using `-save` option.
+objects/samples that fulfill given filtering criteria or by using object identification string.
+At least one search option must be specified. 
+
+Search results can be downloaded into a file by using `save` option.
+
+Recursive option enables searching for datasets of children samples or datasets
 
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **upload**
 
 ```
@@ -561,14 +559,15 @@
 ```
 
 Obis repository folders can be added or removed from openBIS. This can be useful when a repository
 was moved or copied without using the `move` or `copy` commands.
 
 **token**
 
+
 ```
 obis token get <session_name> [--validity-days] [--validity-weeks] [--validity-months]
 ```
 
 Gets or creates a new personal access token (PAT) and stores it in the obis configuration. If
 no `session_name` is provided or is not stored in the configuration, you'll be asked interactively.
 If no validity period is provided, the maximum (configured by the server) is used. If a PAT with
@@ -613,23 +612,40 @@
 cd analysis1
 obis data_set set type=UNKNOWN
 obis object set id=/DEFAULT/DEFAULT
 echo content >> example_file
 obis commit -m 'message'
 ```
 
-## 6. Big Data Link Services
+## 6. Authentication
+
+There are 2 ways to perform user authentication against OpenBIS.
+
+### 6.1. Login
+Obis, internally, stores a session token which is used to connect with OpenBIS. Whenever this token 
+is invalidated, obis will ask user to provide credentials to log into OpenBIS again.   
+
+
+### 6.2. Personal Access Token
+Session token is short-lived and its interactive generation makes it unfeasible for usage in automatic 
+scripts. An alternative way to authorize is to generate personal access token (PAT), which can be 
+configured to last for a long periods of time.
+
+PAT generation is explained in depth in `token` command section.
+
+
+## 7. Big Data Link Services
 
 The Big Data Link Services can be used to download files which are contained in an obis repository.
 The services are included in the installation folder of openBIS,
 under `servers/big_data_link_services`. For how to configure and run them, consult
 the [README.md](https://sissource.ethz.ch/sispub/openbis/blob/master/big_data_link_server/README.md)
 file.
 
-## 7. Rationale for obis
+## 8. Rationale for obis
 
 Data-provenance tracking tools like openBIS make it possible to understand and follow the research
 process. What was studied, what data was acquired and how, how was data analyzed to arrive at final
 results for publication -- this is information that is captured in openBIS. In the standard usage
 scenario, openBIS stores and manages data directly. This has the advantage that openBIS acts as a
 gatekeeper to the data, making it easy to keep backups or enforce access restrictions, etc. However,
 this way of working is not a good solution for all situations.
@@ -650,13 +666,13 @@
 
 Under the covers, `obis` takes advantage of publicly available and tested tools to manage data on
 the file system. In particular, it uses `git` and `git-annex` to track the content of a dataset.
 Using `git-annex`, even large binary artifacts can be tracked efficiently. For communication with
 openBIS, `obis` uses the openBIS API, which offers the power to register and track all metadata
 supported by openBIS.
 
-## 8. Literature
+## 9. Literature
 
 V. Korolev, A. Joshi, V. Korolev, M.A. Grasso, A. Joshi, M.A. Grasso, et al., "PROB: A tool for
 tracking provenance and reproducibility of big data experiments", Reproduce '14. HPCA 2014, vol. 11,
 pp. 264-286, 2014.
 http://ebiquity.umbc.edu/_file_directory_/papers/693.pdf
```

### Comparing `obis-0.4.1/README.md` & `obis-0.4.2rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: obis
+Version: 0.4.2rc1
+Summary: Local data management with assistance from OpenBIS.
+Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
+Author: ID SIS • ETH Zürich
+Author-email: openbis-support@id.ethz.ch
+License: Apache Software License Version 2.0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # openBIS Command Line Tool (oBIS)
 
 oBIS is a command-line tool that makes it possible to handle data sets tracked by OpenBIS,
 where users have complete freedom to structure and manipulate the data as they wish, while retaining
 the benefits of openBIS.
 
 With oBIS, it is possible not only to handle datasets stored in OpenBIS but also available to keep
@@ -18,17 +33,20 @@
     1. [Standard Data Store](#51-standard-data-store)
         1. [Commands](#511-commands)
         2. [Examples](#512-examples)
     2. [External Data Store](#52-external-data-store)
         1. [Settings](#521-settings)
         2. [Commands](#522-commands)
         3. [Examples](#523-examples)
-6. [Big Data Link Services](#6-big-data-link-services)
-7. [Rationale for obis](#7-rationale-for-obis)
-8. [Literature](#8-literature)
+6. [Authentication](#6-authentication)
+   1. [Login](#61-login)
+   2. [Personal Access Token](#62-personal-access-token)
+7. [Big Data Link Services](#7-big-data-link-services)
+8. [Rationale for obis](#8-rationale-for-obis)
+9. [Literature](#9-literature)
 
 ## 1. Prerequisites
 
 - python 3.6 or higher
 - git 2.11 or higher
 - git-annex 6 or higher [Installation guide](https://git-annex.branchable.com/install/)
 
@@ -162,15 +180,15 @@
 | repository set   |          ❌          |          ✅          |
 | repository clear |          ❌          |          ✅          |
 | settings get     |          ❌          |          ✅          |
 | settings set     |          ❌          |          ✅          |
 | settings clear   |          ❌          |          ✅          |
 | status           |          ❌          |          ✅          |
 | sync             |          ❌          |          ✅          |
-| token            |          ❌          |          ✅          |
+| token            |          ✅          |          ✅          |
 | upload           |          ✅          |          ❌          |
 
 **Login**
 
 Some commands like `download` or `upload` will connect to OpenBIS instance. At that time, oBIS will
 use username configured in `.obis/config.json` and will ask for password whenever session expires or
 username changes.
@@ -230,30 +248,35 @@
 
 Options:
   -object_type, --object_type TEXT              
                                   Object type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
   -experiment, --experiment TEXT  Full experiment code
+  -object, --object TEXT          Object identification information, it can be permId or identifier
   -type, --type TEXT              Type code
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -property TEXT                  Property code
   -property-value TEXT            Property value
   -save, --save TEXT              Directory name to save results
+  -r, --recursive                 Search data recursively
 ```
 
 With `data_set search` command, obis connects to a configured OpenBIS instance and searches for all
-data sets that fulfill given filtering criteria.
-At least one filtering criteria must be specified. Search results can be downloaded by
-using `save` option.
+data sets that fulfill given filtering criteria or by using object identification string.
+At least one search option must be specified. 
+
+Search results can be downloaded into a file by using `save` option.
+
+Recursive option enables searching for datasets of children samples or datasets
 
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **download**
 
 ```
@@ -302,29 +325,34 @@
 obis object search [OPTIONS]
 
 Options:
   -type, --type TEXT              Type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
   -experiment, --experiment TEXT  Full experiment 
+  -object, --object TEXT          Object identification information, it can be permId or identifier
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -property TEXT                  Property code
   -property-value TEXT            Property value
   -save, --save TEXT              File name to save results in csv format
+  -r, --recursive                 Search data recursively
 ```
 
 With `object search` command, obis connects to a configured OpenBIS instance and searches for all
-objects/samples that fulfill given filtering criteria.
-At least one filtering criteria must be specified. Search results can be downloaded int a file by
-using `-save` option.
+objects/samples that fulfill given filtering criteria or by using object identification string.
+At least one search option must be specified. 
+
+Search results can be downloaded into a file by using `save` option.
+
+Recursive option enables searching for datasets of children samples or datasets
 
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **upload**
 
 ```
@@ -546,14 +574,15 @@
 ```
 
 Obis repository folders can be added or removed from openBIS. This can be useful when a repository
 was moved or copied without using the `move` or `copy` commands.
 
 **token**
 
+
 ```
 obis token get <session_name> [--validity-days] [--validity-weeks] [--validity-months]
 ```
 
 Gets or creates a new personal access token (PAT) and stores it in the obis configuration. If
 no `session_name` is provided or is not stored in the configuration, you'll be asked interactively.
 If no validity period is provided, the maximum (configured by the server) is used. If a PAT with
@@ -598,23 +627,40 @@
 cd analysis1
 obis data_set set type=UNKNOWN
 obis object set id=/DEFAULT/DEFAULT
 echo content >> example_file
 obis commit -m 'message'
 ```
 
-## 6. Big Data Link Services
+## 6. Authentication
+
+There are 2 ways to perform user authentication against OpenBIS.
+
+### 6.1. Login
+Obis, internally, stores a session token which is used to connect with OpenBIS. Whenever this token 
+is invalidated, obis will ask user to provide credentials to log into OpenBIS again.   
+
+
+### 6.2. Personal Access Token
+Session token is short-lived and its interactive generation makes it unfeasible for usage in automatic 
+scripts. An alternative way to authorize is to generate personal access token (PAT), which can be 
+configured to last for a long periods of time.
+
+PAT generation is explained in depth in `token` command section.
+
+
+## 7. Big Data Link Services
 
 The Big Data Link Services can be used to download files which are contained in an obis repository.
 The services are included in the installation folder of openBIS,
 under `servers/big_data_link_services`. For how to configure and run them, consult
 the [README.md](https://sissource.ethz.ch/sispub/openbis/blob/master/big_data_link_server/README.md)
 file.
 
-## 7. Rationale for obis
+## 8. Rationale for obis
 
 Data-provenance tracking tools like openBIS make it possible to understand and follow the research
 process. What was studied, what data was acquired and how, how was data analyzed to arrive at final
 results for publication -- this is information that is captured in openBIS. In the standard usage
 scenario, openBIS stores and manages data directly. This has the advantage that openBIS acts as a
 gatekeeper to the data, making it easy to keep backups or enforce access restrictions, etc. However,
 this way of working is not a good solution for all situations.
@@ -635,13 +681,13 @@
 
 Under the covers, `obis` takes advantage of publicly available and tested tools to manage data on
 the file system. In particular, it uses `git` and `git-annex` to track the content of a dataset.
 Using `git-annex`, even large binary artifacts can be tracked efficiently. For communication with
 openBIS, `obis` uses the openBIS API, which offers the power to register and track all metadata
 supported by openBIS.
 
-## 8. Literature
+## 9. Literature
 
 V. Korolev, A. Joshi, V. Korolev, M.A. Grasso, A. Joshi, M.A. Grasso, et al., "PROB: A tool for
 tracking provenance and reproducibility of big data experiments", Reproduce '14. HPCA 2014, vol. 11,
 pp. 264-286, 2014.
 http://ebiquity.umbc.edu/_file_directory_/papers/693.pdf
```

### Comparing `obis-0.4.1/man/man1/obis-addref.1` & `obis-0.4.2rc1/man/man1/obis-addref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-clone.1` & `obis-0.4.2rc1/man/man1/obis-clone.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-collection.1` & `obis-0.4.2rc1/man/man1/obis-collection.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-commit.1` & `obis-0.4.2rc1/man/man1/obis-commit.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-config.1` & `obis-0.4.2rc1/man/man1/obis-config.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-data_set.1` & `obis-0.4.2rc1/man/man1/obis-data_set.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-download.1` & `obis-0.4.2rc1/man/man1/obis-download.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-init.1` & `obis-0.4.2rc1/man/man1/obis-init.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-init_analysis.1` & `obis-0.4.2rc1/man/man1/obis-init_analysis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-move.1` & `obis-0.4.2rc1/man/man1/obis-move.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-object.1` & `obis-0.4.2rc1/man/man1/obis-object.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-removeref.1` & `obis-0.4.2rc1/man/man1/obis-removeref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-repository.1` & `obis-0.4.2rc1/man/man1/obis-repository.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-settings.1` & `obis-0.4.2rc1/man/man1/obis-settings.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-status.1` & `obis-0.4.2rc1/man/man1/obis-status.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis-sync.1` & `obis-0.4.2rc1/man/man1/obis-sync.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/man/man1/obis.1` & `obis-0.4.2rc1/man/man1/obis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/__init__.py` & `obis-0.4.2rc1/obis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 __author__ = "ID SIS • ETH Zürich"
 __email__ = "openbis-support@id.ethz.ch"
-__version__ = "0.4.1"
+__version__ = "0.4.2rc1"
 
 from .dm import *
```

### Comparing `obis-0.4.1/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc1/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/conftest.py` & `obis-0.4.2rc1/obis/conftest.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__init__.py` & `obis-0.4.2rc1/obis/dm/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/checksum.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/checksum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/command_log.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/command_log.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/command_result.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/command_result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/config.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/data_mgmt.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/data_mgmt.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar  3 10:44:27 2023 UTC, .py size: 27633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8bcf 0164 f16b 0000  o..........d.k..
+00000000: 6f0d 0d0a 0000 0000 ff8e 2564 316d 0000  o.........%d1m..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6401 6c08  d.l.m.Z...d.d.l.
 00000070: 5a08 6403 6404 6c09 6d0a 5a0b 0100 6403  Z.d.d.l.m.Z...d.
@@ -44,1391 +44,1403 @@
 000002b0: da13 636f 6d70 6c65 7465 5f67 6974 5f63  ..complete_git_c
 000002c0: 6f6e 6669 6729 01da 1763 6f6d 706c 6574  onfig)...complet
 000002d0: 655f 6f70 656e 6269 735f 636f 6e66 6967  e_openbis_config
 000002e0: 2901 da0c 6465 6661 756c 745f 6563 686f  )...default_echo
 000002f0: e902 0000 0029 02da 0a63 6c69 636b 5f65  .....)...click_e
 00000300: 6368 6fda 0c63 6865 636b 5f72 6573 756c  cho..check_resul
 00000310: 7446 5463 0900 0000 0000 0000 0000 0000  tFTc............
-00000320: 0e00 0000 0b00 0000 4300 0000 73f2 0000  ........C...s...
+00000320: 0e00 0000 0b00 0000 4300 0000 73fc 0000  ........C...s...
 00000330: 007c 0064 0175 0172 067c 006e 0174 007d  .|.d.u.r.|.n.t.}
 00000340: 007c 0364 0219 007d 097c 0364 0319 007d  .|.d...}.|.d...}
 00000350: 0a7c 0364 0419 007d 0b7c 0164 0175 0072  .|.d...}.|.d.u.r
 00000360: 1c74 01a0 02a1 007d 017c 0874 036a 046b  .t.....}.|.t.j.k
 00000370: 0272 3d74 056a 06a0 0764 05a1 0172 3a7c  .r=t.j...d...r:|
 00000380: 016a 08a0 09a1 007d 0c7c 0c64 0619 0064  .j.....}.|.d...d
 00000390: 0775 0072 3674 036a 0a7d 086e 0774 036a  .u.r6t.j.}.n.t.j
 000003a0: 0b7d 086e 0374 036a 0b7d 087c 0874 036a  .}.n.t.j.}.|.t.j
-000003b0: 0a6b 0272 4d74 0c7c 0164 0164 017c 047c  .k.rMt.|.d.d.|.|
-000003c0: 057c 097c 0a7c 0b83 0853 0074 0d7c 0383  .|.|.|...S.t.|..
-000003d0: 0101 0074 0e64 0869 007c 03a4 018e 017d  ...t.d.i.|.....}
-000003e0: 0d7c 0da0 0fa1 0073 6774 107c 0164 017c  .|.....sgt.|.d.|
-000003f0: 0d7c 047c 057c 097c 0a7c 0b83 0853 0074  .|.|.|.|.|...S.t
-00000400: 117c 027c 0183 0201 0074 127c 017c 027c  .|.|.....t.|.|.|
-00000410: 0d7c 047c 057c 097c 0a7c 0b7c 067c 0783  .|.|.|.|.|.|.|..
-00000420: 0a53 0029 097a 2546 6163 746f 7279 206d  .S.).z%Factory m
-00000430: 6574 686f 6420 666f 7220 4461 7461 4d67  ethod for DataMg
-00000440: 6d74 2069 6e73 7461 6e63 6573 4eda 0964  mt instancesN..d
-00000450: 6174 615f 7061 7468 da0d 6d65 7461 6461  ata_path..metada
-00000460: 7461 5f70 6174 68da 0f69 6e76 6f63 6174  ta_path..invocat
-00000470: 696f 6e5f 7061 7468 fa05 2e6f 6269 73da  ion_path...obis.
-00000480: 0b69 735f 7068 7973 6963 616c 54a9 0029  .is_physicalT..)
-00000490: 1372 1600 0000 da09 646d 5f63 6f6e 6669  .r......dm_confi
-000004a0: 67da 1053 6574 7469 6e67 7352 6573 6f6c  g..SettingsResol
-000004b0: 7665 7272 1100 0000 da07 554e 4b4e 4f57  verr......UNKNOW
-000004c0: 4eda 026f 73da 0470 6174 68da 0665 7869  N..os..path..exi
-000004d0: 7374 7372 0400 0000 da0b 636f 6e66 6967  stsr......config
-000004e0: 5f64 6963 74da 0850 4859 5349 4341 4cda  _dict..PHYSICAL.
-000004f0: 044c 494e 4bda 1050 6879 7369 6361 6c44  .LINK..PhysicalD
-00000500: 6174 614d 676d 7472 1400 0000 7210 0000  ataMgmtr....r...
-00000510: 00da 0763 616e 5f72 756e da0d 4e6f 4769  ...can_run..NoGi
-00000520: 7444 6174 614d 676d 7472 1500 0000 da0b  tDataMgmtr......
-00000530: 4769 7444 6174 614d 676d 7429 0eda 0965  GitDataMgmt)...e
-00000540: 6368 6f5f 6675 6e63 da11 7365 7474 696e  cho_func..settin
-00000550: 6773 5f72 6573 6f6c 7665 72da 0e6f 7065  gs_resolver..ope
-00000560: 6e62 6973 5f63 6f6e 6669 67da 0a67 6974  nbis_config..git
-00000570: 5f63 6f6e 6669 67da 076f 7065 6e62 6973  _config..openbis
-00000580: da03 6c6f 67da 0564 6562 7567 da05 6c6f  ..log..debug..lo
-00000590: 6769 6eda 0f72 6570 6f73 6974 6f72 795f  gin..repository_
-000005a0: 7479 7065 721a 0000 0072 1b00 0000 721c  typer....r....r.
-000005b0: 0000 0072 2600 0000 da0b 6769 745f 7772  ...r&.....git_wr
-000005c0: 6170 7065 7272 1f00 0000 721f 0000 00fa  apperr....r.....
-000005d0: 5d2f 686f 6d65 2f61 6c61 736b 6f77 736b  ]/home/alaskowsk
-000005e0: 692f 7265 706f 2f6f 7065 6e62 6973 5f70  i/repo/openbis_p
-000005f0: 7974 686f 6e2f 6170 702d 6f70 656e 6269  ython/app-openbi
-00000600: 732d 636f 6d6d 616e 642d 6c69 6e65 2f73  s-command-line/s
-00000610: 7263 2f70 7974 686f 6e2f 6f62 6973 2f64  rc/python/obis/d
-00000620: 6d2f 6461 7461 5f6d 676d 742e 7079 da08  m/data_mgmt.py..
-00000630: 4461 7461 4d67 6d74 3200 0000 7336 0000  DataMgmt2...s6..
-00000640: 0010 0408 0208 0108 0108 0208 010a 020c  ................
-00000650: 010a 010c 0108 0108 0206 020a 020e 0104  ................
-00000660: 0104 ff08 030e 0108 010e 0304 0104 ff0a  ................
-00000670: 030e 0108 0104 ff72 3800 0000 6300 0000  .......r8...c...
-00000680: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00000690: 0040 0000 0073 1a01 0000 6500 5a01 6400  .@...s....e.Z.d.
-000006a0: 5a02 6401 5a03 0903 642b 6404 6405 8401  Z.d.Z...d+d.d...
-000006b0: 5a04 6406 6407 8400 5a05 6506 6a07 6408  Z.d.d...Z.e.j.d.
-000006c0: 6409 8400 8301 5a08 6506 6a07 640a 640b  d.....Z.e.j.d.d.
-000006d0: 8400 8301 5a09 6506 6a07 642c 640d 640e  ....Z.e.j.d,d.d.
-000006e0: 8401 8301 5a0a 6506 6a07 642c 640f 6410  ....Z.e.j.d,d.d.
-000006f0: 8401 8301 5a0b 6506 6a07 642d 6411 6412  ....Z.e.j.d-d.d.
-00000700: 8401 8301 5a0c 6506 6a07 6413 6414 8400  ....Z.e.j.d.d...
-00000710: 8301 5a0d 6506 6a07 6415 6416 8400 8301  ..Z.e.j.d.d.....
-00000720: 5a0e 6506 6a07 6417 6418 8400 8301 5a0f  Z.e.j.d.d.....Z.
-00000730: 6506 6a07 6419 641a 8400 8301 5a10 6506  e.j.d.d.....Z.e.
-00000740: 6a07 641b 641c 8400 8301 5a11 6506 6a07  j.d.d.....Z.e.j.
-00000750: 642c 641d 641e 8401 8301 5a12 6506 6a07  d,d.d.....Z.e.j.
-00000760: 641f 6420 8400 8301 5a13 6506 6a07 6421  d.d ....Z.e.j.d!
-00000770: 6422 8400 8301 5a14 6506 6a07 6423 6424  d"....Z.e.j.d#d$
-00000780: 8400 8301 5a15 6506 6a07 6425 6426 8400  ....Z.e.j.d%d&..
-00000790: 8301 5a16 090c 090c 642e 6427 6428 8401  ..Z.....d.d'd(..
-000007a0: 5a17 6518 642f 6429 642a 8401 8301 5a19  Z.e.d/d)d*....Z.
-000007b0: 640c 5300 2930 da10 4162 7374 7261 6374  d.S.)0..Abstract
-000007c0: 4461 7461 4d67 6d74 7a65 4162 7374 7261  DataMgmtzeAbstra
-000007d0: 6374 206f 626a 6563 7420 7468 6174 2069  ct object that i
-000007e0: 6d70 6c65 6d65 6e74 7320 6f70 6572 6174  mplements operat
-000007f0: 696f 6e73 2e0a 0a20 2020 2041 6c6c 206f  ions...    All o
-00000800: 7065 7261 7469 6f6e 7320 7468 726f 7720  perations throw 
-00000810: 616e 2065 7865 7063 7469 6f6e 2069 6620  an exepction if 
-00000820: 7468 6579 2066 6169 6c2e 0a20 2020 2046  they fail..    F
-00000830: 5463 0b00 0000 0000 0000 0000 0000 0b00  Tc..............
-00000840: 0000 0200 0000 4300 0000 734c 0000 007c  ......C...sL...|
-00000850: 017c 005f 007c 027c 005f 017c 037c 005f  .|._.|.|._.|.|._
-00000860: 027c 047c 005f 037c 057c 005f 047c 067c  .|.|._.|.|._.|.|
-00000870: 005f 057c 077c 005f 067c 087c 005f 077c  ._.|.|._.|.|._.|
-00000880: 097c 005f 087c 0a7c 005f 0964 017c 005f  .|._.|.|._.d.|._
-00000890: 0a64 027c 005f 0b64 0053 0029 034e 5446  .d.|._.d.S.).NTF
-000008a0: 290c 722e 0000 0072 2f00 0000 7236 0000  ).r....r/...r6..
-000008b0: 0072 3100 0000 7232 0000 0072 1a00 0000  .r1...r2...r....
-000008c0: 721b 0000 0072 1c00 0000 7233 0000 0072  r....r....r3...r
-000008d0: 3400 0000 da11 7265 7374 6f72 655f 6f6e  4.....restore_on
-000008e0: 5f73 6967 696e 74da 1569 676e 6f72 655f  _sigint..ignore_
-000008f0: 6d69 7373 696e 675f 7061 7265 6e74 290b  missing_parent).
-00000900: da04 7365 6c66 722e 0000 0072 2f00 0000  ..selfr....r/...
-00000910: 7236 0000 0072 3100 0000 7232 0000 0072  r6...r1...r2...r
-00000920: 1a00 0000 721b 0000 0072 1c00 0000 7233  ....r....r....r3
-00000930: 0000 0072 3400 0000 721f 0000 0072 1f00  ...r4...r....r..
-00000940: 0000 7237 0000 00da 085f 5f69 6e69 745f  ..r7.....__init_
-00000950: 5f60 0000 0073 1800 0000 0602 0601 0601  _`...s..........
-00000960: 0601 0601 0601 0601 0601 0601 0601 0603  ................
-00000970: 0a01 7a19 4162 7374 7261 6374 4461 7461  ..z.AbstractData
-00000980: 4d67 6d74 2e5f 5f69 6e69 745f 5f63 0300  Mgmt.__init__c..
-00000990: 0000 0000 0000 0000 0000 0400 0000 0400  ................
-000009a0: 0000 4300 0000 7314 0000 0064 01a0 007c  ..C...s....d...|
-000009b0: 017c 02a1 027d 0374 017c 0383 0182 0129  .|...}.t.|.....)
-000009c0: 027a 1352 6169 7365 2061 6e20 6578 6365  .z.Raise an exce
-000009d0: 7074 696f 6e2e 7a0f 277b 7d27 2066 6169  ption.z.'{}' fai
-000009e0: 6c65 642e 207b 7d29 02da 0666 6f72 6d61  led. {})...forma
-000009f0: 74da 0a56 616c 7565 4572 726f 7229 0472  t..ValueError).r
-00000a00: 3c00 0000 da07 636f 6d6d 616e 64da 0672  <.....command..r
-00000a10: 6561 736f 6eda 076d 6573 7361 6765 721f  eason..messager.
-00000a20: 0000 0072 1f00 0000 7237 0000 00da 0b65  ...r....r7.....e
-00000a30: 7272 6f72 5f72 6169 7365 7100 0000 7304  rror_raiseq...s.
-00000a40: 0000 000c 0208 017a 1c41 6273 7472 6163  .......z.Abstrac
-00000a50: 7444 6174 614d 676d 742e 6572 726f 725f  tDataMgmt.error_
-00000a60: 7261 6973 6563 0100 0000 0000 0000 0000  raisec..........
-00000a70: 0000 0100 0000 0100 0000 4300 0000 f304  ..........C.....
-00000a80: 0000 0064 0153 0029 027a 1b20 4765 7420  ...d.S.).z. Get 
-00000a90: 7468 6520 7365 7474 696e 6773 2072 6573  the settings res
-00000aa0: 6f6c 7665 7220 4e72 1f00 0000 a901 723c  olver Nr......r<
-00000ab0: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
-00000ac0: 0000 da15 6765 745f 7365 7474 696e 6773  ....get_settings
-00000ad0: 5f72 6573 6f6c 7665 7276 0000 00f3 0200  _resolverv......
-00000ae0: 0000 0403 7a26 4162 7374 7261 6374 4461  ....z&AbstractDa
-00000af0: 7461 4d67 6d74 2e67 6574 5f73 6574 7469  taMgmt.get_setti
-00000b00: 6e67 735f 7265 736f 6c76 6572 6302 0000  ngs_resolverc...
-00000b10: 0000 0000 0000 0000 0002 0000 0001 0000  ................
-00000b20: 0043 0000 0072 4400 0000 2902 7a34 2053  .C...rD...).z4 S
-00000b30: 6574 7570 206c 6f63 616c 2073 6574 7469  etup local setti
-00000b40: 6e67 7320 2d20 666f 7220 7573 696e 6720  ngs - for using 
-00000b50: 6f62 6973 2061 7320 6120 6c69 6272 6172  obis as a librar
-00000b60: 7920 4e72 1f00 0000 a902 723c 0000 00da  y Nr......r<....
-00000b70: 0c61 6c6c 5f73 6574 7469 6e67 7372 1f00  .all_settingsr..
-00000b80: 0000 721f 0000 0072 3700 0000 da14 7365  ..r....r7.....se
-00000b90: 7475 705f 6c6f 6361 6c5f 7365 7474 696e  tup_local_settin
-00000ba0: 6773 7b00 0000 7247 0000 007a 2541 6273  gs{...rG...z%Abs
-00000bb0: 7472 6163 7444 6174 614d 676d 742e 7365  tractDataMgmt.se
-00000bc0: 7475 705f 6c6f 6361 6c5f 7365 7474 696e  tup_local_settin
-00000bd0: 6773 4e63 0200 0000 0000 0000 0000 0000  gsNc............
-00000be0: 0200 0000 0100 0000 4300 0000 7244 0000  ........C...rD..
-00000bf0: 0029 0261 4b01 0000 496e 6974 6961 6c69  .).aK...Initiali
-00000c00: 7a65 2061 2064 6174 6120 7265 706f 7369  ze a data reposi
-00000c10: 746f 7279 2061 7420 7468 6520 7061 7468  tory at the path
-00000c20: 2077 6974 6820 7468 6520 6465 7363 7269   with the descri
-00000c30: 7074 696f 6e2e 0a20 2020 2020 2020 203a  ption..        :
-00000c40: 7061 7261 6d20 7061 7468 3a20 5061 7468  param path: Path
-00000c50: 2066 6f72 2074 6865 2072 6570 6f73 6974   for the reposit
-00000c60: 6f72 792e 0a20 2020 2020 2020 203a 7061  ory..        :pa
-00000c70: 7261 6d20 6465 7363 3a20 416e 206f 7074  ram desc: An opt
-00000c80: 696f 6e61 6c20 7368 6f72 7420 6465 7363  ional short desc
-00000c90: 7269 7074 696f 6e20 6f66 2074 6865 2072  ription of the r
-00000ca0: 6570 6f73 6974 6f72 7920 2875 7365 6420  epository (used 
-00000cb0: 6279 2067 6974 2d61 6e6e 6578 290a 2020  by git-annex).  
-00000cc0: 2020 2020 2020 3a70 6172 616d 2063 7265        :param cre
-00000cd0: 6174 653a 2049 6620 5472 7565 2061 6e64  ate: If True and
-00000ce0: 2074 6865 2066 6f6c 6465 7220 646f 6573   the folder does
-00000cf0: 206e 6f74 2065 7869 7374 2c20 6372 6561   not exist, crea
-00000d00: 7465 2069 742e 2044 6566 6175 6c74 7320  te it. Defaults 
-00000d10: 746f 2074 7275 652e 0a20 2020 2020 2020  to true..       
-00000d20: 203a 7265 7475 726e 3a20 4120 436f 6d6d   :return: A Comm
-00000d30: 616e 6452 6573 756c 742e 0a20 2020 2020  andResult..     
-00000d40: 2020 204e 721f 0000 00a9 0272 3c00 0000     Nr......r<...
-00000d50: da04 6465 7363 721f 0000 0072 1f00 0000  ..descr....r....
-00000d60: 7237 0000 00da 0969 6e69 745f 6461 7461  r7.....init_data
-00000d70: 8000 0000 f302 0000 0004 087a 1a41 6273  ...........z.Abs
-00000d80: 7472 6163 7444 6174 614d 676d 742e 696e  tractDataMgmt.in
-00000d90: 6974 5f64 6174 6163 0300 0000 0000 0000  it_datac........
-00000da0: 0000 0000 0300 0000 0100 0000 4300 0000  ............C...
-00000db0: 7244 0000 0029 027a f549 6e69 7469 616c  rD...).z.Initial
-00000dc0: 697a 6520 616e 2061 6e61 6c79 7369 7320  ize an analysis 
-00000dd0: 7265 706f 7369 746f 7279 2061 7420 7468  repository at th
-00000de0: 6520 7061 7468 2e0a 2020 2020 2020 2020  e path..        
-00000df0: 3a70 6172 616d 2070 6172 656e 745f 666f  :param parent_fo
-00000e00: 6c64 6572 3a20 5061 7468 2066 6f72 2074  lder: Path for t
-00000e10: 6865 2072 6570 6f73 6974 6f72 792e 0a20  he repository.. 
-00000e20: 2020 2020 2020 203a 7061 7261 6d20 7061         :param pa
-00000e30: 7265 6e74 3a20 2872 6571 7569 7265 6420  rent: (required 
-00000e40: 7768 656e 206f 7574 7369 6465 206f 6620  when outside of 
-00000e50: 6578 6973 7469 6e67 2072 6570 6f73 6974  existing reposit
-00000e60: 6f72 7929 2050 6174 6820 666f 7220 7468  ory) Path for th
-00000e70: 6520 7061 7265 6e74 2072 6570 6f73 6974  e parent reposit
-00000e80: 6f72 740a 2020 2020 2020 2020 3a72 6574  ort.        :ret
-00000e90: 7572 6e3a 2041 2043 6f6d 6d61 6e64 5265  urn: A CommandRe
-00000ea0: 7375 6c74 2e0a 2020 2020 2020 2020 4e72  sult..        Nr
-00000eb0: 1f00 0000 a903 723c 0000 00da 0d70 6172  ......r<.....par
-00000ec0: 656e 745f 666f 6c64 6572 724c 0000 0072  ent_folderrL...r
-00000ed0: 1f00 0000 721f 0000 0072 3700 0000 da0d  ....r....r7.....
-00000ee0: 696e 6974 5f61 6e61 6c79 7369 738a 0000  init_analysis...
-00000ef0: 00f3 0200 0000 0407 7a1e 4162 7374 7261  ........z.Abstra
-00000f00: 6374 4461 7461 4d67 6d74 2e69 6e69 745f  ctDataMgmt.init_
-00000f10: 616e 616c 7973 6973 6304 0000 0000 0000  analysisc.......
-00000f20: 0000 0000 0004 0000 0001 0000 0043 0000  .............C..
-00000f30: 0072 4400 0000 2902 615e 0100 0043 6f6d  .rD...).a^...Com
-00000f40: 6d69 7420 7468 6520 6375 7272 656e 7420  mit the current 
-00000f50: 7265 706f 2e0a 0a20 2020 2020 2020 2054  repo...        T
-00000f60: 6869 7320 6973 7375 6573 2061 2067 6974  his issues a git
-00000f70: 2063 6f6d 6d69 7420 616e 6420 636f 6e6e   commit and conn
-00000f80: 6563 7473 2074 6f20 6f70 656e 4249 5320  ects to openBIS 
-00000f90: 616e 6420 6372 6561 7465 7320 6120 6461  and creates a da
-00000fa0: 7461 2073 6574 2069 6e20 6f70 656e 4249  ta set in openBI
-00000fb0: 532e 0a20 2020 2020 2020 203a 7061 7261  S..        :para
-00000fc0: 6d20 6d73 673a 2043 6f6d 6d69 7420 6d65  m msg: Commit me
-00000fd0: 7373 6167 652e 0a20 2020 2020 2020 203a  ssage..        :
-00000fe0: 7061 7261 6d20 6175 746f 5f61 6464 3a20  param auto_add: 
-00000ff0: 4175 746f 6d61 7469 6361 6c6c 7920 6164  Automatically ad
-00001000: 6420 616c 6c20 6669 6c65 7320 696e 2074  d all files in t
-00001010: 6865 2066 6f6c 6465 7220 746f 2074 6865  he folder to the
-00001020: 2072 6570 6f2e 2044 6566 6175 6c74 7320   repo. Defaults 
-00001030: 746f 2054 7275 652e 0a20 2020 2020 2020  to True..       
-00001040: 203a 7061 7261 6d20 7379 6e63 3a20 4966   :param sync: If
-00001050: 2074 7275 652c 2073 796e 6320 7769 7468   true, sync with
-00001060: 206f 7065 6e42 4953 2073 6572 7665 722e   openBIS server.
-00001070: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00001080: 3a20 4120 436f 6d6d 616e 6452 6573 756c  : A CommandResul
-00001090: 742e 0a20 2020 2020 2020 204e 721f 0000  t..        Nr...
-000010a0: 00a9 0472 3c00 0000 da03 6d73 67da 0861  ...r<.....msg..a
-000010b0: 7574 6f5f 6164 64da 0473 796e 6372 1f00  uto_add..syncr..
-000010c0: 0000 721f 0000 0072 3700 0000 da06 636f  ..r....r7.....co
-000010d0: 6d6d 6974 9300 0000 7302 0000 0004 0a7a  mmit....s......z
-000010e0: 1741 6273 7472 6163 7444 6174 614d 676d  .AbstractDataMgm
-000010f0: 742e 636f 6d6d 6974 6301 0000 0000 0000  t.commitc.......
-00001100: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
-00001110: 0072 4400 0000 2902 7a86 5379 6e63 2074  .rD...).z.Sync t
-00001120: 6865 2063 7572 7265 6e74 2072 6570 6f2e  he current repo.
-00001130: 0a0a 2020 2020 2020 2020 5468 6973 2063  ..        This c
-00001140: 6f6e 6e65 6374 7320 746f 206f 7065 6e42  onnects to openB
-00001150: 4953 2061 6e64 2063 7265 6174 6573 2061  IS and creates a
-00001160: 2064 6174 6120 7365 7420 696e 206f 7065   data set in ope
-00001170: 6e42 4953 2e0a 2020 2020 2020 2020 3a72  nBIS..        :r
-00001180: 6574 7572 6e3a 2041 2043 6f6d 6d61 6e64  eturn: A Command
-00001190: 5265 7375 6c74 2e0a 2020 2020 2020 2020  Result..        
-000011a0: 4e72 1f00 0000 7245 0000 0072 1f00 0000  Nr....rE...r....
-000011b0: 721f 0000 0072 3700 0000 7256 0000 009f  r....r7...rV....
-000011c0: 0000 0072 5200 0000 7a15 4162 7374 7261  ...rR...z.Abstra
-000011d0: 6374 4461 7461 4d67 6d74 2e73 796e 6363  ctDataMgmt.syncc
-000011e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000011f0: 0100 0000 4300 0000 7244 0000 0029 027a  ....C...rD...).z
-00001200: 5752 6574 7572 6e20 7468 6520 7374 6174  WReturn the stat
-00001210: 7573 206f 6620 7468 6520 6375 7272 656e  us of the curren
-00001220: 7420 7265 706f 7369 746f 7279 2e0a 2020  t repository..  
-00001230: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
-00001240: 2043 6f6d 6d61 6e64 5265 7375 6c74 2e0a   CommandResult..
-00001250: 2020 2020 2020 2020 4e72 1f00 0000 7245          Nr....rE
-00001260: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
-00001270: 0000 da06 7374 6174 7573 a800 0000 f302  ....status......
-00001280: 0000 0004 057a 1741 6273 7472 6163 7444  .....z.AbstractD
-00001290: 6174 614d 676d 742e 7374 6174 7573 6305  ataMgmt.statusc.
-000012a0: 0000 0000 0000 0000 0000 0005 0000 0001  ................
-000012b0: 0000 0043 0000 0072 4400 0000 2902 617d  ...C...rD...).a}
-000012c0: 0100 0043 6c6f 6e65 202f 2063 6f70 7920  ...Clone / copy 
-000012d0: 6120 7265 706f 7369 746f 7279 2072 656c  a repository rel
-000012e0: 6174 6564 2074 6f20 7468 6520 6769 7665  ated to the give
-000012f0: 6e20 6461 7461 2073 6574 2069 642e 0a20  n data set id.. 
-00001300: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
-00001310: 7461 5f73 6574 5f69 643a 200a 2020 2020  ta_set_id: .    
-00001320: 2020 2020 3a70 6172 616d 2073 7368 5f75      :param ssh_u
-00001330: 7365 723a 2073 7368 2075 7365 7220 666f  ser: ssh user fo
-00001340: 7220 7265 6d6f 7465 2073 7973 7465 6d20  r remote system 
-00001350: 286f 7074 696f 6e61 6c29 0a20 2020 2020  (optional).     
-00001360: 2020 203a 7061 7261 6d20 636f 6e74 656e     :param conten
-00001370: 745f 636f 7079 5f69 6e64 6578 3a20 696e  t_copy_index: in
-00001380: 6465 7820 6f66 2063 6f6e 7465 6e74 2063  dex of content c
-00001390: 6f70 7920 696e 2063 6173 6520 7468 6572  opy in case ther
-000013a0: 6520 6172 6520 6d75 6c74 6970 6c65 2063  e are multiple c
-000013b0: 6f70 6965 7320 286f 7074 696f 6e61 6c29  opies (optional)
-000013c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000013d0: 736b 6970 5f69 6e74 6567 7269 7479 5f63  skip_integrity_c
-000013e0: 6865 636b 3a20 6966 2074 7275 652c 2074  heck: if true, t
-000013f0: 6865 2066 696c 6520 6368 6563 6b73 756d  he file checksum
-00001400: 7320 7769 6c6c 206e 6f74 2062 6520 6368  s will not be ch
-00001410: 6563 6b65 640a 2020 2020 2020 2020 3a72  ecked.        :r
-00001420: 6574 7572 6e3a 2041 2043 6f6d 6d61 6e64  eturn: A Command
-00001430: 5265 7375 6c74 2e0a 2020 2020 2020 2020  Result..        
-00001440: 4e72 1f00 0000 a905 723c 0000 00da 0b64  Nr......r<.....d
-00001450: 6174 615f 7365 745f 6964 da08 7373 685f  ata_set_id..ssh_
-00001460: 7573 6572 da12 636f 6e74 656e 745f 636f  user..content_co
-00001470: 7079 5f69 6e64 6578 da14 736b 6970 5f69  py_index..skip_i
-00001480: 6e74 6567 7269 7479 5f63 6865 636b 721f  ntegrity_checkr.
-00001490: 0000 0072 1f00 0000 7237 0000 00da 0563  ...r....r7.....c
-000014a0: 6c6f 6e65 af00 0000 f302 0000 0004 097a  lone...........z
-000014b0: 1641 6273 7472 6163 7444 6174 614d 676d  .AbstractDataMgm
-000014c0: 742e 636c 6f6e 6563 0500 0000 0000 0000  t.clonec........
-000014d0: 0000 0000 0500 0000 0100 0000 4300 0000  ............C...
-000014e0: 7244 0000 0029 0261 7501 0000 4d6f 7665  rD...).au...Move
-000014f0: 2061 2072 6570 6f73 6974 6f72 7920 7265   a repository re
-00001500: 6c61 7465 6420 746f 2074 6865 2067 6976  lated to the giv
-00001510: 656e 2064 6174 6120 7365 7420 6964 2e0a  en data set id..
-00001520: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00001530: 6174 615f 7365 745f 6964 3a20 0a20 2020  ata_set_id: .   
-00001540: 2020 2020 203a 7061 7261 6d20 7373 685f       :param ssh_
-00001550: 7573 6572 3a20 7373 6820 7573 6572 2066  user: ssh user f
-00001560: 6f72 2072 656d 6f74 6520 7379 7374 656d  or remote system
-00001570: 2028 6f70 7469 6f6e 616c 290a 2020 2020   (optional).    
-00001580: 2020 2020 3a70 6172 616d 2063 6f6e 7465      :param conte
-00001590: 6e74 5f63 6f70 795f 696e 6465 783a 2069  nt_copy_index: i
-000015a0: 6e64 6578 206f 6620 636f 6e74 656e 7420  ndex of content 
-000015b0: 636f 7079 2069 6e20 6361 7365 2074 6865  copy in case the
-000015c0: 7265 2061 7265 206d 756c 7469 706c 6520  re are multiple 
-000015d0: 636f 7069 6573 2028 6f70 7469 6f6e 616c  copies (optional
-000015e0: 290a 2020 2020 2020 2020 3a70 6172 616d  ).        :param
-000015f0: 2073 6b69 705f 696e 7465 6772 6974 795f   skip_integrity_
-00001600: 6368 6563 6b3a 2069 6620 7472 7565 2c20  check: if true, 
-00001610: 7468 6520 6669 6c65 2063 6865 636b 7375  the file checksu
-00001620: 6d73 2077 696c 6c20 6e6f 7420 6265 2063  ms will not be c
-00001630: 6865 636b 6564 0a20 2020 2020 2020 203a  hecked.        :
-00001640: 7265 7475 726e 3a20 4120 436f 6d6d 616e  return: A Comman
-00001650: 6452 6573 756c 742e 0a20 2020 2020 2020  dResult..       
-00001660: 204e 721f 0000 0072 5a00 0000 721f 0000   Nr....rZ...r...
-00001670: 0072 1f00 0000 7237 0000 00da 046d 6f76  .r....r7.....mov
-00001680: 65ba 0000 0072 6000 0000 7a15 4162 7374  e....r`...z.Abst
-00001690: 7261 6374 4461 7461 4d67 6d74 2e6d 6f76  ractDataMgmt.mov
-000016a0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-000016b0: 0000 0100 0000 4300 0000 7244 0000 0029  ......C...rD...)
-000016c0: 027a 6341 6464 2074 6865 2063 7572 7265  .zcAdd the curre
-000016d0: 6e74 2066 6f6c 6465 7220 6173 2061 6e20  nt folder as an 
-000016e0: 6f62 6973 2072 6570 6f73 6974 6f72 7920  obis repository 
-000016f0: 746f 206f 7065 6e42 4953 2e0a 2020 2020  to openBIS..    
-00001700: 2020 2020 3a72 6574 7572 6e3a 2041 2043      :return: A C
-00001710: 6f6d 6d61 6e64 5265 7375 6c74 2e0a 2020  ommandResult..  
-00001720: 2020 2020 2020 4e72 1f00 0000 7245 0000        Nr....rE..
-00001730: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-00001740: da06 6164 6472 6566 c500 0000 7259 0000  ..addref....rY..
-00001750: 007a 1741 6273 7472 6163 7444 6174 614d  .z.AbstractDataM
-00001760: 676d 742e 6164 6472 6566 6302 0000 0000  gmt.addrefc.....
-00001770: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
-00001780: 0000 0072 4400 0000 2902 7ab4 5265 6d6f  ...rD...).z.Remo
-00001790: 7665 2074 6865 2063 7572 7265 6e74 2066  ve the current f
-000017a0: 6f6c 6465 7220 2f20 7265 706f 7369 746f  older / reposito
-000017b0: 7279 2066 726f 6d20 6f70 656e 4249 532e  ry from openBIS.
-000017c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000017d0: 6461 7461 5f73 6574 5f69 643a 2049 6420  data_set_id: Id 
-000017e0: 6f66 2074 6865 2064 6174 6120 6672 6f6d  of the data from
-000017f0: 2077 6869 6368 2061 2072 6566 6572 656e   which a referen
-00001800: 6365 2073 686f 756c 6420 6265 2072 656d  ce should be rem
-00001810: 6f76 6564 2e0a 2020 2020 2020 2020 3a72  oved..        :r
-00001820: 6574 7572 6e3a 2041 2043 6f6d 6d61 6e64  eturn: A Command
-00001830: 5265 7375 6c74 2e0a 2020 2020 2020 2020  Result..        
-00001840: 4e72 1f00 0000 a902 723c 0000 0072 5b00  Nr......r<...r[.
-00001850: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00001860: 00da 0972 656d 6f76 6572 6566 cc00 0000  ...removeref....
-00001870: f302 0000 0004 067a 1a41 6273 7472 6163  .......z.Abstrac
-00001880: 7444 6174 614d 676d 742e 7265 6d6f 7665  tDataMgmt.remove
-00001890: 7265 6663 0500 0000 0000 0000 0000 0000  refc............
-000018a0: 0500 0000 0100 0000 4300 0000 7244 0000  ........C...rD..
-000018b0: 0029 0261 9001 0000 446f 776e 6c6f 6164  .).a....Download
-000018c0: 2066 696c 6573 206f 6620 6120 7265 706f   files of a repo
-000018d0: 7369 746f 7279 2077 6974 686f 7574 2061  sitory without a
-000018e0: 6464 696e 6720 6120 636f 6e74 656e 7420  dding a content 
-000018f0: 636f 7079 2e0a 2020 2020 2020 2020 3a70  copy..        :p
-00001900: 6172 616d 2064 6174 615f 7365 745f 6964  aram data_set_id
-00001910: 3a20 4964 206f 6620 7468 6520 6461 7461  : Id of the data
-00001920: 2073 6574 2074 6f20 646f 776e 6c6f 6164   set to download
-00001930: 2066 726f 6d2e 0a20 2020 2020 2020 203a   from..        :
-00001940: 7061 7261 6d20 6672 6f6d 5f66 696c 653a  param from_file:
-00001950: 2050 6174 6820 6f66 2061 2066 696c 6520   Path of a file 
-00001960: 7769 7468 2061 206c 6973 7420 6f66 2064  with a list of d
-00001970: 6174 6173 6574 7320 746f 2064 6f77 6e6c  atasets to downl
-00001980: 6f61 642e 0a20 2020 2020 2020 203a 7061  oad..        :pa
-00001990: 7261 6d20 6669 6c65 3a20 5061 7468 206f  ram file: Path o
-000019a0: 6620 6120 6669 6c65 2069 6e20 7468 6520  f a file in the 
-000019b0: 6461 7461 2073 6574 2074 6f20 646f 776e  data set to down
-000019c0: 6c6f 6164 2e20 416c 6c20 6669 6c65 7320  load. All files 
-000019d0: 6172 6520 646f 776e 6c6f 6164 6564 2069  are downloaded i
-000019e0: 6620 6974 2069 7320 4e6f 6e65 2e0a 2020  f it is None..  
-000019f0: 2020 2020 2020 3a70 6172 616d 2073 6b69        :param ski
-00001a00: 705f 696e 7465 6772 6974 795f 6368 6563  p_integrity_chec
-00001a10: 6b3a 2043 6865 636b 7375 6d73 206f 6620  k: Checksums of 
-00001a20: 6669 6c65 7320 6172 6520 6e6f 7420 7665  files are not ve
-00001a30: 7269 6669 6564 2069 6620 7472 7565 2e0a  rified if true..
-00001a40: 2020 2020 2020 2020 4e72 1f00 0000 a905          Nr......
-00001a50: 723c 0000 0072 5b00 0000 da09 6672 6f6d  r<...r[.....from
-00001a60: 5f66 696c 65da 0466 696c 6572 5e00 0000  _file..filer^...
-00001a70: 721f 0000 0072 1f00 0000 7237 0000 00da  r....r....r7....
-00001a80: 0864 6f77 6e6c 6f61 64d4 0000 0072 4e00  .download....rN.
-00001a90: 0000 7a19 4162 7374 7261 6374 4461 7461  ..z.AbstractData
-00001aa0: 4d67 6d74 2e64 6f77 6e6c 6f61 6463 0400  Mgmt.downloadc..
-00001ab0: 0000 0000 0000 0000 0000 0400 0000 0100  ................
-00001ac0: 0000 4300 0000 7244 0000 0029 027a ec55  ..C...rD...).z.U
-00001ad0: 706c 6f61 6420 6669 6c65 732f 6469 7265  pload files/dire
-00001ae0: 6374 6f72 6965 7320 696e 746f 2061 206e  ctories into a n
-00001af0: 6577 2064 6174 6120 7365 742e 0a20 2020  ew data set..   
-00001b00: 2020 2020 203a 7061 7261 6d20 7361 6d70       :param samp
-00001b10: 6c65 5f69 643a 2070 6572 6d49 6420 6f72  le_id: permId or
-00001b20: 2073 616d 706c 6520 7061 7468 206f 6620   sample path of 
-00001b30: 7468 6520 7061 7265 6e74 2073 616d 706c  the parent sampl
-00001b40: 650a 2020 2020 2020 2020 3a70 6172 616d  e.        :param
-00001b50: 2064 6174 615f 7365 745f 7479 7065 3a20   data_set_type: 
-00001b60: 7479 7065 206f 6620 6372 6561 7465 6420  type of created 
-00001b70: 6461 7461 2073 6574 0a20 2020 2020 2020  data set.       
-00001b80: 203a 7061 7261 6d20 6669 6c65 733a 206c   :param files: l
-00001b90: 6973 7420 6f66 2066 696c 6573 2f64 6972  ist of files/dir
-00001ba0: 6563 746f 7269 6573 2074 6f20 7570 6c6f  ectories to uplo
-00001bb0: 6164 0a20 2020 2020 2020 204e 721f 0000  ad.        Nr...
-00001bc0: 0029 0472 3c00 0000 da09 7361 6d70 6c65  .).r<.....sample
-00001bd0: 5f69 64da 0d64 6174 615f 7365 745f 7479  _id..data_set_ty
-00001be0: 7065 da05 6669 6c65 7372 1f00 0000 721f  pe..filesr....r.
-00001bf0: 0000 0072 3700 0000 da06 7570 6c6f 6164  ...r7.....upload
-00001c00: de00 0000 7252 0000 007a 1741 6273 7472  ....rR...z.Abstr
-00001c10: 6163 7444 6174 614d 676d 742e 7570 6c6f  actDataMgmt.uplo
-00001c20: 6164 6303 0000 0000 0000 0000 0000 0003  adc.............
-00001c30: 0000 0001 0000 0043 0000 0072 4400 0000  .......C...rD...
-00001c40: 2902 7ad6 5365 6172 6368 2066 6f72 206f  ).z.Search for o
-00001c50: 626a 6563 7473 2069 6e20 6f70 656e 4249  bjects in openBI
-00001c60: 5320 7573 696e 6720 6669 6c74 6572 696e  S using filterin
-00001c70: 6720 6372 6974 6572 6961 2e0a 2020 2020  g criteria..    
-00001c80: 2020 2020 3a70 6172 616d 2066 696c 7465      :param filte
-00001c90: 7273 3a20 6469 6374 696f 6e61 7279 206f  rs: dictionary o
-00001ca0: 6620 6669 6c74 6572 2070 6172 616d 6574  f filter paramet
-00001cb0: 6572 730a 2020 2020 2020 2020 3a70 6172  ers.        :par
-00001cc0: 616d 2073 6176 653a 2046 696c 6520 7061  am save: File pa
-00001cd0: 7468 2074 6f20 7361 7665 2072 6573 756c  th to save resul
-00001ce0: 7473 2e20 4966 206d 6973 7369 6e67 2c20  ts. If missing, 
-00001cf0: 7365 6172 6368 2072 6573 756c 7473 2077  search results w
-00001d00: 696c 6c20 6e6f 7420 6265 2073 6176 6564  ill not be saved
-00001d10: 2e0a 2020 2020 2020 2020 4e72 1f00 0000  ..        Nr....
-00001d20: a903 723c 0000 00da 0766 696c 7465 7273  ..r<.....filters
-00001d30: da04 7361 7665 721f 0000 0072 1f00 0000  ..saver....r....
-00001d40: 7237 0000 00da 0d73 6561 7263 685f 6f62  r7.....search_ob
-00001d50: 6a65 6374 e700 0000 7265 0000 007a 1e41  ject....re...z.A
-00001d60: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
-00001d70: 7365 6172 6368 5f6f 626a 6563 7463 0300  search_objectc..
-00001d80: 0000 0000 0000 0000 0000 0300 0000 0100  ................
-00001d90: 0000 4300 0000 7244 0000 0029 027a d753  ..C...rD...).z.S
-00001da0: 6561 7263 6820 666f 7220 6461 7461 7365  earch for datase
-00001db0: 7473 2069 6e20 6f70 656e 4249 5320 7573  ts in openBIS us
-00001dc0: 696e 6720 6669 6c74 6572 696e 6720 6372  ing filtering cr
-00001dd0: 6974 6572 6961 2e0a 2020 2020 2020 2020  iteria..        
-00001de0: 3a70 6172 616d 2066 696c 7465 7273 3a20  :param filters: 
-00001df0: 6469 6374 696f 6e61 7279 206f 6620 6669  dictionary of fi
-00001e00: 6c74 6572 2070 6172 616d 6574 6572 730a  lter parameters.
-00001e10: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-00001e20: 6176 653a 2046 696c 6520 7061 7468 2074  ave: File path t
-00001e30: 6f20 7361 7665 2072 6573 756c 7473 2e20  o save results. 
-00001e40: 4966 206d 6973 7369 6e67 2c20 7365 6172  If missing, sear
-00001e50: 6368 2072 6573 756c 7473 2077 696c 6c20  ch results will 
-00001e60: 6e6f 7420 6265 2073 6176 6564 2e0a 2020  not be saved..  
-00001e70: 2020 2020 2020 4e72 1f00 0000 726e 0000        Nr....rn..
-00001e80: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-00001e90: da0f 7365 6172 6368 5f64 6174 615f 7365  ..search_data_se
-00001ea0: 74ef 0000 0072 6500 0000 7a20 4162 7374  t....re...z Abst
-00001eb0: 7261 6374 4461 7461 4d67 6d74 2e73 6561  ractDataMgmt.sea
-00001ec0: 7263 685f 6461 7461 5f73 6574 6308 0000  rch_data_setc...
-00001ed0: 0000 0000 0000 0000 000c 0000 000c 0000  ................
-00001ee0: 0043 0000 0073 3e01 0000 7c03 7209 7c01  .C...s>...|.r.|.
-00001ef0: a000 6401 6701 a101 0100 6e06 7c01 a000  ..d.g.....n.|...
-00001f00: 6402 6701 a101 0100 7c01 a001 a100 7d08  d.g.....|.....}.
-00001f10: 7c04 7219 7c08 6403 1900 7d08 7c05 7402  |.r.|.d...}.|.t.
-00001f20: 6a03 7500 725b 7c06 6400 7500 7235 7404  j.u.r[|.d.u.r5t.
-00001f30: 6a05 7c08 6404 6405 6406 8d03 7d09 7406  j.|.d.d.d...}.t.
-00001f40: 6407 a007 7c09 a101 6408 6409 8d02 0100  d...|...d.d.....
-00001f50: 6400 5300 7c06 7c08 7601 7242 7408 640a  d.S.|.|.v.rBt.d.
-00001f60: a007 7c06 7c01 6a09 a102 8301 8201 7c06  ..|.|.j.......|.
-00001f70: 7c08 7c06 1900 6901 7d0a 7404 6a05 7c0a  |.|...i.}.t.j.|.
-00001f80: 6404 6405 6406 8d03 7d09 7406 6407 a007  d.d.d...}.t.d...
-00001f90: 7c09 a101 6408 6409 8d02 0100 6400 5300  |...d.d.....d.S.
-00001fa0: 7c05 7402 6a0a 7500 726d 740b 640b 7c00  |.t.j.u.rmt.d.|.
-00001fb0: a00c 7c02 7c01 7c06 7c07 7c03 7c04 a106  ..|.|.|.|.|.|...
-00001fc0: 8302 5300 7c05 7402 6a0d 7500 729d 7c06  ..S.|.t.j.u.r.|.
-00001fd0: 6400 7500 7290 640c 7d0b 7c08 a00e a100  d.u.r.d.}.|.....
-00001fe0: 4400 5d11 7d06 7c0b 740b 640b 7c00 a00c  D.].}.|.t.d.|...
-00001ff0: 7c02 7c01 7c06 6400 7c03 7c04 a106 8302  |.|.|.d.|.|.....
-00002000: 3700 7d0b 717c 7c0b 5300 740b 640b 7c00  7.}.q||.S.t.d.|.
-00002010: a00c 7c02 7c01 7c06 6400 7c03 7c04 a106  ..|.|.|.d.|.|...
-00002020: 8302 5300 6400 5300 290d 4eda 0667 6c6f  ..S.d.S.).N..glo
-00002030: 6261 6cda 056c 6f63 616c da0a 7072 6f70  bal..local..prop
-00002040: 6572 7469 6573 e904 0000 0054 2902 da06  erties.....T)...
-00002050: 696e 6465 6e74 da09 736f 7274 5f6b 6579  indent..sort_key
-00002060: 737a 027b 7d46 2901 da0e 7769 7468 5f74  sz.{}F)...with_t
-00002070: 696d 6573 7461 6d70 7a1a 556e 6b6e 6f77  imestampz.Unknow
-00002080: 6e20 7365 7474 696e 6720 7b7d 2066 6f72  n setting {} for
-00002090: 207b 7d2e 7204 0000 0072 0100 0000 290f   {}.r....r....).
-000020a0: da19 7365 745f 6c6f 6361 7469 6f6e 5f73  ..set_location_s
-000020b0: 6561 7263 685f 6f72 6465 7272 2600 0000  earch_orderr&...
-000020c0: 7212 0000 00da 0347 4554 da04 6a73 6f6e  r......GET..json
-000020d0: da05 6475 6d70 7372 1800 0000 723e 0000  ..dumpsr....r>..
-000020e0: 0072 3f00 0000 da08 6361 7465 676f 7479  .r?.....categoty
-000020f0: da03 5345 5472 1900 0000 da0c 7365 745f  ..SETr......set_
-00002100: 7072 6f70 6572 7479 da05 434c 4541 52da  property..CLEAR.
-00002110: 046b 6579 7329 0c72 3c00 0000 da08 7265  .keys).r<.....re
-00002120: 736f 6c76 6572 7233 0000 00da 0969 735f  solverr3.....is_
-00002130: 676c 6f62 616c da14 6973 5f64 6174 615f  global..is_data_
-00002140: 7365 745f 7072 6f70 6572 7479 da0e 6f70  set_property..op
-00002150: 6572 6174 696f 6e5f 7479 7065 da04 7072  eration_type..pr
-00002160: 6f70 da05 7661 6c75 6572 2600 0000 da0a  op..valuer&.....
-00002170: 636f 6e66 6967 5f73 7472 da0b 6c69 7474  config_str..litt
-00002180: 6c65 5f64 6963 74da 0b72 6574 7572 6e5f  le_dict..return_
-00002190: 636f 6465 721f 0000 0072 1f00 0000 7237  coder....r....r7
-000021a0: 0000 00da 0d75 7064 6174 655f 636f 6e66  .....update_conf
-000021b0: 6967 f700 0000 734e 0000 0004 030e 010c  ig....sN........
-000021c0: 0208 0204 0108 010a 0208 0110 0116 0108  ................
-000021d0: 0202 010c 0104 ff0c 0210 0116 010a 0104  ................
-000021e0: 010e 0102 0102 ff04 ff0a 0308 0104 010c  ................
-000021f0: 0106 010c 0104 0102 ff08 ff04 0304 020e  ................
-00002200: 0102 0102 ff04 ff04 f77a 1e41 6273 7472  .........z.Abstr
-00002210: 6163 7444 6174 614d 676d 742e 7570 6461  actDataMgmt.upda
-00002220: 7465 5f63 6f6e 6669 6763 0600 0000 0000  te_configc......
-00002230: 0000 0000 0000 0800 0000 0a00 0000 4300  ..............C.
-00002240: 0000 738e 0000 007c 0472 0464 016e 0164  ..s....|.r.d.n.d
-00002250: 027d 067a 187c 0572 147c 016a 0064 037c  .}.z.|.r.|.j.d.|
-00002260: 027c 037c 0664 0464 058d 0501 006e 097c  .|.|.d.d.....n.|
-00002270: 016a 017c 027c 037c 0664 0464 058d 0401  .j.|.|.|.d.d....
-00002280: 0057 006e 2204 0074 0279 4001 007d 0701  .W.n"..t.y@..}..
-00002290: 007a 167c 0064 0475 0072 2c7c 0782 0174  .z.|.d.u.r,|...t
-000022a0: 0364 0664 0774 047c 0783 0117 0064 088d  .d.d.t.|.....d..
-000022b0: 0257 0006 0059 0064 097d 077e 0753 0064  .W...Y.d.}.~.S.d
-000022c0: 097d 077e 0777 0177 0074 0364 0a64 0b64  .}.~.w.w.t.d.d.d
-000022d0: 088d 0253 0029 0c7a 3c48 656c 7065 7220  ...S.).z<Helper 
-000022e0: 6675 6e63 7469 6f6e 2074 6f20 696d 706c  function to impl
-000022f0: 656d 656e 7420 7468 6520 7072 6f70 6572  ement the proper
-00002300: 7479 2073 6574 7469 6e67 2073 656d 616e  ty setting seman
-00002310: 7469 6373 2e72 7300 0000 7274 0000 0072  tics.rs...rt...r
-00002320: 7500 0000 54a9 01da 0b61 7070 6c79 5f72  u...T....apply_r
-00002330: 756c 6573 e9ff ffff fffa 0745 7272 6f72  ules.......Error
-00002340: 3a20 a902 da0a 7265 7475 726e 636f 6465  : ....returncode
-00002350: da06 6f75 7470 7574 4e72 0100 0000 da00  ..outputNr......
-00002360: 2905 da1c 7365 745f 7661 6c75 655f 666f  )...set_value_fo
-00002370: 725f 6a73 6f6e 5f70 6172 616d 6574 6572  r_json_parameter
-00002380: da17 7365 745f 7661 6c75 655f 666f 725f  ..set_value_for_
-00002390: 7061 7261 6d65 7465 72da 0945 7863 6570  parameter..Excep
-000023a0: 7469 6f6e 7205 0000 00da 0373 7472 2908  tionr......str).
-000023b0: 7233 0000 0072 8300 0000 7287 0000 0072  r3...r....r....r
-000023c0: 8800 0000 7284 0000 0072 8500 0000 da03  ....r....r......
-000023d0: 6c6f 63da 0165 721f 0000 0072 1f00 0000  loc..er....r....
-000023e0: 7237 0000 0072 8000 0000 1f01 0000 731e  r7...r........s.
-000023f0: 0000 000c 0302 0104 010c 0102 0108 ff12  ................
-00002400: 0304 800e 0108 0104 0120 0108 8002 fd0c  ......... ......
-00002410: 057a 1d41 6273 7472 6163 7444 6174 614d  .z.AbstractDataM
-00002420: 676d 742e 7365 745f 7072 6f70 6572 7479  gmt.set_property
-00002430: 2902 4654 a901 4ea9 0254 54a9 024e 4e29  ).FT..N..TT..NN)
-00002440: 0146 291a da08 5f5f 6e61 6d65 5f5f da0a  .F)...__name__..
-00002450: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00002460: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
-00002470: 5f72 3d00 0000 7243 0000 00da 0361 6263  _r=...rC.....abc
-00002480: da0e 6162 7374 7261 6374 6d65 7468 6f64  ..abstractmethod
-00002490: 7246 0000 0072 4a00 0000 724d 0000 0072  rF...rJ...rM...r
-000024a0: 5100 0000 7257 0000 0072 5600 0000 7258  Q...rW...rV...rX
-000024b0: 0000 0072 5f00 0000 7261 0000 0072 6200  ...r_...ra...rb.
-000024c0: 0000 7264 0000 0072 6900 0000 726d 0000  ..rd...ri...rm..
-000024d0: 0072 7100 0000 7272 0000 0072 8c00 0000  .rq...rr...r....
-000024e0: da0c 7374 6174 6963 6d65 7468 6f64 7280  ..staticmethodr.
-000024f0: 0000 0072 1f00 0000 721f 0000 0072 1f00  ...r....r....r..
-00002500: 0000 7237 0000 0072 3900 0000 5a00 0000  ..r7...r9...Z...
-00002510: 7350 0000 0008 0004 0102 060a ff08 1104  sP..............
-00002520: 050a 0104 040a 0104 040c 0104 090c 0104  ................
-00002530: 080c 0104 0b0a 0104 080a 0104 060a 0104  ................
-00002540: 0a0a 0104 0a0a 0104 060c 0104 070a 0104  ................
-00002550: 090a 0104 080a 0104 070a 0102 0802 010a  ................
-00002560: fe02 2810 0172 3900 0000 2901 da09 6d65  ..(..r9...)...me
-00002570: 7461 636c 6173 7363 0000 0000 0000 0000  taclassc........
-00002580: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00002590: 7390 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000025a0: 0364 0264 0384 005a 0464 0464 0584 005a  .d.d...Z.d.d...Z
-000025b0: 0564 2264 0764 0884 015a 0664 2264 0964  .d"d.d...Z.d"d.d
-000025c0: 0a84 015a 0764 2364 0c64 0d84 015a 0864  ...Z.d#d.d...Z.d
-000025d0: 0e64 0f84 005a 0964 1064 1184 005a 0a64  .d...Z.d.d...Z.d
-000025e0: 1264 1384 005a 0b64 1464 1584 005a 0c64  .d...Z.d.d...Z.d
-000025f0: 1664 1784 005a 0d64 2264 1864 1984 015a  .d...Z.d"d.d...Z
-00002600: 0e64 1a64 1b84 005a 0f64 1c64 1d84 005a  .d.d...Z.d.d...Z
-00002610: 1064 1e64 1f84 005a 1164 2064 2184 005a  .d.d...Z.d d!..Z
-00002620: 1264 0653 0029 2472 2b00 0000 7a45 4461  .d.S.)$r+...zEDa
-00002630: 7461 4d67 6d74 206f 7065 7261 7469 6f6e  taMgmt operation
-00002640: 7320 7768 656e 2067 6974 2069 7320 6e6f  s when git is no
-00002650: 7420 6176 6169 6c61 626c 6520 2d2d 2073  t available -- s
-00002660: 686f 7720 6572 726f 7220 6d65 7373 6167  how error messag
-00002670: 6573 2e63 0100 0000 0000 0000 0000 0000  es.c............
-00002680: 0100 0000 0400 0000 4300 0000 f310 0000  ........C.......
-00002690: 007c 00a0 0064 0164 02a1 0201 0064 0053  .|...d.d.....d.S
-000026a0: 0029 034e 7a15 6765 7420 7365 7474 696e  .).Nz.get settin
-000026b0: 6773 2072 6573 6f6c 7665 72fa 154e 6f20  gs resolver..No 
-000026c0: 6769 7420 636f 6d6d 616e 6420 666f 756e  git command foun
-000026d0: 642e a901 7243 0000 0072 4500 0000 721f  d...rC...rE...r.
-000026e0: 0000 0072 1f00 0000 7237 0000 0072 4600  ...r....r7...rF.
-000026f0: 0000 3401 0000 f302 0000 0010 017a 234e  ..4..........z#N
-00002700: 6f47 6974 4461 7461 4d67 6d74 2e67 6574  oGitDataMgmt.get
-00002710: 5f73 6574 7469 6e67 735f 7265 736f 6c76  _settings_resolv
-00002720: 6572 6302 0000 0000 0000 0000 0000 0002  erc.............
-00002730: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
-00002740: 2903 4efa 1473 6574 7570 206c 6f63 616c  ).N..setup local
-00002750: 2073 6574 7469 6e67 7372 a700 0000 72a8   settingsr....r.
-00002760: 0000 0072 4800 0000 721f 0000 0072 1f00  ...rH...r....r..
-00002770: 0000 7237 0000 0072 4a00 0000 3701 0000  ..r7...rJ...7...
-00002780: 72a9 0000 007a 224e 6f47 6974 4461 7461  r....z"NoGitData
-00002790: 4d67 6d74 2e73 6574 7570 5f6c 6f63 616c  Mgmt.setup_local
-000027a0: 5f73 6574 7469 6e67 734e 6302 0000 0000  _settingsNc.....
-000027b0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-000027c0: 0000 0072 a600 0000 2903 4e7a 0969 6e69  ...r....).Nz.ini
-000027d0: 7420 6461 7461 72a7 0000 0072 a800 0000  t datar....r....
-000027e0: 724b 0000 0072 1f00 0000 721f 0000 0072  rK...r....r....r
-000027f0: 3700 0000 724d 0000 003a 0100 0072 a900  7...rM...:...r..
-00002800: 0000 7a17 4e6f 4769 7444 6174 614d 676d  ..z.NoGitDataMgm
-00002810: 742e 696e 6974 5f64 6174 6163 0300 0000  t.init_datac....
-00002820: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00002830: 4300 0000 72a6 0000 0029 034e fa0d 696e  C...r....).N..in
-00002840: 6974 2061 6e61 6c79 7369 7372 a700 0000  it analysisr....
-00002850: 72a8 0000 0072 4f00 0000 721f 0000 0072  r....rO...r....r
-00002860: 1f00 0000 7237 0000 0072 5100 0000 3d01  ....r7...rQ...=.
-00002870: 0000 72a9 0000 007a 1b4e 6f47 6974 4461  ..r....z.NoGitDa
-00002880: 7461 4d67 6d74 2e69 6e69 745f 616e 616c  taMgmt.init_anal
-00002890: 7973 6973 5463 0400 0000 0000 0000 0000  ysisTc..........
-000028a0: 0000 0400 0000 0400 0000 4300 0000 72a6  ..........C...r.
-000028b0: 0000 0029 034e 7257 0000 0072 a700 0000  ...).NrW...r....
-000028c0: 72a8 0000 0072 5300 0000 721f 0000 0072  r....rS...r....r
-000028d0: 1f00 0000 7237 0000 0072 5700 0000 4001  ....r7...rW...@.
-000028e0: 0000 72a9 0000 007a 144e 6f47 6974 4461  ..r....z.NoGitDa
-000028f0: 7461 4d67 6d74 2e63 6f6d 6d69 7463 0100  taMgmt.commitc..
-00002900: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00002910: 0000 4300 0000 72a6 0000 0029 034e 7256  ..C...r....).NrV
-00002920: 0000 0072 a700 0000 72a8 0000 0072 4500  ...r....r....rE.
-00002930: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00002940: 0072 5600 0000 4301 0000 72a9 0000 007a  .rV...C...r....z
-00002950: 124e 6f47 6974 4461 7461 4d67 6d74 2e73  .NoGitDataMgmt.s
-00002960: 796e 6363 0100 0000 0000 0000 0000 0000  yncc............
-00002970: 0100 0000 0400 0000 4300 0000 72a6 0000  ........C...r...
-00002980: 0029 034e 7258 0000 0072 a700 0000 72a8  .).NrX...r....r.
-00002990: 0000 0072 4500 0000 721f 0000 0072 1f00  ...rE...r....r..
-000029a0: 0000 7237 0000 0072 5800 0000 4601 0000  ..r7...rX...F...
-000029b0: 72a9 0000 007a 144e 6f47 6974 4461 7461  r....z.NoGitData
-000029c0: 4d67 6d74 2e73 7461 7475 7363 0500 0000  Mgmt.statusc....
-000029d0: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-000029e0: 4300 0000 72a6 0000 0029 034e 725f 0000  C...r....).Nr_..
-000029f0: 0072 a700 0000 72a8 0000 0072 5a00 0000  .r....r....rZ...
-00002a00: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
-00002a10: 5f00 0000 4901 0000 72a9 0000 007a 134e  _...I...r....z.N
-00002a20: 6f47 6974 4461 7461 4d67 6d74 2e63 6c6f  oGitDataMgmt.clo
-00002a30: 6e65 6305 0000 0000 0000 0000 0000 0005  nec.............
-00002a40: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
-00002a50: 2903 4e72 6100 0000 72a7 0000 0072 a800  ).Nra...r....r..
-00002a60: 0000 725a 0000 0072 1f00 0000 721f 0000  ..rZ...r....r...
-00002a70: 0072 3700 0000 7261 0000 004c 0100 0072  .r7...ra...L...r
-00002a80: a900 0000 7a12 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
-00002a90: 676d 742e 6d6f 7665 6301 0000 0000 0000  gmt.movec.......
-00002aa0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00002ab0: 0072 a600 0000 2903 4e72 6200 0000 72a7  .r....).Nrb...r.
-00002ac0: 0000 0072 a800 0000 7245 0000 0072 1f00  ...r....rE...r..
-00002ad0: 0000 721f 0000 0072 3700 0000 7262 0000  ..r....r7...rb..
-00002ae0: 004f 0100 0072 a900 0000 7a14 4e6f 4769  .O...r....z.NoGi
-00002af0: 7444 6174 614d 676d 742e 6164 6472 6566  tDataMgmt.addref
-00002b00: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002b10: 0004 0000 0043 0000 0072 a600 0000 2903  .....C...r....).
-00002b20: 4e72 6400 0000 72a7 0000 0072 a800 0000  Nrd...r....r....
-00002b30: 7263 0000 0072 1f00 0000 721f 0000 0072  rc...r....r....r
-00002b40: 3700 0000 7264 0000 0052 0100 0072 a900  7...rd...R...r..
-00002b50: 0000 7a17 4e6f 4769 7444 6174 614d 676d  ..z.NoGitDataMgm
-00002b60: 742e 7265 6d6f 7665 7265 6663 0100 0000  t.removerefc....
-00002b70: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00002b80: 4700 0000 72a6 0000 0029 034e 7269 0000  G...r....).Nri..
-00002b90: 0072 a700 0000 72a8 0000 00a9 0272 3c00  .r....r......r<.
-00002ba0: 0000 da01 5f72 1f00 0000 721f 0000 0072  ...._r....r....r
-00002bb0: 3700 0000 7269 0000 0055 0100 0072 a900  7...ri...U...r..
-00002bc0: 0000 7a16 4e6f 4769 7444 6174 614d 676d  ..z.NoGitDataMgm
-00002bd0: 742e 646f 776e 6c6f 6164 6301 0000 0000  t.downloadc.....
-00002be0: 0000 0000 0000 0002 0000 0004 0000 0047  ...............G
-00002bf0: 0000 0072 a600 0000 a903 4eda 0673 6561  ...r......N..sea
-00002c00: 7263 6872 a700 0000 72a8 0000 0072 ac00  rchr....r....r..
-00002c10: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00002c20: 0072 7100 0000 5801 0000 72a9 0000 007a  .rq...X...r....z
-00002c30: 1b4e 6f47 6974 4461 7461 4d67 6d74 2e73  .NoGitDataMgmt.s
-00002c40: 6561 7263 685f 6f62 6a65 6374 6301 0000  earch_objectc...
-00002c50: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00002c60: 0047 0000 0072 a600 0000 72ae 0000 0072  .G...r....r....r
-00002c70: a800 0000 72ac 0000 0072 1f00 0000 721f  ....r....r....r.
-00002c80: 0000 0072 3700 0000 7272 0000 005b 0100  ...r7...rr...[..
-00002c90: 0072 a900 0000 7a1d 4e6f 4769 7444 6174  .r....z.NoGitDat
-00002ca0: 614d 676d 742e 7365 6172 6368 5f64 6174  aMgmt.search_dat
-00002cb0: 615f 7365 7463 0100 0000 0000 0000 0000  a_setc..........
-00002cc0: 0000 0200 0000 0400 0000 4700 0000 72a6  ..........G...r.
-00002cd0: 0000 0029 034e 726d 0000 0072 a700 0000  ...).Nrm...r....
-00002ce0: 72a8 0000 0072 ac00 0000 721f 0000 0072  r....r....r....r
-00002cf0: 1f00 0000 7237 0000 0072 6d00 0000 5e01  ....r7...rm...^.
-00002d00: 0000 72a9 0000 007a 144e 6f47 6974 4461  ..r....z.NoGitDa
-00002d10: 7461 4d67 6d74 2e75 706c 6f61 6472 9b00  taMgmt.uploadr..
-00002d20: 0000 729c 0000 0029 1372 9e00 0000 729f  ..r....).r....r.
-00002d30: 0000 0072 a000 0000 72a1 0000 0072 4600  ...r....r....rF.
-00002d40: 0000 724a 0000 0072 4d00 0000 7251 0000  ..rJ...rM...rQ..
-00002d50: 0072 5700 0000 7256 0000 0072 5800 0000  .rW...rV...rX...
-00002d60: 725f 0000 0072 6100 0000 7262 0000 0072  r_...ra...rb...r
-00002d70: 6400 0000 7269 0000 0072 7100 0000 7272  d...ri...rq...rr
-00002d80: 0000 0072 6d00 0000 721f 0000 0072 1f00  ...rm...r....r..
-00002d90: 0000 721f 0000 0072 3700 0000 722b 0000  ..r....r7...r+..
-00002da0: 0031 0100 0073 2200 0000 0800 0401 0802  .1...s".........
-00002db0: 0803 0a03 0a03 0a03 0803 0803 0803 0803  ................
-00002dc0: 0803 0a03 0803 0803 0803 0c03 722b 0000  ............r+..
-00002dd0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002de0: 0000 0300 0000 4300 0000 7316 0000 007c  ......C...s....|
-00002df0: 00a0 00a1 0001 0074 01a0 0264 01a1 0101  .......t...d....
-00002e00: 0064 0053 0029 024e 7201 0000 0029 03da  .d.S.).Nr....)..
-00002e10: 0772 6573 746f 7265 da03 7379 73da 0465  .restore..sys..e
-00002e20: 7869 7429 01da 0964 6174 615f 6d67 6d74  xit)...data_mgmt
-00002e30: 721f 0000 0072 1f00 0000 7237 0000 00da  r....r....r7....
-00002e40: 1672 6573 746f 7265 5f73 6967 6e61 6c5f  .restore_signal_
-00002e50: 6861 6e64 6c65 7262 0100 0073 0400 0000  handlerb...s....
-00002e60: 0801 0e01 72b4 0000 0063 0100 0000 0000  ....r....c......
-00002e70: 0000 0000 0000 0200 0000 0300 0000 0300  ................
-00002e80: 0000 f310 0000 0087 0066 0164 0164 0284  .........f.d.d..
-00002e90: 087d 017c 0153 0029 037a 3320 546f 2062  .}.|.S.).z3 To b
-00002ea0: 6520 7573 6564 2077 6974 6820 636f 6d6d  e used with comm
-00002eb0: 616e 6473 2074 6861 7420 7573 6520 7468  ands that use th
-00002ec0: 6520 436f 6d6d 616e 644c 6f67 2e20 6301  e CommandLog. c.
-00002ed0: 0000 0000 0000 0000 0000 0004 0000 000a  ................
-00002ee0: 0000 0017 0000 0073 6e00 0000 7a0a 8800  .......sn...z...
-00002ef0: 7c00 6701 7c01 a201 5200 8e00 7d02 5700  |.g.|...R...}.W.
-00002f00: 6e16 0400 7400 7920 0100 7d03 0100 7a0a  n...t.y ..}...z.
-00002f10: 7c00 6a01 a002 7403 7c03 8301 a101 0100  |.j...t.|.......
-00002f20: 7c03 8201 6400 7d03 7e03 7701 7700 7c02  |...d.}.~.w.w.|.
-00002f30: a004 a100 6401 6b02 722e 7c00 6a01 a005  ....d.k.r.|.j...
-00002f40: a100 0100 7c02 5300 7c00 6a01 a002 7c02  ....|.S.|.j...|.
-00002f50: 6a06 a101 0100 7c02 5300 2902 4e46 2907  j.....|.S.).NF).
-00002f60: 7297 0000 0072 3200 0000 da09 6c6f 675f  r....r2.....log_
-00002f70: 6572 726f 7272 9800 0000 da07 6661 696c  errorr......fail
-00002f80: 7572 65da 0773 7563 6365 7373 7293 0000  ure..successr...
-00002f90: 00a9 0472 3c00 0000 da04 6172 6773 da06  ...r<.....args..
-00002fa0: 7265 7375 6c74 729a 0000 00a9 01da 0166  resultr........f
-00002fb0: 721f 0000 0072 3700 0000 da0a 665f 7769  r....r7.....f_wi
-00002fc0: 7468 5f6c 6f67 6a01 0000 7318 0000 0002  th_logj...s.....
-00002fd0: 0114 010e 0110 0104 0108 8002 fe0c 030a  ................
-00002fe0: 0104 030e ff04 017a 1c77 6974 685f 6c6f  .......z.with_lo
-00002ff0: 672e 3c6c 6f63 616c 733e 2e66 5f77 6974  g.<locals>.f_wit
-00003000: 685f 6c6f 6772 1f00 0000 2902 72bd 0000  h_logr....).r...
-00003010: 0072 be00 0000 721f 0000 0072 bc00 0000  .r....r....r....
-00003020: 7237 0000 00da 0877 6974 685f 6c6f 6767  r7.....with_logg
-00003030: 0100 0073 0400 0000 0c03 040c 72bf 0000  ...s........r...
-00003040: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00003050: 0000 0300 0000 0300 0000 72b5 0000 0029  ..........r....)
-00003060: 037a 2f20 5365 7473 2074 6865 2072 6573  .z/ Sets the res
-00003070: 746f 7265 2070 6f69 6e74 2061 6e64 2072  tore point and r
-00003080: 6573 746f 7265 7320 6f6e 2065 7272 6f72  estores on error
-00003090: 2e20 6301 0000 0000 0000 0000 0000 0004  . c.............
-000030a0: 0000 000a 0000 0017 0000 0073 aa00 0000  ...........s....
-000030b0: 8800 a000 a100 0100 7a25 8800 6a01 7213  ........z%..j.r.
-000030c0: 7402 a002 7402 6a03 8700 6601 6401 6402  t...t.j...f.d.d.
-000030d0: 8408 a102 0100 8801 8800 6701 7c01 a201  ..........g.|...
-000030e0: 5200 8e00 7d02 7c02 a004 a100 7223 8800  R...}.|.....r#..
-000030f0: a005 a100 0100 8800 a006 a100 0100 7c02  ..............|.
-00003100: 5700 5300 0400 7407 7954 0100 7d03 0100  W.S...t.yT..}...
-00003110: 7a1f 8800 a005 a100 0100 8800 6a08 6403  z...........j.d.
-00003120: 6b02 723c 7c03 8201 8800 a006 a100 0100  k.r<|...........
-00003130: 7409 6404 6405 740a 7c03 8301 1700 6406  t.d.d.t.|.....d.
-00003140: 8d02 5700 0600 5900 6400 7d03 7e03 5300  ..W...Y.d.}.~.S.
-00003150: 6400 7d03 7e03 7701 7700 2907 4e63 0200  d.}.~.w.w.).Nc..
-00003160: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00003170: 0000 1300 0000 7308 0000 0074 0088 0083  ......s....t....
-00003180: 0153 0072 9b00 0000 2901 72b4 0000 0029  .S.r....).r....)
-00003190: 02da 0673 6967 6e61 6cda 0566 7261 6d65  ...signal..frame
-000031a0: 7245 0000 0072 1f00 0000 7237 0000 00da  rE...r....r7....
-000031b0: 083c 6c61 6d62 6461 3e80 0100 0073 0200  .<lambda>....s..
-000031c0: 0000 0800 7a36 7769 7468 5f72 6573 746f  ....z6with_resto
-000031d0: 7265 2e3c 6c6f 6361 6c73 3e2e 665f 7769  re.<locals>.f_wi
-000031e0: 7468 5f72 6573 746f 7265 2e3c 6c6f 6361  th_restore.<loca
-000031f0: 6c73 3e2e 3c6c 616d 6264 613e 5472 8f00  ls>.<lambda>Tr..
-00003200: 0000 7290 0000 0072 9100 0000 290b da10  ..r....r....)...
-00003210: 7365 745f 7265 7374 6f72 6570 6f69 6e74  set_restorepoint
-00003220: 723a 0000 0072 c000 0000 da06 5349 4749  r:...r......SIGI
-00003230: 4e54 72b7 0000 0072 b000 0000 da12 636c  NTr....r......cl
-00003240: 6561 725f 7265 7374 6f72 6570 6f69 6e74  ear_restorepoint
-00003250: 7297 0000 0072 3300 0000 7205 0000 0072  r....r3...r....r
-00003260: 9800 0000 72b9 0000 0072 bc00 0000 7245  ....r....r....rE
-00003270: 0000 0072 3700 0000 da0e 665f 7769 7468  ...r7.....f_with
-00003280: 5f72 6573 746f 7265 7c01 0000 7322 0000  _restore|...s"..
-00003290: 0008 0102 0106 0116 0110 0108 0108 0108  ................
-000032a0: 0106 010e 0108 010a 0104 0108 0120 0108  ............. ..
-000032b0: 8002 fb7a 2477 6974 685f 7265 7374 6f72  ...z$with_restor
-000032c0: 652e 3c6c 6f63 616c 733e 2e66 5f77 6974  e.<locals>.f_wit
-000032d0: 685f 7265 7374 6f72 6572 1f00 0000 2902  h_restorer....).
-000032e0: 72bd 0000 0072 c600 0000 721f 0000 0072  r....r....r....r
-000032f0: bc00 0000 7237 0000 00da 0c77 6974 685f  ....r7.....with_
-00003300: 7265 7374 6f72 6579 0100 0073 0400 0000  restorey...s....
-00003310: 0c03 0411 72c7 0000 0063 0000 0000 0000  ....r....c......
-00003320: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
-00003330: 0000 73dc 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-00003340: 015a 0364 3064 0364 0484 015a 0464 0564  .Z.d0d.d...Z.d.d
-00003350: 0684 005a 0564 0764 0884 005a 0664 0964  ...Z.d.d...Z.d.d
-00003360: 0a84 005a 0764 3064 0b64 0c84 015a 0864  ...Z.d0d.d...Z.d
-00003370: 3064 0d64 0e84 015a 0965 0a64 0f64 1084  0d.d...Z.e.d.d..
-00003380: 0083 015a 0b64 1164 1284 005a 0c65 0a64  ...Z.d.d...Z.e.d
-00003390: 3164 1464 1584 0183 015a 0d64 1664 1784  1d.d.....Z.d.d..
-000033a0: 005a 0e64 1864 1984 005a 0f64 1a64 1b84  .Z.d.d...Z.d.d..
-000033b0: 005a 1064 1c64 1d84 005a 1164 1e64 1f84  .Z.d.d...Z.d.d..
-000033c0: 005a 1265 1364 2064 2184 0083 015a 1464  .Z.e.d d!....Z.d
-000033d0: 2264 2384 005a 1564 3064 2464 2584 015a  "d#..Z.d0d$d%..Z
-000033e0: 1664 2664 2784 005a 1709 0209 0264 3264  .d&d'..Z.....d2d
-000033f0: 2864 2984 015a 1864 2a64 2b84 005a 1964  (d)..Z.d*d+..Z.d
-00003400: 2c64 2d84 005a 1a64 2e64 2f84 005a 1b64  ,d-..Z.d.d/..Z.d
-00003410: 0253 0029 3372 2c00 0000 7a24 4461 7461  .S.)3r,...z$Data
-00003420: 4d67 6d74 206f 7065 7261 7469 6f6e 7320  Mgmt operations 
-00003430: 696e 206e 6f72 6d61 6c20 7374 6174 652e  in normal state.
-00003440: 4e63 0200 0000 0000 0000 0000 0000 0300  Nc..............
-00003450: 0000 0400 0000 4300 0000 7326 0000 007c  ......C...s&...|
-00003460: 0164 0075 0072 077c 006a 0053 0074 01a0  .d.u.r.|.j.S.t..
-00003470: 02a1 007d 027c 02a0 0364 017c 01a1 0201  ...}.|...d.|....
-00003480: 007c 0253 0029 024e da08 6461 7461 5f73  .|.S.).N..data_s
-00003490: 6574 2904 722e 0000 0072 2000 0000 7221  et).r....r ...r!
-000034a0: 0000 00da 1b73 6574 5f72 6573 6f6c 7665  .....set_resolve
-000034b0: 725f 6c6f 6361 7469 6f6e 5f72 6f6f 7473  r_location_roots
-000034c0: a903 723c 0000 00da 0d72 656c 6174 6976  ..r<.....relativ
-000034d0: 655f 7061 7468 722e 0000 0072 1f00 0000  e_pathr....r....
-000034e0: 721f 0000 0072 3700 0000 7246 0000 0093  r....r7...rF....
-000034f0: 0100 0073 0a00 0000 0801 0601 0802 0c01  ...s............
-00003500: 0401 7a21 4769 7444 6174 614d 676d 742e  ..z!GitDataMgmt.
-00003510: 6765 745f 7365 7474 696e 6773 5f72 6573  get_settings_res
-00003520: 6f6c 7665 7263 0200 0000 0000 0000 0000  olverc..........
-00003530: 0000 0700 0000 0700 0000 4300 0000 7350  ..........C...sP
-00003540: 0000 007c 006a 00a0 0164 0164 02a1 0201  ...|.j...d.d....
-00003550: 007c 01a0 02a1 0044 005d 1a5c 027d 027d  .|.....D.].\.}.}
-00003560: 0374 037c 006a 007c 0283 027d 047c 03a0  .t.|.j.|...}.|..
-00003570: 02a1 0044 005d 0b5c 027d 057d 067c 04a0  ...D.].\.}.}.|..
-00003580: 047c 057c 0664 03a1 0301 0071 1971 0b64  .|.|.d.....q.q.d
-00003590: 0053 0029 044e 72c8 0000 00da 012e 7274  .S.).Nr.......rt
-000035a0: 0000 0029 0572 2e00 0000 72c9 0000 00da  ...).r....r.....
-000035b0: 0569 7465 6d73 da07 6765 7461 7474 7272  .items..getattrr
-000035c0: 9600 0000 2907 723c 0000 0072 4900 0000  ....).r<...rI...
-000035d0: da0d 7265 736f 6c76 6572 5f74 7970 65da  ..resolver_type.
-000035e0: 0873 6574 7469 6e67 7372 8300 0000 da03  .settingsr......
-000035f0: 6b65 7972 8800 0000 721f 0000 0072 1f00  keyr....r....r..
-00003600: 0000 7237 0000 0072 4a00 0000 9c01 0000  ..r7...rJ.......
-00003610: 730e 0000 000e 0110 010c 0110 0110 0102  s...............
-00003620: ff04 fe7a 2047 6974 4461 7461 4d67 6d74  ...z GitDataMgmt
-00003630: 2e73 6574 7570 5f6c 6f63 616c 5f73 6574  .setup_local_set
-00003640: 7469 6e67 7363 0200 0000 0000 0000 0000  tingsc..........
-00003650: 0000 0300 0000 0300 0000 4300 0000 f31a  ..........C.....
-00003660: 0000 007c 00a0 007c 01a1 017d 027c 026a  ...|...|...}.|.j
-00003670: 01a0 02a1 00a0 0364 01a1 0153 0029 024e  .......d...S.).N
-00003680: 725b 0000 00a9 0472 4600 0000 da0a 7265  r[.....rF.....re
-00003690: 706f 7369 746f 7279 7226 0000 00da 0367  positoryr&.....g
-000036a0: 6574 72ca 0000 0072 1f00 0000 721f 0000  etr....r....r...
-000036b0: 0072 3700 0000 da0f 6765 745f 6461 7461  .r7.....get_data
-000036c0: 5f73 6574 5f69 64a3 0100 00f3 0400 0000  _set_id.........
-000036d0: 0a01 1001 7a1b 4769 7444 6174 614d 676d  ....z.GitDataMgm
-000036e0: 742e 6765 745f 6461 7461 5f73 6574 5f69  t.get_data_set_i
-000036f0: 6463 0200 0000 0000 0000 0000 0000 0300  dc..............
-00003700: 0000 0300 0000 4300 0000 72d2 0000 0029  ......C...r....)
-00003710: 024e da02 6964 72d3 0000 0072 ca00 0000  .N..idr....r....
-00003720: 721f 0000 0072 1f00 0000 7237 0000 00da  r....r....r7....
-00003730: 1167 6574 5f72 6570 6f73 6974 6f72 795f  .get_repository_
-00003740: 6964 a701 0000 72d7 0000 007a 1d47 6974  id....r....z.Git
-00003750: 4461 7461 4d67 6d74 2e67 6574 5f72 6570  DataMgmt.get_rep
-00003760: 6f73 6974 6f72 795f 6964 6302 0000 0000  ository_idc.....
-00003770: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00003780: 0000 0073 9400 0000 7400 6a01 a002 6401  ...s....t.j...d.
-00003790: a101 720c 7403 6402 6403 6404 8d02 5300  ..r.t.d.d.d...S.
-000037a0: 7c00 6a04 a005 a100 7d02 7c02 a006 a100  |.j.....}.|.....
-000037b0: 7217 7c02 5300 7c00 6a07 6a08 a009 a100  r.|.S.|.j.j.....
-000037c0: a00a 6405 a101 7d03 7c00 6a04 a00b 7c01  ..d...}.|.j...|.
-000037d0: 7c03 a102 7d02 7c02 a006 a100 722d 7c02  |...}.|.....r-|.
-000037e0: 5300 7c00 6a04 a00c a100 7d02 7c02 a006  S.|.j.....}.|...
-000037f0: a100 7238 7c02 5300 7c00 6a07 a00d 6406  ..r8|.S.|.j...d.
-00003800: 6407 a102 0100 7c00 6a07 a00e a100 0100  d.....|.j.......
-00003810: 7403 6408 6409 6404 8d02 5300 290a 4e72  t.d.d.d...S.).Nr
-00003820: 1d00 0000 728f 0000 00fa 2546 6f6c 6465  ....r.....%Folde
-00003830: 7220 6973 2061 6c72 6561 6479 2061 6e20  r is already an 
-00003840: 6f62 6973 2072 6570 6f73 6974 6f72 792e  obis repository.
-00003850: 7291 0000 00da 1167 6974 5f61 6e6e 6578  r......git_annex
-00003860: 5f62 6163 6b65 6e64 72c8 0000 0072 cc00  _backendr....r..
-00003870: 0000 7201 0000 0072 9400 0000 290f 7223  ..r....r....).r#
-00003880: 0000 0072 2400 0000 7225 0000 0072 0500  ...r$...r%...r..
-00003890: 0000 7236 0000 00da 0867 6974 5f69 6e69  ..r6.....git_ini
-000038a0: 7472 b700 0000 722e 0000 0072 0400 0000  tr....r....r....
-000038b0: 7226 0000 0072 d500 0000 da0e 6769 745f  r&...r......git_
-000038c0: 616e 6e65 785f 696e 6974 da0e 696e 6974  annex_init..init
-000038d0: 6961 6c5f 636f 6d6d 6974 72c9 0000 00da  ial_commitr.....
-000038e0: 1463 6f70 795f 676c 6f62 616c 5f74 6f5f  .copy_global_to_
-000038f0: 6c6f 6361 6c29 0472 3c00 0000 724c 0000  local).r<...rL..
-00003900: 0072 bb00 0000 72db 0000 0072 1f00 0000  .r....r....r....
-00003910: 721f 0000 0072 3700 0000 724d 0000 00ab  r....r7...rM....
-00003920: 0100 0073 1e00 0000 0c02 0c01 0a01 0801  ...s............
-00003930: 0401 1201 0e01 0801 0401 0a01 0801 0401  ................
-00003940: 0e02 0a01 0c01 7a15 4769 7444 6174 614d  ......z.GitDataM
-00003950: 676d 742e 696e 6974 5f64 6174 6163 0300  gmt.init_datac..
-00003960: 0000 0000 0000 0000 0000 0900 0000 0a00  ................
-00003970: 0000 4300 0000 7316 0100 007c 00a0 007c  ..C...s....|...|
-00003980: 01a1 017d 037c 00a0 017c 01a1 0164 0075  ...}.|...|...d.u
-00003990: 0072 1274 0264 0164 0264 038d 0253 007c  .r.t.d.d.d...S.|
-000039a0: 00a0 037c 02a1 017d 047c 04a0 04a1 0072  ...|...}.|.....r
-000039b0: 1d7c 0453 0074 056a 06a0 0774 05a0 08a1  .|.S.t.j...t....
-000039c0: 007c 01a1 027d 0574 05a0 08a1 007d 0674  .|...}.t.....}.t
-000039d0: 097c 0683 0174 097c 0583 016a 0a76 0072  .|...t.|...j.v.r
-000039e0: 5474 056a 06a0 0b7c 067c 05a1 027d 0774  Tt.j...|.|...}.t
-000039f0: 0c7c 0183 018f 0e01 007c 006a 0da0 0e7c  .|.......|.j...|
-00003a00: 07a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00003a10: 006e 0831 0073 4f77 0101 0001 0001 0059  .n.1.sOw.......Y
-00003a20: 0001 007a 0d7c 006a 0f6a 106a 1164 047c  ...z.|.j.j.j.d.|
-00003a30: 0364 0564 0664 078d 0401 0057 006e 2304  .d.d.d.....W.n#.
-00003a40: 0074 1279 8401 007d 0801 007a 177c 006a  .t.y...}...z.|.j
-00003a50: 1364 0675 0072 707c 0882 0174 0264 0164  .d.u.rp|...t.d.d
-00003a60: 0874 147c 0883 0117 0064 038d 0257 0006  .t.|.....d...W..
-00003a70: 0059 0064 007d 087e 0853 0064 007d 087e  .Y.d.}.~.S.d.}.~
-00003a80: 0877 0177 0074 0264 0964 0a64 038d 0253  .w.w.t.d.d.d...S
-00003a90: 0029 0b4e 728f 0000 007a 5250 6172 656e  .).Nr....zRParen
-00003aa0: 7420 6461 7461 2073 6574 206d 7573 7420  t data set must 
-00003ab0: 6265 2063 6f6d 6d69 7474 6564 2074 6f20  be committed to 
-00003ac0: 6f70 656e 4249 5320 6265 666f 7265 2063  openBIS before c
-00003ad0: 7265 6174 696e 6720 616e 2061 6e61 6c79  reating an analy
-00003ae0: 7369 7320 6461 7461 2073 6574 2e72 9100  sis data set.r..
-00003af0: 0000 725b 0000 0072 7400 0000 5472 8d00  ..r[...rt...Tr..
-00003b00: 0000 7290 0000 0072 0100 0000 7294 0000  ..r....r....r...
-00003b10: 0029 1572 d600 0000 72d9 0000 0072 0500  .).r....r....r..
-00003b20: 0000 724d 0000 0072 b700 0000 7223 0000  ..rM...r....r#..
-00003b30: 0072 2400 0000 da04 6a6f 696e da06 6765  .r$.....join..ge
-00003b40: 7463 7764 7202 0000 00da 0770 6172 656e  tcwdr......paren
-00003b50: 7473 da07 7265 6c70 6174 6872 1300 0000  ts..relpathr....
-00003b60: 7236 0000 00da 0a67 6974 5f69 676e 6f72  r6.....git_ignor
-00003b70: 6572 2e00 0000 72d4 0000 0072 9600 0000  er....r....r....
-00003b80: 7297 0000 0072 3300 0000 7298 0000 0029  r....r3...r....)
-00003b90: 0972 3c00 0000 7250 0000 0072 4c00 0000  .r<...rP...rL...
-00003ba0: da12 7061 7265 6e74 5f64 6174 615f 7365  ..parent_data_se
-00003bb0: 745f 6964 72bb 0000 00da 1170 6172 656e  t_idr......paren
-00003bc0: 745f 666f 6c64 6572 5f61 6273 da13 616e  t_folder_abs..an
-00003bd0: 616c 7973 6973 5f66 6f6c 6465 725f 6162  alysis_folder_ab
-00003be0: 73da 1861 6e61 6c79 7369 735f 666f 6c64  s..analysis_fold
-00003bf0: 6572 5f72 656c 6174 6976 6572 9a00 0000  er_relativer....
-00003c00: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
-00003c10: 5100 0000 be01 0000 7336 0000 000a 020e  Q.......s6......
-00003c20: 0204 0102 0106 ff0a 0308 0104 0112 0308  ................
-00003c30: 0112 010e 010a 010e 011c ff02 040a 0104  ................
-00003c40: 0102 010a fe0e 030a 0104 0120 0108 8002  ........... ....
-00003c50: fd0c 057a 1947 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
-00003c60: 2e69 6e69 745f 616e 616c 7973 6973 6301  .init_analysisc.
-00003c70: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00003c80: 0000 0043 0000 0073 0800 0000 7c00 a000  ...C...s....|...
-00003c90: a100 5300 729b 0000 0029 01da 055f 7379  ..S.r....)..._sy
-00003ca0: 6e63 7245 0000 0072 1f00 0000 721f 0000  ncrE...r....r...
-00003cb0: 0072 3700 0000 7256 0000 00de 0100 0073  .r7...rV.......s
-00003cc0: 0200 0000 0802 7a10 4769 7444 6174 614d  ......z.GitDataM
-00003cd0: 676d 742e 7379 6e63 6301 0000 0000 0000  gmt.syncc.......
-00003ce0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00003cf0: 0073 1400 0000 7400 7c00 7c00 6a01 8302  .s....t.|.|.j...
-00003d00: 7d01 7c01 a002 a100 5300 729b 0000 0029  }.|.....S.r....)
-00003d10: 0372 0c00 0000 723b 0000 00da 0372 756e  .r....r;.....run
-00003d20: a902 723c 0000 00da 0363 6d64 721f 0000  ..r<.....cmdr...
-00003d30: 0072 1f00 0000 7237 0000 0072 e900 0000  .r....r7...r....
-00003d40: e201 0000 f304 0000 000c 0108 017a 1147  .............z.G
-00003d50: 6974 4461 7461 4d67 6d74 2e5f 7379 6e63  itDataMgmt._sync
-00003d60: 5463 0400 0000 0000 0000 0000 0000 0500  Tc..............
-00003d70: 0000 0300 0000 4300 0000 735c 0000 007c  ......C...s\...|
-00003d80: 0272 1a7c 006a 00a0 01a1 007d 047c 04a0  .r.|.j.....}.|..
-00003d90: 02a1 0072 0d7c 0453 007c 006a 00a0 037c  ...r.|.S.|.j...|
-00003da0: 046a 04a1 017d 047c 04a0 02a1 0072 1a7c  .j...}.|.....r.|
-00003db0: 0453 007c 006a 00a0 057c 01a1 017d 047c  .S.|.j...|...}.|
-00003dc0: 04a0 02a1 0072 267c 0453 007c 0372 2c7c  .....r&|.S.|.r,|
-00003dd0: 00a0 06a1 007d 047c 0453 0029 017a 2820  .....}.|.S.).z( 
-00003de0: 4769 7420 6164 642c 2063 6f6d 6d69 7420  Git add, commit 
-00003df0: 616e 6420 7379 6e63 2077 6974 6820 6f70  and sync with op
-00003e00: 656e 4249 532e 2029 0772 3600 0000 da12  enBIS. ).r6.....
-00003e10: 6769 745f 746f 705f 6c65 7665 6c5f 7061  git_top_level_pa
-00003e20: 7468 72b7 0000 00da 0767 6974 5f61 6464  thr......git_add
-00003e30: 7293 0000 00da 0a67 6974 5f63 6f6d 6d69  r......git_commi
-00003e40: 7472 e900 0000 2905 723c 0000 0072 5400  tr....).r<...rT.
-00003e50: 0000 7255 0000 0072 5600 0000 72bb 0000  ..rU...rV...r...
-00003e60: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-00003e70: 7257 0000 00e6 0100 0073 1a00 0000 0403  rW.......s......
-00003e80: 0a01 0801 0401 0e01 0801 0401 0c01 0801  ................
-00003e90: 0402 0401 0801 0401 7a12 4769 7444 6174  ........z.GitDat
-00003ea0: 614d 676d 742e 636f 6d6d 6974 6301 0000  aMgmt.commitc...
-00003eb0: 0000 0000 0000 0000 0004 0000 0008 0000  ................
-00003ec0: 0043 0000 0073 7a00 0000 7c00 6a00 a001  .C...sz...|.j...
-00003ed0: a100 7d01 7a0a 7402 7c00 8301 6a03 6401  ..}.z.t.|...j.d.
-00003ee0: 6402 8d01 7d02 5700 6e11 0400 7404 6a05  d...}.W.n...t.j.
-00003ef0: 6a06 7920 0100 0100 0100 7407 6403 6404  j.y ......t.d.d.
-00003f00: 6405 8d02 7d02 5900 6e01 7700 7c01 6a08  d...}.Y.n.w.|.j.
-00003f10: 7d03 7c02 a009 a100 7237 740a 7c03 8301  }.|.....r7t.|...
-00003f20: 6406 6b04 7232 7c03 6407 3700 7d03 7c03  d.k.r2|.d.7.}.|.
-00003f30: 7c02 6a08 3700 7d03 7407 6406 7c03 6405  |.j.7.}.t.d.|.d.
-00003f40: 8d02 5300 2908 4e54 2901 da09 696e 666f  ..S.).NT)...info
-00003f50: 5f6f 6e6c 7972 8f00 0000 7a1d 436f 756c  _onlyr....z.Coul
-00003f60: 6420 6e6f 7420 636f 6e6e 6563 7420 746f  d not connect to
-00003f70: 206f 7065 6e42 4953 2e72 9100 0000 7201   openBIS.r....r.
-00003f80: 0000 00da 010a 290b 7236 0000 00da 0a67  ......).r6.....g
-00003f90: 6974 5f73 7461 7475 7372 0c00 0000 72ea  it_statusr....r.
-00003fa0: 0000 00da 0872 6571 7565 7374 73da 0a65  .....requests..e
-00003fb0: 7863 6570 7469 6f6e 73da 0f43 6f6e 6e65  xceptions..Conne
-00003fc0: 6374 696f 6e45 7272 6f72 7205 0000 0072  ctionErrorr....r
-00003fd0: 9300 0000 72b7 0000 00da 036c 656e 2904  ....r......len).
-00003fe0: 723c 0000 0072 f300 0000 da0b 7379 6e63  r<...r......sync
-00003ff0: 5f73 7461 7475 7372 9300 0000 721f 0000  _statusr....r...
-00004000: 0072 1f00 0000 7237 0000 0072 5800 0000  .r....r7...rX...
-00004010: f801 0000 7318 0000 000a 0102 0114 0110  ....s...........
-00004020: 0110 0102 ff06 0208 010c 0108 010a 010c  ................
-00004030: 017a 1247 6974 4461 7461 4d67 6d74 2e73  .z.GitDataMgmt.s
-00004040: 7461 7475 7363 0100 0000 0000 0000 0000  tatusc..........
-00004050: 0000 0100 0000 0400 0000 4300 0000 7326  ..........C...s&
-00004060: 0000 007c 006a 00a0 01a1 006a 027c 005f  ...|.j.....j.|._
-00004070: 037c 00a0 04a1 0001 0074 05a0 0664 0164  .|.......t...d.d
-00004080: 02a1 0201 0064 0353 0029 047a 3a20 5374  .....d.S.).z: St
-00004090: 6f72 6573 2074 6865 2067 6974 2063 6f6d  ores the git com
-000040a0: 6d69 7420 6861 7368 2061 6e64 2063 6f70  mit hash and cop
-000040b0: 6965 7320 7468 6520 6f62 6973 206d 6574  ies the obis met
-000040c0: 6164 6174 612e 2072 1d00 0000 fa12 2e6f  adata. r.......o
-000040d0: 6269 735f 7265 7374 6f72 6570 6f69 6e74  bis_restorepoint
-000040e0: 4e29 0772 3600 0000 da0f 6769 745f 636f  N).r6.....git_co
-000040f0: 6d6d 6974 5f68 6173 6872 9300 0000 da18  mmit_hashr......
-00004100: 7072 6576 696f 7573 5f67 6974 5f63 6f6d  previous_git_com
-00004110: 6d69 745f 6861 7368 72c5 0000 00da 0673  mit_hashr......s
-00004120: 6875 7469 6cda 0863 6f70 7974 7265 6572  hutil..copytreer
-00004130: 4500 0000 721f 0000 0072 1f00 0000 7237  E...r....r....r7
-00004140: 0000 0072 c300 0000 0502 0000 7306 0000  ...r........s...
-00004150: 000e 0208 0110 017a 1c47 6974 4461 7461  .......z.GitData
-00004160: 4d67 6d74 2e73 6574 5f72 6573 746f 7265  Mgmt.set_restore
-00004170: 706f 696e 7463 0100 0000 0000 0000 0000  pointc..........
-00004180: 0000 0100 0000 0400 0000 4300 0000 7328  ..........C...s(
-00004190: 0000 007c 006a 00a0 017c 006a 02a1 0101  ...|.j...|.j....
-000041a0: 0074 03a0 0464 01a1 0101 0074 03a0 0564  .t...d.....t...d
-000041b0: 0264 01a1 0201 0064 0353 0029 047a 4d20  .d.....d.S.).zM 
-000041c0: 5265 7365 7473 2074 6f20 7468 6520 7374  Resets to the st
-000041d0: 6f72 6564 2067 6974 2063 6f6d 6d69 7420  ored git commit 
-000041e0: 6861 7368 2061 6e64 2072 6573 746f 7265  hash and restore
-000041f0: 7320 7468 6520 636f 7069 6564 206f 6269  s the copied obi
-00004200: 7320 6d65 7461 6461 7461 2e20 721d 0000  s metadata. r...
-00004210: 0072 f900 0000 4e29 0672 3600 0000 da0c  .r....N).r6.....
-00004220: 6769 745f 7265 7365 745f 746f 72fb 0000  git_reset_tor...
-00004230: 0072 fc00 0000 da06 726d 7472 6565 72fd  .r......rmtreer.
-00004240: 0000 0072 4500 0000 721f 0000 0072 1f00  ...rE...r....r..
-00004250: 0000 7237 0000 0072 b000 0000 0b02 0000  ..r7...r........
-00004260: 7306 0000 000e 020a 0110 017a 1347 6974  s..........z.Git
-00004270: 4461 7461 4d67 6d74 2e72 6573 746f 7265  DataMgmt.restore
-00004280: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00004290: 0003 0000 0043 0000 0073 1e00 0000 7400  .....C...s....t.
-000042a0: 6a01 a002 6401 a101 720d 7403 a004 6401  j...d...r.t...d.
-000042b0: a101 0100 6402 5300 6402 5300 2903 7a3b  ....d.S.d.S.).z;
-000042c0: 2044 656c 6574 6573 2074 6865 206f 6269   Deletes the obi
-000042d0: 7320 6d65 7461 6461 7461 2063 6f70 792e  s metadata copy.
-000042e0: 2054 6869 7320 6d75 7374 2061 6c77 6179   This must alway
-000042f0: 7320 6265 2064 6f6e 652e 2072 f900 0000  s be done. r....
-00004300: 4e29 0572 2300 0000 7224 0000 0072 2500  N).r#...r$...r%.
-00004310: 0000 72fc 0000 0072 ff00 0000 7245 0000  ..r....r....rE..
-00004320: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-00004330: 72c5 0000 0011 0200 0073 0600 0000 0c02  r........s......
-00004340: 0e01 04ff 7a1e 4769 7444 6174 614d 676d  ....z.GitDataMgm
-00004350: 742e 636c 6561 725f 7265 7374 6f72 6570  t.clear_restorep
-00004360: 6f69 6e74 6305 0000 0000 0000 0000 0000  ointc...........
-00004370: 0006 0000 0006 0000 0043 0000 00f3 1800  .........C......
-00004380: 0000 7400 7c00 7c01 7c02 7c03 7c04 8305  ..t.|.|.|.|.|...
-00004390: 7d05 7c05 a001 a100 5300 729b 0000 0029  }.|.....S.r....)
-000043a0: 0272 0700 0000 72ea 0000 00a9 0672 3c00  .r....r......r<.
-000043b0: 0000 725b 0000 0072 5c00 0000 725d 0000  ..r[...r\...r]..
-000043c0: 0072 5e00 0000 72ec 0000 0072 1f00 0000  .r^...r....r....
-000043d0: 721f 0000 0072 3700 0000 725f 0000 0016  r....r7...r_....
-000043e0: 0200 00f3 0400 0000 1001 0801 7a11 4769  ............z.Gi
-000043f0: 7444 6174 614d 676d 742e 636c 6f6e 6563  tDataMgmt.clonec
-00004400: 0500 0000 0000 0000 0000 0000 0600 0000  ................
-00004410: 0600 0000 4300 0000 7200 0100 0072 9b00  ....C...r....r..
-00004420: 0000 2902 720a 0000 0072 ea00 0000 7201  ..).r....r....r.
-00004430: 0100 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
-00004440: 0000 7261 0000 001a 0200 0073 0400 0000  ..ra.......s....
-00004450: 1002 0801 7a10 4769 7444 6174 614d 676d  ....z.GitDataMgm
-00004460: 742e 6d6f 7665 6301 0000 0000 0000 0000  t.movec.........
-00004470: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
-00004480: 1000 0000 7400 7c00 8301 7d01 7c01 a001  ....t.|...}.|...
-00004490: a100 5300 729b 0000 0029 0272 0600 0000  ..S.r....).r....
-000044a0: 72ea 0000 0072 eb00 0000 721f 0000 0072  r....r....r....r
-000044b0: 1f00 0000 7237 0000 0072 6200 0000 1f02  ....r7...rb.....
-000044c0: 0000 7304 0000 0008 0108 017a 1247 6974  ..s........z.Git
-000044d0: 4461 7461 4d67 6d74 2e61 6464 7265 6663  DataMgmt.addrefc
-000044e0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-000044f0: 0400 0000 4300 0000 7314 0000 0074 007c  ....C...s....t.|
-00004500: 007c 0164 018d 027d 027c 02a0 01a1 0053  .|.d...}.|.....S
-00004510: 0029 024e 2901 725b 0000 0029 0272 0d00  .).N).r[...).r..
-00004520: 0000 72ea 0000 0029 0372 3c00 0000 725b  ..r....).r<...r[
-00004530: 0000 0072 ec00 0000 721f 0000 0072 1f00  ...r....r....r..
-00004540: 0000 7237 0000 0072 6400 0000 2302 0000  ..r7...rd...#...
-00004550: 72ed 0000 007a 1547 6974 4461 7461 4d67  r....z.GitDataMg
-00004560: 6d74 2e72 656d 6f76 6572 6566 6305 0000  mt.removerefc...
-00004570: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00004580: 0043 0000 0072 a600 0000 2903 4e72 6900  .C...r....).Nri.
-00004590: 0000 fa30 5468 6973 2063 6f6d 6d61 6e64  ...0This command
-000045a0: 2069 7320 6f6e 6c79 2061 7661 696c 6162   is only availab
-000045b0: 6c65 2066 6f72 204d 616e 6167 6572 2044  le for Manager D
-000045c0: 6174 612e 72a8 0000 0072 6600 0000 721f  ata.r....rf...r.
-000045d0: 0000 0072 1f00 0000 7237 0000 0072 6900  ...r....r7...ri.
-000045e0: 0000 2702 0000 72a9 0000 007a 1447 6974  ..'...r....z.Git
-000045f0: 4461 7461 4d67 6d74 2e64 6f77 6e6c 6f61  DataMgmt.downloa
-00004600: 6463 0700 0000 0000 0000 0000 0000 0800  dc..............
-00004610: 0000 0900 0000 4300 0000 738a 0000 007c  ......C...s....|
-00004620: 006a 00a0 017c 01a1 017d 077c 0764 0175  .j...|...}.|.d.u
-00004630: 0072 1074 0264 027c 0117 0083 0182 017c  .r.t.d.|.......|
-00004640: 0474 036a 0475 0072 227c 0564 0175 0173  .t.j.u.r"|.d.u.s
-00004650: 1b4a 0082 017c 0664 0175 0173 214a 0082  .J...|.d.u.s!J..
-00004660: 016e 177c 0474 036a 0575 0072 2e7c 0664  .n.|.t.j.u.r.|.d
-00004670: 0175 0073 2d4a 0082 016e 0b7c 0474 036a  .u.s-J...n.|.t.j
-00004680: 0675 0072 397c 0664 0175 0073 394a 0082  .u.r9|.d.u.s9J..
-00004690: 017c 00a0 077c 077c 006a 087c 027c 037c  .|...|.|.j.|.|.|
-000046a0: 047c 057c 06a1 0753 0029 03e1 8501 0000  .|.|...S.)......
-000046b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000046c0: 6361 7465 676f 7279 3a20 636f 6e66 6967  category: config
-000046d0: 2c20 6f62 6a65 6374 2c20 636f 6c6c 6563  , object, collec
-000046e0: 7469 6f6e 2c20 6461 7461 5f73 6574 206f  tion, data_set o
-000046f0: 7220 7265 706f 7369 746f 7279 0a20 2020  r repository.   
-00004700: 2020 2020 203a 7061 7261 6d20 6973 5f67       :param is_g
-00004710: 6c6f 6261 6c3a 2061 6374 206f 6e20 676c  lobal: act on gl
-00004720: 6f62 616c 2073 6574 7469 6e67 7320 2d20  obal settings - 
-00004730: 6c6f 6361 6c20 6966 2066 616c 7365 0a20  local if false. 
-00004740: 2020 2020 2020 203a 7061 7261 6d20 6973         :param is
-00004750: 5f64 6174 615f 7365 745f 7072 6f70 6572  _data_set_proper
-00004760: 7479 3a20 7472 7565 2069 6620 7072 6f70  ty: true if prop
-00004770: 202f 2076 616c 7565 2061 7265 2061 2064   / value are a d
-00004780: 6174 6120 7365 7420 7072 6f70 6572 7479  ata set property
-00004790: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000047a0: 6f70 6572 6174 696f 6e5f 7479 7065 3a20  operation_type: 
-000047b0: 7479 7065 206f 6620 6f70 6572 6174 696f  type of operatio
-000047c0: 6e20 746f 2070 6572 666f 726d 2e20 4974  n to perform. It
-000047d0: 2063 616e 2062 6520 4745 542c 2053 4554   can be GET, SET
-000047e0: 2c20 434c 4541 520a 2020 2020 2020 2020  , CLEAR.        
-000047f0: 3a70 6172 616d 2070 726f 703a 2073 6574  :param prop: set
-00004800: 7469 6e67 206b 6579 0a20 2020 2020 2020  ting key.       
-00004810: 203a 7061 7261 6d20 7661 6c75 653a 2073   :param value: s
-00004820: 6574 7469 6e67 2076 616c 7565 0a20 2020  etting value.   
-00004830: 2020 2020 204e fa1b 496e 7661 6c69 6420       N..Invalid 
-00004840: 7365 7474 696e 6773 2063 6174 6567 6f72  settings categor
-00004850: 793a 2029 0972 2e00 0000 72d5 0000 0072  y: ).r....r....r
-00004860: 3f00 0000 7212 0000 0072 7f00 0000 727b  ?...r....r....r{
-00004870: 0000 0072 8100 0000 728c 0000 0072 3300  ...r....r....r3.
-00004880: 0000 2908 723c 0000 00da 0863 6174 6567  ..).r<.....categ
-00004890: 6f72 7972 8400 0000 7285 0000 0072 8600  oryr....r....r..
-000048a0: 0000 7287 0000 0072 8800 0000 7283 0000  ..r....r....r...
-000048b0: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-000048c0: 7204 0000 002e 0200 0073 1a00 0000 0c0a  r........s......
-000048d0: 0801 0c01 0a01 0c01 0e01 0a01 0e01 0a01  ................
-000048e0: 0c01 0e02 0601 04ff 7a12 4769 7444 6174  ........z.GitDat
-000048f0: 614d 676d 742e 636f 6e66 6967 6301 0000  aMgmt.configc...
-00004900: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00004910: 0047 0000 0072 a600 0000 a903 4e72 af00  .G...r......Nr..
-00004920: 0000 7203 0100 0072 a800 0000 72ac 0000  ..r....r....r...
-00004930: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-00004940: 7271 0000 0046 0200 0072 a900 0000 7a19  rq...F...r....z.
-00004950: 4769 7444 6174 614d 676d 742e 7365 6172  GitDataMgmt.sear
-00004960: 6368 5f6f 626a 6563 7463 0100 0000 0000  ch_objectc......
-00004970: 0000 0000 0000 0200 0000 0400 0000 4700  ..............G.
-00004980: 0000 72a6 0000 0072 0701 0000 72a8 0000  ..r....r....r...
-00004990: 0072 ac00 0000 721f 0000 0072 1f00 0000  .r....r....r....
-000049a0: 7237 0000 0072 7200 0000 4902 0000 72a9  r7...rr...I...r.
-000049b0: 0000 007a 1b47 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
-000049c0: 2e73 6561 7263 685f 6461 7461 5f73 6574  .search_data_set
-000049d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000049e0: 0004 0000 0047 0000 0072 a600 0000 2903  .....G...r....).
-000049f0: 4e72 6d00 0000 7203 0100 0072 a800 0000  Nrm...r....r....
-00004a00: 72ac 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-00004a10: 3700 0000 726d 0000 004c 0200 0072 a900  7...rm...L...r..
-00004a20: 0000 7a12 4769 7444 6174 614d 676d 742e  ..z.GitDataMgmt.
-00004a30: 7570 6c6f 6164 729b 0000 0072 9c00 0000  uploadr....r....
-00004a40: 729d 0000 0029 1c72 9e00 0000 729f 0000  r....).r....r...
-00004a50: 0072 a000 0000 72a1 0000 0072 4600 0000  .r....r....rF...
-00004a60: 724a 0000 0072 d600 0000 72d9 0000 0072  rJ...r....r....r
-00004a70: 4d00 0000 7251 0000 0072 c700 0000 7256  M...rQ...r....rV
-00004a80: 0000 0072 e900 0000 7257 0000 0072 5800  ...r....rW...rX.
-00004a90: 0000 72c3 0000 0072 b000 0000 72c5 0000  ..r....r....r...
-00004aa0: 0072 5f00 0000 72bf 0000 0072 6100 0000  .r_...r....ra...
-00004ab0: 7262 0000 0072 6400 0000 7269 0000 0072  rb...rd...ri...r
-00004ac0: 0400 0000 7271 0000 0072 7200 0000 726d  ....rq...rr...rm
-00004ad0: 0000 0072 1f00 0000 721f 0000 0072 1f00  ...r....r....r..
-00004ae0: 0000 7237 0000 0072 2c00 0000 9001 0000  ..r7...r,.......
-00004af0: 733a 0000 0008 0004 010a 0208 0908 0708  s:..............
-00004b00: 040a 040a 1302 200a 0108 0302 040c 0108  ...... .........
-00004b10: 1108 0d08 0608 0608 0502 040a 0108 040a  ................
-00004b20: 0408 0402 0702 010a ff08 1808 030c 0372  ...............r
-00004b30: 2c00 0000 6300 0000 0000 0000 0000 0000  ,...c...........
-00004b40: 0000 0000 0003 0000 0040 0000 0073 9e00  .........@...s..
-00004b50: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00004b60: 6403 8400 5a04 6404 6405 8400 5a05 6424  d...Z.d.d...Z.d$
-00004b70: 6407 6408 8401 5a06 6424 6409 640a 8401  d.d...Z.d$d.d...
-00004b80: 5a07 6425 640c 640d 8401 5a08 640e 640f  Z.d%d.d...Z.d.d.
-00004b90: 8400 5a09 6410 6411 8400 5a0a 6412 6413  ..Z.d.d...Z.d.d.
-00004ba0: 8400 5a0b 6414 6415 8400 5a0c 6416 6417  ..Z.d.d...Z.d.d.
-00004bb0: 8400 5a0d 6424 6418 6419 8401 5a0e 641a  ..Z.d$d.d...Z.d.
-00004bc0: 641b 8400 5a0f 641c 641d 8400 5a10 641e  d...Z.d.d...Z.d.
-00004bd0: 641f 8400 5a11 6420 6421 8400 5a12 0906  d...Z.d d!..Z...
-00004be0: 0906 6426 6422 6423 8401 5a13 6406 5300  ..d&d"d#..Z.d.S.
-00004bf0: 2927 7229 0000 007a 2844 6174 614d 676d  )'r)...z(DataMgm
-00004c00: 7420 6f70 6572 6174 696f 6e73 2066 6f72  t operations for
-00004c10: 2044 5353 2d73 746f 7265 6420 6461 7461   DSS-stored data
-00004c20: 2e63 0100 0000 0000 0000 0000 0000 0100  .c..............
-00004c30: 0000 0200 0000 4300 0000 7308 0000 0074  ......C...s....t
-00004c40: 00a0 01a1 0053 0072 9b00 0000 2902 7220  .....S.r....).r 
-00004c50: 0000 0072 2100 0000 7245 0000 0072 1f00  ...r!...rE...r..
-00004c60: 0000 721f 0000 0072 3700 0000 7246 0000  ..r....r7...rF..
-00004c70: 0053 0200 0073 0200 0000 0801 7a26 5068  .S...s......z&Ph
-00004c80: 7973 6963 616c 4461 7461 4d67 6d74 2e67  ysicalDataMgmt.g
-00004c90: 6574 5f73 6574 7469 6e67 735f 7265 736f  et_settings_reso
-00004ca0: 6c76 6572 6302 0000 0000 0000 0000 0000  lverc...........
-00004cb0: 0002 0000 0004 0000 0043 0000 0072 a600  .........C...r..
-00004cc0: 0000 2903 4e72 aa00 0000 fa38 5468 6973  ..).Nr.....8This
-00004cd0: 2063 6f6d 6d61 6e64 2069 7320 6f6e 6c79   command is only
-00004ce0: 2061 7661 696c 6162 6c65 2066 6f72 2045   available for E
-00004cf0: 7874 6572 6e61 6c20 4d61 6e61 6765 7220  xternal Manager 
-00004d00: 4461 7461 72a8 0000 0072 4800 0000 721f  Datar....rH...r.
-00004d10: 0000 0072 1f00 0000 7237 0000 0072 4a00  ...r....r7...rJ.
-00004d20: 0000 5602 0000 f306 0000 0006 0102 0108  ..V.............
-00004d30: ff7a 2550 6879 7369 6361 6c44 6174 614d  .z%PhysicalDataM
-00004d40: 676d 742e 7365 7475 705f 6c6f 6361 6c5f  gmt.setup_local_
-00004d50: 7365 7474 696e 6773 4e63 0200 0000 0000  settingsNc......
-00004d60: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00004d70: 0000 7364 0000 0074 006a 01a0 0264 01a1  ..sd...t.j...d..
-00004d80: 0172 0c74 0364 0264 0364 048d 0253 007c  .r.t.d.d.d...S.|
-00004d90: 006a 046a 05a0 06a1 0001 007c 006a 046a  .j.j.......|.j.j
-00004da0: 05a0 0764 0564 0664 07a1 0301 007c 006a  ...d.d.d.....|.j
-00004db0: 046a 05a0 08a1 0064 0819 007d 027c 006a  .j.....d...}.|.j
-00004dc0: 046a 05a0 0764 097c 0264 07a1 0301 0074  .j...d.|.d.....t
-00004dd0: 0364 0a64 0b64 048d 0253 0029 0c4e 721d  .d.d.d...S.).Nr.
-00004de0: 0000 0072 8f00 0000 72da 0000 0072 9100  ...r....r....r..
-00004df0: 0000 721e 0000 0054 7274 0000 00da 0b6f  ..r....Trt.....o
-00004e00: 7065 6e62 6973 5f75 726c da0f 6669 6c65  penbis_url..file
-00004e10: 7365 7276 6963 655f 7572 6c72 0100 0000  service_urlr....
-00004e20: 7a29 4d61 6e61 6765 6420 6461 7461 206f  z)Managed data o
-00004e30: 6269 7320 7265 706f 7369 746f 7279 2069  bis repository i
-00004e40: 6e69 7469 616c 697a 6564 2e29 0972 2300  nitialized.).r#.
-00004e50: 0000 7224 0000 0072 2500 0000 7205 0000  ..r$...r%...r...
-00004e60: 0072 2e00 0000 7204 0000 0072 df00 0000  .r....r....r....
-00004e70: 7296 0000 0072 2600 0000 2903 723c 0000  r....r&...).r<..
-00004e80: 0072 4c00 0000 720a 0100 0072 1f00 0000  .rL...r....r....
-00004e90: 721f 0000 0072 3700 0000 724d 0000 005a  r....r7...rM...Z
-00004ea0: 0200 0073 1200 0000 0c01 0c01 0c01 1201  ...s............
-00004eb0: 1001 0a01 0401 04ff 0c02 7a1a 5068 7973  ..........z.Phys
-00004ec0: 6963 616c 4461 7461 4d67 6d74 2e69 6e69  icalDataMgmt.ini
-00004ed0: 745f 6461 7461 6303 0000 0000 0000 0000  t_datac.........
-00004ee0: 0000 0003 0000 0004 0000 0043 0000 0072  ...........C...r
-00004ef0: a600 0000 2903 4e72 ab00 0000 7208 0100  ....).Nr....r...
-00004f00: 0072 a800 0000 724f 0000 0072 1f00 0000  .r....rO...r....
-00004f10: 721f 0000 0072 3700 0000 7251 0000 0064  r....r7...rQ...d
-00004f20: 0200 0072 0901 0000 7a1e 5068 7973 6963  ...r....z.Physic
-00004f30: 616c 4461 7461 4d67 6d74 2e69 6e69 745f  alDataMgmt.init_
-00004f40: 616e 616c 7973 6973 5463 0400 0000 0000  analysisTc......
-00004f50: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-00004f60: 0000 72a6 0000 0029 034e 7257 0000 0072  ..r....).NrW...r
-00004f70: 0801 0000 72a8 0000 0072 5300 0000 721f  ....r....rS...r.
-00004f80: 0000 0072 1f00 0000 7237 0000 0072 5700  ...r....r7...rW.
-00004f90: 0000 6802 0000 72a9 0000 007a 1750 6879  ..h...r....z.Phy
-00004fa0: 7369 6361 6c44 6174 614d 676d 742e 636f  sicalDataMgmt.co
-00004fb0: 6d6d 6974 6301 0000 0000 0000 0000 0000  mmitc...........
-00004fc0: 0001 0000 0004 0000 0043 0000 0072 a600  .........C...r..
-00004fd0: 0000 2903 4e72 5600 0000 7208 0100 0072  ..).NrV...r....r
-00004fe0: a800 0000 7245 0000 0072 1f00 0000 721f  ....rE...r....r.
-00004ff0: 0000 0072 3700 0000 7256 0000 006b 0200  ...r7...rV...k..
-00005000: 0072 a900 0000 7a15 5068 7973 6963 616c  .r....z.Physical
-00005010: 4461 7461 4d67 6d74 2e73 796e 6363 0100  DataMgmt.syncc..
-00005020: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00005030: 0000 4300 0000 72a6 0000 0029 034e 7258  ..C...r....).NrX
-00005040: 0000 0072 0801 0000 72a8 0000 0072 4500  ...r....r....rE.
-00005050: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00005060: 0072 5800 0000 6e02 0000 72a9 0000 007a  .rX...n...r....z
-00005070: 1750 6879 7369 6361 6c44 6174 614d 676d  .PhysicalDataMgm
-00005080: 742e 7374 6174 7573 6305 0000 0000 0000  t.statusc.......
-00005090: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-000050a0: 0072 a600 0000 2903 4e72 5f00 0000 7208  .r....).Nr_...r.
-000050b0: 0100 0072 a800 0000 725a 0000 0072 1f00  ...r....rZ...r..
-000050c0: 0000 721f 0000 0072 3700 0000 725f 0000  ..r....r7...r_..
-000050d0: 0071 0200 0072 a900 0000 7a16 5068 7973  .q...r....z.Phys
-000050e0: 6963 616c 4461 7461 4d67 6d74 2e63 6c6f  icalDataMgmt.clo
-000050f0: 6e65 6305 0000 0000 0000 0000 0000 0005  nec.............
-00005100: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
-00005110: 2903 4e72 6100 0000 7208 0100 0072 a800  ).Nra...r....r..
-00005120: 0000 725a 0000 0072 1f00 0000 721f 0000  ..rZ...r....r...
-00005130: 0072 3700 0000 7261 0000 0074 0200 0072  .r7...ra...t...r
-00005140: a900 0000 7a15 5068 7973 6963 616c 4461  ....z.PhysicalDa
-00005150: 7461 4d67 6d74 2e6d 6f76 6563 0100 0000  taMgmt.movec....
-00005160: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00005170: 4300 0000 72a6 0000 0029 034e 7262 0000  C...r....).Nrb..
-00005180: 0072 0801 0000 72a8 0000 0072 4500 0000  .r....r....rE...
-00005190: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
-000051a0: 6200 0000 7702 0000 72a9 0000 007a 1750  b...w...r....z.P
-000051b0: 6879 7369 6361 6c44 6174 614d 676d 742e  hysicalDataMgmt.
-000051c0: 6164 6472 6566 6302 0000 0000 0000 0000  addrefc.........
-000051d0: 0000 0002 0000 0004 0000 0043 0000 0072  ...........C...r
-000051e0: a600 0000 2903 4e72 6400 0000 7208 0100  ....).Nrd...r...
-000051f0: 0072 a800 0000 7263 0000 0072 1f00 0000  .r....rc...r....
-00005200: 721f 0000 0072 3700 0000 7264 0000 007a  r....r7...rd...z
-00005210: 0200 0072 a900 0000 7a1a 5068 7973 6963  ...r....z.Physic
-00005220: 616c 4461 7461 4d67 6d74 2e72 656d 6f76  alDataMgmt.remov
-00005230: 6572 6566 6305 0000 0000 0000 0000 0000  erefc...........
-00005240: 0006 0000 0006 0000 0043 0000 0072 0001  .........C...r..
-00005250: 0000 729b 0000 0029 0272 0900 0000 72ea  ..r....).r....r.
-00005260: 0000 0029 0672 3c00 0000 725b 0000 0072  ...).r<...r[...r
-00005270: 6700 0000 7268 0000 0072 5e00 0000 72ec  g...rh...r^...r.
-00005280: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
-00005290: 0000 7269 0000 007d 0200 0072 0201 0000  ..ri...}...r....
-000052a0: 7a19 5068 7973 6963 616c 4461 7461 4d67  z.PhysicalDataMg
-000052b0: 6d74 2e64 6f77 6e6c 6f61 6463 0400 0000  mt.downloadc....
-000052c0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-000052d0: 4300 0000 7316 0000 0074 007c 007c 017c  C...s....t.|.|.|
-000052e0: 027c 0383 047d 047c 04a0 01a1 0053 0072  .|...}.|.....S.r
-000052f0: 9b00 0000 2902 720f 0000 0072 ea00 0000  ....).r....r....
-00005300: 2905 723c 0000 0072 6a00 0000 726b 0000  ).r<...rj...rk..
-00005310: 0072 6c00 0000 72ec 0000 0072 1f00 0000  .rl...r....r....
-00005320: 721f 0000 0072 3700 0000 726d 0000 0081  r....r7...rm....
-00005330: 0200 0073 0400 0000 0e01 0801 7a17 5068  ...s........z.Ph
-00005340: 7973 6963 616c 4461 7461 4d67 6d74 2e75  ysicalDataMgmt.u
-00005350: 706c 6f61 6463 0300 0000 0000 0000 0000  ploadc..........
-00005360: 0000 0400 0000 0400 0000 4300 0000 f314  ..........C.....
-00005370: 0000 0074 007c 007c 017c 0283 037d 037c  ...t.|.|.|...}.|
-00005380: 03a0 01a1 0053 0072 9b00 0000 2902 720e  .....S.r....).r.
-00005390: 0000 00da 0e73 6561 7263 685f 7361 6d70  .....search_samp
-000053a0: 6c65 73a9 0472 3c00 0000 726f 0000 0072  les..r<...ro...r
-000053b0: 7000 0000 72ec 0000 0072 1f00 0000 721f  p...r....r....r.
-000053c0: 0000 0072 3700 0000 7271 0000 0085 0200  ...r7...rq......
-000053d0: 0072 ed00 0000 7a1e 5068 7973 6963 616c  .r....z.Physical
-000053e0: 4461 7461 4d67 6d74 2e73 6561 7263 685f  DataMgmt.search_
-000053f0: 6f62 6a65 6374 6303 0000 0000 0000 0000  objectc.........
-00005400: 0000 0004 0000 0004 0000 0043 0000 0072  ...........C...r
-00005410: 0c01 0000 729b 0000 0029 0272 0e00 0000  ....r....).r....
-00005420: da10 7365 6172 6368 5f64 6174 615f 7365  ..search_data_se
-00005430: 7473 720e 0100 0072 1f00 0000 721f 0000  tsr....r....r...
-00005440: 0072 3700 0000 7272 0000 0089 0200 0072  .r7...rr.......r
-00005450: ed00 0000 7a20 5068 7973 6963 616c 4461  ....z PhysicalDa
-00005460: 7461 4d67 6d74 2e73 6561 7263 685f 6461  taMgmt.search_da
-00005470: 7461 5f73 6574 6307 0000 0000 0000 0000  ta_setc.........
-00005480: 0000 0009 0000 0009 0000 0043 0000 0073  ...........C...s
-00005490: f600 0000 7c00 6a00 a001 7c01 a101 7d07  ....|.j...|...}.
-000054a0: 7c07 6401 7500 7210 7402 6402 7c01 1700  |.d.u.r.t.d.|...
-000054b0: 8301 8201 7c04 7403 6a04 7500 7222 7c05  ....|.t.j.u.r"|.
-000054c0: 6401 7501 731b 4a00 8201 7c06 6401 7501  d.u.s.J...|.d.u.
-000054d0: 7321 4a00 8201 6e1e 7c04 7403 6a05 7500  s!J...n.|.t.j.u.
-000054e0: 722e 7c06 6401 7500 732d 4a00 8201 6e12  r.|.d.u.s-J...n.
-000054f0: 7c04 7403 6a06 7500 7240 7c01 6403 6b03  |.t.j.u.r@|.d.k.
-00005500: 7240 7c00 a007 7c01 9b00 6404 9d02 6405  r@|...|...d...d.
-00005510: a102 0100 7c01 6406 6b02 724f 7408 7c00  ....|.d.k.rOt.|.
-00005520: 7c04 7c05 7c06 8304 7d08 7c08 a009 a100  |.|.|...}.|.....
-00005530: 5300 7c01 6407 6b02 725e 740a 7c00 7c04  S.|.d.k.r^t.|.|.
-00005540: 7c05 7c06 8304 7d08 7c08 a009 a100 5300  |.|...}.|.....S.
-00005550: 7c01 6403 6b02 726e 7c00 a00b 7c07 7c00  |.d.k.rn|...|.|.
-00005560: 6a0c 7c02 7c03 7c04 7c05 7c06 a107 5300  j.|.|.|.|.|...S.
-00005570: 7c00 a007 7c01 9b00 6408 7c04 9b00 9d03  |...|...d.|.....
-00005580: 6405 a102 0100 6401 5300 2909 7204 0100  d.....d.S.).r...
-00005590: 004e 7205 0100 0072 0400 0000 7a06 2063  .Nr....r....z. c
-000055a0: 6c65 6172 7208 0100 00da 066f 626a 6563  learr......objec
-000055b0: 74da 0a63 6f6c 6c65 6374 696f 6efa 0120  t..collection.. 
-000055c0: 290d 722e 0000 0072 d500 0000 723f 0000  ).r....r....r?..
-000055d0: 0072 1200 0000 727f 0000 0072 7b00 0000  .r....r....r{...
-000055e0: 7281 0000 0072 4300 0000 720b 0000 0072  r....rC...r....r
-000055f0: ea00 0000 7208 0000 0072 8c00 0000 7233  ....r....r....r3
-00005600: 0000 0029 0972 3c00 0000 7206 0100 0072  ...).r<...r....r
-00005610: 8400 0000 7285 0000 0072 8600 0000 7287  ....r....r....r.
-00005620: 0000 0072 8800 0000 7283 0000 0072 ec00  ...r....r....r..
-00005630: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00005640: 0072 0400 0000 8d02 0000 7332 0000 000c  .r........s2....
-00005650: 0a08 010c 010a 010c 010e 010a 010e 0112  ................
-00005660: 010c 0102 0104 ff08 030e 0108 0108 010e  ................
-00005670: 0108 0108 010e 0106 0104 ff10 0302 0108  ................
-00005680: ff7a 1750 6879 7369 6361 6c44 6174 614d  .z.PhysicalDataM
-00005690: 676d 742e 636f 6e66 6967 729b 0000 0072  gmt.configr....r
-000056a0: 9c00 0000 729d 0000 0029 1472 9e00 0000  ....r....).r....
-000056b0: 729f 0000 0072 a000 0000 72a1 0000 0072  r....r....r....r
-000056c0: 4600 0000 724a 0000 0072 4d00 0000 7251  F...rJ...rM...rQ
-000056d0: 0000 0072 5700 0000 7256 0000 0072 5800  ...rW...rV...rX.
-000056e0: 0000 725f 0000 0072 6100 0000 7262 0000  ..r_...ra...rb..
-000056f0: 0072 6400 0000 7269 0000 0072 6d00 0000  .rd...ri...rm...
-00005700: 7271 0000 0072 7200 0000 7204 0000 0072  rq...rr...r....r
-00005710: 1f00 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
-00005720: 0000 0072 2900 0000 5002 0000 7328 0000  ...r)...P...s(..
-00005730: 0008 0004 0108 0208 030a 040a 0a0a 0408  ................
-00005740: 0308 0308 0308 0308 030a 0308 0308 0408  ................
-00005750: 0408 0402 0402 010e ff72 2900 0000 2938  .........r)...)8
-00005760: 72a2 0000 0072 7c00 0000 7223 0000 0072  r....r|...r#...r
-00005770: fc00 0000 72c0 0000 0072 b100 0000 da07  ....r....r......
-00005780: 7061 7468 6c69 6272 0200 0000 72f4 0000  pathlibr....r...
-00005790: 0072 9400 0000 7204 0000 0072 2000 0000  .r....r....r ...
-000057a0: da0e 636f 6d6d 616e 645f 7265 7375 6c74  ..command_result
-000057b0: 7205 0000 00da 0f63 6f6d 6d61 6e64 732e  r......commands.
-000057c0: 6164 6472 6566 7206 0000 00da 0e63 6f6d  addrefr......com
-000057d0: 6d61 6e64 732e 636c 6f6e 6572 0700 0000  mands.cloner....
-000057e0: da13 636f 6d6d 616e 6473 2e63 6f6c 6c65  ..commands.colle
-000057f0: 6374 696f 6e72 0800 0000 da1a 636f 6d6d  ctionr......comm
-00005800: 616e 6473 2e64 6f77 6e6c 6f61 645f 7068  ands.download_ph
-00005810: 7973 6963 616c 7209 0000 00da 0d63 6f6d  ysicalr......com
-00005820: 6d61 6e64 732e 6d6f 7665 720a 0000 00da  mands.mover.....
-00005830: 0f63 6f6d 6d61 6e64 732e 6f62 6a65 6374  .commands.object
-00005840: 720b 0000 00da 1563 6f6d 6d61 6e64 732e  r......commands.
-00005850: 6f70 656e 6269 735f 7379 6e63 720c 0000  openbis_syncr...
-00005860: 00da 1263 6f6d 6d61 6e64 732e 7265 6d6f  ...commands.remo
-00005870: 7665 7265 6672 0d00 0000 da0f 636f 6d6d  verefr......comm
-00005880: 616e 6473 2e73 6561 7263 6872 0e00 0000  ands.searchr....
-00005890: da0f 636f 6d6d 616e 6473 2e75 706c 6f61  ..commands.uploa
-000058a0: 6472 0f00 0000 da03 6769 7472 1000 0000  dr......gitr....
-000058b0: da05 7574 696c 7372 1100 0000 7212 0000  ..utilsr....r...
-000058c0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-000058d0: 7216 0000 00da 1273 6372 6970 7473 2e63  r......scripts.c
-000058e0: 6c69 636b 5f75 7469 6c72 1800 0000 7219  lick_utilr....r.
-000058f0: 0000 0072 2200 0000 7238 0000 00da 0741  ...r"...r8.....A
-00005900: 4243 4d65 7461 7239 0000 0072 2b00 0000  BCMetar9...r+...
-00005910: 72b4 0000 0072 bf00 0000 72c7 0000 0072  r....r....r....r
-00005920: 2c00 0000 7229 0000 0072 1f00 0000 721f  ,...r)...r....r.
-00005930: 0000 0072 1f00 0000 7237 0000 00da 083c  ...r....r7.....<
-00005940: 6d6f 6475 6c65 3e01 0000 0073 4e00 0000  module>....sN...
-00005950: 0811 0801 0801 0801 0801 0801 0c01 0802  ................
-00005960: 0c02 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00005970: 0c01 0c01 0c01 0c01 0c01 1001 0c01 0c01  ................
-00005980: 0c01 0c01 1001 0804 0c01 0aff 1428 007f  .............(..
-00005990: 1058 0831 0805 0812 1017 007f 1441       .X.1.........A
+000003b0: 0a6b 0272 5274 0c7c 027c 0183 0201 0074  .k.rRt.|.|.....t
+000003c0: 0d7c 017c 0264 017c 047c 057c 097c 0a7c  .|.|.d.|.|.|.|.|
+000003d0: 0b83 0853 0074 0e7c 0383 0101 0074 0f64  ...S.t.|.....t.d
+000003e0: 0869 007c 03a4 018e 017d 0d7c 0da0 10a1  .i.|.....}.|....
+000003f0: 0073 6c74 117c 0164 017c 0d7c 047c 057c  .slt.|.d.|.|.|.|
+00000400: 097c 0a7c 0b83 0853 0074 0c7c 027c 0183  .|.|...S.t.|.|..
+00000410: 0201 0074 127c 017c 027c 0d7c 047c 057c  ...t.|.|.|.|.|.|
+00000420: 097c 0a7c 0b7c 067c 0783 0a53 0029 097a  .|.|.|.|...S.).z
+00000430: 2546 6163 746f 7279 206d 6574 686f 6420  %Factory method 
+00000440: 666f 7220 4461 7461 4d67 6d74 2069 6e73  for DataMgmt ins
+00000450: 7461 6e63 6573 4eda 0964 6174 615f 7061  tancesN..data_pa
+00000460: 7468 da0d 6d65 7461 6461 7461 5f70 6174  th..metadata_pat
+00000470: 68da 0f69 6e76 6f63 6174 696f 6e5f 7061  h..invocation_pa
+00000480: 7468 fa05 2e6f 6269 73da 0b69 735f 7068  th...obis..is_ph
+00000490: 7973 6963 616c 54a9 0029 1372 1600 0000  ysicalT..).r....
+000004a0: da09 646d 5f63 6f6e 6669 67da 1053 6574  ..dm_config..Set
+000004b0: 7469 6e67 7352 6573 6f6c 7665 7272 1100  tingsResolverr..
+000004c0: 0000 da07 554e 4b4e 4f57 4eda 026f 73da  ....UNKNOWN..os.
+000004d0: 0470 6174 68da 0665 7869 7374 7372 0400  .path..existsr..
+000004e0: 0000 da0b 636f 6e66 6967 5f64 6963 74da  ....config_dict.
+000004f0: 0850 4859 5349 4341 4cda 044c 494e 4b72  .PHYSICAL..LINKr
+00000500: 1500 0000 da10 5068 7973 6963 616c 4461  ......PhysicalDa
+00000510: 7461 4d67 6d74 7214 0000 0072 1000 0000  taMgmtr....r....
+00000520: da07 6361 6e5f 7275 6eda 0d4e 6f47 6974  ..can_run..NoGit
+00000530: 4461 7461 4d67 6d74 da0b 4769 7444 6174  DataMgmt..GitDat
+00000540: 614d 676d 7429 0eda 0965 6368 6f5f 6675  aMgmt)...echo_fu
+00000550: 6e63 da11 7365 7474 696e 6773 5f72 6573  nc..settings_res
+00000560: 6f6c 7665 72da 0e6f 7065 6e62 6973 5f63  olver..openbis_c
+00000570: 6f6e 6669 67da 0a67 6974 5f63 6f6e 6669  onfig..git_confi
+00000580: 67da 076f 7065 6e62 6973 da03 6c6f 67da  g..openbis..log.
+00000590: 0564 6562 7567 da05 6c6f 6769 6eda 0f72  .debug..login..r
+000005a0: 6570 6f73 6974 6f72 795f 7479 7065 721a  epository_typer.
+000005b0: 0000 0072 1b00 0000 721c 0000 0072 2600  ...r....r....r&.
+000005c0: 0000 da0b 6769 745f 7772 6170 7065 7272  ....git_wrapperr
+000005d0: 1f00 0000 721f 0000 00fa 5d2f 686f 6d65  ....r.....]/home
+000005e0: 2f61 6c61 736b 6f77 736b 692f 7265 706f  /alaskowski/repo
+000005f0: 2f6f 7065 6e62 6973 5f70 7974 686f 6e2f  /openbis_python/
+00000600: 6170 702d 6f70 656e 6269 732d 636f 6d6d  app-openbis-comm
+00000610: 616e 642d 6c69 6e65 2f73 7263 2f70 7974  and-line/src/pyt
+00000620: 686f 6e2f 6f62 6973 2f64 6d2f 6461 7461  hon/obis/dm/data
+00000630: 5f6d 676d 742e 7079 da08 4461 7461 4d67  _mgmt.py..DataMg
+00000640: 6d74 3200 0000 7338 0000 0010 0408 0208  mt2...s8........
+00000650: 0108 0108 0208 010a 020c 010a 010c 0108  ................
+00000660: 0108 0206 020a 020a 010e 0104 0104 ff08  ................
+00000670: 030e 0108 010e 0304 0104 ff0a 030e 0108  ................
+00000680: 0104 ff72 3800 0000 6300 0000 0000 0000  ...r8...c.......
+00000690: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
+000006a0: 0073 1a01 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000006b0: 5a03 0903 642b 6404 6405 8401 5a04 6406  Z...d+d.d...Z.d.
+000006c0: 6407 8400 5a05 6506 6a07 6408 6409 8400  d...Z.e.j.d.d...
+000006d0: 8301 5a08 6506 6a07 640a 640b 8400 8301  ..Z.e.j.d.d.....
+000006e0: 5a09 6506 6a07 642c 640d 640e 8401 8301  Z.e.j.d,d.d.....
+000006f0: 5a0a 6506 6a07 642c 640f 6410 8401 8301  Z.e.j.d,d.d.....
+00000700: 5a0b 6506 6a07 642d 6411 6412 8401 8301  Z.e.j.d-d.d.....
+00000710: 5a0c 6506 6a07 6413 6414 8400 8301 5a0d  Z.e.j.d.d.....Z.
+00000720: 6506 6a07 6415 6416 8400 8301 5a0e 6506  e.j.d.d.....Z.e.
+00000730: 6a07 6417 6418 8400 8301 5a0f 6506 6a07  j.d.d.....Z.e.j.
+00000740: 6419 641a 8400 8301 5a10 6506 6a07 641b  d.d.....Z.e.j.d.
+00000750: 641c 8400 8301 5a11 6506 6a07 642c 641d  d.....Z.e.j.d,d.
+00000760: 641e 8401 8301 5a12 6506 6a07 641f 6420  d.....Z.e.j.d.d 
+00000770: 8400 8301 5a13 6506 6a07 6421 6422 8400  ....Z.e.j.d!d"..
+00000780: 8301 5a14 6506 6a07 6423 6424 8400 8301  ..Z.e.j.d#d$....
+00000790: 5a15 6506 6a07 6425 6426 8400 8301 5a16  Z.e.j.d%d&....Z.
+000007a0: 090c 090c 642e 6427 6428 8401 5a17 6518  ....d.d'd(..Z.e.
+000007b0: 642f 6429 642a 8401 8301 5a19 640c 5300  d/d)d*....Z.d.S.
+000007c0: 2930 da10 4162 7374 7261 6374 4461 7461  )0..AbstractData
+000007d0: 4d67 6d74 7a65 4162 7374 7261 6374 206f  MgmtzeAbstract o
+000007e0: 626a 6563 7420 7468 6174 2069 6d70 6c65  bject that imple
+000007f0: 6d65 6e74 7320 6f70 6572 6174 696f 6e73  ments operations
+00000800: 2e0a 0a20 2020 2041 6c6c 206f 7065 7261  ...    All opera
+00000810: 7469 6f6e 7320 7468 726f 7720 616e 2065  tions throw an e
+00000820: 7865 7063 7469 6f6e 2069 6620 7468 6579  xepction if they
+00000830: 2066 6169 6c2e 0a20 2020 2046 5463 0b00   fail..    FTc..
+00000840: 0000 0000 0000 0000 0000 0b00 0000 0200  ................
+00000850: 0000 4300 0000 734c 0000 007c 017c 005f  ..C...sL...|.|._
+00000860: 007c 027c 005f 017c 037c 005f 027c 047c  .|.|._.|.|._.|.|
+00000870: 005f 037c 057c 005f 047c 067c 005f 057c  ._.|.|._.|.|._.|
+00000880: 077c 005f 067c 087c 005f 077c 097c 005f  .|._.|.|._.|.|._
+00000890: 087c 0a7c 005f 0964 017c 005f 0a64 027c  .|.|._.d.|._.d.|
+000008a0: 005f 0b64 0053 0029 034e 5446 290c 722e  ._.d.S.).NTF).r.
+000008b0: 0000 0072 2f00 0000 7236 0000 0072 3100  ...r/...r6...r1.
+000008c0: 0000 7232 0000 0072 1a00 0000 721b 0000  ..r2...r....r...
+000008d0: 0072 1c00 0000 7233 0000 0072 3400 0000  .r....r3...r4...
+000008e0: da11 7265 7374 6f72 655f 6f6e 5f73 6967  ..restore_on_sig
+000008f0: 696e 74da 1569 676e 6f72 655f 6d69 7373  int..ignore_miss
+00000900: 696e 675f 7061 7265 6e74 290b da04 7365  ing_parent)...se
+00000910: 6c66 722e 0000 0072 2f00 0000 7236 0000  lfr....r/...r6..
+00000920: 0072 3100 0000 7232 0000 0072 1a00 0000  .r1...r2...r....
+00000930: 721b 0000 0072 1c00 0000 7233 0000 0072  r....r....r3...r
+00000940: 3400 0000 721f 0000 0072 1f00 0000 7237  4...r....r....r7
+00000950: 0000 00da 085f 5f69 6e69 745f 5f61 0000  .....__init__a..
+00000960: 0073 1800 0000 0602 0601 0601 0601 0601  .s..............
+00000970: 0601 0601 0601 0601 0601 0603 0a01 7a19  ..............z.
+00000980: 4162 7374 7261 6374 4461 7461 4d67 6d74  AbstractDataMgmt
+00000990: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
+000009a0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
+000009b0: 0000 7314 0000 0064 01a0 007c 017c 02a1  ..s....d...|.|..
+000009c0: 027d 0374 017c 0383 0182 0129 027a 1352  .}.t.|.....).z.R
+000009d0: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+000009e0: 6e2e 7a0f 277b 7d27 2066 6169 6c65 642e  n.z.'{}' failed.
+000009f0: 207b 7d29 02da 0666 6f72 6d61 74da 0a56   {})...format..V
+00000a00: 616c 7565 4572 726f 7229 0472 3c00 0000  alueError).r<...
+00000a10: da07 636f 6d6d 616e 64da 0672 6561 736f  ..command..reaso
+00000a20: 6eda 076d 6573 7361 6765 721f 0000 0072  n..messager....r
+00000a30: 1f00 0000 7237 0000 00da 0b65 7272 6f72  ....r7.....error
+00000a40: 5f72 6169 7365 7200 0000 7304 0000 000c  _raiser...s.....
+00000a50: 0208 017a 1c41 6273 7472 6163 7444 6174  ...z.AbstractDat
+00000a60: 614d 676d 742e 6572 726f 725f 7261 6973  aMgmt.error_rais
+00000a70: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
+00000a80: 0000 0100 0000 4300 0000 f304 0000 0064  ......C........d
+00000a90: 0153 0029 027a 1b20 4765 7420 7468 6520  .S.).z. Get the 
+00000aa0: 7365 7474 696e 6773 2072 6573 6f6c 7665  settings resolve
+00000ab0: 7220 4e72 1f00 0000 a901 723c 0000 0072  r Nr......r<...r
+00000ac0: 1f00 0000 721f 0000 0072 3700 0000 da15  ....r....r7.....
+00000ad0: 6765 745f 7365 7474 696e 6773 5f72 6573  get_settings_res
+00000ae0: 6f6c 7665 7277 0000 00f3 0200 0000 0403  olverw..........
+00000af0: 7a26 4162 7374 7261 6374 4461 7461 4d67  z&AbstractDataMg
+00000b00: 6d74 2e67 6574 5f73 6574 7469 6e67 735f  mt.get_settings_
+00000b10: 7265 736f 6c76 6572 6302 0000 0000 0000  resolverc.......
+00000b20: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
+00000b30: 0072 4400 0000 2902 7a34 2053 6574 7570  .rD...).z4 Setup
+00000b40: 206c 6f63 616c 2073 6574 7469 6e67 7320   local settings 
+00000b50: 2d20 666f 7220 7573 696e 6720 6f62 6973  - for using obis
+00000b60: 2061 7320 6120 6c69 6272 6172 7920 4e72   as a library Nr
+00000b70: 1f00 0000 a902 723c 0000 00da 0c61 6c6c  ......r<.....all
+00000b80: 5f73 6574 7469 6e67 7372 1f00 0000 721f  _settingsr....r.
+00000b90: 0000 0072 3700 0000 da14 7365 7475 705f  ...r7.....setup_
+00000ba0: 6c6f 6361 6c5f 7365 7474 696e 6773 7c00  local_settings|.
+00000bb0: 0000 7247 0000 007a 2541 6273 7472 6163  ..rG...z%Abstrac
+00000bc0: 7444 6174 614d 676d 742e 7365 7475 705f  tDataMgmt.setup_
+00000bd0: 6c6f 6361 6c5f 7365 7474 696e 6773 4e63  local_settingsNc
+00000be0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00000bf0: 0100 0000 4300 0000 7244 0000 0029 0261  ....C...rD...).a
+00000c00: 4b01 0000 496e 6974 6961 6c69 7a65 2061  K...Initialize a
+00000c10: 2064 6174 6120 7265 706f 7369 746f 7279   data repository
+00000c20: 2061 7420 7468 6520 7061 7468 2077 6974   at the path wit
+00000c30: 6820 7468 6520 6465 7363 7269 7074 696f  h the descriptio
+00000c40: 6e2e 0a20 2020 2020 2020 203a 7061 7261  n..        :para
+00000c50: 6d20 7061 7468 3a20 5061 7468 2066 6f72  m path: Path for
+00000c60: 2074 6865 2072 6570 6f73 6974 6f72 792e   the repository.
+00000c70: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000c80: 6465 7363 3a20 416e 206f 7074 696f 6e61  desc: An optiona
+00000c90: 6c20 7368 6f72 7420 6465 7363 7269 7074  l short descript
+00000ca0: 696f 6e20 6f66 2074 6865 2072 6570 6f73  ion of the repos
+00000cb0: 6974 6f72 7920 2875 7365 6420 6279 2067  itory (used by g
+00000cc0: 6974 2d61 6e6e 6578 290a 2020 2020 2020  it-annex).      
+00000cd0: 2020 3a70 6172 616d 2063 7265 6174 653a    :param create:
+00000ce0: 2049 6620 5472 7565 2061 6e64 2074 6865   If True and the
+00000cf0: 2066 6f6c 6465 7220 646f 6573 206e 6f74   folder does not
+00000d00: 2065 7869 7374 2c20 6372 6561 7465 2069   exist, create i
+00000d10: 742e 2044 6566 6175 6c74 7320 746f 2074  t. Defaults to t
+00000d20: 7275 652e 0a20 2020 2020 2020 203a 7265  rue..        :re
+00000d30: 7475 726e 3a20 4120 436f 6d6d 616e 6452  turn: A CommandR
+00000d40: 6573 756c 742e 0a20 2020 2020 2020 204e  esult..        N
+00000d50: 721f 0000 00a9 0272 3c00 0000 da04 6465  r......r<.....de
+00000d60: 7363 721f 0000 0072 1f00 0000 7237 0000  scr....r....r7..
+00000d70: 00da 0969 6e69 745f 6461 7461 8100 0000  ...init_data....
+00000d80: f302 0000 0004 087a 1a41 6273 7472 6163  .......z.Abstrac
+00000d90: 7444 6174 614d 676d 742e 696e 6974 5f64  tDataMgmt.init_d
+00000da0: 6174 6163 0300 0000 0000 0000 0000 0000  atac............
+00000db0: 0300 0000 0100 0000 4300 0000 7244 0000  ........C...rD..
+00000dc0: 0029 027a f549 6e69 7469 616c 697a 6520  .).z.Initialize 
+00000dd0: 616e 2061 6e61 6c79 7369 7320 7265 706f  an analysis repo
+00000de0: 7369 746f 7279 2061 7420 7468 6520 7061  sitory at the pa
+00000df0: 7468 2e0a 2020 2020 2020 2020 3a70 6172  th..        :par
+00000e00: 616d 2070 6172 656e 745f 666f 6c64 6572  am parent_folder
+00000e10: 3a20 5061 7468 2066 6f72 2074 6865 2072  : Path for the r
+00000e20: 6570 6f73 6974 6f72 792e 0a20 2020 2020  epository..     
+00000e30: 2020 203a 7061 7261 6d20 7061 7265 6e74     :param parent
+00000e40: 3a20 2872 6571 7569 7265 6420 7768 656e  : (required when
+00000e50: 206f 7574 7369 6465 206f 6620 6578 6973   outside of exis
+00000e60: 7469 6e67 2072 6570 6f73 6974 6f72 7929  ting repository)
+00000e70: 2050 6174 6820 666f 7220 7468 6520 7061   Path for the pa
+00000e80: 7265 6e74 2072 6570 6f73 6974 6f72 740a  rent repositort.
+00000e90: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00000ea0: 2041 2043 6f6d 6d61 6e64 5265 7375 6c74   A CommandResult
+00000eb0: 2e0a 2020 2020 2020 2020 4e72 1f00 0000  ..        Nr....
+00000ec0: a903 723c 0000 00da 0d70 6172 656e 745f  ..r<.....parent_
+00000ed0: 666f 6c64 6572 724c 0000 0072 1f00 0000  folderrL...r....
+00000ee0: 721f 0000 0072 3700 0000 da0d 696e 6974  r....r7.....init
+00000ef0: 5f61 6e61 6c79 7369 738b 0000 00f3 0200  _analysis.......
+00000f00: 0000 0407 7a1e 4162 7374 7261 6374 4461  ....z.AbstractDa
+00000f10: 7461 4d67 6d74 2e69 6e69 745f 616e 616c  taMgmt.init_anal
+00000f20: 7973 6973 6304 0000 0000 0000 0000 0000  ysisc...........
+00000f30: 0004 0000 0001 0000 0043 0000 0072 4400  .........C...rD.
+00000f40: 0000 2902 615e 0100 0043 6f6d 6d69 7420  ..).a^...Commit 
+00000f50: 7468 6520 6375 7272 656e 7420 7265 706f  the current repo
+00000f60: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+00000f70: 6973 7375 6573 2061 2067 6974 2063 6f6d  issues a git com
+00000f80: 6d69 7420 616e 6420 636f 6e6e 6563 7473  mit and connects
+00000f90: 2074 6f20 6f70 656e 4249 5320 616e 6420   to openBIS and 
+00000fa0: 6372 6561 7465 7320 6120 6461 7461 2073  creates a data s
+00000fb0: 6574 2069 6e20 6f70 656e 4249 532e 0a20  et in openBIS.. 
+00000fc0: 2020 2020 2020 203a 7061 7261 6d20 6d73         :param ms
+00000fd0: 673a 2043 6f6d 6d69 7420 6d65 7373 6167  g: Commit messag
+00000fe0: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
+00000ff0: 6d20 6175 746f 5f61 6464 3a20 4175 746f  m auto_add: Auto
+00001000: 6d61 7469 6361 6c6c 7920 6164 6420 616c  matically add al
+00001010: 6c20 6669 6c65 7320 696e 2074 6865 2066  l files in the f
+00001020: 6f6c 6465 7220 746f 2074 6865 2072 6570  older to the rep
+00001030: 6f2e 2044 6566 6175 6c74 7320 746f 2054  o. Defaults to T
+00001040: 7275 652e 0a20 2020 2020 2020 203a 7061  rue..        :pa
+00001050: 7261 6d20 7379 6e63 3a20 4966 2074 7275  ram sync: If tru
+00001060: 652c 2073 796e 6320 7769 7468 206f 7065  e, sync with ope
+00001070: 6e42 4953 2073 6572 7665 722e 0a20 2020  nBIS server..   
+00001080: 2020 2020 203a 7265 7475 726e 3a20 4120       :return: A 
+00001090: 436f 6d6d 616e 6452 6573 756c 742e 0a20  CommandResult.. 
+000010a0: 2020 2020 2020 204e 721f 0000 00a9 0472         Nr......r
+000010b0: 3c00 0000 da03 6d73 67da 0861 7574 6f5f  <.....msg..auto_
+000010c0: 6164 64da 0473 796e 6372 1f00 0000 721f  add..syncr....r.
+000010d0: 0000 0072 3700 0000 da06 636f 6d6d 6974  ...r7.....commit
+000010e0: 9400 0000 7302 0000 0004 0a7a 1741 6273  ....s......z.Abs
+000010f0: 7472 6163 7444 6174 614d 676d 742e 636f  tractDataMgmt.co
+00001100: 6d6d 6974 6301 0000 0000 0000 0000 0000  mmitc...........
+00001110: 0001 0000 0001 0000 0043 0000 0072 4400  .........C...rD.
+00001120: 0000 2902 7a86 5379 6e63 2074 6865 2063  ..).z.Sync the c
+00001130: 7572 7265 6e74 2072 6570 6f2e 0a0a 2020  urrent repo...  
+00001140: 2020 2020 2020 5468 6973 2063 6f6e 6e65        This conne
+00001150: 6374 7320 746f 206f 7065 6e42 4953 2061  cts to openBIS a
+00001160: 6e64 2063 7265 6174 6573 2061 2064 6174  nd creates a dat
+00001170: 6120 7365 7420 696e 206f 7065 6e42 4953  a set in openBIS
+00001180: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00001190: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
+000011a0: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
+000011b0: 0000 7245 0000 0072 1f00 0000 721f 0000  ..rE...r....r...
+000011c0: 0072 3700 0000 7256 0000 00a0 0000 0072  .r7...rV.......r
+000011d0: 5200 0000 7a15 4162 7374 7261 6374 4461  R...z.AbstractDa
+000011e0: 7461 4d67 6d74 2e73 796e 6363 0100 0000  taMgmt.syncc....
+000011f0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
+00001200: 4300 0000 7244 0000 0029 027a 5752 6574  C...rD...).zWRet
+00001210: 7572 6e20 7468 6520 7374 6174 7573 206f  urn the status o
+00001220: 6620 7468 6520 6375 7272 656e 7420 7265  f the current re
+00001230: 706f 7369 746f 7279 2e0a 2020 2020 2020  pository..      
+00001240: 2020 3a72 6574 7572 6e3a 2041 2043 6f6d    :return: A Com
+00001250: 6d61 6e64 5265 7375 6c74 2e0a 2020 2020  mandResult..    
+00001260: 2020 2020 4e72 1f00 0000 7245 0000 0072      Nr....rE...r
+00001270: 1f00 0000 721f 0000 0072 3700 0000 da06  ....r....r7.....
+00001280: 7374 6174 7573 a900 0000 f302 0000 0004  status..........
+00001290: 057a 1741 6273 7472 6163 7444 6174 614d  .z.AbstractDataM
+000012a0: 676d 742e 7374 6174 7573 6305 0000 0000  gmt.statusc.....
+000012b0: 0000 0000 0000 0005 0000 0001 0000 0043  ...............C
+000012c0: 0000 0072 4400 0000 2902 617d 0100 0043  ...rD...).a}...C
+000012d0: 6c6f 6e65 202f 2063 6f70 7920 6120 7265  lone / copy a re
+000012e0: 706f 7369 746f 7279 2072 656c 6174 6564  pository related
+000012f0: 2074 6f20 7468 6520 6769 7665 6e20 6461   to the given da
+00001300: 7461 2073 6574 2069 642e 0a20 2020 2020  ta set id..     
+00001310: 2020 203a 7061 7261 6d20 6461 7461 5f73     :param data_s
+00001320: 6574 5f69 643a 200a 2020 2020 2020 2020  et_id: .        
+00001330: 3a70 6172 616d 2073 7368 5f75 7365 723a  :param ssh_user:
+00001340: 2073 7368 2075 7365 7220 666f 7220 7265   ssh user for re
+00001350: 6d6f 7465 2073 7973 7465 6d20 286f 7074  mote system (opt
+00001360: 696f 6e61 6c29 0a20 2020 2020 2020 203a  ional).        :
+00001370: 7061 7261 6d20 636f 6e74 656e 745f 636f  param content_co
+00001380: 7079 5f69 6e64 6578 3a20 696e 6465 7820  py_index: index 
+00001390: 6f66 2063 6f6e 7465 6e74 2063 6f70 7920  of content copy 
+000013a0: 696e 2063 6173 6520 7468 6572 6520 6172  in case there ar
+000013b0: 6520 6d75 6c74 6970 6c65 2063 6f70 6965  e multiple copie
+000013c0: 7320 286f 7074 696f 6e61 6c29 0a20 2020  s (optional).   
+000013d0: 2020 2020 203a 7061 7261 6d20 736b 6970       :param skip
+000013e0: 5f69 6e74 6567 7269 7479 5f63 6865 636b  _integrity_check
+000013f0: 3a20 6966 2074 7275 652c 2074 6865 2066  : if true, the f
+00001400: 696c 6520 6368 6563 6b73 756d 7320 7769  ile checksums wi
+00001410: 6c6c 206e 6f74 2062 6520 6368 6563 6b65  ll not be checke
+00001420: 640a 2020 2020 2020 2020 3a72 6574 7572  d.        :retur
+00001430: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
+00001440: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
+00001450: 0000 a905 723c 0000 00da 0b64 6174 615f  ....r<.....data_
+00001460: 7365 745f 6964 da08 7373 685f 7573 6572  set_id..ssh_user
+00001470: da12 636f 6e74 656e 745f 636f 7079 5f69  ..content_copy_i
+00001480: 6e64 6578 da14 736b 6970 5f69 6e74 6567  ndex..skip_integ
+00001490: 7269 7479 5f63 6865 636b 721f 0000 0072  rity_checkr....r
+000014a0: 1f00 0000 7237 0000 00da 0563 6c6f 6e65  ....r7.....clone
+000014b0: b000 0000 f302 0000 0004 097a 1641 6273  ...........z.Abs
+000014c0: 7472 6163 7444 6174 614d 676d 742e 636c  tractDataMgmt.cl
+000014d0: 6f6e 6563 0500 0000 0000 0000 0000 0000  onec............
+000014e0: 0500 0000 0100 0000 4300 0000 7244 0000  ........C...rD..
+000014f0: 0029 0261 7501 0000 4d6f 7665 2061 2072  .).au...Move a r
+00001500: 6570 6f73 6974 6f72 7920 7265 6c61 7465  epository relate
+00001510: 6420 746f 2074 6865 2067 6976 656e 2064  d to the given d
+00001520: 6174 6120 7365 7420 6964 2e0a 2020 2020  ata set id..    
+00001530: 2020 2020 3a70 6172 616d 2064 6174 615f      :param data_
+00001540: 7365 745f 6964 3a20 0a20 2020 2020 2020  set_id: .       
+00001550: 203a 7061 7261 6d20 7373 685f 7573 6572   :param ssh_user
+00001560: 3a20 7373 6820 7573 6572 2066 6f72 2072  : ssh user for r
+00001570: 656d 6f74 6520 7379 7374 656d 2028 6f70  emote system (op
+00001580: 7469 6f6e 616c 290a 2020 2020 2020 2020  tional).        
+00001590: 3a70 6172 616d 2063 6f6e 7465 6e74 5f63  :param content_c
+000015a0: 6f70 795f 696e 6465 783a 2069 6e64 6578  opy_index: index
+000015b0: 206f 6620 636f 6e74 656e 7420 636f 7079   of content copy
+000015c0: 2069 6e20 6361 7365 2074 6865 7265 2061   in case there a
+000015d0: 7265 206d 756c 7469 706c 6520 636f 7069  re multiple copi
+000015e0: 6573 2028 6f70 7469 6f6e 616c 290a 2020  es (optional).  
+000015f0: 2020 2020 2020 3a70 6172 616d 2073 6b69        :param ski
+00001600: 705f 696e 7465 6772 6974 795f 6368 6563  p_integrity_chec
+00001610: 6b3a 2069 6620 7472 7565 2c20 7468 6520  k: if true, the 
+00001620: 6669 6c65 2063 6865 636b 7375 6d73 2077  file checksums w
+00001630: 696c 6c20 6e6f 7420 6265 2063 6865 636b  ill not be check
+00001640: 6564 0a20 2020 2020 2020 203a 7265 7475  ed.        :retu
+00001650: 726e 3a20 4120 436f 6d6d 616e 6452 6573  rn: A CommandRes
+00001660: 756c 742e 0a20 2020 2020 2020 204e 721f  ult..        Nr.
+00001670: 0000 0072 5a00 0000 721f 0000 0072 1f00  ...rZ...r....r..
+00001680: 0000 7237 0000 00da 046d 6f76 65bb 0000  ..r7.....move...
+00001690: 0072 6000 0000 7a15 4162 7374 7261 6374  .r`...z.Abstract
+000016a0: 4461 7461 4d67 6d74 2e6d 6f76 6563 0100  DataMgmt.movec..
+000016b0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+000016c0: 0000 4300 0000 7244 0000 0029 027a 6341  ..C...rD...).zcA
+000016d0: 6464 2074 6865 2063 7572 7265 6e74 2066  dd the current f
+000016e0: 6f6c 6465 7220 6173 2061 6e20 6f62 6973  older as an obis
+000016f0: 2072 6570 6f73 6974 6f72 7920 746f 206f   repository to o
+00001700: 7065 6e42 4953 2e0a 2020 2020 2020 2020  penBIS..        
+00001710: 3a72 6574 7572 6e3a 2041 2043 6f6d 6d61  :return: A Comma
+00001720: 6e64 5265 7375 6c74 2e0a 2020 2020 2020  ndResult..      
+00001730: 2020 4e72 1f00 0000 7245 0000 0072 1f00    Nr....rE...r..
+00001740: 0000 721f 0000 0072 3700 0000 da06 6164  ..r....r7.....ad
+00001750: 6472 6566 c600 0000 7259 0000 007a 1741  dref....rY...z.A
+00001760: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
+00001770: 6164 6472 6566 6302 0000 0000 0000 0000  addrefc.........
+00001780: 0000 0002 0000 0001 0000 0043 0000 0072  ...........C...r
+00001790: 4400 0000 2902 7ab4 5265 6d6f 7665 2074  D...).z.Remove t
+000017a0: 6865 2063 7572 7265 6e74 2066 6f6c 6465  he current folde
+000017b0: 7220 2f20 7265 706f 7369 746f 7279 2066  r / repository f
+000017c0: 726f 6d20 6f70 656e 4249 532e 0a20 2020  rom openBIS..   
+000017d0: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
+000017e0: 5f73 6574 5f69 643a 2049 6420 6f66 2074  _set_id: Id of t
+000017f0: 6865 2064 6174 6120 6672 6f6d 2077 6869  he data from whi
+00001800: 6368 2061 2072 6566 6572 656e 6365 2073  ch a reference s
+00001810: 686f 756c 6420 6265 2072 656d 6f76 6564  hould be removed
+00001820: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00001830: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
+00001840: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
+00001850: 0000 a902 723c 0000 0072 5b00 0000 721f  ....r<...r[...r.
+00001860: 0000 0072 1f00 0000 7237 0000 00da 0972  ...r....r7.....r
+00001870: 656d 6f76 6572 6566 cd00 0000 7302 0000  emoveref....s...
+00001880: 0004 067a 1a41 6273 7472 6163 7444 6174  ...z.AbstractDat
+00001890: 614d 676d 742e 7265 6d6f 7665 7265 6663  aMgmt.removerefc
+000018a0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+000018b0: 0100 0000 4300 0000 7244 0000 0029 0261  ....C...rD...).a
+000018c0: 9001 0000 446f 776e 6c6f 6164 2066 696c  ....Download fil
+000018d0: 6573 206f 6620 6120 7265 706f 7369 746f  es of a reposito
+000018e0: 7279 2077 6974 686f 7574 2061 6464 696e  ry without addin
+000018f0: 6720 6120 636f 6e74 656e 7420 636f 7079  g a content copy
+00001900: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00001910: 2064 6174 615f 7365 745f 6964 3a20 4964   data_set_id: Id
+00001920: 206f 6620 7468 6520 6461 7461 2073 6574   of the data set
+00001930: 2074 6f20 646f 776e 6c6f 6164 2066 726f   to download fro
+00001940: 6d2e 0a20 2020 2020 2020 203a 7061 7261  m..        :para
+00001950: 6d20 6672 6f6d 5f66 696c 653a 2050 6174  m from_file: Pat
+00001960: 6820 6f66 2061 2066 696c 6520 7769 7468  h of a file with
+00001970: 2061 206c 6973 7420 6f66 2064 6174 6173   a list of datas
+00001980: 6574 7320 746f 2064 6f77 6e6c 6f61 642e  ets to download.
+00001990: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000019a0: 6669 6c65 3a20 5061 7468 206f 6620 6120  file: Path of a 
+000019b0: 6669 6c65 2069 6e20 7468 6520 6461 7461  file in the data
+000019c0: 2073 6574 2074 6f20 646f 776e 6c6f 6164   set to download
+000019d0: 2e20 416c 6c20 6669 6c65 7320 6172 6520  . All files are 
+000019e0: 646f 776e 6c6f 6164 6564 2069 6620 6974  downloaded if it
+000019f0: 2069 7320 4e6f 6e65 2e0a 2020 2020 2020   is None..      
+00001a00: 2020 3a70 6172 616d 2073 6b69 705f 696e    :param skip_in
+00001a10: 7465 6772 6974 795f 6368 6563 6b3a 2043  tegrity_check: C
+00001a20: 6865 636b 7375 6d73 206f 6620 6669 6c65  hecksums of file
+00001a30: 7320 6172 6520 6e6f 7420 7665 7269 6669  s are not verifi
+00001a40: 6564 2069 6620 7472 7565 2e0a 2020 2020  ed if true..    
+00001a50: 2020 2020 4e72 1f00 0000 a905 723c 0000      Nr......r<..
+00001a60: 0072 5b00 0000 da09 6672 6f6d 5f66 696c  .r[.....from_fil
+00001a70: 65da 0466 696c 6572 5e00 0000 721f 0000  e..filer^...r...
+00001a80: 0072 1f00 0000 7237 0000 00da 0864 6f77  .r....r7.....dow
+00001a90: 6e6c 6f61 64d5 0000 0072 4e00 0000 7a19  nload....rN...z.
+00001aa0: 4162 7374 7261 6374 4461 7461 4d67 6d74  AbstractDataMgmt
+00001ab0: 2e64 6f77 6e6c 6f61 6463 0400 0000 0000  .downloadc......
+00001ac0: 0000 0000 0000 0400 0000 0100 0000 4300  ..............C.
+00001ad0: 0000 7244 0000 0029 027a ec55 706c 6f61  ..rD...).z.Uploa
+00001ae0: 6420 6669 6c65 732f 6469 7265 6374 6f72  d files/director
+00001af0: 6965 7320 696e 746f 2061 206e 6577 2064  ies into a new d
+00001b00: 6174 6120 7365 742e 0a20 2020 2020 2020  ata set..       
+00001b10: 203a 7061 7261 6d20 7361 6d70 6c65 5f69   :param sample_i
+00001b20: 643a 2070 6572 6d49 6420 6f72 2073 616d  d: permId or sam
+00001b30: 706c 6520 7061 7468 206f 6620 7468 6520  ple path of the 
+00001b40: 7061 7265 6e74 2073 616d 706c 650a 2020  parent sample.  
+00001b50: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+00001b60: 615f 7365 745f 7479 7065 3a20 7479 7065  a_set_type: type
+00001b70: 206f 6620 6372 6561 7465 6420 6461 7461   of created data
+00001b80: 2073 6574 0a20 2020 2020 2020 203a 7061   set.        :pa
+00001b90: 7261 6d20 6669 6c65 733a 206c 6973 7420  ram files: list 
+00001ba0: 6f66 2066 696c 6573 2f64 6972 6563 746f  of files/directo
+00001bb0: 7269 6573 2074 6f20 7570 6c6f 6164 0a20  ries to upload. 
+00001bc0: 2020 2020 2020 204e 721f 0000 0029 0472         Nr....).r
+00001bd0: 3c00 0000 da09 7361 6d70 6c65 5f69 64da  <.....sample_id.
+00001be0: 0d64 6174 615f 7365 745f 7479 7065 da05  .data_set_type..
+00001bf0: 6669 6c65 7372 1f00 0000 721f 0000 0072  filesr....r....r
+00001c00: 3700 0000 da06 7570 6c6f 6164 df00 0000  7.....upload....
+00001c10: 7252 0000 007a 1741 6273 7472 6163 7444  rR...z.AbstractD
+00001c20: 6174 614d 676d 742e 7570 6c6f 6164 6304  ataMgmt.uploadc.
+00001c30: 0000 0000 0000 0000 0000 0004 0000 0001  ................
+00001c40: 0000 0043 0000 0072 4400 0000 2902 612e  ...C...rD...).a.
+00001c50: 0100 0053 6561 7263 6820 666f 7220 6f62  ...Search for ob
+00001c60: 6a65 6374 7320 696e 206f 7065 6e42 4953  jects in openBIS
+00001c70: 2075 7369 6e67 2066 696c 7465 7269 6e67   using filtering
+00001c80: 2063 7269 7465 7269 612e 0a20 2020 2020   criteria..     
+00001c90: 2020 203a 7061 7261 6d20 6669 6c74 6572     :param filter
+00001ca0: 733a 2064 6963 7469 6f6e 6172 7920 6f66  s: dictionary of
+00001cb0: 2066 696c 7465 7220 7061 7261 6d65 7465   filter paramete
+00001cc0: 7273 0a20 2020 2020 2020 203a 7061 7261  rs.        :para
+00001cd0: 6d20 7265 6375 7273 6976 653a 2046 6c61  m recursive: Fla
+00001ce0: 6720 696e 6469 6361 7469 6e67 2069 6620  g indicating if 
+00001cf0: 7365 6172 6368 2073 686f 756c 6420 696e  search should in
+00001d00: 636c 7564 6520 6368 696c 6472 656e 2072  clude children r
+00001d10: 6563 7572 7369 7665 6c79 0a20 2020 2020  ecursively.     
+00001d20: 2020 203a 7061 7261 6d20 7361 7665 3a20     :param save: 
+00001d30: 4669 6c65 2070 6174 6820 746f 2073 6176  File path to sav
+00001d40: 6520 7265 7375 6c74 732e 2049 6620 6d69  e results. If mi
+00001d50: 7373 696e 672c 2073 6561 7263 6820 7265  ssing, search re
+00001d60: 7375 6c74 7320 7769 6c6c 206e 6f74 2062  sults will not b
+00001d70: 6520 7361 7665 642e 0a20 2020 2020 2020  e saved..       
+00001d80: 204e 721f 0000 00a9 0472 3c00 0000 da07   Nr......r<.....
+00001d90: 6669 6c74 6572 73da 0972 6563 7572 7369  filters..recursi
+00001da0: 7665 da04 7361 7665 721f 0000 0072 1f00  ve..saver....r..
+00001db0: 0000 7237 0000 00da 0d73 6561 7263 685f  ..r7.....search_
+00001dc0: 6f62 6a65 6374 e800 0000 7252 0000 007a  object....rR...z
+00001dd0: 1e41 6273 7472 6163 7444 6174 614d 676d  .AbstractDataMgm
+00001de0: 742e 7365 6172 6368 5f6f 626a 6563 7463  t.search_objectc
+00001df0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
+00001e00: 0100 0000 4300 0000 7244 0000 0029 0261  ....C...rD...).a
+00001e10: 2f01 0000 5365 6172 6368 2066 6f72 2064  /...Search for d
+00001e20: 6174 6173 6574 7320 696e 206f 7065 6e42  atasets in openB
+00001e30: 4953 2075 7369 6e67 2066 696c 7465 7269  IS using filteri
+00001e40: 6e67 2063 7269 7465 7269 612e 0a20 2020  ng criteria..   
+00001e50: 2020 2020 203a 7061 7261 6d20 6669 6c74       :param filt
+00001e60: 6572 733a 2064 6963 7469 6f6e 6172 7920  ers: dictionary 
+00001e70: 6f66 2066 696c 7465 7220 7061 7261 6d65  of filter parame
+00001e80: 7465 7273 0a20 2020 2020 2020 203a 7061  ters.        :pa
+00001e90: 7261 6d20 7265 6375 7273 6976 653a 2046  ram recursive: F
+00001ea0: 6c61 6720 696e 6469 6361 7469 6e67 2069  lag indicating i
+00001eb0: 6620 7365 6172 6368 2073 686f 756c 6420  f search should 
+00001ec0: 696e 636c 7564 6520 6368 696c 6472 656e  include children
+00001ed0: 2072 6563 7572 7369 7665 6c79 0a20 2020   recursively.   
+00001ee0: 2020 2020 203a 7061 7261 6d20 7361 7665       :param save
+00001ef0: 3a20 4669 6c65 2070 6174 6820 746f 2073  : File path to s
+00001f00: 6176 6520 7265 7375 6c74 732e 2049 6620  ave results. If 
+00001f10: 6d69 7373 696e 672c 2073 6561 7263 6820  missing, search 
+00001f20: 7265 7375 6c74 7320 7769 6c6c 206e 6f74  results will not
+00001f30: 2062 6520 7361 7665 642e 0a20 2020 2020   be saved..     
+00001f40: 2020 204e 721f 0000 0072 6d00 0000 721f     Nr....rm...r.
+00001f50: 0000 0072 1f00 0000 7237 0000 00da 0f73  ...r....r7.....s
+00001f60: 6561 7263 685f 6461 7461 5f73 6574 f100  earch_data_set..
+00001f70: 0000 7252 0000 007a 2041 6273 7472 6163  ..rR...z Abstrac
+00001f80: 7444 6174 614d 676d 742e 7365 6172 6368  tDataMgmt.search
+00001f90: 5f64 6174 615f 7365 7463 0800 0000 0000  _data_setc......
+00001fa0: 0000 0000 0000 0c00 0000 0c00 0000 4300  ..............C.
+00001fb0: 0000 733e 0100 007c 0372 097c 01a0 0064  ..s>...|.r.|...d
+00001fc0: 0167 01a1 0101 006e 067c 01a0 0064 0267  .g.....n.|...d.g
+00001fd0: 01a1 0101 007c 01a0 01a1 007d 087c 0472  .....|.....}.|.r
+00001fe0: 197c 0864 0319 007d 087c 0574 026a 0375  .|.d...}.|.t.j.u
+00001ff0: 0072 5b7c 0664 0075 0072 3574 046a 057c  .r[|.d.u.r5t.j.|
+00002000: 0864 0464 0564 068d 037d 0974 0664 07a0  .d.d.d...}.t.d..
+00002010: 077c 09a1 0164 0864 098d 0201 0064 0053  .|...d.d.....d.S
+00002020: 007c 067c 0876 0172 4274 0864 0aa0 077c  .|.|.v.rBt.d...|
+00002030: 067c 016a 09a1 0283 0182 017c 067c 087c  .|.j.......|.|.|
+00002040: 0619 0069 017d 0a74 046a 057c 0a64 0464  ...i.}.t.j.|.d.d
+00002050: 0564 068d 037d 0974 0664 07a0 077c 09a1  .d...}.t.d...|..
+00002060: 0164 0864 098d 0201 0064 0053 007c 0574  .d.d.....d.S.|.t
+00002070: 026a 0a75 0072 6d74 0b64 0b7c 00a0 0c7c  .j.u.rmt.d.|...|
+00002080: 027c 017c 067c 077c 037c 04a1 0683 0253  .|.|.|.|.|.....S
+00002090: 007c 0574 026a 0d75 0072 9d7c 0664 0075  .|.t.j.u.r.|.d.u
+000020a0: 0072 9064 0c7d 0b7c 08a0 0ea1 0044 005d  .r.d.}.|.....D.]
+000020b0: 117d 067c 0b74 0b64 0b7c 00a0 0c7c 027c  .}.|.t.d.|...|.|
+000020c0: 017c 0664 007c 037c 04a1 0683 0237 007d  .|.d.|.|.....7.}
+000020d0: 0b71 7c7c 0b53 0074 0b64 0b7c 00a0 0c7c  .q||.S.t.d.|...|
+000020e0: 027c 017c 0664 007c 037c 04a1 0683 0253  .|.|.d.|.|.....S
+000020f0: 0064 0053 0029 0d4e da06 676c 6f62 616c  .d.S.).N..global
+00002100: da05 6c6f 6361 6cda 0a70 726f 7065 7274  ..local..propert
+00002110: 6965 73e9 0400 0000 5429 02da 0669 6e64  ies.....T)...ind
+00002120: 656e 74da 0973 6f72 745f 6b65 7973 7a02  ent..sort_keysz.
+00002130: 7b7d 4629 01da 0e77 6974 685f 7469 6d65  {}F)...with_time
+00002140: 7374 616d 707a 1a55 6e6b 6e6f 776e 2073  stampz.Unknown s
+00002150: 6574 7469 6e67 207b 7d20 666f 7220 7b7d  etting {} for {}
+00002160: 2e72 0400 0000 7201 0000 0029 0fda 1973  .r....r....)...s
+00002170: 6574 5f6c 6f63 6174 696f 6e5f 7365 6172  et_location_sear
+00002180: 6368 5f6f 7264 6572 7226 0000 0072 1200  ch_orderr&...r..
+00002190: 0000 da03 4745 54da 046a 736f 6eda 0564  ....GET..json..d
+000021a0: 756d 7073 7218 0000 0072 3e00 0000 723f  umpsr....r>...r?
+000021b0: 0000 00da 0863 6174 6567 6f74 79da 0353  .....categoty..S
+000021c0: 4554 7219 0000 00da 0c73 6574 5f70 726f  ETr......set_pro
+000021d0: 7065 7274 79da 0543 4c45 4152 da04 6b65  perty..CLEAR..ke
+000021e0: 7973 290c 723c 0000 00da 0872 6573 6f6c  ys).r<.....resol
+000021f0: 7665 7272 3300 0000 da09 6973 5f67 6c6f  verr3.....is_glo
+00002200: 6261 6cda 1469 735f 6461 7461 5f73 6574  bal..is_data_set
+00002210: 5f70 726f 7065 7274 79da 0e6f 7065 7261  _property..opera
+00002220: 7469 6f6e 5f74 7970 65da 0470 726f 70da  tion_type..prop.
+00002230: 0576 616c 7565 7226 0000 00da 0a63 6f6e  .valuer&.....con
+00002240: 6669 675f 7374 72da 0b6c 6974 746c 655f  fig_str..little_
+00002250: 6469 6374 da0b 7265 7475 726e 5f63 6f64  dict..return_cod
+00002260: 6572 1f00 0000 721f 0000 0072 3700 0000  er....r....r7...
+00002270: da0d 7570 6461 7465 5f63 6f6e 6669 67fa  ..update_config.
+00002280: 0000 0073 4e00 0000 0403 0e01 0c02 0802  ...sN...........
+00002290: 0401 0801 0a02 0801 1001 1601 0802 0201  ................
+000022a0: 0c01 04ff 0c02 1001 1601 0a01 0401 0e01  ................
+000022b0: 0201 02ff 04ff 0a03 0801 0401 0c01 0601  ................
+000022c0: 0c01 0401 02ff 08ff 0403 0402 0e01 0201  ................
+000022d0: 02ff 04ff 04f7 7a1e 4162 7374 7261 6374  ......z.Abstract
+000022e0: 4461 7461 4d67 6d74 2e75 7064 6174 655f  DataMgmt.update_
+000022f0: 636f 6e66 6967 6306 0000 0000 0000 0000  configc.........
+00002300: 0000 0008 0000 000a 0000 0043 0000 0073  ...........C...s
+00002310: 8e00 0000 7c04 7204 6401 6e01 6402 7d06  ....|.r.d.n.d.}.
+00002320: 7a18 7c05 7214 7c01 6a00 6403 7c02 7c03  z.|.r.|.j.d.|.|.
+00002330: 7c06 6404 6405 8d05 0100 6e09 7c01 6a01  |.d.d.....n.|.j.
+00002340: 7c02 7c03 7c06 6404 6405 8d04 0100 5700  |.|.|.d.d.....W.
+00002350: 6e22 0400 7402 7940 0100 7d07 0100 7a16  n"..t.y@..}...z.
+00002360: 7c00 6404 7500 722c 7c07 8201 7403 6406  |.d.u.r,|...t.d.
+00002370: 6407 7404 7c07 8301 1700 6408 8d02 5700  d.t.|.....d...W.
+00002380: 0600 5900 6409 7d07 7e07 5300 6409 7d07  ..Y.d.}.~.S.d.}.
+00002390: 7e07 7701 7700 7403 640a 640b 6408 8d02  ~.w.w.t.d.d.d...
+000023a0: 5300 290c 7a3c 4865 6c70 6572 2066 756e  S.).z<Helper fun
+000023b0: 6374 696f 6e20 746f 2069 6d70 6c65 6d65  ction to impleme
+000023c0: 6e74 2074 6865 2070 726f 7065 7274 7920  nt the property 
+000023d0: 7365 7474 696e 6720 7365 6d61 6e74 6963  setting semantic
+000023e0: 732e 7273 0000 0072 7400 0000 7275 0000  s.rs...rt...ru..
+000023f0: 0054 a901 da0b 6170 706c 795f 7275 6c65  .T....apply_rule
+00002400: 73e9 ffff ffff fa07 4572 726f 723a 20a9  s.......Error: .
+00002410: 02da 0a72 6574 7572 6e63 6f64 65da 066f  ...returncode..o
+00002420: 7574 7075 744e 7201 0000 00da 0029 05da  utputNr......)..
+00002430: 1c73 6574 5f76 616c 7565 5f66 6f72 5f6a  .set_value_for_j
+00002440: 736f 6e5f 7061 7261 6d65 7465 72da 1773  son_parameter..s
+00002450: 6574 5f76 616c 7565 5f66 6f72 5f70 6172  et_value_for_par
+00002460: 616d 6574 6572 da09 4578 6365 7074 696f  ameter..Exceptio
+00002470: 6e72 0500 0000 da03 7374 7229 0872 3300  nr......str).r3.
+00002480: 0000 7283 0000 0072 8700 0000 7288 0000  ..r....r....r...
+00002490: 0072 8400 0000 7285 0000 00da 036c 6f63  .r....r......loc
+000024a0: da01 6572 1f00 0000 721f 0000 0072 3700  ..er....r....r7.
+000024b0: 0000 7280 0000 0022 0100 0073 1e00 0000  ..r...."...s....
+000024c0: 0c03 0201 0401 0c01 0201 08ff 1203 0480  ................
+000024d0: 0e01 0801 0401 2001 0880 02fd 0c05 7a1d  ...... .......z.
+000024e0: 4162 7374 7261 6374 4461 7461 4d67 6d74  AbstractDataMgmt
+000024f0: 2e73 6574 5f70 726f 7065 7274 7929 0246  .set_property).F
+00002500: 54a9 014e a902 5454 a902 4e4e 2901 4629  T..N..TT..NN).F)
+00002510: 1ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00002520: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00002530: 616d 655f 5fda 075f 5f64 6f63 5f5f 723d  ame__..__doc__r=
+00002540: 0000 0072 4300 0000 da03 6162 63da 0e61  ...rC.....abc..a
+00002550: 6273 7472 6163 746d 6574 686f 6472 4600  bstractmethodrF.
+00002560: 0000 724a 0000 0072 4d00 0000 7251 0000  ..rJ...rM...rQ..
+00002570: 0072 5700 0000 7256 0000 0072 5800 0000  .rW...rV...rX...
+00002580: 725f 0000 0072 6100 0000 7262 0000 0072  r_...ra...rb...r
+00002590: 6400 0000 7268 0000 0072 6c00 0000 7271  d...rh...rl...rq
+000025a0: 0000 0072 7200 0000 728c 0000 00da 0c73  ...rr...r......s
+000025b0: 7461 7469 636d 6574 686f 6472 8000 0000  taticmethodr....
+000025c0: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+000025d0: 3700 0000 7239 0000 005b 0000 0073 5000  7...r9...[...sP.
+000025e0: 0000 0800 0401 0206 0aff 0811 0405 0a01  ................
+000025f0: 0404 0a01 0404 0c01 0409 0c01 0408 0c01  ................
+00002600: 040b 0a01 0408 0a01 0406 0a01 040a 0a01  ................
+00002610: 040a 0a01 0406 0c01 0407 0a01 0409 0a01  ................
+00002620: 0408 0a01 0408 0a01 0209 0201 0afe 0228  ...............(
+00002630: 1001 7239 0000 0029 01da 096d 6574 6163  ..r9...)...metac
+00002640: 6c61 7373 6300 0000 0000 0000 0000 0000  lassc...........
+00002650: 0000 0000 0003 0000 0040 0000 0073 9000  .........@...s..
+00002660: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00002670: 6403 8400 5a04 6404 6405 8400 5a05 6422  d...Z.d.d...Z.d"
+00002680: 6407 6408 8401 5a06 6422 6409 640a 8401  d.d...Z.d"d.d...
+00002690: 5a07 6423 640c 640d 8401 5a08 640e 640f  Z.d#d.d...Z.d.d.
+000026a0: 8400 5a09 6410 6411 8400 5a0a 6412 6413  ..Z.d.d...Z.d.d.
+000026b0: 8400 5a0b 6414 6415 8400 5a0c 6416 6417  ..Z.d.d...Z.d.d.
+000026c0: 8400 5a0d 6422 6418 6419 8401 5a0e 641a  ..Z.d"d.d...Z.d.
+000026d0: 641b 8400 5a0f 641c 641d 8400 5a10 641e  d...Z.d.d...Z.d.
+000026e0: 641f 8400 5a11 6420 6421 8400 5a12 6406  d...Z.d d!..Z.d.
+000026f0: 5300 2924 722b 0000 007a 4544 6174 614d  S.)$r+...zEDataM
+00002700: 676d 7420 6f70 6572 6174 696f 6e73 2077  gmt operations w
+00002710: 6865 6e20 6769 7420 6973 206e 6f74 2061  hen git is not a
+00002720: 7661 696c 6162 6c65 202d 2d20 7368 6f77  vailable -- show
+00002730: 2065 7272 6f72 206d 6573 7361 6765 732e   error messages.
+00002740: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002750: 0004 0000 0043 0000 00f3 1000 0000 7c00  .....C........|.
+00002760: a000 6401 6402 a102 0100 6400 5300 2903  ..d.d.....d.S.).
+00002770: 4e7a 1567 6574 2073 6574 7469 6e67 7320  Nz.get settings 
+00002780: 7265 736f 6c76 6572 fa15 4e6f 2067 6974  resolver..No git
+00002790: 2063 6f6d 6d61 6e64 2066 6f75 6e64 2ea9   command found..
+000027a0: 0172 4300 0000 7245 0000 0072 1f00 0000  .rC...rE...r....
+000027b0: 721f 0000 0072 3700 0000 7246 0000 0037  r....r7...rF...7
+000027c0: 0100 00f3 0200 0000 1001 7a23 4e6f 4769  ..........z#NoGi
+000027d0: 7444 6174 614d 676d 742e 6765 745f 7365  tDataMgmt.get_se
+000027e0: 7474 696e 6773 5f72 6573 6f6c 7665 7263  ttings_resolverc
+000027f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002800: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
+00002810: fa14 7365 7475 7020 6c6f 6361 6c20 7365  ..setup local se
+00002820: 7474 696e 6773 72a7 0000 0072 a800 0000  ttingsr....r....
+00002830: 7248 0000 0072 1f00 0000 721f 0000 0072  rH...r....r....r
+00002840: 3700 0000 724a 0000 003a 0100 0072 a900  7...rJ...:...r..
+00002850: 0000 7a22 4e6f 4769 7444 6174 614d 676d  ..z"NoGitDataMgm
+00002860: 742e 7365 7475 705f 6c6f 6361 6c5f 7365  t.setup_local_se
+00002870: 7474 696e 6773 4e63 0200 0000 0000 0000  ttingsNc........
+00002880: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00002890: 72a6 0000 0029 034e 7a09 696e 6974 2064  r....).Nz.init d
+000028a0: 6174 6172 a700 0000 72a8 0000 0072 4b00  atar....r....rK.
+000028b0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
+000028c0: 0072 4d00 0000 3d01 0000 72a9 0000 007a  .rM...=...r....z
+000028d0: 174e 6f47 6974 4461 7461 4d67 6d74 2e69  .NoGitDataMgmt.i
+000028e0: 6e69 745f 6461 7461 6303 0000 0000 0000  nit_datac.......
+000028f0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00002900: 0072 a600 0000 2903 4efa 0d69 6e69 7420  .r....).N..init 
+00002910: 616e 616c 7973 6973 72a7 0000 0072 a800  analysisr....r..
+00002920: 0000 724f 0000 0072 1f00 0000 721f 0000  ..rO...r....r...
+00002930: 0072 3700 0000 7251 0000 0040 0100 0072  .r7...rQ...@...r
+00002940: a900 0000 7a1b 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
+00002950: 676d 742e 696e 6974 5f61 6e61 6c79 7369  gmt.init_analysi
+00002960: 7354 6304 0000 0000 0000 0000 0000 0004  sTc.............
+00002970: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
+00002980: 2903 4e72 5700 0000 72a7 0000 0072 a800  ).NrW...r....r..
+00002990: 0000 7253 0000 0072 1f00 0000 721f 0000  ..rS...r....r...
+000029a0: 0072 3700 0000 7257 0000 0043 0100 0072  .r7...rW...C...r
+000029b0: a900 0000 7a14 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
+000029c0: 676d 742e 636f 6d6d 6974 6301 0000 0000  gmt.commitc.....
+000029d0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+000029e0: 0000 0072 a600 0000 2903 4e72 5600 0000  ...r....).NrV...
+000029f0: 72a7 0000 0072 a800 0000 7245 0000 0072  r....r....rE...r
+00002a00: 1f00 0000 721f 0000 0072 3700 0000 7256  ....r....r7...rV
+00002a10: 0000 0046 0100 0072 a900 0000 7a12 4e6f  ...F...r....z.No
+00002a20: 4769 7444 6174 614d 676d 742e 7379 6e63  GitDataMgmt.sync
+00002a30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002a40: 0004 0000 0043 0000 0072 a600 0000 2903  .....C...r....).
+00002a50: 4e72 5800 0000 72a7 0000 0072 a800 0000  NrX...r....r....
+00002a60: 7245 0000 0072 1f00 0000 721f 0000 0072  rE...r....r....r
+00002a70: 3700 0000 7258 0000 0049 0100 0072 a900  7...rX...I...r..
+00002a80: 0000 7a14 4e6f 4769 7444 6174 614d 676d  ..z.NoGitDataMgm
+00002a90: 742e 7374 6174 7573 6305 0000 0000 0000  t.statusc.......
+00002aa0: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
+00002ab0: 0072 a600 0000 2903 4e72 5f00 0000 72a7  .r....).Nr_...r.
+00002ac0: 0000 0072 a800 0000 725a 0000 0072 1f00  ...r....rZ...r..
+00002ad0: 0000 721f 0000 0072 3700 0000 725f 0000  ..r....r7...r_..
+00002ae0: 004c 0100 0072 a900 0000 7a13 4e6f 4769  .L...r....z.NoGi
+00002af0: 7444 6174 614d 676d 742e 636c 6f6e 6563  tDataMgmt.clonec
+00002b00: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+00002b10: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
+00002b20: 7261 0000 0072 a700 0000 72a8 0000 0072  ra...r....r....r
+00002b30: 5a00 0000 721f 0000 0072 1f00 0000 7237  Z...r....r....r7
+00002b40: 0000 0072 6100 0000 4f01 0000 72a9 0000  ...ra...O...r...
+00002b50: 007a 124e 6f47 6974 4461 7461 4d67 6d74  .z.NoGitDataMgmt
+00002b60: 2e6d 6f76 6563 0100 0000 0000 0000 0000  .movec..........
+00002b70: 0000 0100 0000 0400 0000 4300 0000 72a6  ..........C...r.
+00002b80: 0000 0029 034e 7262 0000 0072 a700 0000  ...).Nrb...r....
+00002b90: 72a8 0000 0072 4500 0000 721f 0000 0072  r....rE...r....r
+00002ba0: 1f00 0000 7237 0000 0072 6200 0000 5201  ....r7...rb...R.
+00002bb0: 0000 72a9 0000 007a 144e 6f47 6974 4461  ..r....z.NoGitDa
+00002bc0: 7461 4d67 6d74 2e61 6464 7265 6663 0200  taMgmt.addrefc..
+00002bd0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00002be0: 0000 4300 0000 72a6 0000 0029 034e 7264  ..C...r....).Nrd
+00002bf0: 0000 0072 a700 0000 72a8 0000 0072 6300  ...r....r....rc.
+00002c00: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
+00002c10: 0072 6400 0000 5501 0000 72a9 0000 007a  .rd...U...r....z
+00002c20: 174e 6f47 6974 4461 7461 4d67 6d74 2e72  .NoGitDataMgmt.r
+00002c30: 656d 6f76 6572 6566 6301 0000 0000 0000  emoverefc.......
+00002c40: 0000 0000 0002 0000 0004 0000 0047 0000  .............G..
+00002c50: 0072 a600 0000 2903 4e72 6800 0000 72a7  .r....).Nrh...r.
+00002c60: 0000 0072 a800 0000 a902 723c 0000 00da  ...r......r<....
+00002c70: 015f 721f 0000 0072 1f00 0000 7237 0000  ._r....r....r7..
+00002c80: 0072 6800 0000 5801 0000 72a9 0000 007a  .rh...X...r....z
+00002c90: 164e 6f47 6974 4461 7461 4d67 6d74 2e64  .NoGitDataMgmt.d
+00002ca0: 6f77 6e6c 6f61 6463 0100 0000 0000 0000  ownloadc........
+00002cb0: 0000 0000 0200 0000 0400 0000 4700 0000  ............G...
+00002cc0: 72a6 0000 00a9 034e da06 7365 6172 6368  r......N..search
+00002cd0: 72a7 0000 0072 a800 0000 72ac 0000 0072  r....r....r....r
+00002ce0: 1f00 0000 721f 0000 0072 3700 0000 7271  ....r....r7...rq
+00002cf0: 0000 005b 0100 0072 a900 0000 7a1b 4e6f  ...[...r....z.No
+00002d00: 4769 7444 6174 614d 676d 742e 7365 6172  GitDataMgmt.sear
+00002d10: 6368 5f6f 626a 6563 7463 0100 0000 0000  ch_objectc......
+00002d20: 0000 0000 0000 0200 0000 0400 0000 4700  ..............G.
+00002d30: 0000 72a6 0000 0072 ae00 0000 72a8 0000  ..r....r....r...
+00002d40: 0072 ac00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00002d50: 7237 0000 0072 7200 0000 5e01 0000 72a9  r7...rr...^...r.
+00002d60: 0000 007a 1d4e 6f47 6974 4461 7461 4d67  ...z.NoGitDataMg
+00002d70: 6d74 2e73 6561 7263 685f 6461 7461 5f73  mt.search_data_s
+00002d80: 6574 6301 0000 0000 0000 0000 0000 0002  etc.............
+00002d90: 0000 0004 0000 0047 0000 0072 a600 0000  .......G...r....
+00002da0: 2903 4e72 6c00 0000 72a7 0000 0072 a800  ).Nrl...r....r..
+00002db0: 0000 72ac 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00002dc0: 0072 3700 0000 726c 0000 0061 0100 0072  .r7...rl...a...r
+00002dd0: a900 0000 7a14 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
+00002de0: 676d 742e 7570 6c6f 6164 729b 0000 0072  gmt.uploadr....r
+00002df0: 9c00 0000 2913 729e 0000 0072 9f00 0000  ....).r....r....
+00002e00: 72a0 0000 0072 a100 0000 7246 0000 0072  r....r....rF...r
+00002e10: 4a00 0000 724d 0000 0072 5100 0000 7257  J...rM...rQ...rW
+00002e20: 0000 0072 5600 0000 7258 0000 0072 5f00  ...rV...rX...r_.
+00002e30: 0000 7261 0000 0072 6200 0000 7264 0000  ..ra...rb...rd..
+00002e40: 0072 6800 0000 7271 0000 0072 7200 0000  .rh...rq...rr...
+00002e50: 726c 0000 0072 1f00 0000 721f 0000 0072  rl...r....r....r
+00002e60: 1f00 0000 7237 0000 0072 2b00 0000 3401  ....r7...r+...4.
+00002e70: 0000 7322 0000 0008 0004 0108 0208 030a  ..s"............
+00002e80: 030a 030a 0308 0308 0308 0308 0308 030a  ................
+00002e90: 0308 0308 0308 030c 0372 2b00 0000 6301  .........r+...c.
+00002ea0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00002eb0: 0000 0043 0000 0073 1600 0000 7c00 a000  ...C...s....|...
+00002ec0: a100 0100 7401 a002 6401 a101 0100 6400  ....t...d.....d.
+00002ed0: 5300 2902 4e72 0100 0000 2903 da07 7265  S.).Nr....)...re
+00002ee0: 7374 6f72 65da 0373 7973 da04 6578 6974  store..sys..exit
+00002ef0: 2901 da09 6461 7461 5f6d 676d 7472 1f00  )...data_mgmtr..
+00002f00: 0000 721f 0000 0072 3700 0000 da16 7265  ..r....r7.....re
+00002f10: 7374 6f72 655f 7369 676e 616c 5f68 616e  store_signal_han
+00002f20: 646c 6572 6501 0000 7304 0000 0008 010e  dlere...s.......
+00002f30: 0172 b400 0000 6301 0000 0000 0000 0000  .r....c.........
+00002f40: 0000 0002 0000 0003 0000 0003 0000 00f3  ................
+00002f50: 1000 0000 8700 6601 6401 6402 8408 7d01  ......f.d.d...}.
+00002f60: 7c01 5300 2903 7a33 2054 6f20 6265 2075  |.S.).z3 To be u
+00002f70: 7365 6420 7769 7468 2063 6f6d 6d61 6e64  sed with command
+00002f80: 7320 7468 6174 2075 7365 2074 6865 2043  s that use the C
+00002f90: 6f6d 6d61 6e64 4c6f 672e 2063 0100 0000  ommandLog. c....
+00002fa0: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
+00002fb0: 1700 0000 736e 0000 007a 0a88 007c 0067  ....sn...z...|.g
+00002fc0: 017c 01a2 0152 008e 007d 0257 006e 1604  .|...R...}.W.n..
+00002fd0: 0074 0079 2001 007d 0301 007a 0a7c 006a  .t.y ..}...z.|.j
+00002fe0: 01a0 0274 037c 0383 01a1 0101 007c 0382  ...t.|.......|..
+00002ff0: 0164 007d 037e 0377 0177 007c 02a0 04a1  .d.}.~.w.w.|....
+00003000: 0064 016b 0272 2e7c 006a 01a0 05a1 0001  .d.k.r.|.j......
+00003010: 007c 0253 007c 006a 01a0 027c 026a 06a1  .|.S.|.j...|.j..
+00003020: 0101 007c 0253 0029 024e 4629 0772 9700  ...|.S.).NF).r..
+00003030: 0000 7232 0000 00da 096c 6f67 5f65 7272  ..r2.....log_err
+00003040: 6f72 7298 0000 00da 0766 6169 6c75 7265  orr......failure
+00003050: da07 7375 6363 6573 7372 9300 0000 a904  ..successr......
+00003060: 723c 0000 00da 0461 7267 73da 0672 6573  r<.....args..res
+00003070: 756c 7472 9a00 0000 a901 da01 6672 1f00  ultr........fr..
+00003080: 0000 7237 0000 00da 0a66 5f77 6974 685f  ..r7.....f_with_
+00003090: 6c6f 676d 0100 0073 1800 0000 0201 1401  logm...s........
+000030a0: 0e01 1001 0401 0880 02fe 0c03 0a01 0403  ................
+000030b0: 0eff 0401 7a1c 7769 7468 5f6c 6f67 2e3c  ....z.with_log.<
+000030c0: 6c6f 6361 6c73 3e2e 665f 7769 7468 5f6c  locals>.f_with_l
+000030d0: 6f67 721f 0000 0029 0272 bd00 0000 72be  ogr....).r....r.
+000030e0: 0000 0072 1f00 0000 72bc 0000 0072 3700  ...r....r....r7.
+000030f0: 0000 da08 7769 7468 5f6c 6f67 6a01 0000  ....with_logj...
+00003100: 7304 0000 000c 0304 0c72 bf00 0000 6301  s........r....c.
+00003110: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00003120: 0000 0003 0000 0072 b500 0000 2903 7a2f  .......r....).z/
+00003130: 2053 6574 7320 7468 6520 7265 7374 6f72   Sets the restor
+00003140: 6520 706f 696e 7420 616e 6420 7265 7374  e point and rest
+00003150: 6f72 6573 206f 6e20 6572 726f 722e 2063  ores on error. c
+00003160: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00003170: 0a00 0000 1700 0000 73aa 0000 0088 00a0  ........s.......
+00003180: 00a1 0001 007a 2588 006a 0172 1374 02a0  .....z%..j.r.t..
+00003190: 0274 026a 0387 0066 0164 0164 0284 08a1  .t.j...f.d.d....
+000031a0: 0201 0088 0188 0067 017c 01a2 0152 008e  .......g.|...R..
+000031b0: 007d 027c 02a0 04a1 0072 2388 00a0 05a1  .}.|.....r#.....
+000031c0: 0001 0088 00a0 06a1 0001 007c 0257 0053  ...........|.W.S
+000031d0: 0004 0074 0779 5401 007d 0301 007a 1f88  ...t.yT..}...z..
+000031e0: 00a0 05a1 0001 0088 006a 0864 036b 0272  .........j.d.k.r
+000031f0: 3c7c 0382 0188 00a0 06a1 0001 0074 0964  <|...........t.d
+00003200: 0464 0574 0a7c 0383 0117 0064 068d 0257  .d.t.|.....d...W
+00003210: 0006 0059 0064 007d 037e 0353 0064 007d  ...Y.d.}.~.S.d.}
+00003220: 037e 0377 0177 0029 074e 6302 0000 0000  .~.w.w.).Nc.....
+00003230: 0000 0000 0000 0002 0000 0002 0000 0013  ................
+00003240: 0000 0073 0800 0000 7400 8800 8301 5300  ...s....t.....S.
+00003250: 729b 0000 0029 0172 b400 0000 2902 da06  r....).r....)...
+00003260: 7369 676e 616c da05 6672 616d 6572 4500  signal..framerE.
+00003270: 0000 721f 0000 0072 3700 0000 da08 3c6c  ..r....r7.....<l
+00003280: 616d 6264 613e 8301 0000 7302 0000 0008  ambda>....s.....
+00003290: 007a 3677 6974 685f 7265 7374 6f72 652e  .z6with_restore.
+000032a0: 3c6c 6f63 616c 733e 2e66 5f77 6974 685f  <locals>.f_with_
+000032b0: 7265 7374 6f72 652e 3c6c 6f63 616c 733e  restore.<locals>
+000032c0: 2e3c 6c61 6d62 6461 3e54 728f 0000 0072  .<lambda>Tr....r
+000032d0: 9000 0000 7291 0000 0029 0bda 1073 6574  ....r....)...set
+000032e0: 5f72 6573 746f 7265 706f 696e 7472 3a00  _restorepointr:.
+000032f0: 0000 72c0 0000 00da 0653 4947 494e 5472  ..r......SIGINTr
+00003300: b700 0000 72b0 0000 00da 1263 6c65 6172  ....r......clear
+00003310: 5f72 6573 746f 7265 706f 696e 7472 9700  _restorepointr..
+00003320: 0000 7233 0000 0072 0500 0000 7298 0000  ..r3...r....r...
+00003330: 0072 b900 0000 72bc 0000 0072 4500 0000  .r....r....rE...
+00003340: 7237 0000 00da 0e66 5f77 6974 685f 7265  r7.....f_with_re
+00003350: 7374 6f72 657f 0100 0073 2200 0000 0801  store....s".....
+00003360: 0201 0601 1601 1001 0801 0801 0801 0601  ................
+00003370: 0e01 0801 0a01 0401 0801 2001 0880 02fb  .......... .....
+00003380: 7a24 7769 7468 5f72 6573 746f 7265 2e3c  z$with_restore.<
+00003390: 6c6f 6361 6c73 3e2e 665f 7769 7468 5f72  locals>.f_with_r
+000033a0: 6573 746f 7265 721f 0000 0029 0272 bd00  estorer....).r..
+000033b0: 0000 72c6 0000 0072 1f00 0000 72bc 0000  ..r....r....r...
+000033c0: 0072 3700 0000 da0c 7769 7468 5f72 6573  .r7.....with_res
+000033d0: 746f 7265 7c01 0000 7304 0000 000c 0304  tore|...s.......
+000033e0: 1172 c700 0000 6300 0000 0000 0000 0000  .r....c.........
+000033f0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
+00003400: dc00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+00003410: 6430 6403 6404 8401 5a04 6405 6406 8400  d0d.d...Z.d.d...
+00003420: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
+00003430: 5a07 6430 640b 640c 8401 5a08 6430 640d  Z.d0d.d...Z.d0d.
+00003440: 640e 8401 5a09 650a 640f 6410 8400 8301  d...Z.e.d.d.....
+00003450: 5a0b 6411 6412 8400 5a0c 650a 6431 6414  Z.d.d...Z.e.d1d.
+00003460: 6415 8401 8301 5a0d 6416 6417 8400 5a0e  d.....Z.d.d...Z.
+00003470: 6418 6419 8400 5a0f 641a 641b 8400 5a10  d.d...Z.d.d...Z.
+00003480: 641c 641d 8400 5a11 641e 641f 8400 5a12  d.d...Z.d.d...Z.
+00003490: 6513 6420 6421 8400 8301 5a14 6422 6423  e.d d!....Z.d"d#
+000034a0: 8400 5a15 6430 6424 6425 8401 5a16 6426  ..Z.d0d$d%..Z.d&
+000034b0: 6427 8400 5a17 0902 0902 6432 6428 6429  d'..Z.....d2d(d)
+000034c0: 8401 5a18 642a 642b 8400 5a19 642c 642d  ..Z.d*d+..Z.d,d-
+000034d0: 8400 5a1a 642e 642f 8400 5a1b 6402 5300  ..Z.d.d/..Z.d.S.
+000034e0: 2933 722c 0000 007a 2444 6174 614d 676d  )3r,...z$DataMgm
+000034f0: 7420 6f70 6572 6174 696f 6e73 2069 6e20  t operations in 
+00003500: 6e6f 726d 616c 2073 7461 7465 2e4e 6302  normal state.Nc.
+00003510: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00003520: 0000 0043 0000 0073 2600 0000 7c01 6400  ...C...s&...|.d.
+00003530: 7500 7207 7c00 6a00 5300 7401 a002 a100  u.r.|.j.S.t.....
+00003540: 7d02 7c02 a003 6401 7c01 a102 0100 7c02  }.|...d.|.....|.
+00003550: 5300 2902 4eda 0864 6174 615f 7365 7429  S.).N..data_set)
+00003560: 0472 2e00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00003570: da1b 7365 745f 7265 736f 6c76 6572 5f6c  ..set_resolver_l
+00003580: 6f63 6174 696f 6e5f 726f 6f74 73a9 0372  ocation_roots..r
+00003590: 3c00 0000 da0d 7265 6c61 7469 7665 5f70  <.....relative_p
+000035a0: 6174 6872 2e00 0000 721f 0000 0072 1f00  athr....r....r..
+000035b0: 0000 7237 0000 0072 4600 0000 9601 0000  ..r7...rF.......
+000035c0: 730a 0000 0008 0106 0108 020c 0104 017a  s..............z
+000035d0: 2147 6974 4461 7461 4d67 6d74 2e67 6574  !GitDataMgmt.get
+000035e0: 5f73 6574 7469 6e67 735f 7265 736f 6c76  _settings_resolv
+000035f0: 6572 6302 0000 0000 0000 0000 0000 0007  erc.............
+00003600: 0000 0007 0000 0043 0000 0073 5000 0000  .......C...sP...
+00003610: 7c00 6a00 a001 6401 6402 a102 0100 7c01  |.j...d.d.....|.
+00003620: a002 a100 4400 5d1a 5c02 7d02 7d03 7403  ....D.].\.}.}.t.
+00003630: 7c00 6a00 7c02 8302 7d04 7c03 a002 a100  |.j.|...}.|.....
+00003640: 4400 5d0b 5c02 7d05 7d06 7c04 a004 7c05  D.].\.}.}.|...|.
+00003650: 7c06 6403 a103 0100 7119 710b 6400 5300  |.d.....q.q.d.S.
+00003660: 2904 4e72 c800 0000 da01 2e72 7400 0000  ).Nr.......rt...
+00003670: 2905 722e 0000 0072 c900 0000 da05 6974  ).r....r......it
+00003680: 656d 73da 0767 6574 6174 7472 7296 0000  ems..getattrr...
+00003690: 0029 0772 3c00 0000 7249 0000 00da 0d72  .).r<...rI.....r
+000036a0: 6573 6f6c 7665 725f 7479 7065 da08 7365  esolver_type..se
+000036b0: 7474 696e 6773 7283 0000 00da 036b 6579  ttingsr......key
+000036c0: 7288 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+000036d0: 3700 0000 724a 0000 009f 0100 0073 0e00  7...rJ.......s..
+000036e0: 0000 0e01 1001 0c01 1001 1001 02ff 04fe  ................
+000036f0: 7a20 4769 7444 6174 614d 676d 742e 7365  z GitDataMgmt.se
+00003700: 7475 705f 6c6f 6361 6c5f 7365 7474 696e  tup_local_settin
+00003710: 6773 6302 0000 0000 0000 0000 0000 0003  gsc.............
+00003720: 0000 0003 0000 0043 0000 00f3 1a00 0000  .......C........
+00003730: 7c00 a000 7c01 a101 7d02 7c02 6a01 a002  |...|...}.|.j...
+00003740: a100 a003 6401 a101 5300 2902 4e72 5b00  ....d...S.).Nr[.
+00003750: 0000 a904 7246 0000 00da 0a72 6570 6f73  ....rF.....repos
+00003760: 6974 6f72 7972 2600 0000 da03 6765 7472  itoryr&.....getr
+00003770: ca00 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
+00003780: 0000 00da 0f67 6574 5f64 6174 615f 7365  .....get_data_se
+00003790: 745f 6964 a601 0000 f304 0000 000a 0110  t_id............
+000037a0: 017a 1b47 6974 4461 7461 4d67 6d74 2e67  .z.GitDataMgmt.g
+000037b0: 6574 5f64 6174 615f 7365 745f 6964 6302  et_data_set_idc.
+000037c0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+000037d0: 0000 0043 0000 0072 d200 0000 2902 4eda  ...C...r....).N.
+000037e0: 0269 6472 d300 0000 72ca 0000 0072 1f00  .idr....r....r..
+000037f0: 0000 721f 0000 0072 3700 0000 da11 6765  ..r....r7.....ge
+00003800: 745f 7265 706f 7369 746f 7279 5f69 64aa  t_repository_id.
+00003810: 0100 0072 d700 0000 7a1d 4769 7444 6174  ...r....z.GitDat
+00003820: 614d 676d 742e 6765 745f 7265 706f 7369  aMgmt.get_reposi
+00003830: 746f 7279 5f69 6463 0200 0000 0000 0000  tory_idc........
+00003840: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00003850: 7394 0000 0074 006a 01a0 0264 01a1 0172  s....t.j...d...r
+00003860: 0c74 0364 0264 0364 048d 0253 007c 006a  .t.d.d.d...S.|.j
+00003870: 04a0 05a1 007d 027c 02a0 06a1 0072 177c  .....}.|.....r.|
+00003880: 0253 007c 006a 076a 08a0 09a1 00a0 0a64  .S.|.j.j.......d
+00003890: 05a1 017d 037c 006a 04a0 0b7c 017c 03a1  ...}.|.j...|.|..
+000038a0: 027d 027c 02a0 06a1 0072 2d7c 0253 007c  .}.|.....r-|.S.|
+000038b0: 006a 04a0 0ca1 007d 027c 02a0 06a1 0072  .j.....}.|.....r
+000038c0: 387c 0253 007c 006a 07a0 0d64 0664 07a1  8|.S.|.j...d.d..
+000038d0: 0201 007c 006a 07a0 0ea1 0001 0074 0364  ...|.j.......t.d
+000038e0: 0864 0964 048d 0253 0029 0a4e 721d 0000  .d.d...S.).Nr...
+000038f0: 0072 8f00 0000 fa25 466f 6c64 6572 2069  .r.....%Folder i
+00003900: 7320 616c 7265 6164 7920 616e 206f 6269  s already an obi
+00003910: 7320 7265 706f 7369 746f 7279 2e72 9100  s repository.r..
+00003920: 0000 da11 6769 745f 616e 6e65 785f 6261  ....git_annex_ba
+00003930: 636b 656e 6472 c800 0000 72cc 0000 0072  ckendr....r....r
+00003940: 0100 0000 7294 0000 0029 0f72 2300 0000  ....r....).r#...
+00003950: 7224 0000 0072 2500 0000 7205 0000 0072  r$...r%...r....r
+00003960: 3600 0000 da08 6769 745f 696e 6974 72b7  6.....git_initr.
+00003970: 0000 0072 2e00 0000 7204 0000 0072 2600  ...r....r....r&.
+00003980: 0000 72d5 0000 00da 0e67 6974 5f61 6e6e  ..r......git_ann
+00003990: 6578 5f69 6e69 74da 0e69 6e69 7469 616c  ex_init..initial
+000039a0: 5f63 6f6d 6d69 7472 c900 0000 da14 636f  _commitr......co
+000039b0: 7079 5f67 6c6f 6261 6c5f 746f 5f6c 6f63  py_global_to_loc
+000039c0: 616c 2904 723c 0000 0072 4c00 0000 72bb  al).r<...rL...r.
+000039d0: 0000 0072 db00 0000 721f 0000 0072 1f00  ...r....r....r..
+000039e0: 0000 7237 0000 0072 4d00 0000 ae01 0000  ..r7...rM.......
+000039f0: 731e 0000 000c 020c 010a 0108 0104 0112  s...............
+00003a00: 010e 0108 0104 010a 0108 0104 010e 020a  ................
+00003a10: 010c 017a 1547 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
+00003a20: 2e69 6e69 745f 6461 7461 6303 0000 0000  .init_datac.....
+00003a30: 0000 0000 0000 0009 0000 000a 0000 0043  ...............C
+00003a40: 0000 0073 1601 0000 7c00 a000 7c01 a101  ...s....|...|...
+00003a50: 7d03 7c00 a001 7c01 a101 6400 7500 7212  }.|...|...d.u.r.
+00003a60: 7402 6401 6402 6403 8d02 5300 7c00 a003  t.d.d.d...S.|...
+00003a70: 7c02 a101 7d04 7c04 a004 a100 721d 7c04  |...}.|.....r.|.
+00003a80: 5300 7405 6a06 a007 7405 a008 a100 7c01  S.t.j...t.....|.
+00003a90: a102 7d05 7405 a008 a100 7d06 7409 7c06  ..}.t.....}.t.|.
+00003aa0: 8301 7409 7c05 8301 6a0a 7600 7254 7405  ..t.|...j.v.rTt.
+00003ab0: 6a06 a00b 7c06 7c05 a102 7d07 740c 7c01  j...|.|...}.t.|.
+00003ac0: 8301 8f0e 0100 7c00 6a0d a00e 7c07 a101  ......|.j...|...
+00003ad0: 0100 5700 6400 0400 0400 8303 0100 6e08  ..W.d.........n.
+00003ae0: 3100 734f 7701 0100 0100 0100 5900 0100  1.sOw.......Y...
+00003af0: 7a0d 7c00 6a0f 6a10 6a11 6404 7c03 6405  z.|.j.j.j.d.|.d.
+00003b00: 6406 6407 8d04 0100 5700 6e23 0400 7412  d.d.....W.n#..t.
+00003b10: 7984 0100 7d08 0100 7a17 7c00 6a13 6406  y...}...z.|.j.d.
+00003b20: 7500 7270 7c08 8201 7402 6401 6408 7414  u.rp|...t.d.d.t.
+00003b30: 7c08 8301 1700 6403 8d02 5700 0600 5900  |.....d...W...Y.
+00003b40: 6400 7d08 7e08 5300 6400 7d08 7e08 7701  d.}.~.S.d.}.~.w.
+00003b50: 7700 7402 6409 640a 6403 8d02 5300 290b  w.t.d.d.d...S.).
+00003b60: 4e72 8f00 0000 7a52 5061 7265 6e74 2064  Nr....zRParent d
+00003b70: 6174 6120 7365 7420 6d75 7374 2062 6520  ata set must be 
+00003b80: 636f 6d6d 6974 7465 6420 746f 206f 7065  committed to ope
+00003b90: 6e42 4953 2062 6566 6f72 6520 6372 6561  nBIS before crea
+00003ba0: 7469 6e67 2061 6e20 616e 616c 7973 6973  ting an analysis
+00003bb0: 2064 6174 6120 7365 742e 7291 0000 0072   data set.r....r
+00003bc0: 5b00 0000 7274 0000 0054 728d 0000 0072  [...rt...Tr....r
+00003bd0: 9000 0000 7201 0000 0072 9400 0000 2915  ....r....r....).
+00003be0: 72d6 0000 0072 d900 0000 7205 0000 0072  r....r....r....r
+00003bf0: 4d00 0000 72b7 0000 0072 2300 0000 7224  M...r....r#...r$
+00003c00: 0000 00da 046a 6f69 6eda 0667 6574 6377  .....join..getcw
+00003c10: 6472 0200 0000 da07 7061 7265 6e74 73da  dr......parents.
+00003c20: 0772 656c 7061 7468 7213 0000 0072 3600  .relpathr....r6.
+00003c30: 0000 da0a 6769 745f 6967 6e6f 7265 722e  ....git_ignorer.
+00003c40: 0000 0072 d400 0000 7296 0000 0072 9700  ...r....r....r..
+00003c50: 0000 7233 0000 0072 9800 0000 2909 723c  ..r3...r....).r<
+00003c60: 0000 0072 5000 0000 724c 0000 00da 1270  ...rP...rL.....p
+00003c70: 6172 656e 745f 6461 7461 5f73 6574 5f69  arent_data_set_i
+00003c80: 6472 bb00 0000 da11 7061 7265 6e74 5f66  dr......parent_f
+00003c90: 6f6c 6465 725f 6162 73da 1361 6e61 6c79  older_abs..analy
+00003ca0: 7369 735f 666f 6c64 6572 5f61 6273 da18  sis_folder_abs..
+00003cb0: 616e 616c 7973 6973 5f66 6f6c 6465 725f  analysis_folder_
+00003cc0: 7265 6c61 7469 7665 729a 0000 0072 1f00  relativer....r..
+00003cd0: 0000 721f 0000 0072 3700 0000 7251 0000  ..r....r7...rQ..
+00003ce0: 00c1 0100 0073 3600 0000 0a02 0e02 0401  .....s6.........
+00003cf0: 0201 06ff 0a03 0801 0401 1203 0801 1201  ................
+00003d00: 0e01 0a01 0e01 1cff 0204 0a01 0401 0201  ................
+00003d10: 0afe 0e03 0a01 0401 2001 0880 02fd 0c05  ........ .......
+00003d20: 7a19 4769 7444 6174 614d 676d 742e 696e  z.GitDataMgmt.in
+00003d30: 6974 5f61 6e61 6c79 7369 7363 0100 0000  it_analysisc....
+00003d40: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+00003d50: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
+00003d60: 0072 9b00 0000 2901 da05 5f73 796e 6372  .r....)..._syncr
+00003d70: 4500 0000 721f 0000 0072 1f00 0000 7237  E...r....r....r7
+00003d80: 0000 0072 5600 0000 e101 0000 7302 0000  ...rV.......s...
+00003d90: 0008 027a 1047 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
+00003da0: 2e73 796e 6363 0100 0000 0000 0000 0000  .syncc..........
+00003db0: 0000 0200 0000 0300 0000 4300 0000 7314  ..........C...s.
+00003dc0: 0000 0074 007c 007c 006a 0183 027d 017c  ...t.|.|.j...}.|
+00003dd0: 01a0 02a1 0053 0072 9b00 0000 2903 720c  .....S.r....).r.
+00003de0: 0000 0072 3b00 0000 da03 7275 6ea9 0272  ...r;.....run..r
+00003df0: 3c00 0000 da03 636d 6472 1f00 0000 721f  <.....cmdr....r.
+00003e00: 0000 0072 3700 0000 72e9 0000 00e5 0100  ...r7...r.......
+00003e10: 00f3 0400 0000 0c01 0801 7a11 4769 7444  ..........z.GitD
+00003e20: 6174 614d 676d 742e 5f73 796e 6354 6304  ataMgmt._syncTc.
+00003e30: 0000 0000 0000 0000 0000 0005 0000 0003  ................
+00003e40: 0000 0043 0000 0073 5c00 0000 7c02 721a  ...C...s\...|.r.
+00003e50: 7c00 6a00 a001 a100 7d04 7c04 a002 a100  |.j.....}.|.....
+00003e60: 720d 7c04 5300 7c00 6a00 a003 7c04 6a04  r.|.S.|.j...|.j.
+00003e70: a101 7d04 7c04 a002 a100 721a 7c04 5300  ..}.|.....r.|.S.
+00003e80: 7c00 6a00 a005 7c01 a101 7d04 7c04 a002  |.j...|...}.|...
+00003e90: a100 7226 7c04 5300 7c03 722c 7c00 a006  ..r&|.S.|.r,|...
+00003ea0: a100 7d04 7c04 5300 2901 7a28 2047 6974  ..}.|.S.).z( Git
+00003eb0: 2061 6464 2c20 636f 6d6d 6974 2061 6e64   add, commit and
+00003ec0: 2073 796e 6320 7769 7468 206f 7065 6e42   sync with openB
+00003ed0: 4953 2e20 2907 7236 0000 00da 1267 6974  IS. ).r6.....git
+00003ee0: 5f74 6f70 5f6c 6576 656c 5f70 6174 6872  _top_level_pathr
+00003ef0: b700 0000 da07 6769 745f 6164 6472 9300  ......git_addr..
+00003f00: 0000 da0a 6769 745f 636f 6d6d 6974 72e9  ....git_commitr.
+00003f10: 0000 0029 0572 3c00 0000 7254 0000 0072  ...).r<...rT...r
+00003f20: 5500 0000 7256 0000 0072 bb00 0000 721f  U...rV...r....r.
+00003f30: 0000 0072 1f00 0000 7237 0000 0072 5700  ...r....r7...rW.
+00003f40: 0000 e901 0000 731a 0000 0004 030a 0108  ......s.........
+00003f50: 0104 010e 0108 0104 010c 0108 0104 0204  ................
+00003f60: 0108 0104 017a 1247 6974 4461 7461 4d67  .....z.GitDataMg
+00003f70: 6d74 2e63 6f6d 6d69 7463 0100 0000 0000  mt.commitc......
+00003f80: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
+00003f90: 0000 737a 0000 007c 006a 00a0 01a1 007d  ..sz...|.j.....}
+00003fa0: 017a 0a74 027c 0083 016a 0364 0164 028d  .z.t.|...j.d.d..
+00003fb0: 017d 0257 006e 1104 0074 046a 056a 0679  .}.W.n...t.j.j.y
+00003fc0: 2001 0001 0001 0074 0764 0364 0464 058d   ......t.d.d.d..
+00003fd0: 027d 0259 006e 0177 007c 016a 087d 037c  .}.Y.n.w.|.j.}.|
+00003fe0: 02a0 09a1 0072 3774 0a7c 0383 0164 066b  .....r7t.|...d.k
+00003ff0: 0472 327c 0364 0737 007d 037c 037c 026a  .r2|.d.7.}.|.|.j
+00004000: 0837 007d 0374 0764 067c 0364 058d 0253  .7.}.t.d.|.d...S
+00004010: 0029 084e 5429 01da 0969 6e66 6f5f 6f6e  .).NT)...info_on
+00004020: 6c79 728f 0000 007a 1d43 6f75 6c64 206e  lyr....z.Could n
+00004030: 6f74 2063 6f6e 6e65 6374 2074 6f20 6f70  ot connect to op
+00004040: 656e 4249 532e 7291 0000 0072 0100 0000  enBIS.r....r....
+00004050: da01 0a29 0b72 3600 0000 da0a 6769 745f  ...).r6.....git_
+00004060: 7374 6174 7573 720c 0000 0072 ea00 0000  statusr....r....
+00004070: da08 7265 7175 6573 7473 da0a 6578 6365  ..requests..exce
+00004080: 7074 696f 6e73 da0f 436f 6e6e 6563 7469  ptions..Connecti
+00004090: 6f6e 4572 726f 7272 0500 0000 7293 0000  onErrorr....r...
+000040a0: 0072 b700 0000 da03 6c65 6e29 0472 3c00  .r......len).r<.
+000040b0: 0000 72f3 0000 00da 0b73 796e 635f 7374  ..r......sync_st
+000040c0: 6174 7573 7293 0000 0072 1f00 0000 721f  atusr....r....r.
+000040d0: 0000 0072 3700 0000 7258 0000 00fb 0100  ...r7...rX......
+000040e0: 0073 1800 0000 0a01 0201 1401 1001 1001  .s..............
+000040f0: 02ff 0602 0801 0c01 0801 0a01 0c01 7a12  ..............z.
+00004100: 4769 7444 6174 614d 676d 742e 7374 6174  GitDataMgmt.stat
+00004110: 7573 6301 0000 0000 0000 0000 0000 0001  usc.............
+00004120: 0000 0004 0000 0043 0000 0073 2600 0000  .......C...s&...
+00004130: 7c00 6a00 a001 a100 6a02 7c00 5f03 7c00  |.j.....j.|._.|.
+00004140: a004 a100 0100 7405 a006 6401 6402 a102  ......t...d.d...
+00004150: 0100 6403 5300 2904 7a3a 2053 746f 7265  ..d.S.).z: Store
+00004160: 7320 7468 6520 6769 7420 636f 6d6d 6974  s the git commit
+00004170: 2068 6173 6820 616e 6420 636f 7069 6573   hash and copies
+00004180: 2074 6865 206f 6269 7320 6d65 7461 6461   the obis metada
+00004190: 7461 2e20 721d 0000 00fa 122e 6f62 6973  ta. r.......obis
+000041a0: 5f72 6573 746f 7265 706f 696e 744e 2907  _restorepointN).
+000041b0: 7236 0000 00da 0f67 6974 5f63 6f6d 6d69  r6.....git_commi
+000041c0: 745f 6861 7368 7293 0000 00da 1870 7265  t_hashr......pre
+000041d0: 7669 6f75 735f 6769 745f 636f 6d6d 6974  vious_git_commit
+000041e0: 5f68 6173 6872 c500 0000 da06 7368 7574  _hashr......shut
+000041f0: 696c da08 636f 7079 7472 6565 7245 0000  il..copytreerE..
+00004200: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+00004210: 72c3 0000 0008 0200 0073 0600 0000 0e02  r........s......
+00004220: 0801 1001 7a1c 4769 7444 6174 614d 676d  ....z.GitDataMgm
+00004230: 742e 7365 745f 7265 7374 6f72 6570 6f69  t.set_restorepoi
+00004240: 6e74 6301 0000 0000 0000 0000 0000 0001  ntc.............
+00004250: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
+00004260: 7c00 6a00 a001 7c00 6a02 a101 0100 7403  |.j...|.j.....t.
+00004270: a004 6401 a101 0100 7403 a005 6402 6401  ..d.....t...d.d.
+00004280: a102 0100 6403 5300 2904 7a4d 2052 6573  ....d.S.).zM Res
+00004290: 6574 7320 746f 2074 6865 2073 746f 7265  ets to the store
+000042a0: 6420 6769 7420 636f 6d6d 6974 2068 6173  d git commit has
+000042b0: 6820 616e 6420 7265 7374 6f72 6573 2074  h and restores t
+000042c0: 6865 2063 6f70 6965 6420 6f62 6973 206d  he copied obis m
+000042d0: 6574 6164 6174 612e 2072 1d00 0000 72f9  etadata. r....r.
+000042e0: 0000 004e 2906 7236 0000 00da 0c67 6974  ...N).r6.....git
+000042f0: 5f72 6573 6574 5f74 6f72 fb00 0000 72fc  _reset_tor....r.
+00004300: 0000 00da 0672 6d74 7265 6572 fd00 0000  .....rmtreer....
+00004310: 7245 0000 0072 1f00 0000 721f 0000 0072  rE...r....r....r
+00004320: 3700 0000 72b0 0000 000e 0200 0073 0600  7...r........s..
+00004330: 0000 0e02 0a01 1001 7a13 4769 7444 6174  ........z.GitDat
+00004340: 614d 676d 742e 7265 7374 6f72 6563 0100  aMgmt.restorec..
+00004350: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00004360: 0000 4300 0000 731e 0000 0074 006a 01a0  ..C...s....t.j..
+00004370: 0264 01a1 0172 0d74 03a0 0464 01a1 0101  .d...r.t...d....
+00004380: 0064 0253 0064 0253 0029 037a 3b20 4465  .d.S.d.S.).z; De
+00004390: 6c65 7465 7320 7468 6520 6f62 6973 206d  letes the obis m
+000043a0: 6574 6164 6174 6120 636f 7079 2e20 5468  etadata copy. Th
+000043b0: 6973 206d 7573 7420 616c 7761 7973 2062  is must always b
+000043c0: 6520 646f 6e65 2e20 72f9 0000 004e 2905  e done. r....N).
+000043d0: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+000043e0: fc00 0000 72ff 0000 0072 4500 0000 721f  ....r....rE...r.
+000043f0: 0000 0072 1f00 0000 7237 0000 0072 c500  ...r....r7...r..
+00004400: 0000 1402 0000 7306 0000 000c 020e 0104  ......s.........
+00004410: ff7a 1e47 6974 4461 7461 4d67 6d74 2e63  .z.GitDataMgmt.c
+00004420: 6c65 6172 5f72 6573 746f 7265 706f 696e  lear_restorepoin
+00004430: 7463 0500 0000 0000 0000 0000 0000 0600  tc..............
+00004440: 0000 0600 0000 4300 0000 f318 0000 0074  ......C........t
+00004450: 007c 007c 017c 027c 037c 0483 057d 057c  .|.|.|.|.|...}.|
+00004460: 05a0 01a1 0053 0072 9b00 0000 2902 7207  .....S.r....).r.
+00004470: 0000 0072 ea00 0000 a906 723c 0000 0072  ...r......r<...r
+00004480: 5b00 0000 725c 0000 0072 5d00 0000 725e  [...r\...r]...r^
+00004490: 0000 0072 ec00 0000 721f 0000 0072 1f00  ...r....r....r..
+000044a0: 0000 7237 0000 0072 5f00 0000 1902 0000  ..r7...r_.......
+000044b0: f304 0000 0010 0108 017a 1147 6974 4461  .........z.GitDa
+000044c0: 7461 4d67 6d74 2e63 6c6f 6e65 6305 0000  taMgmt.clonec...
+000044d0: 0000 0000 0000 0000 0006 0000 0006 0000  ................
+000044e0: 0043 0000 0072 0001 0000 729b 0000 0029  .C...r....r....)
+000044f0: 0272 0a00 0000 72ea 0000 0072 0101 0000  .r....r....r....
+00004500: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
+00004510: 6100 0000 1d02 0000 7304 0000 0010 0208  a.......s.......
+00004520: 017a 1047 6974 4461 7461 4d67 6d74 2e6d  .z.GitDataMgmt.m
+00004530: 6f76 6563 0100 0000 0000 0000 0000 0000  ovec............
+00004540: 0200 0000 0200 0000 4300 0000 7310 0000  ........C...s...
+00004550: 0074 007c 0083 017d 017c 01a0 01a1 0053  .t.|...}.|.....S
+00004560: 0072 9b00 0000 2902 7206 0000 0072 ea00  .r....).r....r..
+00004570: 0000 72eb 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00004580: 0072 3700 0000 7262 0000 0022 0200 0073  .r7...rb..."...s
+00004590: 0400 0000 0801 0801 7a12 4769 7444 6174  ........z.GitDat
+000045a0: 614d 676d 742e 6164 6472 6566 6302 0000  aMgmt.addrefc...
+000045b0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+000045c0: 0043 0000 0073 1400 0000 7400 7c00 7c01  .C...s....t.|.|.
+000045d0: 6401 8d02 7d02 7c02 a001 a100 5300 2902  d...}.|.....S.).
+000045e0: 4e29 0172 5b00 0000 2902 720d 0000 0072  N).r[...).r....r
+000045f0: ea00 0000 2903 723c 0000 0072 5b00 0000  ....).r<...r[...
+00004600: 72ec 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00004610: 3700 0000 7264 0000 0026 0200 0072 ed00  7...rd...&...r..
+00004620: 0000 7a15 4769 7444 6174 614d 676d 742e  ..z.GitDataMgmt.
+00004630: 7265 6d6f 7665 7265 6663 0500 0000 0000  removerefc......
+00004640: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
+00004650: 0000 72a6 0000 0029 034e 7268 0000 00fa  ..r....).Nrh....
+00004660: 3054 6869 7320 636f 6d6d 616e 6420 6973  0This command is
+00004670: 206f 6e6c 7920 6176 6169 6c61 626c 6520   only available 
+00004680: 666f 7220 4d61 6e61 6765 7220 4461 7461  for Manager Data
+00004690: 2e72 a800 0000 7265 0000 0072 1f00 0000  .r....re...r....
+000046a0: 721f 0000 0072 3700 0000 7268 0000 002a  r....r7...rh...*
+000046b0: 0200 0072 a900 0000 7a14 4769 7444 6174  ...r....z.GitDat
+000046c0: 614d 676d 742e 646f 776e 6c6f 6164 6307  aMgmt.downloadc.
+000046d0: 0000 0000 0000 0000 0000 0008 0000 0009  ................
+000046e0: 0000 0043 0000 0073 8a00 0000 7c00 6a00  ...C...s....|.j.
+000046f0: a001 7c01 a101 7d07 7c07 6401 7500 7210  ..|...}.|.d.u.r.
+00004700: 7402 6402 7c01 1700 8301 8201 7c04 7403  t.d.|.......|.t.
+00004710: 6a04 7500 7222 7c05 6401 7501 731b 4a00  j.u.r"|.d.u.s.J.
+00004720: 8201 7c06 6401 7501 7321 4a00 8201 6e17  ..|.d.u.s!J...n.
+00004730: 7c04 7403 6a05 7500 722e 7c06 6401 7500  |.t.j.u.r.|.d.u.
+00004740: 732d 4a00 8201 6e0b 7c04 7403 6a06 7500  s-J...n.|.t.j.u.
+00004750: 7239 7c06 6401 7500 7339 4a00 8201 7c00  r9|.d.u.s9J...|.
+00004760: a007 7c07 7c00 6a08 7c02 7c03 7c04 7c05  ..|.|.j.|.|.|.|.
+00004770: 7c06 a107 5300 2903 e185 0100 000a 2020  |...S.).......  
+00004780: 2020 2020 2020 3a70 6172 616d 2063 6174        :param cat
+00004790: 6567 6f72 793a 2063 6f6e 6669 672c 206f  egory: config, o
+000047a0: 626a 6563 742c 2063 6f6c 6c65 6374 696f  bject, collectio
+000047b0: 6e2c 2064 6174 615f 7365 7420 6f72 2072  n, data_set or r
+000047c0: 6570 6f73 6974 6f72 790a 2020 2020 2020  epository.      
+000047d0: 2020 3a70 6172 616d 2069 735f 676c 6f62    :param is_glob
+000047e0: 616c 3a20 6163 7420 6f6e 2067 6c6f 6261  al: act on globa
+000047f0: 6c20 7365 7474 696e 6773 202d 206c 6f63  l settings - loc
+00004800: 616c 2069 6620 6661 6c73 650a 2020 2020  al if false.    
+00004810: 2020 2020 3a70 6172 616d 2069 735f 6461      :param is_da
+00004820: 7461 5f73 6574 5f70 726f 7065 7274 793a  ta_set_property:
+00004830: 2074 7275 6520 6966 2070 726f 7020 2f20   true if prop / 
+00004840: 7661 6c75 6520 6172 6520 6120 6461 7461  value are a data
+00004850: 2073 6574 2070 726f 7065 7274 790a 2020   set property.  
+00004860: 2020 2020 2020 3a70 6172 616d 206f 7065        :param ope
+00004870: 7261 7469 6f6e 5f74 7970 653a 2074 7970  ration_type: typ
+00004880: 6520 6f66 206f 7065 7261 7469 6f6e 2074  e of operation t
+00004890: 6f20 7065 7266 6f72 6d2e 2049 7420 6361  o perform. It ca
+000048a0: 6e20 6265 2047 4554 2c20 5345 542c 2043  n be GET, SET, C
+000048b0: 4c45 4152 0a20 2020 2020 2020 203a 7061  LEAR.        :pa
+000048c0: 7261 6d20 7072 6f70 3a20 7365 7474 696e  ram prop: settin
+000048d0: 6720 6b65 790a 2020 2020 2020 2020 3a70  g key.        :p
+000048e0: 6172 616d 2076 616c 7565 3a20 7365 7474  aram value: sett
+000048f0: 696e 6720 7661 6c75 650a 2020 2020 2020  ing value.      
+00004900: 2020 4efa 1b49 6e76 616c 6964 2073 6574    N..Invalid set
+00004910: 7469 6e67 7320 6361 7465 676f 7279 3a20  tings category: 
+00004920: 2909 722e 0000 0072 d500 0000 723f 0000  ).r....r....r?..
+00004930: 0072 1200 0000 727f 0000 0072 7b00 0000  .r....r....r{...
+00004940: 7281 0000 0072 8c00 0000 7233 0000 0029  r....r....r3...)
+00004950: 0872 3c00 0000 da08 6361 7465 676f 7279  .r<.....category
+00004960: 7284 0000 0072 8500 0000 7286 0000 0072  r....r....r....r
+00004970: 8700 0000 7288 0000 0072 8300 0000 721f  ....r....r....r.
+00004980: 0000 0072 1f00 0000 7237 0000 0072 0400  ...r....r7...r..
+00004990: 0000 3102 0000 731a 0000 000c 0a08 010c  ..1...s.........
+000049a0: 010a 010c 010e 010a 010e 010a 010c 010e  ................
+000049b0: 0206 0104 ff7a 1247 6974 4461 7461 4d67  .....z.GitDataMg
+000049c0: 6d74 2e63 6f6e 6669 6763 0100 0000 0000  mt.configc......
+000049d0: 0000 0000 0000 0200 0000 0400 0000 4700  ..............G.
+000049e0: 0000 72a6 0000 00a9 034e 72af 0000 0072  ..r......Nr....r
+000049f0: 0301 0000 72a8 0000 0072 ac00 0000 721f  ....r....r....r.
+00004a00: 0000 0072 1f00 0000 7237 0000 0072 7100  ...r....r7...rq.
+00004a10: 0000 4902 0000 72a9 0000 007a 1947 6974  ..I...r....z.Git
+00004a20: 4461 7461 4d67 6d74 2e73 6561 7263 685f  DataMgmt.search_
+00004a30: 6f62 6a65 6374 6301 0000 0000 0000 0000  objectc.........
+00004a40: 0000 0002 0000 0004 0000 0047 0000 0072  ...........G...r
+00004a50: a600 0000 7207 0100 0072 a800 0000 72ac  ....r....r....r.
+00004a60: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
+00004a70: 0000 7272 0000 004c 0200 0072 a900 0000  ..rr...L...r....
+00004a80: 7a1b 4769 7444 6174 614d 676d 742e 7365  z.GitDataMgmt.se
+00004a90: 6172 6368 5f64 6174 615f 7365 7463 0100  arch_data_setc..
+00004aa0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00004ab0: 0000 4700 0000 72a6 0000 0029 034e 726c  ..G...r....).Nrl
+00004ac0: 0000 0072 0301 0000 72a8 0000 0072 ac00  ...r....r....r..
+00004ad0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
+00004ae0: 0072 6c00 0000 4f02 0000 72a9 0000 007a  .rl...O...r....z
+00004af0: 1247 6974 4461 7461 4d67 6d74 2e75 706c  .GitDataMgmt.upl
+00004b00: 6f61 6472 9b00 0000 729c 0000 0072 9d00  oadr....r....r..
+00004b10: 0000 291c 729e 0000 0072 9f00 0000 72a0  ..).r....r....r.
+00004b20: 0000 0072 a100 0000 7246 0000 0072 4a00  ...r....rF...rJ.
+00004b30: 0000 72d6 0000 0072 d900 0000 724d 0000  ..r....r....rM..
+00004b40: 0072 5100 0000 72c7 0000 0072 5600 0000  .rQ...r....rV...
+00004b50: 72e9 0000 0072 5700 0000 7258 0000 0072  r....rW...rX...r
+00004b60: c300 0000 72b0 0000 0072 c500 0000 725f  ....r....r....r_
+00004b70: 0000 0072 bf00 0000 7261 0000 0072 6200  ...r....ra...rb.
+00004b80: 0000 7264 0000 0072 6800 0000 7204 0000  ..rd...rh...r...
+00004b90: 0072 7100 0000 7272 0000 0072 6c00 0000  .rq...rr...rl...
+00004ba0: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00004bb0: 3700 0000 722c 0000 0093 0100 0073 3a00  7...r,.......s:.
+00004bc0: 0000 0800 0401 0a02 0809 0807 0804 0a04  ................
+00004bd0: 0a13 0220 0a01 0803 0204 0c01 0811 080d  ... ............
+00004be0: 0806 0806 0805 0204 0a01 0804 0a04 0804  ................
+00004bf0: 0207 0201 0aff 0818 0803 0c03 722c 0000  ............r,..
+00004c00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00004c10: 0000 0300 0000 4000 0000 739e 0000 0065  ......@...s....e
+00004c20: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
+00004c30: 005a 0464 0464 0584 005a 0564 2464 0764  .Z.d.d...Z.d$d.d
+00004c40: 0884 015a 0664 2464 0964 0a84 015a 0764  ...Z.d$d.d...Z.d
+00004c50: 2564 0c64 0d84 015a 0864 0e64 0f84 005a  %d.d...Z.d.d...Z
+00004c60: 0964 1064 1184 005a 0a64 1264 1384 005a  .d.d...Z.d.d...Z
+00004c70: 0b64 1464 1584 005a 0c64 1664 1784 005a  .d.d...Z.d.d...Z
+00004c80: 0d64 2464 1864 1984 015a 0e64 1a64 1b84  .d$d.d...Z.d.d..
+00004c90: 005a 0f64 1c64 1d84 005a 1064 1e64 1f84  .Z.d.d...Z.d.d..
+00004ca0: 005a 1164 2064 2184 005a 1209 0609 0664  .Z.d d!..Z.....d
+00004cb0: 2664 2264 2384 015a 1364 0653 0029 2772  &d"d#..Z.d.S.)'r
+00004cc0: 2900 0000 7a28 4461 7461 4d67 6d74 206f  )...z(DataMgmt o
+00004cd0: 7065 7261 7469 6f6e 7320 666f 7220 4453  perations for DS
+00004ce0: 532d 7374 6f72 6564 2064 6174 612e 6301  S-stored data.c.
+00004cf0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00004d00: 0000 0043 0000 0073 0800 0000 7400 a001  ...C...s....t...
+00004d10: a100 5300 729b 0000 0029 0272 2000 0000  ..S.r....).r ...
+00004d20: 7221 0000 0072 4500 0000 721f 0000 0072  r!...rE...r....r
+00004d30: 1f00 0000 7237 0000 0072 4600 0000 5602  ....r7...rF...V.
+00004d40: 0000 7302 0000 0008 017a 2650 6879 7369  ..s......z&Physi
+00004d50: 6361 6c44 6174 614d 676d 742e 6765 745f  calDataMgmt.get_
+00004d60: 7365 7474 696e 6773 5f72 6573 6f6c 7665  settings_resolve
+00004d70: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
+00004d80: 0000 0400 0000 4300 0000 72a6 0000 0029  ......C...r....)
+00004d90: 034e 72aa 0000 00fa 3854 6869 7320 636f  .Nr.....8This co
+00004da0: 6d6d 616e 6420 6973 206f 6e6c 7920 6176  mmand is only av
+00004db0: 6169 6c61 626c 6520 666f 7220 4578 7465  ailable for Exte
+00004dc0: 726e 616c 204d 616e 6167 6572 2044 6174  rnal Manager Dat
+00004dd0: 6172 a800 0000 7248 0000 0072 1f00 0000  ar....rH...r....
+00004de0: 721f 0000 0072 3700 0000 724a 0000 0059  r....r7...rJ...Y
+00004df0: 0200 00f3 0600 0000 0601 0201 08ff 7a25  ..............z%
+00004e00: 5068 7973 6963 616c 4461 7461 4d67 6d74  PhysicalDataMgmt
+00004e10: 2e73 6574 7570 5f6c 6f63 616c 5f73 6574  .setup_local_set
+00004e20: 7469 6e67 734e 6302 0000 0000 0000 0000  tingsNc.........
+00004e30: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+00004e40: 6400 0000 7400 6a01 a002 6401 a101 720c  d...t.j...d...r.
+00004e50: 7403 6402 6403 6404 8d02 5300 7c00 6a04  t.d.d.d...S.|.j.
+00004e60: 6a05 a006 a100 0100 7c00 6a04 6a05 a007  j.......|.j.j...
+00004e70: 6405 6406 6407 a103 0100 7c00 6a04 6a05  d.d.d.....|.j.j.
+00004e80: a008 a100 6408 1900 7d02 7c00 6a04 6a05  ....d...}.|.j.j.
+00004e90: a007 6409 7c02 6407 a103 0100 7403 640a  ..d.|.d.....t.d.
+00004ea0: 640b 6404 8d02 5300 290c 4e72 1d00 0000  d.d...S.).Nr....
+00004eb0: 728f 0000 0072 da00 0000 7291 0000 0072  r....r....r....r
+00004ec0: 1e00 0000 5472 7400 0000 da0b 6f70 656e  ....Trt.....open
+00004ed0: 6269 735f 7572 6cda 0f66 696c 6573 6572  bis_url..fileser
+00004ee0: 7669 6365 5f75 726c 7201 0000 007a 294d  vice_urlr....z)M
+00004ef0: 616e 6167 6564 2064 6174 6120 6f62 6973  anaged data obis
+00004f00: 2072 6570 6f73 6974 6f72 7920 696e 6974   repository init
+00004f10: 6961 6c69 7a65 642e 2909 7223 0000 0072  ialized.).r#...r
+00004f20: 2400 0000 7225 0000 0072 0500 0000 722e  $...r%...r....r.
+00004f30: 0000 0072 0400 0000 72df 0000 0072 9600  ...r....r....r..
+00004f40: 0000 7226 0000 0029 0372 3c00 0000 724c  ..r&...).r<...rL
+00004f50: 0000 0072 0a01 0000 721f 0000 0072 1f00  ...r....r....r..
+00004f60: 0000 7237 0000 0072 4d00 0000 5d02 0000  ..r7...rM...]...
+00004f70: 7312 0000 000c 010c 010c 0112 0110 010a  s...............
+00004f80: 0104 0104 ff0c 027a 1a50 6879 7369 6361  .......z.Physica
+00004f90: 6c44 6174 614d 676d 742e 696e 6974 5f64  lDataMgmt.init_d
+00004fa0: 6174 6163 0300 0000 0000 0000 0000 0000  atac............
+00004fb0: 0300 0000 0400 0000 4300 0000 72a6 0000  ........C...r...
+00004fc0: 0029 034e 72ab 0000 0072 0801 0000 72a8  .).Nr....r....r.
+00004fd0: 0000 0072 4f00 0000 721f 0000 0072 1f00  ...rO...r....r..
+00004fe0: 0000 7237 0000 0072 5100 0000 6702 0000  ..r7...rQ...g...
+00004ff0: 7209 0100 007a 1e50 6879 7369 6361 6c44  r....z.PhysicalD
+00005000: 6174 614d 676d 742e 696e 6974 5f61 6e61  ataMgmt.init_ana
+00005010: 6c79 7369 7354 6304 0000 0000 0000 0000  lysisTc.........
+00005020: 0000 0004 0000 0004 0000 0043 0000 0072  ...........C...r
+00005030: a600 0000 2903 4e72 5700 0000 7208 0100  ....).NrW...r...
+00005040: 0072 a800 0000 7253 0000 0072 1f00 0000  .r....rS...r....
+00005050: 721f 0000 0072 3700 0000 7257 0000 006b  r....r7...rW...k
+00005060: 0200 0072 a900 0000 7a17 5068 7973 6963  ...r....z.Physic
+00005070: 616c 4461 7461 4d67 6d74 2e63 6f6d 6d69  alDataMgmt.commi
+00005080: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00005090: 0000 0400 0000 4300 0000 72a6 0000 0029  ......C...r....)
+000050a0: 034e 7256 0000 0072 0801 0000 72a8 0000  .NrV...r....r...
+000050b0: 0072 4500 0000 721f 0000 0072 1f00 0000  .rE...r....r....
+000050c0: 7237 0000 0072 5600 0000 6e02 0000 72a9  r7...rV...n...r.
+000050d0: 0000 007a 1550 6879 7369 6361 6c44 6174  ...z.PhysicalDat
+000050e0: 614d 676d 742e 7379 6e63 6301 0000 0000  aMgmt.syncc.....
+000050f0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+00005100: 0000 0072 a600 0000 2903 4e72 5800 0000  ...r....).NrX...
+00005110: 7208 0100 0072 a800 0000 7245 0000 0072  r....r....rE...r
+00005120: 1f00 0000 721f 0000 0072 3700 0000 7258  ....r....r7...rX
+00005130: 0000 0071 0200 0072 a900 0000 7a17 5068  ...q...r....z.Ph
+00005140: 7973 6963 616c 4461 7461 4d67 6d74 2e73  ysicalDataMgmt.s
+00005150: 7461 7475 7363 0500 0000 0000 0000 0000  tatusc..........
+00005160: 0000 0500 0000 0400 0000 4300 0000 72a6  ..........C...r.
+00005170: 0000 0029 034e 725f 0000 0072 0801 0000  ...).Nr_...r....
+00005180: 72a8 0000 0072 5a00 0000 721f 0000 0072  r....rZ...r....r
+00005190: 1f00 0000 7237 0000 0072 5f00 0000 7402  ....r7...r_...t.
+000051a0: 0000 72a9 0000 007a 1650 6879 7369 6361  ..r....z.Physica
+000051b0: 6c44 6174 614d 676d 742e 636c 6f6e 6563  lDataMgmt.clonec
+000051c0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
+000051d0: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
+000051e0: 7261 0000 0072 0801 0000 72a8 0000 0072  ra...r....r....r
+000051f0: 5a00 0000 721f 0000 0072 1f00 0000 7237  Z...r....r....r7
+00005200: 0000 0072 6100 0000 7702 0000 72a9 0000  ...ra...w...r...
+00005210: 007a 1550 6879 7369 6361 6c44 6174 614d  .z.PhysicalDataM
+00005220: 676d 742e 6d6f 7665 6301 0000 0000 0000  gmt.movec.......
+00005230: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00005240: 0072 a600 0000 2903 4e72 6200 0000 7208  .r....).Nrb...r.
+00005250: 0100 0072 a800 0000 7245 0000 0072 1f00  ...r....rE...r..
+00005260: 0000 721f 0000 0072 3700 0000 7262 0000  ..r....r7...rb..
+00005270: 007a 0200 0072 a900 0000 7a17 5068 7973  .z...r....z.Phys
+00005280: 6963 616c 4461 7461 4d67 6d74 2e61 6464  icalDataMgmt.add
+00005290: 7265 6663 0200 0000 0000 0000 0000 0000  refc............
+000052a0: 0200 0000 0400 0000 4300 0000 72a6 0000  ........C...r...
+000052b0: 0029 034e 7264 0000 0072 0801 0000 72a8  .).Nrd...r....r.
+000052c0: 0000 0072 6300 0000 721f 0000 0072 1f00  ...rc...r....r..
+000052d0: 0000 7237 0000 0072 6400 0000 7d02 0000  ..r7...rd...}...
+000052e0: 72a9 0000 007a 1a50 6879 7369 6361 6c44  r....z.PhysicalD
+000052f0: 6174 614d 676d 742e 7265 6d6f 7665 7265  ataMgmt.removere
+00005300: 6663 0500 0000 0000 0000 0000 0000 0600  fc..............
+00005310: 0000 0600 0000 4300 0000 7200 0100 0072  ......C...r....r
+00005320: 9b00 0000 2902 7209 0000 0072 ea00 0000  ....).r....r....
+00005330: 2906 723c 0000 0072 5b00 0000 7266 0000  ).r<...r[...rf..
+00005340: 0072 6700 0000 725e 0000 0072 ec00 0000  .rg...r^...r....
+00005350: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
+00005360: 6800 0000 8002 0000 7202 0100 007a 1950  h.......r....z.P
+00005370: 6879 7369 6361 6c44 6174 614d 676d 742e  hysicalDataMgmt.
+00005380: 646f 776e 6c6f 6164 6304 0000 0000 0000  downloadc.......
+00005390: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
+000053a0: 00f3 1600 0000 7400 7c00 7c01 7c02 7c03  ......t.|.|.|.|.
+000053b0: 8304 7d04 7c04 a001 a100 5300 729b 0000  ..}.|.....S.r...
+000053c0: 0029 0272 0f00 0000 72ea 0000 0029 0572  .).r....r....).r
+000053d0: 3c00 0000 7269 0000 0072 6a00 0000 726b  <...ri...rj...rk
+000053e0: 0000 0072 ec00 0000 721f 0000 0072 1f00  ...r....r....r..
+000053f0: 0000 7237 0000 0072 6c00 0000 8402 0000  ..r7...rl.......
+00005400: f304 0000 000e 0108 017a 1750 6879 7369  .........z.Physi
+00005410: 6361 6c44 6174 614d 676d 742e 7570 6c6f  calDataMgmt.uplo
+00005420: 6164 6304 0000 0000 0000 0000 0000 0005  adc.............
+00005430: 0000 0005 0000 0043 0000 0072 0c01 0000  .......C...r....
+00005440: 729b 0000 0029 0272 0e00 0000 da0e 7365  r....).r......se
+00005450: 6172 6368 5f73 616d 706c 6573 a905 723c  arch_samples..r<
+00005460: 0000 0072 6e00 0000 726f 0000 0072 7000  ...rn...ro...rp.
+00005470: 0000 72ec 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00005480: 0072 3700 0000 7271 0000 0088 0200 0072  .r7...rq.......r
+00005490: 0d01 0000 7a1e 5068 7973 6963 616c 4461  ....z.PhysicalDa
+000054a0: 7461 4d67 6d74 2e73 6561 7263 685f 6f62  taMgmt.search_ob
+000054b0: 6a65 6374 6304 0000 0000 0000 0000 0000  jectc...........
+000054c0: 0005 0000 0005 0000 0043 0000 0072 0c01  .........C...r..
+000054d0: 0000 729b 0000 0029 0272 0e00 0000 da10  ..r....).r......
+000054e0: 7365 6172 6368 5f64 6174 615f 7365 7473  search_data_sets
+000054f0: 720f 0100 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00005500: 3700 0000 7272 0000 008c 0200 0072 0d01  7...rr.......r..
+00005510: 0000 7a20 5068 7973 6963 616c 4461 7461  ..z PhysicalData
+00005520: 4d67 6d74 2e73 6561 7263 685f 6461 7461  Mgmt.search_data
+00005530: 5f73 6574 6307 0000 0000 0000 0000 0000  _setc...........
+00005540: 0009 0000 0009 0000 0043 0000 0073 f600  .........C...s..
+00005550: 0000 7c00 6a00 a001 7c01 a101 7d07 7c07  ..|.j...|...}.|.
+00005560: 6401 7500 7210 7402 6402 7c01 1700 8301  d.u.r.t.d.|.....
+00005570: 8201 7c04 7403 6a04 7500 7222 7c05 6401  ..|.t.j.u.r"|.d.
+00005580: 7501 731b 4a00 8201 7c06 6401 7501 7321  u.s.J...|.d.u.s!
+00005590: 4a00 8201 6e1e 7c04 7403 6a05 7500 722e  J...n.|.t.j.u.r.
+000055a0: 7c06 6401 7500 732d 4a00 8201 6e12 7c04  |.d.u.s-J...n.|.
+000055b0: 7403 6a06 7500 7240 7c01 6403 6b03 7240  t.j.u.r@|.d.k.r@
+000055c0: 7c00 a007 7c01 9b00 6404 9d02 6405 a102  |...|...d...d...
+000055d0: 0100 7c01 6406 6b02 724f 7408 7c00 7c04  ..|.d.k.rOt.|.|.
+000055e0: 7c05 7c06 8304 7d08 7c08 a009 a100 5300  |.|...}.|.....S.
+000055f0: 7c01 6407 6b02 725e 740a 7c00 7c04 7c05  |.d.k.r^t.|.|.|.
+00005600: 7c06 8304 7d08 7c08 a009 a100 5300 7c01  |...}.|.....S.|.
+00005610: 6403 6b02 726e 7c00 a00b 7c07 7c00 6a0c  d.k.rn|...|.|.j.
+00005620: 7c02 7c03 7c04 7c05 7c06 a107 5300 7c00  |.|.|.|.|...S.|.
+00005630: a007 7c01 9b00 6408 7c04 9b00 9d03 6405  ..|...d.|.....d.
+00005640: a102 0100 6401 5300 2909 7204 0100 004e  ....d.S.).r....N
+00005650: 7205 0100 0072 0400 0000 7a06 2063 6c65  r....r....z. cle
+00005660: 6172 7208 0100 00da 066f 626a 6563 74da  arr......object.
+00005670: 0a63 6f6c 6c65 6374 696f 6efa 0120 290d  .collection.. ).
+00005680: 722e 0000 0072 d500 0000 723f 0000 0072  r....r....r?...r
+00005690: 1200 0000 727f 0000 0072 7b00 0000 7281  ....r....r{...r.
+000056a0: 0000 0072 4300 0000 720b 0000 0072 ea00  ...rC...r....r..
+000056b0: 0000 7208 0000 0072 8c00 0000 7233 0000  ..r....r....r3..
+000056c0: 0029 0972 3c00 0000 7206 0100 0072 8400  .).r<...r....r..
+000056d0: 0000 7285 0000 0072 8600 0000 7287 0000  ..r....r....r...
+000056e0: 0072 8800 0000 7283 0000 0072 ec00 0000  .r....r....r....
+000056f0: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
+00005700: 0400 0000 9002 0000 7332 0000 000c 0a08  ........s2......
+00005710: 010c 010a 010c 010e 010a 010e 0112 010c  ................
+00005720: 0102 0104 ff08 030e 0108 0108 010e 0108  ................
+00005730: 0108 010e 0106 0104 ff10 0302 0108 ff7a  ...............z
+00005740: 1750 6879 7369 6361 6c44 6174 614d 676d  .PhysicalDataMgm
+00005750: 742e 636f 6e66 6967 729b 0000 0072 9c00  t.configr....r..
+00005760: 0000 729d 0000 0029 1472 9e00 0000 729f  ..r....).r....r.
+00005770: 0000 0072 a000 0000 72a1 0000 0072 4600  ...r....r....rF.
+00005780: 0000 724a 0000 0072 4d00 0000 7251 0000  ..rJ...rM...rQ..
+00005790: 0072 5700 0000 7256 0000 0072 5800 0000  .rW...rV...rX...
+000057a0: 725f 0000 0072 6100 0000 7262 0000 0072  r_...ra...rb...r
+000057b0: 6400 0000 7268 0000 0072 6c00 0000 7271  d...rh...rl...rq
+000057c0: 0000 0072 7200 0000 7204 0000 0072 1f00  ...rr...r....r..
+000057d0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
+000057e0: 0072 2900 0000 5302 0000 7328 0000 0008  .r)...S...s(....
+000057f0: 0004 0108 0208 030a 040a 0a0a 0408 0308  ................
+00005800: 0308 0308 0308 030a 0308 0308 0408 0408  ................
+00005810: 0402 0402 010e ff72 2900 0000 2938 72a2  .......r)...)8r.
+00005820: 0000 0072 7c00 0000 7223 0000 0072 fc00  ...r|...r#...r..
+00005830: 0000 72c0 0000 0072 b100 0000 da07 7061  ..r....r......pa
+00005840: 7468 6c69 6272 0200 0000 72f4 0000 0072  thlibr....r....r
+00005850: 9400 0000 7204 0000 0072 2000 0000 da0e  ....r....r .....
+00005860: 636f 6d6d 616e 645f 7265 7375 6c74 7205  command_resultr.
+00005870: 0000 00da 0f63 6f6d 6d61 6e64 732e 6164  .....commands.ad
+00005880: 6472 6566 7206 0000 00da 0e63 6f6d 6d61  drefr......comma
+00005890: 6e64 732e 636c 6f6e 6572 0700 0000 da13  nds.cloner......
+000058a0: 636f 6d6d 616e 6473 2e63 6f6c 6c65 6374  commands.collect
+000058b0: 696f 6e72 0800 0000 da1a 636f 6d6d 616e  ionr......comman
+000058c0: 6473 2e64 6f77 6e6c 6f61 645f 7068 7973  ds.download_phys
+000058d0: 6963 616c 7209 0000 00da 0d63 6f6d 6d61  icalr......comma
+000058e0: 6e64 732e 6d6f 7665 720a 0000 00da 0f63  nds.mover......c
+000058f0: 6f6d 6d61 6e64 732e 6f62 6a65 6374 720b  ommands.objectr.
+00005900: 0000 00da 1563 6f6d 6d61 6e64 732e 6f70  .....commands.op
+00005910: 656e 6269 735f 7379 6e63 720c 0000 00da  enbis_syncr.....
+00005920: 1263 6f6d 6d61 6e64 732e 7265 6d6f 7665  .commands.remove
+00005930: 7265 6672 0d00 0000 da0f 636f 6d6d 616e  refr......comman
+00005940: 6473 2e73 6561 7263 6872 0e00 0000 da0f  ds.searchr......
+00005950: 636f 6d6d 616e 6473 2e75 706c 6f61 6472  commands.uploadr
+00005960: 0f00 0000 da03 6769 7472 1000 0000 da05  ......gitr......
+00005970: 7574 696c 7372 1100 0000 7212 0000 0072  utilsr....r....r
+00005980: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
+00005990: 0000 00da 1273 6372 6970 7473 2e63 6c69  .....scripts.cli
+000059a0: 636b 5f75 7469 6c72 1800 0000 7219 0000  ck_utilr....r...
+000059b0: 0072 2200 0000 7238 0000 00da 0741 4243  .r"...r8.....ABC
+000059c0: 4d65 7461 7239 0000 0072 2b00 0000 72b4  Metar9...r+...r.
+000059d0: 0000 0072 bf00 0000 72c7 0000 0072 2c00  ...r....r....r,.
+000059e0: 0000 7229 0000 0072 1f00 0000 721f 0000  ..r)...r....r...
+000059f0: 0072 1f00 0000 7237 0000 00da 083c 6d6f  .r....r7.....<mo
+00005a00: 6475 6c65 3e01 0000 0073 4e00 0000 0811  dule>....sN.....
+00005a10: 0801 0801 0801 0801 0801 0c01 0802 0c02  ................
+00005a20: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00005a30: 0c01 0c01 0c01 0c01 1001 0c01 0c01 0c01  ................
+00005a40: 0c01 1001 0804 0c01 0aff 1429 007f 105a  ...........)...Z
+00005a50: 0831 0805 0812 1017 007f 1441            .1.........A
```

### Comparing `obis-0.4.1/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/git.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/git.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Feb 23 08:53:54 2023 UTC, .py size: 8138 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,431 +1,444 @@
-00000000: 6f0d 0d0a 0000 0000 a229 f763 ca1f 0000  o........).c....
+00000000: 6f0d 0d0a 0000 0000 2d65 2564 3621 0000  o.......-e%d6!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
+00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 6402  d.l.m.Z.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 4700 6405 6406  d.l.m.Z...G.d.d.
-00000060: 8400 6406 6507 8303 5a08 4700 6407 6408  ..d.e...Z.G.d.d.
-00000070: 8400 6408 6507 8303 5a09 6401 5300 2909  ..d.e...Z.d.S.).
-00000080: e900 0000 004e e901 0000 0029 02da 1643  .....N.....)...C
-00000090: 6865 636b 7375 6d47 656e 6572 6174 6f72  hecksumGenerator
-000000a0: 4372 6333 32da 1943 6865 636b 7375 6d47  Crc32..ChecksumG
-000000b0: 656e 6572 6174 6f72 4769 7441 6e6e 6578  eneratorGitAnnex
-000000c0: 2901 da09 7275 6e5f 7368 656c 6c63 0000  )...run_shellc..
-000000d0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000000e0: 0000 4000 0000 739a 0000 0065 005a 0164  ..@...s....e.Z.d
-000000f0: 005a 0264 015a 0364 2564 0364 0484 015a  .Z.d.Z.d%d.d...Z
-00000100: 0464 2664 0764 0884 015a 0564 0964 0a84  .d&d.d...Z.d.d..
-00000110: 005a 0664 0b64 0c84 005a 0764 2764 0d64  .Z.d.d...Z.d'd.d
-00000120: 0e84 015a 0864 2764 0f64 1084 015a 0964  ...Z.d'd.d...Z.d
-00000130: 1164 1284 005a 0a64 1364 1484 005a 0b64  .d...Z.d.d...Z.d
-00000140: 1564 1684 005a 0c64 1764 1884 005a 0d64  .d...Z.d.d...Z.d
-00000150: 1964 1a84 005a 0e64 1b64 1c84 005a 0f64  .d...Z.d.d...Z.d
-00000160: 1d64 1e84 005a 1064 2864 1f64 2084 015a  .d...Z.d(d.d ..Z
-00000170: 1164 2164 2284 005a 1264 2364 2484 005a  .d!d"..Z.d#d$..Z
-00000180: 1364 0253 0029 29da 0a47 6974 5772 6170  .d.S.))..GitWrap
-00000190: 7065 727a 2b41 2077 7261 7070 6572 206f  perz+A wrapper o
-000001a0: 6e20 636f 6d6d 616e 6473 2074 6f20 6769  n commands to gi
-000001b0: 7420 616e 6420 6769 7420 616e 6e65 782e  t and git annex.
-000001c0: 4e63 0700 0000 0000 0000 0000 0000 0700  Nc..............
-000001d0: 0000 0200 0000 4300 0000 731c 0000 007c  ......C...s....|
-000001e0: 017c 005f 007c 027c 005f 017c 047c 005f  .|._.|.|._.|.|._
-000001f0: 027c 057c 005f 0364 0053 00a9 014e 2904  .|.|._.d.S...N).
-00000200: da08 6769 745f 7061 7468 da0e 6769 745f  ..git_path..git_
-00000210: 616e 6e65 785f 7061 7468 da09 6461 7461  annex_path..data
-00000220: 5f70 6174 68da 0d6d 6574 6164 6174 615f  _path..metadata_
-00000230: 7061 7468 2907 da04 7365 6c66 7208 0000  path)...selfr...
-00000240: 0072 0900 0000 da08 6669 6e64 5f67 6974  .r......find_git
-00000250: 720a 0000 0072 0b00 0000 da0f 696e 766f  r....r......invo
-00000260: 6361 7469 6f6e 5f70 6174 68a9 0072 0f00  cation_path..r..
-00000270: 0000 fa57 2f68 6f6d 652f 616c 6173 6b6f  ...W/home/alasko
-00000280: 7773 6b69 2f72 6570 6f2f 6f70 656e 6269  wski/repo/openbi
-00000290: 735f 7079 7468 6f6e 2f61 7070 2d6f 7065  s_python/app-ope
-000002a0: 6e62 6973 2d63 6f6d 6d61 6e64 2d6c 696e  nbis-command-lin
-000002b0: 652f 7372 632f 7079 7468 6f6e 2f6f 6269  e/src/python/obi
-000002c0: 732f 646d 2f67 6974 2e70 79da 085f 5f69  s/dm/git.py..__i
-000002d0: 6e69 745f 5f19 0000 0073 0800 0000 0601  nit__....s......
-000002e0: 0601 0601 0a01 7a13 4769 7457 7261 7070  ......z.GitWrapp
-000002f0: 6572 2e5f 5f69 6e69 745f 5f54 da00 6304  er.__init__T..c.
-00000300: 0000 0000 0000 0000 0000 0006 0000 0005  ................
-00000310: 0000 0043 0000 0073 5400 0000 7c00 6a00  ...C...sT...|.j.
-00000320: 6701 7d04 7c00 6a01 6401 7501 7220 7c00  g.}.|.j.d.u.r |.
-00000330: 6a02 6401 7501 7220 7403 6a04 a005 7c00  j.d.u.r t.j...|.
-00000340: 6a02 7c03 6402 a103 7d05 7c04 6403 7c00  j.|.d...}.|.d.|.
-00000350: 6a01 6404 7c05 6704 3700 7d04 7c04 7c01  j.d.|.g.7.}.|.|.
-00000360: 3700 7d04 7406 7c04 7c02 6405 8d02 5300  7.}.t.|.|.d...S.
-00000370: 2906 7a6f 2061 6c6c 2067 6974 2069 6e76  ).zo all git inv
-00000380: 6f63 6174 696f 6e73 206e 6565 6420 746f  ocations need to
-00000390: 2067 6f20 7468 726f 7567 6820 7468 6973   go through this
-000003a0: 206d 6574 686f 640a 2020 2020 2020 2020   method.        
-000003b0: 7369 6e63 6520 6974 2073 6574 7320 2d2d  since it sets --
-000003c0: 776f 726b 2d74 7265 6520 616e 6420 272d  work-tree and '-
-000003d0: 2d67 6974 2d64 6972 2e0a 2020 2020 2020  -git-dir..      
-000003e0: 2020 204e 7a04 2e67 6974 7a0b 2d2d 776f     Nz..gitz.--wo
-000003f0: 726b 2d74 7265 657a 092d 2d67 6974 2d64  rk-treez.--git-d
-00000400: 6972 a901 da18 7374 7269 705f 6c65 6164  ir....strip_lead
-00000410: 696e 675f 7768 6974 6573 7061 6365 2907  ing_whitespace).
-00000420: 7208 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
-00000430: 026f 73da 0470 6174 68da 046a 6f69 6e72  .os..path..joinr
-00000440: 0500 0000 2906 720c 0000 00da 0670 6172  ....).r......par
-00000450: 616d 7372 1400 0000 da12 7265 6c61 7469  amsr......relati
-00000460: 7665 5f72 6570 6f5f 7061 7468 da03 636d  ve_repo_path..cm
-00000470: 64da 0767 6974 5f64 6972 720f 0000 0072  d..git_dirr....r
-00000480: 0f00 0000 7210 0000 00da 045f 6769 741f  ....r......_git.
-00000490: 0000 0073 0c00 0000 0804 1401 1201 1201  ...s............
-000004a0: 0801 0c01 7a0f 4769 7457 7261 7070 6572  ....z.GitWrapper
-000004b0: 2e5f 6769 7463 0100 0000 0000 0000 0000  ._gitc..........
-000004c0: 0000 0400 0000 0a00 0000 4300 0000 73e2  ..........C...s.
-000004d0: 0000 007c 006a 0064 0175 0072 0764 0253  ...|.j.d.u.r.d.S
-000004e0: 007c 006a 0164 0175 0072 0e64 0253 007c  .|.j.d.u.r.d.S.|
-000004f0: 00a0 0264 0367 01a1 01a0 03a1 0072 1864  ...d.g.......r.d
-00000500: 0253 007c 00a0 0264 0464 0367 02a1 01a0  .S.|...d.d.g....
-00000510: 03a1 0072 2364 0253 0074 047c 006a 0064  ...r#d.S.t.|.j.d
-00000520: 0464 0567 0383 017d 017c 01a0 05a1 0072  .d.g...}.|.....r
-00000530: 6f7c 016a 06a0 0764 06a1 0164 0719 00a0  o|.j...d...d....
-00000540: 0764 08a1 017d 0274 087c 0283 0164 096b  .d...}.t.|...d.k
-00000550: 0472 6f7c 0264 0919 00a0 09a1 007c 005f  .ro|.d.......|._
-00000560: 0a7a 0e74 0b7c 006a 0aa0 0764 0aa1 0164  .z.t.|.j...d...d
-00000570: 0719 0083 017c 005f 0c57 0064 0c53 0004  .....|._.W.d.S..
-00000580: 0074 0d79 6e01 007d 0301 007a 0d74 0e64  .t.yn..}...z.t.d
-00000590: 0b7c 016a 0683 0201 0057 0059 0064 017d  .|.j.....W.Y.d.}
-000005a0: 037e 0364 0253 0064 017d 037e 0377 0177  .~.d.S.d.}.~.w.w
-000005b0: 0064 0c53 0029 0d7a 4752 6574 7572 6e20  .d.S.).zGReturn 
-000005c0: 7472 7565 2069 6620 7468 6520 7065 7271  true if the perq
-000005d0: 7569 7369 7465 7320 6172 6520 7361 7469  uisites are sati
-000005e0: 7366 6965 6420 746f 2072 756e 2028 6769  sfied to run (gi
-000005f0: 7420 616e 6420 6769 7420 616e 6e65 7829  t and git annex)
-00000600: 4e46 da04 6865 6c70 da05 616e 6e65 78da  NF..help..annex.
-00000610: 0776 6572 7369 6f6e da01 0a72 0100 0000  .version...r....
-00000620: fa01 3a72 0200 0000 da01 2e7a 1f49 6e76  ..:r.......z.Inv
-00000630: 616c 6964 2067 6974 2d61 6e6e 6578 2076  alid git-annex v
-00000640: 6572 7369 6f6e 206c 696e 653a 5429 0f72  ersion line:T).r
-00000650: 0800 0000 7209 0000 0072 1c00 0000 da07  ....r....r......
-00000660: 6661 696c 7572 6572 0500 0000 da07 7375  failurer......su
-00000670: 6363 6573 73da 066f 7574 7075 74da 0573  ccess..output..s
-00000680: 706c 6974 da03 6c65 6eda 0573 7472 6970  plit..len..strip
-00000690: da0d 616e 6e65 785f 7665 7273 696f 6eda  ..annex_version.
-000006a0: 0369 6e74 da13 616e 6e65 785f 6d61 6a6f  .int..annex_majo
-000006b0: 725f 7665 7273 696f 6eda 0945 7863 6570  r_version..Excep
-000006c0: 7469 6f6e da05 7072 696e 7429 0472 0c00  tion..print).r..
-000006d0: 0000 da06 7265 7375 6c74 da0a 6669 7273  ....result..firs
-000006e0: 745f 6c69 6e65 da01 6572 0f00 0000 720f  t_line..er....r.
-000006f0: 0000 0072 1000 0000 da07 6361 6e5f 7275  ...r......can_ru
-00000700: 6e2b 0000 0073 2c00 0000 0a02 0401 0a01  n+...s,.........
-00000710: 0401 1001 0402 1201 0402 1001 0801 1601  ................
-00000720: 0c01 0e01 0201 1801 0404 0efd 0c01 0e01  ................
-00000730: 0880 02fe 0403 7a12 4769 7457 7261 7070  ......z.GitWrapp
-00000740: 6572 2e63 616e 5f72 756e 6301 0000 0000  er.can_runc.....
-00000750: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00000760: 0000 0073 2400 0000 7c00 a000 6401 6701  ...s$...|...d.g.
-00000770: a101 7d01 7c00 a001 6402 a101 0100 7c00  ..}.|...d.....|.
-00000780: a001 6403 a101 0100 7c01 5300 2904 4eda  ..d.....|.S.).N.
-00000790: 0469 6e69 747a 052e 6f62 6973 7a12 2e6f  .initz..obisz..o
-000007a0: 6269 735f 7265 7374 6f72 6570 6f69 6e74  bis_restorepoint
-000007b0: 2902 721c 0000 00da 0a67 6974 5f69 676e  ).r......git_ign
-000007c0: 6f72 6529 0272 0c00 0000 722e 0000 0072  ore).r....r....r
-000007d0: 0f00 0000 720f 0000 0072 1000 0000 da08  ....r....r......
-000007e0: 6769 745f 696e 6974 4300 0000 7308 0000  git_initC...s...
-000007f0: 000c 010a 010a 0104 017a 1347 6974 5772  .........z.GitWr
-00000800: 6170 7065 722e 6769 745f 696e 6974 6302  apper.git_initc.
-00000810: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000820: 0000 0043 0000 0073 2e00 0000 7c01 6400  ...C...s....|.d.
-00000830: 7500 720d 7c00 6a00 6401 6402 6702 6403  u.r.|.j.d.d.g.d.
-00000840: 6404 8d02 5300 7c00 6a00 6401 6402 7c01  d...S.|.j.d.d.|.
-00000850: 6703 6403 6404 8d02 5300 2905 4e72 1e00  g.d.d...S.).Nr..
-00000860: 0000 da06 7374 6174 7573 4672 1300 0000  ....statusFr....
-00000870: a901 721c 0000 0029 0272 0c00 0000 7216  ..r....).r....r.
-00000880: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000890: 0000 da0a 6769 745f 7374 6174 7573 4900  ....git_statusI.
-000008a0: 0000 7306 0000 0008 0112 0114 027a 1547  ..s..........z.G
-000008b0: 6974 5772 6170 7065 722e 6769 745f 7374  itWrapper.git_st
-000008c0: 6174 7573 6303 0000 0000 0000 0000 0000  atusc...........
-000008d0: 0007 0000 0005 0000 0043 0000 0073 ce00  .........C...s..
-000008e0: 0000 6700 6401 a201 7d03 7c01 6402 7501  ..g.d...}.|.d.u.
-000008f0: 720d 7c03 a000 7c01 a101 0100 7c00 a001  r.|...|.....|...
-00000900: 7c03 a101 7d04 7c04 a002 a100 7218 7c04  |...}.|.....r.|.
-00000910: 5300 6700 6403 a201 7d03 7c00 a001 7c03  S.g.d...}.|...|.
-00000920: a101 7d04 7c04 a002 a100 7227 7c04 5300  ..}.|.....r'|.S.
-00000930: 6404 7c00 6a03 6405 6b05 722f 6406 6e01  d.|.j.d.k.r/d.n.
-00000940: 6407 6702 7d03 7c00 a001 7c03 a101 7d04  d.g.}.|...|...}.
-00000950: 7c04 a002 a100 723d 7c04 5300 6700 6408  |.....r=|.S.g.d.
-00000960: a201 7d03 7c00 a001 7c03 a101 7d04 7c04  ..}.|...|...}.|.
-00000970: a002 a100 724c 7c04 5300 7404 6a05 a006  ....rL|.S.t.j...
-00000980: 7404 6a05 a007 7408 a101 6409 a102 7d05  t.j...t...d...}.
-00000990: 640a 7d06 7409 a00a 7c05 7c06 a102 0100  d.}.t...|.|.....
-000009a0: 7c00 a00b 7c06 7c02 a102 0100 7c04 5300  |...|.|.....|.S.
-000009b0: 290b 7a26 2043 6f6e 6669 6775 7265 7320  ).z& Configures 
-000009c0: 616e 6e65 7820 696e 2061 2067 6974 2072  annex in a git r
-000009d0: 6570 6f73 6974 6f72 792e 2903 721e 0000  epository.).r...
-000009e0: 0072 3200 0000 7a0b 2d2d 7665 7273 696f  .r2...z.--versio
-000009f0: 6e3d 354e 2903 da06 636f 6e66 6967 7a0a  n=5N)...configz.
-00000a00: 616e 6e65 782e 7468 696e da04 7472 7565  annex.thin..true
-00000a10: 721e 0000 00e9 0800 0000 da06 756e 6c6f  r...........unlo
-00000a20: 636b da06 6469 7265 6374 2903 7238 0000  ck..direct).r8..
-00000a30: 007a 072d 2d75 6e73 6574 7a09 636f 7265  .z.--unsetz.core
-00000a40: 2e62 6172 657a 1467 6974 2d61 6e6e 6578  .barez.git-annex
-00000a50: 2d61 7474 7269 6275 7465 737a 142e 6769  -attributesz..gi
-00000a60: 742f 696e 666f 2f61 7474 7269 6275 7465  t/info/attribute
-00000a70: 7329 0cda 0661 7070 656e 6472 1c00 0000  s)...appendr....
-00000a80: 7223 0000 0072 2b00 0000 7215 0000 0072  r#...r+...r....r
-00000a90: 1600 0000 7217 0000 00da 0764 6972 6e61  ....r......dirna
-00000aa0: 6d65 da08 5f5f 6669 6c65 5f5f da06 7368  me..__file__..sh
-00000ab0: 7574 696c da08 636f 7079 6669 6c65 da18  util..copyfile..
-00000ac0: 5f61 7070 6c79 5f67 6974 5f61 6e6e 6578  _apply_git_annex
-00000ad0: 5f62 6163 6b65 6e64 2907 720c 0000 00da  _backend).r.....
-00000ae0: 0464 6573 63da 1167 6974 5f61 6e6e 6578  .desc..git_annex
-00000af0: 5f62 6163 6b65 6e64 721a 0000 0072 2e00  _backendr....r..
-00000b00: 0000 da0e 6174 7472 6962 7574 6573 5f73  ....attributes_s
-00000b10: 7263 da0e 6174 7472 6962 7574 6573 5f64  rc..attributes_d
-00000b20: 7374 720f 0000 0072 0f00 0000 7210 0000  str....r....r...
-00000b30: 00da 0e67 6974 5f61 6e6e 6578 5f69 6e69  ...git_annex_ini
-00000b40: 744f 0000 0073 2e00 0000 0805 0801 0a01  tO...s..........
-00000b50: 0a01 0801 0401 0803 0a01 0801 0401 1603  ................
-00000b60: 0a01 0801 0401 0804 0a01 0801 0401 1603  ................
-00000b70: 0401 0c01 0c01 0402 7a19 4769 7457 7261  ........z.GitWra
-00000b80: 7070 6572 2e67 6974 5f61 6e6e 6578 5f69  pper.git_annex_i
-00000b90: 6e69 7463 0100 0000 0000 0000 0000 0000  nitc............
-00000ba0: 0100 0000 0400 0000 4300 0000 f30e 0000  ........C.......
-00000bb0: 007c 00a0 0067 0064 01a2 01a1 0153 0029  .|...g.d.....S.)
-00000bc0: 024e 2904 da06 636f 6d6d 6974 fa0d 2d2d  .N)...commit..--
-00000bd0: 616c 6c6f 772d 656d 7074 79fa 022d 6d7a  allow-empty..-mz
-00000be0: 0f49 6e69 7469 616c 2063 6f6d 6d69 742e  .Initial commit.
-00000bf0: 7236 0000 00a9 0172 0c00 0000 720f 0000  r6.....r....r...
-00000c00: 0072 0f00 0000 7210 0000 00da 0e69 6e69  .r....r......ini
-00000c10: 7469 616c 5f63 6f6d 6d69 7476 0000 0073  tial_commitv...s
-00000c20: 0200 0000 0e02 7a19 4769 7457 7261 7070  ......z.GitWrapp
-00000c30: 6572 2e69 6e69 7469 616c 5f63 6f6d 6d69  er.initial_commi
-00000c40: 7463 0300 0000 0000 0000 0000 0000 0600  tc..............
-00000c50: 0000 0500 0000 4300 0000 7372 0000 007c  ......C...sr...|
-00000c60: 0264 0075 0172 3767 007d 0374 007c 0164  .d.u.r7g.}.t.|.d
-00000c70: 0183 027d 047c 0444 005d 157d 0564 027c  ...}.|.D.].}.d.|
-00000c80: 0576 0072 1d7c 03a0 0164 037c 0217 0064  .v.r.|...d.|...d
-00000c90: 0417 00a1 0101 0071 0d7c 03a0 017c 05a1  .......q.|...|..
-00000ca0: 0101 0071 0d7c 04a0 02a1 0001 0074 007c  ...q.|.......t.|
-00000cb0: 0164 0583 027d 047c 04a0 037c 03a1 0101  .d...}.|...|....
-00000cc0: 007c 04a0 02a1 0001 0064 0053 0064 0053  .|.......d.S.d.S
-00000cd0: 0029 064e da01 727a 0d61 6e6e 6578 2e62  .).N..rz.annex.b
-00000ce0: 6163 6b65 6e64 7a10 2a20 616e 6e65 782e  ackendz.* annex.
-00000cf0: 6261 636b 656e 643d 7220 0000 00da 0177  backend=r .....w
-00000d00: 2904 da04 6f70 656e 723d 0000 00da 0563  )...openr=.....c
-00000d10: 6c6f 7365 da0a 7772 6974 656c 696e 6573  lose..writelines
-00000d20: 2906 720c 0000 00da 0866 696c 656e 616d  ).r......filenam
-00000d30: 6572 4400 0000 da05 6c69 6e65 73da 0466  erD.....lines..f
-00000d40: 696c 65da 046c 696e 6572 0f00 0000 720f  ile..liner....r.
-00000d50: 0000 0072 1000 0000 7242 0000 007a 0000  ...r....rB...z..
-00000d60: 0073 1800 0000 0801 0401 0a01 0801 0801  .s..............
-00000d70: 1401 0c02 0801 0a01 0a01 0c01 04f5 7a23  ..............z#
-00000d80: 4769 7457 7261 7070 6572 2e5f 6170 706c  GitWrapper._appl
-00000d90: 795f 6769 745f 616e 6e65 785f 6261 636b  y_git_annex_back
-00000da0: 656e 6463 0200 0000 0000 0000 0000 0000  endc............
-00000db0: 0300 0000 0300 0000 4300 0000 7328 0000  ........C...s(..
-00000dc0: 0064 0164 027c 0167 037d 027c 006a 0064  .d.d.|.g.}.|.j.d
-00000dd0: 036b 0072 0f7c 02a0 0164 04a1 0101 007c  .k.r.|...d.....|
-00000de0: 00a0 027c 02a1 0153 0029 054e 721e 0000  ...|...S.).Nr...
-00000df0: 00da 0361 6464 723a 0000 007a 122d 2d69  ...addr:...z.--i
-00000e00: 6e63 6c75 6465 2d64 6f74 6669 6c65 7329  nclude-dotfiles)
-00000e10: 0372 2b00 0000 723d 0000 0072 1c00 0000  .r+...r=...r....
-00000e20: 2903 720c 0000 0072 1600 0000 721a 0000  ).r....r....r...
-00000e30: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000e40: da07 6769 745f 6164 6488 0000 0073 0800  ..git_add....s..
-00000e50: 0000 0a02 0a01 0a01 0a01 7a12 4769 7457  ..........z.GitW
-00000e60: 7261 7070 6572 2e67 6974 5f61 6464 6302  rapper.git_addc.
-00000e70: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00000e80: 0000 0043 0000 0073 1200 0000 7c00 a000  ...C...s....|...
-00000e90: 6401 6402 6403 7c01 6704 a101 5300 2904  d.d.d.|.g...S.).
-00000ea0: 4e72 4900 0000 724a 0000 0072 4b00 0000  NrI...rJ...rK...
-00000eb0: 7236 0000 0029 0272 0c00 0000 da03 6d73  r6...).r......ms
-00000ec0: 6772 0f00 0000 720f 0000 0072 1000 0000  gr....r....r....
-00000ed0: da0a 6769 745f 636f 6d6d 6974 8f00 0000  ..git_commit....
-00000ee0: 7302 0000 0012 017a 1547 6974 5772 6170  s......z.GitWrap
-00000ef0: 7065 722e 6769 745f 636f 6d6d 6974 6301  per.git_commitc.
-00000f00: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000f10: 0000 0043 0000 0073 0e00 0000 7c00 a000  ...C...s....|...
-00000f20: 6401 6402 6702 a101 5300 2903 4efa 0972  d.d.g...S.).N..r
-00000f30: 6576 2d70 6172 7365 7a0f 2d2d 7368 6f77  ev-parsez.--show
-00000f40: 2d74 6f70 6c65 7665 6c72 3600 0000 724c  -toplevelr6...rL
-00000f50: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000f60: 0000 da12 6769 745f 746f 705f 6c65 7665  ....git_top_leve
-00000f70: 6c5f 7061 7468 9200 0000 f302 0000 000e  l_path..........
-00000f80: 017a 1d47 6974 5772 6170 7065 722e 6769  .z.GitWrapper.gi
-00000f90: 745f 746f 705f 6c65 7665 6c5f 7061 7468  t_top_level_path
-00000fa0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000fb0: 0004 0000 0043 0000 0072 4800 0000 2902  .....C...rH...).
-00000fc0: 4e29 0372 5b00 0000 7a07 2d2d 7368 6f72  N).r[...z.--shor
-00000fd0: 74da 0448 4541 4472 3600 0000 724c 0000  t..HEADr6...rL..
-00000fe0: 0072 0f00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000ff0: da0f 6769 745f 636f 6d6d 6974 5f68 6173  ..git_commit_has
-00001000: 6895 0000 0072 5d00 0000 7a1a 4769 7457  h....r]...z.GitW
-00001010: 7261 7070 6572 2e67 6974 5f63 6f6d 6d69  rapper.git_commi
-00001020: 745f 6861 7368 6301 0000 0000 0000 0000  t_hashc.........
-00001030: 0000 0001 0000 0004 0000 0043 0000 0072  ...........C...r
-00001040: 4800 0000 2902 4e29 047a 076c 732d 7472  H...).N).z.ls-tr
-00001050: 6565 7a0b 2d2d 6675 6c6c 2d74 7265 657a  eez.--full-treez
-00001060: 022d 7272 5e00 0000 7236 0000 0072 4c00  .-rr^...r6...rL.
-00001070: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00001080: 00da 0b67 6974 5f6c 735f 7472 6565 9800  ...git_ls_tree..
-00001090: 0000 725d 0000 007a 1647 6974 5772 6170  ..r]...z.GitWrap
-000010a0: 7065 722e 6769 745f 6c73 5f74 7265 6563  per.git_ls_treec
-000010b0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-000010c0: 0400 0000 4300 0000 7324 0000 007c 0272  ....C...s$...|.r
-000010d0: 0b7c 006a 0064 017c 0167 027c 0264 028d  .|.j.d.|.g.|.d..
-000010e0: 0253 007c 00a0 0064 017c 0167 02a1 0153  .S.|...d.|.g...S
-000010f0: 0029 034e da08 6368 6563 6b6f 7574 2901  .).N..checkout).
-00001100: 7219 0000 0072 3600 0000 2903 720c 0000  r....r6...).r...
-00001110: 00da 0c70 6174 685f 6f72 5f68 6173 6872  ...path_or_hashr
-00001120: 1900 0000 720f 0000 0072 0f00 0000 7210  ....r....r....r.
-00001130: 0000 00da 0c67 6974 5f63 6865 636b 6f75  .....git_checkou
-00001140: 749b 0000 0073 0600 0000 0401 1201 0e01  t....s..........
-00001150: 7a17 4769 7457 7261 7070 6572 2e67 6974  z.GitWrapper.git
-00001160: 5f63 6865 636b 6f75 7463 0200 0000 0000  _checkoutc......
-00001170: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00001180: 0000 730e 0000 007c 00a0 0064 017c 0167  ..s....|...d.|.g
-00001190: 02a1 0153 0029 024e da05 7265 7365 7472  ...S.).N..resetr
-000011a0: 3600 0000 2902 720c 0000 00da 0b63 6f6d  6...).r......com
-000011b0: 6d69 745f 6861 7368 720f 0000 0072 0f00  mit_hashr....r..
-000011c0: 0000 7210 0000 00da 0c67 6974 5f72 6573  ..r......git_res
-000011d0: 6574 5f74 6fa0 0000 0072 5d00 0000 7a17  et_to....r]...z.
-000011e0: 4769 7457 7261 7070 6572 2e67 6974 5f72  GitWrapper.git_r
-000011f0: 6573 6574 5f74 6f63 0200 0000 0000 0000  eset_toc........
-00001200: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-00001210: 7360 0000 007c 00a0 0064 017c 0167 02a1  s`...|...d.|.g..
-00001220: 017d 027c 026a 0164 026b 0272 2e74 0264  .}.|.j.d.k.r.t.d
-00001230: 0364 0483 028f 137d 037c 03a0 037c 01a1  .d.....}.|...|..
-00001240: 0101 007c 03a0 0364 05a1 0101 0057 0064  ...|...d.....W.d
-00001250: 0004 0004 0083 0301 0064 0053 0031 0073  .........d.S.1.s
-00001260: 2777 0101 0001 0001 0059 0001 0064 0053  'w.......Y...d.S
-00001270: 0064 0053 0029 064e 7a0c 6368 6563 6b2d  .d.S.).Nz.check-
-00001280: 6967 6e6f 7265 7202 0000 007a 112e 6769  ignorer....z..gi
-00001290: 742f 696e 666f 2f65 7863 6c75 6465 da01  t/info/exclude..
-000012a0: 6172 2000 0000 2904 721c 0000 00da 0a72  ar ...).r......r
-000012b0: 6574 7572 6e63 6f64 6572 5000 0000 da05  eturncoderP.....
-000012c0: 7772 6974 6529 0472 0c00 0000 7216 0000  write).r....r...
-000012d0: 0072 2e00 0000 da09 6769 7469 676e 6f72  .r......gitignor
-000012e0: 6572 0f00 0000 720f 0000 0072 1000 0000  er....r....r....
-000012f0: 7233 0000 00a3 0000 0073 0e00 0000 0e01  r3.......s......
-00001300: 0a01 0c01 0a01 0c01 22fe 04ff 7a15 4769  ........"...z.Gi
-00001310: 7457 7261 7070 6572 2e67 6974 5f69 676e  tWrapper.git_ign
-00001320: 6f72 6529 064e 4e4e 4e4e 4e29 0254 7212  ore).NNNNNN).Tr.
-00001330: 0000 0072 0700 0000 2901 7212 0000 0029  ...r....).r....)
-00001340: 14da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001350: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001360: 616d 655f 5fda 075f 5f64 6f63 5f5f 7211  ame__..__doc__r.
-00001370: 0000 0072 1c00 0000 7231 0000 0072 3400  ...r....r1...r4.
-00001380: 0000 7237 0000 0072 4700 0000 724d 0000  ..r7...rG...rM..
-00001390: 0072 4200 0000 7258 0000 0072 5a00 0000  .rB...rX...rZ...
-000013a0: 725c 0000 0072 5f00 0000 7260 0000 0072  r\...r_...r`...r
-000013b0: 6300 0000 7266 0000 0072 3300 0000 720f  c...rf...r3...r.
-000013c0: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-000013d0: 0000 7206 0000 0016 0000 0073 2400 0000  ..r........s$...
-000013e0: 0800 0401 0a02 0a06 080c 0818 0a06 0a06  ................
-000013f0: 0827 0804 080e 0807 0803 0803 0803 0a03  .'..............
-00001400: 0805 0c03 7206 0000 0063 0000 0000 0000  ....r....c......
-00001410: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00001420: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
-00001430: 015a 0364 0264 0384 005a 0464 0c64 0564  .Z.d.d...Z.d.d.d
-00001440: 0684 015a 0564 0764 0884 005a 0664 0c64  ...Z.d.d...Z.d.d
-00001450: 0964 0a84 015a 0764 0b53 0029 0dda 0f47  .d...Z.d.S.)...G
-00001460: 6974 5265 706f 4669 6c65 496e 666f 7a48  itRepoFileInfozH
-00001470: 436c 6173 7320 7468 6174 2067 6174 6865  Class that gathe
-00001480: 7273 2063 6865 636b 7375 6d73 2061 6e64  rs checksums and
-00001490: 2066 696c 6520 6c65 6e67 7468 7320 666f   file lengths fo
-000014a0: 7220 616c 6c20 6669 6c65 7320 696e 2074  r all files in t
-000014b0: 6865 2072 6570 6f2e 6302 0000 0000 0000  he repo.c.......
-000014c0: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
-000014d0: 0073 0a00 0000 7c01 7c00 5f00 6400 5300  .s....|.|._.d.S.
-000014e0: 7207 0000 0029 01da 0b67 6974 5f77 7261  r....)...git_wra
-000014f0: 7070 6572 2902 720c 0000 0072 7000 0000  pper).r....rp...
-00001500: 720f 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00001510: 1100 0000 ae00 0000 7302 0000 000a 017a  ........s......z
-00001520: 1847 6974 5265 706f 4669 6c65 496e 666f  .GitRepoFileInfo
-00001530: 2e5f 5f69 6e69 745f 5f46 6302 0000 0000  .__init__Fc.....
-00001540: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00001550: 0000 0073 1800 0000 7c00 a000 a100 7d02  ...s....|.....}.
-00001560: 7c00 a001 7c02 7c01 a102 7d03 7c03 5300  |...|.|...}.|.S.
-00001570: 2901 6162 0100 0052 6574 7572 6e20 6120  ).ab...Return a 
-00001580: 6c69 7374 206f 6620 6469 6374 7320 6465  list of dicts de
-00001590: 7363 7269 6269 6e67 2074 6865 2063 6f6e  scribing the con
-000015a0: 7465 6e74 7320 6f66 2074 6865 2072 6570  tents of the rep
-000015b0: 6f2e 0a20 2020 2020 2020 203a 7265 7475  o..        :retu
-000015c0: 726e 3a20 4120 6c69 7374 206f 6620 6469  rn: A list of di
-000015d0: 6374 696f 6e61 7269 6573 0a20 2020 2020  ctionaries.     
-000015e0: 2020 2020 207b 2763 7263 3332 273a 2063       {'crc32': c
-000015f0: 6865 636b 7375 6d2c 0a20 2020 2020 2020  hecksum,.       
-00001600: 2020 2020 2763 6865 636b 7375 6d27 3a20      'checksum': 
-00001610: 6368 6563 6b73 756d 206f 7468 6572 2074  checksum other t
-00001620: 6861 6e20 6372 6333 320a 2020 2020 2020  han crc32.      
-00001630: 2020 2020 2027 6368 6563 6b73 756d 5479       'checksumTy
-00001640: 7065 273a 2074 7970 6520 6f66 2063 6865  pe': type of che
-00001650: 636b 7375 6d0a 2020 2020 2020 2020 2020  cksum.          
-00001660: 2027 6669 6c65 4c65 6e67 7468 273a 2073   'fileLength': s
-00001670: 697a 6520 6f66 2074 6865 2066 696c 652c  ize of the file,
-00001680: 0a20 2020 2020 2020 2020 2020 2770 6174  .           'pat
-00001690: 6827 3a20 7061 7468 2072 656c 6174 6976  h': path relativ
-000016a0: 6520 746f 2072 6570 6f20 726f 6f74 2e0a  e to repo root..
-000016b0: 2020 2020 2020 2020 2020 2027 6469 7265             'dire
-000016c0: 6374 6f72 7927 3a20 4661 6c73 650a 2020  ctory': False.  
-000016d0: 2020 2020 2020 2020 7d29 02da 0966 696c          })...fil
-000016e0: 655f 6c69 7374 da05 636b 7375 6d29 0472  e_list..cksum).r
-000016f0: 0c00 0000 da1a 6769 745f 616e 6e65 785f  ......git_annex_
-00001700: 6861 7368 5f61 735f 6368 6563 6b73 756d  hash_as_checksum
-00001710: da05 6669 6c65 7372 7200 0000 720f 0000  ..filesrr...r...
-00001720: 0072 0f00 0000 7210 0000 00da 0863 6f6e  .r....r......con
-00001730: 7465 6e74 73b1 0000 0073 0600 0000 080a  tents....s......
-00001740: 0c01 0401 7a18 4769 7452 6570 6f46 696c  ....z.GitRepoFil
-00001750: 6549 6e66 6f2e 636f 6e74 656e 7473 6301  eInfo.contentsc.
-00001760: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00001770: 0000 0043 0000 0073 4200 0000 7c00 6a00  ...C...sB...|.j.
-00001780: a001 a100 7d01 7c01 a002 a100 7310 7403  ....}.|.....s.t.
-00001790: 7c01 6a04 8301 6401 6b02 7212 6700 5300  |.j...d.k.r.g.S.
-000017a0: 7c01 6a04 a005 6402 a101 7d02 6403 6404  |.j...d...}.d.d.
-000017b0: 8400 7c02 4400 8301 7d03 7c03 5300 2905  ..|.D...}.|.S.).
-000017c0: 4e72 0100 0000 7220 0000 0063 0100 0000  Nr....r ...c....
-000017d0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000017e0: 5300 0000 731e 0000 0067 007c 005d 0b7d  S...s....g.|.].}
-000017f0: 017c 01a0 0064 00a1 0164 0119 00a0 01a1  .|...d...d......
-00001800: 0091 0271 0253 0029 02fa 0109 e9ff ffff  ...q.S.)........
-00001810: ff29 0272 2600 0000 7228 0000 0029 02da  .).r&...r(...)..
-00001820: 022e 3072 5600 0000 720f 0000 0072 0f00  ..0rV...r....r..
-00001830: 0000 7210 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
-00001840: 6d70 3ec4 0000 0073 0200 0000 1e00 7a2d  mp>....s......z-
-00001850: 4769 7452 6570 6f46 696c 6549 6e66 6f2e  GitRepoFileInfo.
-00001860: 6669 6c65 5f6c 6973 742e 3c6c 6f63 616c  file_list.<local
-00001870: 733e 2e3c 6c69 7374 636f 6d70 3e29 0672  s>.<listcomp>).r
-00001880: 7000 0000 7260 0000 0072 2300 0000 7227  p...r`...r#...r'
-00001890: 0000 0072 2500 0000 7226 0000 0029 0472  ...r%...r&...).r
-000018a0: 0c00 0000 da04 7472 6565 7254 0000 0072  ......treerT...r
-000018b0: 7400 0000 720f 0000 0072 0f00 0000 7210  t...r....r....r.
-000018c0: 0000 0072 7100 0000 bf00 0000 730c 0000  ...rq.......s...
-000018d0: 000a 0116 0104 010c 010e 0104 017a 1947  .............z.G
-000018e0: 6974 5265 706f 4669 6c65 496e 666f 2e66  itRepoFileInfo.f
-000018f0: 696c 655f 6c69 7374 6303 0000 0000 0000  ile_listc.......
-00001900: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
-00001910: 0073 5400 0000 7c02 6401 6b02 720e 7400  .sT...|.d.k.r.t.
-00001920: 7c00 6a01 6a02 7c00 6a01 6a03 8302 7d03  |.j.j.|.j.j...}.
-00001930: 6e09 7404 7c00 6a01 6a02 7c00 6a01 6a03  n.t.|.j.j.|.j.j.
-00001940: 8302 7d03 6700 7d04 7c01 4400 5d0c 7d05  ..}.g.}.|.D.].}.
-00001950: 7c03 a005 7c05 a101 7d06 7c04 a006 7c06  |...|...}.|...|.
-00001960: a101 0100 711b 7c04 5300 2902 4e46 2907  ....q.|.S.).NF).
-00001970: 7203 0000 0072 7000 0000 720a 0000 0072  r....rp...r....r
-00001980: 0b00 0000 7204 0000 00da 0c67 6574 5f63  ....r......get_c
-00001990: 6865 636b 7375 6d72 3d00 0000 2907 720c  hecksumr=...).r.
-000019a0: 0000 0072 7400 0000 7273 0000 00da 1263  ...rt...rs.....c
-000019b0: 6865 636b 7375 6d5f 6765 6e65 7261 746f  hecksum_generato
-000019c0: 72da 0963 6865 636b 7375 6d73 7255 0000  r..checksumsrU..
-000019d0: 00da 0863 6865 636b 7375 6d72 0f00 0000  ...checksumr....
-000019e0: 720f 0000 0072 1000 0000 7272 0000 00c7  r....r....rr....
-000019f0: 0000 0073 1000 0000 0802 1401 1202 0402  ...s............
-00001a00: 0802 0a01 0c01 0402 7a15 4769 7452 6570  ........z.GitRep
-00001a10: 6f46 696c 6549 6e66 6f2e 636b 7375 6d4e  oFileInfo.cksumN
-00001a20: 2901 4629 0872 6b00 0000 726c 0000 0072  ).F).rk...rl...r
-00001a30: 6d00 0000 726e 0000 0072 1100 0000 7275  m...rn...r....ru
-00001a40: 0000 0072 7100 0000 7272 0000 0072 0f00  ...rq...rr...r..
-00001a50: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00001a60: 0072 6f00 0000 ab00 0000 730c 0000 0008  .ro.......s.....
-00001a70: 0004 0108 020a 0308 0e0e 0872 6f00 0000  ...........ro...
-00001a80: 290a 7215 0000 0072 4000 0000 727e 0000  ).r....r@...r~..
-00001a90: 0072 0300 0000 7204 0000 00da 0575 7469  .r....r......uti
-00001aa0: 6c73 7205 0000 00da 066f 626a 6563 7472  lsr......objectr
-00001ab0: 0600 0000 726f 0000 0072 0f00 0000 720f  ....ro...r....r.
-00001ac0: 0000 0072 0f00 0000 7210 0000 00da 083c  ...r....r......<
-00001ad0: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-00001ae0: 080e 0801 1002 0c01 1003 007f 1416       ..............
+00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
+00000060: 6d08 5a08 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
+00000070: 6509 8303 5a0a 4700 6409 640a 8400 640a  e...Z.G.d.d...d.
+00000080: 6509 8303 5a0b 6401 5300 290b e900 0000  e...Z.d.S.).....
+00000090: 004e e901 0000 0029 02da 1643 6865 636b  .N.....)...Check
+000000a0: 7375 6d47 656e 6572 6174 6f72 4372 6333  sumGeneratorCrc3
+000000b0: 32da 1943 6865 636b 7375 6d47 656e 6572  2..ChecksumGener
+000000c0: 6174 6f72 4769 7441 6e6e 6578 2901 da09  atorGitAnnex)...
+000000d0: 7275 6e5f 7368 656c 6ce9 0200 0000 2901  run_shell.....).
+000000e0: da0a 636c 6963 6b5f 6563 686f 6300 0000  ..click_echoc...
+000000f0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000100: 0040 0000 0073 9e00 0000 6500 5a01 6400  .@...s....e.Z.d.
+00000110: 5a02 6401 5a03 0902 0902 6425 6403 6404  Z.d.Z.....d%d.d.
+00000120: 8401 5a04 6426 6407 6408 8401 5a05 6409  ..Z.d&d.d...Z.d.
+00000130: 640a 8400 5a06 640b 640c 8400 5a07 6427  d...Z.d.d...Z.d'
+00000140: 640d 640e 8401 5a08 6427 640f 6410 8401  d.d...Z.d'd.d...
+00000150: 5a09 6411 6412 8400 5a0a 6413 6414 8400  Z.d.d...Z.d.d...
+00000160: 5a0b 6415 6416 8400 5a0c 6417 6418 8400  Z.d.d...Z.d.d...
+00000170: 5a0d 6419 641a 8400 5a0e 641b 641c 8400  Z.d.d...Z.d.d...
+00000180: 5a0f 641d 641e 8400 5a10 6428 641f 6420  Z.d.d...Z.d(d.d 
+00000190: 8401 5a11 6421 6422 8400 5a12 6423 6424  ..Z.d!d"..Z.d#d$
+000001a0: 8400 5a13 6402 5300 2929 da0a 4769 7457  ..Z.d.S.))..GitW
+000001b0: 7261 7070 6572 7a2b 4120 7772 6170 7065  rapperz+A wrappe
+000001c0: 7220 6f6e 2063 6f6d 6d61 6e64 7320 746f  r on commands to
+000001d0: 2067 6974 2061 6e64 2067 6974 2061 6e6e   git and git ann
+000001e0: 6578 2e4e 6307 0000 0000 0000 0000 0000  ex.Nc...........
+000001f0: 0007 0000 0002 0000 0043 0000 0073 1c00  .........C...s..
+00000200: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c04  ..|.|._.|.|._.|.
+00000210: 7c00 5f02 7c05 7c00 5f03 6400 5300 a901  |._.|.|._.d.S...
+00000220: 4e29 04da 0867 6974 5f70 6174 68da 0e67  N)...git_path..g
+00000230: 6974 5f61 6e6e 6578 5f70 6174 68da 0964  it_annex_path..d
+00000240: 6174 615f 7061 7468 da0d 6d65 7461 6461  ata_path..metada
+00000250: 7461 5f70 6174 6829 07da 0473 656c 6672  ta_path)...selfr
+00000260: 0a00 0000 720b 0000 00da 0866 696e 645f  ....r......find_
+00000270: 6769 7472 0c00 0000 720d 0000 00da 0f69  gitr....r......i
+00000280: 6e76 6f63 6174 696f 6e5f 7061 7468 a900  nvocation_path..
+00000290: 7211 0000 00fa 572f 686f 6d65 2f61 6c61  r.....W/home/ala
+000002a0: 736b 6f77 736b 692f 7265 706f 2f6f 7065  skowski/repo/ope
+000002b0: 6e62 6973 5f70 7974 686f 6e2f 6170 702d  nbis_python/app-
+000002c0: 6f70 656e 6269 732d 636f 6d6d 616e 642d  openbis-command-
+000002d0: 6c69 6e65 2f73 7263 2f70 7974 686f 6e2f  line/src/python/
+000002e0: 6f62 6973 2f64 6d2f 6769 742e 7079 da08  obis/dm/git.py..
+000002f0: 5f5f 696e 6974 5f5f 1a00 0000 7308 0000  __init__....s...
+00000300: 0006 0206 0106 010a 017a 1347 6974 5772  .........z.GitWr
+00000310: 6170 7065 722e 5f5f 696e 6974 5f5f 54da  apper.__init__T.
+00000320: 0063 0400 0000 0000 0000 0000 0000 0600  .c..............
+00000330: 0000 0500 0000 4300 0000 7354 0000 007c  ......C...sT...|
+00000340: 006a 0067 017d 047c 006a 0164 0175 0172  .j.g.}.|.j.d.u.r
+00000350: 207c 006a 0264 0175 0172 2074 036a 04a0   |.j.d.u.r t.j..
+00000360: 057c 006a 027c 0364 02a1 037d 057c 0464  .|.j.|.d...}.|.d
+00000370: 037c 006a 0164 047c 0567 0437 007d 047c  .|.j.d.|.g.7.}.|
+00000380: 047c 0137 007d 0474 067c 047c 0264 058d  .|.7.}.t.|.|.d..
+00000390: 0253 0029 067a 6f20 616c 6c20 6769 7420  .S.).zo all git 
+000003a0: 696e 766f 6361 7469 6f6e 7320 6e65 6564  invocations need
+000003b0: 2074 6f20 676f 2074 6872 6f75 6768 2074   to go through t
+000003c0: 6869 7320 6d65 7468 6f64 0a20 2020 2020  his method.     
+000003d0: 2020 2073 696e 6365 2069 7420 7365 7473     since it sets
+000003e0: 202d 2d77 6f72 6b2d 7472 6565 2061 6e64   --work-tree and
+000003f0: 2027 2d2d 6769 742d 6469 722e 0a20 2020   '--git-dir..   
+00000400: 2020 2020 2020 4e7a 042e 6769 747a 0b2d        Nz..gitz.-
+00000410: 2d77 6f72 6b2d 7472 6565 7a09 2d2d 6769  -work-treez.--gi
+00000420: 742d 6469 72a9 01da 1873 7472 6970 5f6c  t-dir....strip_l
+00000430: 6561 6469 6e67 5f77 6869 7465 7370 6163  eading_whitespac
+00000440: 6529 0772 0a00 0000 720c 0000 0072 0d00  e).r....r....r..
+00000450: 0000 da02 6f73 da04 7061 7468 da04 6a6f  ....os..path..jo
+00000460: 696e 7205 0000 0029 0672 0e00 0000 da06  inr....).r......
+00000470: 7061 7261 6d73 7216 0000 00da 1272 656c  paramsr......rel
+00000480: 6174 6976 655f 7265 706f 5f70 6174 68da  ative_repo_path.
+00000490: 0363 6d64 da07 6769 745f 6469 7272 1100  .cmd..git_dirr..
+000004a0: 0000 7211 0000 0072 1200 0000 da04 5f67  ..r....r......_g
+000004b0: 6974 2100 0000 730c 0000 0008 0414 0112  it!...s.........
+000004c0: 0112 0108 010c 017a 0f47 6974 5772 6170  .......z.GitWrap
+000004d0: 7065 722e 5f67 6974 6301 0000 0000 0000  per._gitc.......
+000004e0: 0000 0000 0004 0000 000a 0000 0043 0000  .............C..
+000004f0: 0073 0201 0000 7c00 6a00 6401 7500 720b  .s....|.j.d.u.r.
+00000500: 7401 6402 8301 0100 6403 5300 7c00 6a02  t.d.....d.S.|.j.
+00000510: 6401 7500 7216 7401 6404 8301 0100 6403  d.u.r.t.d.....d.
+00000520: 5300 7c00 a003 6405 6701 a101 a004 a100  S.|...d.g.......
+00000530: 7224 7401 6406 8301 0100 6403 5300 7c00  r$t.d.....d.S.|.
+00000540: a003 6407 6405 6702 a101 a004 a100 7233  ..d.d.g.......r3
+00000550: 7401 6408 8301 0100 6403 5300 7405 7c00  t.d.....d.S.t.|.
+00000560: 6a00 6407 6409 6703 8301 7d01 7c01 a006  j.d.d.g...}.|...
+00000570: a100 727f 7c01 6a07 a008 640a a101 640b  ..r.|.j...d...d.
+00000580: 1900 a008 640c a101 7d02 7409 7c02 8301  ....d...}.t.|...
+00000590: 640d 6b04 727f 7c02 640d 1900 a00a a100  d.k.r.|.d.......
+000005a0: 7c00 5f0b 7a0e 740c 7c00 6a0b a008 640e  |._.z.t.|.j...d.
+000005b0: a101 640b 1900 8301 7c00 5f0d 5700 6410  ..d.....|._.W.d.
+000005c0: 5300 0400 740e 797e 0100 7d03 0100 7a0d  S...t.y~..}...z.
+000005d0: 740f 640f 7c01 6a07 8302 0100 5700 5900  t.d.|.j.....W.Y.
+000005e0: 6401 7d03 7e03 6403 5300 6401 7d03 7e03  d.}.~.d.S.d.}.~.
+000005f0: 7701 7700 6410 5300 2911 7a47 5265 7475  w.w.d.S.).zGRetu
+00000600: 726e 2074 7275 6520 6966 2074 6865 2070  rn true if the p
+00000610: 6572 7175 6973 6974 6573 2061 7265 2073  erquisites are s
+00000620: 6174 6973 6669 6564 2074 6f20 7275 6e20  atisfied to run 
+00000630: 2867 6974 2061 6e64 2067 6974 2061 6e6e  (git and git ann
+00000640: 6578 294e 7a12 4e6f 2067 6974 2070 6174  ex)Nz.No git pat
+00000650: 6820 666f 756e 6421 467a 184e 6f20 6769  h found!Fz.No gi
+00000660: 742d 616e 6e65 7820 7061 7468 2066 6f75  t-annex path fou
+00000670: 6e64 21da 0468 656c 707a 1043 616e 206e  nd!..helpz.Can n
+00000680: 6f74 2072 756e 2067 6974 21da 0561 6e6e  ot run git!..ann
+00000690: 6578 7a16 4361 6e20 6e6f 7420 7275 6e20  exz.Can not run 
+000006a0: 6769 742d 616e 6e65 7821 da07 7665 7273  git-annex!..vers
+000006b0: 696f 6eda 010a 7201 0000 00fa 013a 7202  ion...r......:r.
+000006c0: 0000 00da 012e 7a1f 496e 7661 6c69 6420  ......z.Invalid 
+000006d0: 6769 742d 616e 6e65 7820 7665 7273 696f  git-annex versio
+000006e0: 6e20 6c69 6e65 3a54 2910 720a 0000 0072  n line:T).r....r
+000006f0: 0700 0000 720b 0000 0072 1e00 0000 da07  ....r....r......
+00000700: 6661 696c 7572 6572 0500 0000 da07 7375  failurer......su
+00000710: 6363 6573 73da 066f 7574 7075 74da 0573  ccess..output..s
+00000720: 706c 6974 da03 6c65 6eda 0573 7472 6970  plit..len..strip
+00000730: da0d 616e 6e65 785f 7665 7273 696f 6eda  ..annex_version.
+00000740: 0369 6e74 da13 616e 6e65 785f 6d61 6a6f  .int..annex_majo
+00000750: 725f 7665 7273 696f 6eda 0945 7863 6570  r_version..Excep
+00000760: 7469 6f6e da05 7072 696e 7429 0472 0e00  tion..print).r..
+00000770: 0000 da06 7265 7375 6c74 da0a 6669 7273  ....result..firs
+00000780: 745f 6c69 6e65 da01 6572 1100 0000 7211  t_line..er....r.
+00000790: 0000 0072 1200 0000 da07 6361 6e5f 7275  ...r......can_ru
+000007a0: 6e2c 0000 0073 3400 0000 0a02 0801 0401  n,...s4.........
+000007b0: 0a01 0801 0401 1001 0801 0402 1201 0801  ................
+000007c0: 0402 1001 0801 1601 0c01 0e01 0201 1801  ................
+000007d0: 0404 0efd 0c01 0e01 0880 02fe 0403 7a12  ..............z.
+000007e0: 4769 7457 7261 7070 6572 2e63 616e 5f72  GitWrapper.can_r
+000007f0: 756e 6301 0000 0000 0000 0000 0000 0002  unc.............
+00000800: 0000 0003 0000 0043 0000 0073 2400 0000  .......C...s$...
+00000810: 7c00 a000 6401 6701 a101 7d01 7c00 a001  |...d.g...}.|...
+00000820: 6402 a101 0100 7c00 a001 6403 a101 0100  d.....|...d.....
+00000830: 7c01 5300 2904 4eda 0469 6e69 747a 052e  |.S.).N..initz..
+00000840: 6f62 6973 7a12 2e6f 6269 735f 7265 7374  obisz..obis_rest
+00000850: 6f72 6570 6f69 6e74 2902 721e 0000 00da  orepoint).r.....
+00000860: 0a67 6974 5f69 676e 6f72 6529 0272 0e00  .git_ignore).r..
+00000870: 0000 7230 0000 0072 1100 0000 7211 0000  ..r0...r....r...
+00000880: 0072 1200 0000 da08 6769 745f 696e 6974  .r......git_init
+00000890: 4800 0000 7308 0000 000c 010a 010a 0104  H...s...........
+000008a0: 017a 1347 6974 5772 6170 7065 722e 6769  .z.GitWrapper.gi
+000008b0: 745f 696e 6974 6302 0000 0000 0000 0000  t_initc.........
+000008c0: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
+000008d0: 2e00 0000 7c01 6400 7500 720d 7c00 6a00  ....|.d.u.r.|.j.
+000008e0: 6401 6402 6702 6403 6404 8d02 5300 7c00  d.d.g.d.d...S.|.
+000008f0: 6a00 6401 6402 7c01 6703 6403 6404 8d02  j.d.d.|.g.d.d...
+00000900: 5300 2905 4e72 2000 0000 da06 7374 6174  S.).Nr .....stat
+00000910: 7573 4672 1500 0000 a901 721e 0000 0029  usFr......r....)
+00000920: 0272 0e00 0000 7218 0000 0072 1100 0000  .r....r....r....
+00000930: 7211 0000 0072 1200 0000 da0a 6769 745f  r....r......git_
+00000940: 7374 6174 7573 4e00 0000 7306 0000 0008  statusN...s.....
+00000950: 0112 0114 027a 1547 6974 5772 6170 7065  .....z.GitWrappe
+00000960: 722e 6769 745f 7374 6174 7573 6303 0000  r.git_statusc...
+00000970: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00000980: 0043 0000 0073 ce00 0000 6700 6401 a201  .C...s....g.d...
+00000990: 7d03 7c01 6402 7501 720d 7c03 a000 7c01  }.|.d.u.r.|...|.
+000009a0: a101 0100 7c00 a001 7c03 a101 7d04 7c04  ....|...|...}.|.
+000009b0: a002 a100 7218 7c04 5300 6700 6403 a201  ....r.|.S.g.d...
+000009c0: 7d03 7c00 a001 7c03 a101 7d04 7c04 a002  }.|...|...}.|...
+000009d0: a100 7227 7c04 5300 6404 7c00 6a03 6405  ..r'|.S.d.|.j.d.
+000009e0: 6b05 722f 6406 6e01 6407 6702 7d03 7c00  k.r/d.n.d.g.}.|.
+000009f0: a001 7c03 a101 7d04 7c04 a002 a100 723d  ..|...}.|.....r=
+00000a00: 7c04 5300 6700 6408 a201 7d03 7c00 a001  |.S.g.d...}.|...
+00000a10: 7c03 a101 7d04 7c04 a002 a100 724c 7c04  |...}.|.....rL|.
+00000a20: 5300 7404 6a05 a006 7404 6a05 a007 7408  S.t.j...t.j...t.
+00000a30: a101 6409 a102 7d05 640a 7d06 7409 a00a  ..d...}.d.}.t...
+00000a40: 7c05 7c06 a102 0100 7c00 a00b 7c06 7c02  |.|.....|...|.|.
+00000a50: a102 0100 7c04 5300 290b 7a26 2043 6f6e  ....|.S.).z& Con
+00000a60: 6669 6775 7265 7320 616e 6e65 7820 696e  figures annex in
+00000a70: 2061 2067 6974 2072 6570 6f73 6974 6f72   a git repositor
+00000a80: 792e 2903 7220 0000 0072 3400 0000 7a0b  y.).r ...r4...z.
+00000a90: 2d2d 7665 7273 696f 6e3d 354e 2903 da06  --version=5N)...
+00000aa0: 636f 6e66 6967 7a0a 616e 6e65 782e 7468  configz.annex.th
+00000ab0: 696e da04 7472 7565 7220 0000 00e9 0800  in..truer ......
+00000ac0: 0000 da06 756e 6c6f 636b da06 6469 7265  ....unlock..dire
+00000ad0: 6374 2903 723a 0000 007a 072d 2d75 6e73  ct).r:...z.--uns
+00000ae0: 6574 7a09 636f 7265 2e62 6172 657a 1467  etz.core.barez.g
+00000af0: 6974 2d61 6e6e 6578 2d61 7474 7269 6275  it-annex-attribu
+00000b00: 7465 737a 142e 6769 742f 696e 666f 2f61  tesz..git/info/a
+00000b10: 7474 7269 6275 7465 7329 0cda 0661 7070  ttributes)...app
+00000b20: 656e 6472 1e00 0000 7225 0000 0072 2d00  endr....r%...r-.
+00000b30: 0000 7217 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000b40: 00da 0764 6972 6e61 6d65 da08 5f5f 6669  ...dirname..__fi
+00000b50: 6c65 5f5f da06 7368 7574 696c da08 636f  le__..shutil..co
+00000b60: 7079 6669 6c65 da18 5f61 7070 6c79 5f67  pyfile.._apply_g
+00000b70: 6974 5f61 6e6e 6578 5f62 6163 6b65 6e64  it_annex_backend
+00000b80: 2907 720e 0000 00da 0464 6573 63da 1167  ).r......desc..g
+00000b90: 6974 5f61 6e6e 6578 5f62 6163 6b65 6e64  it_annex_backend
+00000ba0: 721c 0000 0072 3000 0000 da0e 6174 7472  r....r0.....attr
+00000bb0: 6962 7574 6573 5f73 7263 da0e 6174 7472  ibutes_src..attr
+00000bc0: 6962 7574 6573 5f64 7374 7211 0000 0072  ibutes_dstr....r
+00000bd0: 1100 0000 7212 0000 00da 0e67 6974 5f61  ....r......git_a
+00000be0: 6e6e 6578 5f69 6e69 7454 0000 0073 2e00  nnex_initT...s..
+00000bf0: 0000 0805 0801 0a01 0a01 0801 0401 0803  ................
+00000c00: 0a01 0801 0401 1603 0a01 0801 0401 0804  ................
+00000c10: 0a01 0801 0401 1603 0401 0c01 0c01 0402  ................
+00000c20: 7a19 4769 7457 7261 7070 6572 2e67 6974  z.GitWrapper.git
+00000c30: 5f61 6e6e 6578 5f69 6e69 7463 0100 0000  _annex_initc....
+00000c40: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00000c50: 4300 0000 f30e 0000 007c 00a0 0067 0064  C........|...g.d
+00000c60: 01a2 01a1 0153 0029 024e 2904 da06 636f  .....S.).N)...co
+00000c70: 6d6d 6974 fa0d 2d2d 616c 6c6f 772d 656d  mmit..--allow-em
+00000c80: 7074 79fa 022d 6d7a 0f49 6e69 7469 616c  pty..-mz.Initial
+00000c90: 2063 6f6d 6d69 742e 7238 0000 00a9 0172   commit.r8.....r
+00000ca0: 0e00 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
+00000cb0: 0000 00da 0e69 6e69 7469 616c 5f63 6f6d  .....initial_com
+00000cc0: 6d69 747b 0000 0073 0200 0000 0e02 7a19  mit{...s......z.
+00000cd0: 4769 7457 7261 7070 6572 2e69 6e69 7469  GitWrapper.initi
+00000ce0: 616c 5f63 6f6d 6d69 7463 0300 0000 0000  al_commitc......
+00000cf0: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+00000d00: 0000 7372 0000 007c 0264 0075 0172 3767  ..sr...|.d.u.r7g
+00000d10: 007d 0374 007c 0164 0183 027d 047c 0444  .}.t.|.d...}.|.D
+00000d20: 005d 157d 0564 027c 0576 0072 1d7c 03a0  .].}.d.|.v.r.|..
+00000d30: 0164 037c 0217 0064 0417 00a1 0101 0071  .d.|...d.......q
+00000d40: 0d7c 03a0 017c 05a1 0101 0071 0d7c 04a0  .|...|.....q.|..
+00000d50: 02a1 0001 0074 007c 0164 0583 027d 047c  .....t.|.d...}.|
+00000d60: 04a0 037c 03a1 0101 007c 04a0 02a1 0001  ...|.....|......
+00000d70: 0064 0053 0064 0053 0029 064e da01 727a  .d.S.d.S.).N..rz
+00000d80: 0d61 6e6e 6578 2e62 6163 6b65 6e64 7a10  .annex.backendz.
+00000d90: 2a20 616e 6e65 782e 6261 636b 656e 643d  * annex.backend=
+00000da0: 7222 0000 00da 0177 2904 da04 6f70 656e  r".....w)...open
+00000db0: 723f 0000 00da 0563 6c6f 7365 da0a 7772  r?.....close..wr
+00000dc0: 6974 656c 696e 6573 2906 720e 0000 00da  itelines).r.....
+00000dd0: 0866 696c 656e 616d 6572 4600 0000 da05  .filenamerF.....
+00000de0: 6c69 6e65 73da 0466 696c 65da 046c 696e  lines..file..lin
+00000df0: 6572 1100 0000 7211 0000 0072 1200 0000  er....r....r....
+00000e00: 7244 0000 007f 0000 0073 1800 0000 0801  rD.......s......
+00000e10: 0401 0a01 0801 0801 1401 0c02 0801 0a01  ................
+00000e20: 0a01 0c01 04f5 7a23 4769 7457 7261 7070  ......z#GitWrapp
+00000e30: 6572 2e5f 6170 706c 795f 6769 745f 616e  er._apply_git_an
+00000e40: 6e65 785f 6261 636b 656e 6463 0200 0000  nex_backendc....
+00000e50: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000e60: 4300 0000 7328 0000 0064 0164 027c 0167  C...s(...d.d.|.g
+00000e70: 037d 027c 006a 0064 036b 0072 0f7c 02a0  .}.|.j.d.k.r.|..
+00000e80: 0164 04a1 0101 007c 00a0 027c 02a1 0153  .d.....|...|...S
+00000e90: 0029 054e 7220 0000 00da 0361 6464 723c  .).Nr .....addr<
+00000ea0: 0000 007a 122d 2d69 6e63 6c75 6465 2d64  ...z.--include-d
+00000eb0: 6f74 6669 6c65 7329 0372 2d00 0000 723f  otfiles).r-...r?
+00000ec0: 0000 0072 1e00 0000 2903 720e 0000 0072  ...r....).r....r
+00000ed0: 1800 0000 721c 0000 0072 1100 0000 7211  ....r....r....r.
+00000ee0: 0000 0072 1200 0000 da07 6769 745f 6164  ...r......git_ad
+00000ef0: 648d 0000 0073 0800 0000 0a02 0a01 0a01  d....s..........
+00000f00: 0a01 7a12 4769 7457 7261 7070 6572 2e67  ..z.GitWrapper.g
+00000f10: 6974 5f61 6464 6302 0000 0000 0000 0000  it_addc.........
+00000f20: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
+00000f30: 1200 0000 7c00 a000 6401 6402 6403 7c01  ....|...d.d.d.|.
+00000f40: 6704 a101 5300 2904 4e72 4b00 0000 724c  g...S.).NrK...rL
+00000f50: 0000 0072 4d00 0000 7238 0000 0029 0272  ...rM...r8...).r
+00000f60: 0e00 0000 da03 6d73 6772 1100 0000 7211  ......msgr....r.
+00000f70: 0000 0072 1200 0000 da0a 6769 745f 636f  ...r......git_co
+00000f80: 6d6d 6974 9400 0000 7302 0000 0012 017a  mmit....s......z
+00000f90: 1547 6974 5772 6170 7065 722e 6769 745f  .GitWrapper.git_
+00000fa0: 636f 6d6d 6974 6301 0000 0000 0000 0000  commitc.........
+00000fb0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
+00000fc0: 0e00 0000 7c00 a000 6401 6402 6702 a101  ....|...d.d.g...
+00000fd0: 5300 2903 4efa 0972 6576 2d70 6172 7365  S.).N..rev-parse
+00000fe0: 7a0f 2d2d 7368 6f77 2d74 6f70 6c65 7665  z.--show-topleve
+00000ff0: 6c72 3800 0000 724e 0000 0072 1100 0000  lr8...rN...r....
+00001000: 7211 0000 0072 1200 0000 da12 6769 745f  r....r......git_
+00001010: 746f 705f 6c65 7665 6c5f 7061 7468 9700  top_level_path..
+00001020: 0000 f302 0000 000e 017a 1d47 6974 5772  .........z.GitWr
+00001030: 6170 7065 722e 6769 745f 746f 705f 6c65  apper.git_top_le
+00001040: 7665 6c5f 7061 7468 6301 0000 0000 0000  vel_pathc.......
+00001050: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00001060: 0072 4a00 0000 2902 4e29 0372 5d00 0000  .rJ...).N).r]...
+00001070: 7a07 2d2d 7368 6f72 74da 0448 4541 4472  z.--short..HEADr
+00001080: 3800 0000 724e 0000 0072 1100 0000 7211  8...rN...r....r.
+00001090: 0000 0072 1200 0000 da0f 6769 745f 636f  ...r......git_co
+000010a0: 6d6d 6974 5f68 6173 689a 0000 0072 5f00  mmit_hash....r_.
+000010b0: 0000 7a1a 4769 7457 7261 7070 6572 2e67  ..z.GitWrapper.g
+000010c0: 6974 5f63 6f6d 6d69 745f 6861 7368 6301  it_commit_hashc.
+000010d0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000010e0: 0000 0043 0000 0072 4a00 0000 2902 4e29  ...C...rJ...).N)
+000010f0: 047a 076c 732d 7472 6565 7a0b 2d2d 6675  .z.ls-treez.--fu
+00001100: 6c6c 2d74 7265 657a 022d 7272 6000 0000  ll-treez.-rr`...
+00001110: 7238 0000 0072 4e00 0000 7211 0000 0072  r8...rN...r....r
+00001120: 1100 0000 7212 0000 00da 0b67 6974 5f6c  ....r......git_l
+00001130: 735f 7472 6565 9d00 0000 725f 0000 007a  s_tree....r_...z
+00001140: 1647 6974 5772 6170 7065 722e 6769 745f  .GitWrapper.git_
+00001150: 6c73 5f74 7265 6563 0300 0000 0000 0000  ls_treec........
+00001160: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00001170: 7324 0000 007c 0272 0b7c 006a 0064 017c  s$...|.r.|.j.d.|
+00001180: 0167 027c 0264 028d 0253 007c 00a0 0064  .g.|.d...S.|...d
+00001190: 017c 0167 02a1 0153 0029 034e da08 6368  .|.g...S.).N..ch
+000011a0: 6563 6b6f 7574 2901 721b 0000 0072 3800  eckout).r....r8.
+000011b0: 0000 2903 720e 0000 00da 0c70 6174 685f  ..).r......path_
+000011c0: 6f72 5f68 6173 6872 1b00 0000 7211 0000  or_hashr....r...
+000011d0: 0072 1100 0000 7212 0000 00da 0c67 6974  .r....r......git
+000011e0: 5f63 6865 636b 6f75 74a0 0000 0073 0600  _checkout....s..
+000011f0: 0000 0401 1201 0e01 7a17 4769 7457 7261  ........z.GitWra
+00001200: 7070 6572 2e67 6974 5f63 6865 636b 6f75  pper.git_checkou
+00001210: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
+00001220: 0000 0400 0000 4300 0000 730e 0000 007c  ......C...s....|
+00001230: 00a0 0064 017c 0167 02a1 0153 0029 024e  ...d.|.g...S.).N
+00001240: da05 7265 7365 7472 3800 0000 2902 720e  ..resetr8...).r.
+00001250: 0000 00da 0b63 6f6d 6d69 745f 6861 7368  .....commit_hash
+00001260: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00001270: 0c67 6974 5f72 6573 6574 5f74 6fa5 0000  .git_reset_to...
+00001280: 0072 5f00 0000 7a17 4769 7457 7261 7070  .r_...z.GitWrapp
+00001290: 6572 2e67 6974 5f72 6573 6574 5f74 6f63  er.git_reset_toc
+000012a0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+000012b0: 0800 0000 4300 0000 7360 0000 007c 00a0  ....C...s`...|..
+000012c0: 0064 017c 0167 02a1 017d 027c 026a 0164  .d.|.g...}.|.j.d
+000012d0: 026b 0272 2e74 0264 0364 0483 028f 137d  .k.r.t.d.d.....}
+000012e0: 037c 03a0 037c 01a1 0101 007c 03a0 0364  .|...|.....|...d
+000012f0: 05a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+00001300: 0064 0053 0031 0073 2777 0101 0001 0001  .d.S.1.s'w......
+00001310: 0059 0001 0064 0053 0064 0053 0029 064e  .Y...d.S.d.S.).N
+00001320: 7a0c 6368 6563 6b2d 6967 6e6f 7265 7202  z.check-ignorer.
+00001330: 0000 007a 112e 6769 742f 696e 666f 2f65  ...z..git/info/e
+00001340: 7863 6c75 6465 da01 6172 2200 0000 2904  xclude..ar"...).
+00001350: 721e 0000 00da 0a72 6574 7572 6e63 6f64  r......returncod
+00001360: 6572 5200 0000 da05 7772 6974 6529 0472  erR.....write).r
+00001370: 0e00 0000 7218 0000 0072 3000 0000 da09  ....r....r0.....
+00001380: 6769 7469 676e 6f72 6572 1100 0000 7211  gitignorer....r.
+00001390: 0000 0072 1200 0000 7235 0000 00a8 0000  ...r....r5......
+000013a0: 0073 0e00 0000 0e01 0a01 0c01 0a01 0c01  .s..............
+000013b0: 22fe 04ff 7a15 4769 7457 7261 7070 6572  "...z.GitWrapper
+000013c0: 2e67 6974 5f69 676e 6f72 6529 064e 4e4e  .git_ignore).NNN
+000013d0: 4e4e 4e29 0254 7214 0000 0072 0900 0000  NNN).Tr....r....
+000013e0: 2901 7214 0000 0029 14da 085f 5f6e 616d  ).r....)...__nam
+000013f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00001400: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
+00001410: 5f64 6f63 5f5f 7213 0000 0072 1e00 0000  _doc__r....r....
+00001420: 7233 0000 0072 3600 0000 7239 0000 0072  r3...r6...r9...r
+00001430: 4900 0000 724f 0000 0072 4400 0000 725a  I...rO...rD...rZ
+00001440: 0000 0072 5c00 0000 725e 0000 0072 6100  ...r\...r^...ra.
+00001450: 0000 7262 0000 0072 6500 0000 7268 0000  ..rb...re...rh..
+00001460: 0072 3500 0000 7211 0000 0072 1100 0000  .r5...r....r....
+00001470: 7211 0000 0072 1200 0000 7208 0000 0017  r....r....r.....
+00001480: 0000 0073 2800 0000 0800 0401 0202 0201  ...s(...........
+00001490: 0aff 0a07 080b 081c 0a06 0a06 0827 0804  .............'..
+000014a0: 080e 0807 0803 0803 0803 0a03 0805 0c03  ................
+000014b0: 7208 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000014c0: 0000 0000 0000 0300 0000 4000 0000 7334  ..........@...s4
+000014d0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+000014e0: 0264 0384 005a 0464 0c64 0564 0684 015a  .d...Z.d.d.d...Z
+000014f0: 0564 0764 0884 005a 0664 0c64 0964 0a84  .d.d...Z.d.d.d..
+00001500: 015a 0764 0b53 0029 0dda 0f47 6974 5265  .Z.d.S.)...GitRe
+00001510: 706f 4669 6c65 496e 666f 7a48 436c 6173  poFileInfozHClas
+00001520: 7320 7468 6174 2067 6174 6865 7273 2063  s that gathers c
+00001530: 6865 636b 7375 6d73 2061 6e64 2066 696c  hecksums and fil
+00001540: 6520 6c65 6e67 7468 7320 666f 7220 616c  e lengths for al
+00001550: 6c20 6669 6c65 7320 696e 2074 6865 2072  l files in the r
+00001560: 6570 6f2e 6302 0000 0000 0000 0000 0000  epo.c...........
+00001570: 0002 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00001580: 0000 7c01 7c00 5f00 6400 5300 7209 0000  ..|.|._.d.S.r...
+00001590: 0029 01da 0b67 6974 5f77 7261 7070 6572  .)...git_wrapper
+000015a0: 2902 720e 0000 0072 7200 0000 7211 0000  ).r....rr...r...
+000015b0: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+000015c0: b300 0000 7302 0000 000a 017a 1847 6974  ....s......z.Git
+000015d0: 5265 706f 4669 6c65 496e 666f 2e5f 5f69  RepoFileInfo.__i
+000015e0: 6e69 745f 5f46 6302 0000 0000 0000 0000  nit__Fc.........
+000015f0: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00001600: 1800 0000 7c00 a000 a100 7d02 7c00 a001  ....|.....}.|...
+00001610: 7c02 7c01 a102 7d03 7c03 5300 2901 6162  |.|...}.|.S.).ab
+00001620: 0100 0052 6574 7572 6e20 6120 6c69 7374  ...Return a list
+00001630: 206f 6620 6469 6374 7320 6465 7363 7269   of dicts descri
+00001640: 6269 6e67 2074 6865 2063 6f6e 7465 6e74  bing the content
+00001650: 7320 6f66 2074 6865 2072 6570 6f2e 0a20  s of the repo.. 
+00001660: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001670: 4120 6c69 7374 206f 6620 6469 6374 696f  A list of dictio
+00001680: 6e61 7269 6573 0a20 2020 2020 2020 2020  naries.         
+00001690: 207b 2763 7263 3332 273a 2063 6865 636b   {'crc32': check
+000016a0: 7375 6d2c 0a20 2020 2020 2020 2020 2020  sum,.           
+000016b0: 2763 6865 636b 7375 6d27 3a20 6368 6563  'checksum': chec
+000016c0: 6b73 756d 206f 7468 6572 2074 6861 6e20  ksum other than 
+000016d0: 6372 6333 320a 2020 2020 2020 2020 2020  crc32.          
+000016e0: 2027 6368 6563 6b73 756d 5479 7065 273a   'checksumType':
+000016f0: 2074 7970 6520 6f66 2063 6865 636b 7375   type of checksu
+00001700: 6d0a 2020 2020 2020 2020 2020 2027 6669  m.           'fi
+00001710: 6c65 4c65 6e67 7468 273a 2073 697a 6520  leLength': size 
+00001720: 6f66 2074 6865 2066 696c 652c 0a20 2020  of the file,.   
+00001730: 2020 2020 2020 2020 2770 6174 6827 3a20          'path': 
+00001740: 7061 7468 2072 656c 6174 6976 6520 746f  path relative to
+00001750: 2072 6570 6f20 726f 6f74 2e0a 2020 2020   repo root..    
+00001760: 2020 2020 2020 2027 6469 7265 6374 6f72         'director
+00001770: 7927 3a20 4661 6c73 650a 2020 2020 2020  y': False.      
+00001780: 2020 2020 7d29 02da 0966 696c 655f 6c69      })...file_li
+00001790: 7374 da05 636b 7375 6d29 0472 0e00 0000  st..cksum).r....
+000017a0: da1a 6769 745f 616e 6e65 785f 6861 7368  ..git_annex_hash
+000017b0: 5f61 735f 6368 6563 6b73 756d da05 6669  _as_checksum..fi
+000017c0: 6c65 7372 7400 0000 7211 0000 0072 1100  lesrt...r....r..
+000017d0: 0000 7212 0000 00da 0863 6f6e 7465 6e74  ..r......content
+000017e0: 73b6 0000 0073 0600 0000 080a 0c01 0401  s....s..........
+000017f0: 7a18 4769 7452 6570 6f46 696c 6549 6e66  z.GitRepoFileInf
+00001800: 6f2e 636f 6e74 656e 7473 6301 0000 0000  o.contentsc.....
+00001810: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
+00001820: 0000 0073 4200 0000 7c00 6a00 a001 a100  ...sB...|.j.....
+00001830: 7d01 7c01 a002 a100 7310 7403 7c01 6a04  }.|.....s.t.|.j.
+00001840: 8301 6401 6b02 7212 6700 5300 7c01 6a04  ..d.k.r.g.S.|.j.
+00001850: a005 6402 a101 7d02 6403 6404 8400 7c02  ..d...}.d.d...|.
+00001860: 4400 8301 7d03 7c03 5300 2905 4e72 0100  D...}.|.S.).Nr..
+00001870: 0000 7222 0000 0063 0100 0000 0000 0000  ..r"...c........
+00001880: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00001890: 731e 0000 0067 007c 005d 0b7d 017c 01a0  s....g.|.].}.|..
+000018a0: 0064 00a1 0164 0119 00a0 01a1 0091 0271  .d...d.........q
+000018b0: 0253 0029 02fa 0109 e9ff ffff ff29 0272  .S.).........).r
+000018c0: 2800 0000 722a 0000 0029 02da 022e 3072  (...r*...)....0r
+000018d0: 5800 0000 7211 0000 0072 1100 0000 7212  X...r....r....r.
+000018e0: 0000 00da 0a3c 6c69 7374 636f 6d70 3ec9  .....<listcomp>.
+000018f0: 0000 0073 0200 0000 1e00 7a2d 4769 7452  ...s......z-GitR
+00001900: 6570 6f46 696c 6549 6e66 6f2e 6669 6c65  epoFileInfo.file
+00001910: 5f6c 6973 742e 3c6c 6f63 616c 733e 2e3c  _list.<locals>.<
+00001920: 6c69 7374 636f 6d70 3e29 0672 7200 0000  listcomp>).rr...
+00001930: 7262 0000 0072 2500 0000 7229 0000 0072  rb...r%...r)...r
+00001940: 2700 0000 7228 0000 0029 0472 0e00 0000  '...r(...).r....
+00001950: da04 7472 6565 7256 0000 0072 7600 0000  ..treerV...rv...
+00001960: 7211 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
+00001970: 7300 0000 c400 0000 730c 0000 000a 0116  s.......s.......
+00001980: 0104 010c 010e 0104 017a 1947 6974 5265  .........z.GitRe
+00001990: 706f 4669 6c65 496e 666f 2e66 696c 655f  poFileInfo.file_
+000019a0: 6c69 7374 6303 0000 0000 0000 0000 0000  listc...........
+000019b0: 0007 0000 0004 0000 0043 0000 0073 5400  .........C...sT.
+000019c0: 0000 7c02 6401 6b02 720e 7400 7c00 6a01  ..|.d.k.r.t.|.j.
+000019d0: 6a02 7c00 6a01 6a03 8302 7d03 6e09 7404  j.|.j.j...}.n.t.
+000019e0: 7c00 6a01 6a02 7c00 6a01 6a03 8302 7d03  |.j.j.|.j.j...}.
+000019f0: 6700 7d04 7c01 4400 5d0c 7d05 7c03 a005  g.}.|.D.].}.|...
+00001a00: 7c05 a101 7d06 7c04 a006 7c06 a101 0100  |...}.|...|.....
+00001a10: 711b 7c04 5300 2902 4e46 2907 7203 0000  q.|.S.).NF).r...
+00001a20: 0072 7200 0000 720c 0000 0072 0d00 0000  .rr...r....r....
+00001a30: 7204 0000 00da 0c67 6574 5f63 6865 636b  r......get_check
+00001a40: 7375 6d72 3f00 0000 2907 720e 0000 0072  sumr?...).r....r
+00001a50: 7600 0000 7275 0000 00da 1263 6865 636b  v...ru.....check
+00001a60: 7375 6d5f 6765 6e65 7261 746f 72da 0963  sum_generator..c
+00001a70: 6865 636b 7375 6d73 7257 0000 00da 0863  hecksumsrW.....c
+00001a80: 6865 636b 7375 6d72 1100 0000 7211 0000  hecksumr....r...
+00001a90: 0072 1200 0000 7274 0000 00cc 0000 0073  .r....rt.......s
+00001aa0: 1800 0000 0802 0801 0601 06ff 0803 0601  ................
+00001ab0: 04ff 0403 0802 0a01 0c01 0402 7a15 4769  ............z.Gi
+00001ac0: 7452 6570 6f46 696c 6549 6e66 6f2e 636b  tRepoFileInfo.ck
+00001ad0: 7375 6d4e 2901 4629 0872 6d00 0000 726e  sumN).F).rm...rn
+00001ae0: 0000 0072 6f00 0000 7270 0000 0072 1300  ...ro...rp...r..
+00001af0: 0000 7277 0000 0072 7300 0000 7274 0000  ..rw...rs...rt..
+00001b00: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+00001b10: 7212 0000 0072 7100 0000 b000 0000 730c  r....rq.......s.
+00001b20: 0000 0008 0004 0108 020a 0308 0e0e 0872  ...............r
+00001b30: 7100 0000 290c 7217 0000 0072 4200 0000  q...).r....rB...
+00001b40: 7280 0000 0072 0300 0000 7204 0000 00da  r....r....r.....
+00001b50: 0575 7469 6c73 7205 0000 00da 1273 6372  .utilsr......scr
+00001b60: 6970 7473 2e63 6c69 636b 5f75 7469 6c72  ipts.click_utilr
+00001b70: 0700 0000 da06 6f62 6a65 6374 7208 0000  ......objectr...
+00001b80: 0072 7100 0000 7211 0000 0072 1100 0000  .rq...r....r....
+00001b90: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
+00001ba0: 756c 653e 0100 0000 7310 0000 0008 0e08  ule>....s.......
+00001bb0: 0110 020c 010c 0110 0300 7f14 1a         .............
```

### Comparing `obis-0.4.1/obis/dm/__pycache__/repository_utils.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/repository_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/__pycache__/utils.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Feb 27 10:08:42 2023 UTC, .py size: 3720 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a81 fc63 880e 0000  o.......*..c....
+00000000: 6f0d 0d0a 0000 0000 b669 2564 cd0e 0000  o........i%d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6506 8303  ..G.d.d...d.e...
@@ -47,150 +47,151 @@
 000002e0: 0000 720b 0000 0072 0d00 0000 4e29 0772  ..r....r....N).r
 000002f0: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
 00000300: 0000 00da 0347 4554 da03 5345 54da 0543  .....GET..SET..C
 00000310: 4c45 4152 7215 0000 0072 1500 0000 7215  LEARr....r....r.
 00000320: 0000 0072 1600 0000 7218 0000 001f 0000  ...r....r.......
 00000330: 0072 1700 0000 7218 0000 0054 6303 0000  .r....r....Tc...
 00000340: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-00000350: 0043 0000 0073 9000 0000 7c01 6a00 a001  .C...s....|.j...
+00000350: 0043 0000 0073 a000 0000 7c01 6a00 a001  .C...s....|.j...
 00000360: 7c02 a101 7d03 7c00 a002 6401 a101 6402  |...}.|...d...d.
 00000370: 7500 7213 7c03 6403 1900 7c00 6401 3c00  u.r.|.d...|.d.<.
 00000380: 7c00 a002 6404 a101 6402 7500 7220 7c03  |...d...d.u.r |.
 00000390: 6404 1900 7c00 6404 3c00 7c00 a002 6405  d...|.d.<.|...d.
 000003a0: a101 6402 7500 722b 6402 7c00 6405 3c00  ..d.u.r+d.|.d.<.
-000003b0: 7c00 a002 6406 a101 6402 7500 7236 6402  |...d...d.u.r6d.
-000003c0: 7c00 6406 3c00 7c00 a002 6407 a101 6402  |.d.<.|...d...d.
-000003d0: 7500 7246 7c03 6408 1900 0c00 7c00 6407  u.rF|.d.....|.d.
-000003e0: 3c00 6402 5300 6402 5300 2909 fa33 4164  <.d.S.d.S.)..3Ad
-000003f0: 6420 6465 6661 756c 7420 7661 6c75 6573  d default values
-00000400: 2066 6f72 2065 6d70 7479 2065 6e74 7269   for empty entri
-00000410: 6573 2069 6e20 7468 6520 636f 6e66 6967  es in the config
-00000420: 2eda 0375 726c 4eda 0b6f 7065 6e62 6973  ...urlN..openbis
-00000430: 5f75 726c da13 7665 7269 6679 5f63 6572  _url..verify_cer
-00000440: 7469 6669 6361 7465 73da 0574 6f6b 656e  tificates..token
-00000450: da0b 6973 5f70 6879 7369 6361 6cda 4a61  ..is_physical.Ja
-00000460: 6c6c 6f77 5f68 7474 705f 6275 745f 646f  llow_http_but_do
-00000470: 5f6e 6f74 5f75 7365 5f74 6869 735f 696e  _not_use_this_in
-00000480: 5f70 726f 6475 6374 696f 6e5f 616e 645f  _production_and_
-00000490: 6f6e 6c79 5f77 6974 6869 6e5f 7361 6665  only_within_safe
-000004a0: 5f6e 6574 776f 726b 73da 1061 6c6c 6f77  _networks..allow
-000004b0: 5f6f 6e6c 795f 6874 7470 7329 03da 0663  _only_https)...c
-000004c0: 6f6e 6669 67da 0b63 6f6e 6669 675f 6469  onfig..config_di
-000004d0: 6374 da03 6765 7429 0472 2400 0000 da08  ct..get).r$.....
-000004e0: 7265 736f 6c76 6572 da0a 6c6f 6361 6c5f  resolver..local_
-000004f0: 6f6e 6c79 7225 0000 0072 1500 0000 7215  onlyr%...r....r.
-00000500: 0000 0072 1600 0000 da17 636f 6d70 6c65  ...r......comple
-00000510: 7465 5f6f 7065 6e62 6973 5f63 6f6e 6669  te_openbis_confi
-00000520: 6726 0000 0073 2200 0000 0c02 0e01 0c01  g&...s".........
-00000530: 0e01 0c01 0e01 0801 0e01 0801 0401 0201  ................
-00000540: 02ff 0201 04ff 0603 0cff 04fe 7229 0000  ............r)..
-00000550: 0063 0100 0000 0000 0000 0000 0000 0400  .c..............
-00000560: 0000 0300 0000 4300 0000 735e 0000 007c  ......C...s^...|
-00000570: 00a0 0064 01a1 0164 0275 0172 0b7c 0064  ...d...d.u.r.|.d
-00000580: 0119 006e 0164 037d 017c 0172 2b74 0164  ...n.d.}.|.r+t.d
-00000590: 0483 017d 027c 02a0 02a1 0072 1c7c 026a  ...}.|.....r.|.j
-000005a0: 037c 0064 053c 0074 0164 0683 017d 037c  .|.d.<.t.d...}.|
-000005b0: 03a0 02a1 0072 2d7c 036a 037c 0064 073c  .....r-|.j.|.d.<
-000005c0: 0064 0253 0064 0253 0064 0253 0029 0872  .d.S.d.S.d.S.).r
-000005d0: 1c00 0000 da08 6669 6e64 5f67 6974 4e54  ......find_gitNT
-000005e0: da03 6769 74da 0867 6974 5f70 6174 687a  ..git..git_pathz
-000005f0: 0967 6974 2d61 6e6e 6578 da0e 6769 745f  .git-annex..git_
-00000600: 616e 6e65 785f 7061 7468 2904 7226 0000  annex_path).r&..
-00000610: 00da 0e6c 6f63 6174 655f 636f 6d6d 616e  ...locate_comman
-00000620: 64da 0773 7563 6365 7373 da06 6f75 7470  d..success..outp
-00000630: 7574 2904 7224 0000 0072 2a00 0000 da07  ut).r$...r*.....
-00000640: 6769 745f 636d 64da 0d67 6974 5f61 6e6e  git_cmd..git_ann
-00000650: 6578 5f63 6d64 7215 0000 0072 1500 0000  ex_cmdr....r....
-00000660: 7216 0000 00da 1363 6f6d 706c 6574 655f  r......complete_
-00000670: 6769 745f 636f 6e66 6967 3700 0000 7314  git_config7...s.
-00000680: 0000 001a 0304 0108 0108 010a 0108 0208  ................
-00000690: 010e 0104 f904 0672 3300 0000 6301 0000  .......r3...c...
-000006a0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-000006b0: 0043 0000 0073 2200 0000 7c00 a000 6401  .C...s"...|...d.
-000006c0: a101 6402 6b03 720f 7401 7c00 6403 1900  ..d.k.r.t.|.d...
-000006d0: 8301 0100 6400 5300 6400 5300 2904 4eda  ....d.S.d.S.).N.
-000006e0: 056c 6576 656c da05 4445 4255 47da 076d  .level..DEBUG..m
-000006f0: 6573 7361 6765 2902 7226 0000 00da 0570  essage).r&.....p
-00000700: 7269 6e74 2901 da07 6465 7461 696c 7372  rint)...detailsr
-00000710: 1500 0000 7215 0000 0072 1600 0000 da0c  ....r....r......
-00000720: 6465 6661 756c 745f 6563 686f 4500 0000  default_echoE...
-00000730: 7306 0000 000e 0110 0104 ff72 3900 0000  s..........r9...
-00000740: 4663 0400 0000 0000 0000 0000 0000 0500  Fc..............
-00000750: 0000 0700 0000 4300 0000 733a 0000 0074  ......C...s:...t
-00000760: 0074 016a 027c 0074 016a 0374 016a 037c  .t.j.|.t.j.t.j.|
-00000770: 0164 018d 047c 0264 028d 027d 047c 0364  .d...|.d...}.|.d
-00000780: 036b 0272 1b7c 04a0 04a1 0072 1b74 057c  .k.r.|.....r.t.|
-00000790: 0483 0182 017c 0453 0029 044e 2903 da06  .....|.S.).N)...
-000007a0: 7374 646f 7574 da06 7374 6465 7272 da05  stdout..stderr..
-000007b0: 7368 656c 6c29 01da 1873 7472 6970 5f6c  shell)...strip_l
-000007c0: 6561 6469 6e67 5f77 6869 7465 7370 6163  eading_whitespac
-000007d0: 6554 2906 7206 0000 00da 0a73 7562 7072  eT).r......subpr
-000007e0: 6f63 6573 73da 0372 756e da04 5049 5045  ocess..run..PIPE
-000007f0: da07 6661 696c 7572 6572 0700 0000 2905  ..failurer....).
-00000800: da04 6172 6773 723c 0000 0072 3d00 0000  ..argsr<...r=...
-00000810: da1a 7261 6973 655f 6578 6365 7074 696f  ..raise_exceptio
-00000820: 6e5f 6f6e 5f66 6169 6c75 7265 da06 7265  n_on_failure..re
-00000830: 7375 6c74 7215 0000 0072 1500 0000 7216  sultr....r....r.
-00000840: 0000 00da 0972 756e 5f73 6865 6c6c 4a00  .....run_shellJ.
-00000850: 0000 730e 0000 0002 0114 0102 0106 fe10  ..s.............
-00000860: 0308 0104 0172 4500 0000 6301 0000 0000  .....rE...c.....
-00000870: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-00000880: 0000 0073 3200 0000 7400 6401 a001 7c00  ...s2...t.d...|.
-00000890: a101 6701 6402 6403 8d02 7d01 7c01 a002  ..g.d.d...}.|...
-000008a0: a100 7217 7c01 6a03 a004 6404 a101 6405  ..r.|.j...d...d.
-000008b0: 1900 7c01 5f03 7c01 5300 2906 7a27 5265  ..|._.|.S.).z'Re
-000008c0: 7475 726e 2061 2074 7570 6c65 206f 6620  turn a tuple of 
-000008d0: 2872 6574 7572 6e63 6f64 652c 2073 7464  (returncode, std
-000008e0: 6f75 7429 2e7a 0774 7970 6520 7b7d 5429  out).z.type {}T)
-000008f0: 0172 3c00 0000 fa01 20e9 ffff ffff 2905  .r<..... .....).
-00000900: 7245 0000 00da 0666 6f72 6d61 7472 2f00  rE.....formatr/.
-00000910: 0000 7230 0000 00da 0573 706c 6974 2902  ..r0.....split).
-00000920: da07 636f 6d6d 616e 6472 4400 0000 7215  ..commandrD...r.
-00000930: 0000 0072 1500 0000 7216 0000 0072 2e00  ...r....r....r..
-00000940: 0000 5300 0000 7308 0000 0014 0308 0212  ..S...s.........
-00000950: 0104 0172 2e00 0000 6301 0000 0000 0000  ...r....c.......
-00000960: 0000 0000 0002 0000 0009 0000 0063 0000  .............c..
-00000970: 0073 4000 0000 8100 7400 a001 a100 7d01  .s@.....t.....}.
-00000980: 7400 a002 7400 6a03 a004 7c00 a101 a101  t...t.j...|.....
-00000990: 0100 7a0b 6401 5600 0100 5700 7400 a002  ..z.d.V...W.t...
-000009a0: 7c01 a101 0100 6401 5300 7400 a002 7c01  |.....d.S.t...|.
-000009b0: a101 0100 7700 2902 7a52 5361 6665 2063  ....w.).zRSafe c
-000009c0: 6420 2d2d 2072 6574 7572 6e20 746f 206f  d -- return to o
-000009d0: 7269 6769 6e61 6c20 6469 7220 6166 7465  riginal dir afte
-000009e0: 7220 6578 6563 7574 696f 6e2c 2065 7665  r execution, eve
-000009f0: 6e20 6966 2061 6e20 6578 6365 7074 696f  n if an exceptio
-00000a00: 6e20 6973 2072 6169 7365 642e 4e29 05da  n is raised.N)..
-00000a10: 026f 73da 0667 6574 6377 64da 0563 6864  .os..getcwd..chd
-00000a20: 6972 da04 7061 7468 da0a 6578 7061 6e64  ir..path..expand
-00000a30: 7573 6572 2902 da06 6e65 7764 6972 da07  user)...newdir..
-00000a40: 7072 6576 6469 7272 1500 0000 7215 0000  prevdirr....r...
-00000a50: 0072 1600 0000 da02 6364 5d00 0000 730c  .r......cd]...s.
-00000a60: 0000 0002 8008 0312 0102 0108 011a 0272  ...............r
-00000a70: 5200 0000 6301 0000 0000 0000 0000 0000  R...c...........
-00000a80: 0002 0000 0008 0000 0043 0000 0073 4e00  .........C...sN.
-00000a90: 0000 6401 7c00 7601 7206 6402 5300 7c00  ..d.|.v.r.d.S.|.
-00000aa0: a000 6401 a101 7d01 7a11 7401 a002 7c01  ..d...}.z.t...|.
-00000ab0: 6403 1900 6404 a102 0100 7403 7c01 6405  d...d.....t.|.d.
-00000ac0: 1900 8301 0100 5700 6406 5300 0400 7404  ......W.d.S...t.
-00000ad0: 7926 0100 0100 0100 5900 6402 5300 7700  y&......Y.d.S.w.
-00000ae0: 2907 4efa 012d 4672 0100 0000 7a0e 2559  ).N..-Fr....z.%Y
-00000af0: 256d 2564 2548 254d 2553 2566 7205 0000  %m%d%H%M%S%fr...
-00000b00: 0054 2905 7249 0000 0072 0300 0000 da08  .T).rI...r......
-00000b10: 7374 7270 7469 6d65 da03 696e 74da 0a56  strptime..int..V
-00000b20: 616c 7565 4572 726f 7229 02da 046e 616d  alueError)...nam
-00000b30: 6572 4900 0000 7215 0000 0072 1500 0000  erI...r....r....
-00000b40: 7216 0000 00da 1069 735f 7661 6c69 645f  r......is_valid_
-00000b50: 7065 726d 5f69 6468 0000 0073 1400 0000  perm_idh...s....
-00000b60: 0801 0401 0a01 0201 1001 0c01 0601 0c01  ................
-00000b70: 0601 02ff 7258 0000 0029 0154 2903 4654  ....rX...).T).FT
-00000b80: 4629 1372 4b00 0000 723e 0000 00da 0a63  F).rK...r>.....c
-00000b90: 6f6e 7465 7874 6c69 6272 0200 0000 7203  ontextlibr....r.
-00000ba0: 0000 00da 0465 6e75 6d72 0400 0000 da0e  .....enumr......
-00000bb0: 636f 6d6d 616e 645f 7265 7375 6c74 7206  command_resultr.
-00000bc0: 0000 0072 0700 0000 7209 0000 0072 1800  ...r....r....r..
-00000bd0: 0000 7229 0000 0072 3300 0000 7239 0000  ..r)...r3...r9..
-00000be0: 0072 4500 0000 722e 0000 0072 5200 0000  .rE...r....rR...
-00000bf0: 7258 0000 0072 1500 0000 7215 0000 0072  rX...r....r....r
-00000c00: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
-00000c10: 6c65 3e01 0000 0073 2000 0000 080e 0801  le>....s .......
-00000c20: 0c01 0c01 0c01 1002 1003 1007 0a07 0811  ................
-00000c30: 080e 0a05 0809 020a 0a01 0c0a            ............
+000003b0: 7c00 a002 6406 a101 6402 7500 723e 7c03  |...d...d.u.r>|.
+000003c0: 6406 1900 6402 7501 723e 7c03 6406 1900  d...d.u.r>|.d...
+000003d0: 7c00 6406 3c00 7c00 a002 6407 a101 6402  |.d.<.|...d...d.
+000003e0: 7500 724e 7c03 6408 1900 0c00 7c00 6407  u.rN|.d.....|.d.
+000003f0: 3c00 6402 5300 6402 5300 2909 fa33 4164  <.d.S.d.S.)..3Ad
+00000400: 6420 6465 6661 756c 7420 7661 6c75 6573  d default values
+00000410: 2066 6f72 2065 6d70 7479 2065 6e74 7269   for empty entri
+00000420: 6573 2069 6e20 7468 6520 636f 6e66 6967  es in the config
+00000430: 2eda 0375 726c 4eda 0b6f 7065 6e62 6973  ...urlN..openbis
+00000440: 5f75 726c da13 7665 7269 6679 5f63 6572  _url..verify_cer
+00000450: 7469 6669 6361 7465 73da 0574 6f6b 656e  tificates..token
+00000460: da0b 6973 5f70 6879 7369 6361 6cda 4a61  ..is_physical.Ja
+00000470: 6c6c 6f77 5f68 7474 705f 6275 745f 646f  llow_http_but_do
+00000480: 5f6e 6f74 5f75 7365 5f74 6869 735f 696e  _not_use_this_in
+00000490: 5f70 726f 6475 6374 696f 6e5f 616e 645f  _production_and_
+000004a0: 6f6e 6c79 5f77 6974 6869 6e5f 7361 6665  only_within_safe
+000004b0: 5f6e 6574 776f 726b 73da 1061 6c6c 6f77  _networks..allow
+000004c0: 5f6f 6e6c 795f 6874 7470 7329 03da 0663  _only_https)...c
+000004d0: 6f6e 6669 67da 0b63 6f6e 6669 675f 6469  onfig..config_di
+000004e0: 6374 da03 6765 7429 0472 2400 0000 da08  ct..get).r$.....
+000004f0: 7265 736f 6c76 6572 da0a 6c6f 6361 6c5f  resolver..local_
+00000500: 6f6e 6c79 7225 0000 0072 1500 0000 7215  onlyr%...r....r.
+00000510: 0000 0072 1600 0000 da17 636f 6d70 6c65  ...r......comple
+00000520: 7465 5f6f 7065 6e62 6973 5f63 6f6e 6669  te_openbis_confi
+00000530: 6726 0000 0073 2200 0000 0c02 0e01 0c01  g&...s".........
+00000540: 0e01 0c01 0e01 0801 1a01 0c01 0401 0201  ................
+00000550: 02ff 0201 04ff 0603 0cff 04fe 7229 0000  ............r)..
+00000560: 0063 0100 0000 0000 0000 0000 0000 0400  .c..............
+00000570: 0000 0300 0000 4300 0000 735e 0000 007c  ......C...s^...|
+00000580: 00a0 0064 01a1 0164 0275 0172 0b7c 0064  ...d...d.u.r.|.d
+00000590: 0119 006e 0164 037d 017c 0172 2b74 0164  ...n.d.}.|.r+t.d
+000005a0: 0483 017d 027c 02a0 02a1 0072 1c7c 026a  ...}.|.....r.|.j
+000005b0: 037c 0064 053c 0074 0164 0683 017d 037c  .|.d.<.t.d...}.|
+000005c0: 03a0 02a1 0072 2d7c 036a 037c 0064 073c  .....r-|.j.|.d.<
+000005d0: 0064 0253 0064 0253 0064 0253 0029 0872  .d.S.d.S.d.S.).r
+000005e0: 1c00 0000 da08 6669 6e64 5f67 6974 4e54  ......find_gitNT
+000005f0: da03 6769 74da 0867 6974 5f70 6174 687a  ..git..git_pathz
+00000600: 0967 6974 2d61 6e6e 6578 da0e 6769 745f  .git-annex..git_
+00000610: 616e 6e65 785f 7061 7468 2904 7226 0000  annex_path).r&..
+00000620: 00da 0e6c 6f63 6174 655f 636f 6d6d 616e  ...locate_comman
+00000630: 64da 0773 7563 6365 7373 da06 6f75 7470  d..success..outp
+00000640: 7574 2904 7224 0000 0072 2a00 0000 da07  ut).r$...r*.....
+00000650: 6769 745f 636d 64da 0d67 6974 5f61 6e6e  git_cmd..git_ann
+00000660: 6578 5f63 6d64 7215 0000 0072 1500 0000  ex_cmdr....r....
+00000670: 7216 0000 00da 1363 6f6d 706c 6574 655f  r......complete_
+00000680: 6769 745f 636f 6e66 6967 3700 0000 7314  git_config7...s.
+00000690: 0000 001a 0304 0108 0108 010a 0108 0208  ................
+000006a0: 010e 0104 f904 0672 3300 0000 6301 0000  .......r3...c...
+000006b0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000006c0: 0043 0000 0073 2200 0000 7c00 a000 6401  .C...s"...|...d.
+000006d0: a101 6402 6b03 720f 7401 7c00 6403 1900  ..d.k.r.t.|.d...
+000006e0: 8301 0100 6400 5300 6400 5300 2904 4eda  ....d.S.d.S.).N.
+000006f0: 056c 6576 656c da05 4445 4255 47da 076d  .level..DEBUG..m
+00000700: 6573 7361 6765 2902 7226 0000 00da 0570  essage).r&.....p
+00000710: 7269 6e74 2901 da07 6465 7461 696c 7372  rint)...detailsr
+00000720: 1500 0000 7215 0000 0072 1600 0000 da0c  ....r....r......
+00000730: 6465 6661 756c 745f 6563 686f 4500 0000  default_echoE...
+00000740: 7306 0000 000e 0110 0104 ff72 3900 0000  s..........r9...
+00000750: 4663 0400 0000 0000 0000 0000 0000 0500  Fc..............
+00000760: 0000 0700 0000 4300 0000 733a 0000 0074  ......C...s:...t
+00000770: 0074 016a 027c 0074 016a 0374 016a 037c  .t.j.|.t.j.t.j.|
+00000780: 0164 018d 047c 0264 028d 027d 047c 0364  .d...|.d...}.|.d
+00000790: 036b 0272 1b7c 04a0 04a1 0072 1b74 057c  .k.r.|.....r.t.|
+000007a0: 0483 0182 017c 0453 0029 044e 2903 da06  .....|.S.).N)...
+000007b0: 7374 646f 7574 da06 7374 6465 7272 da05  stdout..stderr..
+000007c0: 7368 656c 6c29 01da 1873 7472 6970 5f6c  shell)...strip_l
+000007d0: 6561 6469 6e67 5f77 6869 7465 7370 6163  eading_whitespac
+000007e0: 6554 2906 7206 0000 00da 0a73 7562 7072  eT).r......subpr
+000007f0: 6f63 6573 73da 0372 756e da04 5049 5045  ocess..run..PIPE
+00000800: da07 6661 696c 7572 6572 0700 0000 2905  ..failurer....).
+00000810: da04 6172 6773 723c 0000 0072 3d00 0000  ..argsr<...r=...
+00000820: da1a 7261 6973 655f 6578 6365 7074 696f  ..raise_exceptio
+00000830: 6e5f 6f6e 5f66 6169 6c75 7265 da06 7265  n_on_failure..re
+00000840: 7375 6c74 7215 0000 0072 1500 0000 7216  sultr....r....r.
+00000850: 0000 00da 0972 756e 5f73 6865 6c6c 4a00  .....run_shellJ.
+00000860: 0000 730e 0000 0002 0114 0102 0106 fe10  ..s.............
+00000870: 0308 0104 0172 4500 0000 6301 0000 0000  .....rE...c.....
+00000880: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000890: 0000 0073 3200 0000 7400 6401 a001 7c00  ...s2...t.d...|.
+000008a0: a101 6701 6402 6403 8d02 7d01 7c01 a002  ..g.d.d...}.|...
+000008b0: a100 7217 7c01 6a03 a004 6404 a101 6405  ..r.|.j...d...d.
+000008c0: 1900 7c01 5f03 7c01 5300 2906 7a27 5265  ..|._.|.S.).z'Re
+000008d0: 7475 726e 2061 2074 7570 6c65 206f 6620  turn a tuple of 
+000008e0: 2872 6574 7572 6e63 6f64 652c 2073 7464  (returncode, std
+000008f0: 6f75 7429 2e7a 0774 7970 6520 7b7d 5429  out).z.type {}T)
+00000900: 0172 3c00 0000 fa01 20e9 ffff ffff 2905  .r<..... .....).
+00000910: 7245 0000 00da 0666 6f72 6d61 7472 2f00  rE.....formatr/.
+00000920: 0000 7230 0000 00da 0573 706c 6974 2902  ..r0.....split).
+00000930: da07 636f 6d6d 616e 6472 4400 0000 7215  ..commandrD...r.
+00000940: 0000 0072 1500 0000 7216 0000 0072 2e00  ...r....r....r..
+00000950: 0000 5300 0000 7308 0000 0014 0308 0212  ..S...s.........
+00000960: 0104 0172 2e00 0000 6301 0000 0000 0000  ...r....c.......
+00000970: 0000 0000 0002 0000 0009 0000 0063 0000  .............c..
+00000980: 0073 4000 0000 8100 7400 a001 a100 7d01  .s@.....t.....}.
+00000990: 7400 a002 7400 6a03 a004 7c00 a101 a101  t...t.j...|.....
+000009a0: 0100 7a0b 6401 5600 0100 5700 7400 a002  ..z.d.V...W.t...
+000009b0: 7c01 a101 0100 6401 5300 7400 a002 7c01  |.....d.S.t...|.
+000009c0: a101 0100 7700 2902 7a52 5361 6665 2063  ....w.).zRSafe c
+000009d0: 6420 2d2d 2072 6574 7572 6e20 746f 206f  d -- return to o
+000009e0: 7269 6769 6e61 6c20 6469 7220 6166 7465  riginal dir afte
+000009f0: 7220 6578 6563 7574 696f 6e2c 2065 7665  r execution, eve
+00000a00: 6e20 6966 2061 6e20 6578 6365 7074 696f  n if an exceptio
+00000a10: 6e20 6973 2072 6169 7365 642e 4e29 05da  n is raised.N)..
+00000a20: 026f 73da 0667 6574 6377 64da 0563 6864  .os..getcwd..chd
+00000a30: 6972 da04 7061 7468 da0a 6578 7061 6e64  ir..path..expand
+00000a40: 7573 6572 2902 da06 6e65 7764 6972 da07  user)...newdir..
+00000a50: 7072 6576 6469 7272 1500 0000 7215 0000  prevdirr....r...
+00000a60: 0072 1600 0000 da02 6364 5d00 0000 730c  .r......cd]...s.
+00000a70: 0000 0002 8008 0312 0102 0108 011a 0272  ...............r
+00000a80: 5200 0000 6301 0000 0000 0000 0000 0000  R...c...........
+00000a90: 0002 0000 0008 0000 0043 0000 0073 4e00  .........C...sN.
+00000aa0: 0000 6401 7c00 7601 7206 6402 5300 7c00  ..d.|.v.r.d.S.|.
+00000ab0: a000 6401 a101 7d01 7a11 7401 a002 7c01  ..d...}.z.t...|.
+00000ac0: 6403 1900 6404 a102 0100 7403 7c01 6405  d...d.....t.|.d.
+00000ad0: 1900 8301 0100 5700 6406 5300 0400 7404  ......W.d.S...t.
+00000ae0: 7926 0100 0100 0100 5900 6402 5300 7700  y&......Y.d.S.w.
+00000af0: 2907 4efa 012d 4672 0100 0000 7a0e 2559  ).N..-Fr....z.%Y
+00000b00: 256d 2564 2548 254d 2553 2566 7205 0000  %m%d%H%M%S%fr...
+00000b10: 0054 2905 7249 0000 0072 0300 0000 da08  .T).rI...r......
+00000b20: 7374 7270 7469 6d65 da03 696e 74da 0a56  strptime..int..V
+00000b30: 616c 7565 4572 726f 7229 02da 046e 616d  alueError)...nam
+00000b40: 6572 4900 0000 7215 0000 0072 1500 0000  erI...r....r....
+00000b50: 7216 0000 00da 1069 735f 7661 6c69 645f  r......is_valid_
+00000b60: 7065 726d 5f69 6468 0000 0073 1400 0000  perm_idh...s....
+00000b70: 0801 0401 0a01 0201 1001 0c01 0601 0c01  ................
+00000b80: 0601 02ff 7258 0000 0029 0154 2903 4654  ....rX...).T).FT
+00000b90: 4629 1372 4b00 0000 723e 0000 00da 0a63  F).rK...r>.....c
+00000ba0: 6f6e 7465 7874 6c69 6272 0200 0000 7203  ontextlibr....r.
+00000bb0: 0000 00da 0465 6e75 6d72 0400 0000 da0e  .....enumr......
+00000bc0: 636f 6d6d 616e 645f 7265 7375 6c74 7206  command_resultr.
+00000bd0: 0000 0072 0700 0000 7209 0000 0072 1800  ...r....r....r..
+00000be0: 0000 7229 0000 0072 3300 0000 7239 0000  ..r)...r3...r9..
+00000bf0: 0072 4500 0000 722e 0000 0072 5200 0000  .rE...r....rR...
+00000c00: 7258 0000 0072 1500 0000 7215 0000 0072  rX...r....r....r
+00000c10: 1500 0000 7216 0000 00da 083c 6d6f 6475  ....r......<modu
+00000c20: 6c65 3e01 0000 0073 2000 0000 080e 0801  le>....s .......
+00000c30: 0c01 0c01 0c01 1002 1003 1007 0a07 0811  ................
+00000c40: 080e 0a05 0809 020a 0a01 0c0a            ............
```

### Comparing `obis-0.4.1/obis/dm/checksum.py` & `obis-0.4.2rc1/obis/dm/checksum.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/command_log.py` & `obis-0.4.2rc1/obis/dm/command_log.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/command_result.py` & `obis-0.4.2rc1/obis/dm/command_result.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__init__.py` & `obis-0.4.2rc1/obis/dm/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/addref.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/addref.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 1897 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 6907 0000  o..........ci...
+00000000: 6f0d 0d0a 0000 0000 014b 2464 6907 0000  o........K$di...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6404 6406 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6407 6408 8400 6408 6502 8303 5a08 6401  d.d...d.e...Z.d.
 00000070: 5300 2909 e900 0000 004e e901 0000 0029  S.)......N.....)
```

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/clone.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/clone.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/collection.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/download.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/download.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/move.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/move.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/object.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/object.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 29 13:49:21 2023 UTC, .py size: 12023 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e141 2464 f72e 0000  o........A$d....
+00000000: 6f0d 0d0a 0000 0000 9862 2564 672f 0000  o........b%dg/..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c08 6d09 5a09 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c08 6d0a 5a0a 0100 6402 6406 6c0b  d.l.m.Z...d.d.l.
@@ -340,344 +340,345 @@
 00001530: 0000 0072 5e00 0000 725f 0000 0072 0500  ...r^...r_...r..
 00001540: 0000 7226 0000 0072 1e00 0000 721e 0000  ..r&...r....r...
 00001550: 0072 1f00 0000 7262 0000 0096 0000 0073  .r....rb.......s
 00001560: 0200 0000 0c02 7a22 4f70 656e 6269 7343  ......z"OpenbisC
 00001570: 6f6d 6d61 6e64 2e63 6865 636b 5f63 6f6e  ommand.check_con
 00001580: 6669 6775 7261 7469 6f6e 6301 0000 0000  figurationc.....
 00001590: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
-000015a0: 0000 0073 fa00 0000 6401 7c00 6a00 a001  ...s....d.|.j...
-000015b0: a100 7600 721c 6402 7c00 6a00 6401 1900  ..v.r.d.|.j.d...
-000015c0: a001 a100 7600 721c 7c00 6a02 a003 7c00  ....v.r.|.j...|.
-000015d0: 6a00 6401 1900 6402 1900 6403 a102 0100  j.d...d...d.....
-000015e0: 0900 7c00 a004 a100 7d01 7c00 6a02 a005  ..|.....}.|.j...
-000015f0: a100 7241 7c00 6a02 6a06 a007 7c01 a101  ..rA|.j.j...|...
-00001600: 7336 7c00 6a02 6a06 a007 6404 7c01 1700  s6|.j.j...d.|...
-00001610: a101 723c 7408 6405 6406 6407 8d02 5300  ..r<t.d.d.d...S.
-00001620: 7c00 6a02 a009 a100 0100 7c00 6a0a 6a0b  |.j.......|.j.j.
-00001630: 6408 6b02 724d 7408 6409 640a 6407 8d02  d.k.rMt.d.d.d...
-00001640: 5300 740c a00c 640b a00d 7c01 a101 a101  S.t...d...|.....
-00001650: 7d02 7a0b 7c00 6a02 6a0b 7c01 7c02 6403  }.z.|.j.j.|.|.d.
-00001660: 640c 8d03 0100 5700 6e16 0400 740e 7976  d.....W.n...t.yv
-00001670: 0100 0100 0100 640d a00d 7c00 a00f a100  ......d...|.....
-00001680: a101 7d03 7408 6409 7c03 6407 8d02 0600  ..}.t.d.|.d.....
-00001690: 5900 5300 7700 7408 6405 6406 6407 8d02  Y.S.w.t.d.d.d...
-000016a0: 5300 290e 7a25 2052 6573 746f 7265 2073  S.).z% Restore s
-000016b0: 6573 7369 6f6e 2074 6f6b 656e 2069 6620  ession token if 
-000016c0: 6176 6169 6c61 626c 652e 2072 0300 0000  available. r....
-000016d0: 7257 0000 0054 7a05 2470 6174 2d72 0100  rW...Tz.$pat-r..
-000016e0: 0000 725e 0000 0072 5f00 0000 46e9 ffff  ..r^...r_...F...
-000016f0: ffff 7a12 4e6f 2061 6374 6976 6520 7365  ..z.No active se
-00001700: 7373 696f 6e2e 7a10 5061 7373 776f 7264  ssion.z.Password
-00001710: 2066 6f72 207b 7d3a 2901 da0a 7361 7665   for {}:)...save
-00001720: 5f74 6f6b 656e 7a1d 436f 756c 6420 6e6f  _tokenz.Could no
-00001730: 7420 6c6f 6720 696e 746f 206f 7065 6e62  t log into openb
-00001740: 6973 207b 7d29 1072 1300 0000 da04 6b65  is {}).r......ke
-00001750: 7973 7210 0000 00da 0973 6574 5f74 6f6b  ysr......set_tok
-00001760: 656e 7218 0000 00da 1169 735f 7365 7373  enr......is_sess
-00001770: 696f 6e5f 6163 7469 7665 720c 0000 00da  ion_activer.....
-00001780: 0a73 7461 7274 7377 6974 6872 0600 0000  .startswithr....
-00001790: da06 6c6f 676f 7574 720f 0000 0072 1900  ..logoutr....r..
-000017a0: 0000 da07 6765 7470 6173 73da 0666 6f72  ....getpass..for
-000017b0: 6d61 74da 0a56 616c 7565 4572 726f 7272  mat..ValueErrorr
-000017c0: 5400 0000 2904 721b 0000 0072 1800 0000  T...).r....r....
-000017d0: da06 7061 7373 7764 da03 6d73 6772 1e00  ..passwd..msgr..
-000017e0: 0000 721e 0000 0072 1f00 0000 7219 0000  ..r....r....r...
-000017f0: 009a 0000 0073 2600 0000 0e02 1201 1801  .....s&.........
-00001800: 0201 0802 0a01 2001 0c01 0a02 0c01 0c01  ...... .........
-00001810: 1001 0201 1601 0c01 0e01 1001 02fe 0c03  ................
-00001820: 7a14 4f70 656e 6269 7343 6f6d 6d61 6e64  z.OpenbisCommand
-00001830: 2e6c 6f67 696e 6301 0000 0000 0000 0000  .loginc.........
-00001840: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-00001850: 3e00 0000 7c00 a000 a100 7d01 7c01 a001  >...|.....}.|...
-00001860: a100 720a 7c01 5300 7c01 6a02 7d02 7c00  ..r.|.S.|.j.}.|.
-00001870: 6a03 6a04 a005 6401 7c02 6a06 6402 a103  j.j...d.|.j.d...
-00001880: 0100 7c00 a007 7c02 6a06 a101 0100 7c01  ..|...|.j.....|.
-00001890: 5300 2903 4e72 2400 0000 da05 6c6f 6361  S.).Nr$.....loca
-000018a0: 6c29 08da 2d67 6574 5f6f 725f 6372 6561  l)..-get_or_crea
-000018b0: 7465 5f65 7874 6572 6e61 6c5f 6461 7461  te_external_data
-000018c0: 5f6d 616e 6167 656d 656e 745f 7379 7374  _management_syst
-000018d0: 656d 721a 0000 0072 6100 0000 7212 0000  emr....ra...r...
-000018e0: 0072 2300 0000 da17 7365 745f 7661 6c75  .r#.....set_valu
-000018f0: 655f 666f 725f 7061 7261 6d65 7465 72da  e_for_parameter.
-00001900: 0463 6f64 6572 2b00 0000 2903 721b 0000  .coder+...).r...
-00001910: 0072 1d00 0000 da0c 6578 7465 726e 616c  .r......external
-00001920: 5f64 6d73 721e 0000 0072 1e00 0000 721f  _dmsr....r....r.
-00001930: 0000 00da 1470 7265 7061 7265 5f65 7874  .....prepare_ext
-00001940: 6572 6e61 6c5f 646d 73b1 0000 0073 1200  ernal_dms....s..
-00001950: 0000 0802 0801 0401 0601 0801 0801 04ff  ................
-00001960: 0c02 0401 7a23 4f70 656e 6269 7343 6f6d  ....z#OpenbisCom
-00001970: 6d61 6e64 2e70 7265 7061 7265 5f65 7874  mand.prepare_ext
-00001980: 6572 6e61 6c5f 646d 7363 0400 0000 0000  ernal_dmsc......
-00001990: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
-000019a0: 0000 732e 0000 0074 00a0 017c 03a0 0264  ..s....t...|...d
-000019b0: 01a1 01a1 01a0 03a1 0064 0264 0385 0219  .........d.d....
-000019c0: 007d 0464 04a0 047c 017c 027c 04a1 03a0  .}.d...|.|.|....
-000019d0: 05a1 0053 0029 054e 7a05 7574 662d 3872  ...S.).Nz.utf-8r
-000019e0: 0100 0000 e908 0000 007a 087b 7d2d 7b7d  .........z.{}-{}
-000019f0: 2d7b 7d29 06da 0768 6173 686c 6962 da04  -{})...hashlib..
-00001a00: 7368 6131 da06 656e 636f 6465 da09 6865  sha1..encode..he
-00001a10: 7864 6967 6573 7472 6d00 0000 da05 7570  xdigestrm.....up
-00001a20: 7065 7229 0572 1b00 0000 7218 0000 0072  per).r....r....r
-00001a30: 4b00 0000 da09 6564 6d73 5f70 6174 68da  K.....edms_path.
-00001a40: 0970 6174 685f 6861 7368 721e 0000 0072  .path_hashr....r
-00001a50: 1e00 0000 721f 0000 00da 2d67 656e 6572  ....r.....-gener
-00001a60: 6174 655f 6578 7465 726e 616c 5f64 6174  ate_external_dat
-00001a70: 615f 6d61 6e61 6765 6d65 6e74 5f73 7973  a_management_sys
-00001a80: 7465 6d5f 636f 6465 bc00 0000 7304 0000  tem_code....s...
-00001a90: 001c 0112 017a 3c4f 7065 6e62 6973 436f  .....z<OpenbisCo
-00001aa0: 6d6d 616e 642e 6765 6e65 7261 7465 5f65  mmand.generate_e
-00001ab0: 7874 6572 6e61 6c5f 6461 7461 5f6d 616e  xternal_data_man
-00001ac0: 6167 656d 656e 745f 7379 7374 656d 5f63  agement_system_c
-00001ad0: 6f64 6563 0100 0000 0000 0000 0000 0000  odec............
-00001ae0: 0900 0000 0d00 0000 4300 0000 73e0 0000  ........C...s...
-00001af0: 007c 00a0 00a1 007d 017c 00a0 01a1 007d  .|.....}.|.....}
-00001b00: 027c 00a0 02a1 007d 037c 006a 03a0 04a1  .|.....}.|.j....
-00001b10: 007d 047c 04a0 05a1 0072 177c 0453 0074  .}.|.....r.|.S.t
-00001b20: 066a 07a0 087c 046a 09a1 015c 027d 057d  .j...|.j...\.}.}
-00001b30: 067c 0164 0075 0072 2b7c 00a0 0a7c 027c  .|.d.u.r+|...|.|
-00001b40: 037c 05a1 037d 017a 0a7c 006a 0ba0 0c7c  .|...}.z.|.j...|
-00001b50: 01a0 0da1 00a1 017d 0757 006e 3404 0074  .......}.W.n4..t
-00001b60: 0e79 6901 0001 0001 007a 0e7c 006a 0ba0  .yi......z.|.j..
-00001b70: 0f7c 017c 0164 01a0 107c 037c 05a1 02a1  .|.|.d...|.|....
-00001b80: 037d 0757 006e 1c04 0074 1179 6601 007d  .}.W.n...t.yf..}
-00001b90: 0801 007a 1074 1264 0274 137c 0883 0164  ...z.t.d.t.|...d
-00001ba0: 038d 0257 0006 0059 0064 007d 087e 0806  ...W...Y.d.}.~..
-00001bb0: 0059 0053 0064 007d 087e 0877 0177 0059  .Y.S.d.}.~.w.w.Y
-00001bc0: 006e 0177 0074 1264 047c 0764 038d 0253  .n.w.t.d.|.d...S
-00001bd0: 0029 054e 7a06 7b7d 3a2f 7b7d 7265 0000  .).Nz.{}:/{}re..
-00001be0: 0072 5f00 0000 7201 0000 0029 1472 2400  .r_...r....).r$.
-00001bf0: 0000 7218 0000 00da 1264 6574 6572 6d69  ..r......determi
-00001c00: 6e65 5f68 6f73 746e 616d 6572 1100 0000  ne_hostnamer....
-00001c10: da12 6769 745f 746f 705f 6c65 7665 6c5f  ..git_top_level_
-00001c20: 7061 7468 721a 0000 00da 026f 73da 0470  pathr......os..p
-00001c30: 6174 68da 0573 706c 6974 7261 0000 0072  ath..splitra...r
-00001c40: 7f00 0000 7210 0000 00da 2367 6574 5f65  ....r.....#get_e
-00001c50: 7874 6572 6e61 6c5f 6461 7461 5f6d 616e  xternal_data_man
-00001c60: 6167 656d 656e 745f 7379 7374 656d 727c  agement_systemr|
-00001c70: 0000 0072 6e00 0000 da26 6372 6561 7465  ...rn....&create
-00001c80: 5f65 7874 6572 6e61 6c5f 6461 7461 5f6d  _external_data_m
-00001c90: 616e 6167 656d 656e 745f 7379 7374 656d  anagement_system
-00001ca0: 726d 0000 00da 0945 7863 6570 7469 6f6e  rm.....Exception
-00001cb0: 7206 0000 00da 0373 7472 2909 721b 0000  r......str).r...
-00001cc0: 0072 2400 0000 7218 0000 0072 4b00 0000  .r$...r....rK...
-00001cd0: 721d 0000 0072 7d00 0000 da09 7061 7468  r....r}.....path
-00001ce0: 5f6e 616d 6572 7500 0000 da05 6572 726f  _nameru.....erro
-00001cf0: 7272 1e00 0000 721e 0000 0072 1f00 0000  rr....r....r....
-00001d00: 7272 0000 00c0 0000 0073 3e00 0000 0801  rr.......s>.....
-00001d10: 0801 0801 0a01 0801 0401 1201 0801 0401  ................
-00001d20: 0601 04ff 0202 0601 0601 08ff 0c02 0202  ................
-00001d30: 0801 0201 0401 0201 0201 02fe 08fe 0e05  ................
-00001d40: 2001 0880 02ff 04fb 02fd 0c0a 7a3c 4f70   ...........z<Op
-00001d50: 656e 6269 7343 6f6d 6d61 6e64 2e67 6574  enbisCommand.get
-00001d60: 5f6f 725f 6372 6561 7465 5f65 7874 6572  _or_create_exter
-00001d70: 6e61 6c5f 6461 7461 5f6d 616e 6167 656d  nal_data_managem
-00001d80: 656e 745f 7379 7374 656d 6301 0000 0000  ent_systemc.....
-00001d90: 0000 0000 0000 0002 0000 0008 0000 0043  ...............C
-00001da0: 0000 0073 4000 0000 7c00 a000 a100 7d01  ...s@...|.....}.
-00001db0: 7c01 6401 7501 720a 7c01 5300 7c00 a001  |.d.u.r.|.S.|...
-00001dc0: 7402 a003 a100 a101 7d01 7c00 6a04 6a05  t.......}.|.j.j.
-00001dd0: 6402 6403 6404 7406 6a07 6405 7c01 6406  d.d.d.t.j.d.|.d.
-00001de0: 8d06 0100 7c01 5300 2907 7a7b 2052 6574  ....|.S.).z{ Ret
-00001df0: 7572 6e73 2067 6c6f 6261 6c6c 7920 6465  urns globally de
-00001e00: 6669 6e65 6420 686f 7374 6e61 6d65 2069  fined hostname i
-00001e10: 6620 6176 6169 6c61 626c 652e 0a20 2020  f available..   
-00001e20: 2020 2020 2020 2020 204f 7468 6572 7769           Otherwi
-00001e30: 6573 2c20 6c65 7473 2074 6865 2075 7365  es, lets the use
-00001e40: 7220 6368 6f6f 7365 206f 6e65 2061 6e64  r choose one and
-00001e50: 2073 746f 7265 7320 7468 6174 2067 6c6f   stores that glo
-00001e60: 6261 6c6c 792e 204e 7203 0000 0054 4672  bally. Nr....TFr
-00001e70: 4b00 0000 2902 da04 7072 6f70 722a 0000  K...)...propr*..
-00001e80: 0029 0872 4b00 0000 da10 6173 6b5f 666f  .).rK.....ask_fo
-00001e90: 725f 686f 7374 6e61 6d65 da06 736f 636b  r_hostname..sock
-00001ea0: 6574 da0b 6765 7468 6f73 746e 616d 6572  et..gethostnamer
-00001eb0: 0f00 0000 7203 0000 0072 0800 0000 da03  ....r....r......
-00001ec0: 5345 5429 0272 1b00 0000 724b 0000 0072  SET).r....rK...r
-00001ed0: 1e00 0000 721e 0000 0072 1f00 0000 7280  ....r....r....r.
-00001ee0: 0000 00da 0000 0073 0c00 0000 0804 0801  .......s........
-00001ef0: 0401 0e02 1a02 0401 7a21 4f70 656e 6269  ........z!Openbi
-00001f00: 7343 6f6d 6d61 6e64 2e64 6574 6572 6d69  sCommand.determi
-00001f10: 6e65 5f68 6f73 746e 616d 6563 0200 0000  ne_hostnamec....
-00001f20: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00001f30: 4300 0000 7320 0000 0074 0064 0174 017c  C...s ...t.d.t.|
-00001f40: 0183 0117 0064 0217 0083 017d 027c 0272  .....d.....}.|.r
-00001f50: 0e7c 0253 007c 0153 0029 037a 4920 4173  .|.S.|.S.).zI As
-00001f60: 6b73 2074 6865 2075 7365 7220 746f 2063  ks the user to c
-00001f70: 6f6e 6669 726d 2074 6865 2073 7567 6765  onfirm the sugge
-00001f80: 7374 6573 2068 6f73 746e 616d 6520 6f72  stes hostname or
-00001f90: 2063 686f 6f73 6520 6120 6375 7374 6f6d   choose a custom
-00001fa0: 206f 6e65 2e20 7a22 456e 7465 7220 686f   one. z"Enter ho
-00001fb0: 7374 6e61 6d65 2028 656d 7074 7920 746f  stname (empty to
-00001fc0: 2063 6f6e 6669 726d 2027 7a04 2729 3a20   confirm 'z.'): 
-00001fd0: 2902 da05 696e 7075 7472 8800 0000 2903  )...inputr....).
-00001fe0: 721b 0000 0072 4b00 0000 da0e 686f 7374  r....rK.....host
-00001ff0: 6e61 6d65 5f69 6e70 7574 721e 0000 0072  name_inputr....r
-00002000: 1e00 0000 721f 0000 0072 8c00 0000 e700  ....r....r......
-00002010: 0000 730c 0000 0002 020e 0104 ff04 0204  ..s.............
-00002020: 0104 027a 1f4f 7065 6e62 6973 436f 6d6d  ...z.OpenbisComm
-00002030: 616e 642e 6173 6b5f 666f 725f 686f 7374  and.ask_for_host
-00002040: 6e61 6d65 6301 0000 0000 0000 0000 0000  namec...........
-00002050: 0002 0000 0002 0000 0043 0000 0073 1c00  .........C...s..
-00002060: 0000 7c00 6a00 a001 a100 7d01 7c01 a002  ..|.j.....}.|...
-00002070: a100 720b 7c01 5300 7c01 6a03 5300 7259  ..r.|.S.|.j.S.rY
-00002080: 0000 0029 0472 1100 0000 7281 0000 0072  ...).r....r....r
-00002090: 1a00 0000 7261 0000 0072 6300 0000 721e  ....ra...rc...r.
-000020a0: 0000 0072 1e00 0000 721f 0000 0072 8300  ...r....r....r..
-000020b0: 0000 f000 0000 7308 0000 000a 0108 0104  ......s.........
-000020c0: 0106 017a 134f 7065 6e62 6973 436f 6d6d  ...z.OpenbisComm
-000020d0: 616e 642e 7061 7468 6302 0000 0000 0000  and.pathc.......
-000020e0: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
-000020f0: 0073 2200 0000 7400 a001 a100 7d02 6900  .s"...t.....}.i.
-00002100: 7d03 7402 7c03 7c02 6401 8303 0100 7c03  }.t.|.|.d.....|.
-00002110: 7c01 5f03 6402 5300 2903 7a29 0a20 2020  |._.d.S.).z).   
-00002120: 2020 2020 2055 7365 2067 6c6f 6261 6c20       Use global 
-00002130: 636f 6e66 6967 206f 6e6c 792e 0a20 2020  config only..   
-00002140: 2020 2020 2046 4e29 04da 0964 6d5f 636f       FN)...dm_co
-00002150: 6e66 6967 da10 5365 7474 696e 6773 5265  nfig..SettingsRe
-00002160: 736f 6c76 6572 7207 0000 0072 1400 0000  solverr....r....
-00002170: 2904 721b 0000 0072 1c00 0000 da08 7265  ).r....r......re
-00002180: 736f 6c76 6572 7203 0000 0072 1e00 0000  solverr....r....
-00002190: 721e 0000 0072 1f00 0000 da12 6c6f 6164  r....r......load
-000021a0: 5f67 6c6f 6261 6c5f 636f 6e66 6967 f600  _global_config..
-000021b0: 0000 7308 0000 0008 0404 010c 010a 017a  ..s............z
-000021c0: 214f 7065 6e62 6973 436f 6d6d 616e 642e  !OpenbisCommand.
-000021d0: 6c6f 6164 5f67 6c6f 6261 6c5f 636f 6e66  load_global_conf
-000021e0: 6967 4e29 2c72 5a00 0000 da0a 5f5f 6d6f  igN),rZ.....__mo
-000021f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00002200: 6d65 5f5f da07 5f5f 646f 635f 5f72 2000  me__..__doc__r .
-00002210: 0000 7224 0000 0072 2b00 0000 722f 0000  ..r$...r+...r/..
-00002220: 0072 3000 0000 7232 0000 0072 3300 0000  .r0...r2...r3...
-00002230: 7237 0000 0072 3800 0000 723b 0000 0072  r7...r8...r;...r
-00002240: 3c00 0000 723f 0000 0072 4100 0000 7242  <...r?...rA...rB
-00002250: 0000 0072 4500 0000 7246 0000 0072 4700  ...rE...rF...rG.
-00002260: 0000 7218 0000 0072 4900 0000 724b 0000  ..r....rI...rK..
-00002270: 0072 4c00 0000 724e 0000 0072 4f00 0000  .rL...rN...rO...
-00002280: 7251 0000 0072 5200 0000 7254 0000 0072  rQ...rR...rT...r
-00002290: 5500 0000 7257 0000 0072 5800 0000 725b  U...rW...rX...r[
-000022a0: 0000 0072 6400 0000 7262 0000 0072 1900  ...rd...rb...r..
-000022b0: 0000 7276 0000 0072 7f00 0000 7272 0000  ..rv...r....rr..
-000022c0: 0072 8000 0000 728c 0000 0072 8300 0000  .r....r....r....
-000022d0: 7295 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
-000022e0: 1e00 0000 721f 0000 0072 0900 0000 1c00  ....r....r......
-000022f0: 0000 7354 0000 0008 0004 0108 0308 1508  ..sT............
-00002300: 0308 0308 0308 0308 0308 0308 0308 0308  ................
-00002310: 0308 0308 0308 0308 0308 0308 0308 0308  ................
-00002320: 0308 0308 0308 0308 0308 0308 0308 0308  ................
-00002330: 0308 0308 0308 0308 0408 0908 0408 1708  ................
-00002340: 0b08 0408 1a08 0d08 090c 0672 0900 0000  ...........r....
-00002350: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002360: 0003 0000 0040 0000 0073 3200 0000 6500  .....@...s2...e.
-00002370: 5a01 6400 5a02 6401 5a03 640c 6404 6405  Z.d.Z.d.Z.d.d.d.
-00002380: 8401 5a04 6406 6407 8400 5a05 6408 6409  ..Z.d.d...Z.d.d.
-00002390: 8400 5a06 640a 640b 8400 5a07 6402 5300  ..Z.d.d...Z.d.S.
-000023a0: 290d da13 436f 6e74 656e 7443 6f70 7953  )...ContentCopyS
-000023b0: 656c 6563 746f 727a 7a20 496e 2063 6173  electorzz In cas
-000023c0: 6520 6120 636f 6d6d 616e 6420 6e65 6564  e a command need
-000023d0: 7320 696e 666f 726d 6174 696f 6e20 6672  s information fr
-000023e0: 6f6d 2061 2063 6f6e 7465 6e74 2063 6f70  om a content cop
-000023f0: 792c 2074 6869 7320 636c 6173 730a 2020  y, this class.  
-00002400: 2020 6173 6b73 2074 6865 2075 7365 7220    asks the user 
-00002410: 746f 2070 6963 6b20 6f6e 6520 6966 2074  to pick one if t
-00002420: 6865 7265 2061 7265 206d 756c 7469 706c  here are multipl
-00002430: 652e 204e 4663 0400 0000 0000 0000 0000  e. NFc..........
-00002440: 0000 0400 0000 0200 0000 4300 0000 7316  ..........C...s.
-00002450: 0000 007c 017c 005f 007c 027c 005f 017c  ...|.|._.|.|._.|
-00002460: 037c 005f 0264 0053 0072 5900 0000 2903  .|._.d.S.rY...).
-00002470: 7235 0000 00da 1263 6f6e 7465 6e74 5f63  r5.....content_c
-00002480: 6f70 795f 696e 6465 78da 0967 6574 5f69  opy_index..get_i
-00002490: 6e64 6578 2904 721b 0000 0072 3500 0000  ndex).r....r5...
-000024a0: 729a 0000 0072 9b00 0000 721e 0000 0072  r....r....r....r
-000024b0: 1e00 0000 721f 0000 0072 2000 0000 0401  ....r....r .....
-000024c0: 0000 7306 0000 0006 0106 010a 017a 1c43  ..s..........z.C
-000024d0: 6f6e 7465 6e74 436f 7079 5365 6c65 6374  ontentCopySelect
-000024e0: 6f72 2e5f 5f69 6e69 745f 5f63 0100 0000  or.__init__c....
-000024f0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00002500: 4300 0000 732a 0000 007c 00a0 00a1 007d  C...s*...|.....}
-00002510: 017c 006a 0164 016b 0272 0b7c 0153 007c  .|.j.d.k.r.|.S.|
-00002520: 006a 026a 0364 0219 0064 0319 007c 0119  .j.j.d...d...|..
-00002530: 0053 0029 044e 54da 0a6c 696e 6b65 6444  .S.).NT..linkedD
-00002540: 6174 61da 0d63 6f6e 7465 6e74 436f 7069  ata..contentCopi
-00002550: 6573 2904 da0c 7365 6c65 6374 5f69 6e64  es)...select_ind
-00002560: 6578 729b 0000 0072 3500 0000 da04 6461  exr....r5.....da
-00002570: 7461 2902 721b 0000 0072 9a00 0000 721e  ta).r....r....r.
-00002580: 0000 0072 1e00 0000 721f 0000 00da 0673  ...r....r......s
-00002590: 656c 6563 7409 0100 0073 0800 0000 0801  elect....s......
-000025a0: 0a01 0401 1402 7a1a 436f 6e74 656e 7443  ......z.ContentC
-000025b0: 6f70 7953 656c 6563 746f 722e 7365 6c65  opySelector.sele
-000025c0: 6374 6301 0000 0000 0000 0000 0000 0002  ctc.............
-000025d0: 0000 0004 0000 0043 0000 0073 6600 0000  .......C...sf...
-000025e0: 7c00 6a00 6a01 6401 1900 6402 6b03 7214  |.j.j.d...d.k.r.
-000025f0: 7402 6403 7c00 6a00 6a01 6401 1900 1700  t.d.|.j.j.d.....
-00002600: 6404 1700 8301 8201 7c00 6a00 6a01 6405  d.......|.j.j.d.
-00002610: 1900 6406 1900 7d01 7403 7c01 8301 6407  ..d...}.t.|...d.
-00002620: 6b02 7226 7402 6408 8301 8201 7403 7c01  k.r&t.d.....t.|.
-00002630: 8301 6409 6b02 722e 6407 5300 7c00 a004  ..d.k.r.d.S.|...
-00002640: 7c01 a101 5300 290a 4eda 046b 696e 64da  |...S.).N..kind.
-00002650: 044c 494e 4b7a 1444 6174 6120 7365 7420  .LINKz.Data set 
-00002660: 6973 206f 6620 7479 7065 207a 1420 6275  is of type z. bu
-00002670: 7420 7368 6f75 6c64 2062 6520 4c49 4e4b  t should be LINK
-00002680: 2e72 9c00 0000 729d 0000 0072 0100 0000  .r....r....r....
-00002690: 7a1f 4461 7461 2073 6574 2068 6173 206e  z.Data set has n
-000026a0: 6f20 636f 6e74 656e 7420 636f 7069 6573  o content copies
-000026b0: 2ee9 0100 0000 2905 7235 0000 0072 9f00  ......).r5...r..
-000026c0: 0000 726e 0000 00da 036c 656e da19 7365  ..rn.....len..se
-000026d0: 6c65 6374 5f63 6f6e 7465 6e74 5f63 6f70  lect_content_cop
-000026e0: 795f 696e 6465 7829 0272 1b00 0000 da0e  y_index).r......
-000026f0: 636f 6e74 656e 745f 636f 7069 6573 721e  content_copiesr.
-00002700: 0000 0072 1e00 0000 721f 0000 0072 9e00  ...r....r....r..
-00002710: 0000 1001 0000 7318 0000 0010 0104 010a  ......s.........
-00002720: 0102 ff02 0106 ff10 020c 0108 010c 0104  ................
-00002730: 010a 027a 2043 6f6e 7465 6e74 436f 7079  ...z ContentCopy
-00002740: 5365 6c65 6374 6f72 2e73 656c 6563 745f  Selector.select_
-00002750: 696e 6465 7863 0200 0000 0000 0000 0000  indexc..........
-00002760: 0000 0800 0000 0700 0000 4300 0000 73ae  ..........C...s.
-00002770: 0000 007c 006a 0064 0075 0172 187c 006a  ...|.j.d.u.r.|.j
-00002780: 0064 016b 0572 147c 006a 0074 017c 0183  .d.k.r.|.j.t.|..
-00002790: 016b 0072 147c 006a 0053 0074 0264 0283  .k.r.|.j.S.t.d..
-000027a0: 0182 0109 0074 0364 0483 0101 0074 047c  .....t.d.....t.|
-000027b0: 0183 0144 005d 1c5c 027d 027d 037c 0364  ...D.].\.}.}.|.d
-000027c0: 0519 0064 0619 00a0 0564 07a1 0164 0119  ...d.....d...d..
-000027d0: 007d 047c 0364 0819 007d 0574 0364 09a0  .}.|.d...}.t.d..
-000027e0: 067c 027c 047c 05a1 0383 0101 0071 2174  .|.|.|.......q!t
-000027f0: 0764 0a83 017d 067c 06a0 08a1 0072 5674  .d...}.|.....rVt
-00002800: 097c 0683 017d 077c 0764 016b 0572 567c  .|...}.|.d.k.rV|
-00002810: 0774 017c 0183 016b 0072 567c 0753 0071  .t.|...k.rV|.S.q
-00002820: 1929 0b4e 7201 0000 007a 1b49 6e76 616c  .).Nr....z.Inval
-00002830: 6964 2063 6f6e 7465 6e74 2063 6f70 7920  id content copy 
-00002840: 696e 6465 782e 547a 2f46 726f 6d20 7768  index.Tz/From wh
-00002850: 6963 6820 6c6f 6361 7469 6f6e 2073 686f  ich location sho
-00002860: 756c 6420 7468 6520 6669 6c65 7320 6265  uld the files be
-00002870: 2063 6f70 6965 643f da0b 6578 7465 726e   copied?..extern
-00002880: 616c 446d 73da 0761 6464 7265 7373 fa01  alDms..address..
-00002890: 3a72 8300 0000 7a0b 2020 7b7d 2920 7b7d  :r....z.  {}) {}
-000028a0: 3a7b 7d7a 023e 2029 0a72 9a00 0000 72a4  :{}z.> ).r....r.
-000028b0: 0000 0072 6e00 0000 da05 7072 696e 74da  ...rn.....print.
-000028c0: 0965 6e75 6d65 7261 7465 7284 0000 0072  .enumerater....r
-000028d0: 6d00 0000 7290 0000 00da 0769 7364 6967  m...r......isdig
-000028e0: 6974 da03 696e 7429 0872 1b00 0000 72a6  it..int).r....r.
-000028f0: 0000 00da 0169 da0c 636f 6e74 656e 745f  .....i..content_
-00002900: 636f 7079 da04 686f 7374 7283 0000 00da  copy..hostr.....
-00002910: 1163 6f70 795f 696e 6465 785f 7374 7269  .copy_index_stri
-00002920: 6e67 da0e 636f 7079 5f69 6e64 6578 5f69  ng..copy_index_i
-00002930: 6e74 721e 0000 0072 1e00 0000 721f 0000  ntr....r....r...
-00002940: 0072 a500 0000 1c01 0000 7320 0000 000a  .r........s ....
-00002950: 0118 0206 0108 0202 0308 0110 0116 0108  ................
-00002960: 0114 0108 0208 0108 0114 0104 0102 f57a  ...............z
-00002970: 2d43 6f6e 7465 6e74 436f 7079 5365 6c65  -ContentCopySele
-00002980: 6374 6f72 2e73 656c 6563 745f 636f 6e74  ctor.select_cont
-00002990: 656e 745f 636f 7079 5f69 6e64 6578 2902  ent_copy_index).
-000029a0: 4e46 2908 725a 0000 0072 9600 0000 7297  NF).rZ...r....r.
-000029b0: 0000 0072 9800 0000 7220 0000 0072 a000  ...r....r ...r..
-000029c0: 0000 729e 0000 0072 a500 0000 721e 0000  ..r....r....r...
-000029d0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000029e0: 7299 0000 0000 0100 0073 0c00 0000 0800  r........s......
-000029f0: 0401 0a03 0805 0807 0c0c 7299 0000 0029  ..........r....)
-00002a00: 1172 6c00 0000 7278 0000 0072 8200 0000  .rl...rx...r....
-00002a10: 728d 0000 0072 1600 0000 725e 0000 0072  r....r....r^...r
-00002a20: 0300 0000 7292 0000 00da 0e63 6f6d 6d61  ....r......comma
-00002a30: 6e64 5f72 6573 756c 7472 0400 0000 7206  nd_resultr....r.
-00002a40: 0000 00da 0575 7469 6c73 7207 0000 0072  .....utilsr....r
-00002a50: 0800 0000 723e 0000 0072 0900 0000 7299  ....r>...r....r.
-00002a60: 0000 0072 1e00 0000 721e 0000 0072 1e00  ...r....r....r..
-00002a70: 0000 721f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00002a80: 3e01 0000 0073 1800 0000 080e 0801 0801  >....s..........
-00002a90: 0801 0802 0c02 0c01 0c01 1001 1003 007f  ................
-00002aa0: 1465                                     .e
+000015a0: 0000 0073 0c01 0000 6401 7c00 6a00 a001  ...s....d.|.j...
+000015b0: a100 7600 7225 6402 7c00 6a00 6401 1900  ..v.r%d.|.j.d...
+000015c0: a001 a100 7600 7225 7c00 6a00 6401 1900  ....v.r%|.j.d...
+000015d0: 6402 1900 6403 7501 7225 7c00 6a02 a003  d...d.u.r%|.j...
+000015e0: 7c00 6a00 6401 1900 6402 1900 6404 a102  |.j.d...d...d...
+000015f0: 0100 0900 7c00 a004 a100 7d01 7c00 6a02  ....|.....}.|.j.
+00001600: a005 a100 724a 7c00 6a02 6a06 a007 7c01  ....rJ|.j.j...|.
+00001610: a101 733f 7c00 6a02 6a06 a007 6405 7c01  ..s?|.j.j...d.|.
+00001620: 1700 a101 7245 7408 6406 6407 6408 8d02  ....rEt.d.d.d...
+00001630: 5300 7c00 6a02 a009 a100 0100 7c00 6a0a  S.|.j.......|.j.
+00001640: 6a0b 6409 6b02 7256 7408 640a 640b 6408  j.d.k.rVt.d.d.d.
+00001650: 8d02 5300 740c a00c 640c a00d 7c01 a101  ..S.t...d...|...
+00001660: a101 7d02 7a0b 7c00 6a02 6a0b 7c01 7c02  ..}.z.|.j.j.|.|.
+00001670: 6404 640d 8d03 0100 5700 6e16 0400 740e  d.d.....W.n...t.
+00001680: 797f 0100 0100 0100 640e a00d 7c00 a00f  y.......d...|...
+00001690: a100 a101 7d03 7408 640a 7c03 6408 8d02  ....}.t.d.|.d...
+000016a0: 0600 5900 5300 7700 7408 6406 6407 6408  ..Y.S.w.t.d.d.d.
+000016b0: 8d02 5300 290f 7a25 2052 6573 746f 7265  ..S.).z% Restore
+000016c0: 2073 6573 7369 6f6e 2074 6f6b 656e 2069   session token i
+000016d0: 6620 6176 6169 6c61 626c 652e 2072 0300  f available. r..
+000016e0: 0000 7257 0000 004e 547a 0524 7061 742d  ..rW...NTz.$pat-
+000016f0: 7201 0000 0072 5e00 0000 725f 0000 0046  r....r^...r_...F
+00001700: e9ff ffff ff7a 124e 6f20 6163 7469 7665  .....z.No active
+00001710: 2073 6573 7369 6f6e 2e7a 1050 6173 7377   session.z.Passw
+00001720: 6f72 6420 666f 7220 7b7d 3a29 01da 0a73  ord for {}:)...s
+00001730: 6176 655f 746f 6b65 6e7a 1d43 6f75 6c64  ave_tokenz.Could
+00001740: 206e 6f74 206c 6f67 2069 6e74 6f20 6f70   not log into op
+00001750: 656e 6269 7320 7b7d 2910 7213 0000 00da  enbis {}).r.....
+00001760: 046b 6579 7372 1000 0000 da09 7365 745f  .keysr......set_
+00001770: 746f 6b65 6e72 1800 0000 da11 6973 5f73  tokenr......is_s
+00001780: 6573 7369 6f6e 5f61 6374 6976 6572 0c00  ession_activer..
+00001790: 0000 da0a 7374 6172 7473 7769 7468 7206  ....startswithr.
+000017a0: 0000 00da 066c 6f67 6f75 7472 0f00 0000  .....logoutr....
+000017b0: 7219 0000 00da 0767 6574 7061 7373 da06  r......getpass..
+000017c0: 666f 726d 6174 da0a 5661 6c75 6545 7272  format..ValueErr
+000017d0: 6f72 7254 0000 0029 0472 1b00 0000 7218  orrT...).r....r.
+000017e0: 0000 00da 0670 6173 7377 64da 036d 7367  .....passwd..msg
+000017f0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00001800: 1900 0000 9a00 0000 732a 0000 000e 0212  ........s*......
+00001810: 0110 0102 ff18 0202 0108 020a 0120 010c  ............. ..
+00001820: 010a 020c 010c 0110 0102 0116 010c 010e  ................
+00001830: 0110 0102 fe0c 037a 144f 7065 6e62 6973  .......z.Openbis
+00001840: 436f 6d6d 616e 642e 6c6f 6769 6e63 0100  Command.loginc..
+00001850: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00001860: 0000 4300 0000 733e 0000 007c 00a0 00a1  ..C...s>...|....
+00001870: 007d 017c 01a0 01a1 0072 0a7c 0153 007c  .}.|.....r.|.S.|
+00001880: 016a 027d 027c 006a 036a 04a0 0564 017c  .j.}.|.j.j...d.|
+00001890: 026a 0664 02a1 0301 007c 00a0 077c 026a  .j.d.....|...|.j
+000018a0: 06a1 0101 007c 0153 0029 034e 7224 0000  .....|.S.).Nr$..
+000018b0: 00da 056c 6f63 616c 2908 da2d 6765 745f  ...local)..-get_
+000018c0: 6f72 5f63 7265 6174 655f 6578 7465 726e  or_create_extern
+000018d0: 616c 5f64 6174 615f 6d61 6e61 6765 6d65  al_data_manageme
+000018e0: 6e74 5f73 7973 7465 6d72 1a00 0000 7261  nt_systemr....ra
+000018f0: 0000 0072 1200 0000 7223 0000 00da 1773  ...r....r#.....s
+00001900: 6574 5f76 616c 7565 5f66 6f72 5f70 6172  et_value_for_par
+00001910: 616d 6574 6572 da04 636f 6465 722b 0000  ameter..coder+..
+00001920: 0029 0372 1b00 0000 721d 0000 00da 0c65  .).r....r......e
+00001930: 7874 6572 6e61 6c5f 646d 7372 1e00 0000  xternal_dmsr....
+00001940: 721e 0000 0072 1f00 0000 da14 7072 6570  r....r......prep
+00001950: 6172 655f 6578 7465 726e 616c 5f64 6d73  are_external_dms
+00001960: b200 0000 7312 0000 0008 0208 0104 0106  ....s...........
+00001970: 0108 0108 0104 ff0c 0204 017a 234f 7065  ...........z#Ope
+00001980: 6e62 6973 436f 6d6d 616e 642e 7072 6570  nbisCommand.prep
+00001990: 6172 655f 6578 7465 726e 616c 5f64 6d73  are_external_dms
+000019a0: 6304 0000 0000 0000 0000 0000 0005 0000  c...............
+000019b0: 0005 0000 0043 0000 0073 2e00 0000 7400  .....C...s....t.
+000019c0: a001 7c03 a002 6401 a101 a101 a003 a100  ..|...d.........
+000019d0: 6402 6403 8502 1900 7d04 6404 a004 7c01  d.d.....}.d...|.
+000019e0: 7c02 7c04 a103 a005 a100 5300 2905 4e7a  |.|.......S.).Nz
+000019f0: 0575 7466 2d38 7201 0000 00e9 0800 0000  .utf-8r.........
+00001a00: 7a08 7b7d 2d7b 7d2d 7b7d 2906 da07 6861  z.{}-{}-{})...ha
+00001a10: 7368 6c69 62da 0473 6861 31da 0665 6e63  shlib..sha1..enc
+00001a20: 6f64 65da 0968 6578 6469 6765 7374 726d  ode..hexdigestrm
+00001a30: 0000 00da 0575 7070 6572 2905 721b 0000  .....upper).r...
+00001a40: 0072 1800 0000 724b 0000 00da 0965 646d  .r....rK.....edm
+00001a50: 735f 7061 7468 da09 7061 7468 5f68 6173  s_path..path_has
+00001a60: 6872 1e00 0000 721e 0000 0072 1f00 0000  hr....r....r....
+00001a70: da2d 6765 6e65 7261 7465 5f65 7874 6572  .-generate_exter
+00001a80: 6e61 6c5f 6461 7461 5f6d 616e 6167 656d  nal_data_managem
+00001a90: 656e 745f 7379 7374 656d 5f63 6f64 65bd  ent_system_code.
+00001aa0: 0000 0073 0400 0000 1c01 1201 7a3c 4f70  ...s........z<Op
+00001ab0: 656e 6269 7343 6f6d 6d61 6e64 2e67 656e  enbisCommand.gen
+00001ac0: 6572 6174 655f 6578 7465 726e 616c 5f64  erate_external_d
+00001ad0: 6174 615f 6d61 6e61 6765 6d65 6e74 5f73  ata_management_s
+00001ae0: 7973 7465 6d5f 636f 6465 6301 0000 0000  ystem_codec.....
+00001af0: 0000 0000 0000 0009 0000 000d 0000 0043  ...............C
+00001b00: 0000 0073 e000 0000 7c00 a000 a100 7d01  ...s....|.....}.
+00001b10: 7c00 a001 a100 7d02 7c00 a002 a100 7d03  |.....}.|.....}.
+00001b20: 7c00 6a03 a004 a100 7d04 7c04 a005 a100  |.j.....}.|.....
+00001b30: 7217 7c04 5300 7406 6a07 a008 7c04 6a09  r.|.S.t.j...|.j.
+00001b40: a101 5c02 7d05 7d06 7c01 6400 7500 722b  ..\.}.}.|.d.u.r+
+00001b50: 7c00 a00a 7c02 7c03 7c05 a103 7d01 7a0a  |...|.|.|...}.z.
+00001b60: 7c00 6a0b a00c 7c01 a00d a100 a101 7d07  |.j...|.......}.
+00001b70: 5700 6e34 0400 740e 7969 0100 0100 0100  W.n4..t.yi......
+00001b80: 7a0e 7c00 6a0b a00f 7c01 7c01 6401 a010  z.|.j...|.|.d...
+00001b90: 7c03 7c05 a102 a103 7d07 5700 6e1c 0400  |.|.....}.W.n...
+00001ba0: 7411 7966 0100 7d08 0100 7a10 7412 6402  t.yf..}...z.t.d.
+00001bb0: 7413 7c08 8301 6403 8d02 5700 0600 5900  t.|...d...W...Y.
+00001bc0: 6400 7d08 7e08 0600 5900 5300 6400 7d08  d.}.~...Y.S.d.}.
+00001bd0: 7e08 7701 7700 5900 6e01 7700 7412 6404  ~.w.w.Y.n.w.t.d.
+00001be0: 7c07 6403 8d02 5300 2905 4e7a 067b 7d3a  |.d...S.).Nz.{}:
+00001bf0: 2f7b 7d72 6500 0000 725f 0000 0072 0100  /{}re...r_...r..
+00001c00: 0000 2914 7224 0000 0072 1800 0000 da12  ..).r$...r......
+00001c10: 6465 7465 726d 696e 655f 686f 7374 6e61  determine_hostna
+00001c20: 6d65 7211 0000 00da 1267 6974 5f74 6f70  mer......git_top
+00001c30: 5f6c 6576 656c 5f70 6174 6872 1a00 0000  _level_pathr....
+00001c40: da02 6f73 da04 7061 7468 da05 7370 6c69  ..os..path..spli
+00001c50: 7472 6100 0000 727f 0000 0072 1000 0000  tra...r....r....
+00001c60: da23 6765 745f 6578 7465 726e 616c 5f64  .#get_external_d
+00001c70: 6174 615f 6d61 6e61 6765 6d65 6e74 5f73  ata_management_s
+00001c80: 7973 7465 6d72 7c00 0000 726e 0000 00da  ystemr|...rn....
+00001c90: 2663 7265 6174 655f 6578 7465 726e 616c  &create_external
+00001ca0: 5f64 6174 615f 6d61 6e61 6765 6d65 6e74  _data_management
+00001cb0: 5f73 7973 7465 6d72 6d00 0000 da09 4578  _systemrm.....Ex
+00001cc0: 6365 7074 696f 6e72 0600 0000 da03 7374  ceptionr......st
+00001cd0: 7229 0972 1b00 0000 7224 0000 0072 1800  r).r....r$...r..
+00001ce0: 0000 724b 0000 0072 1d00 0000 727d 0000  ..rK...r....r}..
+00001cf0: 00da 0970 6174 685f 6e61 6d65 7275 0000  ...path_nameru..
+00001d00: 00da 0565 7272 6f72 721e 0000 0072 1e00  ...errorr....r..
+00001d10: 0000 721f 0000 0072 7200 0000 c100 0000  ..r....rr.......
+00001d20: 733e 0000 0008 0108 0108 010a 0108 0104  s>..............
+00001d30: 0112 0108 0104 0106 0104 ff02 0206 0106  ................
+00001d40: 0108 ff0c 0202 0208 0102 0104 0102 0102  ................
+00001d50: 0102 fe08 fe0e 0520 0108 8002 ff04 fb02  ....... ........
+00001d60: fd0c 0a7a 3c4f 7065 6e62 6973 436f 6d6d  ...z<OpenbisComm
+00001d70: 616e 642e 6765 745f 6f72 5f63 7265 6174  and.get_or_creat
+00001d80: 655f 6578 7465 726e 616c 5f64 6174 615f  e_external_data_
+00001d90: 6d61 6e61 6765 6d65 6e74 5f73 7973 7465  management_syste
+00001da0: 6d63 0100 0000 0000 0000 0000 0000 0200  mc..............
+00001db0: 0000 0800 0000 4300 0000 7340 0000 007c  ......C...s@...|
+00001dc0: 00a0 00a1 007d 017c 0164 0175 0172 0a7c  .....}.|.d.u.r.|
+00001dd0: 0153 007c 00a0 0174 02a0 03a1 00a1 017d  .S.|...t.......}
+00001de0: 017c 006a 046a 0564 0264 0364 0474 066a  .|.j.j.d.d.d.t.j
+00001df0: 0764 057c 0164 068d 0601 007c 0153 0029  .d.|.d.....|.S.)
+00001e00: 077a 7b20 5265 7475 726e 7320 676c 6f62  .z{ Returns glob
+00001e10: 616c 6c79 2064 6566 696e 6564 2068 6f73  ally defined hos
+00001e20: 746e 616d 6520 6966 2061 7661 696c 6162  tname if availab
+00001e30: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+00001e40: 4f74 6865 7277 6965 732c 206c 6574 7320  Otherwies, lets 
+00001e50: 7468 6520 7573 6572 2063 686f 6f73 6520  the user choose 
+00001e60: 6f6e 6520 616e 6420 7374 6f72 6573 2074  one and stores t
+00001e70: 6861 7420 676c 6f62 616c 6c79 2e20 4e72  hat globally. Nr
+00001e80: 0300 0000 5446 724b 0000 0029 02da 0470  ....TFrK...)...p
+00001e90: 726f 7072 2a00 0000 2908 724b 0000 00da  ropr*...).rK....
+00001ea0: 1061 736b 5f66 6f72 5f68 6f73 746e 616d  .ask_for_hostnam
+00001eb0: 65da 0673 6f63 6b65 74da 0b67 6574 686f  e..socket..getho
+00001ec0: 7374 6e61 6d65 720f 0000 0072 0300 0000  stnamer....r....
+00001ed0: 7208 0000 00da 0353 4554 2902 721b 0000  r......SET).r...
+00001ee0: 0072 4b00 0000 721e 0000 0072 1e00 0000  .rK...r....r....
+00001ef0: 721f 0000 0072 8000 0000 db00 0000 7310  r....r........s.
+00001f00: 0000 0008 0408 0104 010e 0212 0202 0106  ................
+00001f10: ff04 027a 214f 7065 6e62 6973 436f 6d6d  ...z!OpenbisComm
+00001f20: 616e 642e 6465 7465 726d 696e 655f 686f  and.determine_ho
+00001f30: 7374 6e61 6d65 6302 0000 0000 0000 0000  stnamec.........
+00001f40: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00001f50: 2000 0000 7400 6401 7401 7c01 8301 1700   ...t.d.t.|.....
+00001f60: 6402 1700 8301 7d02 7c02 720e 7c02 5300  d.....}.|.r.|.S.
+00001f70: 7c01 5300 2903 7a49 2041 736b 7320 7468  |.S.).zI Asks th
+00001f80: 6520 7573 6572 2074 6f20 636f 6e66 6972  e user to confir
+00001f90: 6d20 7468 6520 7375 6767 6573 7465 7320  m the suggestes 
+00001fa0: 686f 7374 6e61 6d65 206f 7220 6368 6f6f  hostname or choo
+00001fb0: 7365 2061 2063 7573 746f 6d20 6f6e 652e  se a custom one.
+00001fc0: 207a 2245 6e74 6572 2068 6f73 746e 616d   z"Enter hostnam
+00001fd0: 6520 2865 6d70 7479 2074 6f20 636f 6e66  e (empty to conf
+00001fe0: 6972 6d20 277a 0427 293a 2029 02da 0569  irm 'z.'): )...i
+00001ff0: 6e70 7574 7288 0000 0029 0372 1b00 0000  nputr....).r....
+00002000: 724b 0000 00da 0e68 6f73 746e 616d 655f  rK.....hostname_
+00002010: 696e 7075 7472 1e00 0000 721e 0000 0072  inputr....r....r
+00002020: 1f00 0000 728c 0000 00e9 0000 0073 0c00  ....r........s..
+00002030: 0000 0202 0e01 04ff 0402 0401 0402 7a1f  ..............z.
+00002040: 4f70 656e 6269 7343 6f6d 6d61 6e64 2e61  OpenbisCommand.a
+00002050: 736b 5f66 6f72 5f68 6f73 746e 616d 6563  sk_for_hostnamec
+00002060: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00002070: 0200 0000 4300 0000 731c 0000 007c 006a  ....C...s....|.j
+00002080: 00a0 01a1 007d 017c 01a0 02a1 0072 0b7c  .....}.|.....r.|
+00002090: 0153 007c 016a 0353 0072 5900 0000 2904  .S.|.j.S.rY...).
+000020a0: 7211 0000 0072 8100 0000 721a 0000 0072  r....r....r....r
+000020b0: 6100 0000 7263 0000 0072 1e00 0000 721e  a...rc...r....r.
+000020c0: 0000 0072 1f00 0000 7283 0000 00f2 0000  ...r....r.......
+000020d0: 0073 0800 0000 0a01 0801 0401 0601 7a13  .s............z.
+000020e0: 4f70 656e 6269 7343 6f6d 6d61 6e64 2e70  OpenbisCommand.p
+000020f0: 6174 6863 0200 0000 0000 0000 0000 0000  athc............
+00002100: 0400 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
+00002110: 0074 00a0 01a1 007d 0269 007d 0374 027c  .t.....}.i.}.t.|
+00002120: 037c 0264 0183 0301 007c 037c 015f 0364  .|.d.....|.|._.d
+00002130: 0253 0029 037a 290a 2020 2020 2020 2020  .S.).z).        
+00002140: 5573 6520 676c 6f62 616c 2063 6f6e 6669  Use global confi
+00002150: 6720 6f6e 6c79 2e0a 2020 2020 2020 2020  g only..        
+00002160: 464e 2904 da09 646d 5f63 6f6e 6669 67da  FN)...dm_config.
+00002170: 1053 6574 7469 6e67 7352 6573 6f6c 7665  .SettingsResolve
+00002180: 7272 0700 0000 7214 0000 0029 0472 1b00  rr....r....).r..
+00002190: 0000 721c 0000 00da 0872 6573 6f6c 7665  ..r......resolve
+000021a0: 7272 0300 0000 721e 0000 0072 1e00 0000  rr....r....r....
+000021b0: 721f 0000 00da 126c 6f61 645f 676c 6f62  r......load_glob
+000021c0: 616c 5f63 6f6e 6669 67f8 0000 0073 0800  al_config....s..
+000021d0: 0000 0804 0401 0c01 0a01 7a21 4f70 656e  ..........z!Open
+000021e0: 6269 7343 6f6d 6d61 6e64 2e6c 6f61 645f  bisCommand.load_
+000021f0: 676c 6f62 616c 5f63 6f6e 6669 674e 292c  global_configN),
+00002200: 725a 0000 00da 0a5f 5f6d 6f64 756c 655f  rZ.....__module_
+00002210: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00002220: 075f 5f64 6f63 5f5f 7220 0000 0072 2400  .__doc__r ...r$.
+00002230: 0000 722b 0000 0072 2f00 0000 7230 0000  ..r+...r/...r0..
+00002240: 0072 3200 0000 7233 0000 0072 3700 0000  .r2...r3...r7...
+00002250: 7238 0000 0072 3b00 0000 723c 0000 0072  r8...r;...r<...r
+00002260: 3f00 0000 7241 0000 0072 4200 0000 7245  ?...rA...rB...rE
+00002270: 0000 0072 4600 0000 7247 0000 0072 1800  ...rF...rG...r..
+00002280: 0000 7249 0000 0072 4b00 0000 724c 0000  ..rI...rK...rL..
+00002290: 0072 4e00 0000 724f 0000 0072 5100 0000  .rN...rO...rQ...
+000022a0: 7252 0000 0072 5400 0000 7255 0000 0072  rR...rT...rU...r
+000022b0: 5700 0000 7258 0000 0072 5b00 0000 7264  W...rX...r[...rd
+000022c0: 0000 0072 6200 0000 7219 0000 0072 7600  ...rb...r....rv.
+000022d0: 0000 727f 0000 0072 7200 0000 7280 0000  ..r....rr...r...
+000022e0: 0072 8c00 0000 7283 0000 0072 9500 0000  .r....r....r....
+000022f0: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+00002300: 1f00 0000 7209 0000 001c 0000 0073 5400  ....r........sT.
+00002310: 0000 0800 0401 0803 0815 0803 0803 0803  ................
+00002320: 0803 0803 0803 0803 0803 0803 0803 0803  ................
+00002330: 0803 0803 0803 0803 0803 0803 0803 0803  ................
+00002340: 0803 0803 0803 0803 0803 0803 0803 0803  ................
+00002350: 0803 0804 0809 0804 0818 080b 0804 081a  ................
+00002360: 080e 0809 0c06 7209 0000 0063 0000 0000  ......r....c....
+00002370: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00002380: 4000 0000 7332 0000 0065 005a 0164 005a  @...s2...e.Z.d.Z
+00002390: 0264 015a 0364 0c64 0464 0584 015a 0464  .d.Z.d.d.d...Z.d
+000023a0: 0664 0784 005a 0564 0864 0984 005a 0664  .d...Z.d.d...Z.d
+000023b0: 0a64 0b84 005a 0764 0253 0029 0dda 1343  .d...Z.d.S.)...C
+000023c0: 6f6e 7465 6e74 436f 7079 5365 6c65 6374  ontentCopySelect
+000023d0: 6f72 7a7a 2049 6e20 6361 7365 2061 2063  orzz In case a c
+000023e0: 6f6d 6d61 6e64 206e 6565 6473 2069 6e66  ommand needs inf
+000023f0: 6f72 6d61 7469 6f6e 2066 726f 6d20 6120  ormation from a 
+00002400: 636f 6e74 656e 7420 636f 7079 2c20 7468  content copy, th
+00002410: 6973 2063 6c61 7373 0a20 2020 2061 736b  is class.    ask
+00002420: 7320 7468 6520 7573 6572 2074 6f20 7069  s the user to pi
+00002430: 636b 206f 6e65 2069 6620 7468 6572 6520  ck one if there 
+00002440: 6172 6520 6d75 6c74 6970 6c65 2e20 4e46  are multiple. NF
+00002450: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
+00002460: 0002 0000 0043 0000 0073 1600 0000 7c01  .....C...s....|.
+00002470: 7c00 5f00 7c02 7c00 5f01 7c03 7c00 5f02  |._.|.|._.|.|._.
+00002480: 6400 5300 7259 0000 0029 0372 3500 0000  d.S.rY...).r5...
+00002490: da12 636f 6e74 656e 745f 636f 7079 5f69  ..content_copy_i
+000024a0: 6e64 6578 da09 6765 745f 696e 6465 7829  ndex..get_index)
+000024b0: 0472 1b00 0000 7235 0000 0072 9a00 0000  .r....r5...r....
+000024c0: 729b 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+000024d0: 1f00 0000 7220 0000 0006 0100 0073 0600  ....r .......s..
+000024e0: 0000 0601 0601 0a01 7a1c 436f 6e74 656e  ........z.Conten
+000024f0: 7443 6f70 7953 656c 6563 746f 722e 5f5f  tCopySelector.__
+00002500: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00002510: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+00002520: 2a00 0000 7c00 a000 a100 7d01 7c00 6a01  *...|.....}.|.j.
+00002530: 6401 6b02 720b 7c01 5300 7c00 6a02 6a03  d.k.r.|.S.|.j.j.
+00002540: 6402 1900 6403 1900 7c01 1900 5300 2904  d...d...|...S.).
+00002550: 4e54 da0a 6c69 6e6b 6564 4461 7461 da0d  NT..linkedData..
+00002560: 636f 6e74 656e 7443 6f70 6965 7329 04da  contentCopies)..
+00002570: 0c73 656c 6563 745f 696e 6465 7872 9b00  .select_indexr..
+00002580: 0000 7235 0000 00da 0464 6174 6129 0272  ..r5.....data).r
+00002590: 1b00 0000 729a 0000 0072 1e00 0000 721e  ....r....r....r.
+000025a0: 0000 0072 1f00 0000 da06 7365 6c65 6374  ...r......select
+000025b0: 0b01 0000 7308 0000 0008 010a 0104 0114  ....s...........
+000025c0: 027a 1a43 6f6e 7465 6e74 436f 7079 5365  .z.ContentCopySe
+000025d0: 6c65 6374 6f72 2e73 656c 6563 7463 0100  lector.selectc..
+000025e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000025f0: 0000 4300 0000 7366 0000 007c 006a 006a  ..C...sf...|.j.j
+00002600: 0164 0119 0064 026b 0372 1474 0264 037c  .d...d.k.r.t.d.|
+00002610: 006a 006a 0164 0119 0017 0064 0417 0083  .j.j.d.....d....
+00002620: 0182 017c 006a 006a 0164 0519 0064 0619  ...|.j.j.d...d..
+00002630: 007d 0174 037c 0183 0164 076b 0272 2674  .}.t.|...d.k.r&t
+00002640: 0264 0883 0182 0174 037c 0183 0164 096b  .d.....t.|...d.k
+00002650: 0272 2e64 0753 007c 00a0 047c 01a1 0153  .r.d.S.|...|...S
+00002660: 0029 0a4e da04 6b69 6e64 da04 4c49 4e4b  .).N..kind..LINK
+00002670: 7a14 4461 7461 2073 6574 2069 7320 6f66  z.Data set is of
+00002680: 2074 7970 6520 7a14 2062 7574 2073 686f   type z. but sho
+00002690: 756c 6420 6265 204c 494e 4b2e 729c 0000  uld be LINK.r...
+000026a0: 0072 9d00 0000 7201 0000 007a 1f44 6174  .r....r....z.Dat
+000026b0: 6120 7365 7420 6861 7320 6e6f 2063 6f6e  a set has no con
+000026c0: 7465 6e74 2063 6f70 6965 732e e901 0000  tent copies.....
+000026d0: 0029 0572 3500 0000 729f 0000 0072 6e00  .).r5...r....rn.
+000026e0: 0000 da03 6c65 6eda 1973 656c 6563 745f  ....len..select_
+000026f0: 636f 6e74 656e 745f 636f 7079 5f69 6e64  content_copy_ind
+00002700: 6578 2902 721b 0000 00da 0e63 6f6e 7465  ex).r......conte
+00002710: 6e74 5f63 6f70 6965 7372 1e00 0000 721e  nt_copiesr....r.
+00002720: 0000 0072 1f00 0000 729e 0000 0012 0100  ...r....r.......
+00002730: 0073 1800 0000 1001 0401 0a01 02ff 0201  .s..............
+00002740: 06ff 1002 0c01 0801 0c01 0401 0a02 7a20  ..............z 
+00002750: 436f 6e74 656e 7443 6f70 7953 656c 6563  ContentCopySelec
+00002760: 746f 722e 7365 6c65 6374 5f69 6e64 6578  tor.select_index
+00002770: 6302 0000 0000 0000 0000 0000 0008 0000  c...............
+00002780: 0007 0000 0043 0000 0073 ae00 0000 7c00  .....C...s....|.
+00002790: 6a00 6400 7501 7218 7c00 6a00 6401 6b05  j.d.u.r.|.j.d.k.
+000027a0: 7214 7c00 6a00 7401 7c01 8301 6b00 7214  r.|.j.t.|...k.r.
+000027b0: 7c00 6a00 5300 7402 6402 8301 8201 0900  |.j.S.t.d.......
+000027c0: 7403 6404 8301 0100 7404 7c01 8301 4400  t.d.....t.|...D.
+000027d0: 5d1c 5c02 7d02 7d03 7c03 6405 1900 6406  ].\.}.}.|.d...d.
+000027e0: 1900 a005 6407 a101 6401 1900 7d04 7c03  ....d...d...}.|.
+000027f0: 6408 1900 7d05 7403 6409 a006 7c02 7c04  d...}.t.d...|.|.
+00002800: 7c05 a103 8301 0100 7121 7407 640a 8301  |.......q!t.d...
+00002810: 7d06 7c06 a008 a100 7256 7409 7c06 8301  }.|.....rVt.|...
+00002820: 7d07 7c07 6401 6b05 7256 7c07 7401 7c01  }.|.d.k.rV|.t.|.
+00002830: 8301 6b00 7256 7c07 5300 7119 290b 4e72  ..k.rV|.S.q.).Nr
+00002840: 0100 0000 7a1b 496e 7661 6c69 6420 636f  ....z.Invalid co
+00002850: 6e74 656e 7420 636f 7079 2069 6e64 6578  ntent copy index
+00002860: 2e54 7a2f 4672 6f6d 2077 6869 6368 206c  .Tz/From which l
+00002870: 6f63 6174 696f 6e20 7368 6f75 6c64 2074  ocation should t
+00002880: 6865 2066 696c 6573 2062 6520 636f 7069  he files be copi
+00002890: 6564 3fda 0b65 7874 6572 6e61 6c44 6d73  ed?..externalDms
+000028a0: da07 6164 6472 6573 73fa 013a 7283 0000  ..address..:r...
+000028b0: 007a 0b20 207b 7d29 207b 7d3a 7b7d 7a02  .z.  {}) {}:{}z.
+000028c0: 3e20 290a 729a 0000 0072 a400 0000 726e  > ).r....r....rn
+000028d0: 0000 00da 0570 7269 6e74 da09 656e 756d  .....print..enum
+000028e0: 6572 6174 6572 8400 0000 726d 0000 0072  erater....rm...r
+000028f0: 9000 0000 da07 6973 6469 6769 74da 0369  ......isdigit..i
+00002900: 6e74 2908 721b 0000 0072 a600 0000 da01  nt).r....r......
+00002910: 69da 0c63 6f6e 7465 6e74 5f63 6f70 79da  i..content_copy.
+00002920: 0468 6f73 7472 8300 0000 da11 636f 7079  .hostr......copy
+00002930: 5f69 6e64 6578 5f73 7472 696e 67da 0e63  _index_string..c
+00002940: 6f70 795f 696e 6465 785f 696e 7472 1e00  opy_index_intr..
+00002950: 0000 721e 0000 0072 1f00 0000 72a5 0000  ..r....r....r...
+00002960: 001e 0100 0073 2000 0000 0a01 1802 0601  .....s .........
+00002970: 0802 0203 0801 1001 1601 0801 1401 0802  ................
+00002980: 0801 0801 1401 0401 02f5 7a2d 436f 6e74  ..........z-Cont
+00002990: 656e 7443 6f70 7953 656c 6563 746f 722e  entCopySelector.
+000029a0: 7365 6c65 6374 5f63 6f6e 7465 6e74 5f63  select_content_c
+000029b0: 6f70 795f 696e 6465 7829 024e 4629 0872  opy_index).NF).r
+000029c0: 5a00 0000 7296 0000 0072 9700 0000 7298  Z...r....r....r.
+000029d0: 0000 0072 2000 0000 72a0 0000 0072 9e00  ...r ...r....r..
+000029e0: 0000 72a5 0000 0072 1e00 0000 721e 0000  ..r....r....r...
+000029f0: 0072 1e00 0000 721f 0000 0072 9900 0000  .r....r....r....
+00002a00: 0201 0000 730c 0000 0008 0004 010a 0308  ....s...........
+00002a10: 0508 070c 0c72 9900 0000 2911 726c 0000  .....r....).rl..
+00002a20: 0072 7800 0000 7282 0000 0072 8d00 0000  .rx...r....r....
+00002a30: 7216 0000 0072 5e00 0000 7203 0000 0072  r....r^...r....r
+00002a40: 9200 0000 da0e 636f 6d6d 616e 645f 7265  ......command_re
+00002a50: 7375 6c74 7204 0000 0072 0600 0000 da05  sultr....r......
+00002a60: 7574 696c 7372 0700 0000 7208 0000 0072  utilsr....r....r
+00002a70: 3e00 0000 7209 0000 0072 9900 0000 721e  >...r....r....r.
+00002a80: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+00002a90: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00002aa0: 7318 0000 0008 0e08 0108 0108 0108 020c  s...............
+00002ab0: 020c 010c 0110 0110 0300 7f14 67         ............g
```

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/removeref.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/removeref.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/__pycache__/upload.cpython-310.pyc` & `obis-0.4.2rc1/obis/dm/commands/__pycache__/upload.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/addref.py` & `obis-0.4.2rc1/obis/dm/commands/addref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/clone.py` & `obis-0.4.2rc1/obis/dm/commands/clone.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/collection.py` & `obis-0.4.2rc1/obis/dm/commands/collection.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/download.py` & `obis-0.4.2rc1/obis/dm/commands/download.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/download_physical.py` & `obis-0.4.2rc1/obis/dm/commands/download_physical.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/move.py` & `obis-0.4.2rc1/obis/dm/commands/move.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/object.py` & `obis-0.4.2rc1/obis/dm/commands/object.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/openbis_command.py` & `obis-0.4.2rc1/obis/dm/commands/openbis_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,16 @@
     def check_configuration(self):
         """ overwrite in subclass """
         return CommandResult(returncode=0, output="")
 
     def login(self):
         """ Restore session token if available. """
         if 'config' in self.config_dict.keys():
-            if 'openbis_token' in self.config_dict['config'].keys():
+            if 'openbis_token' in self.config_dict['config'].keys() and \
+                    self.config_dict['config']['openbis_token'] is not None:
                 self.openbis.set_token(self.config_dict['config']['openbis_token'], True)
         """ Checks for valid session and asks user for password
         if login is needed. """
         user = self.user()
         if self.openbis.is_session_active():
             if self.openbis.token.startswith(user) or self.openbis.token.startswith('$pat-' + user):
                 return CommandResult(returncode=0, output="")
@@ -221,15 +222,16 @@
         # from global config
         hostname = self.hostname()
         if hostname is not None:
             return hostname
         # ask user
         hostname = self.ask_for_hostname(socket.gethostname())
         # store
-        self.data_mgmt.config('config', True, False, OperationType.SET, prop='hostname', value=hostname)
+        self.data_mgmt.config('config', True, False, OperationType.SET, prop='hostname',
+                              value=hostname)
         return hostname
 
     def ask_for_hostname(self, hostname):
         """ Asks the user to confirm the suggestes hostname or choose a custom one. """
         hostname_input = input(
             'Enter hostname (empty to confirm \'' + str(hostname) + '\'): ')
         if hostname_input:
```

### Comparing `obis-0.4.1/obis/dm/commands/openbis_command_test.py` & `obis-0.4.2rc1/obis/dm/commands/openbis_command_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/openbis_sync.py` & `obis-0.4.2rc1/obis/dm/commands/openbis_sync.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/removeref.py` & `obis-0.4.2rc1/obis/dm/commands/removeref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/commands/upload.py` & `obis-0.4.2rc1/obis/dm/commands/upload.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/config.py` & `obis-0.4.2rc1/obis/dm/config.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/config_test.py` & `obis-0.4.2rc1/obis/dm/config_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/data_mgmt.py` & `obis-0.4.2rc1/obis/dm/data_mgmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,16 @@
                 repository_type = Type.PHYSICAL
             else:
                 repository_type = Type.LINK
         else:
             repository_type = Type.LINK
 
     if repository_type == Type.PHYSICAL:
-        return PhysicalDataMgmt(settings_resolver, None, None, openbis, log, data_path,
+        complete_openbis_config(openbis_config, settings_resolver)
+        return PhysicalDataMgmt(settings_resolver, openbis_config, None, openbis, log, data_path,
                                 metadata_path, invocation_path)
     else:
         complete_git_config(git_config)
         git_wrapper = GitWrapper(**git_config)
         if not git_wrapper.can_run():
             # TODO We could just as well throw an error here instead of creating
             #      creating the NoGitDataMgmt which will fail later.
@@ -225,25 +226,27 @@
         :param sample_id: permId or sample path of the parent sample
         :param data_set_type: type of created data set
         :param files: list of files/directories to upload
         """
         return
 
     @abc.abstractmethod
-    def search_object(self, filters, save):
+    def search_object(self, filters, recursive, save):
         """Search for objects in openBIS using filtering criteria.
         :param filters: dictionary of filter parameters
+        :param recursive: Flag indicating if search should include children recursively
         :param save: File path to save results. If missing, search results will not be saved.
         """
         return
 
     @abc.abstractmethod
-    def search_data_set(self, filters, save):
+    def search_data_set(self, filters, recursive, save):
         """Search for datasets in openBIS using filtering criteria.
         :param filters: dictionary of filter parameters
+        :param recursive: Flag indicating if search should include children recursively
         :param save: File path to save results. If missing, search results will not be saved.
         """
         return
 
     def update_config(self, resolver, debug, is_global, is_data_set_property, operation_type,
                       prop=None,
                       value=None):
@@ -638,20 +641,20 @@
         cmd = DownloadPhysical(self, data_set_id, from_file, file, skip_integrity_check)
         return cmd.run()
 
     def upload(self, sample_id, data_set_type, files):
         cmd = Upload(self, sample_id, data_set_type, files)
         return cmd.run()
 
-    def search_object(self,filters, save):
-        cmd = Search(self, filters, save)
+    def search_object(self, filters, recursive, save):
+        cmd = Search(self, filters, recursive, save)
         return cmd.search_samples()
 
-    def search_data_set(self, filters, save):
-        cmd = Search(self, filters, save)
+    def search_data_set(self, filters, recursive, save):
+        cmd = Search(self, filters, recursive, save)
         return cmd.search_data_sets()
 
     def config(self, category, is_global, is_data_set_property, operation_type, prop=None,
                value=None):
         """
         :param category: config, object, collection, data_set or repository
         :param is_global: act on global settings - local if false
```

### Comparing `obis-0.4.1/obis/dm/data_mgmt_test.py` & `obis-0.4.2rc1/obis/dm/data_mgmt_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/git.py` & `obis-0.4.2rc1/obis/dm/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 #   limitations under the License.
 #
 import os
 import shutil
 
 from .checksum import ChecksumGeneratorCrc32, ChecksumGeneratorGitAnnex
 from .utils import run_shell
+from ..scripts.click_util import click_echo
 
 
 class GitWrapper(object):
     """A wrapper on commands to git and git annex."""
 
-    def __init__(self, git_path=None, git_annex_path=None, find_git=None, data_path=None, metadata_path=None, invocation_path=None):
+    def __init__(self, git_path=None, git_annex_path=None, find_git=None, data_path=None,
+                 metadata_path=None, invocation_path=None):
         self.git_path = git_path
         self.git_annex_path = git_annex_path
         self.data_path = data_path
         self.metadata_path = metadata_path
 
     def _git(self, params, strip_leading_whitespace=True, relative_repo_path=''):
         """ all git invocations need to go through this method
@@ -35,36 +37,39 @@
         cmd = [self.git_path]
         if self.data_path is not None and self.metadata_path is not None:
             git_dir = os.path.join(self.metadata_path, relative_repo_path, '.git')
             cmd += ['--work-tree', self.data_path, '--git-dir', git_dir]
         cmd += params
         return run_shell(cmd, strip_leading_whitespace=strip_leading_whitespace)
 
-
     def can_run(self):
         """Return true if the perquisites are satisfied to run (git and git annex)"""
         if self.git_path is None:
+            click_echo('No git path found!')
             return False
         if self.git_annex_path is None:
+            click_echo('No git-annex path found!')
             return False
         if self._git(['help']).failure():
+            click_echo('Can not run git!')
             # git help should have a returncode of 0
             return False
         if self._git(['annex', 'help']).failure():
+            click_echo('Can not run git-annex!')
             # git help should have a returncode of 0
             return False
         result = run_shell([self.git_path, 'annex', 'version'])
         if result.success():
             first_line = result.output.split("\n")[0].split(":")
             if len(first_line) > 1:
                 self.annex_version = first_line[1].strip()
                 try:
                     self.annex_major_version = int(self.annex_version.split(".")[0])
                 except Exception as e:
-                    print("Invalid git-annex version line:",result.output)
+                    print("Invalid git-annex version line:", result.output)
                     return False
         return True
 
     def git_init(self):
         result = self._git(["init"])
         self.git_ignore('.obis')
         self.git_ignore('.obis_restorepoint')
@@ -195,17 +200,19 @@
         lines = tree.output.split("\n")
         files = [line.split("\t")[-1].strip() for line in lines]
         return files
 
     def cksum(self, files, git_annex_hash_as_checksum=False):
 
         if git_annex_hash_as_checksum == False:
-            checksum_generator = ChecksumGeneratorCrc32(self.git_wrapper.data_path, self.git_wrapper.metadata_path)
+            checksum_generator = ChecksumGeneratorCrc32(self.git_wrapper.data_path,
+                                                        self.git_wrapper.metadata_path)
         else:
-            checksum_generator = ChecksumGeneratorGitAnnex(self.git_wrapper.data_path, self.git_wrapper.metadata_path)
+            checksum_generator = ChecksumGeneratorGitAnnex(self.git_wrapper.data_path,
+                                                           self.git_wrapper.metadata_path)
 
         checksums = []
 
         for file in files:
             checksum = checksum_generator.get_checksum(file)
             checksums.append(checksum)
```

### Comparing `obis-0.4.1/obis/dm/repository_utils.py` & `obis-0.4.2rc1/obis/dm/repository_utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/dm/utils.py` & `obis-0.4.2rc1/obis/dm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     config_dict = resolver.config.config_dict(local_only)
     if config.get('url') is None:
         config['url'] = config_dict['openbis_url']
     if config.get('verify_certificates') is None:
         config['verify_certificates'] = config_dict['verify_certificates']
     if config.get('token') is None:
         config['token'] = None
-    if config.get('is_physical') is None:
-        config['is_physical'] = None
+    if config.get('is_physical') is None and config_dict['is_physical'] is not None:
+        config['is_physical'] = config_dict['is_physical']
     if config.get(
             'allow_http_but_do_not_use_this_in_production_and_only_within_safe_networks') is None:
         config['allow_http_but_do_not_use_this_in_production_and_only_within_safe_networks'] = not \
-        config_dict['allow_only_https']
+            config_dict['allow_only_https']
 
 
 def complete_git_config(config):
     """Add default values for empty entries in the config."""
 
     find_git = config['find_git'] if config.get('find_git') is not None else True
     if find_git:
```

### Comparing `obis-0.4.1/obis/dm/utils_test.py` & `obis-0.4.2rc1/obis/dm/utils_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/scripts/__init__.py` & `obis-0.4.2rc1/obis/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/scripts/__pycache__/cli.cpython-310.pyc` & `obis-0.4.2rc1/obis/scripts/__pycache__/cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar  3 11:10:13 2023 UTC, .py size: 31141 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 95d5 0164 a579 0000  o..........d.y..
+00000000: 6f0d 0d0a 0000 0000 f7b2 2664 938a 0000  o.........&d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000f 0000 0040 0000 0073 760b 0000 6400  .....@...sv...d.
+00000020: 0013 0000 0040 0000 0073 b20b 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d03 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c04 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c09 6d0a 5a0a 0100 6407 6408 6c0b  d.l.m.Z...d.d.l.
 00000080: 6d0c 5a0c 0100 6407 6409 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
 00000090: 0100 640a 640b 6c0f 6d10 5a10 0100 640a  ..d.d.l.m.Z...d.
@@ -17,15 +17,15 @@
 00000100: 6417 641f 6419 8d05 6504 6a19 6420 6421  d.d.d...e.j.d d!
 00000110: 8400 8301 8301 8301 8301 8301 8301 5a1a  ..............Z.
 00000120: 6422 6423 8400 5a1b 6424 6425 8400 5a1c  d"d#..Z.d$d%..Z.
 00000130: 4700 6426 6427 8400 6427 6504 6a1d 8303  G.d&d'..d'e.j...
 00000140: 5a1e 4700 6428 6429 8400 6429 651e 8303  Z.G.d(d)..d)e...
 00000150: 5a1f 4700 642a 642b 8400 642b 6504 6a1d  Z.G.d*d+..d+e.j.
 00000160: 8303 5a20 642c 642d 8400 5a21 642e 642f  ..Z d,d-..Z!d.d/
-00000170: 8400 5a22 9001 6412 6430 6431 8401 5a23  ..Z"..d.d0d1..Z#
+00000170: 8400 5a22 9001 641c 6430 6431 8401 5a23  ..Z"..d.d0d1..Z#
 00000180: 6432 6433 8400 5a24 6434 6435 8400 5a25  d2d3..Z$d4d5..Z%
 00000190: 6436 6437 8400 5a26 651a a016 a100 6504  d6d7..Z&e.....e.
 000001a0: 6a18 6438 6439 6416 6417 643a 6419 8d05  j.d8d9d.d.d:d...
 000001b0: 6504 6a19 643b 643c 8400 8301 8301 8301  e.j.d;d<........
 000001c0: 5a27 6527 a028 643d a101 6504 6a19 643e  Z'e'.(d=..e.j.d>
 000001d0: 643f 8400 8301 8301 5a29 651a a016 a100  d?......Z)e.....
 000001e0: 6504 6a18 6438 6439 6416 6417 6440 6419  e.j.d8d9d.d.d@d.
@@ -38,1557 +38,1772 @@
 00000250: 8301 8301 8301 5a2d 652a a028 644a a101  ......Z-e*.(dJ..
 00000260: 6504 6a2b 643c 651f 8300 6444 6445 8d03  e.j+d<e...dDdE..
 00000270: 6504 6a19 644b 644c 8400 8301 8301 8301  e.j.dKdL........
 00000280: 5a2e 6504 6a18 644d 644e 644f 6402 6450  Z.e.j.dMdNdOd.dP
 00000290: 6451 8d05 6504 6a18 6452 6453 6402 6454  dQ..e.j.dRdSd.dT
 000002a0: 6451 8d04 6504 6a18 6455 6456 6402 6457  dQ..e.j.dUdVd.dW
 000002b0: 6451 8d04 6504 6a18 6458 6459 6402 645a  dQ..e.j.dXdYd.dZ
-000002c0: 6451 8d04 6504 6a18 645b 645c 644f 6402  dQ..e.j.d[d\dOd.
-000002d0: 645d 6451 8d05 6504 6a18 645e 645f 6402  d]dQ..e.j.d^d_d.
-000002e0: 6460 6451 8d04 6504 6a18 6461 6462 6402  d`dQ..e.j.dadbd.
-000002f0: 6463 6451 8d04 6504 6a18 6464 6465 6466  dcdQ..e.j.dddedf
-00000300: 6402 6467 6451 8d05 6504 6a18 6468 6469  d.dgdQ..e.j.dhdi
+000002c0: 6451 8d04 6504 6a18 645b 645c 645d 6402  dQ..e.j.d[d\d]d.
+000002d0: 645e 6451 8d05 6504 6a18 645f 6460 644f  d^dQ..e.j.d_d`dO
+000002e0: 6402 6461 6451 8d05 6504 6a18 6462 6463  d.dadQ..e.j.dbdc
+000002f0: 6402 6464 6451 8d04 6504 6a18 6465 6466  d.dddQ..e.j.dedf
+00000300: 6402 6467 6451 8d04 6504 6a18 6468 6469  d.dgdQ..e.j.dhdi
 00000310: 646a 6402 646b 6451 8d05 6504 6a18 646c  djd.dkdQ..e.j.dl
-00000320: 646d 6402 646e 6451 8d04 670a 5a2f 651a  dmd.dndQ..g.Z/e.
-00000330: a016 646f a101 6504 6a18 6438 6439 6416  ..do..e.j.d8d9d.
-00000340: 6417 6440 6419 8d05 6504 6a18 6470 6471  d.d@d...e.j.dpdq
-00000350: 6416 6417 6472 6419 8d05 6504 6a19 6473  d.d.drd...e.j.ds
-00000360: 646f 8400 8301 8301 8301 8301 5a30 6530  do..........Z0e0
-00000370: a028 6443 a101 6504 6a2b 6474 6520 8300  .(dC..e.j+dte ..
-00000380: 6444 6445 8d03 6504 6a19 6475 6476 8400  dDdE..e.j.dudv..
-00000390: 8301 8301 8301 5a31 6530 a028 643d a101  ......Z1e0.(d=..
-000003a0: 6504 6a2b 6474 651e 8300 6444 6445 8d03  e.j+dte...dDdE..
-000003b0: 6504 6a19 6477 6478 8400 8301 8301 8301  e.j.dwdx........
-000003c0: 5a32 6530 a028 644a a101 6504 6a2b 6474  Z2e0.(dJ..e.j+dt
-000003d0: 651f 8300 6444 6445 8d03 6504 6a19 6479  e...dDdE..e.j.dy
-000003e0: 647a 8400 8301 8301 8301 5a33 6530 6a28  dz........Z3e0j(
-000003f0: 647b 647c 647d 8d02 6515 652f 8301 6504  d{d|d}..e.e/..e.
-00000400: 6a19 647e 647f 8400 8301 8301 8301 5a34  j.d~d.........Z4
-00000410: 651a a016 a100 6504 6a18 6438 6439 6416  e.....e.j.d8d9d.
-00000420: 6417 6440 6419 8d05 6504 6a19 6480 6481  d.d@d...e.j.d.d.
-00000430: 8400 8301 8301 8301 5a35 6535 a028 6443  ........Z5e5.(dC
-00000440: a101 6504 6a2b 6482 6520 8300 6444 6445  ..e.j+d.e ..dDdE
-00000450: 8d03 6504 6a19 6483 6484 8400 8301 8301  ..e.j.d.d.......
-00000460: 8301 5a36 6535 a028 643d a101 6504 6a2b  ..Z6e5.(d=..e.j+
-00000470: 6482 651e 8300 6444 6445 8d03 6504 6a19  d.e...dDdE..e.j.
-00000480: 6485 6486 8400 8301 8301 8301 5a37 6535  d.d.........Z7e5
-00000490: a028 644a a101 6504 6a2b 6482 651f 8300  .(dJ..e.j+d.e...
-000004a0: 6444 6445 8d03 6504 6a19 6487 6488 8400  dDdE..e.j.d.d...
-000004b0: 8301 8301 8301 5a38 6535 6a28 647b 6489  ......Z8e5j(d{d.
-000004c0: 647d 8d02 6515 652f 8301 6504 6a19 648a  d}..e.e/..e.j.d.
-000004d0: 648b 8400 8301 8301 8301 5a39 651a a016  d.........Z9e...
-000004e0: a100 6504 6a18 6438 6439 6416 6417 6440  ..e.j.d8d9d.d.d@
-000004f0: 6419 8d05 6504 6a19 648c 648d 8400 8301  d...e.j.d.d.....
-00000500: 8301 8301 5a3a 653a a028 6443 a101 6504  ....Z:e:.(dC..e.
-00000510: 6a2b 643c 6520 8300 6444 6445 8d03 6504  j+d<e ..dDdE..e.
-00000520: 6a19 648e 648f 8400 8301 8301 8301 5a3b  j.d.d.........Z;
-00000530: 653a a028 643d a101 6504 6a2b 643c 651e  e:.(d=..e.j+d<e.
-00000540: 8300 6444 6445 8d03 6504 6a19 6490 6491  ..dDdE..e.j.d.d.
-00000550: 8400 8301 8301 8301 5a3c 653a a028 644a  ........Z<e:.(dJ
-00000560: a101 6504 6a2b 643c 651f 8300 6444 6445  ..e.j+d<e...dDdE
-00000570: 8d03 6504 6a19 6492 6493 8400 8301 8301  ..e.j.d.d.......
-00000580: 8301 5a3d 651a a016 a100 6504 6a18 6438  ..Z=e.....e.j.d8
-00000590: 6439 6416 6417 6440 6419 8d05 6504 6a19  d9d.d.d@d...e.j.
-000005a0: 6494 6495 8400 8301 8301 8301 5a3e 653e  d.d.........Z>e>
-000005b0: a028 6443 a101 6504 6a2b 643c 6520 8300  .(dC..e.j+d<e ..
-000005c0: 6444 6445 8d03 6504 6a19 6496 6497 8400  dDdE..e.j.d.d...
-000005d0: 8301 8301 8301 5a3f 653e a028 643d a101  ......Z?e>.(d=..
-000005e0: 6504 6a2b 643c 651e 8300 6444 6445 8d03  e.j+d<e...dDdE..
-000005f0: 6504 6a19 6498 6499 8400 8301 8301 8301  e.j.d.d.........
-00000600: 5a40 653e a028 644a a101 6504 6a2b 643c  Z@e>.(dJ..e.j+d<
-00000610: 651f 8300 6444 6445 8d03 6504 6a19 649a  e...dDdE..e.j.d.
-00000620: 649b 8400 8301 8301 8301 5a41 6504 6a18  d.........ZAe.j.
-00000630: 649c 649d 649e 649f 6451 8d04 6504 6a18  d.d.d.d.dQ..e.j.
-00000640: 64a0 64a1 6417 6417 64a2 6419 8d05 6504  d.d.d.d.d.d...e.
-00000650: 6a18 64a3 64a4 6417 6417 64a5 6419 8d05  j.d.d.d.d.d.d...
-00000660: 6504 6a2b 6442 6504 6a42 6417 6416 64a6  e.j+dBe.jBd.d.d.
-00000670: 8d02 6416 64a7 8d03 6704 5a43 652a 6a28  ..d.d...g.ZCe*j(
-00000680: 64a8 64a9 647d 8d02 6504 6a19 6515 6543  d.d.d}..e.j.e.eC
-00000690: 8301 64aa 64ab 8400 8301 8301 8301 5a44  ..d.d.........ZD
-000006a0: 651a 6a28 64a9 647d 8d01 6504 6a19 6515  e.j(d.d}..e.j.e.
-000006b0: 6543 8301 64ac 64a8 8400 8301 8301 8301  eC..d.d.........
-000006c0: 5a45 6504 6a2b 64ad 6504 6a42 6416 6416  ZEe.j+d.e.jBd.d.
-000006d0: 64a6 8d02 6416 64a7 8d03 6504 6a2b 64ae  d...d.d...e.j+d.
-000006e0: 64af 64b0 8d02 6702 5a46 652a 6a28 64b1  d.d...g.ZFe*j(d.
-000006f0: 64b2 647d 8d02 6504 6a19 6515 6546 8301  d.d}..e.j.e.eF..
-00000700: 64b3 64b4 8400 8301 8301 8301 5a47 6546  d.d.........ZGeF
-00000710: 6504 6a18 6470 64b5 64b6 6416 6417 64a5  e.j.dpd.d.d.d.d.
-00000720: 6419 8d06 6701 1700 5a48 651a 6a28 64b2  d...g...ZHe.j(d.
-00000730: 647d 8d01 6504 6a19 6515 6548 8301 64b7  d}..e.j.e.eH..d.
-00000740: 64b1 8400 8301 8301 8301 5a49 6504 6a18  d.........ZIe.j.
-00000750: 6470 64b8 6504 6a42 6416 6416 64a6 8d02  dpd.e.jBd.d.d...
-00000760: 64b9 8d03 6701 5a4a 654a 6546 3700 5a4a  d...g.ZJeJeF7.ZJ
-00000770: 652a 6a28 64ba 64bb 647d 8d02 6504 6a19  e*j(d.d.d}..e.j.
-00000780: 6515 654a 8301 64bc 64bd 8400 8301 8301  e.eJ..d.d.......
-00000790: 8301 5a4b 651a 6a28 64ba 64bb 64be 8d02  ..ZKe.j(d.d.d...
-000007a0: 6504 6a19 6515 654a 8301 64bf 64ba 8400  e.j.e.eJ..d.d...
-000007b0: 8301 8301 8301 5a4c 6504 6a2b 6442 6504  ......ZLe.j+dBe.
-000007c0: 6a42 6417 6416 64a6 8d02 6416 64a7 8d03  jBd.d.d...d.d...
-000007d0: 6701 5a4d 652a 6a28 64c0 64c1 647d 8d02  g.ZMe*j(d.d.d}..
-000007e0: 6504 6a19 6515 654d 8301 64c2 64c3 8400  e.j.e.eM..d.d...
-000007f0: 8301 8301 8301 5a4e 651a 6a28 64c1 647d  ......ZNe.j(d.d}
-00000800: 8d01 6504 6a19 6515 654d 8301 64c4 64c0  ..e.j.e.eM..d.d.
-00000810: 8400 8301 8301 8301 5a4f 6504 6a18 64a3  ........ZOe.j.d.
-00000820: 64a4 6417 6417 64a5 6419 8d05 6504 6a2b  d.d.d.d.d...e.j+
-00000830: 6442 6504 6a42 6417 6416 64a6 8d02 6416  dBe.jBd.d.d...d.
-00000840: 64a7 8d03 6702 5a50 64c5 64c6 8400 5a51  d...g.ZPd.d...ZQ
-00000850: 652a 6a28 64c7 64c8 647d 8d02 6504 6a19  e*j(d.d.d}..e.j.
-00000860: 6515 6550 8301 64c9 64ca 8400 8301 8301  e.eP..d.d.......
-00000870: 8301 5a52 651a 6a28 64c8 647d 8d01 6504  ..ZRe.j(d.d}..e.
-00000880: 6a19 6515 6550 8301 64cb 64c7 8400 8301  j.e.eP..d.d.....
-00000890: 8301 8301 5a53 651a 6a16 64cc 647d 8d01  ....ZSe.j.d.d}..
-000008a0: 6504 6a19 64cd 64ce 8400 8301 8301 5a54  e.j.d.d.......ZT
-000008b0: 6554 6a28 643d 64cf 647d 8d02 6504 6a2b  eTj(d=d.d}..e.j+
-000008c0: 64d0 6416 64d1 8d02 6504 6a18 64d2 64d3  d.d.d...e.j.d.d.
-000008d0: 64d4 8d02 6504 6a18 64d5 64d6 64d4 8d02  d...e.j.d.d.d...
-000008e0: 6504 6a18 64d7 64d8 64d4 8d02 6504 6a19  e.j.d.d.d...e.j.
-000008f0: 9001 6413 64d9 64da 8401 8301 8301 8301  ..d.d.d.........
-00000900: 8301 8301 8301 5a55 6504 6a2b 6442 6504  ......ZUe.j+dBe.
-00000910: 6a42 6417 6416 64a6 8d02 6416 64a7 8d03  jBd.d.d...d.d...
-00000920: 6701 5a56 652a 6a28 64db 64dc 647d 8d02  g.ZVe*j(d.d.d}..
-00000930: 6504 6a19 6515 6556 8301 64dd 64de 8400  e.j.e.eV..d.d...
-00000940: 8301 8301 8301 5a57 651a 6a28 64dc 647d  ......ZWe.j(d.d}
-00000950: 8d01 6504 6a19 6515 6556 8301 64df 64db  ..e.j.e.eV..d.d.
-00000960: 8400 8301 8301 8301 5a58 6504 6a18 641d  ........ZXe.j.d.
-00000970: 64e0 64e1 64d4 8d03 6504 6a2b 6442 6504  d.d.d...e.j+dBe.
-00000980: 6a42 6417 6416 64a6 8d02 6416 64a7 8d03  jBd.d.d...d.d...
-00000990: 6702 5a59 652a 6a28 64e2 64e3 647d 8d02  g.ZYe*j(d.d.d}..
-000009a0: 6504 6a19 6515 6559 8301 64e4 64e5 8400  e.j.e.eY..d.d...
-000009b0: 8301 8301 8301 5a5a 651a 6a28 64e3 647d  ......ZZe.j(d.d}
-000009c0: 8d01 6504 6a19 6515 6559 8301 64e6 64e2  ..e.j.e.eY..d.d.
-000009d0: 8400 8301 8301 8301 5a5b 6504 6a2b 64e7  ........Z[e.j+d.
-000009e0: 6416 64d1 8d02 6504 6a18 64e8 64e9 64ea  d.d...e.j.d.d.d.
-000009f0: 64eb 64d4 8d04 6504 6a18 64ec 64ed 64ee  d.d...e.j.d.d.d.
-00000a00: 64ef 64d4 8d04 6504 6a18 641a 64f0 6416  d.d...e.j.d.d.d.
-00000a10: 6417 64f1 6419 8d05 6704 5a5c 651a 6a28  d.d.d...g.Z\e.j(
-00000a20: 64f2 64f3 647d 8d02 6515 655c 8301 6504  d.d.d}..e.e\..e.
-00000a30: 6a19 64f4 64f2 8400 8301 8301 8301 5a5d  j.d.d.........Z]
-00000a40: 6504 6a18 64ec 64ed 64f5 64f6 6417 6417  e.j.d.d.d.d.d.d.
-00000a50: 64f7 8d06 6504 a02b 64f8 a101 6504 a02b  d...e..+d...e..+
-00000a60: 64f9 a101 6703 5a5e 651a 6a28 64fa 64fb  d...g.Z^e.j(d.d.
-00000a70: 647d 8d02 6515 655e 8301 6504 6a19 64fc  d}..e.e^..e.j.d.
-00000a80: 64fa 8400 8301 8301 8301 5a5f 6504 6a18  d.........Z_e.j.
-00000a90: 64fd 64fe 6402 64ff 6451 8d04 6504 6a18  d.d.d.d.dQ..e.j.
-00000aa0: 9001 6400 9001 6401 6560 6402 9001 6402  ..d...d.e`d...d.
-00000ab0: 9001 6403 8d05 6504 6a18 641a 64f0 6416  ..d...e.j.d.d.d.
-00000ac0: 6417 9001 6404 6419 8d05 6504 a02b 64e7  d...d.d...e..+d.
-00000ad0: a101 6704 5a61 6530 6a28 9001 6405 9001  ..g.Zae0j(..d...
-00000ae0: 6406 647d 8d02 6504 6a19 6515 6561 8301  d.d}..e.j.e.ea..
-00000af0: 9001 6407 9001 6408 8400 8301 8301 8301  ..d...d.........
-00000b00: 5a62 651a 6a28 9001 6406 647d 8d01 6504  Zbe.j(..d.d}..e.
-00000b10: 6a19 6515 6561 8301 9001 6409 9001 6405  j.e.ea....d...d.
-00000b20: 8400 8301 8301 8301 5a63 6530 6a28 9001  ........Zce0j(..
-00000b30: 640a 9001 640b 647d 8d02 6504 6a19 6515  d...d.d}..e.j.e.
-00000b40: 6561 8301 9001 640c 9001 640d 8400 8301  ea....d...d.....
-00000b50: 8301 8301 5a64 651a 6a28 9001 640b 647d  ....Zde.j(..d.d}
-00000b60: 8d01 6504 6a19 6515 6561 8301 9001 640e  ..e.j.e.ea....d.
-00000b70: 9001 640a 8400 8301 8301 8301 5a65 9001  ..d.........Ze..
-00000b80: 640f 9001 6410 8400 5a66 6567 9001 6411  d...d...Zfeg..d.
-00000b90: 6b02 9005 72b9 6566 8300 0100 6402 5300  k...r.ef....d.S.
-00000ba0: 6402 5300 2814 0100 007a 360a 636c 692e  d.S.(....z6.cli.
-00000bb0: 7079 0a0a 5468 6520 6d6f 6475 6c65 2074  py..The module t
-00000bc0: 6861 7420 696d 706c 656d 656e 7473 2074  hat implements t
-00000bd0: 6865 2043 4c49 2066 6f72 206f 6269 732e  he CLI for obis.
-00000be0: 0ae9 0000 0000 4e29 01da 0864 6174 6574  ......N)...datet
-00000bf0: 696d 6529 01da 0d72 656c 6174 6976 6564  ime)...relatived
-00000c00: 656c 7461 2901 da07 4f70 656e 6269 7329  elta)...Openbis)
-00000c10: 01da 0f43 6f6e 6e65 6374 696f 6e45 7272  ...ConnectionErr
-00000c20: 6f72 e901 0000 00a9 01da 0a63 6c69 636b  or.........click
-00000c30: 5f65 6368 6f29 01da 0e44 6174 614d 676d  _echo)...DataMgm
-00000c40: 7452 756e 6e65 72e9 0200 0000 2901 da0d  tRunner.....)...
-00000c50: 436f 6d6d 616e 6452 6573 756c 7429 01da  CommandResult)..
-00000c60: 0d4f 7065 7261 7469 6f6e 5479 7065 6301  .OperationTypec.
-00000c70: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000c80: 0000 0043 0000 0073 2000 0000 7c00 6401  ...C...s ...|.d.
-00000c90: 1900 6402 6b02 720e 7400 7c00 6403 1900  ..d.k.r.t.|.d...
-00000ca0: 8301 0100 6400 5300 6400 5300 2904 4eda  ....d.S.d.S.).N.
-00000cb0: 0474 7970 65da 0870 726f 6772 6573 73da  .type..progress.
-00000cc0: 076d 6573 7361 6765 7207 0000 00a9 01da  .messager.......
-00000cd0: 0d70 726f 6772 6573 735f 6461 7461 a900  .progress_data..
-00000ce0: 7212 0000 00fa 5c2f 686f 6d65 2f61 6c61  r.....\/home/ala
-00000cf0: 736b 6f77 736b 692f 7265 706f 2f6f 7065  skowski/repo/ope
-00000d00: 6e62 6973 5f70 7974 686f 6e2f 6170 702d  nbis_python/app-
-00000d10: 6f70 656e 6269 732d 636f 6d6d 616e 642d  openbis-command-
-00000d20: 6c69 6e65 2f73 7263 2f70 7974 686f 6e2f  line/src/python/
-00000d30: 6f62 6973 2f73 6372 6970 7473 2f63 6c69  obis/scripts/cli
-00000d40: 2e70 79da 0e63 6c69 636b 5f70 726f 6772  .py..click_progr
-00000d50: 6573 7327 0000 0073 0600 0000 0c01 1001  ess'...s........
-00000d60: 04ff 7214 0000 0063 0100 0000 0000 0000  ..r....c........
-00000d70: 0000 0000 0100 0000 0600 0000 4300 0000  ............C...
-00000d80: 7328 0000 007c 0064 0119 0064 026b 0272  s(...|.d...d.k.r
-00000d90: 1274 00a0 0164 03a0 027c 0064 0419 00a1  .t...d...|.d....
-00000da0: 01a1 0101 0064 0053 0064 0053 0029 054e  .....d.S.d.S.).N
-00000db0: 720d 0000 0072 0e00 0000 fa02 7b7d 720f  r....r......{}r.
-00000dc0: 0000 0029 03da 0563 6c69 636b da04 6563  ...)...click..ec
-00000dd0: 686f da06 666f 726d 6174 7210 0000 0072  ho..formatr....r
-00000de0: 1200 0000 7212 0000 0072 1300 0000 da14  ....r....r......
-00000df0: 636c 6963 6b5f 7072 6f67 7265 7373 5f6e  click_progress_n
-00000e00: 6f5f 7473 2c00 0000 7306 0000 000c 0118  o_ts,...s.......
-00000e10: 0104 ff72 1900 0000 6301 0000 0000 0000  ...r....c.......
-00000e20: 0000 0000 0002 0000 0003 0000 0003 0000  ................
-00000e30: 0073 1000 0000 8700 6601 6401 6402 8408  .s......f.d.d...
-00000e40: 7d01 7c01 5300 2903 4e63 0100 0000 0000  }.|.S.).Nc......
-00000e50: 0000 0000 0000 0200 0000 0300 0000 1300  ................
-00000e60: 0000 731a 0000 0074 0088 0083 0144 005d  ..s....t.....D.]
-00000e70: 067d 017c 017c 0083 017d 0071 047c 0053  .}.|.|...}.q.|.S
-00000e80: 00a9 014e 2901 da08 7265 7665 7273 6564  ...N)...reversed
-00000e90: 2902 da04 6675 6e63 da05 7061 7261 6da9  )...func..param.
-00000ea0: 01da 0670 6172 616d 7372 1200 0000 7213  ...paramsr....r.
-00000eb0: 0000 00da 0b5f 6164 645f 7061 7261 6d73  ....._add_params
-00000ec0: 3200 0000 7306 0000 000c 010a 0104 017a  2...s..........z
-00000ed0: 1f61 6464 5f70 6172 616d 732e 3c6c 6f63  .add_params.<loc
-00000ee0: 616c 733e 2e5f 6164 645f 7061 7261 6d73  als>._add_params
-00000ef0: 7212 0000 0029 0272 1f00 0000 7220 0000  r....).r....r ..
-00000f00: 0072 1200 0000 721e 0000 0072 1300 0000  .r....r....r....
-00000f10: da0a 6164 645f 7061 7261 6d73 3100 0000  ..add_params1...
-00000f20: 7304 0000 000c 0104 0572 2100 0000 2901  s........r!...).
-00000f30: da07 7665 7273 696f 6e7a 022d 717a 072d  ..versionz.-qz.-
-00000f40: 2d71 7569 6574 4654 7a1a 5375 7070 7265  -quietFTz.Suppre
-00000f50: 7373 2073 7461 7475 7320 7265 706f 7274  ss status report
-00000f60: 696e 672e 2903 da07 6465 6661 756c 74da  ing.)...default.
-00000f70: 0769 735f 666c 6167 da04 6865 6c70 7a02  .is_flag..helpz.
-00000f80: 2d73 7a13 2d2d 736b 6970 5f76 6572 6966  -sz.--skip_verif
-00000f90: 6963 6174 696f 6e7a 1944 6f20 6e6f 7420  icationz.Do not 
-00000fa0: 7665 7269 6679 2063 6572 6669 6369 6174  verify cerficiat
-00000fb0: 6573 7a02 2d64 7a07 2d2d 6465 6275 677a  esz.-dz.--debugz
-00000fc0: 1a53 686f 7720 7374 6163 6b20 7472 6163  .Show stack trac
-00000fd0: 6520 6f6e 2065 7272 6f72 2e63 0400 0000  e on error.c....
-00000fe0: 0000 0000 0000 0000 0400 0000 0300 0000  ................
-00000ff0: 4300 0000 7326 0000 007c 017c 006a 0064  C...s&...|.|.j.d
-00001000: 013c 007c 0272 0c64 027c 006a 0064 033c  .<.|.r.d.|.j.d.<
-00001010: 007c 037c 006a 0064 043c 0064 0053 0029  .|.|.j.d.<.d.S.)
-00001020: 054e da05 7175 6965 7446 da13 7665 7269  .N..quietF..veri
-00001030: 6679 5f63 6572 7469 6669 6361 7465 73da  fy_certificates.
-00001040: 0564 6562 7567 a901 da03 6f62 6a29 04da  .debug....obj)..
-00001050: 0363 7478 7226 0000 00da 1173 6b69 705f  .ctxr&.....skip_
-00001060: 7665 7269 6669 6361 7469 6f6e 7228 0000  verificationr(..
-00001070: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00001080: da03 636c 693a 0000 0073 0800 0000 0a08  ..cli:...s......
-00001090: 0401 0a01 0e01 722d 0000 0063 0300 0000  ......r-...c....
-000010a0: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-000010b0: 0300 0000 7346 0000 007c 0164 0175 0072  ....sF...|.d.u.r
-000010c0: 0664 027d 0174 0064 03a0 017c 01a1 0183  .d.}.t.d...|....
-000010d0: 0101 0088 0064 046b 0372 1388 006e 0164  .....d.k.r...n.d
-000010e0: 0189 007c 006a 0264 0519 00a0 0364 0687  ...|.j.d.....d..
-000010f0: 0066 0164 0764 0884 087c 01a1 0353 0029  .f.d.d...|...S.)
-00001100: 097a 3053 6861 7265 6420 696d 706c 656d  .z0Shared implem
-00001110: 656e 7461 7469 6f6e 2066 6f72 2074 6865  entation for the
-00001120: 2069 6e69 745f 6461 7461 2063 6f6d 6d61   init_data comma
-00001130: 6e64 2e4e da01 2e7a 0c69 6e69 745f 6461  nd.N...z.init_da
-00001140: 7461 207b 7dda 00da 0672 756e 6e65 72da  ta {}....runner.
-00001150: 0969 6e69 745f 6461 7461 6301 0000 0000  .init_datac.....
-00001160: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-00001170: 0000 0073 0a00 0000 7c00 a000 8800 a101  ...s....|.......
-00001180: 5300 721a 0000 0029 0172 3100 0000 a901  S.r....).r1.....
-00001190: da02 646d a901 da04 6465 7363 7212 0000  ..dm....descr...
-000011a0: 0072 1300 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
-000011b0: 4e00 0000 f302 0000 000a 007a 2069 6e69  N..........z ini
-000011c0: 745f 6461 7461 5f69 6d70 6c2e 3c6c 6f63  t_data_impl.<loc
-000011d0: 616c 733e 2e3c 6c61 6d62 6461 3e29 0472  als>.<lambda>).r
-000011e0: 0800 0000 7218 0000 0072 2a00 0000 da03  ....r....r*.....
-000011f0: 7275 6e29 0372 2b00 0000 da0a 7265 706f  run).r+.....repo
-00001200: 7369 746f 7279 7235 0000 0072 1200 0000  sitoryr5...r....
-00001210: 7234 0000 0072 1300 0000 da0e 696e 6974  r4...r......init
-00001220: 5f64 6174 615f 696d 706c 4800 0000 730a  _data_implH...s.
-00001230: 0000 0008 0204 010e 0110 011c 0172 3a00  .............r:.
-00001240: 0000 6304 0000 0000 0000 0000 0000 0006  ..c.............
-00001250: 0000 0006 0000 0003 0000 0073 ce00 0000  ...........s....
-00001260: 7400 6401 a001 7c02 a101 8301 0100 8801  t.d...|.........
-00001270: 6400 7501 7217 7402 6a03 a004 8801 a101  d.u.r.t.j.......
-00001280: 7217 7400 6402 8301 0100 6403 5300 7c02  r.t.d.....d.S.|.
-00001290: 6400 7501 7227 7402 6a03 a004 7c02 a101  d.u.r't.j...|...
-000012a0: 7227 7400 6404 8301 0100 6403 5300 8800  r't.d.....d.S...
-000012b0: 6405 6b03 722d 8800 6e01 6400 8900 8801  d.k.r-..n.d.....
-000012c0: 6400 7500 7237 7402 a005 a100 6e08 7402  d.u.r7t.....n.t.
-000012d0: 6a03 a006 7402 a005 a100 8801 a102 7d04  j...t.........}.
-000012e0: 7402 6a03 a006 7402 a005 a100 7c02 a102  t.j...t.....|...
-000012f0: 7d05 7402 6a03 a007 7c04 7c05 a102 8901  }.t.j...|.|.....
-00001300: 8801 6400 7500 7256 6406 6e01 8801 8901  ..d.u.rVd.n.....
-00001310: 7c00 6a08 6407 1900 a009 6408 8700 8701  |.j.d.....d.....
-00001320: 6602 6409 640a 8408 7c02 a103 5300 290b  f.d.d...|...S.).
-00001330: 4e7a 1069 6e69 745f 616e 616c 7973 6973  Nz.init_analysis
-00001340: 207b 7d7a 3345 7272 6f72 3a20 5468 6520   {}z3Error: The 
-00001350: 7061 7265 6e74 206d 7573 7420 6265 2067  parent must be g
-00001360: 6976 656e 2061 7320 6120 7265 6c61 7469  iven as a relati
-00001370: 7665 2070 6174 682e e9ff ffff ff7a 3745  ve path......z7E
-00001380: 7272 6f72 3a20 5468 6520 7265 706f 7369  rror: The reposi
-00001390: 746f 7279 206d 7573 7420 6265 2067 6976  tory must be giv
-000013a0: 656e 2061 7320 6120 7265 6c61 7469 7665  en as a relative
-000013b0: 2070 6174 682e 722f 0000 007a 022e 2e72   path.r/...z...r
-000013c0: 3000 0000 da0d 696e 6974 5f61 6e61 6c79  0.....init_analy
-000013d0: 7369 7363 0100 0000 0000 0000 0000 0000  sisc............
-000013e0: 0100 0000 0400 0000 1300 0000 730c 0000  ............s...
-000013f0: 007c 00a0 0088 0188 00a1 0253 0072 1a00  .|.........S.r..
-00001400: 0000 2901 723c 0000 0072 3200 0000 a902  ..).r<...r2.....
-00001410: da0b 6465 7363 7269 7074 696f 6eda 0670  ..description..p
-00001420: 6172 656e 7472 1200 0000 7213 0000 0072  arentr....r....r
-00001430: 3600 0000 5e00 0000 f302 0000 000c 007a  6...^..........z
-00001440: 2469 6e69 745f 616e 616c 7973 6973 5f69  $init_analysis_i
-00001450: 6d70 6c2e 3c6c 6f63 616c 733e 2e3c 6c61  mpl.<locals>.<la
-00001460: 6d62 6461 3e29 0a72 0800 0000 7218 0000  mbda>).r....r...
-00001470: 00da 026f 73da 0470 6174 68da 0569 7361  ...os..path..isa
-00001480: 6273 da06 6765 7463 7764 da04 6a6f 696e  bs..getcwd..join
-00001490: da07 7265 6c70 6174 6872 2a00 0000 7238  ..relpathr*...r8
-000014a0: 0000 0029 0672 2b00 0000 723f 0000 0072  ...).r+...r?...r
-000014b0: 3900 0000 723e 0000 00da 0a70 6172 656e  9...r>.....paren
-000014c0: 745f 6469 72da 0c61 6e61 6c79 7369 735f  t_dir..analysis_
-000014d0: 6469 7272 1200 0000 723d 0000 0072 1300  dirr....r=...r..
-000014e0: 0000 da12 696e 6974 5f61 6e61 6c79 7369  ....init_analysi
-000014f0: 735f 696d 706c 5100 0000 731e 0000 000e  s_implQ...s.....
-00001500: 0114 0108 0104 0114 0108 0104 0110 0122  ..............."
-00001510: 0112 010e 0110 0118 0102 0104 ff72 4900  .............rI.
-00001520: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001530: 0000 0002 0000 0040 0000 0073 2000 0000  .......@...s ...
-00001540: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
-00001550: 8400 5a04 6404 6405 8400 5a05 6406 5300  ..Z.d.d...Z.d.S.
-00001560: 2907 da0b 5365 7474 696e 6773 4765 74da  )...SettingsGet.
-00001570: 0c73 6574 7469 6e67 735f 6765 7463 0400  .settings_getc..
-00001580: 0000 0000 0000 0000 0000 0500 0000 0600  ................
-00001590: 0000 4300 0000 7336 0000 007a 0f74 0074  ..C...s6...z.t.t
-000015a0: 0164 0164 0284 007c 01a0 0264 03a1 0183  .d.d...|...d....
-000015b0: 0283 017d 047c 0457 0053 0001 0001 0001  ...}.|.W.S......
-000015c0: 007c 00a0 037c 02a1 0101 0059 0064 0053  .|...|.....Y.d.S
-000015d0: 0029 044e 6301 0000 0000 0000 0000 0000  .).Nc...........
-000015e0: 0001 0000 0002 0000 0053 0000 00f3 0c00  .........S......
-000015f0: 0000 7400 7c00 8301 6401 6b04 5300 a902  ..t.|...d.k.S...
-00001600: 4e72 0100 0000 a901 da03 6c65 6ea9 01da  Nr........len...
-00001610: 0474 6572 6d72 1200 0000 7212 0000 0072  .termr....r....r
-00001620: 1300 0000 7236 0000 006a 0000 0072 4000  ....r6...j...r@.
-00001630: 0000 7a25 5365 7474 696e 6773 4765 742e  ..z%SettingsGet.
-00001640: 636f 6e76 6572 742e 3c6c 6f63 616c 733e  convert.<locals>
-00001650: 2e3c 6c61 6d62 6461 3efa 012c 2904 da04  .<lambda>..,)...
-00001660: 6c69 7374 da06 6669 6c74 6572 da05 7370  list..filter..sp
-00001670: 6c69 74da 055f 6661 696c 2905 da04 7365  lit.._fail)...se
-00001680: 6c66 da05 7661 6c75 6572 1d00 0000 722b  lf..valuer....r+
-00001690: 0000 0072 5500 0000 7212 0000 0072 1200  ...rU...r....r..
-000016a0: 0000 7213 0000 00da 0763 6f6e 7665 7274  ..r......convert
-000016b0: 6800 0000 730a 0000 0002 0118 0106 0106  h...s...........
-000016c0: 0110 017a 1353 6574 7469 6e67 7347 6574  ...z.SettingsGet
-000016d0: 2e63 6f6e 7665 7274 6302 0000 0000 0000  .convertc.......
-000016e0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-000016f0: 00f3 1200 0000 7c00 6a00 7c01 6401 6402  ......|.j.|.d.d.
-00001700: 8d02 0100 6400 5300 2903 4e7a 2f53 6574  ....d.S.).Nz/Set
-00001710: 7469 6e67 7320 6d75 7374 2062 6520 696e  tings must be in
-00001720: 2074 6865 2066 6f72 6d61 743a 206b 6579   the format: key
-00001730: 312c 206b 6579 322c 202e 2e2e a902 721d  1, key2, .....r.
-00001740: 0000 0072 0f00 0000 a901 da04 6661 696c  ...r........fail
-00001750: a902 7257 0000 0072 1d00 0000 7212 0000  ..rW...r....r...
-00001760: 0072 1200 0000 7213 0000 0072 5600 0000  .r....r....rV...
-00001770: 6f00 0000 f306 0000 0004 0104 010a ff7a  o..............z
-00001780: 1153 6574 7469 6e67 7347 6574 2e5f 6661  .SettingsGet._fa
-00001790: 696c 4e29 06da 085f 5f6e 616d 655f 5fda  ilN)...__name__.
-000017a0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000017b0: 7561 6c6e 616d 655f 5fda 046e 616d 6572  ualname__..namer
-000017c0: 5900 0000 7256 0000 0072 1200 0000 7212  Y...rV...r....r.
-000017d0: 0000 0072 1200 0000 7213 0000 0072 4a00  ...r....r....rJ.
-000017e0: 0000 6500 0000 7308 0000 0008 0004 0108  ..e...s.........
-000017f0: 020c 0772 4a00 0000 6300 0000 0000 0000  ...rJ...c.......
-00001800: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00001810: 0073 0c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
-00001820: 5300 2902 da0d 5365 7474 696e 6773 436c  S.)...SettingsCl
-00001830: 6561 724e 2903 7260 0000 0072 6100 0000  earN).r`...ra...
-00001840: 7262 0000 0072 1200 0000 7212 0000 0072  rb...r....r....r
-00001850: 1200 0000 7213 0000 0072 6400 0000 7400  ....r....rd...t.
-00001860: 0000 7304 0000 0008 0004 0172 6400 0000  ..s........rd...
-00001870: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001880: 0002 0000 0040 0000 0073 3000 0000 6500  .....@...s0...e.
-00001890: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
-000018a0: 5a04 6404 6405 8400 5a05 6406 6407 8400  Z.d.d...Z.d.d...
-000018b0: 5a06 6408 6409 8400 5a07 640a 5300 290b  Z.d.d...Z.d.S.).
-000018c0: da0b 5365 7474 696e 6773 5365 74da 0c73  ..SettingsSet..s
-000018d0: 6574 7469 6e67 735f 7365 7463 0400 0000  ettings_setc....
-000018e0: 0000 0000 0000 0000 0900 0000 0600 0000  ................
-000018f0: 4300 0000 738c 0000 007a 3a7c 00a0 007c  C...s....z:|...|
-00001900: 01a1 017d 0169 007d 0474 0174 0264 0164  ...}.i.}.t.t.d.d
-00001910: 0284 007c 01a0 0364 03a1 0183 0283 017d  ...|...d.......}
-00001920: 057c 0544 005d 217d 067c 06a0 0364 04a1  .|.D.]!}.|...d..
-00001930: 017d 0774 047c 0783 0164 056b 0372 287c  .}.t.|...d.k.r(|
-00001940: 00a0 057c 02a1 0101 007c 0764 0619 007d  ...|.....|.d...}
-00001950: 087c 0764 0719 007d 017c 00a0 067c 01a1  .|.d...}.|...|..
-00001960: 017c 047c 083c 0071 167c 0457 0053 0001  .|.|.<.q.|.W.S..
-00001970: 0001 0001 007c 00a0 057c 02a1 0101 0059  .....|...|.....Y
-00001980: 0064 0053 0029 084e 6301 0000 0000 0000  .d.S.).Nc.......
-00001990: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-000019a0: 0072 4c00 0000 724d 0000 0072 4e00 0000  .rL...rM...rN...
-000019b0: 7250 0000 0072 1200 0000 7212 0000 0072  rP...r....r....r
-000019c0: 1300 0000 7236 0000 007f 0000 0072 4000  ....r6.......r@.
-000019d0: 0000 7a25 5365 7474 696e 6773 5365 742e  ..z%SettingsSet.
-000019e0: 636f 6e76 6572 742e 3c6c 6f63 616c 733e  convert.<locals>
-000019f0: 2e3c 6c61 6d62 6461 3e72 5200 0000 fa01  .<lambda>rR.....
-00001a00: 3d72 0a00 0000 7201 0000 0072 0600 0000  =r....r....r....
-00001a10: 2907 da0c 5f65 6e63 6f64 655f 6a73 6f6e  )..._encode_json
-00001a20: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00001a30: 4f00 0000 7256 0000 00da 0c5f 6465 636f  O...rV....._deco
-00001a40: 6465 5f6a 736f 6e29 0972 5700 0000 7258  de_json).rW...rX
-00001a50: 0000 0072 1d00 0000 722b 0000 00da 0873  ...r....r+.....s
-00001a60: 6574 7469 6e67 7372 5500 0000 da07 7365  ettingsrU.....se
-00001a70: 7474 696e 67da 0d73 6574 7469 6e67 5f73  tting..setting_s
-00001a80: 706c 6974 da03 6b65 7972 1200 0000 7212  plit..keyr....r.
-00001a90: 0000 0072 1300 0000 7259 0000 007b 0000  ...r....rY...{..
-00001aa0: 0073 1c00 0000 0201 0a01 0401 1801 0801  .s..............
-00001ab0: 0a01 0c01 0a01 0801 0801 1001 0601 0601  ................
-00001ac0: 1001 7a13 5365 7474 696e 6773 5365 742e  ..z.SettingsSet.
-00001ad0: 636f 6e76 6572 7463 0200 0000 0000 0000  convertc........
-00001ae0: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
-00001af0: 7362 0000 0064 017d 0264 027d 0364 037d  sb...d.}.d.}.d.}
-00001b00: 047c 037d 057c 0144 005d 247d 067c 0664  .|.}.|.D.]$}.|.d
-00001b10: 046b 0272 137c 047d 056e 067c 0664 056b  .k.r.|.}.n.|.d.k
-00001b20: 0272 197c 037d 057c 057c 036b 0272 227c  .r.|.}.|.|.k.r"|
-00001b30: 027c 0637 007d 0271 0a7c 057c 046b 0272  .|.7.}.q.|.|.k.r
-00001b40: 2e7c 027c 06a0 0064 0664 07a1 0237 007d  .|.|...d.d...7.}
-00001b50: 0271 0a7c 0253 0029 084e 722f 0000 0072  .q.|.S.).Nr/...r
-00001b60: 0100 0000 7206 0000 00da 017b da01 7d72  ....r......{..}r
-00001b70: 5200 0000 fa01 7ca9 01da 0772 6570 6c61  R.....|....repla
-00001b80: 6365 2907 7257 0000 0072 5800 0000 da07  ce).rW...rX.....
-00001b90: 656e 636f 6465 64da 0453 4545 4bda 0645  encoded..SEEK..E
-00001ba0: 4e43 4f44 45da 046d 6f64 65da 0463 6861  NCODE..mode..cha
-00001bb0: 7272 1200 0000 7212 0000 0072 1300 0000  rr....r....r....
-00001bc0: 7268 0000 008b 0000 0073 1e00 0000 0401  rh.......s......
-00001bd0: 0401 0401 0401 0801 0801 0601 0801 0401  ................
-00001be0: 0801 0a01 0801 1001 0280 0401 7a18 5365  ............z.Se
-00001bf0: 7474 696e 6773 5365 742e 5f65 6e63 6f64  ttingsSet._encod
-00001c00: 655f 6a73 6f6e 6302 0000 0000 0000 0000  e_jsonc.........
-00001c10: 0000 0002 0000 0004 0000 0043 0000 0073  ...........C...s
-00001c20: 0c00 0000 7c01 a000 6401 6402 a102 5300  ....|...d.d...S.
-00001c30: 2903 4e72 7000 0000 7252 0000 0072 7100  ).Nrp...rR...rq.
-00001c40: 0000 2902 7257 0000 0072 5800 0000 7212  ..).rW...rX...r.
-00001c50: 0000 0072 1200 0000 7213 0000 0072 6900  ...r....r....ri.
-00001c60: 0000 9b00 0000 7302 0000 000c 017a 1853  ......s......z.S
-00001c70: 6574 7469 6e67 7353 6574 2e5f 6465 636f  ettingsSet._deco
-00001c80: 6465 5f6a 736f 6e63 0200 0000 0000 0000  de_jsonc........
-00001c90: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001ca0: 725a 0000 0029 034e 7a3d 5365 7474 696e  rZ...).Nz=Settin
-00001cb0: 6773 206d 7573 7420 6265 2069 6e20 7468  gs must be in th
-00001cc0: 6520 666f 726d 6174 3a20 6b65 7931 3d76  e format: key1=v
-00001cd0: 616c 7565 312c 206b 6579 323d 7661 6c75  alue1, key2=valu
-00001ce0: 6532 2c20 2e2e 2e72 5b00 0000 725c 0000  e2, ...r[...r\..
-00001cf0: 0072 5e00 0000 7212 0000 0072 1200 0000  .r^...r....r....
-00001d00: 7213 0000 0072 5600 0000 9e00 0000 725f  r....rV.......r_
-00001d10: 0000 007a 1153 6574 7469 6e67 7353 6574  ...z.SettingsSet
-00001d20: 2e5f 6661 696c 4e29 0872 6000 0000 7261  ._failN).r`...ra
-00001d30: 0000 0072 6200 0000 7263 0000 0072 5900  ...rb...rc...rY.
-00001d40: 0000 7268 0000 0072 6900 0000 7256 0000  ..rh...ri...rV..
-00001d50: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00001d60: 7213 0000 0072 6500 0000 7800 0000 730c  r....re...x...s.
-00001d70: 0000 0008 0004 0108 0208 1008 100c 0372  ...............r
-00001d80: 6500 0000 6301 0000 0000 0000 0000 0000  e...c...........
-00001d90: 0005 0000 0005 0000 0043 0000 0073 2c00  .........C...s,.
-00001da0: 0000 6900 7d01 7c00 4400 5d0f 7d02 7c02  ..i.}.|.D.].}.|.
-00001db0: a000 a100 4400 5d08 5c02 7d03 7d04 7c04  ....D.].\.}.}.|.
-00001dc0: 7c01 7c03 3c00 710a 7104 7c01 5300 721a  |.|.<.q.q.|.S.r.
-00001dd0: 0000 0029 01da 0569 7465 6d73 2905 da0d  ...)...items)...
-00001de0: 7365 7474 696e 675f 6469 6374 73da 066a  setting_dicts..j
-00001df0: 6f69 6e65 64da 0c73 6574 7469 6e67 5f64  oined..setting_d
-00001e00: 6963 7472 6d00 0000 7258 0000 0072 1200  ictrm...rX...r..
-00001e10: 0000 7212 0000 0072 1300 0000 da12 5f6a  ..r....r......_j
-00001e20: 6f69 6e5f 7365 7474 696e 6773 5f73 6574  oin_settings_set
-00001e30: a300 0000 730c 0000 0004 0108 0110 010a  ....s...........
-00001e40: 0102 ff04 0272 7c00 0000 6301 0000 0000  .....r|...c.....
-00001e50: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-00001e60: 0000 0073 1a00 0000 6700 7d01 7c00 4400  ...s....g.}.|.D.
-00001e70: 5d06 7d02 7c01 7c02 3700 7d01 7104 7c01  ].}.|.|.7.}.q.|.
-00001e80: 5300 721a 0000 0072 1200 0000 2903 da0d  S.r....r....)...
-00001e90: 7365 7474 696e 675f 6c69 7374 7372 7a00  setting_listsrz.
-00001ea0: 0000 da0c 7365 7474 696e 675f 6c69 7374  ....setting_list
-00001eb0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00001ec0: 125f 6a6f 696e 5f73 6574 7469 6e67 735f  ._join_settings_
-00001ed0: 6765 74ab 0000 0073 0800 0000 0401 0801  get....s........
-00001ee0: 0a01 0401 727f 0000 0063 0400 0000 0000  ....r....c......
-00001ef0: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
-00001f00: 0000 7350 0000 007c 006a 0064 0119 007d  ..sP...|.j.d...}
-00001f10: 047c 006a 0064 0219 007d 057c 006a 0064  .|.j.d...}.|.j.d
-00001f20: 0319 007d 0664 047d 0764 057c 006a 0076  ...}.d.}.d.|.j.v
-00001f30: 0072 1b7c 006a 0064 0519 007d 077c 056a  .r.|.j.d...}.|.j
-00001f40: 017c 067c 047c 077c 017c 027c 0364 068d  .|.|.|.|.|.|.d..
-00001f50: 0601 0064 0053 0029 074e da09 6973 5f67  ...d.S.).N..is_g
-00001f60: 6c6f 6261 6c72 3000 0000 da08 7265 736f  lobalr0.....reso
-00001f70: 6c76 6572 46da 1469 735f 6461 7461 5f73  lverF..is_data_s
-00001f80: 6574 5f70 726f 7065 7274 79a9 02da 0470  et_property....p
-00001f90: 726f 7072 5800 0000 2902 722a 0000 00da  roprX...).r*....
-00001fa0: 0663 6f6e 6669 6729 0872 2b00 0000 da0e  .config).r+.....
-00001fb0: 6f70 6572 6174 696f 6e5f 7479 7065 7284  operation_typer.
-00001fc0: 0000 0072 5800 0000 7280 0000 0072 3000  ...rX...r....r0.
-00001fd0: 0000 7281 0000 0072 8200 0000 7212 0000  ..r....r....r...
-00001fe0: 0072 1200 0000 7213 0000 00da 105f 6163  .r....r......_ac
-00001ff0: 6365 7373 5f73 6574 7469 6e67 73b2 0000  cess_settings...
-00002000: 0073 1200 0000 0a01 0a01 0a01 0401 0a01  .s..............
-00002010: 0a01 0c01 0401 0aff 7287 0000 0063 0200  ........r....c..
-00002020: 0000 0000 0000 0000 0000 0500 0000 0700  ................
-00002030: 0000 4300 0000 7338 0000 0074 007c 0183  ..C...s8...t.|..
-00002040: 017d 027c 02a0 01a1 0044 005d 0d5c 027d  .}.|.....D.].\.}
-00002050: 037d 0474 027c 0074 036a 047c 037c 0464  .}.t.|.t.j.|.|.d
-00002060: 018d 0401 0071 0874 0564 0264 0364 048d  .....q.t.d.d.d..
-00002070: 0253 0029 054e 7283 0000 0072 0100 0000  .S.).Nr....r....
-00002080: 722f 0000 00a9 02da 0a72 6574 7572 6e63  r/.......returnc
-00002090: 6f64 65da 066f 7574 7075 7429 0672 7c00  ode..output).r|.
-000020a0: 0000 7278 0000 0072 8700 0000 720c 0000  ..rx...r....r...
-000020b0: 00da 0353 4554 720b 0000 0029 0572 2b00  ...SETr....).r+.
-000020c0: 0000 726a 0000 00da 0d73 6574 7469 6e67  ..rj.....setting
-000020d0: 735f 6469 6374 7284 0000 0072 5800 0000  s_dictr....rX...
-000020e0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-000020f0: 045f 7365 74bd 0000 0073 0800 0000 0801  ._set....s......
-00002100: 1001 1401 0c01 728d 0000 0063 0200 0000  ......r....c....
-00002110: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00002120: 4300 0000 f340 0000 0074 007c 0183 017d  C....@...t.|...}
-00002130: 0274 017c 0283 0164 016b 0272 0d64 0067  .t.|...d.k.r.d.g
-00002140: 017d 027c 0244 005d 0a7d 0374 027c 0074  .}.|.D.].}.t.|.t
-00002150: 036a 047c 0364 028d 0301 0071 0f74 0564  .j.|.d.....q.t.d
-00002160: 0164 0364 048d 0253 00a9 054e 7201 0000  .d.d...S...Nr...
-00002170: 0029 0172 8400 0000 722f 0000 0072 8800  .).r....r/...r..
-00002180: 0000 2906 727f 0000 0072 4f00 0000 7287  ..).r....rO...r.
-00002190: 0000 0072 0c00 0000 da03 4745 5472 0b00  ...r......GETr..
-000021a0: 0000 a904 722b 0000 0072 6a00 0000 da0d  ....r+...rj.....
-000021b0: 7365 7474 696e 6773 5f6c 6973 7472 8400  settings_listr..
-000021c0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000021d0: 00da 045f 6765 74c4 0000 00f3 0c00 0000  ..._get.........
-000021e0: 0801 0c01 0601 0801 1201 0c01 7293 0000  ............r...
-000021f0: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-00002200: 0000 0600 0000 4300 0000 728e 0000 0072  ......C...r....r
-00002210: 8f00 0000 2906 727f 0000 0072 4f00 0000  ....).r....rO...
-00002220: 7287 0000 0072 0c00 0000 da05 434c 4541  r....r......CLEA
-00002230: 5272 0b00 0000 7291 0000 0072 1200 0000  Rr....r....r....
-00002240: 7212 0000 0072 1300 0000 da06 5f63 6c65  r....r......_cle
-00002250: 6172 cd00 0000 7294 0000 0072 9600 0000  ar....r....r....
-00002260: 7a02 2d67 7a0b 2d2d 6973 5f67 6c6f 6261  z.-gz.--is_globa
-00002270: 6c7a 1447 6574 2067 6c6f 6261 6c20 6f72  lz.Get global or
-00002280: 206c 6f63 616c 2e63 0200 0000 0000 0000   local.c........
-00002290: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-000022a0: 730e 0000 007c 017c 006a 0064 013c 0064  s....|.|.j.d.<.d
-000022b0: 0253 0029 037a 1720 4765 7420 616c 6c20  .S.).z. Get all 
-000022c0: 7365 7474 696e 6773 2e0a 2020 2020 7280  settings..    r.
-000022d0: 0000 004e 7229 0000 0029 0272 2b00 0000  ...Nr)...).r+...
-000022e0: 7280 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-000022f0: 1300 0000 726a 0000 00d8 0000 0073 0200  ....rj.......s..
-00002300: 0000 0e06 726a 0000 00da 0367 6574 6301  ....rj.....getc.
-00002310: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-00002320: 0000 0043 0000 0073 3a00 0000 7400 7c00  ...C...s:...t.|.
-00002330: 6a01 6401 6402 8d02 7d01 7c01 a002 a100  j.d.d...}.|.....
-00002340: 7d02 7403 6a04 7c02 6403 6404 6405 8d03  }.t.j.|.d.d.d...
-00002350: 7d03 7405 a006 6406 a007 7c03 a101 a101  }.t...d...|.....
-00002360: 0100 6400 5300 2907 4e46 a901 da11 6861  ..d.S.).NF....ha
-00002370: 6c74 5f6f 6e5f 6572 726f 725f 6c6f 67e9  lt_on_error_log.
-00002380: 0400 0000 5429 02da 0669 6e64 656e 74da  ....T)...indent.
-00002390: 0973 6f72 745f 6b65 7973 7215 0000 0029  .sort_keysr....)
-000023a0: 0872 0900 0000 722a 0000 00da 0c67 6574  .r....r*.....get
-000023b0: 5f73 6574 7469 6e67 73da 046a 736f 6eda  _settings..json.
-000023c0: 0564 756d 7073 7216 0000 0072 1700 0000  .dumpsr....r....
-000023d0: 7218 0000 0029 0472 2b00 0000 7230 0000  r....).r+...r0..
-000023e0: 0072 6a00 0000 da0c 7365 7474 696e 6773  .rj.....settings
-000023f0: 5f73 7472 7212 0000 0072 1200 0000 7213  _strr....r....r.
-00002400: 0000 0072 4b00 0000 e100 0000 7308 0000  ...rK.......s...
-00002410: 000e 0308 0110 0114 0172 4b00 0000 7a18  .........rK...z.
-00002420: 5365 742f 6765 7420 676c 6f62 616c 206f  Set/get global o
-00002430: 7220 6c6f 6361 6c2e 6302 0000 0000 0000  r local.c.......
-00002440: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00002450: 00f3 3000 0000 7400 7c00 6a01 6401 6402  ..0...t.|.j.d.d.
-00002460: 8d02 7d02 7c01 7c00 6a01 6403 3c00 7c02  ..}.|.|.j.d.<.|.
-00002470: 7c00 6a01 6404 3c00 6405 7c00 6a01 6406  |.j.d.<.d.|.j.d.
-00002480: 3c00 6407 5300 2908 7a31 2047 6574 2f73  <.d.S.).z1 Get/s
-00002490: 6574 2073 6574 7469 6e67 7320 7265 6c61  et settings rela
-000024a0: 7465 6420 746f 2074 6865 2072 6570 6f73  ted to the repos
-000024b0: 6974 6f72 792e 0a20 2020 2046 7298 0000  itory..    Fr...
-000024c0: 0072 8000 0000 7230 0000 0072 3900 0000  .r....r0...r9...
-000024d0: 7281 0000 004e a902 7209 0000 0072 2a00  r....N..r....r*.
-000024e0: 0000 a903 722b 0000 0072 8000 0000 7230  ....r+...r....r0
-000024f0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00002500: 0000 7239 0000 00ec 0000 00f3 0800 0000  ..r9............
-00002510: 0e06 0a01 0a01 0e01 7239 0000 00da 0373  ........r9.....s
-00002520: 6574 723b 0000 0029 0272 0d00 0000 da05  etr;...).r......
-00002530: 6e61 7267 7363 0200 0000 0000 0000 0000  nargsc..........
-00002540: 0000 0200 0000 0600 0000 0300 0000 f31c  ................
-00002550: 0000 0088 006a 0064 0119 00a0 0164 0287  .....j.d.....d..
-00002560: 0087 0166 0264 0364 0484 08a1 0253 0029  ...f.d.d.....S.)
-00002570: 054e 7230 0000 00da 0e72 6570 6f73 6974  .Nr0.....reposit
-00002580: 6f72 795f 7365 7463 0100 0000 0000 0000  ory_setc........
-00002590: 0000 0000 0100 0000 0300 0000 1300 0000  ................
-000025a0: f30a 0000 0074 0088 0088 0183 0253 0072  .....t.......S.r
-000025b0: 1a00 0000 a901 728d 0000 0072 3200 0000  ......r....r2...
-000025c0: a902 722b 0000 0072 6a00 0000 7212 0000  ..r+...rj...r...
-000025d0: 0072 1300 0000 7236 0000 00fc 0000 0072  .r....r6.......r
-000025e0: 3700 0000 7a20 7265 706f 7369 746f 7279  7...z repository
-000025f0: 5f73 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c  _set.<locals>.<l
-00002600: 616d 6264 613e a902 722a 0000 0072 3800  ambda>..r*...r8.
-00002610: 0000 72ab 0000 0072 1200 0000 72ab 0000  ..r....r....r...
-00002620: 0072 1300 0000 72a8 0000 00f8 0000 00f3  .r....r.........
-00002630: 0200 0000 1c04 72a8 0000 0063 0200 0000  ......r....c....
-00002640: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00002650: 0300 0000 72a7 0000 0029 054e 7230 0000  ....r....).Nr0..
-00002660: 00da 0e72 6570 6f73 6974 6f72 795f 6765  ...repository_ge
-00002670: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-00002680: 0000 0300 0000 1300 0000 72a9 0000 0072  ..........r....r
-00002690: 1a00 0000 a901 7293 0000 0072 3200 0000  ......r....r2...
-000026a0: 72ab 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000026b0: 3600 0000 0301 0000 7237 0000 007a 2072  6.......r7...z r
-000026c0: 6570 6f73 6974 6f72 795f 6765 742e 3c6c  epository_get.<l
-000026d0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-000026e0: ac00 0000 72ab 0000 0072 1200 0000 72ab  ....r....r....r.
-000026f0: 0000 0072 1300 0000 72ae 0000 00ff 0000  ...r....r.......
-00002700: 0072 ad00 0000 72ae 0000 00da 0563 6c65  .r....r......cle
-00002710: 6172 6302 0000 0000 0000 0000 0000 0002  arc.............
-00002720: 0000 0006 0000 0003 0000 0072 a700 0000  ...........r....
-00002730: 2905 4e72 3000 0000 da10 7265 706f 7369  ).Nr0.....reposi
-00002740: 746f 7279 5f63 6c65 6172 6301 0000 0000  tory_clearc.....
-00002750: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-00002760: 0000 0072 a900 0000 721a 0000 00a9 0172  ...r....r......r
-00002770: 9600 0000 7232 0000 0072 ab00 0000 7212  ....r2...r....r.
-00002780: 0000 0072 1300 0000 7236 0000 000a 0100  ...r....r6......
-00002790: 0072 3700 0000 7a22 7265 706f 7369 746f  .r7...z"reposito
-000027a0: 7279 5f63 6c65 6172 2e3c 6c6f 6361 6c73  ry_clear.<locals
-000027b0: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
-000027c0: ab00 0000 7212 0000 0072 ab00 0000 7213  ....r....r....r.
-000027d0: 0000 0072 b100 0000 0601 0000 72ad 0000  ...r........r...
-000027e0: 0072 b100 0000 7a0c 2d6f 626a 6563 745f  .r....z.-object_
-000027f0: 7479 7065 7a0d 2d2d 6f62 6a65 6374 5f74  typez.--object_t
-00002800: 7970 65da 0974 7970 655f 636f 6465 7a1d  ype..type_codez.
-00002810: 4f62 6a65 6374 2074 7970 6520 636f 6465  Object type code
-00002820: 2074 6f20 6669 6c74 6572 2062 7929 0272   to filter by).r
-00002830: 2300 0000 7225 0000 007a 062d 7370 6163  #...r%...z.-spac
-00002840: 657a 072d 2d73 7061 6365 7a0a 5370 6163  ez.--spacez.Spac
-00002850: 6520 636f 6465 7a08 2d70 726f 6a65 6374  e codez.-project
-00002860: 7a09 2d2d 7072 6f6a 6563 747a 2046 756c  z.--projectz Ful
-00002870: 6c20 7072 6f6a 6563 7420 6964 656e 7469  l project identi
-00002880: 6669 6361 7469 6f6e 2063 6f64 657a 0b2d  fication codez.-
-00002890: 6578 7065 7269 6d65 6e74 7a0c 2d2d 6578  experimentz.--ex
-000028a0: 7065 7269 6d65 6e74 7a14 4675 6c6c 2065  perimentz.Full e
-000028b0: 7870 6572 696d 656e 7420 636f 6465 7a05  xperiment codez.
-000028c0: 2d74 7970 657a 062d 2d74 7970 657a 0954  -typez.--typez.T
-000028d0: 7970 6520 636f 6465 7a09 2d70 726f 7065  ype codez.-prope
-000028e0: 7274 79da 0d70 726f 7065 7274 795f 636f  rty..property_co
-000028f0: 6465 7a0d 5072 6f70 6572 7479 2063 6f64  dez.Property cod
-00002900: 657a 0f2d 7072 6f70 6572 7479 2d76 616c  ez.-property-val
-00002910: 7565 da0e 7072 6f70 6572 7479 5f76 616c  ue..property_val
-00002920: 7565 7a0e 5072 6f70 6572 7479 2076 616c  uez.Property val
-00002930: 7565 7a12 2d72 6567 6973 7472 6174 696f  uez.-registratio
-00002940: 6e2d 6461 7465 7a13 2d2d 7265 6769 7374  n-datez.--regist
-00002950: 7261 7469 6f6e 2d64 6174 65da 1172 6567  ration-date..reg
-00002960: 6973 7472 6174 696f 6e5f 6461 7465 7a4d  istration_datezM
-00002970: 5265 6769 7374 7261 7469 6f6e 2064 6174  Registration dat
-00002980: 652c 2069 7420 6361 6e20 6265 2069 6e20  e, it can be in 
-00002990: 7468 6520 666f 726d 6174 2022 6f59 5959  the format "oYYY
-000029a0: 592d 4d4d 2d44 4422 2028 652e 672e 2022  Y-MM-DD" (e.g. "
-000029b0: 3e32 3032 332d 3031 2d30 3122 297a 122d  >2023-01-01")z.-
-000029c0: 6d6f 6469 6669 6361 7469 6f6e 2d64 6174  modification-dat
-000029d0: 657a 132d 2d6d 6f64 6966 6963 6174 696f  ez.--modificatio
-000029e0: 6e2d 6461 7465 da11 6d6f 6469 6669 6361  n-date..modifica
-000029f0: 7469 6f6e 5f64 6174 657a 4d4d 6f64 6966  tion_datezMModif
-00002a00: 6963 6174 696f 6e20 6461 7465 2c20 6974  ication date, it
-00002a10: 2063 616e 2062 6520 696e 2074 6865 2066   can be in the f
-00002a20: 6f72 6d61 7420 226f 5959 5959 2d4d 4d2d  ormat "oYYYY-MM-
-00002a30: 4444 2220 2865 2e67 2e20 223e 3230 3233  DD" (e.g. ">2023
-00002a40: 2d30 312d 3031 2229 7a05 2d73 6176 657a  -01-01")z.-savez
-00002a50: 062d 2d73 6176 657a 1846 696c 656e 616d  .--savez.Filenam
-00002a60: 6520 746f 2073 6176 6520 7265 7375 6c74  e to save result
-00002a70: 73da 0864 6174 615f 7365 747a 022d 707a  s..data_setz.-pz
-00002a80: 162d 2d69 735f 6461 7461 5f73 6574 5f70  .--is_data_set_p
-00002a90: 726f 7065 7274 797a 1c43 6f6e 6669 6775  ropertyz.Configu
-00002aa0: 7265 2064 6174 6120 7365 7420 7072 6f70  re data set prop
-00002ab0: 6572 7479 2e63 0300 0000 0000 0000 0000  erty.c..........
-00002ac0: 0000 0400 0000 0400 0000 4300 0000 733a  ..........C...s:
-00002ad0: 0000 0074 007c 006a 0164 0164 028d 027d  ...t.|.j.d.d...}
-00002ae0: 037c 017c 006a 0164 033c 007c 027c 006a  .|.|.j.d.<.|.|.j
-00002af0: 0164 043c 007c 037c 006a 0164 053c 0064  .d.<.|.|.j.d.<.d
-00002b00: 067c 006a 0164 073c 0064 0853 0029 097a  .|.j.d.<.d.S.).z
-00002b10: 2f20 4765 742f 7365 7420 7365 7474 696e  / Get/set settin
-00002b20: 6773 2072 656c 6174 6564 2074 6f20 7468  gs related to th
-00002b30: 6520 6461 7461 2073 6574 2e0a 2020 2020  e data set..    
-00002b40: 4672 9800 0000 7280 0000 0072 8200 0000  Fr....r....r....
-00002b50: 7230 0000 0072 b800 0000 7281 0000 004e  r0...r....r....N
-00002b60: 72a2 0000 0029 0472 2b00 0000 7280 0000  r....).r+...r...
-00002b70: 0072 8200 0000 7230 0000 0072 1200 0000  .r....r0...r....
-00002b80: 7212 0000 0072 1300 0000 72b8 0000 0022  r....r....r...."
-00002b90: 0100 0073 0a00 0000 0e08 0a01 0a01 0a01  ...s............
-00002ba0: 0e01 da11 6461 7461 5f73 6574 5f73 6574  ....data_set_set
-00002bb0: 7469 6e67 7363 0200 0000 0000 0000 0000  tingsc..........
-00002bc0: 0000 0200 0000 0600 0000 0300 0000 72a7  ..............r.
-00002bd0: 0000 0029 054e 7230 0000 00da 0c64 6174  ...).Nr0.....dat
-00002be0: 615f 7365 745f 7365 7463 0100 0000 0000  a_set_setc......
-00002bf0: 0000 0000 0000 0100 0000 0300 0000 1300  ................
-00002c00: 0000 72a9 0000 0072 1a00 0000 72aa 0000  ..r....r....r...
-00002c10: 0072 3200 0000 a902 722b 0000 0072 b900  .r2.....r+...r..
-00002c20: 0000 7212 0000 0072 1300 0000 7236 0000  ..r....r....r6..
-00002c30: 0035 0100 0072 3700 0000 7a1e 6461 7461  .5...r7...z.data
-00002c40: 5f73 6574 5f73 6574 2e3c 6c6f 6361 6c73  _set_set.<locals
-00002c50: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
-00002c60: bb00 0000 7212 0000 0072 bb00 0000 7213  ....r....r....r.
-00002c70: 0000 0072 ba00 0000 3101 0000 72ad 0000  ...r....1...r...
-00002c80: 0072 ba00 0000 6302 0000 0000 0000 0000  .r....c.........
-00002c90: 0000 0002 0000 0006 0000 0003 0000 0072  ...............r
-00002ca0: a700 0000 2905 4e72 3000 0000 da0c 6461  ....).Nr0.....da
-00002cb0: 7461 5f73 6574 5f67 6574 6301 0000 0000  ta_set_getc.....
-00002cc0: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-00002cd0: 0000 0072 a900 0000 721a 0000 0072 af00  ...r....r....r..
-00002ce0: 0000 7232 0000 0072 bb00 0000 7212 0000  ..r2...r....r...
-00002cf0: 0072 1300 0000 7236 0000 003c 0100 0072  .r....r6...<...r
-00002d00: 3700 0000 7a1e 6461 7461 5f73 6574 5f67  7...z.data_set_g
-00002d10: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  et.<locals>.<lam
-00002d20: 6264 613e 72ac 0000 0072 bb00 0000 7212  bda>r....r....r.
-00002d30: 0000 0072 bb00 0000 7213 0000 0072 bc00  ...r....r....r..
-00002d40: 0000 3801 0000 72ad 0000 0072 bc00 0000  ..8...r....r....
-00002d50: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002d60: 0006 0000 0003 0000 0072 a700 0000 2905  .........r....).
-00002d70: 4e72 3000 0000 da0e 6461 7461 5f73 6574  Nr0.....data_set
-00002d80: 5f63 6c65 6172 6301 0000 0000 0000 0000  _clearc.........
-00002d90: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-00002da0: a900 0000 721a 0000 0072 b200 0000 7232  ....r....r....r2
-00002db0: 0000 0072 bb00 0000 7212 0000 0072 1300  ...r....r....r..
-00002dc0: 0000 7236 0000 0043 0100 0072 3700 0000  ..r6...C...r7...
-00002dd0: 7a20 6461 7461 5f73 6574 5f63 6c65 6172  z data_set_clear
-00002de0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00002df0: 613e 72ac 0000 0072 bb00 0000 7212 0000  a>r....r....r...
-00002e00: 0072 bb00 0000 7213 0000 0072 bd00 0000  .r....r....r....
-00002e10: 3f01 0000 72ad 0000 0072 bd00 0000 da06  ?...r....r......
-00002e20: 7365 6172 6368 7a2f 5365 6172 6368 2066  searchz/Search f
-00002e30: 6f72 2064 6174 6173 6574 7320 7573 696e  or datasets usin
-00002e40: 6720 6120 6669 6c74 6572 696e 6720 6372  g a filtering cr
-00002e50: 6974 6572 6961 2e29 01da 0a73 686f 7274  iteria.)...short
-00002e60: 5f68 656c 7063 0a00 0000 0000 0000 0000  _helpc..........
-00002e70: 0000 0a00 0000 0a00 0000 0300 0000 73a4  ..............s.
-00002e80: 0000 0074 0064 0164 0284 007c 017c 027c  ...t.d.d...|.|.|
-00002e90: 037c 047c 057c 067c 077c 0866 0844 0083  .|.|.|.|.|.f.D..
-00002ea0: 0183 0172 1774 0164 0383 0101 0064 0453  ...r.t.d.....d.S
-00002eb0: 007c 0764 0075 0072 1f7c 0864 0075 0173  .|.d.u.r.|.d.u.s
-00002ec0: 277c 0764 0075 0172 2d7c 0864 0075 0072  '|.d.u.r-|.d.u.r
-00002ed0: 2d74 0164 0583 0101 0064 0453 0074 027c  -t.d.....d.S.t.|
-00002ee0: 006a 0364 0664 078d 027c 006a 0364 083c  .j.d.d...|.j.d.<
-00002ef0: 0074 047c 017c 027c 037c 047c 077c 057c  .t.|.|.|.|.|.|.|
-00002f00: 067c 0864 098d 0889 007c 006a 0364 0819  .|.d.....|.j.d..
-00002f10: 00a0 0564 0a87 0087 0166 0264 0b64 0c84  ...d.....f.d.d..
-00002f20: 08a1 0266 0153 0029 0d4e 6301 0000 0000  ...f.S.).Nc.....
-00002f30: 0000 0000 0000 0002 0000 0003 0000 0073  ...............s
-00002f40: 0000 00f3 1800 0000 8100 7c00 5d07 7d01  ..........|.].}.
-00002f50: 7c01 6400 7500 5600 0100 7102 6400 5300  |.d.u.V...q.d.S.
-00002f60: 721a 0000 0072 1200 0000 a902 da02 2e30  r....r.........0
-00002f70: da01 7672 1200 0000 7212 0000 0072 1300  ..vr....r....r..
-00002f80: 0000 da09 3c67 656e 6578 7072 3e4b 0100  ....<genexpr>K..
-00002f90: 00f3 0400 0000 0280 1600 7a22 6461 7461  ..........z"data
-00002fa0: 5f73 6574 5f73 6561 7263 682e 3c6c 6f63  _set_search.<loc
-00002fb0: 616c 733e 2e3c 6765 6e65 7870 723e fa31  als>.<genexpr>.1
-00002fc0: 596f 7520 6d75 7374 2070 726f 7669 6465  You must provide
-00002fd0: 2061 7420 6c65 6173 7420 6f6e 6520 6669   at least one fi
-00002fe0: 6c74 6572 696e 6720 6372 6974 6572 6961  ltering criteria
-00002ff0: 2172 3b00 0000 fa36 5072 6f70 6572 7479  !r;....6Property
-00003000: 2063 6f64 6520 616e 6420 7072 6f70 6572   code and proper
-00003010: 7479 2076 616c 7565 206e 6565 6420 746f  ty value need to
-00003020: 2062 6520 7370 6563 6966 6965 6421 4672   be specified!Fr
-00003030: 9800 0000 7230 0000 00a9 0872 b300 0000  ....r0.....r....
-00003040: da05 7370 6163 65da 0770 726f 6a65 6374  ..space..project
-00003050: da0a 6578 7065 7269 6d65 6e74 72b4 0000  ..experimentr...
-00003060: 0072 b600 0000 72b7 0000 0072 b500 0000  .r....r....r....
-00003070: da0f 6461 7461 5f73 6574 5f73 6561 7263  ..data_set_searc
-00003080: 6863 0100 0000 0000 0000 0000 0000 0100  hc..............
-00003090: 0000 0400 0000 1300 0000 f30c 0000 007c  ...............|
-000030a0: 00a0 0088 0088 01a1 0253 0072 1a00 0000  .........S.r....
-000030b0: 2901 da0f 7365 6172 6368 5f64 6174 615f  )...search_data_
-000030c0: 7365 7472 3200 0000 a902 da07 6669 6c74  setr2.......filt
-000030d0: 6572 73da 0473 6176 6572 1200 0000 7213  ers..saver....r.
-000030e0: 0000 0072 3600 0000 5a01 0000 7240 0000  ...r6...Z...r@..
-000030f0: 007a 2164 6174 615f 7365 745f 7365 6172  .z!data_set_sear
-00003100: 6368 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ch.<locals>.<lam
-00003110: 6264 613e a906 da03 616c 6c72 0800 0000  bda>....allr....
-00003120: 7209 0000 0072 2a00 0000 da04 6469 6374  r....r*.....dict
-00003130: 7238 0000 00a9 0a72 2b00 0000 72b3 0000  r8.....r+...r...
-00003140: 0072 c900 0000 72ca 0000 0072 cb00 0000  .r....r....r....
-00003150: 72b6 0000 0072 b700 0000 72b4 0000 0072  r....r....r....r
-00003160: b500 0000 72d1 0000 0072 1200 0000 72cf  ....r....r....r.
-00003170: 0000 0072 1300 0000 72cc 0000 0046 0100  ...r....r....F..
-00003180: 0073 2e00 0000 0805 0c01 0401 02ff 08ff  .s..............
-00003190: 0803 0401 1001 0601 02ff 0601 02ff 0802  ................
-000031a0: 0401 1401 0601 0601 0401 0201 06fd 0c04  ................
-000031b0: 0c01 06ff 72cc 0000 0063 0200 0000 0000  ....r....c......
-000031c0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-000031d0: 0000 72a1 0000 0029 087a 2d20 4765 742f  ..r....).z- Get/
-000031e0: 7365 7420 7365 7474 696e 6773 2072 656c  set settings rel
-000031f0: 6174 6564 2074 6f20 7468 6520 6f62 6a65  ated to the obje
-00003200: 6374 2e0a 2020 2020 4672 9800 0000 7280  ct..    Fr....r.
-00003210: 0000 0072 3000 0000 da06 6f62 6a65 6374  ...r0.....object
-00003220: 7281 0000 004e 72a2 0000 0072 a300 0000  r....Nr....r....
-00003230: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00003240: d600 0000 6001 0000 72a4 0000 0072 d600  ....`...r....r..
-00003250: 0000 da0f 6f62 6a65 6374 5f73 6574 7469  ....object_setti
-00003260: 6e67 7363 0200 0000 0000 0000 0000 0000  ngsc............
-00003270: 0200 0000 0600 0000 0300 0000 72a7 0000  ............r...
-00003280: 0029 054e 7230 0000 00da 0a6f 626a 6563  .).Nr0.....objec
-00003290: 745f 7365 7463 0100 0000 0000 0000 0000  t_setc..........
-000032a0: 0000 0100 0000 0300 0000 1300 0000 72a9  ..............r.
-000032b0: 0000 0072 1a00 0000 72aa 0000 0072 3200  ...r....r....r2.
-000032c0: 0000 a902 722b 0000 0072 d700 0000 7212  ....r+...r....r.
-000032d0: 0000 0072 1300 0000 7236 0000 0070 0100  ...r....r6...p..
-000032e0: 0072 3700 0000 7a1c 6f62 6a65 6374 5f73  .r7...z.object_s
-000032f0: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  et.<locals>.<lam
-00003300: 6264 613e 72ac 0000 0072 d900 0000 7212  bda>r....r....r.
-00003310: 0000 0072 d900 0000 7213 0000 0072 d800  ...r....r....r..
-00003320: 0000 6c01 0000 72ad 0000 0072 d800 0000  ..l...r....r....
-00003330: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00003340: 0006 0000 0003 0000 0072 a700 0000 2905  .........r....).
-00003350: 4e72 3000 0000 da0a 6f62 6a65 6374 5f67  Nr0.....object_g
-00003360: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
-00003370: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
-00003380: 721a 0000 0072 af00 0000 7232 0000 0072  r....r....r2...r
-00003390: d900 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
-000033a0: 0000 0077 0100 0072 3700 0000 7a1c 6f62  ...w...r7...z.ob
-000033b0: 6a65 6374 5f67 6574 2e3c 6c6f 6361 6c73  ject_get.<locals
-000033c0: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
-000033d0: d900 0000 7212 0000 0072 d900 0000 7213  ....r....r....r.
-000033e0: 0000 0072 da00 0000 7301 0000 72ad 0000  ...r....s...r...
-000033f0: 0072 da00 0000 6302 0000 0000 0000 0000  .r....c.........
-00003400: 0000 0002 0000 0006 0000 0003 0000 0072  ...............r
-00003410: a700 0000 2905 4e72 3000 0000 da0c 6f62  ....).Nr0.....ob
-00003420: 6a65 6374 5f63 6c65 6172 6301 0000 0000  ject_clearc.....
-00003430: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-00003440: 0000 0072 a900 0000 721a 0000 0072 b200  ...r....r....r..
-00003450: 0000 7232 0000 0072 d900 0000 7212 0000  ..r2...r....r...
-00003460: 0072 1300 0000 7236 0000 007e 0100 0072  .r....r6...~...r
-00003470: 3700 0000 7a1e 6f62 6a65 6374 5f63 6c65  7...z.object_cle
-00003480: 6172 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ar.<locals>.<lam
-00003490: 6264 613e 72ac 0000 0072 d900 0000 7212  bda>r....r....r.
-000034a0: 0000 0072 d900 0000 7213 0000 0072 db00  ...r....r....r..
-000034b0: 0000 7a01 0000 72ad 0000 0072 db00 0000  ..z...r....r....
-000034c0: 7a2e 5365 6172 6368 2066 6f72 2073 616d  z.Search for sam
-000034d0: 706c 6573 2075 7369 6e67 2061 2066 696c  ples using a fil
-000034e0: 7465 7269 6e67 2063 7269 7465 7269 612e  tering criteria.
-000034f0: 630a 0000 0000 0000 0000 0000 000a 0000  c...............
-00003500: 000a 0000 0003 0000 0073 a200 0000 7400  .........s....t.
-00003510: 6401 6402 8400 7c01 7c02 7c03 7c04 7c05  d.d...|.|.|.|.|.
-00003520: 7c06 7c07 7c08 6608 4400 8301 8301 7217  |.|.|.f.D.....r.
-00003530: 7401 6403 8301 0100 6404 5300 7c07 6400  t.d.....d.S.|.d.
-00003540: 7500 721f 7c08 6400 7501 7327 7c07 6400  u.r.|.d.u.s'|.d.
-00003550: 7501 722d 7c08 6400 7500 722d 7401 6405  u.r-|.d.u.r-t.d.
-00003560: 8301 0100 6404 5300 7402 7c00 6a03 6406  ....d.S.t.|.j.d.
-00003570: 6407 8d02 7c00 6a03 6408 3c00 7404 7c01  d...|.j.d.<.t.|.
-00003580: 7c02 7c03 7c04 7c07 7c05 7c06 7c08 6409  |.|.|.|.|.|.|.d.
-00003590: 8d08 8900 7c00 6a03 6408 1900 a005 640a  ....|.j.d.....d.
-000035a0: 8700 8701 6602 640b 640c 8408 a102 5300  ....f.d.d.....S.
-000035b0: 290d 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
-000035c0: 0200 0000 0300 0000 7300 0000 72c0 0000  ........s...r...
-000035d0: 0072 1a00 0000 7212 0000 0072 c100 0000  .r....r....r....
-000035e0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000035f0: c400 0000 8601 0000 72c5 0000 007a 206f  ........r....z o
-00003600: 626a 6563 745f 7365 6172 6368 2e3c 6c6f  bject_search.<lo
-00003610: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-00003620: c600 0000 723b 0000 0072 c700 0000 4672  ....r;...r....Fr
-00003630: 9800 0000 7230 0000 0072 c800 0000 da0d  ....r0...r......
-00003640: 6f62 6a65 6374 5f73 6561 7263 6863 0100  object_searchc..
-00003650: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00003660: 0000 1300 0000 72cd 0000 0072 1a00 0000  ......r....r....
-00003670: 2901 da0d 7365 6172 6368 5f6f 626a 6563  )...search_objec
-00003680: 7472 3200 0000 72cf 0000 0072 1200 0000  tr2...r....r....
-00003690: 7213 0000 0072 3600 0000 9501 0000 7240  r....r6.......r@
-000036a0: 0000 007a 1f6f 626a 6563 745f 7365 6172  ...z.object_sear
-000036b0: 6368 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ch.<locals>.<lam
-000036c0: 6264 613e 72d2 0000 0072 d500 0000 7212  bda>r....r....r.
-000036d0: 0000 0072 cf00 0000 7213 0000 0072 dc00  ...r....r....r..
-000036e0: 0000 8101 0000 732e 0000 0008 050c 0104  ......s.........
-000036f0: 0102 ff08 ff08 0304 0110 0106 0102 ff06  ................
-00003700: 0102 ff08 0204 0114 0106 0106 0104 0102  ................
-00003710: 0106 fd0c 040c 0104 ff72 dc00 0000 6302  .........r....c.
-00003720: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00003730: 0000 0043 0000 0072 a100 0000 2908 7a31  ...C...r....).z1
-00003740: 2047 6574 2f73 6574 2073 6574 7469 6e67   Get/set setting
-00003750: 7320 7265 6c61 7465 6420 746f 2074 6865  s related to the
-00003760: 2063 6f6c 6c65 6374 696f 6e2e 0a20 2020   collection..   
-00003770: 2046 7298 0000 0072 8000 0000 7230 0000   Fr....r....r0..
-00003780: 00da 0a63 6f6c 6c65 6374 696f 6e72 8100  ...collectionr..
-00003790: 0000 4e72 a200 0000 72a3 0000 0072 1200  ..Nr....r....r..
-000037a0: 0000 7212 0000 0072 1300 0000 72de 0000  ..r....r....r...
-000037b0: 009b 0100 0072 a400 0000 72de 0000 0063  .....r....r....c
-000037c0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-000037d0: 0600 0000 0300 0000 72a7 0000 0029 054e  ........r....).N
-000037e0: 7230 0000 00da 0e63 6f6c 6c65 6374 696f  r0.....collectio
-000037f0: 6e5f 7365 7463 0100 0000 0000 0000 0000  n_setc..........
-00003800: 0000 0100 0000 0300 0000 1300 0000 72a9  ..............r.
-00003810: 0000 0072 1a00 0000 72aa 0000 0072 3200  ...r....r....r2.
-00003820: 0000 72ab 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00003830: 0072 3600 0000 ab01 0000 7237 0000 007a  .r6.......r7...z
-00003840: 2063 6f6c 6c65 6374 696f 6e5f 7365 742e   collection_set.
-00003850: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00003860: 3e72 ac00 0000 72ab 0000 0072 1200 0000  >r....r....r....
-00003870: 72ab 0000 0072 1300 0000 72df 0000 00a7  r....r....r.....
-00003880: 0100 0072 ad00 0000 72df 0000 0063 0200  ...r....r....c..
-00003890: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000038a0: 0000 0300 0000 72a7 0000 0029 054e 7230  ......r....).Nr0
-000038b0: 0000 00da 0e63 6f6c 6c65 6374 696f 6e5f  .....collection_
-000038c0: 6765 7463 0100 0000 0000 0000 0000 0000  getc............
-000038d0: 0100 0000 0300 0000 1300 0000 72a9 0000  ............r...
-000038e0: 0072 1a00 0000 72af 0000 0072 3200 0000  .r....r....r2...
-000038f0: 72ab 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00003900: 3600 0000 b201 0000 7237 0000 007a 2063  6.......r7...z c
-00003910: 6f6c 6c65 6374 696f 6e5f 6765 742e 3c6c  ollection_get.<l
-00003920: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-00003930: ac00 0000 72ab 0000 0072 1200 0000 72ab  ....r....r....r.
-00003940: 0000 0072 1300 0000 72e0 0000 00ae 0100  ...r....r.......
-00003950: 0072 ad00 0000 72e0 0000 0063 0200 0000  .r....r....c....
-00003960: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00003970: 0300 0000 72a7 0000 0029 054e 7230 0000  ....r....).Nr0..
-00003980: 00da 1063 6f6c 6c65 6374 696f 6e5f 636c  ...collection_cl
-00003990: 6561 7263 0100 0000 0000 0000 0000 0000  earc............
-000039a0: 0100 0000 0300 0000 1300 0000 72a9 0000  ............r...
-000039b0: 0072 1a00 0000 72b2 0000 0072 3200 0000  .r....r....r2...
-000039c0: 72ab 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000039d0: 3600 0000 b901 0000 7237 0000 007a 2263  6.......r7...z"c
-000039e0: 6f6c 6c65 6374 696f 6e5f 636c 6561 722e  ollection_clear.
-000039f0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00003a00: 3e72 ac00 0000 72ab 0000 0072 1200 0000  >r....r....r....
-00003a10: 72ab 0000 0072 1300 0000 72e1 0000 00b5  r....r....r.....
-00003a20: 0100 0072 ad00 0000 72e1 0000 0063 0200  ...r....r....c..
-00003a30: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00003a40: 0000 4300 0000 734a 0000 007c 0164 0175  ..C...sJ...|.d.u
-00003a50: 0072 0d74 007c 006a 0164 0264 0164 038d  .r.t.|.j.d.d.d..
-00003a60: 037d 026e 0774 007c 006a 0164 0264 048d  .}.n.t.|.j.d.d..
-00003a70: 027d 027c 017c 006a 0164 053c 007c 027c  .}.|.|.j.d.<.|.|
-00003a80: 006a 0164 063c 0064 077c 006a 0164 083c  .j.d.<.d.|.j.d.<
-00003a90: 0064 0953 0029 0a7a 1d20 4765 742f 7365  .d.S.).z. Get/se
-00003aa0: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
-00003ab0: 2e0a 2020 2020 5446 a902 7299 0000 00da  ..    TF..r.....
-00003ac0: 0b69 735f 7068 7973 6963 616c 7298 0000  .is_physicalr...
-00003ad0: 0072 8000 0000 7230 0000 0072 8500 0000  .r....r0...r....
-00003ae0: 7281 0000 004e 72a2 0000 0072 a300 0000  r....Nr....r....
-00003af0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00003b00: 8500 0000 bf01 0000 730c 0000 0008 0612  ........s.......
-00003b10: 010e 020a 010a 010e 0172 8500 0000 6302  .........r....c.
-00003b20: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00003b30: 0000 0003 0000 0072 a700 0000 2905 4e72  .......r....).Nr
-00003b40: 3000 0000 da0a 636f 6e66 6967 5f73 6574  0.....config_set
-00003b50: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00003b60: 0003 0000 0013 0000 0072 a900 0000 721a  .........r....r.
-00003b70: 0000 0072 aa00 0000 7232 0000 0072 ab00  ...r....r2...r..
-00003b80: 0000 7212 0000 0072 1300 0000 7236 0000  ..r....r....r6..
-00003b90: 00d2 0100 0072 3700 0000 7a1c 636f 6e66  .....r7...z.conf
-00003ba0: 6967 5f73 6574 2e3c 6c6f 6361 6c73 3e2e  ig_set.<locals>.
-00003bb0: 3c6c 616d 6264 613e 72ac 0000 0072 ab00  <lambda>r....r..
-00003bc0: 0000 7212 0000 0072 ab00 0000 7213 0000  ..r....r....r...
-00003bd0: 0072 e400 0000 ce01 0000 72ad 0000 0072  .r........r....r
-00003be0: e400 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00003bf0: 0002 0000 0006 0000 0003 0000 0072 a700  .............r..
-00003c00: 0000 2905 4e72 3000 0000 da0a 636f 6e66  ..).Nr0.....conf
-00003c10: 6967 5f67 6574 6301 0000 0000 0000 0000  ig_getc.........
-00003c20: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-00003c30: a900 0000 721a 0000 0072 af00 0000 7232  ....r....r....r2
-00003c40: 0000 0072 ab00 0000 7212 0000 0072 1300  ...r....r....r..
-00003c50: 0000 7236 0000 00d9 0100 0072 3700 0000  ..r6.......r7...
-00003c60: 7a1c 636f 6e66 6967 5f67 6574 2e3c 6c6f  z.config_get.<lo
-00003c70: 6361 6c73 3e2e 3c6c 616d 6264 613e 72ac  cals>.<lambda>r.
-00003c80: 0000 0072 ab00 0000 7212 0000 0072 ab00  ...r....r....r..
-00003c90: 0000 7213 0000 0072 e500 0000 d501 0000  ..r....r........
-00003ca0: 72ad 0000 0072 e500 0000 6302 0000 0000  r....r....c.....
-00003cb0: 0000 0000 0000 0002 0000 0006 0000 0003  ................
-00003cc0: 0000 0072 a700 0000 2905 4e72 3000 0000  ...r....).Nr0...
-00003cd0: da0c 636f 6e66 6967 5f63 6c65 6172 6301  ..config_clearc.
-00003ce0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00003cf0: 0000 0013 0000 0072 a900 0000 721a 0000  .......r....r...
-00003d00: 0072 b200 0000 7232 0000 0072 ab00 0000  .r....r2...r....
-00003d10: 7212 0000 0072 1300 0000 7236 0000 00e0  r....r....r6....
-00003d20: 0100 0072 3700 0000 7a1e 636f 6e66 6967  ...r7...z.config
-00003d30: 5f63 6c65 6172 2e3c 6c6f 6361 6c73 3e2e  _clear.<locals>.
-00003d40: 3c6c 616d 6264 613e 72ac 0000 0072 ab00  <lambda>r....r..
-00003d50: 0000 7212 0000 0072 ab00 0000 7213 0000  ..r....r....r...
-00003d60: 0072 e600 0000 dc01 0000 72ad 0000 0072  .r........r....r
-00003d70: e600 0000 7a02 2d6d 7a05 2d2d 6d73 677a  ....z.-mz.--msgz
-00003d80: 0b6f 6269 7320 636f 6d6d 6974 7a23 4120  .obis commitz#A 
-00003d90: 6d65 7373 6167 6520 6578 706c 6169 6e69  message explaini
-00003da0: 6e67 2077 6861 7420 7761 7320 646f 6e65  ng what was done
-00003db0: 2e7a 022d 617a 0a2d 2d61 7574 6f5f 6164  .z.-az.--auto_ad
-00003dc0: 647a 2641 7574 6f6d 6174 6963 616c 6c79  dz&Automatically
-00003dd0: 2061 6464 2061 6c6c 2075 6e74 7261 636b   add all untrack
-00003de0: 6564 2066 696c 6573 2e7a 022d 697a 172d  ed files.z.-iz.-
-00003df0: 2d69 676e 6f72 655f 6d69 7373 696e 675f  -ignore_missing_
-00003e00: 7061 7265 6e74 7a29 4966 2070 6172 656e  parentz)If paren
-00003e10: 7420 6461 7461 2073 6574 2069 7320 6d69  t data set is mi
-00003e20: 7373 696e 672c 2069 676e 6f72 6520 6974  ssing, ignore it
-00003e30: 2e29 02da 0665 7869 7374 73da 0966 696c  .)...exists..fil
-00003e40: 655f 6f6b 6179 2902 720d 0000 00da 0872  e_okay).r......r
-00003e50: 6571 7569 7265 64da 0663 6f6d 6d69 747a  equired..commitz
-00003e60: 3043 6f6d 6d69 7420 7468 6520 7265 706f  0Commit the repo
-00003e70: 7369 746f 7279 2074 6f20 6769 7420 616e  sitory to git an
-00003e80: 6420 696e 666f 726d 206f 7065 6e42 4953  d inform openBIS
-00003e90: 2e63 0500 0000 0000 0000 0000 0000 0500  .c..............
-00003ea0: 0000 0600 0000 0300 0000 7320 0000 007c  ..........s ...|
-00003eb0: 006a 0064 0119 00a0 0164 0287 0087 0187  .j.d.....d......
-00003ec0: 0266 0364 0364 0484 087c 04a1 0353 0029  .f.d.d...|...S.)
-00003ed0: 054e 7230 0000 0072 ea00 0000 6301 0000  .Nr0...r....c...
-00003ee0: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00003ef0: 0013 0000 00f3 0e00 0000 7c00 a000 8802  ..........|.....
-00003f00: 8800 8801 a103 5300 721a 0000 0029 0172  ......S.r....).r
-00003f10: ea00 0000 7232 0000 00a9 03da 0861 7574  ....r2.......aut
-00003f20: 6f5f 6164 64da 1569 676e 6f72 655f 6d69  o_add..ignore_mi
-00003f30: 7373 696e 675f 7061 7265 6e74 da03 6d73  ssing_parent..ms
-00003f40: 6772 1200 0000 7213 0000 0072 3600 0000  gr....r....r6...
-00003f50: f801 0000 f302 0000 000e 007a 2372 6570  ...........z#rep
-00003f60: 6f73 6974 6f72 795f 636f 6d6d 6974 2e3c  ository_commit.<
-00003f70: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-00003f80: 72ac 0000 00a9 0572 2b00 0000 72ef 0000  r......r+...r...
-00003f90: 0072 ed00 0000 72ee 0000 0072 3900 0000  .r....r....r9...
-00003fa0: 7212 0000 0072 ec00 0000 7213 0000 00da  r....r....r.....
-00003fb0: 1172 6570 6f73 6974 6f72 795f 636f 6d6d  .repository_comm
-00003fc0: 6974 f301 0000 7308 0000 000c 040e 0102  it....s.........
-00003fd0: 0104 fe72 f200 0000 6305 0000 0000 0000  ...r....c.......
-00003fe0: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
-00003ff0: 00f3 2c00 0000 7400 7c00 6a01 6401 6402  ..,...t.|.j.d.d.
-00004000: 8d02 7c00 6a01 6403 3c00 7c00 6a02 7403  ..|.j.d.<.|.j.t.
-00004010: 7c01 7c02 7c03 7c04 6404 8d05 0100 6400  |.|.|.|.d.....d.
-00004020: 5300 2905 4e46 7298 0000 0072 3000 0000  S.).NFr....r0...
-00004030: 2904 72ef 0000 0072 ed00 0000 72ee 0000  ).r....r....r...
-00004040: 0072 3900 0000 2904 7209 0000 0072 2a00  .r9...).r....r*.
-00004050: 0000 da06 696e 766f 6b65 72f2 0000 0072  ....invoker....r
-00004060: f100 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00004070: 0000 0072 ea00 0000 fc01 0000 f308 0000  ...r............
-00004080: 0014 040a 0104 010a ffda 0f72 6570 6f73  ...........repos
-00004090: 6974 6f72 795f 7061 7468 723e 0000 0072  itory_pathr>...r
-000040a0: 2f00 0000 2901 7223 0000 00da 0469 6e69  /...).r#.....ini
-000040b0: 747a 2b49 6e69 7469 616c 697a 6520 7468  tz+Initialize th
-000040c0: 6520 666f 6c64 6572 2061 7320 6120 6461  e folder as a da
-000040d0: 7461 2072 6570 6f73 6974 6f72 792e 6303  ta repository.c.
-000040e0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000040f0: 0000 0043 0000 0073 0c00 0000 7400 7c00  ...C...s....t.|.
-00004100: 7c01 7c02 8303 5300 721a 0000 0029 0172  |.|...S.r....).r
-00004110: 3a00 0000 2903 722b 0000 0072 f600 0000  :...).r+...r....
-00004120: 723e 0000 0072 1200 0000 7212 0000 0072  r>...r....r....r
-00004130: 1300 0000 da0f 7265 706f 7369 746f 7279  ......repository
-00004140: 5f69 6e69 7410 0200 0073 0200 0000 0c04  _init....s......
-00004150: 72f8 0000 007a 0a2d 2d70 6879 7369 6361  r....z.--physica
-00004160: 6c72 e300 0000 6304 0000 0000 0000 0000  lr....c.........
-00004170: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
-00004180: 2a00 0000 7400 7c00 6a01 6401 7c03 6402  *...t.|.j.d.|.d.
-00004190: 8d03 7c00 6a01 6403 3c00 7c00 6a02 7403  ..|.j.d.<.|.j.t.
-000041a0: 7c01 7c02 6404 8d03 0100 6400 5300 2905  |.|.d.....d.S.).
-000041b0: 4e46 72e2 0000 0072 3000 0000 2902 72f6  NFr....r0...).r.
-000041c0: 0000 0072 3e00 0000 2904 7209 0000 0072  ...r>...).r....r
-000041d0: 2a00 0000 72f4 0000 0072 f800 0000 2904  *...r....r....).
-000041e0: 722b 0000 0072 f600 0000 723e 0000 0072  r+...r....r>...r
-000041f0: e300 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00004200: 0000 0072 f700 0000 1d02 0000 7304 0000  ...r........s...
-00004210: 0016 0414 017a 082d 2d70 6172 656e 7429  .....z.--parent)
-00004220: 0172 0d00 0000 723c 0000 007a 2c49 6e69  .r....r<...z,Ini
-00004230: 7469 616c 697a 6520 7468 6520 666f 6c64  tialize the fold
-00004240: 6572 2061 7320 616e 2061 6e61 6c79 7369  er as an analysi
-00004250: 7320 666f 6c64 6572 2e63 0400 0000 0000  s folder.c......
-00004260: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00004270: 0000 730e 0000 0074 007c 007c 017c 027c  ..s....t.|.|.|.|
-00004280: 0383 0453 0072 1a00 0000 2901 7249 0000  ...S.r....).rI..
-00004290: 00a9 0472 2b00 0000 723f 0000 0072 f600  ...r+...r?...r..
-000042a0: 0000 723e 0000 0072 1200 0000 7212 0000  ..r>...r....r...
-000042b0: 0072 1300 0000 da18 7265 706f 7369 746f  .r......reposito
-000042c0: 7279 5f69 6e69 745f 616e 616c 7973 6973  ry_init_analysis
-000042d0: 2f02 0000 7302 0000 000e 0472 fa00 0000  /...s......r....
-000042e0: 2902 7263 0000 0072 bf00 0000 6304 0000  ).rc...r....c...
-000042f0: 0000 0000 0000 0000 0004 0000 0006 0000  ................
-00004300: 0043 0000 0073 2a00 0000 7400 7c00 6a01  .C...s*...t.|.j.
-00004310: 6401 6402 8d02 7c00 6a01 6403 3c00 7c00  d.d...|.j.d.<.|.
-00004320: 6a02 7403 7c01 7c02 7c03 6404 8d04 0100  j.t.|.|.|.d.....
-00004330: 6400 5300 2905 4e46 7298 0000 0072 3000  d.S.).NFr....r0.
-00004340: 0000 2903 723f 0000 0072 f600 0000 723e  ..).r?...r....r>
-00004350: 0000 0029 0472 0900 0000 722a 0000 0072  ...).r....r*...r
-00004360: f400 0000 72fa 0000 0072 f900 0000 7212  ....r....r....r.
-00004370: 0000 0072 1200 0000 7213 0000 0072 3c00  ...r....r....r<.
-00004380: 0000 3602 0000 7308 0000 0014 0408 0104  ..6...s.........
-00004390: 010a ffda 0673 7461 7475 737a 2653 686f  .....statusz&Sho
-000043a0: 7720 7468 6520 7374 6174 6520 6f66 2074  w the state of t
-000043b0: 6865 206f 6269 7320 7265 706f 7369 746f  he obis reposito
-000043c0: 7279 2e63 0200 0000 0000 0000 0000 0000  ry.c............
-000043d0: 0200 0000 0500 0000 4300 0000 f318 0000  ........C.......
-000043e0: 007c 006a 0064 0119 00a0 0164 0264 0364  .|.j.d.....d.d.d
-000043f0: 0484 007c 01a1 0353 0029 054e 7230 0000  ...|...S.).Nr0..
-00004400: 00da 1172 6570 6f73 6974 6f72 795f 7374  ...repository_st
-00004410: 6174 7573 6301 0000 0000 0000 0000 0000  atusc...........
-00004420: 0001 0000 0002 0000 0053 0000 00f3 0800  .........S......
-00004430: 0000 7c00 a000 a100 5300 721a 0000 0029  ..|.....S.r....)
-00004440: 0172 fb00 0000 7232 0000 0072 1200 0000  .r....r2...r....
-00004450: 7212 0000 0072 1300 0000 7236 0000 004c  r....r....r6...L
-00004460: 0200 00f3 0200 0000 0800 7a23 7265 706f  ..........z#repo
-00004470: 7369 746f 7279 5f73 7461 7475 732e 3c6c  sitory_status.<l
-00004480: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-00004490: ac00 0000 a902 722b 0000 0072 3900 0000  ......r+...r9...
-000044a0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000044b0: fd00 0000 4802 0000 f302 0000 0018 0472  ....H..........r
-000044c0: fd00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-000044d0: 0002 0000 0004 0000 0043 0000 00f3 2600  .........C....&.
-000044e0: 0000 7400 7c00 6a01 6401 6402 8d02 7c00  ..t.|.j.d.d...|.
-000044f0: 6a01 6403 3c00 7c00 6a02 7403 7c01 6404  j.d.<.|.j.t.|.d.
-00004500: 8d02 0100 6400 5300 a905 4e46 7298 0000  ....d.S...NFr...
-00004510: 0072 3000 0000 2901 7239 0000 0029 0472  .r0...).r9...).r
-00004520: 0900 0000 722a 0000 0072 f400 0000 72fd  ....r*...r....r.
-00004530: 0000 0072 0001 0000 7212 0000 0072 1200  ...r....r....r..
-00004540: 0000 7213 0000 0072 fb00 0000 4f02 0000  ..r....r....O...
-00004550: f304 0000 0014 0412 0163 0200 0000 0000  .........c......
-00004560: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00004570: 0000 730e 0000 007c 017c 005f 007c 00a0  ..s....|.|._.|..
-00004580: 01a1 0053 0072 1a00 0000 2902 72ee 0000  ...S.r....).r...
-00004590: 00da 0473 796e 6329 0272 3300 0000 72ee  ...sync).r3...r.
-000045a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-000045b0: 0000 da10 5f72 6570 6f73 6974 6f72 795f  ...._repository_
-000045c0: 7379 6e63 6202 0000 7304 0000 0006 0108  syncb...s.......
-000045d0: 0172 0601 0000 7205 0100 007a 2153 796e  .r....r....z!Syn
-000045e0: 6320 7468 6520 7265 706f 7369 746f 7279  c the repository
-000045f0: 2077 6974 6820 6f70 656e 4249 532e 6303   with openBIS.c.
-00004600: 0000 0000 0000 0000 0000 0003 0000 0006  ................
-00004610: 0000 0003 0000 0073 1c00 0000 7c00 6a00  .......s....|.j.
-00004620: 6401 1900 a001 6402 8700 6601 6403 6404  d.....d...f.d.d.
-00004630: 8408 7c02 a103 5300 2905 4e72 3000 0000  ..|...S.).Nr0...
-00004640: 7205 0100 0063 0100 0000 0000 0000 0000  r....c..........
-00004650: 0000 0100 0000 0300 0000 1300 0000 730a  ..............s.
-00004660: 0000 0074 007c 0088 0083 0253 0072 1a00  ...t.|.....S.r..
-00004670: 0000 2901 7206 0100 0072 3200 0000 a901  ..).r....r2.....
-00004680: 72ee 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00004690: 3600 0000 6b02 0000 7237 0000 007a 2172  6...k...r7...z!r
-000046a0: 6570 6f73 6974 6f72 795f 7379 6e63 2e3c  epository_sync.<
-000046b0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-000046c0: 72ac 0000 00a9 0372 2b00 0000 72ee 0000  r......r+...r...
-000046d0: 0072 3900 0000 7212 0000 0072 0701 0000  .r9...r....r....
-000046e0: 7213 0000 00da 0f72 6570 6f73 6974 6f72  r......repositor
-000046f0: 795f 7379 6e63 6702 0000 7306 0000 0016  y_syncg...s.....
-00004700: 0402 0104 ff72 0901 0000 6303 0000 0000  .....r....c.....
-00004710: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-00004720: 0000 00f3 2800 0000 7400 7c00 6a01 6401  ....(...t.|.j.d.
-00004730: 6402 8d02 7c00 6a01 6403 3c00 7c00 6a02  d...|.j.d.<.|.j.
-00004740: 7403 7c01 7c02 6404 8d03 0100 6400 5300  t.|.|.d.....d.S.
-00004750: 2905 4e46 7298 0000 0072 3000 0000 2902  ).NFr....r0...).
-00004760: 72ee 0000 0072 3900 0000 2904 7209 0000  r....r9...).r...
-00004770: 0072 2a00 0000 72f4 0000 0072 0901 0000  .r*...r....r....
-00004780: 7208 0100 0072 1200 0000 7212 0000 0072  r....r....r....r
-00004790: 1300 0000 7205 0100 006f 0200 0073 0800  ....r....o...s..
-000047a0: 0000 1404 0601 0401 0aff 7a1b 6372 6561  ..........z.crea
-000047b0: 7465 2f73 686f 7720 6120 6f70 656e 4249  te/show a openBI
-000047c0: 5320 746f 6b65 6e63 0100 0000 0000 0000  S tokenc........
-000047d0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000047e0: 7304 0000 0064 0053 0072 1a00 0000 7212  s....d.S.r....r.
-000047f0: 0000 0029 0172 2b00 0000 7212 0000 0072  ...).r+...r....r
-00004800: 1200 0000 7213 0000 00da 0574 6f6b 656e  ....r......token
-00004810: 7802 0000 7302 0000 0004 0372 0b01 0000  x...s......r....
-00004820: 7a36 4765 7420 6578 6973 7469 6e67 2070  z6Get existing p
-00004830: 6572 736f 6e61 6c20 6163 6365 7373 2074  ersonal access t
-00004840: 6f6b 656e 206f 7220 6372 6561 7465 2061  oken or create a
-00004850: 206e 6577 206f 6e65 7a0c 7365 7373 696f   new onez.sessio
-00004860: 6e2d 6e61 6d65 2901 72e9 0000 007a 0f2d  n-name).r....z.-
-00004870: 2d76 616c 6964 6974 792d 6461 7973 7a21  -validity-daysz!
-00004880: 4e75 6d62 6572 206f 6620 6461 7973 2074  Number of days t
-00004890: 6865 2074 6f6b 656e 2069 7320 7661 6c69  he token is vali
-000048a0: 6429 0172 2500 0000 7a10 2d2d 7661 6c69  d).r%...z.--vali
-000048b0: 6469 7479 2d77 6565 6b73 7a22 4e75 6d62  dity-weeksz"Numb
-000048c0: 6572 206f 6620 7765 656b 7320 7468 6520  er of weeks the 
-000048d0: 746f 6b65 6e20 6973 2076 616c 6964 7a11  token is validz.
-000048e0: 2d2d 7661 6c69 6469 7479 2d6d 6f6e 7468  --validity-month
-000048f0: 737a 234e 756d 6265 7220 6f66 206d 6f6e  sz#Number of mon
-00004900: 7468 7320 7468 6520 746f 6b65 6e20 6973  ths the token is
-00004910: 2076 616c 6964 6302 0000 0000 0000 0000   validc.........
-00004920: 0000 000e 0000 000a 0000 000b 0000 0073  ...............s
-00004930: e801 0000 7400 8800 6a01 6401 6402 8d02  ....t...j.d.d...
-00004940: 7d03 7c03 a002 a100 8901 7c01 7313 8801  }.|.......|.s...
-00004950: 6403 1900 6404 1900 7d01 7c01 721f 7403  d...d...}.|.r.t.
-00004960: a004 6405 7c01 9b00 6406 9d03 a101 0100  ..d.|...d.......
-00004970: 6e05 7403 a005 6407 a101 7d01 8801 6403  n.t...d...}...d.
-00004980: 1900 6408 1900 7d04 7c04 7331 7403 a005  ..d...}.|.s1t...
-00004990: 6409 a101 7d04 8801 6403 1900 640a 1900  d...}...d...d...
-000049a0: 7d05 7c05 7341 7403 a005 640b 7c04 9b00  }.|.sAt...d.|...
-000049b0: 9d02 a101 7d05 7403 6a05 640c 7c05 9b00  ....}.t.j.d.|...
-000049c0: 640d 7c04 9b00 9d04 640e 640f 8d02 7d06  d.|.....d.d...}.
-000049d0: 7406 7c04 8801 6403 1900 a007 6410 640e  t.|...d.....d.d.
-000049e0: a102 6411 8d02 7d07 7a08 7c07 a008 7c05  ..d...}.z.|...|.
-000049f0: 7c06 a102 0100 5700 6e16 0400 7409 740a  |.....W.n...t.t.
-00004a00: 6602 7978 0100 7d08 0100 7a08 7403 a00b  f.yx..}...z.t...
-00004a10: 6412 7c08 9b00 9d02 a101 8201 6400 7d08  d.|.........d.}.
-00004a20: 7e08 7701 7700 740c a00d a100 7d09 7c02  ~.w.w.t.....}.|.
-00004a30: a007 6413 a101 728f 7c09 740e 740f 7c02  ..d...r.|.t.t.|.
-00004a40: a007 6413 a101 8301 6414 8d01 1700 7d0a  ..d.....d.....}.
-00004a50: 6e32 7c02 a007 6415 a101 72a1 7c09 740e  n2|...d...r.|.t.
-00004a60: 740f 7c02 a007 6415 a101 8301 6416 8d01  t.|...d.....d...
-00004a70: 1700 7d0a 6e20 7c02 a007 6417 a101 72b3  ..}.n |...d...r.
-00004a80: 7c09 740e 740f 7c02 a007 6417 a101 8301  |.t.t.|...d.....
-00004a90: 6418 8d01 1700 7d0a 6e0e 7c07 a010 a100  d.....}.n.|.....
-00004aa0: 7d0b 7c0b 6a11 7d0c 7c09 740e 7c0c 6419  }.|.j.}.|.t.|.d.
-00004ab0: 8d01 1700 7d0a 7c07 6a12 7c01 7c09 7c0a  ....}.|.j.|.|.|.
-00004ac0: 641a 8d03 7d0d 640a 7c05 6901 6408 7c04  d...}.d.|.i.d.|.
-00004ad0: 6901 641b 7c0d 6a13 6901 6404 7c01 6901  i.d.|.j.i.d.|.i.
-00004ae0: 6604 8901 6401 8800 6a01 641c 3c00 7c03  f...d...j.d.<.|.
-00004af0: 8800 6a01 641d 3c00 6403 8800 6a01 641e  ..j.d.<.d...j.d.
-00004b00: 3c00 7c03 a014 641f 8700 8701 6602 6420  <.|...d.....f.d 
-00004b10: 6421 8408 a102 0100 6400 5300 2922 4e46  d!......d.S.)"NF
-00004b20: 7298 0000 0072 8500 0000 da0c 7365 7373  r....r......sess
-00004b30: 696f 6e5f 6e61 6d65 7528 0000 0047 6574  ion_nameu(...Get
-00004b40: 2070 6572 736f 6e61 6c20 6163 6365 7373   personal access
-00004b50: 2074 6f6b 656e 2066 6f72 2073 6573 7369   token for sessi
-00004b60: 6f6e 20c2 abf5 0200 0000 c2bb 7a1b 506c  on .........z.Pl
-00004b70: 6561 7365 2065 6e74 6572 2061 2073 6573  ease enter a ses
-00004b80: 7369 6f6e 206e 616d 65da 0b6f 7065 6e62  sion name..openb
-00004b90: 6973 5f75 726c 7a1c 506c 6561 7365 2065  is_urlz.Please e
-00004ba0: 6e74 6572 2074 6865 206f 7065 6e42 4953  nter the openBIS
-00004bb0: 2055 524c da04 7573 6572 7a1a 506c 6561   URL..userz.Plea
-00004bc0: 7365 2065 6e74 6572 2075 7365 726e 616d  se enter usernam
-00004bd0: 6520 666f 7220 7a0d 5061 7373 776f 7264  e for z.Password
-00004be0: 2066 6f72 20fa 0140 5429 01da 0a68 6964   for ..@T)...hid
-00004bf0: 655f 696e 7075 7472 2700 0000 2901 7227  e_inputr'...).r'
-00004c00: 0000 007a 1b43 616e 6e6f 7420 636f 6e6e  ...z.Cannot conn
-00004c10: 6563 7420 746f 206f 7065 6e42 4953 3a20  ect to openBIS: 
-00004c20: da0f 7661 6c69 6469 7479 5f6d 6f6e 7468  ..validity_month
-00004c30: 7329 01da 066d 6f6e 7468 73da 0e76 616c  s)...months..val
-00004c40: 6964 6974 795f 7765 656b 7329 01da 0577  idity_weeks)...w
-00004c50: 6565 6b73 da0d 7661 6c69 6469 7479 5f64  eeks..validity_d
-00004c60: 6179 7329 01da 0464 6179 7329 01da 0773  ays)...days)...s
-00004c70: 6563 6f6e 6473 2903 da0b 7365 7373 696f  econds)...sessio
-00004c80: 6e4e 616d 65da 0976 616c 6964 4672 6f6d  nName..validFrom
-00004c90: da07 7661 6c69 6454 6fda 0d6f 7065 6e62  ..validTo..openb
-00004ca0: 6973 5f74 6f6b 656e 7280 0000 0072 3000  is_tokenr....r0.
-00004cb0: 0000 7281 0000 0072 e400 0000 6301 0000  ..r....r....c...
-00004cc0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00004cd0: 0013 0000 0072 a900 0000 721a 0000 0072  .....r....r....r
-00004ce0: aa00 0000 7232 0000 0072 ab00 0000 7212  ....r2...r....r.
-00004cf0: 0000 0072 1300 0000 7236 0000 00b8 0200  ...r....r6......
-00004d00: 0072 3700 0000 7a1b 6e65 775f 746f 6b65  .r7...z.new_toke
-00004d10: 6e2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  n.<locals>.<lamb
-00004d20: 6461 3e29 1572 0900 0000 722a 0000 0072  da>).r....r*...r
-00004d30: 9d00 0000 7216 0000 0072 1700 0000 da06  ....r....r......
-00004d40: 7072 6f6d 7074 7204 0000 0072 9700 0000  promptr....r....
-00004d50: da05 6c6f 6769 6e72 0500 0000 da0a 5661  ..loginr......Va
-00004d60: 6c75 6545 7272 6f72 da0e 436c 6963 6b45  lueError..ClickE
-00004d70: 7863 6570 7469 6f6e 7202 0000 00da 036e  xceptionr......n
-00004d80: 6f77 7203 0000 00da 0369 6e74 da16 6765  owr......int..ge
-00004d90: 745f 7365 7276 6572 5f69 6e66 6f72 6d61  t_server_informa
-00004da0: 7469 6f6e da2a 7065 7273 6f6e 616c 5f61  tion.*personal_a
-00004db0: 6363 6573 735f 746f 6b65 6e73 5f6d 6178  ccess_tokens_max
-00004dc0: 5f76 616c 6964 6974 795f 7065 7269 6f64  _validity_period
-00004dd0: da23 6765 745f 6f72 5f63 7265 6174 655f  .#get_or_create_
-00004de0: 7065 7273 6f6e 616c 5f61 6363 6573 735f  personal_access_
-00004df0: 746f 6b65 6eda 0670 6572 6d49 6472 3800  token..permIdr8.
-00004e00: 0000 290e 722b 0000 0072 0c01 0000 da06  ..).r+...r......
-00004e10: 6b77 6172 6773 7230 0000 00da 0375 726c  kwargsr0.....url
-00004e20: da08 7573 6572 6e61 6d65 da08 7061 7373  ..username..pass
-00004e30: 776f 7264 da01 6fda 0365 7863 721a 0100  word..o..excr...
-00004e40: 0072 1b01 0000 da0a 7365 7276 6572 696e  .r......serverin
-00004e50: 666f 7218 0100 00da 0974 6f6b 656e 5f6f  for......token_o
-00004e60: 626a 7212 0000 0072 ab00 0000 7213 0000  bjr....r....r...
-00004e70: 00da 096e 6577 5f74 6f6b 656e 7e02 0000  ...new_token~...
-00004e80: 7366 0000 000e 0708 0104 020c 0104 0114  sf..............
-00004e90: 010a 020c 0204 010a 010c 0204 0110 011a  ................
-00004ea0: 010c 0104 0108 ff02 0210 0112 0110 0108  ................
-00004eb0: 8002 ff08 030a 0102 0112 0106 ff0a 0202  ................
-00004ec0: 0112 0106 ff0a 0202 0112 0106 ff08 0306  ................
-00004ed0: 010e 0104 0106 0106 ff06 0306 0108 0106  ................
-00004ee0: 0104 fc0a 070a 010a 011a 0172 2f01 0000  ...........r/...
-00004ef0: da06 6164 6472 6566 7a33 4164 6420 7468  ..addrefz3Add th
-00004f00: 6520 6769 7665 6e20 7265 706f 7369 746f  e given reposito
-00004f10: 7279 2061 7320 6120 7265 6665 7265 6e63  ry as a referenc
-00004f20: 6520 746f 206f 7065 6e42 4953 2e63 0200  e to openBIS.c..
-00004f30: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00004f40: 0000 4300 0000 72fc 0000 0029 054e 7230  ..C...r....).Nr0
-00004f50: 0000 0072 3001 0000 6301 0000 0000 0000  ...r0...c.......
-00004f60: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00004f70: 0072 fe00 0000 721a 0000 0029 0172 3001  .r....r....).r0.
-00004f80: 0000 7232 0000 0072 1200 0000 7212 0000  ..r2...r....r...
-00004f90: 0072 1300 0000 7236 0000 00c5 0200 0072  .r....r6.......r
-00004fa0: ff00 0000 7a23 7265 706f 7369 746f 7279  ....z#repository
-00004fb0: 5f61 6464 7265 662e 3c6c 6f63 616c 733e  _addref.<locals>
-00004fc0: 2e3c 6c61 6d62 6461 3e72 ac00 0000 7200  .<lambda>r....r.
-00004fd0: 0100 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00004fe0: 0000 da11 7265 706f 7369 746f 7279 5f61  ....repository_a
-00004ff0: 6464 7265 66c1 0200 0072 0101 0000 7231  ddref....r....r1
-00005000: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
-00005010: 0200 0000 0400 0000 4300 0000 7202 0100  ........C...r...
-00005020: 0072 0301 0000 2904 7209 0000 0072 2a00  .r....).r....r*.
-00005030: 0000 72f4 0000 0072 3101 0000 7200 0100  ..r....r1...r...
-00005040: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00005050: 7230 0100 00c8 0200 0072 0401 0000 7a0d  r0.......r....z.
-00005060: 2d2d 6461 7461 5f73 6574 5f69 647a 4b52  --data_set_idzKR
-00005070: 656d 6f76 6520 7265 6620 6279 2064 6174  emove ref by dat
-00005080: 6120 7365 7420 6964 2c20 696e 2063 6173  a set id, in cas
-00005090: 6520 7468 6520 7265 706f 7369 746f 7279  e the repository
-000050a0: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
-000050b0: 6520 616e 796d 6f72 652e da09 7265 6d6f  e anymore...remo
-000050c0: 7665 7265 667a 3a52 656d 6f76 6520 7468  verefz:Remove th
-000050d0: 6520 7265 6665 7265 6e63 6520 746f 2074  e reference to t
-000050e0: 6865 2067 6976 656e 2072 6570 6f73 6974  he given reposit
-000050f0: 6f72 7920 6672 6f6d 206f 7065 6e42 4953  ory from openBIS
-00005100: 2e63 0300 0000 0000 0000 0000 0000 0300  .c..............
-00005110: 0000 0600 0000 0300 0000 7338 0000 0088  ..........s8....
-00005120: 0064 0075 0172 0e7c 0264 0075 0172 0e74  .d.u.r.|.d.u.r.t
-00005130: 0064 0183 0101 0064 0253 007c 006a 0164  .d.....d.S.|.j.d
-00005140: 0319 00a0 0264 0487 0066 0164 0564 0684  .....d...f.d.d..
-00005150: 087c 02a1 0353 0029 074e 7a2f 4f6e 6c79  .|...S.).Nz/Only
-00005160: 2070 726f 7669 6465 2074 6865 2064 6174   provide the dat
-00005170: 615f 7365 7420 6964 204f 5220 7468 6520  a_set id OR the 
-00005180: 7265 706f 7369 746f 7279 2e72 3b00 0000  repository.r;...
-00005190: 7230 0000 0072 3201 0000 6301 0000 0000  r0...r2...c.....
-000051a0: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-000051b0: 0000 0073 0c00 0000 7c00 6a00 8800 6401  ...s....|.j...d.
-000051c0: 8d01 5300 2902 4ea9 01da 0b64 6174 615f  ..S.).N....data_
-000051d0: 7365 745f 6964 2901 7232 0100 0072 3200  set_id).r2...r2.
-000051e0: 0000 7233 0100 0072 1200 0000 7213 0000  ..r3...r....r...
-000051f0: 0072 3600 0000 e302 0000 7240 0000 007a  .r6.......r@...z
-00005200: 2672 6570 6f73 6974 6f72 795f 7265 6d6f  &repository_remo
-00005210: 7665 7265 662e 3c6c 6f63 616c 733e 2e3c  veref.<locals>.<
-00005220: 6c61 6d62 6461 3e29 0372 0800 0000 722a  lambda>).r....r*
-00005230: 0000 0072 3800 0000 a903 722b 0000 0072  ...r8.....r+...r
-00005240: 3401 0000 7239 0000 0072 1200 0000 7233  4...r9...r....r3
-00005250: 0100 0072 1300 0000 da14 7265 706f 7369  ...r......reposi
-00005260: 746f 7279 5f72 656d 6f76 6572 6566 db02  tory_removeref..
-00005270: 0000 730c 0000 0010 0508 0104 0116 0102  ..s.............
-00005280: 0104 ff72 3601 0000 6303 0000 0000 0000  ...r6...c.......
-00005290: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-000052a0: 0072 0a01 0000 2905 4e46 7298 0000 0072  .r....).NFr....r
-000052b0: 3000 0000 2902 7234 0100 0072 3900 0000  0...).r4...r9...
-000052c0: 2904 7209 0000 0072 2a00 0000 72f4 0000  ).r....r*...r...
-000052d0: 0072 3601 0000 7235 0100 0072 1200 0000  .r6...r5...r....
-000052e0: 7212 0000 0072 1300 0000 7232 0100 00e7  r....r....r2....
-000052f0: 0200 0073 0800 0000 1404 0801 0201 0aff  ...s............
-00005300: 7234 0100 007a 0a2d 6672 6f6d 2d66 696c  r4...z.-from-fil
-00005310: 657a 0b2d 2d66 726f 6d2d 6669 6c65 da09  ez.--from-file..
-00005320: 6672 6f6d 5f66 696c 657a 6a41 6e20 6f75  from_filezjAn ou
-00005330: 7470 7574 202e 4353 5620 6669 6c65 2066  tput .CSV file f
-00005340: 726f 6d20 606f 6269 7320 6461 7461 5f73  rom `obis data_s
-00005350: 6574 2073 6561 7263 6860 2063 6f6d 6d61  et search` comma
-00005360: 6e64 2077 6974 6820 7468 6520 6c69 7374  nd with the list
-00005370: 206f 6620 6f62 6a65 6374 7320 746f 2064   of objects to d
-00005380: 6f77 6e6c 6f61 6420 6461 7461 7365 7473  ownload datasets
-00005390: 2066 726f 6d7a 022d 667a 062d 2d66 696c   fromz.-fz.--fil
-000053a0: 65da 0466 696c 657a 4046 696c 6520 696e  e..filez@File in
-000053b0: 2074 6865 2064 6174 6120 7365 7420 746f   the data set to
-000053c0: 2064 6f77 6e6c 6f61 6420 2d20 646f 776e   download - down
-000053d0: 6c6f 6164 696e 6720 616c 6c20 6966 206e  loading all if n
-000053e0: 6f74 2067 6976 656e 2e7a 162d 2d73 6b69  ot given.z.--ski
-000053f0: 705f 696e 7465 6772 6974 795f 6368 6563  p_integrity_chec
-00005400: 6b7a 3046 6c61 6720 746f 2073 6b69 7020  kz0Flag to skip 
-00005410: 6669 6c65 2069 6e74 6567 7269 7479 2063  file integrity c
-00005420: 6865 636b 2077 6974 6820 6368 6563 6b73  heck with checks
-00005430: 756d 73da 0864 6f77 6e6c 6f61 647a 1d44  ums..downloadz.D
-00005440: 6f77 6e6c 6f61 6420 6669 6c65 7320 6f66  ownload files of
-00005450: 2061 2064 6174 6120 7365 742e 6305 0000   a data set.c...
-00005460: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-00005470: 0003 0000 0073 6000 0000 8800 6401 7500  .....s`.....d.u.
-00005480: 7208 8802 6401 7500 7310 8800 6401 7501  r...d.u.s...d.u.
-00005490: 7216 8802 6401 7501 7216 7400 6402 8301  r...d.u.r.t.d...
-000054a0: 0100 6403 5300 7401 7c00 6a02 6404 6405  ..d.S.t.|.j.d.d.
-000054b0: 8d02 7c00 6a02 6406 3c00 7c00 6a02 6406  ..|.j.d.<.|.j.d.
-000054c0: 1900 a003 6407 8700 8701 8702 8703 6604  ....d.........f.
-000054d0: 6408 6409 8408 a102 5300 290a 7a76 2044  d.d.....S.).zv D
-000054e0: 6f77 6e6c 6f61 6473 2064 6174 6173 6574  ownloads dataset
-000054f0: 2066 696c 6573 2066 726f 6d20 4f70 656e   files from Open
-00005500: 4249 5320 696e 7374 616e 6365 2e0a 0a20  BIS instance... 
-00005510: 2020 2044 4154 415f 5345 5420 2020 2055     DATA_SET    U
-00005520: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
-00005530: 206f 6620 6461 7461 7365 7420 7769 7468   of dataset with
-00005540: 696e 204f 7065 6e42 4953 2069 6e73 7461  in OpenBIS insta
-00005550: 6e63 652e 4e7a 2e27 6461 7461 5f73 6574  nce.Nz.'data_set
-00005560: 5f69 6427 206f 7220 2766 726f 6d5f 6669  _id' or 'from_fi
-00005570: 6c65 2720 6d75 7374 2062 6520 7072 6f76  le' must be prov
-00005580: 6964 6564 2172 3b00 0000 4672 9800 0000  ided!r;...Fr....
-00005590: 7230 0000 0072 3901 0000 6301 0000 0000  r0...r9...c.....
-000055a0: 0000 0000 0000 0001 0000 0006 0000 0013  ................
-000055b0: 0000 0073 1200 0000 7c00 6a00 8800 8802  ...s....|.j.....
-000055c0: 8801 8803 6401 8d04 5300 2902 4e29 0472  ....d...S.).N).r
-000055d0: 3401 0000 7237 0100 0072 3801 0000 da14  4...r7...r8.....
-000055e0: 736b 6970 5f69 6e74 6567 7269 7479 5f63  skip_integrity_c
-000055f0: 6865 636b 2901 7239 0100 0072 3200 0000  heck).r9...r2...
-00005600: a904 7234 0100 0072 3801 0000 7237 0100  ..r4...r8...r7..
-00005610: 0072 3a01 0000 7212 0000 0072 1300 0000  .r:...r....r....
-00005620: 7236 0000 000d 0300 0073 0800 0000 0600  r6.......s......
-00005630: 0401 0201 06fe 7a1a 646f 776e 6c6f 6164  ......z.download
-00005640: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00005650: 613e 2904 7208 0000 0072 0900 0000 722a  a>).r....r....r*
-00005660: 0000 0072 3800 0000 2905 722b 0000 0072  ...r8...).r+...r
-00005670: 3401 0000 7237 0100 0072 3801 0000 723a  4...r7...r8...r:
-00005680: 0100 0072 1200 0000 723b 0100 0072 1300  ...r....r;...r..
-00005690: 0000 7239 0100 0001 0300 0073 1600 0000  ..r9.......s....
-000056a0: 1006 0601 02ff 0601 02ff 0802 0401 1401  ................
-000056b0: 0c01 1001 04ff da05 6669 6c65 737a 1c66  ........filesz.f
-000056c0: 696c 6520 6f72 2064 6972 6563 746f 7279  ile or directory
-000056d0: 2074 6f20 7570 6c6f 6164 2e29 0372 2500   to upload.).r%.
-000056e0: 0000 72e9 0000 00da 086d 756c 7469 706c  ..r......multipl
-000056f0: 65da 0973 616d 706c 655f 6964 da0d 6461  e..sample_id..da
-00005700: 7461 5f73 6574 5f74 7970 65da 0675 706c  ta_set_type..upl
-00005710: 6f61 647a 2055 706c 6f61 6420 6669 6c65  oadz Upload file
-00005720: 7320 746f 2066 6f72 6d20 6120 6461 7461  s to form a data
-00005730: 2073 6574 2e63 0400 0000 0000 0000 0000   set.c..........
-00005740: 0000 0400 0000 0600 0000 0300 0000 7336  ..............s6
-00005750: 0000 0074 007c 006a 0164 0164 028d 027c  ...t.|.j.d.d...|
-00005760: 006a 0164 033c 007c 006a 0164 0319 00a0  .j.d.<.|.j.d....
-00005770: 0264 0487 0087 0187 0266 0364 0564 0684  .d.......f.d.d..
-00005780: 08a1 0201 0064 0753 0029 087a aa20 4372  .....d.S.).z. Cr
-00005790: 6561 7465 7320 6461 7461 2073 6574 2075  eates data set u
-000057a0: 6e64 6572 206f 626a 6563 7420 616e 6420  nder object and 
-000057b0: 7570 6c6f 6164 2066 696c 6573 2074 6f20  upload files to 
-000057c0: 6974 2e0a 0a20 2020 2053 414d 504c 455f  it...    SAMPLE_
-000057d0: 4944 2020 2020 2020 2055 6e69 7175 6520  ID       Unique 
-000057e0: 6964 656e 7469 6669 6572 2061 6e20 6f62  identifier an ob
-000057f0: 6a65 6374 2069 6e20 4f70 656e 4249 532e  ject in OpenBIS.
-00005800: 0a0a 2020 2020 4441 5441 5f53 4554 5f54  ..    DATA_SET_T
-00005810: 5950 4520 2020 4e65 776c 7920 6372 6561  YPE   Newly crea
-00005820: 7465 6420 6461 7461 2073 6574 2074 7970  ted data set typ
-00005830: 652e 0a20 2020 2046 7298 0000 0072 3000  e..    Fr....r0.
-00005840: 0000 7240 0100 0063 0100 0000 0000 0000  ..r@...c........
-00005850: 0000 0000 0100 0000 0500 0000 1300 0000  ................
-00005860: 72eb 0000 0072 1a00 0000 2901 7240 0100  r....r....).r@..
-00005870: 0072 3200 0000 a903 723f 0100 0072 3c01  .r2.....r?...r<.
-00005880: 0000 723e 0100 0072 1200 0000 7213 0000  ..r>...r....r...
-00005890: 0072 3600 0000 2703 0000 72f0 0000 007a  .r6...'...r....z
-000058a0: 1875 706c 6f61 642e 3c6c 6f63 616c 733e  .upload.<locals>
-000058b0: 2e3c 6c61 6d62 6461 3e4e 2903 7209 0000  .<lambda>N).r...
-000058c0: 0072 2a00 0000 7238 0000 0029 0472 2b00  .r*...r8...).r+.
-000058d0: 0000 723e 0100 0072 3f01 0000 723c 0100  ..r>...r?...r<..
-000058e0: 0072 1200 0000 7241 0100 0072 1300 0000  .r....rA...r....
-000058f0: 7240 0100 001d 0300 0073 0800 0000 1408  r@.......s......
-00005900: 0c01 0e01 08ff 7a02 2d75 7a0a 2d2d 7373  ......z.-uz.--ss
-00005910: 685f 7573 6572 7a29 5573 6572 2074 6f20  h_userz)User to 
-00005920: 636f 6e6e 6563 7420 746f 2072 656d 6f74  connect to remot
-00005930: 6520 7379 7374 656d 7320 7669 6120 7373  e systems via ss
-00005940: 687a 022d 637a 142d 2d63 6f6e 7465 6e74  hz.-cz.--content
-00005950: 5f63 6f70 795f 696e 6465 787a 4949 6e64  _copy_indexzIInd
-00005960: 6578 206f 6620 7468 6520 636f 6e74 656e  ex of the conten
-00005970: 7420 636f 7079 2074 6f20 636c 6f6e 6520  t copy to clone 
-00005980: 6672 6f6d 2069 6e20 6361 7365 2074 6865  from in case the
-00005990: 7265 2061 7265 206d 756c 7469 706c 6520  re are multiple 
-000059a0: 636f 7069 6573 2903 720d 0000 0072 2300  copies).r....r#.
-000059b0: 0000 7225 0000 007a 2953 6b69 7020 6669  ..r%...z)Skip fi
-000059c0: 6c65 2069 6e74 6567 7269 7479 2063 6865  le integrity che
-000059d0: 636b 2077 6974 6820 6368 6563 6b73 756d  ck with checksum
-000059e0: 732e da05 636c 6f6e 657a 3443 6c6f 6e65  s...clonez4Clone
-000059f0: 2074 6865 2072 6570 6f73 6974 6f72 7920   the repository 
-00005a00: 666f 756e 6420 696e 2074 6865 2067 6976  found in the giv
-00005a10: 656e 2064 6174 6120 7365 7420 6964 2e63  en data set id.c
-00005a20: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-00005a30: 0700 0000 0300 0000 f320 0000 007c 006a  ......... ...|.j
-00005a40: 0064 0119 00a0 0164 0287 0087 0187 0287  .d.....d........
-00005a50: 0366 0464 0364 0484 08a1 0253 0029 054e  .f.d.d.....S.).N
-00005a60: 7230 0000 0072 4201 0000 6301 0000 0000  r0...rB...c.....
-00005a70: 0000 0000 0000 0001 0000 0006 0000 0013  ................
-00005a80: 0000 00f3 1000 0000 7c00 a000 8801 8803  ........|.......
-00005a90: 8800 8802 a104 5300 721a 0000 0029 0172  ......S.r....).r
-00005aa0: 4201 0000 7232 0000 00a9 04da 1263 6f6e  B...r2.......con
-00005ab0: 7465 6e74 5f63 6f70 795f 696e 6465 7872  tent_copy_indexr
-00005ac0: 3401 0000 723a 0100 00da 0873 7368 5f75  4...r:.....ssh_u
-00005ad0: 7365 7272 1200 0000 7213 0000 0072 3600  serr....r....r6.
-00005ae0: 0000 3d03 0000 f306 0000 000a 0002 0104  ..=.............
-00005af0: ff7a 2064 6174 615f 7365 745f 636c 6f6e  .z data_set_clon
-00005b00: 652e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  e.<locals>.<lamb
-00005b10: 6461 3e72 ac00 0000 a905 722b 0000 0072  da>r......r+...r
-00005b20: 4701 0000 7246 0100 0072 3401 0000 723a  G...rF...r4...r:
-00005b30: 0100 0072 1200 0000 7245 0100 0072 1300  ...r....rE...r..
-00005b40: 0000 da0e 6461 7461 5f73 6574 5f63 6c6f  ....data_set_clo
-00005b50: 6e65 3803 0000 f306 0000 000c 0410 0104  ne8.............
-00005b60: ff72 4a01 0000 6305 0000 0000 0000 0000  .rJ...c.........
-00005b70: 0000 0005 0000 0007 0000 0043 0000 0072  ...........C...r
-00005b80: f300 0000 a905 4e46 7298 0000 0072 3000  ......NFr....r0.
-00005b90: 0000 2904 7247 0100 0072 4601 0000 7234  ..).rG...rF...r4
-00005ba0: 0100 0072 3a01 0000 2904 7209 0000 0072  ...r:...).r....r
-00005bb0: 2a00 0000 72f4 0000 0072 4a01 0000 7249  *...r....rJ...rI
-00005bc0: 0100 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00005bd0: 0000 7242 0100 0041 0300 0072 f500 0000  ..rB...A...r....
-00005be0: da04 6d6f 7665 7a33 4d6f 7665 2074 6865  ..movez3Move the
-00005bf0: 2072 6570 6f73 6974 6f72 7920 666f 756e   repository foun
-00005c00: 6420 696e 2074 6865 2067 6976 656e 2064  d in the given d
-00005c10: 6174 6120 7365 7420 6964 2e63 0500 0000  ata set id.c....
-00005c20: 0000 0000 0000 0000 0500 0000 0700 0000  ................
-00005c30: 0300 0000 7243 0100 0029 054e 7230 0000  ....rC...).Nr0..
-00005c40: 0072 4d01 0000 6301 0000 0000 0000 0000  .rM...c.........
-00005c50: 0000 0001 0000 0006 0000 0013 0000 0072  ...............r
-00005c60: 4401 0000 721a 0000 0029 0172 4d01 0000  D...r....).rM...
-00005c70: 7232 0000 0072 4501 0000 7212 0000 0072  r2...rE...r....r
-00005c80: 1300 0000 7236 0000 0051 0300 0072 4801  ....r6...Q...rH.
-00005c90: 0000 7a1f 6461 7461 5f73 6574 5f6d 6f76  ..z.data_set_mov
-00005ca0: 652e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  e.<locals>.<lamb
-00005cb0: 6461 3e72 ac00 0000 7249 0100 0072 1200  da>r....rI...r..
-00005cc0: 0000 7245 0100 0072 1300 0000 da0d 6461  ..rE...r......da
-00005cd0: 7461 5f73 6574 5f6d 6f76 654c 0300 0072  ta_set_moveL...r
-00005ce0: 4b01 0000 724e 0100 0063 0500 0000 0000  K...rN...c......
-00005cf0: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-00005d00: 0000 72f3 0000 0072 4c01 0000 2904 7209  ..r....rL...).r.
-00005d10: 0000 0072 2a00 0000 72f4 0000 0072 4e01  ...r*...r....rN.
-00005d20: 0000 7249 0100 0072 1200 0000 7212 0000  ..rI...r....r...
-00005d30: 0072 1300 0000 724d 0100 0055 0300 0072  .r....rM...U...r
-00005d40: f500 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00005d50: 0000 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
-00005d60: 0000 7400 6900 6401 8d01 0100 6400 5300  ..t.i.d.....d.S.
-00005d70: 2902 4e72 2900 0000 2901 722d 0000 0072  ).Nr)...).r-...r
-00005d80: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00005d90: 0000 00da 046d 6169 6e5e 0300 0073 0200  .....main^...s..
-00005da0: 0000 0e01 724f 0100 00da 085f 5f6d 6169  ....rO.....__mai
-00005db0: 6e5f 5f29 024e 4e72 1a00 0000 2968 da07  n__).NNr....)h..
-00005dc0: 5f5f 646f 635f 5f72 9e00 0000 7241 0000  __doc__r....rA..
-00005dd0: 0072 0200 0000 7216 0000 00da 1664 6174  .r....r......dat
-00005de0: 6575 7469 6c2e 7265 6c61 7469 7665 6465  eutil.relativede
-00005df0: 6c74 6172 0300 0000 da05 7079 6269 7372  ltar......pybisr
-00005e00: 0400 0000 da08 7265 7175 6573 7473 7205  ......requestsr.
-00005e10: 0000 00da 0a63 6c69 636b 5f75 7469 6c72  .....click_utilr
-00005e20: 0800 0000 da10 6461 7461 5f6d 676d 745f  ......data_mgmt_
-00005e30: 7275 6e6e 6572 7209 0000 00da 1164 6d2e  runnerr......dm.
-00005e40: 636f 6d6d 616e 645f 7265 7375 6c74 720b  command_resultr.
-00005e50: 0000 00da 0864 6d2e 7574 696c 7372 0c00  .....dm.utilsr..
-00005e60: 0000 7214 0000 0072 1900 0000 7221 0000  ..r....r....r!..
-00005e70: 00da 0567 726f 7570 da0e 7665 7273 696f  ...group..versio
-00005e80: 6e5f 6f70 7469 6f6e da06 6f70 7469 6f6e  n_option..option
-00005e90: da0c 7061 7373 5f63 6f6e 7465 7874 722d  ..pass_contextr-
-00005ea0: 0000 0072 3a00 0000 7249 0000 00da 0950  ...r:...rI.....P
-00005eb0: 6172 616d 5479 7065 724a 0000 0072 6400  aramTyperJ...rd.
-00005ec0: 0000 7265 0000 0072 7c00 0000 727f 0000  ..re...r|...r...
-00005ed0: 0072 8700 0000 728d 0000 0072 9300 0000  .r....r....r....
-00005ee0: 7296 0000 0072 6a00 0000 da07 636f 6d6d  r....rj.....comm
-00005ef0: 616e 6472 4b00 0000 7239 0000 00da 0861  andrK...r9.....a
-00005f00: 7267 756d 656e 7472 a800 0000 72ae 0000  rgumentr....r...
-00005f10: 0072 b100 0000 da0e 5f73 6561 7263 685f  .r......_search_
-00005f20: 7061 7261 6d73 72b8 0000 0072 ba00 0000  paramsr....r....
-00005f30: 72bc 0000 0072 bd00 0000 72cc 0000 0072  r....r....r....r
-00005f40: d600 0000 72d8 0000 0072 da00 0000 72db  ....r....r....r.
-00005f50: 0000 0072 dc00 0000 72de 0000 0072 df00  ...r....r....r..
-00005f60: 0000 72e0 0000 0072 e100 0000 7285 0000  ..r....r....r...
-00005f70: 0072 e400 0000 72e5 0000 0072 e600 0000  .r....r....r....
-00005f80: da04 5061 7468 da0e 5f63 6f6d 6d69 745f  ..Path.._commit_
-00005f90: 7061 7261 6d73 72f2 0000 0072 ea00 0000  paramsr....r....
-00005fa0: da0c 5f69 6e69 745f 7061 7261 6d73 72f8  .._init_paramsr.
-00005fb0: 0000 00da 155f 696e 6974 5f70 6172 616d  ....._init_param
-00005fc0: 735f 7068 7973 6963 616c 72f7 0000 00da  s_physicalr.....
-00005fd0: 155f 696e 6974 5f61 6e61 6c79 7369 735f  ._init_analysis_
-00005fe0: 7061 7261 6d73 72fa 0000 0072 3c00 0000  paramsr....r<...
-00005ff0: da0e 5f73 7461 7475 735f 7061 7261 6d73  .._status_params
-00006000: 72fd 0000 0072 fb00 0000 da0c 5f73 796e  r....r......_syn
-00006010: 635f 7061 7261 6d73 7206 0100 0072 0901  c_paramsr....r..
-00006020: 0000 7205 0100 0072 0b01 0000 722f 0100  ..r....r....r/..
-00006030: 00da 0e5f 6164 6472 6566 5f70 6172 616d  ..._addref_param
-00006040: 7372 3101 0000 7230 0100 00da 115f 7265  sr1...r0....._re
-00006050: 6d6f 7665 7265 665f 7061 7261 6d73 7236  moveref_paramsr6
-00006060: 0100 0072 3201 0000 da10 5f64 6f77 6e6c  ...r2....._downl
-00006070: 6f61 645f 7061 7261 6d73 7239 0100 00da  oad_paramsr9....
-00006080: 0e5f 7570 6c6f 6164 5f70 6172 616d 7372  ._upload_paramsr
-00006090: 4001 0000 7222 0100 00da 125f 636c 6f6e  @...r"....._clon
-000060a0: 655f 6d6f 7665 5f70 6172 616d 7372 4a01  e_move_paramsrJ.
-000060b0: 0000 7242 0100 0072 4e01 0000 724d 0100  ..rB...rN...rM..
-000060c0: 0072 4f01 0000 7260 0000 0072 1200 0000  .rO...r`...r....
-000060d0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-000060e0: 083c 6d6f 6475 6c65 3e01 0000 0073 aa02  .<module>....s..
-000060f0: 0000 0412 0805 0801 0c01 0802 0c01 0c01  ................
-00006100: 0c01 0c02 0c01 0c01 0c01 0803 0805 0805  ................
-00006110: 0609 0a01 1201 0c01 0201 04ff 1202 0401  ................
-00006120: 1401 0807 0809 1214 100f 1204 082b 0808  .............+..
-00006130: 0c07 080b 0807 0809 060b 1201 0401 0e01  ................
-00006140: 0806 0401 0c01 0609 1201 0401 0e01 0809  ................
-00006150: 1001 0401 0e01 0804 1001 0401 0e01 0804  ................
-00006160: 1001 0401 0e01 0c08 0201 04ff 1002 1001  ................
-00006170: 1001 1201 1001 0a01 0201 04ff 0c02 0201  ................
-00006180: 04ff 0c02 0201 04ff 1002 04f2 0812 1201  ................
-00006190: 0c01 0201 04ff 0402 1001 080a 1001 0401  ................
-000061a0: 0e01 0804 1001 0401 0e01 0804 1001 0401  ................
-000061b0: 0e01 0c04 0601 0401 0e01 0617 1201 0401  ................
-000061c0: 0e01 0809 1001 0401 0e01 0804 1001 0401  ................
-000061d0: 0e01 0804 1001 0401 0e01 0c04 0601 0401  ................
-000061e0: 0e01 0617 1201 0401 0e01 0809 1001 0401  ................
-000061f0: 0e01 0804 1001 0401 0e01 0804 1001 0401  ................
-00006200: 0e01 0607 1201 0401 0e01 080c 1001 0401  ................
-00006210: 0e01 0804 1001 0401 0e01 0804 1001 0401  ................
-00006220: 0e01 0a09 0201 04ff 0c02 0201 04ff 0a02  ................
-00006230: 0401 04ff 0a02 0401 04ff 0201 04ff 04f9  ................
-00006240: 0c0c 0401 0601 0e01 0a06 0401 0601 0e01  ................
-00006250: 0a0a 0401 04ff 0201 04ff 0c02 04fd 0c08  ................
-00006260: 0401 0601 0e01 0205 0e01 0201 06ff 02ff  ................
-00006270: 02ff 0a06 0401 0601 0e01 0809 0c01 04ff  ................
-00006280: 04ff 0804 0c03 0401 0601 0e01 0c04 0401  ................
-00006290: 0601 0e01 0a0a 0401 04ff 0201 04ff 04ff  ................
-000062a0: 0c06 0401 0601 0e01 0a04 0401 0601 0e01  ................
-000062b0: 0a09 0401 04ff 0a02 0401 04ff 0201 04ff  ................
-000062c0: 04fd 0808 0c05 0401 0601 0e01 0a05 0401  ................
-000062d0: 0601 0e01 0a06 0401 0c01 0c04 0c01 0c01  ................
-000062e0: 0c01 0c01 0401 1801 0a38 0401 04ff 0201  .........8......
-000062f0: 04ff 04ff 0c06 0401 0601 0e01 0a04 0401  ................
-00006300: 0601 0e01 0809 0201 04ff 0a02 0401 04ff  ................
-00006310: 0201 04ff 04fd 0608 0201 04ff 0402 0601  ................
-00006320: 0e01 0a08 0401 0601 0e01 0c0b 0a01 0201  ................
-00006330: 04ff 0403 0601 0201 04fe 0c03 0201 04ff  ................
-00006340: 04f8 0c0d 0601 0401 0e01 0412 0c01 04ff  ................
-00006350: 0802 0801 04fc 0c08 0601 0401 0e01 0a0e  ................
-00006360: 0201 04ff 1002 0401 06ff 0a02 0601 04ff  ................
-00006370: 0802 04f9 100b 0401 0601 1201 0c06 0401  ................
-00006380: 0601 1201 1008 0401 0601 1201 0c06 0401  ................
-00006390: 0601 1201 0c06 0c04 0a01 04ff            ............
+00000320: 646d 646e 6402 646f 6451 8d05 6504 6a18  dmdnd.dodQ..e.j.
+00000330: 6470 6471 6402 6472 6451 8d04 6504 6a18  dpdqd.drdQ..e.j.
+00000340: 6473 6474 6475 6417 6416 6476 6477 8d06  dsdtdud.d.dvdw..
+00000350: 670c 5a2f 651a a016 6478 a101 6504 6a18  g.Z/e...dx..e.j.
+00000360: 6438 6439 6416 6417 6440 6419 8d05 6504  d8d9d.d.d@d...e.
+00000370: 6a18 6479 647a 6416 6417 647b 6419 8d05  j.dydzd.d.d{d...
+00000380: 6504 6a19 647c 6478 8400 8301 8301 8301  e.j.d|dx........
+00000390: 8301 5a30 6530 a028 6443 a101 6504 6a2b  ..Z0e0.(dC..e.j+
+000003a0: 647d 6520 8300 6444 6445 8d03 6504 6a19  d}e ..dDdE..e.j.
+000003b0: 647e 647f 8400 8301 8301 8301 5a31 6530  d~d.........Z1e0
+000003c0: a028 643d a101 6504 6a2b 647d 651e 8300  .(d=..e.j+d}e...
+000003d0: 6444 6445 8d03 6504 6a19 6480 6481 8400  dDdE..e.j.d.d...
+000003e0: 8301 8301 8301 5a32 6530 a028 644a a101  ......Z2e0.(dJ..
+000003f0: 6504 6a2b 647d 651f 8300 6444 6445 8d03  e.j+d}e...dDdE..
+00000400: 6504 6a19 6482 6483 8400 8301 8301 8301  e.j.d.d.........
+00000410: 5a33 6530 6a28 6484 6485 6486 8d02 6515  Z3e0j(d.d.d...e.
+00000420: 652f 8301 6504 6a19 6487 6488 8400 8301  e/..e.j.d.d.....
+00000430: 8301 8301 5a34 651a a016 a100 6504 6a18  ....Z4e.....e.j.
+00000440: 6438 6439 6416 6417 6440 6419 8d05 6504  d8d9d.d.d@d...e.
+00000450: 6a19 6489 648a 8400 8301 8301 8301 5a35  j.d.d.........Z5
+00000460: 6535 a028 6443 a101 6504 6a2b 648b 6520  e5.(dC..e.j+d.e 
+00000470: 8300 6444 6445 8d03 6504 6a19 648c 648d  ..dDdE..e.j.d.d.
+00000480: 8400 8301 8301 8301 5a36 6535 a028 643d  ........Z6e5.(d=
+00000490: a101 6504 6a2b 648b 651e 8300 6444 6445  ..e.j+d.e...dDdE
+000004a0: 8d03 6504 6a19 648e 648f 8400 8301 8301  ..e.j.d.d.......
+000004b0: 8301 5a37 6535 a028 644a a101 6504 6a2b  ..Z7e5.(dJ..e.j+
+000004c0: 648b 651f 8300 6444 6445 8d03 6504 6a19  d.e...dDdE..e.j.
+000004d0: 6490 6491 8400 8301 8301 8301 5a38 6535  d.d.........Z8e5
+000004e0: 6a28 6484 6492 6486 8d02 6515 652f 8301  j(d.d.d...e.e/..
+000004f0: 6504 6a19 6493 6494 8400 8301 8301 8301  e.j.d.d.........
+00000500: 5a39 651a a016 a100 6504 6a18 6438 6439  Z9e.....e.j.d8d9
+00000510: 6416 6417 6440 6419 8d05 6504 6a19 6495  d.d.d@d...e.j.d.
+00000520: 6496 8400 8301 8301 8301 5a3a 653a a028  d.........Z:e:.(
+00000530: 6443 a101 6504 6a2b 643c 6520 8300 6444  dC..e.j+d<e ..dD
+00000540: 6445 8d03 6504 6a19 6497 6498 8400 8301  dE..e.j.d.d.....
+00000550: 8301 8301 5a3b 653a a028 643d a101 6504  ....Z;e:.(d=..e.
+00000560: 6a2b 643c 651e 8300 6444 6445 8d03 6504  j+d<e...dDdE..e.
+00000570: 6a19 6499 649a 8400 8301 8301 8301 5a3c  j.d.d.........Z<
+00000580: 653a a028 644a a101 6504 6a2b 643c 651f  e:.(dJ..e.j+d<e.
+00000590: 8300 6444 6445 8d03 6504 6a19 649b 649c  ..dDdE..e.j.d.d.
+000005a0: 8400 8301 8301 8301 5a3d 651a a016 a100  ........Z=e.....
+000005b0: 6504 6a18 6438 6439 6416 6417 6440 6419  e.j.d8d9d.d.d@d.
+000005c0: 8d05 6504 6a19 649d 649e 8400 8301 8301  ..e.j.d.d.......
+000005d0: 8301 5a3e 653e a028 6443 a101 6504 6a2b  ..Z>e>.(dC..e.j+
+000005e0: 643c 6520 8300 6444 6445 8d03 6504 6a19  d<e ..dDdE..e.j.
+000005f0: 649f 64a0 8400 8301 8301 8301 5a3f 653e  d.d.........Z?e>
+00000600: a028 643d a101 6504 6a2b 643c 651e 8300  .(d=..e.j+d<e...
+00000610: 6444 6445 8d03 6504 6a19 64a1 64a2 8400  dDdE..e.j.d.d...
+00000620: 8301 8301 8301 5a40 653e a028 644a a101  ......Z@e>.(dJ..
+00000630: 6504 6a2b 643c 651f 8300 6444 6445 8d03  e.j+d<e...dDdE..
+00000640: 6504 6a19 64a3 64a4 8400 8301 8301 8301  e.j.d.d.........
+00000650: 5a41 6504 6a18 64a5 64a6 64a7 64a8 6451  ZAe.j.d.d.d.d.dQ
+00000660: 8d04 6504 6a18 64a9 64aa 6417 6417 64ab  ..e.j.d.d.d.d.d.
+00000670: 6419 8d05 6504 6a18 64ac 64ad 6417 6417  d...e.j.d.d.d.d.
+00000680: 64ae 6419 8d05 6504 6a2b 6442 6504 6a42  d.d...e.j+dBe.jB
+00000690: 6417 6416 64af 8d02 6416 64b0 8d03 6704  d.d.d...d.d...g.
+000006a0: 5a43 652a 6a28 64b1 64b2 6486 8d02 6504  ZCe*j(d.d.d...e.
+000006b0: 6a19 6515 6543 8301 64b3 64b4 8400 8301  j.e.eC..d.d.....
+000006c0: 8301 8301 5a44 651a 6a28 64b2 6486 8d01  ....ZDe.j(d.d...
+000006d0: 6504 6a19 6515 6543 8301 64b5 64b1 8400  e.j.e.eC..d.d...
+000006e0: 8301 8301 8301 5a45 6504 6a2b 64b6 6504  ......ZEe.j+d.e.
+000006f0: 6a42 6416 6416 64af 8d02 6416 64b0 8d03  jBd.d.d...d.d...
+00000700: 6504 6a2b 64b7 64b8 64b9 8d02 6702 5a46  e.j+d.d.d...g.ZF
+00000710: 652a 6a28 64ba 64bb 6486 8d02 6504 6a19  e*j(d.d.d...e.j.
+00000720: 6515 6546 8301 64bc 64bd 8400 8301 8301  e.eF..d.d.......
+00000730: 8301 5a47 6546 6504 6a18 6479 64be 64bf  ..ZGeFe.j.dyd.d.
+00000740: 6416 6417 64c0 6419 8d06 6701 1700 5a48  d.d.d.d...g...ZH
+00000750: 651a 6a28 64bb 6486 8d01 6504 6a19 6515  e.j(d.d...e.j.e.
+00000760: 6548 8301 64c1 64ba 8400 8301 8301 8301  eH..d.d.........
+00000770: 5a49 6504 6a18 6479 64c2 6504 6a42 6416  ZIe.j.dyd.e.jBd.
+00000780: 6416 64af 8d02 64c3 8d03 6701 5a4a 654a  d.d...d...g.ZJeJ
+00000790: 6546 3700 5a4a 652a 6a28 64c4 64c5 6486  eF7.ZJe*j(d.d.d.
+000007a0: 8d02 6504 6a19 6515 654a 8301 64c6 64c7  ..e.j.e.eJ..d.d.
+000007b0: 8400 8301 8301 8301 5a4b 651a 6a28 64c4  ........ZKe.j(d.
+000007c0: 64c5 64c8 8d02 6504 6a19 6515 654a 8301  d.d...e.j.e.eJ..
+000007d0: 64c9 64c4 8400 8301 8301 8301 5a4c 6504  d.d.........ZLe.
+000007e0: 6a2b 6442 6504 6a42 6417 6416 64af 8d02  j+dBe.jBd.d.d...
+000007f0: 6416 64b0 8d03 6701 5a4d 652a 6a28 64ca  d.d...g.ZMe*j(d.
+00000800: 64cb 6486 8d02 6504 6a19 6515 654d 8301  d.d...e.j.e.eM..
+00000810: 64cc 64cd 8400 8301 8301 8301 5a4e 651a  d.d.........ZNe.
+00000820: 6a28 64cb 6486 8d01 6504 6a19 6515 654d  j(d.d...e.j.e.eM
+00000830: 8301 64ce 64ca 8400 8301 8301 8301 5a4f  ..d.d.........ZO
+00000840: 6504 6a18 64ac 64ad 6417 6417 64ae 6419  e.j.d.d.d.d.d.d.
+00000850: 8d05 6504 6a2b 6442 6504 6a42 6417 6416  ..e.j+dBe.jBd.d.
+00000860: 64af 8d02 6416 64b0 8d03 6702 5a50 64cf  d...d.d...g.ZPd.
+00000870: 64d0 8400 5a51 652a 6a28 64d1 64d2 6486  d...ZQe*j(d.d.d.
+00000880: 8d02 6504 6a19 6515 6550 8301 64d3 64d4  ..e.j.e.eP..d.d.
+00000890: 8400 8301 8301 8301 5a52 651a 6a28 64d2  ........ZRe.j(d.
+000008a0: 6486 8d01 6504 6a19 6515 6550 8301 64d5  d...e.j.e.eP..d.
+000008b0: 64d1 8400 8301 8301 8301 5a53 651a 6a16  d.........ZSe.j.
+000008c0: 64d6 6486 8d01 6504 6a19 64d7 64d8 8400  d.d...e.j.d.d...
+000008d0: 8301 8301 5a54 6554 6a28 643d 64d9 6486  ....ZTeTj(d=d.d.
+000008e0: 8d02 6504 6a2b 64da 6416 64db 8d02 6504  ..e.j+d.d.d...e.
+000008f0: 6a18 64dc 64dd 64de 8d02 6504 6a18 64df  j.d.d.d...e.j.d.
+00000900: 64e0 64de 8d02 6504 6a18 64e1 64e2 64de  d.d...e.j.d.d.d.
+00000910: 8d02 6504 6a19 9001 641d 64e3 64e4 8401  ..e.j...d.d.d...
+00000920: 8301 8301 8301 8301 8301 8301 5a55 6504  ............ZUe.
+00000930: 6a2b 6442 6504 6a42 6417 6416 64af 8d02  j+dBe.jBd.d.d...
+00000940: 6416 64b0 8d03 6701 5a56 652a 6a28 64e5  d.d...g.ZVe*j(d.
+00000950: 64e6 6486 8d02 6504 6a19 6515 6556 8301  d.d...e.j.e.eV..
+00000960: 64e7 64e8 8400 8301 8301 8301 5a57 651a  d.d.........ZWe.
+00000970: 6a28 64e6 6486 8d01 6504 6a19 6515 6556  j(d.d...e.j.e.eV
+00000980: 8301 64e9 64e5 8400 8301 8301 8301 5a58  ..d.d.........ZX
+00000990: 6504 6a18 641d 64ea 64eb 64de 8d03 6504  e.j.d.d.d.d...e.
+000009a0: 6a2b 6442 6504 6a42 6417 6416 64af 8d02  j+dBe.jBd.d.d...
+000009b0: 6416 64b0 8d03 6702 5a59 652a 6a28 64ec  d.d...g.ZYe*j(d.
+000009c0: 64ed 6486 8d02 6504 6a19 6515 6559 8301  d.d...e.j.e.eY..
+000009d0: 64ee 64ef 8400 8301 8301 8301 5a5a 651a  d.d.........ZZe.
+000009e0: 6a28 64ed 6486 8d01 6504 6a19 6515 6559  j(d.d...e.j.e.eY
+000009f0: 8301 64f0 64ec 8400 8301 8301 8301 5a5b  ..d.d.........Z[
+00000a00: 6504 6a2b 64f1 6416 64db 8d02 6504 6a18  e.j+d.d.d...e.j.
+00000a10: 64f2 64f3 64f4 64f5 64de 8d04 6504 6a18  d.d.d.d.d...e.j.
+00000a20: 64f6 64f7 64f8 64f9 64de 8d04 6504 6a18  d.d.d.d.d...e.j.
+00000a30: 641a 64fa 6416 6417 64fb 6419 8d05 6704  d.d.d.d.d.d...g.
+00000a40: 5a5c 651a 6a28 64fc 64fd 6486 8d02 6515  Z\e.j(d.d.d...e.
+00000a50: 655c 8301 6504 6a19 64fe 64fc 8400 8301  e\..e.j.d.d.....
+00000a60: 8301 8301 5a5d 6504 6a18 64f6 64f7 64ff  ....Z]e.j.d.d.d.
+00000a70: 9001 6400 6417 6417 9001 6401 8d06 6504  ..d.d.d...d...e.
+00000a80: a02b 9001 6402 a101 6504 a02b 9001 6403  .+..d...e..+..d.
+00000a90: a101 6703 5a5e 651a 6a28 9001 6404 9001  ..g.Z^e.j(..d...
+00000aa0: 6405 6486 8d02 6515 655e 8301 6504 6a19  d.d...e.e^..e.j.
+00000ab0: 9001 6406 9001 6404 8400 8301 8301 8301  ..d...d.........
+00000ac0: 5a5f 6504 6a18 9001 6407 9001 6408 6402  Z_e.j...d...d.d.
+00000ad0: 9001 6409 6451 8d04 6504 6a18 9001 640a  ..d.dQ..e.j...d.
+00000ae0: 9001 640b 6560 6402 9001 640c 9001 640d  ..d.e`d...d...d.
+00000af0: 8d05 6504 6a18 641a 64fa 6416 6417 9001  ..e.j.d.d.d.d...
+00000b00: 640e 6419 8d05 6504 a02b 64f1 a101 6704  d.d...e..+d...g.
+00000b10: 5a61 6530 6a28 9001 640f 9001 6410 6486  Zae0j(..d...d.d.
+00000b20: 8d02 6504 6a19 6515 6561 8301 9001 6411  ..e.j.e.ea....d.
+00000b30: 9001 6412 8400 8301 8301 8301 5a62 651a  ..d.........Zbe.
+00000b40: 6a28 9001 6410 6486 8d01 6504 6a19 6515  j(..d.d...e.j.e.
+00000b50: 6561 8301 9001 6413 9001 640f 8400 8301  ea....d...d.....
+00000b60: 8301 8301 5a63 6530 6a28 9001 6414 9001  ....Zce0j(..d...
+00000b70: 6415 6486 8d02 6504 6a19 6515 6561 8301  d.d...e.j.e.ea..
+00000b80: 9001 6416 9001 6417 8400 8301 8301 8301  ..d...d.........
+00000b90: 5a64 651a 6a28 9001 6415 6486 8d01 6504  Zde.j(..d.d...e.
+00000ba0: 6a19 6515 6561 8301 9001 6418 9001 6414  j.e.ea....d...d.
+00000bb0: 8400 8301 8301 8301 5a65 9001 6419 9001  ........Ze..d...
+00000bc0: 641a 8400 5a66 6567 9001 641b 6b02 9005  d...Zfeg..d.k...
+00000bd0: 72d7 6566 8300 0100 6402 5300 6402 5300  r.ef....d.S.d.S.
+00000be0: 281e 0100 007a 360a 636c 692e 7079 0a0a  (....z6.cli.py..
+00000bf0: 5468 6520 6d6f 6475 6c65 2074 6861 7420  The module that 
+00000c00: 696d 706c 656d 656e 7473 2074 6865 2043  implements the C
+00000c10: 4c49 2066 6f72 206f 6269 732e 0ae9 0000  LI for obis.....
+00000c20: 0000 4e29 01da 0864 6174 6574 696d 6529  ..N)...datetime)
+00000c30: 01da 0d72 656c 6174 6976 6564 656c 7461  ...relativedelta
+00000c40: 2901 da07 4f70 656e 6269 7329 01da 0f43  )...Openbis)...C
+00000c50: 6f6e 6e65 6374 696f 6e45 7272 6f72 e901  onnectionError..
+00000c60: 0000 00a9 01da 0a63 6c69 636b 5f65 6368  .......click_ech
+00000c70: 6f29 01da 0e44 6174 614d 676d 7452 756e  o)...DataMgmtRun
+00000c80: 6e65 72e9 0200 0000 2901 da0d 436f 6d6d  ner.....)...Comm
+00000c90: 616e 6452 6573 756c 7429 01da 0d4f 7065  andResult)...Ope
+00000ca0: 7261 7469 6f6e 5479 7065 6301 0000 0000  rationTypec.....
+00000cb0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00000cc0: 0000 0073 2000 0000 7c00 6401 1900 6402  ...s ...|.d...d.
+00000cd0: 6b02 720e 7400 7c00 6403 1900 8301 0100  k.r.t.|.d.......
+00000ce0: 6400 5300 6400 5300 2904 4eda 0474 7970  d.S.d.S.).N..typ
+00000cf0: 65da 0870 726f 6772 6573 73da 076d 6573  e..progress..mes
+00000d00: 7361 6765 7207 0000 00a9 01da 0d70 726f  sager........pro
+00000d10: 6772 6573 735f 6461 7461 a900 7212 0000  gress_data..r...
+00000d20: 00fa 5c2f 686f 6d65 2f61 6c61 736b 6f77  ..\/home/alaskow
+00000d30: 736b 692f 7265 706f 2f6f 7065 6e62 6973  ski/repo/openbis
+00000d40: 5f70 7974 686f 6e2f 6170 702d 6f70 656e  _python/app-open
+00000d50: 6269 732d 636f 6d6d 616e 642d 6c69 6e65  bis-command-line
+00000d60: 2f73 7263 2f70 7974 686f 6e2f 6f62 6973  /src/python/obis
+00000d70: 2f73 6372 6970 7473 2f63 6c69 2e70 79da  /scripts/cli.py.
+00000d80: 0e63 6c69 636b 5f70 726f 6772 6573 7327  .click_progress'
+00000d90: 0000 0073 0600 0000 0c01 1001 04ff 7214  ...s..........r.
+00000da0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000db0: 0100 0000 0600 0000 4300 0000 7328 0000  ........C...s(..
+00000dc0: 007c 0064 0119 0064 026b 0272 1274 00a0  .|.d...d.k.r.t..
+00000dd0: 0164 03a0 027c 0064 0419 00a1 01a1 0101  .d...|.d........
+00000de0: 0064 0053 0064 0053 0029 054e 720d 0000  .d.S.d.S.).Nr...
+00000df0: 0072 0e00 0000 fa02 7b7d 720f 0000 0029  .r......{}r....)
+00000e00: 03da 0563 6c69 636b da04 6563 686f da06  ...click..echo..
+00000e10: 666f 726d 6174 7210 0000 0072 1200 0000  formatr....r....
+00000e20: 7212 0000 0072 1300 0000 da14 636c 6963  r....r......clic
+00000e30: 6b5f 7072 6f67 7265 7373 5f6e 6f5f 7473  k_progress_no_ts
+00000e40: 2c00 0000 7306 0000 000c 0118 0104 ff72  ,...s..........r
+00000e50: 1900 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000e60: 0002 0000 0003 0000 0003 0000 0073 1000  .............s..
+00000e70: 0000 8700 6601 6401 6402 8408 7d01 7c01  ....f.d.d...}.|.
+00000e80: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
+00000e90: 0000 0200 0000 0300 0000 1300 0000 731a  ..............s.
+00000ea0: 0000 0074 0088 0083 0144 005d 067d 017c  ...t.....D.].}.|
+00000eb0: 017c 0083 017d 0071 047c 0053 00a9 014e  .|...}.q.|.S...N
+00000ec0: 2901 da08 7265 7665 7273 6564 2902 da04  )...reversed)...
+00000ed0: 6675 6e63 da05 7061 7261 6da9 01da 0670  func..param....p
+00000ee0: 6172 616d 7372 1200 0000 7213 0000 00da  aramsr....r.....
+00000ef0: 0b5f 6164 645f 7061 7261 6d73 3200 0000  ._add_params2...
+00000f00: 7306 0000 000c 010a 0104 017a 1f61 6464  s..........z.add
+00000f10: 5f70 6172 616d 732e 3c6c 6f63 616c 733e  _params.<locals>
+00000f20: 2e5f 6164 645f 7061 7261 6d73 7212 0000  ._add_paramsr...
+00000f30: 0029 0272 1f00 0000 7220 0000 0072 1200  .).r....r ...r..
+00000f40: 0000 721e 0000 0072 1300 0000 da0a 6164  ..r....r......ad
+00000f50: 645f 7061 7261 6d73 3100 0000 7304 0000  d_params1...s...
+00000f60: 000c 0104 0572 2100 0000 2901 da07 7665  .....r!...)...ve
+00000f70: 7273 696f 6e7a 022d 717a 072d 2d71 7569  rsionz.-qz.--qui
+00000f80: 6574 4654 7a1a 5375 7070 7265 7373 2073  etFTz.Suppress s
+00000f90: 7461 7475 7320 7265 706f 7274 696e 672e  tatus reporting.
+00000fa0: 2903 da07 6465 6661 756c 74da 0769 735f  )...default..is_
+00000fb0: 666c 6167 da04 6865 6c70 7a02 2d73 7a13  flag..helpz.-sz.
+00000fc0: 2d2d 736b 6970 5f76 6572 6966 6963 6174  --skip_verificat
+00000fd0: 696f 6e7a 1944 6f20 6e6f 7420 7665 7269  ionz.Do not veri
+00000fe0: 6679 2063 6572 6669 6369 6174 6573 7a02  fy cerficiatesz.
+00000ff0: 2d64 7a07 2d2d 6465 6275 677a 1a53 686f  -dz.--debugz.Sho
+00001000: 7720 7374 6163 6b20 7472 6163 6520 6f6e  w stack trace on
+00001010: 2065 7272 6f72 2e63 0400 0000 0000 0000   error.c........
+00001020: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
+00001030: 7326 0000 007c 017c 006a 0064 013c 007c  s&...|.|.j.d.<.|
+00001040: 0272 0c64 027c 006a 0064 033c 007c 037c  .r.d.|.j.d.<.|.|
+00001050: 006a 0064 043c 0064 0053 0029 054e da05  .j.d.<.d.S.).N..
+00001060: 7175 6965 7446 da13 7665 7269 6679 5f63  quietF..verify_c
+00001070: 6572 7469 6669 6361 7465 73da 0564 6562  ertificates..deb
+00001080: 7567 a901 da03 6f62 6a29 04da 0363 7478  ug....obj)...ctx
+00001090: 7226 0000 00da 1173 6b69 705f 7665 7269  r&.....skip_veri
+000010a0: 6669 6361 7469 6f6e 7228 0000 0072 1200  ficationr(...r..
+000010b0: 0000 7212 0000 0072 1300 0000 da03 636c  ..r....r......cl
+000010c0: 693a 0000 0073 0800 0000 0a08 0401 0a01  i:...s..........
+000010d0: 0e01 722d 0000 0063 0300 0000 0000 0000  ..r-...c........
+000010e0: 0000 0000 0300 0000 0600 0000 0300 0000  ................
+000010f0: 7346 0000 007c 0164 0175 0072 0664 027d  sF...|.d.u.r.d.}
+00001100: 0174 0064 03a0 017c 01a1 0183 0101 0088  .t.d...|........
+00001110: 0064 046b 0372 1388 006e 0164 0189 007c  .d.k.r...n.d...|
+00001120: 006a 0264 0519 00a0 0364 0687 0066 0164  .j.d.....d...f.d
+00001130: 0764 0884 087c 01a1 0353 0029 097a 3053  .d...|...S.).z0S
+00001140: 6861 7265 6420 696d 706c 656d 656e 7461  hared implementa
+00001150: 7469 6f6e 2066 6f72 2074 6865 2069 6e69  tion for the ini
+00001160: 745f 6461 7461 2063 6f6d 6d61 6e64 2e4e  t_data command.N
+00001170: da01 2e7a 0c69 6e69 745f 6461 7461 207b  ...z.init_data {
+00001180: 7dda 00da 0672 756e 6e65 72da 0969 6e69  }....runner..ini
+00001190: 745f 6461 7461 6301 0000 0000 0000 0000  t_datac.........
+000011a0: 0000 0001 0000 0003 0000 0013 0000 0073  ...............s
+000011b0: 0a00 0000 7c00 a000 8800 a101 5300 721a  ....|.......S.r.
+000011c0: 0000 0029 0172 3100 0000 a901 da02 646d  ...).r1.......dm
+000011d0: a901 da04 6465 7363 7212 0000 0072 1300  ....descr....r..
+000011e0: 0000 da08 3c6c 616d 6264 613e 4e00 0000  ....<lambda>N...
+000011f0: f302 0000 000a 007a 2069 6e69 745f 6461  .......z init_da
+00001200: 7461 5f69 6d70 6c2e 3c6c 6f63 616c 733e  ta_impl.<locals>
+00001210: 2e3c 6c61 6d62 6461 3e29 0472 0800 0000  .<lambda>).r....
+00001220: 7218 0000 0072 2a00 0000 da03 7275 6e29  r....r*.....run)
+00001230: 0372 2b00 0000 da0a 7265 706f 7369 746f  .r+.....reposito
+00001240: 7279 7235 0000 0072 1200 0000 7234 0000  ryr5...r....r4..
+00001250: 0072 1300 0000 da0e 696e 6974 5f64 6174  .r......init_dat
+00001260: 615f 696d 706c 4800 0000 730a 0000 0008  a_implH...s.....
+00001270: 0204 010e 0110 011c 0172 3a00 0000 6304  .........r:...c.
+00001280: 0000 0000 0000 0000 0000 0006 0000 0006  ................
+00001290: 0000 0003 0000 0073 ce00 0000 7400 6401  .......s....t.d.
+000012a0: a001 7c02 a101 8301 0100 8801 6400 7501  ..|.........d.u.
+000012b0: 7217 7402 6a03 a004 8801 a101 7217 7400  r.t.j.......r.t.
+000012c0: 6402 8301 0100 6403 5300 7c02 6400 7501  d.....d.S.|.d.u.
+000012d0: 7227 7402 6a03 a004 7c02 a101 7227 7400  r't.j...|...r't.
+000012e0: 6404 8301 0100 6403 5300 8800 6405 6b03  d.....d.S...d.k.
+000012f0: 722d 8800 6e01 6400 8900 8801 6400 7500  r-..n.d.....d.u.
+00001300: 7237 7402 a005 a100 6e08 7402 6a03 a006  r7t.....n.t.j...
+00001310: 7402 a005 a100 8801 a102 7d04 7402 6a03  t.........}.t.j.
+00001320: a006 7402 a005 a100 7c02 a102 7d05 7402  ..t.....|...}.t.
+00001330: 6a03 a007 7c04 7c05 a102 8901 8801 6400  j...|.|.......d.
+00001340: 7500 7256 6406 6e01 8801 8901 7c00 6a08  u.rVd.n.....|.j.
+00001350: 6407 1900 a009 6408 8700 8701 6602 6409  d.....d.....f.d.
+00001360: 640a 8408 7c02 a103 5300 290b 4e7a 1069  d...|...S.).Nz.i
+00001370: 6e69 745f 616e 616c 7973 6973 207b 7d7a  nit_analysis {}z
+00001380: 3345 7272 6f72 3a20 5468 6520 7061 7265  3Error: The pare
+00001390: 6e74 206d 7573 7420 6265 2067 6976 656e  nt must be given
+000013a0: 2061 7320 6120 7265 6c61 7469 7665 2070   as a relative p
+000013b0: 6174 682e e9ff ffff ff7a 3745 7272 6f72  ath......z7Error
+000013c0: 3a20 5468 6520 7265 706f 7369 746f 7279  : The repository
+000013d0: 206d 7573 7420 6265 2067 6976 656e 2061   must be given a
+000013e0: 7320 6120 7265 6c61 7469 7665 2070 6174  s a relative pat
+000013f0: 682e 722f 0000 007a 022e 2e72 3000 0000  h.r/...z...r0...
+00001400: da0d 696e 6974 5f61 6e61 6c79 7369 7363  ..init_analysisc
+00001410: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001420: 0400 0000 1300 0000 730c 0000 007c 00a0  ........s....|..
+00001430: 0088 0188 00a1 0253 0072 1a00 0000 2901  .......S.r....).
+00001440: 723c 0000 0072 3200 0000 a902 da0b 6465  r<...r2.......de
+00001450: 7363 7269 7074 696f 6eda 0670 6172 656e  scription..paren
+00001460: 7472 1200 0000 7213 0000 0072 3600 0000  tr....r....r6...
+00001470: 5e00 0000 f302 0000 000c 007a 2469 6e69  ^..........z$ini
+00001480: 745f 616e 616c 7973 6973 5f69 6d70 6c2e  t_analysis_impl.
+00001490: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+000014a0: 3e29 0a72 0800 0000 7218 0000 00da 026f  >).r....r......o
+000014b0: 73da 0470 6174 68da 0569 7361 6273 da06  s..path..isabs..
+000014c0: 6765 7463 7764 da04 6a6f 696e da07 7265  getcwd..join..re
+000014d0: 6c70 6174 6872 2a00 0000 7238 0000 0029  lpathr*...r8...)
+000014e0: 0672 2b00 0000 723f 0000 0072 3900 0000  .r+...r?...r9...
+000014f0: 723e 0000 00da 0a70 6172 656e 745f 6469  r>.....parent_di
+00001500: 72da 0c61 6e61 6c79 7369 735f 6469 7272  r..analysis_dirr
+00001510: 1200 0000 723d 0000 0072 1300 0000 da12  ....r=...r......
+00001520: 696e 6974 5f61 6e61 6c79 7369 735f 696d  init_analysis_im
+00001530: 706c 5100 0000 731e 0000 000e 0114 0108  plQ...s.........
+00001540: 0104 0114 0108 0104 0110 0122 0112 010e  ..........."....
+00001550: 0110 0118 0102 0104 ff72 4900 0000 6300  .........rI...c.
+00001560: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00001570: 0000 0040 0000 0073 2000 0000 6500 5a01  ...@...s ...e.Z.
+00001580: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
+00001590: 6404 6405 8400 5a05 6406 5300 2907 da0b  d.d...Z.d.S.)...
+000015a0: 5365 7474 696e 6773 4765 74da 0c73 6574  SettingsGet..set
+000015b0: 7469 6e67 735f 6765 7463 0400 0000 0000  tings_getc......
+000015c0: 0000 0000 0000 0500 0000 0600 0000 4300  ..............C.
+000015d0: 0000 7336 0000 007a 0f74 0074 0164 0164  ..s6...z.t.t.d.d
+000015e0: 0284 007c 01a0 0264 03a1 0183 0283 017d  ...|...d.......}
+000015f0: 047c 0457 0053 0001 0001 0001 007c 00a0  .|.W.S.......|..
+00001600: 037c 02a1 0101 0059 0064 0053 0029 044e  .|.....Y.d.S.).N
+00001610: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001620: 0002 0000 0053 0000 00f3 0c00 0000 7400  .....S........t.
+00001630: 7c00 8301 6401 6b04 5300 a902 4e72 0100  |...d.k.S...Nr..
+00001640: 0000 a901 da03 6c65 6ea9 01da 0474 6572  ......len....ter
+00001650: 6d72 1200 0000 7212 0000 0072 1300 0000  mr....r....r....
+00001660: 7236 0000 006a 0000 0072 4000 0000 7a25  r6...j...r@...z%
+00001670: 5365 7474 696e 6773 4765 742e 636f 6e76  SettingsGet.conv
+00001680: 6572 742e 3c6c 6f63 616c 733e 2e3c 6c61  ert.<locals>.<la
+00001690: 6d62 6461 3efa 012c 2904 da04 6c69 7374  mbda>..,)...list
+000016a0: da06 6669 6c74 6572 da05 7370 6c69 74da  ..filter..split.
+000016b0: 055f 6661 696c 2905 da04 7365 6c66 da05  ._fail)...self..
+000016c0: 7661 6c75 6572 1d00 0000 722b 0000 0072  valuer....r+...r
+000016d0: 5500 0000 7212 0000 0072 1200 0000 7213  U...r....r....r.
+000016e0: 0000 00da 0763 6f6e 7665 7274 6800 0000  .....converth...
+000016f0: 730a 0000 0002 0118 0106 0106 0110 017a  s..............z
+00001700: 1353 6574 7469 6e67 7347 6574 2e63 6f6e  .SettingsGet.con
+00001710: 7665 7274 6302 0000 0000 0000 0000 0000  vertc...........
+00001720: 0002 0000 0004 0000 0043 0000 00f3 1200  .........C......
+00001730: 0000 7c00 6a00 7c01 6401 6402 8d02 0100  ..|.j.|.d.d.....
+00001740: 6400 5300 2903 4e7a 2f53 6574 7469 6e67  d.S.).Nz/Setting
+00001750: 7320 6d75 7374 2062 6520 696e 2074 6865  s must be in the
+00001760: 2066 6f72 6d61 743a 206b 6579 312c 206b   format: key1, k
+00001770: 6579 322c 202e 2e2e a902 721d 0000 0072  ey2, .....r....r
+00001780: 0f00 0000 a901 da04 6661 696c a902 7257  ........fail..rW
+00001790: 0000 0072 1d00 0000 7212 0000 0072 1200  ...r....r....r..
+000017a0: 0000 7213 0000 0072 5600 0000 6f00 0000  ..r....rV...o...
+000017b0: f306 0000 0004 0104 010a ff7a 1153 6574  ...........z.Set
+000017c0: 7469 6e67 7347 6574 2e5f 6661 696c 4e29  tingsGet._failN)
+000017d0: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000017e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000017f0: 616d 655f 5fda 046e 616d 6572 5900 0000  ame__..namerY...
+00001800: 7256 0000 0072 1200 0000 7212 0000 0072  rV...r....r....r
+00001810: 1200 0000 7213 0000 0072 4a00 0000 6500  ....r....rJ...e.
+00001820: 0000 7308 0000 0008 0004 0108 020c 0772  ..s............r
+00001830: 4a00 0000 6300 0000 0000 0000 0000 0000  J...c...........
+00001840: 0000 0000 0001 0000 0040 0000 0073 0c00  .........@...s..
+00001850: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
+00001860: da0d 5365 7474 696e 6773 436c 6561 724e  ..SettingsClearN
+00001870: 2903 7260 0000 0072 6100 0000 7262 0000  ).r`...ra...rb..
+00001880: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00001890: 7213 0000 0072 6400 0000 7400 0000 7304  r....rd...t...s.
+000018a0: 0000 0008 0004 0172 6400 0000 6300 0000  .......rd...c...
+000018b0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+000018c0: 0040 0000 0073 3000 0000 6500 5a01 6400  .@...s0...e.Z.d.
+000018d0: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
+000018e0: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
+000018f0: 6409 8400 5a07 640a 5300 290b da0b 5365  d...Z.d.S.)...Se
+00001900: 7474 696e 6773 5365 74da 0c73 6574 7469  ttingsSet..setti
+00001910: 6e67 735f 7365 7463 0400 0000 0000 0000  ngs_setc........
+00001920: 0000 0000 0900 0000 0600 0000 4300 0000  ............C...
+00001930: 738c 0000 007a 3a7c 00a0 007c 01a1 017d  s....z:|...|...}
+00001940: 0169 007d 0474 0174 0264 0164 0284 007c  .i.}.t.t.d.d...|
+00001950: 01a0 0364 03a1 0183 0283 017d 057c 0544  ...d.......}.|.D
+00001960: 005d 217d 067c 06a0 0364 04a1 017d 0774  .]!}.|...d...}.t
+00001970: 047c 0783 0164 056b 0372 287c 00a0 057c  .|...d.k.r(|...|
+00001980: 02a1 0101 007c 0764 0619 007d 087c 0764  .....|.d...}.|.d
+00001990: 0719 007d 017c 00a0 067c 01a1 017c 047c  ...}.|...|...|.|
+000019a0: 083c 0071 167c 0457 0053 0001 0001 0001  .<.q.|.W.S......
+000019b0: 007c 00a0 057c 02a1 0101 0059 0064 0053  .|...|.....Y.d.S
+000019c0: 0029 084e 6301 0000 0000 0000 0000 0000  .).Nc...........
+000019d0: 0001 0000 0002 0000 0053 0000 0072 4c00  .........S...rL.
+000019e0: 0000 724d 0000 0072 4e00 0000 7250 0000  ..rM...rN...rP..
+000019f0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001a00: 7236 0000 007f 0000 0072 4000 0000 7a25  r6.......r@...z%
+00001a10: 5365 7474 696e 6773 5365 742e 636f 6e76  SettingsSet.conv
+00001a20: 6572 742e 3c6c 6f63 616c 733e 2e3c 6c61  ert.<locals>.<la
+00001a30: 6d62 6461 3e72 5200 0000 fa01 3d72 0a00  mbda>rR.....=r..
+00001a40: 0000 7201 0000 0072 0600 0000 2907 da0c  ..r....r....)...
+00001a50: 5f65 6e63 6f64 655f 6a73 6f6e 7253 0000  _encode_jsonrS..
+00001a60: 0072 5400 0000 7255 0000 0072 4f00 0000  .rT...rU...rO...
+00001a70: 7256 0000 00da 0c5f 6465 636f 6465 5f6a  rV....._decode_j
+00001a80: 736f 6e29 0972 5700 0000 7258 0000 0072  son).rW...rX...r
+00001a90: 1d00 0000 722b 0000 00da 0873 6574 7469  ....r+.....setti
+00001aa0: 6e67 7372 5500 0000 da07 7365 7474 696e  ngsrU.....settin
+00001ab0: 67da 0d73 6574 7469 6e67 5f73 706c 6974  g..setting_split
+00001ac0: da03 6b65 7972 1200 0000 7212 0000 0072  ..keyr....r....r
+00001ad0: 1300 0000 7259 0000 007b 0000 0073 1c00  ....rY...{...s..
+00001ae0: 0000 0201 0a01 0401 1801 0801 0a01 0c01  ................
+00001af0: 0a01 0801 0801 1001 0601 0601 1001 7a13  ..............z.
+00001b00: 5365 7474 696e 6773 5365 742e 636f 6e76  SettingsSet.conv
+00001b10: 6572 7463 0200 0000 0000 0000 0000 0000  ertc............
+00001b20: 0700 0000 0600 0000 4300 0000 7362 0000  ........C...sb..
+00001b30: 0064 017d 0264 027d 0364 037d 047c 037d  .d.}.d.}.d.}.|.}
+00001b40: 057c 0144 005d 247d 067c 0664 046b 0272  .|.D.]$}.|.d.k.r
+00001b50: 137c 047d 056e 067c 0664 056b 0272 197c  .|.}.n.|.d.k.r.|
+00001b60: 037d 057c 057c 036b 0272 227c 027c 0637  .}.|.|.k.r"|.|.7
+00001b70: 007d 0271 0a7c 057c 046b 0272 2e7c 027c  .}.q.|.|.k.r.|.|
+00001b80: 06a0 0064 0664 07a1 0237 007d 0271 0a7c  ...d.d...7.}.q.|
+00001b90: 0253 0029 084e 722f 0000 0072 0100 0000  .S.).Nr/...r....
+00001ba0: 7206 0000 00da 017b da01 7d72 5200 0000  r......{..}rR...
+00001bb0: fa01 7ca9 01da 0772 6570 6c61 6365 2907  ..|....replace).
+00001bc0: 7257 0000 0072 5800 0000 da07 656e 636f  rW...rX.....enco
+00001bd0: 6465 64da 0453 4545 4bda 0645 4e43 4f44  ded..SEEK..ENCOD
+00001be0: 45da 046d 6f64 65da 0463 6861 7272 1200  E..mode..charr..
+00001bf0: 0000 7212 0000 0072 1300 0000 7268 0000  ..r....r....rh..
+00001c00: 008b 0000 0073 1e00 0000 0401 0401 0401  .....s..........
+00001c10: 0401 0801 0801 0601 0801 0401 0801 0a01  ................
+00001c20: 0801 1001 0280 0401 7a18 5365 7474 696e  ........z.Settin
+00001c30: 6773 5365 742e 5f65 6e63 6f64 655f 6a73  gsSet._encode_js
+00001c40: 6f6e 6302 0000 0000 0000 0000 0000 0002  onc.............
+00001c50: 0000 0004 0000 0043 0000 0073 0c00 0000  .......C...s....
+00001c60: 7c01 a000 6401 6402 a102 5300 2903 4e72  |...d.d...S.).Nr
+00001c70: 7000 0000 7252 0000 0072 7100 0000 2902  p...rR...rq...).
+00001c80: 7257 0000 0072 5800 0000 7212 0000 0072  rW...rX...r....r
+00001c90: 1200 0000 7213 0000 0072 6900 0000 9b00  ....r....ri.....
+00001ca0: 0000 7302 0000 000c 017a 1853 6574 7469  ..s......z.Setti
+00001cb0: 6e67 7353 6574 2e5f 6465 636f 6465 5f6a  ngsSet._decode_j
+00001cc0: 736f 6e63 0200 0000 0000 0000 0000 0000  sonc............
+00001cd0: 0200 0000 0400 0000 4300 0000 725a 0000  ........C...rZ..
+00001ce0: 0029 034e 7a3d 5365 7474 696e 6773 206d  .).Nz=Settings m
+00001cf0: 7573 7420 6265 2069 6e20 7468 6520 666f  ust be in the fo
+00001d00: 726d 6174 3a20 6b65 7931 3d76 616c 7565  rmat: key1=value
+00001d10: 312c 206b 6579 323d 7661 6c75 6532 2c20  1, key2=value2, 
+00001d20: 2e2e 2e72 5b00 0000 725c 0000 0072 5e00  ...r[...r\...r^.
+00001d30: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00001d40: 0072 5600 0000 9e00 0000 725f 0000 007a  .rV.......r_...z
+00001d50: 1153 6574 7469 6e67 7353 6574 2e5f 6661  .SettingsSet._fa
+00001d60: 696c 4e29 0872 6000 0000 7261 0000 0072  ilN).r`...ra...r
+00001d70: 6200 0000 7263 0000 0072 5900 0000 7268  b...rc...rY...rh
+00001d80: 0000 0072 6900 0000 7256 0000 0072 1200  ...ri...rV...r..
+00001d90: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00001da0: 0072 6500 0000 7800 0000 730c 0000 0008  .re...x...s.....
+00001db0: 0004 0108 0208 1008 100c 0372 6500 0000  ...........re...
+00001dc0: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00001dd0: 0005 0000 0043 0000 0073 2c00 0000 6900  .....C...s,...i.
+00001de0: 7d01 7c00 4400 5d0f 7d02 7c02 a000 a100  }.|.D.].}.|.....
+00001df0: 4400 5d08 5c02 7d03 7d04 7c04 7c01 7c03  D.].\.}.}.|.|.|.
+00001e00: 3c00 710a 7104 7c01 5300 721a 0000 0029  <.q.q.|.S.r....)
+00001e10: 01da 0569 7465 6d73 2905 da0d 7365 7474  ...items)...sett
+00001e20: 696e 675f 6469 6374 73da 066a 6f69 6e65  ing_dicts..joine
+00001e30: 64da 0c73 6574 7469 6e67 5f64 6963 7472  d..setting_dictr
+00001e40: 6d00 0000 7258 0000 0072 1200 0000 7212  m...rX...r....r.
+00001e50: 0000 0072 1300 0000 da12 5f6a 6f69 6e5f  ...r......_join_
+00001e60: 7365 7474 696e 6773 5f73 6574 a300 0000  settings_set....
+00001e70: 730c 0000 0004 0108 0110 010a 0102 ff04  s...............
+00001e80: 0272 7c00 0000 6301 0000 0000 0000 0000  .r|...c.........
+00001e90: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
+00001ea0: 1a00 0000 6700 7d01 7c00 4400 5d06 7d02  ....g.}.|.D.].}.
+00001eb0: 7c01 7c02 3700 7d01 7104 7c01 5300 721a  |.|.7.}.q.|.S.r.
+00001ec0: 0000 0072 1200 0000 2903 da0d 7365 7474  ...r....)...sett
+00001ed0: 696e 675f 6c69 7374 7372 7a00 0000 da0c  ing_listsrz.....
+00001ee0: 7365 7474 696e 675f 6c69 7374 7212 0000  setting_listr...
+00001ef0: 0072 1200 0000 7213 0000 00da 125f 6a6f  .r....r......_jo
+00001f00: 696e 5f73 6574 7469 6e67 735f 6765 74ab  in_settings_get.
+00001f10: 0000 0073 0800 0000 0401 0801 0a01 0401  ...s............
+00001f20: 727f 0000 0063 0400 0000 0000 0000 0000  r....c..........
+00001f30: 0000 0800 0000 0800 0000 4300 0000 7350  ..........C...sP
+00001f40: 0000 007c 006a 0064 0119 007d 047c 006a  ...|.j.d...}.|.j
+00001f50: 0064 0219 007d 057c 006a 0064 0319 007d  .d...}.|.j.d...}
+00001f60: 0664 047d 0764 057c 006a 0076 0072 1b7c  .d.}.d.|.j.v.r.|
+00001f70: 006a 0064 0519 007d 077c 056a 017c 067c  .j.d...}.|.j.|.|
+00001f80: 047c 077c 017c 027c 0364 068d 0601 0064  .|.|.|.|.d.....d
+00001f90: 0053 0029 074e da09 6973 5f67 6c6f 6261  .S.).N..is_globa
+00001fa0: 6c72 3000 0000 da08 7265 736f 6c76 6572  lr0.....resolver
+00001fb0: 46da 1469 735f 6461 7461 5f73 6574 5f70  F..is_data_set_p
+00001fc0: 726f 7065 7274 79a9 02da 0470 726f 7072  roperty....propr
+00001fd0: 5800 0000 2902 722a 0000 00da 0663 6f6e  X...).r*.....con
+00001fe0: 6669 6729 0872 2b00 0000 da0e 6f70 6572  fig).r+.....oper
+00001ff0: 6174 696f 6e5f 7479 7065 7284 0000 0072  ation_typer....r
+00002000: 5800 0000 7280 0000 0072 3000 0000 7281  X...r....r0...r.
+00002010: 0000 0072 8200 0000 7212 0000 0072 1200  ...r....r....r..
+00002020: 0000 7213 0000 00da 105f 6163 6365 7373  ..r......_access
+00002030: 5f73 6574 7469 6e67 73b2 0000 0073 1200  _settings....s..
+00002040: 0000 0a01 0a01 0a01 0401 0a01 0a01 0c01  ................
+00002050: 0401 0aff 7287 0000 0063 0200 0000 0000  ....r....c......
+00002060: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
+00002070: 0000 7338 0000 0074 007c 0183 017d 027c  ..s8...t.|...}.|
+00002080: 02a0 01a1 0044 005d 0d5c 027d 037d 0474  .....D.].\.}.}.t
+00002090: 027c 0074 036a 047c 037c 0464 018d 0401  .|.t.j.|.|.d....
+000020a0: 0071 0874 0564 0264 0364 048d 0253 0029  .q.t.d.d.d...S.)
+000020b0: 054e 7283 0000 0072 0100 0000 722f 0000  .Nr....r....r/..
+000020c0: 00a9 02da 0a72 6574 7572 6e63 6f64 65da  .....returncode.
+000020d0: 066f 7574 7075 7429 0672 7c00 0000 7278  .output).r|...rx
+000020e0: 0000 0072 8700 0000 720c 0000 00da 0353  ...r....r......S
+000020f0: 4554 720b 0000 0029 0572 2b00 0000 726a  ETr....).r+...rj
+00002100: 0000 00da 0d73 6574 7469 6e67 735f 6469  .....settings_di
+00002110: 6374 7284 0000 0072 5800 0000 7212 0000  ctr....rX...r...
+00002120: 0072 1200 0000 7213 0000 00da 045f 7365  .r....r......_se
+00002130: 74bd 0000 0073 0800 0000 0801 1001 1401  t....s..........
+00002140: 0c01 728d 0000 0063 0200 0000 0000 0000  ..r....c........
+00002150: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00002160: f340 0000 0074 007c 0183 017d 0274 017c  .@...t.|...}.t.|
+00002170: 0283 0164 016b 0272 0d64 0067 017d 027c  ...d.k.r.d.g.}.|
+00002180: 0244 005d 0a7d 0374 027c 0074 036a 047c  .D.].}.t.|.t.j.|
+00002190: 0364 028d 0301 0071 0f74 0564 0164 0364  .d.....q.t.d.d.d
+000021a0: 048d 0253 00a9 054e 7201 0000 0029 0172  ...S...Nr....).r
+000021b0: 8400 0000 722f 0000 0072 8800 0000 2906  ....r/...r....).
+000021c0: 727f 0000 0072 4f00 0000 7287 0000 0072  r....rO...r....r
+000021d0: 0c00 0000 da03 4745 5472 0b00 0000 a904  ......GETr......
+000021e0: 722b 0000 0072 6a00 0000 da0d 7365 7474  r+...rj.....sett
+000021f0: 696e 6773 5f6c 6973 7472 8400 0000 7212  ings_listr....r.
+00002200: 0000 0072 1200 0000 7213 0000 00da 045f  ...r....r......_
+00002210: 6765 74c4 0000 00f3 0c00 0000 0801 0c01  get.............
+00002220: 0601 0801 1201 0c01 7293 0000 0063 0200  ........r....c..
+00002230: 0000 0000 0000 0000 0000 0400 0000 0600  ................
+00002240: 0000 4300 0000 728e 0000 0072 8f00 0000  ..C...r....r....
+00002250: 2906 727f 0000 0072 4f00 0000 7287 0000  ).r....rO...r...
+00002260: 0072 0c00 0000 da05 434c 4541 5272 0b00  .r......CLEARr..
+00002270: 0000 7291 0000 0072 1200 0000 7212 0000  ..r....r....r...
+00002280: 0072 1300 0000 da06 5f63 6c65 6172 cd00  .r......_clear..
+00002290: 0000 7294 0000 0072 9600 0000 7a02 2d67  ..r....r....z.-g
+000022a0: 7a0b 2d2d 6973 5f67 6c6f 6261 6c7a 1447  z.--is_globalz.G
+000022b0: 6574 2067 6c6f 6261 6c20 6f72 206c 6f63  et global or loc
+000022c0: 616c 2e63 0200 0000 0000 0000 0000 0000  al.c............
+000022d0: 0200 0000 0300 0000 4300 0000 730e 0000  ........C...s...
+000022e0: 007c 017c 006a 0064 013c 0064 0253 0029  .|.|.j.d.<.d.S.)
+000022f0: 037a 2820 4578 7465 726e 616c 2044 6174  .z( External Dat
+00002300: 6120 5374 6f72 653a 2047 6574 2061 6c6c  a Store: Get all
+00002310: 2073 6574 7469 6e67 732e 2072 8000 0000   settings. r....
+00002320: 4e72 2900 0000 2902 722b 0000 0072 8000  Nr)...).r+...r..
+00002330: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00002340: 0072 6a00 0000 d800 0000 f302 0000 000e  .rj.............
+00002350: 0572 6a00 0000 da03 6765 7463 0100 0000  .rj.....getc....
+00002360: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+00002370: 4300 0000 733a 0000 0074 007c 006a 0164  C...s:...t.|.j.d
+00002380: 0164 028d 027d 017c 01a0 02a1 007d 0274  .d...}.|.....}.t
+00002390: 036a 047c 0264 0364 0464 058d 037d 0374  .j.|.d.d.d...}.t
+000023a0: 05a0 0664 06a0 077c 03a1 01a1 0101 0064  ...d...|.......d
+000023b0: 0753 0029 087a 2320 4578 7465 726e 616c  .S.).z# External
+000023c0: 2044 6174 6120 5374 6f72 653a 2047 6574   Data Store: Get
+000023d0: 2073 6574 7469 6e67 2e20 46a9 01da 1168   setting. F....h
+000023e0: 616c 745f 6f6e 5f65 7272 6f72 5f6c 6f67  alt_on_error_log
+000023f0: e904 0000 0054 2902 da06 696e 6465 6e74  .....T)...indent
+00002400: da09 736f 7274 5f6b 6579 7372 1500 0000  ..sort_keysr....
+00002410: 4e29 0872 0900 0000 722a 0000 00da 0c67  N).r....r*.....g
+00002420: 6574 5f73 6574 7469 6e67 73da 046a 736f  et_settings..jso
+00002430: 6eda 0564 756d 7073 7216 0000 0072 1700  n..dumpsr....r..
+00002440: 0000 7218 0000 0029 0472 2b00 0000 7230  ..r....).r+...r0
+00002450: 0000 0072 6a00 0000 da0c 7365 7474 696e  ...rj.....settin
+00002460: 6773 5f73 7472 7212 0000 0072 1200 0000  gs_strr....r....
+00002470: 7213 0000 0072 4b00 0000 e000 0000 7308  r....rK.......s.
+00002480: 0000 000e 0408 0110 0114 0172 4b00 0000  ...........rK...
+00002490: 7a18 5365 742f 6765 7420 676c 6f62 616c  z.Set/get global
+000024a0: 206f 7220 6c6f 6361 6c2e 6302 0000 0000   or local.c.....
+000024b0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+000024c0: 0000 00f3 3000 0000 7400 7c00 6a01 6401  ....0...t.|.j.d.
+000024d0: 6402 8d02 7d02 7c01 7c00 6a01 6403 3c00  d...}.|.|.j.d.<.
+000024e0: 7c02 7c00 6a01 6404 3c00 6405 7c00 6a01  |.|.j.d.<.d.|.j.
+000024f0: 6406 3c00 6407 5300 2908 7a42 2045 7874  d.<.d.S.).zB Ext
+00002500: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00002510: 3a20 4765 742f 7365 7420 7365 7474 696e  : Get/set settin
+00002520: 6773 2072 656c 6174 6564 2074 6f20 7468  gs related to th
+00002530: 6520 7265 706f 7369 746f 7279 2e20 4672  e repository. Fr
+00002540: 9900 0000 7280 0000 0072 3000 0000 7239  ....r....r0...r9
+00002550: 0000 0072 8100 0000 4ea9 0272 0900 0000  ...r....N..r....
+00002560: 722a 0000 00a9 0372 2b00 0000 7280 0000  r*.....r+...r...
+00002570: 0072 3000 0000 7212 0000 0072 1200 0000  .r0...r....r....
+00002580: 7213 0000 0072 3900 0000 ec00 0000 7308  r....r9.......s.
+00002590: 0000 000e 050a 010a 010e 0172 3900 0000  ...........r9...
+000025a0: da03 7365 7472 3b00 0000 2902 720d 0000  ..setr;...).r...
+000025b0: 00da 056e 6172 6773 6302 0000 0000 0000  ...nargsc.......
+000025c0: 0000 0000 0002 0000 0006 0000 0003 0000  ................
+000025d0: 00f3 1c00 0000 8800 6a00 6401 1900 a001  ........j.d.....
+000025e0: 6402 8700 8701 6602 6403 6404 8408 a102  d.....f.d.d.....
+000025f0: 5300 2905 7a3e 2045 7874 6572 6e61 6c20  S.).z> External 
+00002600: 4461 7461 2053 746f 7265 3a20 5365 7420  Data Store: Set 
+00002610: 7365 7474 696e 6773 2072 656c 6174 6564  settings related
+00002620: 2074 6f20 7468 6520 7265 706f 7369 746f   to the reposito
+00002630: 7279 2e20 7230 0000 00da 0e72 6570 6f73  ry. r0.....repos
+00002640: 6974 6f72 795f 7365 7463 0100 0000 0000  itory_setc......
+00002650: 0000 0000 0000 0100 0000 0300 0000 1300  ................
+00002660: 0000 f30a 0000 0074 0088 0088 0183 0253  .......t.......S
+00002670: 0072 1a00 0000 a901 728d 0000 0072 3200  .r......r....r2.
+00002680: 0000 a902 722b 0000 0072 6a00 0000 7212  ....r+...rj...r.
+00002690: 0000 0072 1300 0000 7236 0000 00fc 0000  ...r....r6......
+000026a0: 0072 3700 0000 7a20 7265 706f 7369 746f  .r7...z reposito
+000026b0: 7279 5f73 6574 2e3c 6c6f 6361 6c73 3e2e  ry_set.<locals>.
+000026c0: 3c6c 616d 6264 613e a902 722a 0000 0072  <lambda>..r*...r
+000026d0: 3800 0000 72ab 0000 0072 1200 0000 72ab  8...r....r....r.
+000026e0: 0000 0072 1300 0000 72a8 0000 00f7 0000  ...r....r.......
+000026f0: 00f3 0200 0000 1c05 72a8 0000 0063 0200  ........r....c..
+00002700: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00002710: 0000 0300 0000 72a7 0000 0029 057a 3e20  ......r....).z> 
+00002720: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
+00002730: 6f72 653a 2047 6574 2073 6574 7469 6e67  ore: Get setting
+00002740: 7320 7265 6c61 7465 6420 746f 2074 6865  s related to the
+00002750: 2072 6570 6f73 6974 6f72 792e 2072 3000   repository. r0.
+00002760: 0000 da0e 7265 706f 7369 746f 7279 5f67  ....repository_g
+00002770: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
+00002780: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
+00002790: 721a 0000 00a9 0172 9300 0000 7232 0000  r......r....r2..
+000027a0: 0072 ab00 0000 7212 0000 0072 1300 0000  .r....r....r....
+000027b0: 7236 0000 0004 0100 0072 3700 0000 7a20  r6.......r7...z 
+000027c0: 7265 706f 7369 746f 7279 5f67 6574 2e3c  repository_get.<
+000027d0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+000027e0: 72ac 0000 0072 ab00 0000 7212 0000 0072  r....r....r....r
+000027f0: ab00 0000 7213 0000 0072 ae00 0000 ff00  ....r....r......
+00002800: 0000 72ad 0000 0072 ae00 0000 da05 636c  ..r....r......cl
+00002810: 6561 7263 0200 0000 0000 0000 0000 0000  earc............
+00002820: 0200 0000 0600 0000 0300 0000 72a7 0000  ............r...
+00002830: 0029 057a 4020 4578 7465 726e 616c 2044  .).z@ External D
+00002840: 6174 6120 5374 6f72 653a 2043 6c65 6172  ata Store: Clear
+00002850: 2073 6574 7469 6e67 7320 7265 6c61 7465   settings relate
+00002860: 6420 746f 2074 6865 2072 6570 6f73 6974  d to the reposit
+00002870: 6f72 792e 2072 3000 0000 da10 7265 706f  ory. r0.....repo
+00002880: 7369 746f 7279 5f63 6c65 6172 6301 0000  sitory_clearc...
+00002890: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000028a0: 0013 0000 0072 a900 0000 721a 0000 00a9  .....r....r.....
+000028b0: 0172 9600 0000 7232 0000 0072 ab00 0000  .r....r2...r....
+000028c0: 7212 0000 0072 1300 0000 7236 0000 000c  r....r....r6....
+000028d0: 0100 0072 3700 0000 7a22 7265 706f 7369  ...r7...z"reposi
+000028e0: 746f 7279 5f63 6c65 6172 2e3c 6c6f 6361  tory_clear.<loca
+000028f0: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
+00002900: 0072 ab00 0000 7212 0000 0072 ab00 0000  .r....r....r....
+00002910: 7213 0000 0072 b100 0000 0701 0000 72ad  r....r........r.
+00002920: 0000 0072 b100 0000 7a0c 2d6f 626a 6563  ...r....z.-objec
+00002930: 745f 7479 7065 7a0d 2d2d 6f62 6a65 6374  t_typez.--object
+00002940: 5f74 7970 65da 0974 7970 655f 636f 6465  _type..type_code
+00002950: 7a1d 4f62 6a65 6374 2074 7970 6520 636f  z.Object type co
+00002960: 6465 2074 6f20 6669 6c74 6572 2062 7929  de to filter by)
+00002970: 0272 2300 0000 7225 0000 007a 062d 7370  .r#...r%...z.-sp
+00002980: 6163 657a 072d 2d73 7061 6365 7a0a 5370  acez.--spacez.Sp
+00002990: 6163 6520 636f 6465 7a08 2d70 726f 6a65  ace codez.-proje
+000029a0: 6374 7a09 2d2d 7072 6f6a 6563 747a 2046  ctz.--projectz F
+000029b0: 756c 6c20 7072 6f6a 6563 7420 6964 656e  ull project iden
+000029c0: 7469 6669 6361 7469 6f6e 2063 6f64 657a  tification codez
+000029d0: 0b2d 6578 7065 7269 6d65 6e74 7a0c 2d2d  .-experimentz.--
+000029e0: 6578 7065 7269 6d65 6e74 7a14 4675 6c6c  experimentz.Full
+000029f0: 2065 7870 6572 696d 656e 7420 636f 6465   experiment code
+00002a00: 7a07 2d6f 626a 6563 747a 082d 2d6f 626a  z.-objectz.--obj
+00002a10: 6563 74da 0b6f 626a 6563 745f 636f 6465  ect..object_code
+00002a20: 7a41 4f62 6a65 6374 2069 6465 6e74 6966  zAObject identif
+00002a30: 6963 6174 696f 6e20 696e 666f 726d 6174  ication informat
+00002a40: 696f 6e2c 2069 7420 6361 6e20 6265 2070  ion, it can be p
+00002a50: 6572 6d49 6420 6f72 2069 6465 6e74 6966  ermId or identif
+00002a60: 6965 727a 052d 7479 7065 7a06 2d2d 7479  ierz.-typez.--ty
+00002a70: 7065 7a09 5479 7065 2063 6f64 657a 092d  pez.Type codez.-
+00002a80: 7072 6f70 6572 7479 da0d 7072 6f70 6572  property..proper
+00002a90: 7479 5f63 6f64 657a 0d50 726f 7065 7274  ty_codez.Propert
+00002aa0: 7920 636f 6465 7a0f 2d70 726f 7065 7274  y codez.-propert
+00002ab0: 792d 7661 6c75 65da 0e70 726f 7065 7274  y-value..propert
+00002ac0: 795f 7661 6c75 657a 0e50 726f 7065 7274  y_valuez.Propert
+00002ad0: 7920 7661 6c75 657a 122d 7265 6769 7374  y valuez.-regist
+00002ae0: 7261 7469 6f6e 2d64 6174 657a 132d 2d72  ration-datez.--r
+00002af0: 6567 6973 7472 6174 696f 6e2d 6461 7465  egistration-date
+00002b00: da11 7265 6769 7374 7261 7469 6f6e 5f64  ..registration_d
+00002b10: 6174 657a 4d52 6567 6973 7472 6174 696f  atezMRegistratio
+00002b20: 6e20 6461 7465 2c20 6974 2063 616e 2062  n date, it can b
+00002b30: 6520 696e 2074 6865 2066 6f72 6d61 7420  e in the format 
+00002b40: 226f 5959 5959 2d4d 4d2d 4444 2220 2865  "oYYYY-MM-DD" (e
+00002b50: 2e67 2e20 223e 3230 3233 2d30 312d 3031  .g. ">2023-01-01
+00002b60: 2229 7a12 2d6d 6f64 6966 6963 6174 696f  ")z.-modificatio
+00002b70: 6e2d 6461 7465 7a13 2d2d 6d6f 6469 6669  n-datez.--modifi
+00002b80: 6361 7469 6f6e 2d64 6174 65da 116d 6f64  cation-date..mod
+00002b90: 6966 6963 6174 696f 6e5f 6461 7465 7a4d  ification_datezM
+00002ba0: 4d6f 6469 6669 6361 7469 6f6e 2064 6174  Modification dat
+00002bb0: 652c 2069 7420 6361 6e20 6265 2069 6e20  e, it can be in 
+00002bc0: 7468 6520 666f 726d 6174 2022 6f59 5959  the format "oYYY
+00002bd0: 592d 4d4d 2d44 4422 2028 652e 672e 2022  Y-MM-DD" (e.g. "
+00002be0: 3e32 3032 332d 3031 2d30 3122 297a 052d  >2023-01-01")z.-
+00002bf0: 7361 7665 7a06 2d2d 7361 7665 7a18 4669  savez.--savez.Fi
+00002c00: 6c65 6e61 6d65 2074 6f20 7361 7665 2072  lename to save r
+00002c10: 6573 756c 7473 7a02 2d72 7a0b 2d2d 7265  esultsz.-rz.--re
+00002c20: 6375 7273 6976 65da 0972 6563 7572 7369  cursive..recursi
+00002c30: 7665 7a17 5365 6172 6368 2064 6174 6120  vez.Search data 
+00002c40: 7265 6375 7273 6976 656c 7929 0372 2400  recursively).r$.
+00002c50: 0000 7223 0000 0072 2500 0000 da08 6461  ..r#...r%.....da
+00002c60: 7461 5f73 6574 7a02 2d70 7a16 2d2d 6973  ta_setz.-pz.--is
+00002c70: 5f64 6174 615f 7365 745f 7072 6f70 6572  _data_set_proper
+00002c80: 7479 7a1c 436f 6e66 6967 7572 6520 6461  tyz.Configure da
+00002c90: 7461 2073 6574 2070 726f 7065 7274 792e  ta set property.
+00002ca0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
+00002cb0: 0004 0000 0043 0000 0073 3a00 0000 7400  .....C...s:...t.
+00002cc0: 7c00 6a01 6401 6402 8d02 7d03 7c01 7c00  |.j.d.d...}.|.|.
+00002cd0: 6a01 6403 3c00 7c02 7c00 6a01 6404 3c00  j.d.<.|.|.j.d.<.
+00002ce0: 7c03 7c00 6a01 6405 3c00 6406 7c00 6a01  |.|.j.d.<.d.|.j.
+00002cf0: 6407 3c00 6408 5300 2909 7a40 2045 7874  d.<.d.S.).z@ Ext
+00002d00: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00002d10: 3a20 4765 742f 7365 7420 7365 7474 696e  : Get/set settin
+00002d20: 6773 2072 656c 6174 6564 2074 6f20 7468  gs related to th
+00002d30: 6520 6461 7461 2073 6574 2e20 4672 9900  e data set. Fr..
+00002d40: 0000 7280 0000 0072 8200 0000 7230 0000  ..r....r....r0..
+00002d50: 0072 ba00 0000 7281 0000 004e 72a3 0000  .r....r....Nr...
+00002d60: 0029 0472 2b00 0000 7280 0000 0072 8200  .).r+...r....r..
+00002d70: 0000 7230 0000 0072 1200 0000 7212 0000  ..r0...r....r...
+00002d80: 0072 1300 0000 72ba 0000 0028 0100 0073  .r....r....(...s
+00002d90: 0a00 0000 0e07 0a01 0a01 0a01 0e01 da11  ................
+00002da0: 6461 7461 5f73 6574 5f73 6574 7469 6e67  data_set_setting
+00002db0: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+00002dc0: 0000 0600 0000 0300 0000 72a7 0000 0029  ..........r....)
+00002dd0: 057a 3c20 4578 7465 726e 616c 2044 6174  .z< External Dat
+00002de0: 6120 5374 6f72 653a 2053 6574 2073 6574  a Store: Set set
+00002df0: 7469 6e67 7320 7265 6c61 7465 6420 746f  tings related to
+00002e00: 2074 6865 2064 6174 6120 7365 742e 2072   the data set. r
+00002e10: 3000 0000 da0c 6461 7461 5f73 6574 5f73  0.....data_set_s
+00002e20: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
+00002e30: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
+00002e40: 721a 0000 0072 aa00 0000 7232 0000 00a9  r....r....r2....
+00002e50: 0272 2b00 0000 72bb 0000 0072 1200 0000  .r+...r....r....
+00002e60: 7213 0000 0072 3600 0000 3b01 0000 7237  r....r6...;...r7
+00002e70: 0000 007a 1e64 6174 615f 7365 745f 7365  ...z.data_set_se
+00002e80: 742e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  t.<locals>.<lamb
+00002e90: 6461 3e72 ac00 0000 72bd 0000 0072 1200  da>r....r....r..
+00002ea0: 0000 72bd 0000 0072 1300 0000 72bc 0000  ..r....r....r...
+00002eb0: 0036 0100 0072 ad00 0000 72bc 0000 0063  .6...r....r....c
+00002ec0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002ed0: 0600 0000 0300 0000 72a7 0000 0029 057a  ........r....).z
+00002ee0: 3c20 4578 7465 726e 616c 2044 6174 6120  < External Data 
+00002ef0: 5374 6f72 653a 2047 6574 2073 6574 7469  Store: Get setti
+00002f00: 6e67 7320 7265 6c61 7465 6420 746f 2074  ngs related to t
+00002f10: 6865 2064 6174 6120 7365 742e 2072 3000  he data set. r0.
+00002f20: 0000 da0c 6461 7461 5f73 6574 5f67 6574  ....data_set_get
+00002f30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002f40: 0003 0000 0013 0000 0072 a900 0000 721a  .........r....r.
+00002f50: 0000 0072 af00 0000 7232 0000 0072 bd00  ...r....r2...r..
+00002f60: 0000 7212 0000 0072 1300 0000 7236 0000  ..r....r....r6..
+00002f70: 0043 0100 0072 3700 0000 7a1e 6461 7461  .C...r7...z.data
+00002f80: 5f73 6574 5f67 6574 2e3c 6c6f 6361 6c73  _set_get.<locals
+00002f90: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
+00002fa0: bd00 0000 7212 0000 0072 bd00 0000 7213  ....r....r....r.
+00002fb0: 0000 0072 be00 0000 3e01 0000 72ad 0000  ...r....>...r...
+00002fc0: 0072 be00 0000 6302 0000 0000 0000 0000  .r....c.........
+00002fd0: 0000 0002 0000 0006 0000 0003 0000 0072  ...............r
+00002fe0: a700 0000 2905 7a3e 2045 7874 6572 6e61  ....).z> Externa
+00002ff0: 6c20 4461 7461 2053 746f 7265 3a20 436c  l Data Store: Cl
+00003000: 6561 7220 7365 7474 696e 6773 2072 656c  ear settings rel
+00003010: 6174 6564 2074 6f20 7468 6520 6461 7461  ated to the data
+00003020: 2073 6574 2e20 7230 0000 00da 0e64 6174   set. r0.....dat
+00003030: 615f 7365 745f 636c 6561 7263 0100 0000  a_set_clearc....
+00003040: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00003050: 1300 0000 72a9 0000 0072 1a00 0000 72b2  ....r....r....r.
+00003060: 0000 0072 3200 0000 72bd 0000 0072 1200  ...r2...r....r..
+00003070: 0000 7213 0000 0072 3600 0000 4b01 0000  ..r....r6...K...
+00003080: 7237 0000 007a 2064 6174 615f 7365 745f  r7...z data_set_
+00003090: 636c 6561 722e 3c6c 6f63 616c 733e 2e3c  clear.<locals>.<
+000030a0: 6c61 6d62 6461 3e72 ac00 0000 72bd 0000  lambda>r....r...
+000030b0: 0072 1200 0000 72bd 0000 0072 1300 0000  .r....r....r....
+000030c0: 72bf 0000 0046 0100 0072 ad00 0000 72bf  r....F...r....r.
+000030d0: 0000 00da 0673 6561 7263 687a 2f53 6561  .....searchz/Sea
+000030e0: 7263 6820 666f 7220 6461 7461 7365 7473  rch for datasets
+000030f0: 2075 7369 6e67 2061 2066 696c 7465 7269   using a filteri
+00003100: 6e67 2063 7269 7465 7269 612e 2901 da0a  ng criteria.)...
+00003110: 7368 6f72 745f 6865 6c70 630c 0000 0000  short_helpc.....
+00003120: 0000 0000 0000 000d 0000 000a 0000 0003  ................
+00003130: 0000 0073 de00 0000 7c01 7c02 7c03 7c04  ...s....|.|.|.|.
+00003140: 7c05 7c06 7c08 7c09 6708 7d0c 7400 6401  |.|.|.|.g.}.t.d.
+00003150: 6402 8400 7c0c 7c07 6701 1700 4400 8301  d...|.|.g...D...
+00003160: 8301 721c 7401 6403 8301 0100 6404 5300  ..r.t.d.....d.S.
+00003170: 7c08 6405 7500 7224 7c09 6405 7501 732c  |.d.u.r$|.d.u.s,
+00003180: 7c08 6405 7501 7232 7c09 6405 7500 7232  |.d.u.r2|.d.u.r2
+00003190: 7401 6406 8301 0100 6404 5300 7402 7c00  t.d.....d.S.t.|.
+000031a0: 6a03 6407 6408 8d02 7c00 6a03 6409 3c00  j.d.d...|.j.d.<.
+000031b0: 7c07 6405 7501 7253 7404 640a 6402 8400  |.d.u.rSt.d.d...
+000031c0: 7c0c 4400 8301 8301 724d 7401 640b 8301  |.D.....rMt.d...
+000031d0: 0100 7405 7c07 640c 8d01 8900 6e0c 7405  ..t.|.d.....n.t.
+000031e0: 7c01 7c02 7c03 7c04 7c08 7c05 7c06 7c09  |.|.|.|.|.|.|.|.
+000031f0: 640d 8d08 8900 7c00 6a03 6409 1900 a006  d.....|.j.d.....
+00003200: 640e 8700 8701 8702 6603 640f 6410 8408  d.......f.d.d...
+00003210: a102 6601 5300 2911 7a94 5374 616e 6461  ..f.S.).z.Standa
+00003220: 7264 2044 6174 6120 5374 6f72 653a 2053  rd Data Store: S
+00003230: 6561 7263 6820 6461 7461 2073 6574 7320  earch data sets 
+00003240: 6769 7665 6e20 7468 6520 6669 6c74 6572  given the filter
+00003250: 696e 6720 6372 6974 6572 6961 206f 7220  ing criteria or 
+00003260: 6f62 6a65 6374 2069 6465 6e74 6966 6965  object identifie
+00003270: 722e 0a20 2020 2052 6573 756c 7473 206f  r..    Results o
+00003280: 6620 7468 6973 2063 6f6d 6d61 6e64 2063  f this command c
+00003290: 616e 2062 6520 7573 6564 2069 6e20 606f  an be used in `o
+000032a0: 6269 7320 646f 776e 6c6f 6164 602e 6301  bis download`.c.
+000032b0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000032c0: 0000 0073 0000 00f3 1800 0000 8100 7c00  ...s..........|.
+000032d0: 5d07 7d01 7c01 6400 7500 5600 0100 7102  ].}.|.d.u.V...q.
+000032e0: 6400 5300 721a 0000 0072 1200 0000 a902  d.S.r....r......
+000032f0: da02 2e30 da01 7672 1200 0000 7212 0000  ...0..vr....r...
+00003300: 0072 1300 0000 da09 3c67 656e 6578 7072  .r......<genexpr
+00003310: 3e58 0100 00f3 0400 0000 0280 1600 7a22  >X............z"
+00003320: 6461 7461 5f73 6574 5f73 6561 7263 682e  data_set_search.
+00003330: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00003340: 723e fa31 596f 7520 6d75 7374 2070 726f  r>.1You must pro
+00003350: 7669 6465 2061 7420 6c65 6173 7420 6f6e  vide at least on
+00003360: 6520 6669 6c74 6572 696e 6720 6372 6974  e filtering crit
+00003370: 6572 6961 2172 3b00 0000 4efa 3650 726f  eria!r;...N.6Pro
+00003380: 7065 7274 7920 636f 6465 2061 6e64 2070  perty code and p
+00003390: 726f 7065 7274 7920 7661 6c75 6520 6e65  roperty value ne
+000033a0: 6564 2074 6f20 6265 2073 7065 6369 6669  ed to be specifi
+000033b0: 6564 2146 7299 0000 0072 3000 0000 6301  ed!Fr....r0...c.
+000033c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000033d0: 0000 0073 0000 00f3 1800 0000 8100 7c00  ...s..........|.
+000033e0: 5d07 7d01 7c01 6400 7501 5600 0100 7102  ].}.|.d.u.V...q.
+000033f0: 6400 5300 721a 0000 0072 1200 0000 72c3  d.S.r....r....r.
+00003400: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00003410: 0000 72c6 0000 0061 0100 0072 c700 0000  ..r....a...r....
+00003420: fa45 4f62 6a65 6374 2070 6172 616d 6574  .EObject paramet
+00003430: 6572 2064 6574 6563 7465 6421 204f 7468  er detected! Oth
+00003440: 6572 2066 696c 7465 7269 6e67 2061 7267  er filtering arg
+00003450: 756d 656e 7473 2077 696c 6c20 6265 206f  uments will be o
+00003460: 6d69 7474 6564 21a9 0172 b400 0000 a908  mitted!..r......
+00003470: 72b3 0000 00da 0573 7061 6365 da07 7072  r......space..pr
+00003480: 6f6a 6563 74da 0a65 7870 6572 696d 656e  oject..experimen
+00003490: 7472 b500 0000 72b7 0000 0072 b800 0000  tr....r....r....
+000034a0: 72b6 0000 00da 0f64 6174 615f 7365 745f  r......data_set_
+000034b0: 7365 6172 6368 6301 0000 0000 0000 0000  searchc.........
+000034c0: 0000 0001 0000 0005 0000 0013 0000 00f3  ................
+000034d0: 0e00 0000 7c00 a000 8800 8801 8802 a103  ....|...........
+000034e0: 5300 721a 0000 0029 01da 0f73 6561 7263  S.r....)...searc
+000034f0: 685f 6461 7461 5f73 6574 7232 0000 00a9  h_data_setr2....
+00003500: 03da 0766 696c 7465 7273 72b9 0000 00da  ...filtersr.....
+00003510: 0473 6176 6572 1200 0000 7213 0000 0072  .saver....r....r
+00003520: 3600 0000 6a01 0000 f302 0000 000e 007a  6...j..........z
+00003530: 2164 6174 615f 7365 745f 7365 6172 6368  !data_set_search
+00003540: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00003550: 613e a907 da03 616c 6c72 0800 0000 7209  a>....allr....r.
+00003560: 0000 0072 2a00 0000 da03 616e 79da 0464  ...r*.....any..d
+00003570: 6963 7472 3800 0000 a90d 722b 0000 0072  ictr8.....r+...r
+00003580: b300 0000 72ce 0000 0072 cf00 0000 72d0  ....r....r....r.
+00003590: 0000 0072 b700 0000 72b8 0000 0072 b400  ...r....r....r..
+000035a0: 0000 72b5 0000 0072 b600 0000 72d6 0000  ..r....r....r...
+000035b0: 0072 b900 0000 da13 6669 6c74 6572 696e  .r......filterin
+000035c0: 675f 6172 6775 6d65 6e74 7372 1200 0000  g_argumentsr....
+000035d0: 72d4 0000 0072 1300 0000 72d1 0000 004e  r....r....r....N
+000035e0: 0100 0073 3600 0000 0a07 0201 0401 04fe  ...s6...........
+000035f0: 1803 0801 0401 1001 0601 02ff 0601 02ff  ................
+00003600: 0802 0401 1401 0801 1201 0801 0c01 0602  ................
+00003610: 0601 0401 0201 06fd 0c04 0e01 06ff 72d1  ..............r.
+00003620: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00003630: 0300 0000 0400 0000 4300 0000 72a2 0000  ........C...r...
+00003640: 0029 087a 9e20 4578 7465 726e 616c 2044  .).z. External D
+00003650: 6174 6120 5374 6f72 653a 2047 6574 2f73  ata Store: Get/s
+00003660: 6574 2070 726f 7065 7274 6965 7320 7265  et properties re
+00003670: 6c61 7465 6420 746f 2074 6865 206f 626a  lated to the obj
+00003680: 6563 742e 0a0a 2020 2020 5374 616e 6461  ect...    Standa
+00003690: 7264 2044 6174 6120 5374 6f72 653a 2047  rd Data Store: G
+000036a0: 6574 2f73 6574 2070 726f 7065 7274 6965  et/set propertie
+000036b0: 7320 6f66 206f 626a 6563 7473 2063 6f6e  s of objects con
+000036c0: 6e65 6374 6564 2074 6f20 646f 776e 6c6f  nected to downlo
+000036d0: 6164 6564 2064 6174 6173 6574 732e 0a20  aded datasets.. 
+000036e0: 2020 2046 7299 0000 0072 8000 0000 7230     Fr....r....r0
+000036f0: 0000 00da 066f 626a 6563 7472 8100 0000  .....objectr....
+00003700: 4e72 a300 0000 72a4 0000 0072 1200 0000  Nr....r....r....
+00003710: 7212 0000 0072 1300 0000 72de 0000 0070  r....r....r....p
+00003720: 0100 00f3 0800 0000 0e08 0a01 0a01 0e01  ................
+00003730: 72de 0000 00da 0f6f 626a 6563 745f 7365  r......object_se
+00003740: 7474 696e 6773 6302 0000 0000 0000 0000  ttingsc.........
+00003750: 0000 0002 0000 0006 0000 0003 0000 0072  ...............r
+00003760: a700 0000 2905 7a98 2045 7874 6572 6e61  ....).z. Externa
+00003770: 6c20 4461 7461 2053 746f 7265 3a20 5365  l Data Store: Se
+00003780: 7420 7072 6f70 6572 7469 6573 2072 656c  t properties rel
+00003790: 6174 6564 2074 6f20 7468 6520 6f62 6a65  ated to the obje
+000037a0: 6374 2e0a 0a20 2020 2053 7461 6e64 6172  ct...    Standar
+000037b0: 6420 4461 7461 2053 746f 7265 3a20 5365  d Data Store: Se
+000037c0: 7420 7072 6f70 6572 7479 2074 6f20 616c  t property to al
+000037d0: 6c20 6f62 6a65 6374 7320 636f 6e6e 6563  l objects connec
+000037e0: 7465 6420 746f 2064 6f77 6e6c 6f61 6465  ted to downloade
+000037f0: 6420 6461 7461 7365 7473 2e0a 2020 2020  d datasets..    
+00003800: 7230 0000 00da 0a6f 626a 6563 745f 7365  r0.....object_se
+00003810: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00003820: 0000 0300 0000 1300 0000 72a9 0000 0072  ..........r....r
+00003830: 1a00 0000 72aa 0000 0072 3200 0000 a902  ....r....r2.....
+00003840: 722b 0000 0072 e000 0000 7212 0000 0072  r+...r....r....r
+00003850: 1300 0000 7236 0000 0086 0100 0072 3700  ....r6.......r7.
+00003860: 0000 7a1c 6f62 6a65 6374 5f73 6574 2e3c  ..z.object_set.<
+00003870: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00003880: 72ac 0000 0072 e200 0000 7212 0000 0072  r....r....r....r
+00003890: e200 0000 7213 0000 0072 e100 0000 7e01  ....r....r....~.
+000038a0: 0000 f302 0000 001c 0872 e100 0000 6302  .........r....c.
+000038b0: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+000038c0: 0000 0003 0000 0072 a700 0000 2905 7aa0  .......r....).z.
+000038d0: 2045 7874 6572 6e61 6c20 4461 7461 2053   External Data S
+000038e0: 746f 7265 3a20 5365 7420 7072 6f70 6572  tore: Set proper
+000038f0: 7469 6573 2072 656c 6174 6564 2074 6f20  ties related to 
+00003900: 7468 6520 6f62 6a65 6374 2e0a 0a20 2020  the object...   
+00003910: 2053 7461 6e64 6172 6420 4461 7461 2053   Standard Data S
+00003920: 746f 7265 3a20 4765 7420 6769 7665 6e20  tore: Get given 
+00003930: 7072 6f70 6572 7469 6573 206f 6620 616c  properties of al
+00003940: 6c20 6f62 6a65 6374 7320 636f 6e6e 6563  l objects connec
+00003950: 7465 6420 746f 2064 6f77 6e6c 6f61 6465  ted to downloade
+00003960: 6420 6461 7461 7365 7473 2e0a 2020 2020  d datasets..    
+00003970: 7230 0000 00da 0a6f 626a 6563 745f 6765  r0.....object_ge
+00003980: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00003990: 0000 0300 0000 1300 0000 72a9 0000 0072  ..........r....r
+000039a0: 1a00 0000 72af 0000 0072 3200 0000 72e2  ....r....r2...r.
+000039b0: 0000 0072 1200 0000 7213 0000 0072 3600  ...r....r....r6.
+000039c0: 0000 9101 0000 7237 0000 007a 1c6f 626a  ......r7...z.obj
+000039d0: 6563 745f 6765 742e 3c6c 6f63 616c 733e  ect_get.<locals>
+000039e0: 2e3c 6c61 6d62 6461 3e72 ac00 0000 72e2  .<lambda>r....r.
+000039f0: 0000 0072 1200 0000 72e2 0000 0072 1300  ...r....r....r..
+00003a00: 0000 72e4 0000 0089 0100 0072 e300 0000  ..r........r....
+00003a10: 72e4 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00003a20: 0000 0200 0000 0600 0000 0300 0000 72a7  ..............r.
+00003a30: 0000 0029 057a 3e20 4578 7465 726e 616c  ...).z> External
+00003a40: 2044 6174 6120 5374 6f72 653a 2043 6c65   Data Store: Cle
+00003a50: 6172 2070 726f 7065 7274 6965 7320 7265  ar properties re
+00003a60: 6c61 7465 6420 746f 2074 6865 206f 626a  lated to the obj
+00003a70: 6563 742e 2072 3000 0000 da0c 6f62 6a65  ect. r0.....obje
+00003a80: 6374 5f63 6c65 6172 6301 0000 0000 0000  ct_clearc.......
+00003a90: 0000 0000 0001 0000 0003 0000 0013 0000  ................
+00003aa0: 0072 a900 0000 721a 0000 0072 b200 0000  .r....r....r....
+00003ab0: 7232 0000 0072 e200 0000 7212 0000 0072  r2...r....r....r
+00003ac0: 1300 0000 7236 0000 0099 0100 0072 3700  ....r6.......r7.
+00003ad0: 0000 7a1e 6f62 6a65 6374 5f63 6c65 6172  ..z.object_clear
+00003ae0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00003af0: 613e 72ac 0000 0072 e200 0000 7212 0000  a>r....r....r...
+00003b00: 0072 e200 0000 7213 0000 0072 e500 0000  .r....r....r....
+00003b10: 9401 0000 72ad 0000 0072 e500 0000 7a2e  ....r....r....z.
+00003b20: 5365 6172 6368 2066 6f72 2073 616d 706c  Search for sampl
+00003b30: 6573 2075 7369 6e67 2061 2066 696c 7465  es using a filte
+00003b40: 7269 6e67 2063 7269 7465 7269 612e 630c  ring criteria.c.
+00003b50: 0000 0000 0000 0000 0000 000d 0000 000a  ................
+00003b60: 0000 0003 0000 0073 dc00 0000 7c01 7c02  .......s....|.|.
+00003b70: 7c03 7c04 7c05 7c06 7c08 7c09 6708 7d0c  |.|.|.|.|.|.g.}.
+00003b80: 7400 6401 6402 8400 7c0c 7c07 6701 1700  t.d.d...|.|.g...
+00003b90: 4400 8301 8301 721c 7401 6403 8301 0100  D.....r.t.d.....
+00003ba0: 6404 5300 7c08 6405 7500 7224 7c09 6405  d.S.|.d.u.r$|.d.
+00003bb0: 7501 732c 7c08 6405 7501 7232 7c09 6405  u.s,|.d.u.r2|.d.
+00003bc0: 7500 7232 7401 6406 8301 0100 6404 5300  u.r2t.d.....d.S.
+00003bd0: 7402 7c00 6a03 6407 6408 8d02 7c00 6a03  t.|.j.d.d...|.j.
+00003be0: 6409 3c00 7c07 6405 7501 7253 7404 640a  d.<.|.d.u.rSt.d.
+00003bf0: 6402 8400 7c0c 4400 8301 8301 724d 7401  d...|.D.....rMt.
+00003c00: 640b 8301 0100 7405 7c07 640c 8d01 8900  d.....t.|.d.....
+00003c10: 6e0c 7405 7c01 7c02 7c03 7c04 7c08 7c05  n.t.|.|.|.|.|.|.
+00003c20: 7c06 7c09 640d 8d08 8900 7c00 6a03 6409  |.|.d.....|.j.d.
+00003c30: 1900 a006 640e 8700 8701 8702 6603 640f  ....d.......f.d.
+00003c40: 6410 8408 a102 5300 2911 7a58 5374 616e  d.....S.).zXStan
+00003c50: 6461 7264 2044 6174 6120 5374 6f72 653a  dard Data Store:
+00003c60: 2053 6561 7263 6820 666f 7220 6f62 6a65   Search for obje
+00003c70: 6374 7320 7573 696e 6720 6120 6669 6c74  cts using a filt
+00003c80: 6572 696e 6720 6372 6974 6572 6961 206f  ering criteria o
+00003c90: 7220 6f62 6a65 6374 2069 6465 6e74 6966  r object identif
+00003ca0: 6965 722e 6301 0000 0000 0000 0000 0000  ier.c...........
+00003cb0: 0002 0000 0003 0000 0073 0000 0072 c200  .........s...r..
+00003cc0: 0000 721a 0000 0072 1200 0000 72c3 0000  ..r....r....r...
+00003cd0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00003ce0: 72c6 0000 00a4 0100 0072 c700 0000 7a20  r........r....z 
+00003cf0: 6f62 6a65 6374 5f73 6561 7263 682e 3c6c  object_search.<l
+00003d00: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
+00003d10: 72c8 0000 0072 3b00 0000 4e72 c900 0000  r....r;...Nr....
+00003d20: 4672 9900 0000 7230 0000 0063 0100 0000  Fr....r0...c....
+00003d30: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00003d40: 7300 0000 72ca 0000 0072 1a00 0000 7212  s...r....r....r.
+00003d50: 0000 0072 c300 0000 7212 0000 0072 1200  ...r....r....r..
+00003d60: 0000 7213 0000 0072 c600 0000 ad01 0000  ..r....r........
+00003d70: 72c7 0000 0072 cb00 0000 72cc 0000 0072  r....r....r....r
+00003d80: cd00 0000 da0d 6f62 6a65 6374 5f73 6561  ......object_sea
+00003d90: 7263 6863 0100 0000 0000 0000 0000 0000  rchc............
+00003da0: 0100 0000 0500 0000 1300 0000 72d2 0000  ............r...
+00003db0: 0072 1a00 0000 2901 da0d 7365 6172 6368  .r....)...search
+00003dc0: 5f6f 626a 6563 7472 3200 0000 72d4 0000  _objectr2...r...
+00003dd0: 0072 1200 0000 7213 0000 0072 3600 0000  .r....r....r6...
+00003de0: b601 0000 72d7 0000 007a 1f6f 626a 6563  ....r....z.objec
+00003df0: 745f 7365 6172 6368 2e3c 6c6f 6361 6c73  t_search.<locals
+00003e00: 3e2e 3c6c 616d 6264 613e 72d8 0000 0072  >.<lambda>r....r
+00003e10: dc00 0000 7212 0000 0072 d400 0000 7213  ....r....r....r.
+00003e20: 0000 0072 e600 0000 9c01 0000 7334 0000  ...r........s4..
+00003e30: 000a 0606 0104 ff18 0208 0104 0110 0106  ................
+00003e40: 0102 ff06 0102 ff08 0204 0114 0108 0112  ................
+00003e50: 0108 010c 0106 0206 0104 0102 0106 fd0c  ................
+00003e60: 040e 0104 ff72 e600 0000 6302 0000 0000  .....r....c.....
+00003e70: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00003e80: 0000 0072 a200 0000 2908 7aa8 2045 7874  ...r....).z. Ext
+00003e90: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00003ea0: 3a20 4765 742f 7365 7420 7365 7474 696e  : Get/set settin
+00003eb0: 6773 2072 656c 6174 6564 2074 6f20 7468  gs related to th
+00003ec0: 6520 636f 6c6c 6563 7469 6f6e 2e0a 0a20  e collection... 
+00003ed0: 2020 2053 7461 6e64 6172 6420 4461 7461     Standard Data
+00003ee0: 2053 746f 7265 3a20 4765 742f 7365 7420   Store: Get/set 
+00003ef0: 7072 6f70 6572 7469 6573 206f 6620 616c  properties of al
+00003f00: 6c20 636f 6c6c 6563 7469 6f6e 7320 636f  l collections co
+00003f10: 6e6e 6563 7465 6420 746f 2064 6f77 6e6c  nnected to downl
+00003f20: 6f61 6465 6420 6461 7461 7365 7473 2e0a  oaded datasets..
+00003f30: 2020 2020 4672 9900 0000 7280 0000 0072      Fr....r....r
+00003f40: 3000 0000 da0a 636f 6c6c 6563 7469 6f6e  0.....collection
+00003f50: 7281 0000 004e 72a3 0000 0072 a400 0000  r....Nr....r....
+00003f60: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00003f70: e800 0000 bc01 0000 72df 0000 0072 e800  ........r....r..
+00003f80: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00003f90: 0000 0006 0000 0003 0000 0072 a700 0000  ...........r....
+00003fa0: 2905 7aa6 2045 7874 6572 6e61 6c20 4461  ).z. External Da
+00003fb0: 7461 2053 746f 7265 3a20 5365 7420 7365  ta Store: Set se
+00003fc0: 7474 696e 6773 2072 656c 6174 6564 2074  ttings related t
+00003fd0: 6f20 7468 6520 636f 6c6c 6563 7469 6f6e  o the collection
+00003fe0: 2e0a 0a20 2020 2053 7461 6e64 6172 6420  ...    Standard 
+00003ff0: 4461 7461 2053 746f 7265 3a20 5365 7420  Data Store: Set 
+00004000: 6769 7665 6e20 7072 6f70 6572 7469 6573  given properties
+00004010: 206f 6620 616c 6c20 636f 6c6c 6563 7469   of all collecti
+00004020: 6f6e 7320 636f 6e6e 6563 7465 6420 746f  ons connected to
+00004030: 2064 6f77 6e6c 6f61 6465 6420 6461 7461   downloaded data
+00004040: 7365 7473 2e0a 2020 2020 7230 0000 00da  sets..    r0....
+00004050: 0e63 6f6c 6c65 6374 696f 6e5f 7365 7463  .collection_setc
+00004060: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00004070: 0300 0000 1300 0000 72a9 0000 0072 1a00  ........r....r..
+00004080: 0000 72aa 0000 0072 3200 0000 72ab 0000  ..r....r2...r...
+00004090: 0072 1200 0000 7213 0000 0072 3600 0000  .r....r....r6...
+000040a0: d201 0000 7237 0000 007a 2063 6f6c 6c65  ....r7...z colle
+000040b0: 6374 696f 6e5f 7365 742e 3c6c 6f63 616c  ction_set.<local
+000040c0: 733e 2e3c 6c61 6d62 6461 3e72 ac00 0000  s>.<lambda>r....
+000040d0: 72ab 0000 0072 1200 0000 72ab 0000 0072  r....r....r....r
+000040e0: 1300 0000 72e9 0000 00ca 0100 0072 e300  ....r........r..
+000040f0: 0000 72e9 0000 0063 0200 0000 0000 0000  ..r....c........
+00004100: 0000 0000 0200 0000 0600 0000 0300 0000  ................
+00004110: 72a7 0000 0029 057a a620 4578 7465 726e  r....).z. Extern
+00004120: 616c 2044 6174 6120 5374 6f72 653a 2047  al Data Store: G
+00004130: 6574 2073 6574 7469 6e67 7320 7265 6c61  et settings rela
+00004140: 7465 6420 746f 2074 6865 2063 6f6c 6c65  ted to the colle
+00004150: 6374 696f 6e2e 0a0a 2020 2020 5374 616e  ction...    Stan
+00004160: 6461 7264 2044 6174 6120 5374 6f72 653a  dard Data Store:
+00004170: 2047 6574 2067 6976 656e 2070 726f 7065   Get given prope
+00004180: 7274 6965 7320 6f66 2061 6c6c 2063 6f6c  rties of all col
+00004190: 6c65 6374 696f 6e73 2063 6f6e 6e65 6374  lections connect
+000041a0: 6564 2074 6f20 646f 776e 6c6f 6164 6564  ed to downloaded
+000041b0: 2064 6174 6173 6574 732e 0a20 2020 2072   datasets..    r
+000041c0: 3000 0000 da0e 636f 6c6c 6563 7469 6f6e  0.....collection
+000041d0: 5f67 6574 6301 0000 0000 0000 0000 0000  _getc...........
+000041e0: 0001 0000 0003 0000 0013 0000 0072 a900  .............r..
+000041f0: 0000 721a 0000 0072 af00 0000 7232 0000  ..r....r....r2..
+00004200: 0072 ab00 0000 7212 0000 0072 1300 0000  .r....r....r....
+00004210: 7236 0000 00dd 0100 0072 3700 0000 7a20  r6.......r7...z 
+00004220: 636f 6c6c 6563 7469 6f6e 5f67 6574 2e3c  collection_get.<
+00004230: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00004240: 72ac 0000 0072 ab00 0000 7212 0000 0072  r....r....r....r
+00004250: ab00 0000 7213 0000 0072 ea00 0000 d501  ....r....r......
+00004260: 0000 72e3 0000 0072 ea00 0000 6302 0000  ..r....r....c...
+00004270: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+00004280: 0003 0000 0072 a700 0000 2905 7a3e 4578  .....r....).z>Ex
+00004290: 7465 726e 616c 2044 6174 6120 5374 6f72  ternal Data Stor
+000042a0: 653a 2043 6c65 6172 2073 6574 7469 6e67  e: Clear setting
+000042b0: 7320 7265 6c61 7465 6420 746f 2074 6865  s related to the
+000042c0: 2063 6f6c 6c65 6374 696f 6e2e 7230 0000   collection.r0..
+000042d0: 00da 1063 6f6c 6c65 6374 696f 6e5f 636c  ...collection_cl
+000042e0: 6561 7263 0100 0000 0000 0000 0000 0000  earc............
+000042f0: 0100 0000 0300 0000 1300 0000 72a9 0000  ............r...
+00004300: 0072 1a00 0000 72b2 0000 0072 3200 0000  .r....r....r2...
+00004310: 72ab 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00004320: 3600 0000 e501 0000 7237 0000 007a 2263  6.......r7...z"c
+00004330: 6f6c 6c65 6374 696f 6e5f 636c 6561 722e  ollection_clear.
+00004340: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00004350: 3e72 ac00 0000 72ab 0000 0072 1200 0000  >r....r....r....
+00004360: 72ab 0000 0072 1300 0000 72eb 0000 00e0  r....r....r.....
+00004370: 0100 0072 ad00 0000 72eb 0000 0063 0200  ...r....r....c..
+00004380: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00004390: 0000 4300 0000 734a 0000 007c 0164 0175  ..C...sJ...|.d.u
+000043a0: 0072 0d74 007c 006a 0164 0264 0164 038d  .r.t.|.j.d.d.d..
+000043b0: 037d 026e 0774 007c 006a 0164 0264 048d  .}.n.t.|.j.d.d..
+000043c0: 027d 027c 017c 006a 0164 053c 007c 027c  .}.|.|.j.d.<.|.|
+000043d0: 006a 0164 063c 0064 077c 006a 0164 083c  .j.d.<.d.|.j.d.<
+000043e0: 0064 0953 0029 0a7a 6345 7874 6572 6e61  .d.S.).zcExterna
+000043f0: 6c20 4461 7461 2053 746f 7265 3a20 4765  l Data Store: Ge
+00004400: 742f 7365 7420 636f 6e66 6967 7572 6174  t/set configurat
+00004410: 696f 6e73 2e0a 0a20 2020 2053 7461 6e64  ions...    Stand
+00004420: 6172 6420 4461 7461 2053 746f 7265 3a20  ard Data Store: 
+00004430: 4765 742f 7365 7420 636f 6e66 6967 7572  Get/set configur
+00004440: 6174 696f 6e73 2e0a 2020 2020 5446 a902  ations..    TF..
+00004450: 729a 0000 00da 0b69 735f 7068 7973 6963  r......is_physic
+00004460: 616c 7299 0000 0072 8000 0000 7230 0000  alr....r....r0..
+00004470: 0072 8500 0000 7281 0000 004e 72a3 0000  .r....r....Nr...
+00004480: 0072 a400 0000 7212 0000 0072 1200 0000  .r....r....r....
+00004490: 7213 0000 0072 8500 0000 eb01 0000 730c  r....r........s.
+000044a0: 0000 0008 0812 010e 020a 010a 010e 0172  ...............r
+000044b0: 8500 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000044c0: 0002 0000 0006 0000 0003 0000 0072 a700  .............r..
+000044d0: 0000 2905 7a5b 4578 7465 726e 616c 2044  ..).z[External D
+000044e0: 6174 6120 5374 6f72 653a 2053 6574 2063  ata Store: Set c
+000044f0: 6f6e 6669 6775 7261 7469 6f6e 732e 0a0a  onfigurations...
+00004500: 2020 2020 5374 616e 6461 7264 2044 6174      Standard Dat
+00004510: 6120 5374 6f72 653a 2053 6574 2063 6f6e  a Store: Set con
+00004520: 6669 6775 7261 7469 6f6e 732e 0a20 2020  figurations..   
+00004530: 2072 3000 0000 da0a 636f 6e66 6967 5f73   r0.....config_s
+00004540: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
+00004550: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
+00004560: 721a 0000 0072 aa00 0000 7232 0000 0072  r....r....r2...r
+00004570: ab00 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
+00004580: 0000 0004 0200 0072 3700 0000 7a1c 636f  .......r7...z.co
+00004590: 6e66 6967 5f73 6574 2e3c 6c6f 6361 6c73  nfig_set.<locals
+000045a0: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
+000045b0: ab00 0000 7212 0000 0072 ab00 0000 7213  ....r....r....r.
+000045c0: 0000 0072 ee00 0000 fc01 0000 72e3 0000  ...r........r...
+000045d0: 0072 ee00 0000 6302 0000 0000 0000 0000  .r....c.........
+000045e0: 0000 0002 0000 0006 0000 0003 0000 0072  ...............r
+000045f0: a700 0000 2905 7a5b 4578 7465 726e 616c  ....).z[External
+00004600: 2044 6174 6120 5374 6f72 653a 2047 6574   Data Store: Get
+00004610: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
+00004620: 0a0a 2020 2020 5374 616e 6461 7264 2044  ..    Standard D
+00004630: 6174 6120 5374 6f72 653a 2047 6574 2063  ata Store: Get c
+00004640: 6f6e 6669 6775 7261 7469 6f6e 732e 0a20  onfigurations.. 
+00004650: 2020 2072 3000 0000 da0a 636f 6e66 6967     r0.....config
+00004660: 5f67 6574 6301 0000 0000 0000 0000 0000  _getc...........
+00004670: 0001 0000 0003 0000 0013 0000 0072 a900  .............r..
+00004680: 0000 721a 0000 0072 af00 0000 7232 0000  ..r....r....r2..
+00004690: 0072 ab00 0000 7212 0000 0072 1300 0000  .r....r....r....
+000046a0: 7236 0000 000f 0200 0072 3700 0000 7a1c  r6.......r7...z.
+000046b0: 636f 6e66 6967 5f67 6574 2e3c 6c6f 6361  config_get.<loca
+000046c0: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
+000046d0: 0072 ab00 0000 7212 0000 0072 ab00 0000  .r....r....r....
+000046e0: 7213 0000 0072 ef00 0000 0702 0000 72e3  r....r........r.
+000046f0: 0000 0072 ef00 0000 6302 0000 0000 0000  ...r....c.......
+00004700: 0000 0000 0002 0000 0006 0000 0003 0000  ................
+00004710: 0072 a700 0000 2905 7a2f 4578 7465 726e  .r....).z/Extern
+00004720: 616c 2044 6174 6120 5374 6f72 653a 2043  al Data Store: C
+00004730: 6c65 6172 2063 6f6e 6669 6775 7261 7469  lear configurati
+00004740: 6f6e 732e 0a20 2020 2072 3000 0000 da0c  ons..    r0.....
+00004750: 636f 6e66 6967 5f63 6c65 6172 6301 0000  config_clearc...
+00004760: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00004770: 0013 0000 0072 a900 0000 721a 0000 0072  .....r....r....r
+00004780: b200 0000 7232 0000 0072 ab00 0000 7212  ....r2...r....r.
+00004790: 0000 0072 1300 0000 7236 0000 0018 0200  ...r....r6......
+000047a0: 0072 3700 0000 7a1e 636f 6e66 6967 5f63  .r7...z.config_c
+000047b0: 6c65 6172 2e3c 6c6f 6361 6c73 3e2e 3c6c  lear.<locals>.<l
+000047c0: 616d 6264 613e 72ac 0000 0072 ab00 0000  ambda>r....r....
+000047d0: 7212 0000 0072 ab00 0000 7213 0000 0072  r....r....r....r
+000047e0: f000 0000 1202 0000 7302 0000 001c 0672  ........s......r
+000047f0: f000 0000 7a02 2d6d 7a05 2d2d 6d73 677a  ....z.-mz.--msgz
+00004800: 0b6f 6269 7320 636f 6d6d 6974 7a23 4120  .obis commitz#A 
+00004810: 6d65 7373 6167 6520 6578 706c 6169 6e69  message explaini
+00004820: 6e67 2077 6861 7420 7761 7320 646f 6e65  ng what was done
+00004830: 2e7a 022d 617a 0a2d 2d61 7574 6f5f 6164  .z.-az.--auto_ad
+00004840: 647a 2641 7574 6f6d 6174 6963 616c 6c79  dz&Automatically
+00004850: 2061 6464 2061 6c6c 2075 6e74 7261 636b   add all untrack
+00004860: 6564 2066 696c 6573 2e7a 022d 697a 172d  ed files.z.-iz.-
+00004870: 2d69 676e 6f72 655f 6d69 7373 696e 675f  -ignore_missing_
+00004880: 7061 7265 6e74 7a29 4966 2070 6172 656e  parentz)If paren
+00004890: 7420 6461 7461 2073 6574 2069 7320 6d69  t data set is mi
+000048a0: 7373 696e 672c 2069 676e 6f72 6520 6974  ssing, ignore it
+000048b0: 2e29 02da 0665 7869 7374 73da 0966 696c  .)...exists..fil
+000048c0: 655f 6f6b 6179 2902 720d 0000 00da 0872  e_okay).r......r
+000048d0: 6571 7569 7265 64da 0663 6f6d 6d69 747a  equired..commitz
+000048e0: 3043 6f6d 6d69 7420 7468 6520 7265 706f  0Commit the repo
+000048f0: 7369 746f 7279 2074 6f20 6769 7420 616e  sitory to git an
+00004900: 6420 696e 666f 726d 206f 7065 6e42 4953  d inform openBIS
+00004910: 2e63 0500 0000 0000 0000 0000 0000 0500  .c..............
+00004920: 0000 0600 0000 0300 0000 7320 0000 007c  ..........s ...|
+00004930: 006a 0064 0119 00a0 0164 0287 0087 0187  .j.d.....d......
+00004940: 0266 0364 0364 0484 087c 04a1 0353 0029  .f.d.d...|...S.)
+00004950: 05fa 4a45 7874 6572 6e61 6c20 4461 7461  ..JExternal Data
+00004960: 2053 746f 7265 3a20 436f 6d6d 6974 2074   Store: Commit t
+00004970: 6865 2072 6570 6f73 6974 6f72 7920 746f  he repository to
+00004980: 2067 6974 2061 6e64 2069 6e66 6f72 6d20   git and inform 
+00004990: 6f70 656e 4249 532e 0a20 2020 2072 3000  openBIS..    r0.
+000049a0: 0000 72f4 0000 0063 0100 0000 0000 0000  ..r....c........
+000049b0: 0000 0000 0100 0000 0500 0000 1300 0000  ................
+000049c0: f30e 0000 007c 00a0 0088 0288 0088 01a1  .....|..........
+000049d0: 0353 0072 1a00 0000 2901 72f4 0000 0072  .S.r....).r....r
+000049e0: 3200 0000 a903 da08 6175 746f 5f61 6464  2.......auto_add
+000049f0: da15 6967 6e6f 7265 5f6d 6973 7369 6e67  ..ignore_missing
+00004a00: 5f70 6172 656e 74da 036d 7367 7212 0000  _parent..msgr...
+00004a10: 0072 1300 0000 7236 0000 0032 0200 0072  .r....r6...2...r
+00004a20: d700 0000 7a23 7265 706f 7369 746f 7279  ....z#repository
+00004a30: 5f63 6f6d 6d69 742e 3c6c 6f63 616c 733e  _commit.<locals>
+00004a40: 2e3c 6c61 6d62 6461 3e72 ac00 0000 a905  .<lambda>r......
+00004a50: 722b 0000 0072 fa00 0000 72f8 0000 0072  r+...r....r....r
+00004a60: f900 0000 7239 0000 0072 1200 0000 72f7  ....r9...r....r.
+00004a70: 0000 0072 1300 0000 da11 7265 706f 7369  ...r......reposi
+00004a80: 746f 7279 5f63 6f6d 6d69 742b 0200 0073  tory_commit+...s
+00004a90: 0800 0000 0c06 0e01 0201 04fe 72fc 0000  ............r...
+00004aa0: 0063 0500 0000 0000 0000 0000 0000 0500  .c..............
+00004ab0: 0000 0700 0000 4300 0000 732c 0000 0074  ......C...s,...t
+00004ac0: 007c 006a 0164 0164 028d 027c 006a 0164  .|.j.d.d...|.j.d
+00004ad0: 033c 007c 006a 0274 037c 017c 027c 037c  .<.|.j.t.|.|.|.|
+00004ae0: 0464 048d 0501 0064 0553 0029 0672 f500  .d.....d.S.).r..
+00004af0: 0000 4672 9900 0000 7230 0000 0029 0472  ..Fr....r0...).r
+00004b00: fa00 0000 72f8 0000 0072 f900 0000 7239  ....r....r....r9
+00004b10: 0000 004e 2904 7209 0000 0072 2a00 0000  ...N).r....r*...
+00004b20: da06 696e 766f 6b65 72fc 0000 0072 fb00  ..invoker....r..
+00004b30: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00004b40: 0072 f400 0000 3602 0000 7308 0000 0014  .r....6...s.....
+00004b50: 060a 0104 010a ffda 0f72 6570 6f73 6974  .........reposit
+00004b60: 6f72 795f 7061 7468 723e 0000 0072 2f00  ory_pathr>...r/.
+00004b70: 0000 2901 7223 0000 00da 0469 6e69 747a  ..).r#.....initz
+00004b80: 2b49 6e69 7469 616c 697a 6520 7468 6520  +Initialize the 
+00004b90: 666f 6c64 6572 2061 7320 6120 6461 7461  folder as a data
+00004ba0: 2072 6570 6f73 6974 6f72 792e 6303 0000   repository.c...
+00004bb0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00004bc0: 0043 0000 0073 0c00 0000 7400 7c00 7c01  .C...s....t.|.|.
+00004bd0: 7c02 8303 5300 2901 7a45 4578 7465 726e  |...S.).zEExtern
+00004be0: 616c 2044 6174 6120 5374 6f72 653a 2049  al Data Store: I
+00004bf0: 6e69 7469 616c 697a 6520 7468 6520 666f  nitialize the fo
+00004c00: 6c64 6572 2061 7320 6120 6461 7461 2072  lder as a data r
+00004c10: 6570 6f73 6974 6f72 792e 0a20 2020 2029  epository..    )
+00004c20: 0172 3a00 0000 2903 722b 0000 0072 fe00  .r:...).r+...r..
+00004c30: 0000 723e 0000 0072 1200 0000 7212 0000  ..r>...r....r...
+00004c40: 0072 1300 0000 da0f 7265 706f 7369 746f  .r......reposito
+00004c50: 7279 5f69 6e69 744c 0200 0073 0200 0000  ry_initL...s....
+00004c60: 0c06 7200 0100 007a 0a2d 2d70 6879 7369  ..r....z.--physi
+00004c70: 6361 6c72 ed00 0000 7a38 496e 6974 6961  calr....z8Initia
+00004c80: 6c69 7a65 2066 6f6c 6465 7220 666f 7220  lize folder for 
+00004c90: 5374 616e 6461 7264 2044 6174 6120 5374  Standard Data St
+00004ca0: 6f72 6520 6461 7461 2068 616e 646c 696e  ore data handlin
+00004cb0: 672e 6304 0000 0000 0000 0000 0000 0004  g.c.............
+00004cc0: 0000 0005 0000 0043 0000 0073 2a00 0000  .......C...s*...
+00004cd0: 7400 7c00 6a01 6401 7c03 6402 8d03 7c00  t.|.j.d.|.d...|.
+00004ce0: 6a01 6403 3c00 7c00 6a02 7403 7c01 7c02  j.d.<.|.j.t.|.|.
+00004cf0: 6404 8d03 0100 6405 5300 2906 7adf 4578  d.....d.S.).z.Ex
+00004d00: 7465 726e 616c 2044 6174 6120 5374 6f72  ternal Data Stor
+00004d10: 653a 2049 6e69 7469 616c 697a 6520 7468  e: Initialize th
+00004d20: 6520 666f 6c64 6572 2061 7320 6120 6461  e folder as a da
+00004d30: 7461 2072 6570 6f73 6974 6f72 7920 666f  ta repository fo
+00004d40: 7220 4578 7465 726e 616c 2044 6174 6120  r External Data 
+00004d50: 5374 6f72 650a 2020 2020 6461 7461 2068  Store.    data h
+00004d60: 616e 646c 696e 672e 0a0a 2020 2020 5374  andling...    St
+00004d70: 616e 6461 7264 2044 6174 6120 5374 6f72  andard Data Stor
+00004d80: 653a 2049 6e69 7469 616c 697a 6520 7468  e: Initialize th
+00004d90: 6520 666f 6c64 6572 2061 7320 6120 6461  e folder as a da
+00004da0: 7461 2072 6570 6f73 6974 6f72 7920 666f  ta repository fo
+00004db0: 7220 5374 616e 6461 7264 2044 6174 6120  r Standard Data 
+00004dc0: 5374 6f72 650a 2020 2020 6461 7461 2068  Store.    data h
+00004dd0: 616e 646c 696e 672e 0a20 2020 2046 72ec  andling..    Fr.
+00004de0: 0000 0072 3000 0000 2902 72fe 0000 0072  ...r0...).r....r
+00004df0: 3e00 0000 4e29 0472 0900 0000 722a 0000  >...N).r....r*..
+00004e00: 0072 fd00 0000 7200 0100 0029 0472 2b00  .r....r....).r+.
+00004e10: 0000 72fe 0000 0072 3e00 0000 72ed 0000  ..r....r>...r...
+00004e20: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00004e30: 72ff 0000 005b 0200 0073 0400 0000 160a  r....[...s......
+00004e40: 1401 7a08 2d2d 7061 7265 6e74 2901 720d  ..z.--parent).r.
+00004e50: 0000 0072 3c00 0000 7a2c 496e 6974 6961  ...r<...z,Initia
+00004e60: 6c69 7a65 2074 6865 2066 6f6c 6465 7220  lize the folder 
+00004e70: 6173 2061 6e20 616e 616c 7973 6973 2066  as an analysis f
+00004e80: 6f6c 6465 722e 6304 0000 0000 0000 0000  older.c.........
+00004e90: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+00004ea0: 0e00 0000 7400 7c00 7c01 7c02 7c03 8304  ....t.|.|.|.|...
+00004eb0: 5300 2901 fa41 4578 7465 726e 616c 2044  S.)..AExternal D
+00004ec0: 6174 6120 5374 6f72 653a 2049 6e69 7469  ata Store: Initi
+00004ed0: 616c 697a 6520 7468 6520 666f 6c64 6572  alize the folder
+00004ee0: 2061 7320 616e 2061 6e61 6c79 7369 7320   as an analysis 
+00004ef0: 666f 6c64 6572 2e29 0172 4900 0000 a904  folder.).rI.....
+00004f00: 722b 0000 0072 3f00 0000 72fe 0000 0072  r+...r?...r....r
+00004f10: 3e00 0000 7212 0000 0072 1200 0000 7213  >...r....r....r.
+00004f20: 0000 00da 1872 6570 6f73 6974 6f72 795f  .....repository_
+00004f30: 696e 6974 5f61 6e61 6c79 7369 7373 0200  init_analysiss..
+00004f40: 0072 9700 0000 7203 0100 0029 0272 6300  .r....r....).rc.
+00004f50: 0000 72c1 0000 0063 0400 0000 0000 0000  ..r....c........
+00004f60: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
+00004f70: 732a 0000 0074 007c 006a 0164 0164 028d  s*...t.|.j.d.d..
+00004f80: 027c 006a 0164 033c 007c 006a 0274 037c  .|.j.d.<.|.j.t.|
+00004f90: 017c 027c 0364 048d 0401 0064 0553 0029  .|.|.d.....d.S.)
+00004fa0: 0672 0101 0000 4672 9900 0000 7230 0000  .r....Fr....r0..
+00004fb0: 0029 0372 3f00 0000 72fe 0000 0072 3e00  .).r?...r....r>.
+00004fc0: 0000 4e29 0472 0900 0000 722a 0000 0072  ..N).r....r*...r
+00004fd0: fd00 0000 7203 0100 0072 0201 0000 7212  ....r....r....r.
+00004fe0: 0000 0072 1200 0000 7213 0000 0072 3c00  ...r....r....r<.
+00004ff0: 0000 7b02 0000 7308 0000 0014 0508 0104  ..{...s.........
+00005000: 010a ffda 0673 7461 7475 737a 2653 686f  .....statusz&Sho
+00005010: 7720 7468 6520 7374 6174 6520 6f66 2074  w the state of t
+00005020: 6865 206f 6269 7320 7265 706f 7369 746f  he obis reposito
+00005030: 7279 2e63 0200 0000 0000 0000 0000 0000  ry.c............
+00005040: 0200 0000 0500 0000 4300 0000 f318 0000  ........C.......
+00005050: 007c 006a 0064 0119 00a0 0164 0264 0364  .|.j.d.....d.d.d
+00005060: 0484 007c 01a1 0353 0029 05fa 3b45 7874  ...|...S.)..;Ext
+00005070: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00005080: 3a20 5368 6f77 2074 6865 2073 7461 7465  : Show the state
+00005090: 206f 6620 7468 6520 6f62 6973 2072 6570   of the obis rep
+000050a0: 6f73 6974 6f72 792e 7230 0000 00da 1172  ository.r0.....r
+000050b0: 6570 6f73 6974 6f72 795f 7374 6174 7573  epository_status
+000050c0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000050d0: 0002 0000 0053 0000 00f3 0800 0000 7c00  .....S........|.
+000050e0: a000 a100 5300 721a 0000 0029 0172 0401  ....S.r....).r..
+000050f0: 0000 7232 0000 0072 1200 0000 7212 0000  ..r2...r....r...
+00005100: 0072 1300 0000 7236 0000 0093 0200 00f3  .r....r6........
+00005110: 0200 0000 0800 7a23 7265 706f 7369 746f  ......z#reposito
+00005120: 7279 5f73 7461 7475 732e 3c6c 6f63 616c  ry_status.<local
+00005130: 733e 2e3c 6c61 6d62 6461 3e72 ac00 0000  s>.<lambda>r....
+00005140: a902 722b 0000 0072 3900 0000 7212 0000  ..r+...r9...r...
+00005150: 0072 1200 0000 7213 0000 0072 0701 0000  .r....r....r....
+00005160: 8e02 0000 f302 0000 0018 0572 0701 0000  ...........r....
+00005170: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00005180: 0004 0000 0043 0000 00f3 2600 0000 7400  .....C....&...t.
+00005190: 7c00 6a01 6401 6402 8d02 7c00 6a01 6403  |.j.d.d...|.j.d.
+000051a0: 3c00 7c00 6a02 7403 7c01 6404 8d02 0100  <.|.j.t.|.d.....
+000051b0: 6405 5300 2906 7206 0100 0046 7299 0000  d.S.).r....Fr...
+000051c0: 0072 3000 0000 a901 7239 0000 004e 2904  .r0.....r9...N).
+000051d0: 7209 0000 0072 2a00 0000 72fd 0000 0072  r....r*...r....r
+000051e0: 0701 0000 720a 0100 0072 1200 0000 7212  ....r....r....r.
+000051f0: 0000 0072 1300 0000 7204 0100 0096 0200  ...r....r.......
+00005200: 00f3 0400 0000 1405 1201 6302 0000 0000  ..........c.....
+00005210: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
+00005220: 0000 0073 0e00 0000 7c01 7c00 5f00 7c00  ...s....|.|._.|.
+00005230: a001 a100 5300 721a 0000 0029 0272 f900  ....S.r....).r..
+00005240: 0000 da04 7379 6e63 2902 7233 0000 0072  ....sync).r3...r
+00005250: f900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00005260: 0000 00da 105f 7265 706f 7369 746f 7279  ....._repository
+00005270: 5f73 796e 63aa 0200 0073 0400 0000 0601  _sync....s......
+00005280: 0801 7210 0100 0072 0f01 0000 7a21 5379  ..r....r....z!Sy
+00005290: 6e63 2074 6865 2072 6570 6f73 6974 6f72  nc the repositor
+000052a0: 7920 7769 7468 206f 7065 6e42 4953 2e63  y with openBIS.c
+000052b0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+000052c0: 0600 0000 0300 0000 731c 0000 007c 006a  ........s....|.j
+000052d0: 0064 0119 00a0 0164 0287 0066 0164 0364  .d.....d...f.d.d
+000052e0: 0484 087c 02a1 0353 0029 05fa 3645 7874  ...|...S.)..6Ext
+000052f0: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00005300: 3a20 5379 6e63 2074 6865 2072 6570 6f73  : Sync the repos
+00005310: 6974 6f72 7920 7769 7468 206f 7065 6e42  itory with openB
+00005320: 4953 2e72 3000 0000 720f 0100 0063 0100  IS.r0...r....c..
+00005330: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00005340: 0000 1300 0000 730a 0000 0074 007c 0088  ......s....t.|..
+00005350: 0083 0253 0072 1a00 0000 2901 7210 0100  ...S.r....).r...
+00005360: 0072 3200 0000 a901 72f9 0000 0072 1200  .r2.....r....r..
+00005370: 0000 7213 0000 0072 3600 0000 b402 0000  ..r....r6.......
+00005380: 7237 0000 007a 2172 6570 6f73 6974 6f72  r7...z!repositor
+00005390: 795f 7379 6e63 2e3c 6c6f 6361 6c73 3e2e  y_sync.<locals>.
+000053a0: 3c6c 616d 6264 613e 72ac 0000 00a9 0372  <lambda>r......r
+000053b0: 2b00 0000 72f9 0000 0072 3900 0000 7212  +...r....r9...r.
+000053c0: 0000 0072 1201 0000 7213 0000 00da 0f72  ...r....r......r
+000053d0: 6570 6f73 6974 6f72 795f 7379 6e63 af02  epository_sync..
+000053e0: 0000 7306 0000 0016 0502 0104 ff72 1401  ..s..........r..
+000053f0: 0000 6303 0000 0000 0000 0000 0000 0003  ..c.............
+00005400: 0000 0005 0000 0043 0000 00f3 2800 0000  .......C....(...
+00005410: 7400 7c00 6a01 6401 6402 8d02 7c00 6a01  t.|.j.d.d...|.j.
+00005420: 6403 3c00 7c00 6a02 7403 7c01 7c02 6404  d.<.|.j.t.|.|.d.
+00005430: 8d03 0100 6405 5300 2906 7211 0100 0046  ....d.S.).r....F
+00005440: 7299 0000 0072 3000 0000 2902 72f9 0000  r....r0...).r...
+00005450: 0072 3900 0000 4e29 0472 0900 0000 722a  .r9...N).r....r*
+00005460: 0000 0072 fd00 0000 7214 0100 0072 1301  ...r....r....r..
+00005470: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00005480: 0072 0f01 0000 b802 0000 7308 0000 0014  .r........s.....
+00005490: 0506 0104 010a ff7a 1b63 7265 6174 652f  .......z.create/
+000054a0: 7368 6f77 2061 206f 7065 6e42 4953 2074  show a openBIS t
+000054b0: 6f6b 656e 6301 0000 0000 0000 0000 0000  okenc...........
+000054c0: 0001 0000 0001 0000 0043 0000 0073 0400  .........C...s..
+000054d0: 0000 6400 5300 721a 0000 0072 1200 0000  ..d.S.r....r....
+000054e0: 2901 722b 0000 0072 1200 0000 7212 0000  ).r+...r....r...
+000054f0: 0072 1300 0000 da05 746f 6b65 6ec2 0200  .r......token...
+00005500: 0073 0200 0000 0403 7216 0100 007a 3647  .s......r....z6G
+00005510: 6574 2065 7869 7374 696e 6720 7065 7273  et existing pers
+00005520: 6f6e 616c 2061 6363 6573 7320 746f 6b65  onal access toke
+00005530: 6e20 6f72 2063 7265 6174 6520 6120 6e65  n or create a ne
+00005540: 7720 6f6e 657a 0c73 6573 7369 6f6e 2d6e  w onez.session-n
+00005550: 616d 6529 0172 f300 0000 7a0f 2d2d 7661  ame).r....z.--va
+00005560: 6c69 6469 7479 2d64 6179 737a 214e 756d  lidity-daysz!Num
+00005570: 6265 7220 6f66 2064 6179 7320 7468 6520  ber of days the 
+00005580: 746f 6b65 6e20 6973 2076 616c 6964 2901  token is valid).
+00005590: 7225 0000 007a 102d 2d76 616c 6964 6974  r%...z.--validit
+000055a0: 792d 7765 656b 737a 224e 756d 6265 7220  y-weeksz"Number 
+000055b0: 6f66 2077 6565 6b73 2074 6865 2074 6f6b  of weeks the tok
+000055c0: 656e 2069 7320 7661 6c69 647a 112d 2d76  en is validz.--v
+000055d0: 616c 6964 6974 792d 6d6f 6e74 6873 7a23  alidity-monthsz#
+000055e0: 4e75 6d62 6572 206f 6620 6d6f 6e74 6873  Number of months
+000055f0: 2074 6865 2074 6f6b 656e 2069 7320 7661   the token is va
+00005600: 6c69 6463 0200 0000 0000 0000 0000 0000  lidc............
+00005610: 0e00 0000 0a00 0000 0b00 0000 73e8 0100  ............s...
+00005620: 0074 0088 006a 0164 0164 028d 027d 037c  .t...j.d.d...}.|
+00005630: 03a0 02a1 0089 017c 0173 1388 0164 0319  .......|.s...d..
+00005640: 0064 0419 007d 017c 0172 1f74 03a0 0464  .d...}.|.r.t...d
+00005650: 057c 019b 0064 069d 03a1 0101 006e 0574  .|...d.......n.t
+00005660: 03a0 0564 07a1 017d 0188 0164 0319 0064  ...d...}...d...d
+00005670: 0819 007d 047c 0473 3174 03a0 0564 09a1  ...}.|.s1t...d..
+00005680: 017d 0488 0164 0319 0064 0a19 007d 057c  .}...d...d...}.|
+00005690: 0573 4174 03a0 0564 0b7c 049b 009d 02a1  .sAt...d.|......
+000056a0: 017d 0574 036a 0564 0c7c 059b 0064 0d7c  .}.t.j.d.|...d.|
+000056b0: 049b 009d 0464 0e64 0f8d 027d 0674 067c  .....d.d...}.t.|
+000056c0: 0488 0164 0319 00a0 0764 1064 0ea1 0264  ...d.....d.d...d
+000056d0: 118d 027d 077a 087c 07a0 087c 057c 06a1  ...}.z.|...|.|..
+000056e0: 0201 0057 006e 1604 0074 0974 0a66 0279  ...W.n...t.t.f.y
+000056f0: 7801 007d 0801 007a 0874 03a0 0b64 127c  x..}...z.t...d.|
+00005700: 089b 009d 02a1 0182 0164 007d 087e 0877  .........d.}.~.w
+00005710: 0177 0074 0ca0 0da1 007d 097c 02a0 0764  .w.t.....}.|...d
+00005720: 13a1 0172 8f7c 0974 0e74 0f7c 02a0 0764  ...r.|.t.t.|...d
+00005730: 13a1 0183 0164 148d 0117 007d 0a6e 327c  .....d.....}.n2|
+00005740: 02a0 0764 15a1 0172 a17c 0974 0e74 0f7c  ...d...r.|.t.t.|
+00005750: 02a0 0764 15a1 0183 0164 168d 0117 007d  ...d.....d.....}
+00005760: 0a6e 207c 02a0 0764 17a1 0172 b37c 0974  .n |...d...r.|.t
+00005770: 0e74 0f7c 02a0 0764 17a1 0183 0164 188d  .t.|...d.....d..
+00005780: 0117 007d 0a6e 0e7c 07a0 10a1 007d 0b7c  ...}.n.|.....}.|
+00005790: 0b6a 117d 0c7c 0974 0e7c 0c64 198d 0117  .j.}.|.t.|.d....
+000057a0: 007d 0a7c 076a 127c 017c 097c 0a64 1a8d  .}.|.j.|.|.|.d..
+000057b0: 037d 0d64 0a7c 0569 0164 087c 0469 0164  .}.d.|.i.d.|.i.d
+000057c0: 1b7c 0d6a 1369 0164 047c 0169 0166 0489  .|.j.i.d.|.i.f..
+000057d0: 0164 0188 006a 0164 1c3c 007c 0388 006a  .d...j.d.<.|...j
+000057e0: 0164 1d3c 0064 0388 006a 0164 1e3c 007c  .d.<.d...j.d.<.|
+000057f0: 03a0 1464 1f87 0087 0166 0264 2064 2184  ...d.....f.d d!.
+00005800: 08a1 0201 0064 0053 0029 224e 4672 9900  .....d.S.)"NFr..
+00005810: 0000 7285 0000 00da 0c73 6573 7369 6f6e  ..r......session
+00005820: 5f6e 616d 6575 2800 0000 4765 7420 7065  _nameu(...Get pe
+00005830: 7273 6f6e 616c 2061 6363 6573 7320 746f  rsonal access to
+00005840: 6b65 6e20 666f 7220 7365 7373 696f 6e20  ken for session 
+00005850: c2ab f502 0000 00c2 bb7a 1b50 6c65 6173  .........z.Pleas
+00005860: 6520 656e 7465 7220 6120 7365 7373 696f  e enter a sessio
+00005870: 6e20 6e61 6d65 da0b 6f70 656e 6269 735f  n name..openbis_
+00005880: 7572 6c7a 1c50 6c65 6173 6520 656e 7465  urlz.Please ente
+00005890: 7220 7468 6520 6f70 656e 4249 5320 5552  r the openBIS UR
+000058a0: 4cda 0475 7365 727a 1a50 6c65 6173 6520  L..userz.Please 
+000058b0: 656e 7465 7220 7573 6572 6e61 6d65 2066  enter username f
+000058c0: 6f72 207a 0d50 6173 7377 6f72 6420 666f  or z.Password fo
+000058d0: 7220 fa01 4054 2901 da0a 6869 6465 5f69  r ..@T)...hide_i
+000058e0: 6e70 7574 7227 0000 0029 0172 2700 0000  nputr'...).r'...
+000058f0: 7a1b 4361 6e6e 6f74 2063 6f6e 6e65 6374  z.Cannot connect
+00005900: 2074 6f20 6f70 656e 4249 533a 20da 0f76   to openBIS: ..v
+00005910: 616c 6964 6974 795f 6d6f 6e74 6873 2901  alidity_months).
+00005920: da06 6d6f 6e74 6873 da0e 7661 6c69 6469  ..months..validi
+00005930: 7479 5f77 6565 6b73 2901 da05 7765 656b  ty_weeks)...week
+00005940: 73da 0d76 616c 6964 6974 795f 6461 7973  s..validity_days
+00005950: 2901 da04 6461 7973 2901 da07 7365 636f  )...days)...seco
+00005960: 6e64 7329 03da 0b73 6573 7369 6f6e 4e61  nds)...sessionNa
+00005970: 6d65 da09 7661 6c69 6446 726f 6dda 0776  me..validFrom..v
+00005980: 616c 6964 546f da0d 6f70 656e 6269 735f  alidTo..openbis_
+00005990: 746f 6b65 6e72 8000 0000 7230 0000 0072  tokenr....r0...r
+000059a0: 8100 0000 72ee 0000 0063 0100 0000 0000  ....r....c......
+000059b0: 0000 0000 0000 0100 0000 0300 0000 1300  ................
+000059c0: 0000 72a9 0000 0072 1a00 0000 72aa 0000  ..r....r....r...
+000059d0: 0072 3200 0000 72ab 0000 0072 1200 0000  .r2...r....r....
+000059e0: 7213 0000 0072 3600 0000 0203 0000 7237  r....r6.......r7
+000059f0: 0000 007a 1b6e 6577 5f74 6f6b 656e 2e3c  ...z.new_token.<
+00005a00: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00005a10: 2915 7209 0000 0072 2a00 0000 729e 0000  ).r....r*...r...
+00005a20: 0072 1600 0000 7217 0000 00da 0670 726f  .r....r......pro
+00005a30: 6d70 7472 0400 0000 7298 0000 00da 056c  mptr....r......l
+00005a40: 6f67 696e 7205 0000 00da 0a56 616c 7565  oginr......Value
+00005a50: 4572 726f 72da 0e43 6c69 636b 4578 6365  Error..ClickExce
+00005a60: 7074 696f 6e72 0200 0000 da03 6e6f 7772  ptionr......nowr
+00005a70: 0300 0000 da03 696e 74da 1667 6574 5f73  ......int..get_s
+00005a80: 6572 7665 725f 696e 666f 726d 6174 696f  erver_informatio
+00005a90: 6eda 2a70 6572 736f 6e61 6c5f 6163 6365  n.*personal_acce
+00005aa0: 7373 5f74 6f6b 656e 735f 6d61 785f 7661  ss_tokens_max_va
+00005ab0: 6c69 6469 7479 5f70 6572 696f 64da 2367  lidity_period.#g
+00005ac0: 6574 5f6f 725f 6372 6561 7465 5f70 6572  et_or_create_per
+00005ad0: 736f 6e61 6c5f 6163 6365 7373 5f74 6f6b  sonal_access_tok
+00005ae0: 656e da06 7065 726d 4964 7238 0000 0029  en..permIdr8...)
+00005af0: 0e72 2b00 0000 7217 0100 00da 066b 7761  .r+...r......kwa
+00005b00: 7267 7372 3000 0000 da03 7572 6cda 0875  rgsr0.....url..u
+00005b10: 7365 726e 616d 65da 0870 6173 7377 6f72  sername..passwor
+00005b20: 64da 016f da03 6578 6372 2501 0000 7226  d..o..excr%...r&
+00005b30: 0100 00da 0a73 6572 7665 7269 6e66 6f72  .....serverinfor
+00005b40: 2301 0000 da09 746f 6b65 6e5f 6f62 6a72  #.....token_objr
+00005b50: 1200 0000 72ab 0000 0072 1300 0000 da09  ....r....r......
+00005b60: 6e65 775f 746f 6b65 6ec8 0200 0073 6600  new_token....sf.
+00005b70: 0000 0e07 0801 0402 0c01 0401 1401 0a02  ................
+00005b80: 0c02 0401 0a01 0c02 0401 1001 1a01 0c01  ................
+00005b90: 0401 08ff 0202 1001 1201 1001 0880 02ff  ................
+00005ba0: 0803 0a01 0201 1201 06ff 0a02 0201 1201  ................
+00005bb0: 06ff 0a02 0201 1201 06ff 0803 0601 0e01  ................
+00005bc0: 0401 0601 06ff 0603 0601 0801 0601 04fc  ................
+00005bd0: 0a07 0a01 0a01 1a01 723a 0100 00da 0661  ........r:.....a
+00005be0: 6464 7265 667a 3341 6464 2074 6865 2067  ddrefz3Add the g
+00005bf0: 6976 656e 2072 6570 6f73 6974 6f72 7920  iven repository 
+00005c00: 6173 2061 2072 6566 6572 656e 6365 2074  as a reference t
+00005c10: 6f20 6f70 656e 4249 532e 6302 0000 0000  o openBIS.c.....
+00005c20: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00005c30: 0000 0072 0501 0000 2905 fa22 5573 6564  ...r....).."Used
+00005c40: 2066 6f72 2045 7874 6572 6e61 6c20 4461   for External Da
+00005c50: 7461 2053 746f 7265 206f 6e6c 792e 7230  ta Store only.r0
+00005c60: 0000 0072 3b01 0000 6301 0000 0000 0000  ...r;...c.......
+00005c70: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
+00005c80: 0072 0801 0000 721a 0000 0029 0172 3b01  .r....r....).r;.
+00005c90: 0000 7232 0000 0072 1200 0000 7212 0000  ..r2...r....r...
+00005ca0: 0072 1300 0000 7236 0000 0010 0300 0072  .r....r6.......r
+00005cb0: 0901 0000 7a23 7265 706f 7369 746f 7279  ....z#repository
+00005cc0: 5f61 6464 7265 662e 3c6c 6f63 616c 733e  _addref.<locals>
+00005cd0: 2e3c 6c61 6d62 6461 3e72 ac00 0000 720a  .<lambda>r....r.
+00005ce0: 0100 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00005cf0: 0000 da11 7265 706f 7369 746f 7279 5f61  ....repository_a
+00005d00: 6464 7265 660b 0300 0072 0b01 0000 723d  ddref....r....r=
+00005d10: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
+00005d20: 0200 0000 0400 0000 4300 0000 720c 0100  ........C...r...
+00005d30: 0029 0672 3c01 0000 4672 9900 0000 7230  .).r<...Fr....r0
+00005d40: 0000 0072 0d01 0000 4e29 0472 0900 0000  ...r....N).r....
+00005d50: 722a 0000 0072 fd00 0000 723d 0100 0072  r*...r....r=...r
+00005d60: 0a01 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00005d70: 0000 0072 3b01 0000 1303 0000 720e 0100  ...r;.......r...
+00005d80: 007a 0d2d 2d64 6174 615f 7365 745f 6964  .z.--data_set_id
+00005d90: 7a4b 5265 6d6f 7665 2072 6566 2062 7920  zKRemove ref by 
+00005da0: 6461 7461 2073 6574 2069 642c 2069 6e20  data set id, in 
+00005db0: 6361 7365 2074 6865 2072 6570 6f73 6974  case the reposit
+00005dc0: 6f72 7920 6973 206e 6f74 2061 7661 696c  ory is not avail
+00005dd0: 6162 6c65 2061 6e79 6d6f 7265 2eda 0972  able anymore...r
+00005de0: 656d 6f76 6572 6566 7a3a 5265 6d6f 7665  emoverefz:Remove
+00005df0: 2074 6865 2072 6566 6572 656e 6365 2074   the reference t
+00005e00: 6f20 7468 6520 6769 7665 6e20 7265 706f  o the given repo
+00005e10: 7369 746f 7279 2066 726f 6d20 6f70 656e  sitory from open
+00005e20: 4249 532e 6303 0000 0000 0000 0000 0000  BIS.c...........
+00005e30: 0003 0000 0006 0000 0003 0000 0073 3800  .............s8.
+00005e40: 0000 8800 6401 7501 720e 7c02 6401 7501  ....d.u.r.|.d.u.
+00005e50: 720e 7400 6402 8301 0100 6403 5300 7c00  r.t.d.....d.S.|.
+00005e60: 6a01 6404 1900 a002 6405 8700 6601 6406  j.d.....d...f.d.
+00005e70: 6407 8408 7c02 a103 5300 2908 723c 0100  d...|...S.).r<..
+00005e80: 004e 7a2f 4f6e 6c79 2070 726f 7669 6465  .Nz/Only provide
+00005e90: 2074 6865 2064 6174 615f 7365 7420 6964   the data_set id
+00005ea0: 204f 5220 7468 6520 7265 706f 7369 746f   OR the reposito
+00005eb0: 7279 2e72 3b00 0000 7230 0000 0072 3e01  ry.r;...r0...r>.
+00005ec0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
+00005ed0: 0000 0003 0000 0013 0000 0073 0c00 0000  ...........s....
+00005ee0: 7c00 6a00 8800 6401 8d01 5300 2902 4ea9  |.j...d...S.).N.
+00005ef0: 01da 0b64 6174 615f 7365 745f 6964 2901  ...data_set_id).
+00005f00: 723e 0100 0072 3200 0000 723f 0100 0072  r>...r2...r?...r
+00005f10: 1200 0000 7213 0000 0072 3600 0000 3003  ....r....r6...0.
+00005f20: 0000 7240 0000 007a 2672 6570 6f73 6974  ..r@...z&reposit
+00005f30: 6f72 795f 7265 6d6f 7665 7265 662e 3c6c  ory_removeref.<l
+00005f40: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00005f50: 0372 0800 0000 722a 0000 0072 3800 0000  .r....r*...r8...
+00005f60: a903 722b 0000 0072 4001 0000 7239 0000  ..r+...r@...r9..
+00005f70: 0072 1200 0000 723f 0100 0072 1300 0000  .r....r?...r....
+00005f80: da14 7265 706f 7369 746f 7279 5f72 656d  ..repository_rem
+00005f90: 6f76 6572 6566 2703 0000 730c 0000 0010  overef'...s.....
+00005fa0: 0608 0104 0116 0102 0104 ff72 4201 0000  ...........rB...
+00005fb0: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
+00005fc0: 0005 0000 0043 0000 0072 1501 0000 2906  .....C...r....).
+00005fd0: 723c 0100 0046 7299 0000 0072 3000 0000  r<...Fr....r0...
+00005fe0: 2902 7240 0100 0072 3900 0000 4e29 0472  ).r@...r9...N).r
+00005ff0: 0900 0000 722a 0000 0072 fd00 0000 7242  ....r*...r....rB
+00006000: 0100 0072 4101 0000 7212 0000 0072 1200  ...rA...r....r..
+00006010: 0000 7213 0000 0072 3e01 0000 3403 0000  ..r....r>...4...
+00006020: 7308 0000 0014 0508 0102 010a ff72 4001  s............r@.
+00006030: 0000 7a0a 2d66 726f 6d2d 6669 6c65 7a0b  ..z.-from-filez.
+00006040: 2d2d 6672 6f6d 2d66 696c 65da 0966 726f  --from-file..fro
+00006050: 6d5f 6669 6c65 7a6a 416e 206f 7574 7075  m_filezjAn outpu
+00006060: 7420 2e43 5356 2066 696c 6520 6672 6f6d  t .CSV file from
+00006070: 2060 6f62 6973 2064 6174 615f 7365 7420   `obis data_set 
+00006080: 7365 6172 6368 6020 636f 6d6d 616e 6420  search` command 
+00006090: 7769 7468 2074 6865 206c 6973 7420 6f66  with the list of
+000060a0: 206f 626a 6563 7473 2074 6f20 646f 776e   objects to down
+000060b0: 6c6f 6164 2064 6174 6173 6574 7320 6672  load datasets fr
+000060c0: 6f6d 7a02 2d66 7a06 2d2d 6669 6c65 da04  omz.-fz.--file..
+000060d0: 6669 6c65 7a40 4669 6c65 2069 6e20 7468  filez@File in th
+000060e0: 6520 6461 7461 2073 6574 2074 6f20 646f  e data set to do
+000060f0: 776e 6c6f 6164 202d 2064 6f77 6e6c 6f61  wnload - downloa
+00006100: 6469 6e67 2061 6c6c 2069 6620 6e6f 7420  ding all if not 
+00006110: 6769 7665 6e2e 7a16 2d2d 736b 6970 5f69  given.z.--skip_i
+00006120: 6e74 6567 7269 7479 5f63 6865 636b 7a30  ntegrity_checkz0
+00006130: 466c 6167 2074 6f20 736b 6970 2066 696c  Flag to skip fil
+00006140: 6520 696e 7465 6772 6974 7920 6368 6563  e integrity chec
+00006150: 6b20 7769 7468 2063 6865 636b 7375 6d73  k with checksums
+00006160: da08 646f 776e 6c6f 6164 7a1d 446f 776e  ..downloadz.Down
+00006170: 6c6f 6164 2066 696c 6573 206f 6620 6120  load files of a 
+00006180: 6461 7461 2073 6574 2e63 0500 0000 0000  data set.c......
+00006190: 0000 0000 0000 0500 0000 0700 0000 0300  ................
+000061a0: 0000 7360 0000 0088 0064 0175 0072 0888  ..s`.....d.u.r..
+000061b0: 0264 0175 0073 1088 0064 0175 0172 1688  .d.u.s...d.u.r..
+000061c0: 0264 0175 0172 1674 0064 0283 0101 0064  .d.u.r.t.d.....d
+000061d0: 0353 0074 017c 006a 0264 0464 058d 027c  .S.t.|.j.d.d...|
+000061e0: 006a 0264 063c 007c 006a 0264 0619 00a0  .j.d.<.|.j.d....
+000061f0: 0364 0787 0087 0187 0287 0366 0464 0864  .d.........f.d.d
+00006200: 0984 08a1 0253 0029 0a7a 7620 446f 776e  .....S.).zv Down
+00006210: 6c6f 6164 7320 6461 7461 7365 7420 6669  loads dataset fi
+00006220: 6c65 7320 6672 6f6d 204f 7065 6e42 4953  les from OpenBIS
+00006230: 2069 6e73 7461 6e63 652e 0a0a 2020 2020   instance...    
+00006240: 4441 5441 5f53 4554 2020 2020 556e 6971  DATA_SET    Uniq
+00006250: 7565 2069 6465 6e74 6966 6965 7220 6f66  ue identifier of
+00006260: 2064 6174 6173 6574 2077 6974 6869 6e20   dataset within 
+00006270: 4f70 656e 4249 5320 696e 7374 616e 6365  OpenBIS instance
+00006280: 2e4e 7a2e 2764 6174 615f 7365 745f 6964  .Nz.'data_set_id
+00006290: 2720 6f72 2027 6672 6f6d 5f66 696c 6527  ' or 'from_file'
+000062a0: 206d 7573 7420 6265 2070 726f 7669 6465   must be provide
+000062b0: 6421 723b 0000 0046 7299 0000 0072 3000  d!r;...Fr....r0.
+000062c0: 0000 7245 0100 0063 0100 0000 0000 0000  ..rE...c........
+000062d0: 0000 0000 0100 0000 0600 0000 1300 0000  ................
+000062e0: 7312 0000 007c 006a 0088 0088 0288 0188  s....|.j........
+000062f0: 0364 018d 0453 0029 024e 2904 7240 0100  .d...S.).N).r@..
+00006300: 0072 4301 0000 7244 0100 00da 1473 6b69  .rC...rD.....ski
+00006310: 705f 696e 7465 6772 6974 795f 6368 6563  p_integrity_chec
+00006320: 6b29 0172 4501 0000 7232 0000 00a9 0472  k).rE...r2.....r
+00006330: 4001 0000 7244 0100 0072 4301 0000 7246  @...rD...rC...rF
+00006340: 0100 0072 1200 0000 7213 0000 0072 3600  ...r....r....r6.
+00006350: 0000 5b03 0000 7308 0000 0006 0004 0102  ..[...s.........
+00006360: 0106 fe7a 1a64 6f77 6e6c 6f61 642e 3c6c  ...z.download.<l
+00006370: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00006380: 0472 0800 0000 7209 0000 0072 2a00 0000  .r....r....r*...
+00006390: 7238 0000 0029 0572 2b00 0000 7240 0100  r8...).r+...r@..
+000063a0: 0072 4301 0000 7244 0100 0072 4601 0000  .rC...rD...rF...
+000063b0: 7212 0000 0072 4701 0000 7213 0000 0072  r....rG...r....r
+000063c0: 4501 0000 4f03 0000 7316 0000 0010 0606  E...O...s.......
+000063d0: 0102 ff06 0102 ff08 0204 0114 010c 0110  ................
+000063e0: 0104 ffda 0566 696c 6573 7a1c 6669 6c65  .....filesz.file
+000063f0: 206f 7220 6469 7265 6374 6f72 7920 746f   or directory to
+00006400: 2075 706c 6f61 642e 2903 7225 0000 0072   upload.).r%...r
+00006410: f300 0000 da08 6d75 6c74 6970 6c65 da09  ......multiple..
+00006420: 7361 6d70 6c65 5f69 64da 0d64 6174 615f  sample_id..data_
+00006430: 7365 745f 7479 7065 da06 7570 6c6f 6164  set_type..upload
+00006440: 7a20 5570 6c6f 6164 2066 696c 6573 2074  z Upload files t
+00006450: 6f20 666f 726d 2061 2064 6174 6120 7365  o form a data se
+00006460: 742e 6304 0000 0000 0000 0000 0000 0004  t.c.............
+00006470: 0000 0006 0000 0003 0000 0073 3600 0000  ...........s6...
+00006480: 7400 7c00 6a01 6401 6402 8d02 7c00 6a01  t.|.j.d.d...|.j.
+00006490: 6403 3c00 7c00 6a01 6403 1900 a002 6404  d.<.|.j.d.....d.
+000064a0: 8700 8701 8702 6603 6405 6406 8408 a102  ......f.d.d.....
+000064b0: 0100 6407 5300 2908 7aaa 2043 7265 6174  ..d.S.).z. Creat
+000064c0: 6573 2064 6174 6120 7365 7420 756e 6465  es data set unde
+000064d0: 7220 6f62 6a65 6374 2061 6e64 2075 706c  r object and upl
+000064e0: 6f61 6420 6669 6c65 7320 746f 2069 742e  oad files to it.
+000064f0: 0a0a 2020 2020 5341 4d50 4c45 5f49 4420  ..    SAMPLE_ID 
+00006500: 2020 2020 2020 556e 6971 7565 2069 6465        Unique ide
+00006510: 6e74 6966 6965 7220 616e 206f 626a 6563  ntifier an objec
+00006520: 7420 696e 204f 7065 6e42 4953 2e0a 0a20  t in OpenBIS... 
+00006530: 2020 2044 4154 415f 5345 545f 5459 5045     DATA_SET_TYPE
+00006540: 2020 204e 6577 6c79 2063 7265 6174 6564     Newly created
+00006550: 2064 6174 6120 7365 7420 7479 7065 2e0a   data set type..
+00006560: 2020 2020 4672 9900 0000 7230 0000 0072      Fr....r0...r
+00006570: 4c01 0000 6301 0000 0000 0000 0000 0000  L...c...........
+00006580: 0001 0000 0005 0000 0013 0000 0072 f600  .............r..
+00006590: 0000 721a 0000 0029 0172 4c01 0000 7232  ..r....).rL...r2
+000065a0: 0000 00a9 0372 4b01 0000 7248 0100 0072  .....rK...rH...r
+000065b0: 4a01 0000 7212 0000 0072 1300 0000 7236  J...r....r....r6
+000065c0: 0000 0075 0300 0072 d700 0000 7a18 7570  ...u...r....z.up
+000065d0: 6c6f 6164 2e3c 6c6f 6361 6c73 3e2e 3c6c  load.<locals>.<l
+000065e0: 616d 6264 613e 4e29 0372 0900 0000 722a  ambda>N).r....r*
+000065f0: 0000 0072 3800 0000 2904 722b 0000 0072  ...r8...).r+...r
+00006600: 4a01 0000 724b 0100 0072 4801 0000 7212  J...rK...rH...r.
+00006610: 0000 0072 4d01 0000 7213 0000 0072 4c01  ...rM...r....rL.
+00006620: 0000 6b03 0000 7308 0000 0014 080c 010e  ..k...s.........
+00006630: 0108 ff7a 022d 757a 0a2d 2d73 7368 5f75  ...z.-uz.--ssh_u
+00006640: 7365 727a 2955 7365 7220 746f 2063 6f6e  serz)User to con
+00006650: 6e65 6374 2074 6f20 7265 6d6f 7465 2073  nect to remote s
+00006660: 7973 7465 6d73 2076 6961 2073 7368 7a02  ystems via sshz.
+00006670: 2d63 7a14 2d2d 636f 6e74 656e 745f 636f  -cz.--content_co
+00006680: 7079 5f69 6e64 6578 7a49 496e 6465 7820  py_indexzIIndex 
+00006690: 6f66 2074 6865 2063 6f6e 7465 6e74 2063  of the content c
+000066a0: 6f70 7920 746f 2063 6c6f 6e65 2066 726f  opy to clone fro
+000066b0: 6d20 696e 2063 6173 6520 7468 6572 6520  m in case there 
+000066c0: 6172 6520 6d75 6c74 6970 6c65 2063 6f70  are multiple cop
+000066d0: 6965 7329 0372 0d00 0000 7223 0000 0072  ies).r....r#...r
+000066e0: 2500 0000 7a29 536b 6970 2066 696c 6520  %...z)Skip file 
+000066f0: 696e 7465 6772 6974 7920 6368 6563 6b20  integrity check 
+00006700: 7769 7468 2063 6865 636b 7375 6d73 2eda  with checksums..
+00006710: 0563 6c6f 6e65 7a34 436c 6f6e 6520 7468  .clonez4Clone th
+00006720: 6520 7265 706f 7369 746f 7279 2066 6f75  e repository fou
+00006730: 6e64 2069 6e20 7468 6520 6769 7665 6e20  nd in the given 
+00006740: 6461 7461 2073 6574 2069 642e 6305 0000  data set id.c...
+00006750: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+00006760: 0003 0000 00f3 2000 0000 7c00 6a00 6401  ...... ...|.j.d.
+00006770: 1900 a001 6402 8700 8701 8702 8703 6604  ....d.........f.
+00006780: 6403 6404 8408 a102 5300 2905 4e72 3000  d.d.....S.).Nr0.
+00006790: 0000 724e 0100 0063 0100 0000 0000 0000  ..rN...c........
+000067a0: 0000 0000 0100 0000 0600 0000 1300 0000  ................
+000067b0: f310 0000 007c 00a0 0088 0188 0388 0088  .....|..........
+000067c0: 02a1 0453 0072 1a00 0000 2901 724e 0100  ...S.r....).rN..
+000067d0: 0072 3200 0000 a904 da12 636f 6e74 656e  .r2.......conten
+000067e0: 745f 636f 7079 5f69 6e64 6578 7240 0100  t_copy_indexr@..
+000067f0: 0072 4601 0000 da08 7373 685f 7573 6572  .rF.....ssh_user
+00006800: 7212 0000 0072 1300 0000 7236 0000 008b  r....r....r6....
+00006810: 0300 00f3 0600 0000 0a00 0201 04ff 7a20  ..............z 
+00006820: 6461 7461 5f73 6574 5f63 6c6f 6e65 2e3c  data_set_clone.<
+00006830: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00006840: 72ac 0000 00a9 0572 2b00 0000 7253 0100  r......r+...rS..
+00006850: 0072 5201 0000 7240 0100 0072 4601 0000  .rR...r@...rF...
+00006860: 7212 0000 0072 5101 0000 7213 0000 00da  r....rQ...r.....
+00006870: 0e64 6174 615f 7365 745f 636c 6f6e 6586  .data_set_clone.
+00006880: 0300 00f3 0600 0000 0c04 1001 04ff 7256  ..............rV
+00006890: 0100 0063 0500 0000 0000 0000 0000 0000  ...c............
+000068a0: 0500 0000 0700 0000 4300 0000 f32c 0000  ........C....,..
+000068b0: 0074 007c 006a 0164 0164 028d 027c 006a  .t.|.j.d.d...|.j
+000068c0: 0164 033c 007c 006a 0274 037c 017c 027c  .d.<.|.j.t.|.|.|
+000068d0: 037c 0464 048d 0501 0064 0053 00a9 054e  .|.d.....d.S...N
+000068e0: 4672 9900 0000 7230 0000 0029 0472 5301  Fr....r0...).rS.
+000068f0: 0000 7252 0100 0072 4001 0000 7246 0100  ..rR...r@...rF..
+00006900: 0029 0472 0900 0000 722a 0000 0072 fd00  .).r....r*...r..
+00006910: 0000 7256 0100 0072 5501 0000 7212 0000  ..rV...rU...r...
+00006920: 0072 1200 0000 7213 0000 0072 4e01 0000  .r....r....rN...
+00006930: 8f03 0000 f308 0000 0014 040a 0104 010a  ................
+00006940: ffda 046d 6f76 657a 334d 6f76 6520 7468  ...movez3Move th
+00006950: 6520 7265 706f 7369 746f 7279 2066 6f75  e repository fou
+00006960: 6e64 2069 6e20 7468 6520 6769 7665 6e20  nd in the given 
+00006970: 6461 7461 2073 6574 2069 642e 6305 0000  data set id.c...
+00006980: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+00006990: 0003 0000 0072 4f01 0000 2905 4e72 3000  .....rO...).Nr0.
+000069a0: 0000 725b 0100 0063 0100 0000 0000 0000  ..r[...c........
+000069b0: 0000 0000 0100 0000 0600 0000 1300 0000  ................
+000069c0: 7250 0100 0072 1a00 0000 2901 725b 0100  rP...r....).r[..
+000069d0: 0072 3200 0000 7251 0100 0072 1200 0000  .r2...rQ...r....
+000069e0: 7213 0000 0072 3600 0000 9f03 0000 7254  r....r6.......rT
+000069f0: 0100 007a 1f64 6174 615f 7365 745f 6d6f  ...z.data_set_mo
+00006a00: 7665 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ve.<locals>.<lam
+00006a10: 6264 613e 72ac 0000 0072 5501 0000 7212  bda>r....rU...r.
+00006a20: 0000 0072 5101 0000 7213 0000 00da 0d64  ...rQ...r......d
+00006a30: 6174 615f 7365 745f 6d6f 7665 9a03 0000  ata_set_move....
+00006a40: 7257 0100 0072 5c01 0000 6305 0000 0000  rW...r\...c.....
+00006a50: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
+00006a60: 0000 0072 5801 0000 7259 0100 0029 0472  ...rX...rY...).r
+00006a70: 0900 0000 722a 0000 0072 fd00 0000 725c  ....r*...r....r\
+00006a80: 0100 0072 5501 0000 7212 0000 0072 1200  ...rU...r....r..
+00006a90: 0000 7213 0000 0072 5b01 0000 a303 0000  ..r....r[.......
+00006aa0: 725a 0100 0063 0000 0000 0000 0000 0000  rZ...c..........
+00006ab0: 0000 0000 0000 0300 0000 4300 0000 730e  ..........C...s.
+00006ac0: 0000 0074 0069 0064 018d 0101 0064 0053  ...t.i.d.....d.S
+00006ad0: 0029 024e 7229 0000 0029 0172 2d00 0000  .).Nr)...).r-...
+00006ae0: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00006af0: 1300 0000 da04 6d61 696e ac03 0000 7302  ......main....s.
+00006b00: 0000 000e 0172 5d01 0000 da08 5f5f 6d61  .....r].....__ma
+00006b10: 696e 5f5f 2902 4e4e 721a 0000 0029 68da  in__).NNr....)h.
+00006b20: 075f 5f64 6f63 5f5f 729f 0000 0072 4100  .__doc__r....rA.
+00006b30: 0000 7202 0000 0072 1600 0000 da16 6461  ..r....r......da
+00006b40: 7465 7574 696c 2e72 656c 6174 6976 6564  teutil.relatived
+00006b50: 656c 7461 7203 0000 00da 0570 7962 6973  eltar......pybis
+00006b60: 7204 0000 00da 0872 6571 7565 7374 7372  r......requestsr
+00006b70: 0500 0000 da0a 636c 6963 6b5f 7574 696c  ......click_util
+00006b80: 7208 0000 00da 1064 6174 615f 6d67 6d74  r......data_mgmt
+00006b90: 5f72 756e 6e65 7272 0900 0000 da11 646d  _runnerr......dm
+00006ba0: 2e63 6f6d 6d61 6e64 5f72 6573 756c 7472  .command_resultr
+00006bb0: 0b00 0000 da08 646d 2e75 7469 6c73 720c  ......dm.utilsr.
+00006bc0: 0000 0072 1400 0000 7219 0000 0072 2100  ...r....r....r!.
+00006bd0: 0000 da05 6772 6f75 70da 0e76 6572 7369  ....group..versi
+00006be0: 6f6e 5f6f 7074 696f 6eda 066f 7074 696f  on_option..optio
+00006bf0: 6eda 0c70 6173 735f 636f 6e74 6578 7472  n..pass_contextr
+00006c00: 2d00 0000 723a 0000 0072 4900 0000 da09  -...r:...rI.....
+00006c10: 5061 7261 6d54 7970 6572 4a00 0000 7264  ParamTyperJ...rd
+00006c20: 0000 0072 6500 0000 727c 0000 0072 7f00  ...re...r|...r..
+00006c30: 0000 7287 0000 0072 8d00 0000 7293 0000  ..r....r....r...
+00006c40: 0072 9600 0000 726a 0000 00da 0763 6f6d  .r....rj.....com
+00006c50: 6d61 6e64 724b 0000 0072 3900 0000 da08  mandrK...r9.....
+00006c60: 6172 6775 6d65 6e74 72a8 0000 0072 ae00  argumentr....r..
+00006c70: 0000 72b1 0000 00da 0e5f 7365 6172 6368  ..r......_search
+00006c80: 5f70 6172 616d 7372 ba00 0000 72bc 0000  _paramsr....r...
+00006c90: 0072 be00 0000 72bf 0000 0072 d100 0000  .r....r....r....
+00006ca0: 72de 0000 0072 e100 0000 72e4 0000 0072  r....r....r....r
+00006cb0: e500 0000 72e6 0000 0072 e800 0000 72e9  ....r....r....r.
+00006cc0: 0000 0072 ea00 0000 72eb 0000 0072 8500  ...r....r....r..
+00006cd0: 0000 72ee 0000 0072 ef00 0000 72f0 0000  ..r....r....r...
+00006ce0: 00da 0450 6174 68da 0e5f 636f 6d6d 6974  ...Path.._commit
+00006cf0: 5f70 6172 616d 7372 fc00 0000 72f4 0000  _paramsr....r...
+00006d00: 00da 0c5f 696e 6974 5f70 6172 616d 7372  ..._init_paramsr
+00006d10: 0001 0000 da15 5f69 6e69 745f 7061 7261  ......_init_para
+00006d20: 6d73 5f70 6879 7369 6361 6c72 ff00 0000  ms_physicalr....
+00006d30: da15 5f69 6e69 745f 616e 616c 7973 6973  .._init_analysis
+00006d40: 5f70 6172 616d 7372 0301 0000 723c 0000  _paramsr....r<..
+00006d50: 00da 0e5f 7374 6174 7573 5f70 6172 616d  ..._status_param
+00006d60: 7372 0701 0000 7204 0100 00da 0c5f 7379  sr....r......_sy
+00006d70: 6e63 5f70 6172 616d 7372 1001 0000 7214  nc_paramsr....r.
+00006d80: 0100 0072 0f01 0000 7216 0100 0072 3a01  ...r....r....r:.
+00006d90: 0000 da0e 5f61 6464 7265 665f 7061 7261  ...._addref_para
+00006da0: 6d73 723d 0100 0072 3b01 0000 da11 5f72  msr=...r;....._r
+00006db0: 656d 6f76 6572 6566 5f70 6172 616d 7372  emoveref_paramsr
+00006dc0: 4201 0000 723e 0100 00da 105f 646f 776e  B...r>....._down
+00006dd0: 6c6f 6164 5f70 6172 616d 7372 4501 0000  load_paramsrE...
+00006de0: da0e 5f75 706c 6f61 645f 7061 7261 6d73  .._upload_params
+00006df0: 724c 0100 0072 2d01 0000 da12 5f63 6c6f  rL...r-....._clo
+00006e00: 6e65 5f6d 6f76 655f 7061 7261 6d73 7256  ne_move_paramsrV
+00006e10: 0100 0072 4e01 0000 725c 0100 0072 5b01  ...rN...r\...r[.
+00006e20: 0000 725d 0100 0072 6000 0000 7212 0000  ..r]...r`...r...
+00006e30: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00006e40: da08 3c6d 6f64 756c 653e 0100 0000 73b6  ..<module>....s.
+00006e50: 0200 0004 1208 0508 010c 0108 020c 010c  ................
+00006e60: 010c 010c 020c 010c 010c 0108 0308 0508  ................
+00006e70: 0506 090a 0112 010c 0102 0104 ff12 0204  ................
+00006e80: 0114 0108 0708 0912 1410 0f12 0408 2b08  ..............+.
+00006e90: 080c 0708 0b08 0708 0906 0b12 0104 010e  ................
+00006ea0: 0108 0504 010c 0106 0a12 0104 010e 0108  ................
+00006eb0: 0810 0104 010e 0108 0510 0104 010e 0108  ................
+00006ec0: 0510 0104 010e 010c 0902 0104 ff10 0210  ................
+00006ed0: 0110 010c 0102 0104 ff12 0210 010a 0102  ................
+00006ee0: 0104 ff0c 0202 0104 ff0c 0202 0104 ff10  ................
+00006ef0: 020e 0102 0104 ff04 ef08 1612 010c 0102  ................
+00006f00: 0104 ff04 0210 0108 0910 0104 010e 0108  ................
+00006f10: 0510 0104 010e 0108 0510 0104 010e 010c  ................
+00006f20: 0506 0104 010e 0106 1f12 0104 010e 0108  ................
+00006f30: 0b10 0104 010e 0108 0810 0104 010e 0108  ................
+00006f40: 0810 0104 010e 010c 0506 0104 010e 0106  ................
+00006f50: 1d12 0104 010e 0108 0b10 0104 010e 0108  ................
+00006f60: 0810 0104 010e 0108 0810 0104 010e 0106  ................
+00006f70: 0812 0104 010e 0108 0e10 0104 010e 0108  ................
+00006f80: 0810 0104 010e 0108 0810 0104 010e 010a  ................
+00006f90: 0b02 0104 ff0c 0202 0104 ff0a 0204 0104  ................
+00006fa0: ff0a 0204 0104 ff02 0104 ff04 f90c 0c04  ................
+00006fb0: 0106 010e 010a 0804 0106 010e 010a 0c04  ................
+00006fc0: 0104 ff02 0104 ff0c 0204 fd0c 0804 0106  ................
+00006fd0: 010e 0102 070e 0102 0106 ff02 ff02 ff0a  ................
+00006fe0: 0604 0106 010e 0108 0f0c 0104 ff04 ff08  ................
+00006ff0: 040c 0304 0106 010e 010c 0504 0106 010e  ................
+00007000: 010a 0b04 0104 ff02 0104 ff04 ff0c 0604  ................
+00007010: 0106 010e 010a 0504 0106 010e 010a 0a04  ................
+00007020: 0104 ff0a 0204 0104 ff02 0104 ff04 fd08  ................
+00007030: 080c 0504 0106 010e 010a 0604 0106 010e  ................
+00007040: 010a 0704 010c 010c 040c 010c 010c 010c  ................
+00007050: 0104 0118 010a 3804 0104 ff02 0104 ff04  ......8.........
+00007060: ff0c 0604 0106 010e 010a 0504 0106 010e  ................
+00007070: 0108 0a02 0104 ff0a 0204 0104 ff02 0104  ................
+00007080: ff04 fd06 0802 0104 ff04 0206 010e 010a  ................
+00007090: 0904 0106 010e 010c 0c0a 0102 0104 ff04  ................
+000070a0: 0306 0102 0104 fe0c 0302 0104 ff04 f80c  ................
+000070b0: 0d06 0104 010e 0104 120e 0106 ff0a 020a  ................
+000070c0: 0104 fc10 0806 0104 0112 010e 0e04 0104  ................
+000070d0: ff10 0204 0106 ff0a 0206 0104 ff08 0204  ................
+000070e0: f910 0b04 0106 0112 010c 0604 0106 0112  ................
+000070f0: 0110 0804 0106 0112 010c 0604 0106 0112  ................
+00007100: 010c 060c 040a 0104 ff                   .........
```

### Comparing `obis-0.4.1/obis/scripts/__pycache__/click_util.cpython-310.pyc` & `obis-0.4.2rc1/obis/scripts/__pycache__/click_util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc` & `obis-0.4.2rc1/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 28 13:09:09 2023 UTC, .py size: 5701 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f5fc fd63 4516 0000  o..........cE...
+00000000: 6f0d 0d0a 0000 0000 7a6b 2564 4516 0000  o.......zk%dE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 6404  d.l.m.Z.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6404 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6404 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6404 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `obis-0.4.1/obis/scripts/cli.py` & `obis-0.4.2rc1/obis/scripts/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -213,274 +213,330 @@
 
 # get all settings
 
 @cli.group()
 @click.option('-g', '--is_global', default=False, is_flag=True, help='Get global or local.')
 @click.pass_context
 def settings(ctx, is_global):
-    """ Get all settings.
-    """
+    """ External Data Store: Get all settings. """
     ctx.obj['is_global'] = is_global
 
 
 @settings.command('get')
 @click.pass_context
 def settings_get(ctx):
+    """ External Data Store: Get setting. """
     runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     settings = runner.get_settings()
     settings_str = json.dumps(settings, indent=4, sort_keys=True)
     click.echo("{}".format(settings_str))
 
 
 # repository: repository_id, external_dms_id, data_set_id
 
 @cli.group()
 @click.option('-g', '--is_global', default=False, is_flag=True, help='Set/get global or local.')
 @click.pass_context
 def repository(ctx, is_global):
-    """ Get/set settings related to the repository.
-    """
+    """ External Data Store: Get/set settings related to the repository. """
     runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.obj['is_global'] = is_global
     ctx.obj['runner'] = runner
     ctx.obj['resolver'] = 'repository'
 
 
 @repository.command('set')
 @click.argument('settings', type=SettingsSet(), nargs=-1)
 @click.pass_context
 def repository_set(ctx, settings):
+    """ External Data Store: Set settings related to the repository. """
     return ctx.obj['runner'].run("repository_set", lambda dm: _set(ctx, settings))
 
 
 @repository.command('get')
 @click.argument('settings', type=SettingsGet(), nargs=-1)
 @click.pass_context
 def repository_get(ctx, settings):
+    """ External Data Store: Get settings related to the repository. """
     return ctx.obj['runner'].run("repository_get", lambda dm: _get(ctx, settings))
 
 
 @repository.command('clear')
 @click.argument('settings', type=SettingsClear(), nargs=-1)
 @click.pass_context
 def repository_clear(ctx, settings):
+    """ External Data Store: Clear settings related to the repository. """
     return ctx.obj['runner'].run("repository_clear", lambda dm: _clear(ctx, settings))
 
 
 # data_set: type, properties
 
 
 _search_params = [
     click.option('-object_type', '--object_type', 'type_code', default=None,
                  help='Object type code to filter by'),
     click.option('-space', '--space', default=None, help='Space code'),
     click.option('-project', '--project', default=None, help='Full project identification code'),
     click.option('-experiment', '--experiment', default=None, help='Full experiment code'),
+    click.option('-object', '--object', 'object_code', default=None,
+                 help='Object identification information, it can be permId or identifier'),
     click.option('-type', '--type', 'type_code', default=None, help='Type code'),
     click.option('-property', 'property_code', default=None, help='Property code'),
     click.option('-property-value', 'property_value', default=None,
                  help='Property value'),
     click.option('-registration-date', '--registration-date', 'registration_date', default=None,
                  help='Registration date, it can be in the format "oYYYY-MM-DD" (e.g. ">2023-01-01")'),
     click.option('-modification-date', '--modification-date', 'modification_date', default=None,
                  help='Modification date, it can be in the format "oYYYY-MM-DD" (e.g. ">2023-01-01")'),
     click.option('-save', '--save', default=None, help='Filename to save results'),
+    click.option('-r', '--recursive', 'recursive', is_flag=True, default=False,
+                 help='Search data recursively'),
 ]
 
 
 @cli.group('data_set')
 @click.option('-g', '--is_global', default=False, is_flag=True, help='Set/get global or local.')
 @click.option('-p', '--is_data_set_property', default=False, is_flag=True,
               help='Configure data set property.')
 @click.pass_context
 def data_set(ctx, is_global, is_data_set_property):
-    """ Get/set settings related to the data set.
-    """
+    """ External Data Store: Get/set settings related to the data set. """
     runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.obj['is_global'] = is_global
     ctx.obj['is_data_set_property'] = is_data_set_property
     ctx.obj['runner'] = runner
     ctx.obj['resolver'] = 'data_set'
 
 
 @data_set.command('set')
 @click.argument('data_set_settings', type=SettingsSet(), nargs=-1)
 @click.pass_context
 def data_set_set(ctx, data_set_settings):
+    """ External Data Store: Set settings related to the data set. """
     return ctx.obj['runner'].run("data_set_set", lambda dm: _set(ctx, data_set_settings))
 
 
 @data_set.command('get')
 @click.argument('data_set_settings', type=SettingsGet(), nargs=-1)
 @click.pass_context
 def data_set_get(ctx, data_set_settings):
+    """ External Data Store: Get settings related to the data set. """
     return ctx.obj['runner'].run("data_set_get", lambda dm: _get(ctx, data_set_settings))
 
 
 @data_set.command('clear')
 @click.argument('data_set_settings', type=SettingsClear(), nargs=-1)
 @click.pass_context
 def data_set_clear(ctx, data_set_settings):
+    """ External Data Store: Clear settings related to the data set. """
     return ctx.obj['runner'].run("data_set_clear", lambda dm: _clear(ctx, data_set_settings))
 
 
 @data_set.command('search', short_help="Search for datasets using a filtering criteria.")
 @add_params(_search_params)
 @click.pass_context
 def data_set_search(ctx, type_code, space, project, experiment, registration_date,
-                    modification_date, property_code, property_value, save):
-    if all(v is None for v in
-           [type_code, space, project, experiment, registration_date, modification_date,
-            property_code, property_value]):
+                    modification_date, object_code, property_code, property_value, save, recursive):
+    """Standard Data Store: Search data sets given the filtering criteria or object identifier.
+    Results of this command can be used in `obis download`."""
+    filtering_arguments = [type_code, space, project, experiment, registration_date,
+                           modification_date,
+                           property_code, property_value]
+    if all(v is None for v in filtering_arguments + [object_code]):
         click_echo("You must provide at least one filtering criteria!")
         return -1
     if (property_code is None and property_value is not None) or (
             property_code is not None and property_value is None):
         click_echo("Property code and property value need to be specified!")
         return -1
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
-    filters = dict(type_code=type_code, space=space,
-                   project=project, experiment=experiment, property_code=property_code,
-                   registration_date=registration_date, modification_date=modification_date,
-                   property_value=property_value)
+    if object_code is not None:
+        if any(v is not None for v in filtering_arguments):
+            click_echo("Object parameter detected! Other filtering arguments will be omitted!")
+        filters = dict(object_code=object_code)
+    else:
+        filters = dict(type_code=type_code, space=space,
+                       project=project, experiment=experiment, property_code=property_code,
+                       registration_date=registration_date, modification_date=modification_date,
+                       property_value=property_value)
     return ctx.obj['runner'].run("data_set_search",
-                                 lambda dm: dm.search_data_set(filters, save)),
+                                 lambda dm: dm.search_data_set(filters, recursive, save)),
 
 
 # # object: object_id
 
 
 @cli.group()
 @click.option('-g', '--is_global', default=False, is_flag=True, help='Set/get global or local.')
 @click.pass_context
 def object(ctx, is_global):
-    """ Get/set settings related to the object.
+    """ External Data Store: Get/set properties related to the object.
+
+    Standard Data Store: Get/set properties of objects connected to downloaded datasets.
     """
     runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.obj['is_global'] = is_global
     ctx.obj['runner'] = runner
     ctx.obj['resolver'] = 'object'
 
 
 @object.command('set')
 @click.argument('object_settings', type=SettingsSet(), nargs=-1)
 @click.pass_context
 def object_set(ctx, object_settings):
+    """ External Data Store: Set properties related to the object.
+
+    Standard Data Store: Set property to all objects connected to downloaded datasets.
+    """
     return ctx.obj['runner'].run("object_set", lambda dm: _set(ctx, object_settings))
 
 
 @object.command('get')
 @click.argument('object_settings', type=SettingsGet(), nargs=-1)
 @click.pass_context
 def object_get(ctx, object_settings):
+    """ External Data Store: Set properties related to the object.
+
+    Standard Data Store: Get given properties of all objects connected to downloaded datasets.
+    """
     return ctx.obj['runner'].run("object_get", lambda dm: _get(ctx, object_settings))
 
 
 @object.command('clear')
 @click.argument('object_settings', type=SettingsClear(), nargs=-1)
 @click.pass_context
 def object_clear(ctx, object_settings):
+    """ External Data Store: Clear properties related to the object. """
     return ctx.obj['runner'].run("object_clear", lambda dm: _clear(ctx, object_settings))
 
 
 @object.command('search', short_help="Search for samples using a filtering criteria.")
 @add_params(_search_params)
 @click.pass_context
 def object_search(ctx, type_code, space, project, experiment, registration_date,
-                  modification_date, property_code, property_value, save):
-    if all(v is None for v in
-           [type_code, space, project, experiment, registration_date, modification_date,
-            property_code, property_value]):
+                  modification_date, object_code, property_code, property_value, save, recursive):
+    """Standard Data Store: Search for objects using a filtering criteria or object identifier."""
+    filtering_arguments = [type_code, space, project, experiment, registration_date,
+                           modification_date, property_code, property_value]
+    if all(v is None for v in filtering_arguments + [object_code]):
         click_echo("You must provide at least one filtering criteria!")
         return -1
     if (property_code is None and property_value is not None) or (
             property_code is not None and property_value is None):
         click_echo("Property code and property value need to be specified!")
         return -1
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
-    filters = dict(type_code=type_code, space=space,
-                   project=project, experiment=experiment, property_code=property_code,
-                   registration_date=registration_date, modification_date=modification_date,
-                   property_value=property_value)
+    if object_code is not None:
+        if any(v is not None for v in filtering_arguments):
+            click_echo("Object parameter detected! Other filtering arguments will be omitted!")
+        filters = dict(object_code=object_code)
+    else:
+        filters = dict(type_code=type_code, space=space,
+                       project=project, experiment=experiment, property_code=property_code,
+                       registration_date=registration_date, modification_date=modification_date,
+                       property_value=property_value)
     return ctx.obj['runner'].run("object_search",
-                                 lambda dm: dm.search_object(filters, save))
+                                 lambda dm: dm.search_object(filters, recursive, save))
 
 
 # # collection: collection_id
 
 
 @cli.group()
 @click.option('-g', '--is_global', default=False, is_flag=True, help='Set/get global or local.')
 @click.pass_context
 def collection(ctx, is_global):
-    """ Get/set settings related to the collection.
+    """ External Data Store: Get/set settings related to the collection.
+
+    Standard Data Store: Get/set properties of all collections connected to downloaded datasets.
     """
     runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.obj['is_global'] = is_global
     ctx.obj['runner'] = runner
     ctx.obj['resolver'] = 'collection'
 
 
 @collection.command('set')
 @click.argument('settings', type=SettingsSet(), nargs=-1)
 @click.pass_context
 def collection_set(ctx, settings):
+    """ External Data Store: Set settings related to the collection.
+
+    Standard Data Store: Set given properties of all collections connected to downloaded datasets.
+    """
     return ctx.obj['runner'].run("collection_set", lambda dm: _set(ctx, settings))
 
 
 @collection.command('get')
 @click.argument('settings', type=SettingsGet(), nargs=-1)
 @click.pass_context
 def collection_get(ctx, settings):
+    """ External Data Store: Get settings related to the collection.
+
+    Standard Data Store: Get given properties of all collections connected to downloaded datasets.
+    """
     return ctx.obj['runner'].run("collection_get", lambda dm: _get(ctx, settings))
 
 
 @collection.command('clear')
 @click.argument('settings', type=SettingsClear(), nargs=-1)
 @click.pass_context
 def collection_clear(ctx, settings):
+    """External Data Store: Clear settings related to the collection."""
     return ctx.obj['runner'].run("collection_clear", lambda dm: _clear(ctx, settings))
 
 
 # config: fileservice_url, git_annex_hash_as_checksum, hostname, openbis_url, user, verify_certificates
 
 
 @cli.group()
 @click.option('-g', '--is_global', default=False, is_flag=True, help='Set/get global or local.')
 @click.pass_context
 def config(ctx, is_global):
-    """ Get/set configurations.
+    """External Data Store: Get/set configurations.
+
+    Standard Data Store: Get/set configurations.
     """
     if is_global is True:
         runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False, is_physical=True)
     else:
         runner = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.obj['is_global'] = is_global
     ctx.obj['runner'] = runner
     ctx.obj['resolver'] = 'config'
 
 
 @config.command('set')
 @click.argument('settings', type=SettingsSet(), nargs=-1)
 @click.pass_context
 def config_set(ctx, settings):
+    """External Data Store: Set configurations.
+
+    Standard Data Store: Set configurations.
+    """
     return ctx.obj['runner'].run("config_set", lambda dm: _set(ctx, settings))
 
 
 @config.command('get')
 @click.argument('settings', type=SettingsGet(), nargs=-1)
 @click.pass_context
 def config_get(ctx, settings):
+    """External Data Store: Get configurations.
+
+    Standard Data Store: Get configurations.
+    """
     return ctx.obj['runner'].run("config_get", lambda dm: _get(ctx, settings))
 
 
 @config.command('clear')
 @click.argument('settings', type=SettingsClear(), nargs=-1)
 @click.pass_context
 def config_clear(ctx, settings):
+    """External Data Store: Clear configurations.
+    """
     return ctx.obj['runner'].run("config_clear", lambda dm: _clear(ctx, settings))
 
 
 # repository commands: status, sync, commit, init, addref, removeref, init_analysis
 
 # commit
 
@@ -496,23 +552,27 @@
 ]
 
 
 @repository.command("commit", short_help="Commit the repository to git and inform openBIS.")
 @click.pass_context
 @add_params(_commit_params)
 def repository_commit(ctx, msg, auto_add, ignore_missing_parent, repository):
+    """External Data Store: Commit the repository to git and inform openBIS.
+    """
     return ctx.obj['runner'].run("commit",
                                  lambda dm: dm.commit(msg, auto_add, ignore_missing_parent),
                                  repository)
 
 
 @cli.command(short_help="Commit the repository to git and inform openBIS.")
 @click.pass_context
 @add_params(_commit_params)
 def commit(ctx, msg, auto_add, ignore_missing_parent, repository):
+    """External Data Store: Commit the repository to git and inform openBIS.
+    """
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.invoke(repository_commit, msg=msg, auto_add=auto_add,
                ignore_missing_parent=ignore_missing_parent, repository=repository)
 
 
 # init
 
@@ -525,27 +585,35 @@
 ]
 
 
 @repository.command("init", short_help="Initialize the folder as a data repository.")
 @click.pass_context
 @add_params(_init_params)
 def repository_init(ctx, repository_path, description):
+    """External Data Store: Initialize the folder as a data repository.
+    """
     return init_data_impl(ctx, repository_path, description)
 
 
 _init_params_physical = \
     _init_params + \
     [click.option('-p', '--physical', 'is_physical', default=False, is_flag=True,
-                  help='If parent data set is missing, ignore it.')]
+                  help='Initialize folder for Standard Data Store data handling.')]
 
 
 @cli.command(short_help="Initialize the folder as a data repository.")
 @click.pass_context
 @add_params(_init_params_physical)
 def init(ctx, repository_path, description, is_physical):
+    """External Data Store: Initialize the folder as a data repository for External Data Store
+    data handling.
+
+    Standard Data Store: Initialize the folder as a data repository for Standard Data Store
+    data handling.
+    """
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False, is_physical=is_physical)
     ctx.invoke(repository_init, repository_path=repository_path, description=description)
 
 
 # init analysis
 
 
@@ -556,21 +624,23 @@
 _init_analysis_params += _init_params
 
 
 @repository.command("init_analysis", short_help="Initialize the folder as an analysis folder.")
 @click.pass_context
 @add_params(_init_analysis_params)
 def repository_init_analysis(ctx, parent, repository_path, description):
+    """External Data Store: Initialize the folder as an analysis folder."""
     return init_analysis_impl(ctx, parent, repository_path, description)
 
 
 @cli.command(name='init_analysis', short_help="Initialize the folder as an analysis folder.")
 @click.pass_context
 @add_params(_init_analysis_params)
 def init_analysis(ctx, parent, repository_path, description):
+    """External Data Store: Initialize the folder as an analysis folder."""
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.invoke(repository_init_analysis, parent=parent,
                repository_path=repository_path, description=description)
 
 
 # status
 
@@ -581,21 +651,23 @@
 ]
 
 
 @repository.command("status", short_help="Show the state of the obis repository.")
 @click.pass_context
 @add_params(_status_params)
 def repository_status(ctx, repository):
+    """External Data Store: Show the state of the obis repository."""
     return ctx.obj['runner'].run("repository_status", lambda dm: dm.status(), repository)
 
 
 @cli.command(short_help="Show the state of the obis repository.")
 @click.pass_context
 @add_params(_status_params)
 def status(ctx, repository):
+    """External Data Store: Show the state of the obis repository."""
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.invoke(repository_status, repository=repository)
 
 
 # sync
 
 
@@ -612,22 +684,24 @@
     return dm.sync()
 
 
 @repository.command("sync", short_help="Sync the repository with openBIS.")
 @click.pass_context
 @add_params(_sync_params)
 def repository_sync(ctx, ignore_missing_parent, repository):
+    """External Data Store: Sync the repository with openBIS."""
     return ctx.obj['runner'].run("sync", lambda dm: _repository_sync(dm, ignore_missing_parent),
                                  repository)
 
 
 @cli.command(short_help="Sync the repository with openBIS.")
 @click.pass_context
 @add_params(_sync_params)
 def sync(ctx, ignore_missing_parent, repository):
+    """External Data Store: Sync the repository with openBIS."""
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.invoke(repository_sync,
                ignore_missing_parent=ignore_missing_parent, repository=repository)
 
 
 @cli.group(short_help="create/show a openBIS token")
 @click.pass_context
@@ -702,21 +776,23 @@
 ]
 
 
 @repository.command("addref", short_help="Add the given repository as a reference to openBIS.")
 @click.pass_context
 @add_params(_addref_params)
 def repository_addref(ctx, repository):
+    """Used for External Data Store only."""
     return ctx.obj['runner'].run("addref", lambda dm: dm.addref(), repository)
 
 
 @cli.command(short_help="Add the given repository as a reference to openBIS.")
 @click.pass_context
 @add_params(_addref_params)
 def addref(ctx, repository):
+    """Used for External Data Store only."""
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.invoke(repository_addref, repository=repository)
 
 
 # removeref
 
 
@@ -729,25 +805,27 @@
 
 
 @repository.command("removeref",
                     short_help="Remove the reference to the given repository from openBIS.")
 @click.pass_context
 @add_params(_removeref_params)
 def repository_removeref(ctx, data_set_id, repository):
+    """Used for External Data Store only."""
     if data_set_id is not None and repository is not None:
         click_echo("Only provide the data_set id OR the repository.")
         return -1
     return ctx.obj['runner'].run("removeref", lambda dm: dm.removeref(data_set_id=data_set_id),
                                  repository)
 
 
 @cli.command(short_help="Remove the reference to the given repository from openBIS.")
 @click.pass_context
 @add_params(_removeref_params)
 def removeref(ctx, data_set_id, repository):
+    """Used for External Data Store only."""
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.invoke(repository_removeref, data_set_id=data_set_id,
                repository=repository)
 
 
 # data set commands: download, upload, clone
```

### Comparing `obis-0.4.1/obis/scripts/click_util.py` & `obis-0.4.2rc1/obis/scripts/click_util.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/scripts/data_mgmt_runner.py` & `obis-0.4.2rc1/obis/scripts/data_mgmt_runner.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis/test-data/snb-data.zip` & `obis-0.4.2rc1/obis/test-data/snb-data.zip`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/obis.egg-info/PKG-INFO` & `obis-0.4.2rc1/obis.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.1
+Version: 0.4.2rc1
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,17 +33,20 @@
     1. [Standard Data Store](#51-standard-data-store)
         1. [Commands](#511-commands)
         2. [Examples](#512-examples)
     2. [External Data Store](#52-external-data-store)
         1. [Settings](#521-settings)
         2. [Commands](#522-commands)
         3. [Examples](#523-examples)
-6. [Big Data Link Services](#6-big-data-link-services)
-7. [Rationale for obis](#7-rationale-for-obis)
-8. [Literature](#8-literature)
+6. [Authentication](#6-authentication)
+   1. [Login](#61-login)
+   2. [Personal Access Token](#62-personal-access-token)
+7. [Big Data Link Services](#7-big-data-link-services)
+8. [Rationale for obis](#8-rationale-for-obis)
+9. [Literature](#9-literature)
 
 ## 1. Prerequisites
 
 - python 3.6 or higher
 - git 2.11 or higher
 - git-annex 6 or higher [Installation guide](https://git-annex.branchable.com/install/)
 
@@ -177,15 +180,15 @@
 | repository set   |          ❌          |          ✅          |
 | repository clear |          ❌          |          ✅          |
 | settings get     |          ❌          |          ✅          |
 | settings set     |          ❌          |          ✅          |
 | settings clear   |          ❌          |          ✅          |
 | status           |          ❌          |          ✅          |
 | sync             |          ❌          |          ✅          |
-| token            |          ❌          |          ✅          |
+| token            |          ✅          |          ✅          |
 | upload           |          ✅          |          ❌          |
 
 **Login**
 
 Some commands like `download` or `upload` will connect to OpenBIS instance. At that time, oBIS will
 use username configured in `.obis/config.json` and will ask for password whenever session expires or
 username changes.
@@ -245,30 +248,35 @@
 
 Options:
   -object_type, --object_type TEXT              
                                   Object type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
   -experiment, --experiment TEXT  Full experiment code
+  -object, --object TEXT          Object identification information, it can be permId or identifier
   -type, --type TEXT              Type code
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -property TEXT                  Property code
   -property-value TEXT            Property value
   -save, --save TEXT              Directory name to save results
+  -r, --recursive                 Search data recursively
 ```
 
 With `data_set search` command, obis connects to a configured OpenBIS instance and searches for all
-data sets that fulfill given filtering criteria.
-At least one filtering criteria must be specified. Search results can be downloaded by
-using `save` option.
+data sets that fulfill given filtering criteria or by using object identification string.
+At least one search option must be specified. 
+
+Search results can be downloaded into a file by using `save` option.
+
+Recursive option enables searching for datasets of children samples or datasets
 
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **download**
 
 ```
@@ -317,29 +325,34 @@
 obis object search [OPTIONS]
 
 Options:
   -type, --type TEXT              Type code to filter by
   -space, --space TEXT            Space code
   -project, --project TEXT        Full project identification code
   -experiment, --experiment TEXT  Full experiment 
+  -object, --object TEXT          Object identification information, it can be permId or identifier
   -registration-date, --registration-date TEXT
                                   Registration date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -modification-date, --modification-date TEXT
                                   Modification date, it can be in the format
                                   "oYYYY-MM-DD" (e.g. ">2023-01-31", "=2023-01-31", "<2023-01-31")
   -property TEXT                  Property code
   -property-value TEXT            Property value
   -save, --save TEXT              File name to save results in csv format
+  -r, --recursive                 Search data recursively
 ```
 
 With `object search` command, obis connects to a configured OpenBIS instance and searches for all
-objects/samples that fulfill given filtering criteria.
-At least one filtering criteria must be specified. Search results can be downloaded int a file by
-using `-save` option.
+objects/samples that fulfill given filtering criteria or by using object identification string.
+At least one search option must be specified. 
+
+Search results can be downloaded into a file by using `save` option.
+
+Recursive option enables searching for datasets of children samples or datasets
 
 *Note: Filtering by `-project` may not work when `Project Samples` are disabled in OpenBIS
 configuration.*
 
 **upload**
 
 ```
@@ -561,14 +574,15 @@
 ```
 
 Obis repository folders can be added or removed from openBIS. This can be useful when a repository
 was moved or copied without using the `move` or `copy` commands.
 
 **token**
 
+
 ```
 obis token get <session_name> [--validity-days] [--validity-weeks] [--validity-months]
 ```
 
 Gets or creates a new personal access token (PAT) and stores it in the obis configuration. If
 no `session_name` is provided or is not stored in the configuration, you'll be asked interactively.
 If no validity period is provided, the maximum (configured by the server) is used. If a PAT with
@@ -613,23 +627,40 @@
 cd analysis1
 obis data_set set type=UNKNOWN
 obis object set id=/DEFAULT/DEFAULT
 echo content >> example_file
 obis commit -m 'message'
 ```
 
-## 6. Big Data Link Services
+## 6. Authentication
+
+There are 2 ways to perform user authentication against OpenBIS.
+
+### 6.1. Login
+Obis, internally, stores a session token which is used to connect with OpenBIS. Whenever this token 
+is invalidated, obis will ask user to provide credentials to log into OpenBIS again.   
+
+
+### 6.2. Personal Access Token
+Session token is short-lived and its interactive generation makes it unfeasible for usage in automatic 
+scripts. An alternative way to authorize is to generate personal access token (PAT), which can be 
+configured to last for a long periods of time.
+
+PAT generation is explained in depth in `token` command section.
+
+
+## 7. Big Data Link Services
 
 The Big Data Link Services can be used to download files which are contained in an obis repository.
 The services are included in the installation folder of openBIS,
 under `servers/big_data_link_services`. For how to configure and run them, consult
 the [README.md](https://sissource.ethz.ch/sispub/openbis/blob/master/big_data_link_server/README.md)
 file.
 
-## 7. Rationale for obis
+## 8. Rationale for obis
 
 Data-provenance tracking tools like openBIS make it possible to understand and follow the research
 process. What was studied, what data was acquired and how, how was data analyzed to arrive at final
 results for publication -- this is information that is captured in openBIS. In the standard usage
 scenario, openBIS stores and manages data directly. This has the advantage that openBIS acts as a
 gatekeeper to the data, making it easy to keep backups or enforce access restrictions, etc. However,
 this way of working is not a good solution for all situations.
@@ -650,13 +681,13 @@
 
 Under the covers, `obis` takes advantage of publicly available and tested tools to manage data on
 the file system. In particular, it uses `git` and `git-annex` to track the content of a dataset.
 Using `git-annex`, even large binary artifacts can be tracked efficiently. For communication with
 openBIS, `obis` uses the openBIS API, which offers the power to register and track all metadata
 supported by openBIS.
 
-## 8. Literature
+## 9. Literature
 
 V. Korolev, A. Joshi, V. Korolev, M.A. Grasso, A. Joshi, M.A. Grasso, et al., "PROB: A tool for
 tracking provenance and reproducibility of big data experiments", Reproduce '14. HPCA 2014, vol. 11,
 pp. 264-286, 2014.
 http://ebiquity.umbc.edu/_file_directory_/papers/693.pdf
```

### Comparing `obis-0.4.1/obis.egg-info/SOURCES.txt` & `obis-0.4.2rc1/obis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obis-0.4.1/setup.py` & `obis-0.4.2rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 data_dir = os.path.join("man", "man1")
 data_files = [
     (d, [os.path.join(d, f) for f in files]) for d, folders, files in os.walk(data_dir)
 ]
 
 setup(
     name="obis",
-    version="0.4.1",
+    version="0.4.2rc1",
     description="Local data management with assistance from OpenBIS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line",
     author="ID SIS • ETH Zürich",
     author_email="openbis-support@id.ethz.ch",
     license="Apache Software License Version 2.0",
```

