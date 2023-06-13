# Comparing `tmp/robotframework-datadriver-1.7.0.tar.gz` & `tmp/robotframework-datadriver-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-datadriver-1.7.0.tar", last modified: Wed Nov 30 19:59:15 2022, max compression
+gzip compressed data, was "robotframework-datadriver-1.8.0.tar", last modified: Tue Jun 13 23:50:52 2023, max compression
```

## Comparing `robotframework-datadriver-1.7.0.tar` & `robotframework-datadriver-1.8.0.tar`

### file list

```diff
@@ -1,191 +1,194 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.261039 robotframework-datadriver-1.7.0/
--rw-r--r--   0 rener      (502) wheel        (0)      896 2022-02-11 20:38:01.000000 robotframework-datadriver-1.7.0/CONTRIBUTION.md
--rw-r--r--   0 rener      (502) wheel        (0)      554 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/COPYRIGHT.txt
--rw-r--r--   0 rener      (502) wheel        (0)    11357 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)      982 2022-03-23 19:07:37.000000 robotframework-datadriver-1.7.0/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)    47053 2022-11-30 19:59:15.260741 robotframework-datadriver-1.7.0/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)    46290 2022-11-30 19:50:41.000000 robotframework-datadriver-1.7.0/Readme.rst
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.205947 robotframework-datadriver-1.7.0/atest/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.195940 robotframework-datadriver-1.7.0/atest/.mypy_cache/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.218891 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/
--rw-r--r--   0 rener      (502) wheel        (0)        2 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/@plugins_snapshot.json
--rw-r--r--   0 rener      (502) wheel        (0)    99868 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_ast.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1505 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_ast.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    13536 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_importlib_modulespec.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1526 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_importlib_modulespec.meta.json
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.219629 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_typeshed/
--rw-r--r--   0 rener      (502) wheel        (0)    37540 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_typeshed/__init__.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1604 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_typeshed/__init__.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    12862 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/abc.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1474 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/abc.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    50191 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/array.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1538 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/array.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)   103778 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/ast.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1547 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/ast.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)   776932 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/builtins.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1587 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/builtins.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)   113431 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/codecs.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1557 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/codecs.meta.json
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.220550 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/collections/
--rw-r--r--   0 rener      (502) wheel        (0)   231870 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/collections/__init__.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1529 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/collections/__init__.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)     8178 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/genericpath.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1523 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/genericpath.meta.json
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.221831 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/
--rw-r--r--   0 rener      (502) wheel        (0)     5413 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/__init__.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1534 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/__init__.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    47296 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/abc.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1610 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/abc.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    78905 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/io.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1553 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/io.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    30440 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/mmap.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1528 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/mmap.meta.json
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.223474 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/
--rw-r--r--   0 rener      (502) wheel        (0)   212697 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/__init__.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1624 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/__init__.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    69699 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/path.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1564 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/path.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    84216 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/posix.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1519 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/posix.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    64922 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/sys.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1579 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/sys.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    98298 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/types.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1568 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/types.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)   393499 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1558 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing.meta.json
--rw-r--r--   0 rener      (502) wheel        (0)    27519 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing_extensions.data.json
--rw-r--r--   0 rener      (502) wheel        (0)     1540 2021-08-27 18:50:08.000000 robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing_extensions.meta.json
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.199665 robotframework-datadriver-1.7.0/atest/TestCases/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.224146 robotframework-datadriver-1.7.0/atest/TestCases/ConfigKeyword/
--rw-r--r--   0 rener      (502) wheel        (0)      843 2022-02-11 17:13:39.000000 robotframework-datadriver-1.7.0/atest/TestCases/ConfigKeyword/config_keyword_generate_file.robot
--rw-r--r--   0 rener      (502) wheel        (0)      543 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/ConfigKeyword/custom_reader.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.226826 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/
--rw-r--r--   0 rener      (502) wheel        (0)     1385 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes.csv
--rw-r--r--   0 rener      (502) wheel        (0)     1178 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes.robot
--rw-r--r--   0 rener      (502) wheel        (0)     1140 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.robot
--rw-r--r--   0 rener      (502) wheel        (0)    11397 2021-03-22 22:15:57.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.xlsx
--rw-r--r--   0 rener      (502) wheel        (0)      603 2020-03-01 14:44:14.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/LiteralEval.csv
--rw-r--r--   0 rener      (502) wheel        (0)      639 2021-06-23 20:06:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/LiteralEval.robot
--rw-r--r--   0 rener      (502) wheel        (0)      293 2020-09-26 18:23:34.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Types_in_dicts.csv
--rw-r--r--   0 rener      (502) wheel        (0)      269 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Types_in_dicts.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.198342 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.229627 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/
--rw-r--r--   0 rener      (502) wheel        (0)      451 2022-11-30 18:47:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/defaults.csv
--rw-r--r--   0 rener      (502) wheel        (0)     1103 2022-02-11 22:25:41.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/defaults.robot
--rw-r--r--   0 rener      (502) wheel        (0)      223 2022-11-30 18:46:42.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/generic_csv_reader.csv
--rw-r--r--   0 rener      (502) wheel        (0)      797 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/generic_csv_reader.robot
--rw-r--r--   0 rener      (502) wheel        (0)      545 2022-11-30 19:13:16.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_names.csv
--rw-r--r--   0 rener      (502) wheel        (0)     1125 2022-11-30 19:11:56.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_names.robot
--rw-r--r--   0 rener      (502) wheel        (0)      507 2022-11-30 19:39:12.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_no_names.csv
--rw-r--r--   0 rener      (502) wheel        (0)     1125 2022-11-30 19:11:56.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_no_names.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.230323 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.231283 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/DataFiles/
--rw-r--r--   0 rener      (502) wheel        (0)       33 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/DataFiles/First_File.json
--rw-r--r--   0 rener      (502) wheel        (0)       32 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/DataFiles/Last_File.json
--rw-r--r--   0 rener      (502) wheel        (0)       30 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/DataFiles/Wrong_File.NoJson
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.198022 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/FoldersToFind/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.231612 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder1/
--rw-r--r--   0 rener      (502) wheel        (0)        7 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder1/verify.txt
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.231940 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder2/
--rw-r--r--   0 rener      (502) wheel        (0)        7 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder2/verify.txt
--rw-r--r--   0 rener      (502) wheel        (0)      474 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/defaults_glob_files.robot
--rw-r--r--   0 rener      (502) wheel        (0)      438 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/GLOB/defaults_glob_folders.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.233252 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/PICT/
--rw-r--r--   0 rener      (502) wheel        (0)      152 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/PICT/defaults_pict.pict
--rw-r--r--   0 rener      (502) wheel        (0)      447 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/PICT/defaults_pict.robot
--rw-r--r--   0 rener      (502) wheel        (0)      251 2022-02-11 19:07:06.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/PICT/pict_arg.pict
--rw-r--r--   0 rener      (502) wheel        (0)      666 2022-03-23 19:11:21.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/PICT/pict_arguments.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.235430 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/
--rw-r--r--   0 rener      (502) wheel        (0)     1123 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xls.robot
--rw-r--r--   0 rener      (502) wheel        (0)    27136 2021-03-22 22:15:44.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xls.xls
--rw-r--r--   0 rener      (502) wheel        (0)     1112 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx.robot
--rw-r--r--   0 rener      (502) wheel        (0)    12379 2022-03-23 19:13:59.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx.xlsx
--rw-r--r--   0 rener      (502) wheel        (0)     1034 2022-03-23 19:11:12.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx_data_type.robot
--rw-r--r--   0 rener      (502) wheel        (0)     1175 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx_sheet_name.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.236101 robotframework-datadriver-1.7.0/atest/TestCases/Setup_Teardown/
--rw-r--r--   0 rener      (502) wheel        (0)      212 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/Setup_Teardown/Setups_Teardowns.csv
--rw-r--r--   0 rener      (502) wheel        (0)     1060 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/Setup_Teardown/Setups_Teardowns.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.236744 robotframework-datadriver-1.7.0/atest/TestCases/Some_Fail/
--rw-r--r--   0 rener      (502) wheel        (0)      200 2022-02-11 21:48:30.000000 robotframework-datadriver-1.7.0/atest/TestCases/Some_Fail/2_of_10_fail.csv
--rw-r--r--   0 rener      (502) wheel        (0)      268 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/Some_Fail/2_of_10_fail.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.237429 robotframework-datadriver-1.7.0/atest/TestCases/Tags/
--rw-r--r--   0 rener      (502) wheel        (0)      705 2022-11-30 18:22:06.000000 robotframework-datadriver-1.7.0/atest/TestCases/Tags/foo_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)      335 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/Tags/test.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.238042 robotframework-datadriver-1.7.0/atest/TestCases/Timeouts/
--rw-r--r--   0 rener      (502) wheel        (0)      439 2022-08-21 12:47:10.000000 robotframework-datadriver-1.7.0/atest/TestCases/Timeouts/timeout.csv
--rw-r--r--   0 rener      (502) wheel        (0)     1097 2022-08-21 12:51:24.000000 robotframework-datadriver-1.7.0/atest/TestCases/Timeouts/timeout.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.239352 robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/
--rw-r--r--   0 rener      (502) wheel        (0)     1379 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/reader_by_filename.robot
--rw-r--r--   0 rener      (502) wheel        (0)     1376 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/reader_by_name.robot
--rw-r--r--   0 rener      (502) wheel        (0)     1396 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/reader_by_path.robot
--rw-r--r--   0 rener      (502) wheel        (0)      669 2022-11-30 18:32:19.000000 robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/tab-csv-file-name.tsv
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.241877 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/
--rw-r--r--   0 rener      (502) wheel        (0)     1465 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/custom_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)      336 2022-11-30 19:44:25.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/custom_reader.robot
--rw-r--r--   0 rener      (502) wheel        (0)      290 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/custom_reader_local.robot
--rw-r--r--   0 rener      (502) wheel        (0)      443 2022-06-21 21:04:56.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/data.json
--rw-r--r--   0 rener      (502) wheel        (0)       63 2020-02-08 16:13:42.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/dummy.txt
--rw-r--r--   0 rener      (502) wheel        (0)      501 2020-09-27 08:41:35.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/file_search_strategy_none.robot
--rw-r--r--   0 rener      (502) wheel        (0)      291 2022-06-21 21:04:56.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/jsonreader.robot
--rw-r--r--   0 rener      (502) wheel        (0)      436 2020-09-27 08:41:35.000000 robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/with_path_and_file.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.242501 robotframework-datadriver-1.7.0/atest/TestCases/performance/
--rw-r--r--   0 rener      (502) wheel        (0)      816 2022-02-11 18:25:47.000000 robotframework-datadriver-1.7.0/atest/TestCases/performance/10.000.robot
--rw-r--r--   0 rener      (502) wheel        (0)   245597 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/atest/TestCases/performance/10000.csv
--rw-r--r--   0 rener      (502) wheel        (0)      125 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/atest/run_atest.bat
--rw-r--r--   0 rener      (502) wheel        (0)      125 2022-11-30 18:49:56.000000 robotframework-datadriver-1.7.0/atest/run_atest.sh
--rw-r--r--   0 rener      (502) wheel        (0)      175 2022-02-11 20:34:32.000000 robotframework-datadriver-1.7.0/atest/run_atest_pabot.bat
--rw-r--r--   0 rener      (502) wheel        (0)      175 2022-11-30 19:09:14.000000 robotframework-datadriver-1.7.0/atest/run_atest_pabot.sh
--rw-r--r--   0 rener      (502) wheel        (0)      236 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/create_readme.py
--rw-r--r--   0 rener      (502) wheel        (0)       86 2022-02-11 19:46:43.000000 robotframework-datadriver-1.7.0/dev-requirements.txt
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.243106 robotframework-datadriver-1.7.0/doc/
--rw-r--r--   0 rener      (502) wheel        (0)   280453 2022-11-30 19:50:40.000000 robotframework-datadriver-1.7.0/doc/DataDriver.html
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.200438 robotframework-datadriver-1.7.0/example/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.247308 robotframework-datadriver-1.7.0/example/Login Tests/
--rw-r--r--   0 rener      (502) wheel        (0)      425 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.csv
--rw-r--r--   0 rener      (502) wheel        (0)      132 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.pict
--rw-r--r--   0 rener      (502) wheel        (0)      516 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.robot
--rw-r--r--   0 rener      (502) wheel        (0)    30720 2021-06-23 18:33:56.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.xls
--rw-r--r--   0 rener      (502) wheel        (0)    13432 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.xlsx
--rw-r--r--   0 rener      (502) wheel        (0)      556 2020-03-04 18:22:33.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_pict.robot
--rw-r--r--   0 rener      (502) wheel        (0)      711 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_regex.robot
--rw-r--r--   0 rener      (502) wheel        (0)      555 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_xls.robot
--rw-r--r--   0 rener      (502) wheel        (0)      556 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_xlsx.robot
--rw-r--r--   0 rener      (502) wheel        (0)      798 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/invalidLogins.robot
--rw-r--r--   0 rener      (502) wheel        (0)      759 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/login_resources.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.248362 robotframework-datadriver-1.7.0/example/Login Tests/logs/
--rw-r--r--   0 rener      (502) wheel        (0)   233926 2021-06-23 21:06:14.000000 robotframework-datadriver-1.7.0/example/Login Tests/logs/log.html
--rw-r--r--   0 rener      (502) wheel        (0)   233026 2021-06-23 21:06:14.000000 robotframework-datadriver-1.7.0/example/Login Tests/logs/report.html
--rw-r--r--   0 rener      (502) wheel        (0)      258 2020-02-08 15:44:38.000000 robotframework-datadriver-1.7.0/example/Login Tests/validTest.robot
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.249110 robotframework-datadriver-1.7.0/example/demo_web_server/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.251947 robotframework-datadriver-1.7.0/example/demo_web_server/html/
--rw-r--r--   0 rener      (502) wheel        (0)      228 2021-12-13 20:58:25.000000 robotframework-datadriver-1.7.0/example/demo_web_server/html/demo.css
--rw-r--r--   0 rener      (502) wheel        (0)      275 2021-12-13 20:58:25.000000 robotframework-datadriver-1.7.0/example/demo_web_server/html/error.html
--rw-r--r--   0 rener      (502) wheel        (0)     1204 2021-12-13 20:58:25.000000 robotframework-datadriver-1.7.0/example/demo_web_server/html/index.html
--rw-r--r--   0 rener      (502) wheel        (0)   227843 2021-12-10 19:56:24.000000 robotframework-datadriver-1.7.0/example/demo_web_server/html/log.html
--rw-r--r--   0 rener      (502) wheel        (0)      275 2021-12-13 20:58:25.000000 robotframework-datadriver-1.7.0/example/demo_web_server/html/welcome.html
--rw-r--r--   0 rener      (502) wheel        (0)     1374 2021-12-13 20:58:25.000000 robotframework-datadriver-1.7.0/example/demo_web_server/server.py
--rw-r--r--   0 rener      (502) wheel        (0)       38 2022-11-30 19:59:15.261117 robotframework-datadriver-1.7.0/setup.cfg
--rw-r--r--   0 rener      (502) wheel        (0)     1421 2022-11-30 18:06:02.000000 robotframework-datadriver-1.7.0/setup.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.201167 robotframework-datadriver-1.7.0/src/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.258185 robotframework-datadriver-1.7.0/src/DataDriver/
--rw-r--r--   0 rener      (502) wheel        (0)     7012 2022-11-30 19:07:26.000000 robotframework-datadriver-1.7.0/src/DataDriver/AbstractReaderClass.py
--rw-r--r--   0 rener      (502) wheel        (0)    73730 2022-11-30 19:50:26.000000 robotframework-datadriver-1.7.0/src/DataDriver/DataDriver.py
--rw-r--r--   0 rener      (502) wheel        (0)     2868 2022-11-30 19:07:26.000000 robotframework-datadriver-1.7.0/src/DataDriver/ReaderConfig.py
--rw-r--r--   0 rener      (502) wheel        (0)       35 2020-06-14 22:01:10.000000 robotframework-datadriver-1.7.0/src/DataDriver/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)     1775 2021-03-12 01:16:06.000000 robotframework-datadriver-1.7.0/src/DataDriver/argument_utils.py
--rw-r--r--   0 rener      (502) wheel        (0)     2229 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/src/DataDriver/csv_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     2255 2022-11-30 18:38:34.000000 robotframework-datadriver-1.7.0/src/DataDriver/generic_csv_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     1604 2022-02-11 14:32:21.000000 robotframework-datadriver-1.7.0/src/DataDriver/glob_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     1359 2022-11-30 18:22:06.000000 robotframework-datadriver-1.7.0/src/DataDriver/json_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     2254 2022-11-30 18:22:06.000000 robotframework-datadriver-1.7.0/src/DataDriver/pict_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     2033 2022-02-11 14:32:48.000000 robotframework-datadriver-1.7.0/src/DataDriver/rerunfailed.py
--rw-r--r--   0 rener      (502) wheel        (0)     8324 2022-02-11 21:27:22.000000 robotframework-datadriver-1.7.0/src/DataDriver/search.py
--rw-r--r--   0 rener      (502) wheel        (0)     7708 2022-11-30 18:22:06.000000 robotframework-datadriver-1.7.0/src/DataDriver/utils.py
--rw-r--r--   0 rener      (502) wheel        (0)     1152 2022-02-11 14:33:18.000000 robotframework-datadriver-1.7.0/src/DataDriver/xls_reader.py
--rw-r--r--   0 rener      (502) wheel        (0)     1750 2022-03-23 19:10:54.000000 robotframework-datadriver-1.7.0/src/DataDriver/xlsx_reader.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-30 19:59:15.260219 robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/
--rwxrwxrwx   0 rener      (502) wheel        (0)    47053 2022-11-30 19:59:14.000000 robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/PKG-INFO
--rwxrwxrwx   0 rener      (502) wheel        (0)     6353 2022-11-30 19:59:15.000000 robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/SOURCES.txt
--rwxrwxrwx   0 rener      (502) wheel        (0)        1 2022-11-30 19:59:14.000000 robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/dependency_links.txt
--rwxrwxrwx   0 rener      (502) wheel        (0)       75 2022-11-30 19:59:14.000000 robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/requires.txt
--rwxrwxrwx   0 rener      (502) wheel        (0)       11 2022-11-30 19:59:14.000000 robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.260855 robotframework-datadriver-1.8.0/
+-rw-r--r--   0 rener      (502) wheel        (0)      896 2022-02-11 20:38:01.000000 robotframework-datadriver-1.8.0/CONTRIBUTION.md
+-rw-r--r--   0 rener      (502) wheel        (0)      554 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/COPYRIGHT.txt
+-rw-r--r--   0 rener      (502) wheel        (0)    11357 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)     1039 2023-06-13 23:42:59.000000 robotframework-datadriver-1.8.0/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)    47255 2023-06-13 23:50:52.260652 robotframework-datadriver-1.8.0/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)    46290 2023-06-13 23:42:45.000000 robotframework-datadriver-1.8.0/Readme.rst
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.234685 robotframework-datadriver-1.8.0/atest/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.229684 robotframework-datadriver-1.8.0/atest/.mypy_cache/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.240844 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/
+-rw-r--r--   0 rener      (502) wheel        (0)        2 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/@plugins_snapshot.json
+-rw-r--r--   0 rener      (502) wheel        (0)    99868 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_ast.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1505 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_ast.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    13536 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_importlib_modulespec.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1526 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_importlib_modulespec.meta.json
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.241190 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_typeshed/
+-rw-r--r--   0 rener      (502) wheel        (0)    37540 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_typeshed/__init__.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1604 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_typeshed/__init__.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    12862 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/abc.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1474 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/abc.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    50191 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/array.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1538 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/array.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)   103778 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/ast.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1547 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/ast.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)   776932 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/builtins.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1587 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/builtins.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)   113431 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/codecs.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1557 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/codecs.meta.json
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.241695 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/collections/
+-rw-r--r--   0 rener      (502) wheel        (0)   231870 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/collections/__init__.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1529 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/collections/__init__.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)     8178 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/genericpath.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1523 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/genericpath.meta.json
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.242373 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/
+-rw-r--r--   0 rener      (502) wheel        (0)     5413 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/__init__.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1534 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/__init__.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    47296 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/abc.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1610 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/abc.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    78905 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/io.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1553 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/io.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    30440 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/mmap.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1528 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/mmap.meta.json
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.243224 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/
+-rw-r--r--   0 rener      (502) wheel        (0)   212697 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/__init__.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1624 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/__init__.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    69699 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/path.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1564 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/path.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    84216 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/posix.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1519 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/posix.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    64922 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/sys.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1579 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/sys.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    98298 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/types.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1568 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/types.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)   393499 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1558 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing.meta.json
+-rw-r--r--   0 rener      (502) wheel        (0)    27519 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing_extensions.data.json
+-rw-r--r--   0 rener      (502) wheel        (0)     1540 2021-08-27 18:50:08.000000 robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing_extensions.meta.json
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.231655 robotframework-datadriver-1.8.0/atest/TestCases/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.243574 robotframework-datadriver-1.8.0/atest/TestCases/ConfigKeyword/
+-rw-r--r--   0 rener      (502) wheel        (0)      843 2022-02-11 17:13:39.000000 robotframework-datadriver-1.8.0/atest/TestCases/ConfigKeyword/config_keyword_generate_file.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      543 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/ConfigKeyword/custom_reader.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.244903 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/
+-rw-r--r--   0 rener      (502) wheel        (0)     1385 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes.csv
+-rw-r--r--   0 rener      (502) wheel        (0)     1178 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes.robot
+-rw-r--r--   0 rener      (502) wheel        (0)     1140 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.robot
+-rw-r--r--   0 rener      (502) wheel        (0)    11397 2021-03-22 22:15:57.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.xlsx
+-rw-r--r--   0 rener      (502) wheel        (0)      603 2020-03-01 14:44:14.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/LiteralEval.csv
+-rw-r--r--   0 rener      (502) wheel        (0)      639 2021-06-23 20:06:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/LiteralEval.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      293 2020-09-26 18:23:34.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Types_in_dicts.csv
+-rw-r--r--   0 rener      (502) wheel        (0)      269 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Types_in_dicts.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.230951 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.246162 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/
+-rw-r--r--   0 rener      (502) wheel        (0)      451 2022-11-30 18:47:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/defaults.csv
+-rw-r--r--   0 rener      (502) wheel        (0)     1103 2022-02-11 22:25:41.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/defaults.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      223 2022-11-30 18:46:42.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/generic_csv_reader.csv
+-rw-r--r--   0 rener      (502) wheel        (0)      797 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/generic_csv_reader.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      545 2022-11-30 19:13:16.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_names.csv
+-rw-r--r--   0 rener      (502) wheel        (0)     1125 2022-11-30 19:11:56.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_names.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      507 2022-11-30 19:39:12.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_no_names.csv
+-rw-r--r--   0 rener      (502) wheel        (0)     1125 2022-11-30 19:11:56.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_no_names.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.246464 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.246989 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/DataFiles/
+-rw-r--r--   0 rener      (502) wheel        (0)       33 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/DataFiles/First_File.json
+-rw-r--r--   0 rener      (502) wheel        (0)       32 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/DataFiles/Last_File.json
+-rw-r--r--   0 rener      (502) wheel        (0)       30 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/DataFiles/Wrong_File.NoJson
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.230759 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/FoldersToFind/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.247150 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder1/
+-rw-r--r--   0 rener      (502) wheel        (0)        7 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder1/verify.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.247305 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder2/
+-rw-r--r--   0 rener      (502) wheel        (0)        7 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/FoldersToFind/Folder2/verify.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      474 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/defaults_glob_files.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      438 2022-02-11 14:32:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/GLOB/defaults_glob_folders.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.247934 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/PICT/
+-rw-r--r--   0 rener      (502) wheel        (0)      152 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/PICT/defaults_pict.pict
+-rw-r--r--   0 rener      (502) wheel        (0)      447 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/PICT/defaults_pict.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      251 2022-02-11 19:07:06.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/PICT/pict_arg.pict
+-rw-r--r--   0 rener      (502) wheel        (0)      666 2022-03-23 19:11:21.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/PICT/pict_arguments.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.249050 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/
+-rw-r--r--   0 rener      (502) wheel        (0)     1123 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xls.robot
+-rw-r--r--   0 rener      (502) wheel        (0)    27136 2021-03-22 22:15:44.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xls.xls
+-rw-r--r--   0 rener      (502) wheel        (0)     1112 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx.robot
+-rw-r--r--   0 rener      (502) wheel        (0)    12379 2022-03-23 19:13:59.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx.xlsx
+-rw-r--r--   0 rener      (502) wheel        (0)     1034 2022-03-23 19:11:12.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx_data_type.robot
+-rw-r--r--   0 rener      (502) wheel        (0)     1175 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx_sheet_name.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.249396 robotframework-datadriver-1.8.0/atest/TestCases/Setup_Teardown/
+-rw-r--r--   0 rener      (502) wheel        (0)      212 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/Setup_Teardown/Setups_Teardowns.csv
+-rw-r--r--   0 rener      (502) wheel        (0)     1060 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/Setup_Teardown/Setups_Teardowns.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.249732 robotframework-datadriver-1.8.0/atest/TestCases/Some_Fail/
+-rw-r--r--   0 rener      (502) wheel        (0)      200 2022-02-11 21:48:30.000000 robotframework-datadriver-1.8.0/atest/TestCases/Some_Fail/2_of_10_fail.csv
+-rw-r--r--   0 rener      (502) wheel        (0)      268 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/Some_Fail/2_of_10_fail.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.250048 robotframework-datadriver-1.8.0/atest/TestCases/Tags/
+-rw-r--r--   0 rener      (502) wheel        (0)      705 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/atest/TestCases/Tags/foo_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)      335 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/Tags/test.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.250394 robotframework-datadriver-1.8.0/atest/TestCases/Timeouts/
+-rw-r--r--   0 rener      (502) wheel        (0)      439 2022-08-21 12:47:10.000000 robotframework-datadriver-1.8.0/atest/TestCases/Timeouts/timeout.csv
+-rw-r--r--   0 rener      (502) wheel        (0)     1097 2022-08-21 12:51:24.000000 robotframework-datadriver-1.8.0/atest/TestCases/Timeouts/timeout.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.251104 robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/
+-rw-r--r--   0 rener      (502) wheel        (0)     1379 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/reader_by_filename.robot
+-rw-r--r--   0 rener      (502) wheel        (0)     1376 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/reader_by_name.robot
+-rw-r--r--   0 rener      (502) wheel        (0)     1396 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/reader_by_path.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      669 2022-11-30 18:32:19.000000 robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/tab-csv-file-name.tsv
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.252581 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/
+-rw-r--r--   0 rener      (502) wheel        (0)     1474 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/custom_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)      336 2022-11-30 19:44:25.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/custom_reader.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      290 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/custom_reader_local.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      443 2022-06-21 21:04:56.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/data.json
+-rw-r--r--   0 rener      (502) wheel        (0)       63 2020-02-08 16:13:42.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/dummy.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      501 2020-09-27 08:41:35.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/file_search_strategy_none.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      291 2022-06-21 21:04:56.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/jsonreader.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      436 2020-09-27 08:41:35.000000 robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/with_path_and_file.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.252946 robotframework-datadriver-1.8.0/atest/TestCases/performance/
+-rw-r--r--   0 rener      (502) wheel        (0)      816 2022-02-11 18:25:47.000000 robotframework-datadriver-1.8.0/atest/TestCases/performance/10.000.robot
+-rw-r--r--   0 rener      (502) wheel        (0)   245597 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/atest/TestCases/performance/10000.csv
+-rw-r--r--   0 rener      (502) wheel        (0)      125 2022-02-11 14:33:18.000000 robotframework-datadriver-1.8.0/atest/run_atest.bat
+-rw-r--r--   0 rener      (502) wheel        (0)      125 2022-11-30 18:49:56.000000 robotframework-datadriver-1.8.0/atest/run_atest.sh
+-rw-r--r--   0 rener      (502) wheel        (0)      175 2022-02-11 20:34:32.000000 robotframework-datadriver-1.8.0/atest/run_atest_pabot.bat
+-rw-r--r--   0 rener      (502) wheel        (0)      175 2022-11-30 19:09:14.000000 robotframework-datadriver-1.8.0/atest/run_atest_pabot.sh
+-rw-r--r--   0 rener      (502) wheel        (0)      267 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/create_readme.py
+-rw-r--r--   0 rener      (502) wheel        (0)       86 2023-06-13 22:49:48.000000 robotframework-datadriver-1.8.0/dev-requirements.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.253282 robotframework-datadriver-1.8.0/doc/
+-rw-r--r--   0 rener      (502) wheel        (0)   281578 2023-06-13 23:42:45.000000 robotframework-datadriver-1.8.0/doc/DataDriver.html
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.253614 robotframework-datadriver-1.8.0/docs/
+-rw-r--r--   0 rener      (502) wheel        (0)   280453 2023-06-13 22:10:16.000000 robotframework-datadriver-1.8.0/docs/index.html
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.232227 robotframework-datadriver-1.8.0/example/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.255677 robotframework-datadriver-1.8.0/example/Login Tests/
+-rw-r--r--   0 rener      (502) wheel        (0)      425 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.csv
+-rw-r--r--   0 rener      (502) wheel        (0)      132 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.pict
+-rw-r--r--   0 rener      (502) wheel        (0)      516 2022-02-11 14:32:48.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.robot
+-rw-r--r--   0 rener      (502) wheel        (0)    30720 2021-06-23 18:33:56.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.xls
+-rw-r--r--   0 rener      (502) wheel        (0)    13432 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.xlsx
+-rw-r--r--   0 rener      (502) wheel        (0)      556 2020-03-04 18:22:33.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_pict.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      711 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_regex.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      555 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_xls.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      556 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_xlsx.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      798 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/invalidLogins.robot
+-rw-r--r--   0 rener      (502) wheel        (0)      759 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/login_resources.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.256095 robotframework-datadriver-1.8.0/example/Login Tests/logs/
+-rw-r--r--   0 rener      (502) wheel        (0)   233926 2021-06-23 21:06:14.000000 robotframework-datadriver-1.8.0/example/Login Tests/logs/log.html
+-rw-r--r--   0 rener      (502) wheel        (0)   233026 2021-06-23 21:06:14.000000 robotframework-datadriver-1.8.0/example/Login Tests/logs/report.html
+-rw-r--r--   0 rener      (502) wheel        (0)      258 2020-02-08 15:44:38.000000 robotframework-datadriver-1.8.0/example/Login Tests/validTest.robot
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.256389 robotframework-datadriver-1.8.0/example/demo_web_server/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.257238 robotframework-datadriver-1.8.0/example/demo_web_server/html/
+-rw-r--r--   0 rener      (502) wheel        (0)      228 2021-12-13 20:58:25.000000 robotframework-datadriver-1.8.0/example/demo_web_server/html/demo.css
+-rw-r--r--   0 rener      (502) wheel        (0)      275 2021-12-13 20:58:25.000000 robotframework-datadriver-1.8.0/example/demo_web_server/html/error.html
+-rw-r--r--   0 rener      (502) wheel        (0)     1204 2021-12-13 20:58:25.000000 robotframework-datadriver-1.8.0/example/demo_web_server/html/index.html
+-rw-r--r--   0 rener      (502) wheel        (0)   227843 2021-12-10 19:56:24.000000 robotframework-datadriver-1.8.0/example/demo_web_server/html/log.html
+-rw-r--r--   0 rener      (502) wheel        (0)      275 2021-12-13 20:58:25.000000 robotframework-datadriver-1.8.0/example/demo_web_server/html/welcome.html
+-rw-r--r--   0 rener      (502) wheel        (0)     1374 2021-12-13 20:58:25.000000 robotframework-datadriver-1.8.0/example/demo_web_server/server.py
+-rw-r--r--   0 rener      (502) wheel        (0)      974 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)       38 2023-06-13 23:50:52.260923 robotframework-datadriver-1.8.0/setup.cfg
+-rw-r--r--   0 rener      (502) wheel        (0)     1588 2023-06-13 23:01:52.000000 robotframework-datadriver-1.8.0/setup.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.232601 robotframework-datadriver-1.8.0/src/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.259476 robotframework-datadriver-1.8.0/src/DataDriver/
+-rw-r--r--   0 rener      (502) wheel        (0)     7020 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/AbstractReaderClass.py
+-rw-r--r--   0 rener      (502) wheel        (0)    73535 2023-06-13 22:59:11.000000 robotframework-datadriver-1.8.0/src/DataDriver/DataDriver.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2870 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/ReaderConfig.py
+-rw-r--r--   0 rener      (502) wheel        (0)       49 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1829 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/argument_utils.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2255 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/csv_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2281 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/generic_csv_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1545 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/glob_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1385 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/json_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2280 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/pict_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     2046 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/rerunfailed.py
+-rw-r--r--   0 rener      (502) wheel        (0)     8294 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/search.py
+-rw-r--r--   0 rener      (502) wheel        (0)     7703 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/utils.py
+-rw-r--r--   0 rener      (502) wheel        (0)      836 2023-06-13 22:52:07.000000 robotframework-datadriver-1.8.0/src/DataDriver/xls_reader.py
+-rw-r--r--   0 rener      (502) wheel        (0)     1798 2023-06-13 23:31:43.000000 robotframework-datadriver-1.8.0/src/DataDriver/xlsx_reader.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-06-13 23:50:52.260335 robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/
+-rwxrwxrwx   0 rener      (502) wheel        (0)    47255 2023-06-13 23:50:52.000000 robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/PKG-INFO
+-rwxrwxrwx   0 rener      (502) wheel        (0)     6384 2023-06-13 23:50:52.000000 robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rener      (502) wheel        (0)        1 2023-06-13 23:50:52.000000 robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rener      (502) wheel        (0)       75 2023-06-13 23:50:52.000000 robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/requires.txt
+-rwxrwxrwx   0 rener      (502) wheel        (0)       11 2023-06-13 23:50:52.000000 robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/top_level.txt
```

### Comparing `robotframework-datadriver-1.7.0/CONTRIBUTION.md` & `robotframework-datadriver-1.8.0/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/COPYRIGHT.txt` & `robotframework-datadriver-1.8.0/COPYRIGHT.txt`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/LICENSE` & `robotframework-datadriver-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/MANIFEST.in` & `robotframework-datadriver-1.8.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -35,7 +35,10 @@
 
 # added by check-manifest
 recursive-include atest *.NoJson
 recursive-include atest *.json
 
 # added by check-manifest
 include *.md
+
+# added by check-manifest
+recursive-include docs *.html
```

### Comparing `robotframework-datadriver-1.7.0/PKG-INFO` & `robotframework-datadriver-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: robotframework-datadriver
-Version: 1.7.0
+Version: 1.8.0
 Summary: A library for Data-Driven Testing.
 Home-page: https://github.com/Snooz82/robotframework-datadriver
 Author: René Rohner(Snooz82)
 Author-email: snooz@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Framework :: Robot Framework
-Requires-Python: >=3.6.15
+Requires-Python: >=3.7.12
 Description-Content-Type: text/x-rst
 Provides-Extra: xls
 License-File: LICENSE
 
 ===================================================
 DataDriver for Robot Framework®
 ===================================================
```

### Comparing `robotframework-datadriver-1.7.0/Readme.rst` & `robotframework-datadriver-1.8.0/Readme.rst`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_ast.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_ast.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_ast.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_importlib_modulespec.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_importlib_modulespec.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_importlib_modulespec.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_importlib_modulespec.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_typeshed/__init__.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/_typeshed/__init__.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/abc.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/abc.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/abc.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/abc.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/array.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/array.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/array.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/array.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/ast.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/ast.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/ast.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/ast.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/builtins.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/builtins.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/builtins.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/codecs.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/codecs.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/codecs.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/collections/__init__.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/collections/__init__.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/genericpath.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/genericpath.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/__init__.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/__init__.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/abc.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/importlib/abc.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/io.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/io.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/io.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/io.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/mmap.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/mmap.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/mmap.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/__init__.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/__init__.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/path.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/path.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/os/path.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/posix.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/posix.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/posix.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/posix.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/sys.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/sys.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/sys.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/sys.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/types.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/types.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/types.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/types.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing_extensions.data.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/.mypy_cache/3.9/typing_extensions.meta.json` & `robotframework-datadriver-1.8.0/atest/.mypy_cache/3.9/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/ConfigKeyword/config_keyword_generate_file.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/ConfigKeyword/config_keyword_generate_file.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/ConfigKeyword/custom_reader.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/ConfigKeyword/custom_reader.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes.csv` & `robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes.csv`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.xlsx` & `robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/Check_DataTypes_xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/LiteralEval.csv` & `robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/LiteralEval.csv`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/DataTypes/LiteralEval.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/DataTypes/LiteralEval.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/defaults.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/defaults.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/generic_csv_reader.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/generic_csv_reader.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_names.csv` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_names.csv`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_names.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_names.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/CSV/test_case_no_names.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/CSV/test_case_no_names.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/PICT/pict_arguments.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/PICT/pict_arguments.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xls.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xls.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xls.xls` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xls.xls`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx.xlsx` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx_data_type.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx_data_type.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Defaults/XLS/defaults_xlsx_sheet_name.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Defaults/XLS/defaults_xlsx_sheet_name.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Setup_Teardown/Setups_Teardowns.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Setup_Teardown/Setups_Teardowns.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Tags/foo_reader.py` & `robotframework-datadriver-1.8.0/atest/TestCases/Tags/foo_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     def get_data_from_source(self):
         return self._read_file_to_data_table()
 
     def _read_file_to_data_table(self):
         test_data = []
         flipflop = True
         for i in range(6):
-            args = {'${fooarg}': i}
+            args = {"${fooarg}": i}
             tags = ["included"]
             if flipflop:
                 tags = ["filtered"]
                 flipflop = False
             else:
                 flipflop = True
             if i == 3:
```

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/Timeouts/timeout.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/Timeouts/timeout.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/reader_by_filename.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/reader_by_filename.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/reader_by_name.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/reader_by_name.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/reader_by_path.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/reader_by_path.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/csv_reader_config/tab-csv-file-name.tsv` & `robotframework-datadriver-1.8.0/atest/TestCases/csv_reader_config/tab-csv-file-name.tsv`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/custom_reader/custom_reader.py` & `robotframework-datadriver-1.8.0/atest/TestCases/custom_reader/custom_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from DataDriver.AbstractReaderClass import (
     AbstractReaderClass,
 )  # inherit class from AbstractReaderClass
-from DataDriver.ReaderConfig import TestCaseData  # return list of TestCaseData to DataDriver
+from DataDriver.ReaderConfig import (
+    TestCaseData,
+)  # return list of TestCaseData to DataDriver
 
 
 class custom_reader(AbstractReaderClass):
 
     # This method will be called from DataDriver to get the TestCaseData list.
     def get_data_from_source(self):
         test_data = []
```

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/performance/10.000.robot` & `robotframework-datadriver-1.8.0/atest/TestCases/performance/10.000.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/atest/TestCases/performance/10000.csv` & `robotframework-datadriver-1.8.0/atest/TestCases/performance/10000.csv`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/doc/DataDriver.html` & `robotframework-datadriver-1.8.0/docs/index.html`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.xls` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.xls`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven.xlsx` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven.xlsx`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_pict.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_pict.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_regex.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_regex.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_xls.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_xls.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/DataDriven_xlsx.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/DataDriven_xlsx.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/invalidLogins.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/invalidLogins.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/login_resources.robot` & `robotframework-datadriver-1.8.0/example/Login Tests/login_resources.robot`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/logs/log.html` & `robotframework-datadriver-1.8.0/example/Login Tests/logs/log.html`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/Login Tests/logs/report.html` & `robotframework-datadriver-1.8.0/example/Login Tests/logs/report.html`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/demo_web_server/html/index.html` & `robotframework-datadriver-1.8.0/example/demo_web_server/html/index.html`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/demo_web_server/html/log.html` & `robotframework-datadriver-1.8.0/example/demo_web_server/html/log.html`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/example/demo_web_server/server.py` & `robotframework-datadriver-1.8.0/example/demo_web_server/server.py`

 * *Files identical despite different names*

### Comparing `robotframework-datadriver-1.7.0/setup.py` & `robotframework-datadriver-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup
 from setuptools import find_packages
 import re
-from os.path import abspath, dirname, join
+from pathlib import Path
 
-CURDIR = dirname(abspath(__file__))
 
-with open("Readme.rst", "r", encoding="utf-8") as fh:
+with Path("Readme.rst").open(encoding="utf-8") as fh:
     long_description = fh.read()
 
-with open(join(CURDIR, "src", "DataDriver", "DataDriver.py"), encoding="utf-8") as f:
+with (Path(__file__).resolve().parent / "src" / "DataDriver" / "DataDriver.py").open(encoding="utf-8") as f:
     VERSION = re.search('\n__version__ = "(.*)"', f.read()).group(1)
 
 setup(
     name="robotframework-datadriver",
     version=VERSION,
     author="René Rohner(Snooz82)",
     author_email="snooz@posteo.de",
@@ -22,17 +21,21 @@
     url="https://github.com/Snooz82/robotframework-datadriver",
     package_dir={"": "src"},
     packages=find_packages("src"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Testing :: Acceptance",
         "Framework :: Robot Framework",
     ],
     install_requires=["robotframework >= 4.0.2", "docutils", "Pygments"],
     extras_require={"xls": ["pandas", "xlrd >= 1.2.0", "openpyxl"]},
-    python_requires=">=3.6.15",
+    python_requires=">=3.7.12",
 )
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/AbstractReaderClass.py` & `robotframework-datadriver-1.8.0/src/DataDriver/AbstractReaderClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import ABC
+from abc import ABC, abstractmethod
 from re import compile
 from typing import List
 
-from .ReaderConfig import ReaderConfig
-from .ReaderConfig import TestCaseData
-from .search import search_variable
-
 from robot.libraries.BuiltIn import BuiltIn  # type: ignore
 from robot.utils import DotDict  # type: ignore
 
+from .ReaderConfig import ReaderConfig, TestCaseData
+from .search import search_variable
 
 built_in = BuiltIn()
 
 
 class AbstractReaderClass(ABC):
     def __init__(self, reader_config: ReaderConfig):
 
@@ -44,32 +42,31 @@
         self.list_separator = reader_config.list_separator
         self.handle_template_tags = reader_config.handle_template_tags
         self.kwargs = reader_config.kwargs
         for key, value in reader_config.kwargs.items():
             setattr(self, key, value)
 
         self.test_case_column_id = None
-        self.arguments_column_ids: List = list()
+        self.arguments_column_ids: List = []
         self.tags_column_id = None
         self.documentation_column_id = None
-        self.header: List = list()
-        self.data_table: List = list()
+        self.header: List = []
+        self.data_table: List[TestCaseData] = []
 
         self.TESTCASE_TABLE_NAME = ReaderConfig.TEST_CASE_TABLE_NAME
         self.TEST_CASE_TABLE_PATTERN = compile(r"(?i)^(\*+\s*test ?cases?[\s*].*)")
         self.TASK_TABLE_PATTERN = compile(r"(?i)^(\*+\s*tasks?[\s*].*)")
         self.VARIABLE_PATTERN = compile(r"([$@&e]\{)(.*?)(\})")
         self.TAGS_PATTERN = compile(r"(?i)(\[)(tags)(\])")
         self.DOCUMENTATION_PATTERN = compile(r"(?i)(\[)(documentation)(\])")
         self.LIT_EVAL_PATTERN = compile(r"e\{(.+)\}")
 
-    def get_data_from_source(self):
-        raise NotImplementedError(
-            "This method should be implemented and return self.data_table to DataDriver..."
-        )
+    @abstractmethod
+    def get_data_from_source(self) -> List[TestCaseData]:
+        """This method must be implemented and return self.data_table ( a List[TestCaseData] )."""
 
     def _is_test_case_header(self, header_string: str):
         return self.TEST_CASE_TABLE_PATTERN.fullmatch(
             header_string
         ) or self.TASK_TABLE_PATTERN.fullmatch(header_string)
 
     def _is_variable(self, header_string: str):
@@ -80,22 +77,22 @@
 
     def _is_documentation(self, header_string: str):
         return self.DOCUMENTATION_PATTERN.match(header_string)
 
     def _analyse_header(self, header_cells):
         self.header = header_cells
         for cell_index, cell in enumerate(self.header):
-            cell = cell.strip()
-            if self._is_test_case_header(cell):
+            naked_cell = cell.strip()
+            if self._is_test_case_header(naked_cell):
                 self.test_case_column_id = cell_index
-            elif self._is_variable(cell):
+            elif self._is_variable(naked_cell):
                 self.arguments_column_ids.append(cell_index)
-            elif self._is_tags(cell):
+            elif self._is_tags(naked_cell):
                 self.tags_column_id = cell_index
-            elif self._is_documentation(cell):
+            elif self._is_documentation(naked_cell):
                 self.documentation_column_id = cell_index
 
     def _read_data_from_table(self, row):
         test_case_name = (
             row[self.test_case_column_id] if self.test_case_column_id is not None else ""
         )
         arguments = {}
@@ -153,12 +150,11 @@
             for key in items:
                 if key != items[-1]:
                     if key not in selected_key or not isinstance(selected_key[key], DotDict):
                         selected_key[key] = built_in.create_dictionary()
                     selected_key = selected_key[key]
             selected_key[items[-1]] = built_in.replace_variables(value)
             return argument
-        else:
-            raise TypeError(f"{self._as_var(base)} is defined with a wrong type. Not defaultdict.")
+        raise TypeError(f"{self._as_var(base)} is defined with a wrong type. Not defaultdict.")
 
     def _as_var(self, base):
         return f"${{{base}}}"
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/DataDriver.py` & `robotframework-datadriver-1.8.0/src/DataDriver/DataDriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,49 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
 import inspect
-import os
-import os.path
 import re
 import traceback
 from glob import glob
+from pathlib import Path
+from typing import Any, Optional, Union  # type: ignore
 
 from robot.api.logger import console  # type: ignore
 from robot.libraries.BuiltIn import BuiltIn  # type: ignore
+from robot.model.tags import Tags  # type: ignore
 from robot.model.testsuite import TestSuite  # type: ignore
 from robot.running.model import TestCase  # type: ignore
-from robot.model.tags import Tags  # type: ignore
 from robot.utils.dotdict import DotDict  # type: ignore
 from robot.utils.importer import Importer  # type: ignore
-from typing import Optional, Union, Any  # type: ignore
 
 from .AbstractReaderClass import AbstractReaderClass  # type: ignore
-from .ReaderConfig import ReaderConfig  # type: ignore
-from .ReaderConfig import TestCaseData  # type: ignore
 from .argument_utils import robot_options  # type: ignore
+from .ReaderConfig import (
+    ReaderConfig,  # type: ignore
+    TestCaseData,  # type: ignore
+)
 from .utils import (  # type: ignore
+    Encodings,
     PabotOpt,
-    is_same_keyword,
+    TagHandling,
+    binary_partition_test_list,
+    debug,
+    equally_partition_test_list,
+    error,
     get_filter_dynamic_test_names,
     get_variable_value,
     is_pabot_dry_run,
-    debug,
+    is_same_keyword,
     warn,
-    error,
-    equally_partition_test_list,
-    binary_partition_test_list,
-    Encodings,
-    TagHandling,
 )
 
-__version__ = "1.7.0"
+__version__ = "1.8.0"
 
 
 class DataDriver:
     # region: docstring
     """
 
     ===================================================
@@ -1469,16 +1470,16 @@
             re.compile(file_regex)
         except re.error as e:
             file_regex = r"(?i)(.*?)(\.csv)"
             console(f"[ DataDriver ] invalid Regex! used {file_regex} instead.")
             console(e)
 
         self.robot_options = robot_options()
-        self.include = self.robot_options["include"] if not include else include
-        self.exclude = self.robot_options["exclude"] if not exclude else exclude
+        self.include = include if include else self.robot_options["include"]
+        self.exclude = exclude if exclude else self.robot_options["exclude"]
         self.handle_template_tags = handle_template_tags
         encoding_str = encoding.name if isinstance(encoding, Encodings) else str(encoding)
 
         self.config_dict = DotDict(
             file=file,
             encoding=encoding_str,
             dialect=dialect,
@@ -1536,30 +1537,30 @@
                 suite.tests.extend(test_list)
             self._set_date_table_to_robot_variable()
             debug(f"[ DataDriver ] {len(test_list)} tests added.")
         except Exception as exception:
             error(f'[ DataDriver ] Error in robot file:\n  File "{suite.source}", line 0')
             if self.reader_config.file:
                 error(
-                    f'In source file:\n'
+                    f"In source file:\n"
                     f'  File "{self.reader_config.file}", line {exception.row if hasattr(exception, "row") else "0"}'  # type: ignore
                 )
             debug(traceback.format_exc())
             raise exception
 
     def _start_test(self, test: TestCase, *_):
         BuiltIn().set_test_variable(
-            '${DataDriver_TEST_DATA}',
+            "${DataDriver_TEST_DATA}",
             self.data_table_dict.get(test.name, {"ERROR": "Test Case not found..."}),
         )
 
     def _set_date_table_to_robot_variable(self):
-        BuiltIn().set_suite_variable('${DataDriver_DATA_LIST}', self.data_table)
+        BuiltIn().set_suite_variable("${DataDriver_DATA_LIST}", self.data_table)
         self.data_table_dict = DotDict([(item.test_case_name, item) for item in self.data_table])
-        BuiltIn().set_suite_variable('${DataDriver_DATA_DICT}', self.data_table_dict)
+        BuiltIn().set_suite_variable("${DataDriver_DATA_DICT}", self.data_table_dict)
 
     def _get_all_tags(self):
         all_tags = set()
         for test_data in self.data_table:
             all_tags.update(test_data.tags or [])
         return all_tags
 
@@ -1574,18 +1575,18 @@
     def _update_config(self):
         if self.config_dict.config_keyword:
             config = self.config_dict
             config_update = BuiltIn().run_keyword(self.config_dict.config_keyword, config)
             self.reader_config = ReaderConfig(**{**config, **config_update})
 
     def _get_filtered_test_list(self):
-        temp_test_list = list()
-        temp_data_table = list()
+        temp_test_list = []
+        temp_data_table = []
         dynamic_test_list = get_filter_dynamic_test_names()
-        for index, self.test_case_data in enumerate(self.data_table):
+        for self.test_case_data in self.data_table:  # noqa: B020
             if self._included_by_tags() and self._not_excluded_by_tags():
                 self._create_test_from_template()
                 if (
                     dynamic_test_list is None
                     or f"{self.test.parent.name}.{self.test.name}" in dynamic_test_list
                     or self.test.longname in dynamic_test_list
                 ):
@@ -1635,51 +1636,47 @@
             self.reader_config.reader_class = self._get_data_reader_from_reader_class()
         reader_instance = self.reader_config.reader_class(self.reader_config)
         if not isinstance(reader_instance, AbstractReaderClass):
             raise ImportError(f"{reader_class} in no instance of AbstractDataReader!")
         return reader_instance
 
     def _get_data_reader_from_file_extension(self):
-        file_extension = os.path.splitext(self.reader_config.file)[1]
-        reader_type = file_extension.lower()[1:]
+        reader_type = Path(self.reader_config.file).suffix.lower()[1:]
         debug(f"[ DataDriver ] Initialized in {reader_type}-mode.")
         reader_module = importlib.import_module(f"..{reader_type}_reader", "DataDriver.DataDriver")
         debug(f"[ DataDriver ] Reader Module: {reader_module}")
-        reader_class = getattr(reader_module, f"{reader_type}_reader")
-        return reader_class
+        return getattr(reader_module, f"{reader_type}_reader")
 
     def _get_data_reader_from_reader_class(self):
-        reader_name = self.reader_config.reader_class
+        reader_name = Path(self.reader_config.reader_class)
         debug(f"[ DataDriver ] Initializes  {reader_name}")
-        if os.path.isfile(reader_name):
+        if reader_name.is_file():
             reader_class = self._get_reader_class_from_path(reader_name)
         else:
-            local_file = os.path.join(os.path.split(os.path.realpath(__file__))[0], reader_name)
-            relative_file = os.path.join(
-                os.path.realpath(os.path.split(self.suite_source)[0]), reader_name
-            )
-            if os.path.isfile(local_file):
+            local_file = Path(__file__).resolve().parent / reader_name
+            relative_file = Path(self.suite_source).resolve().parent / reader_name
+            if local_file.is_file():
                 reader_class = self._get_reader_class_from_path(local_file)
-            elif os.path.isfile(relative_file):
+            elif relative_file.is_file():
                 reader_class = self._get_reader_class_from_path(relative_file)
             else:
                 try:
                     reader_class = self._get_reader_class_from_module(reader_name)
                 except Exception:
                     reader_module = importlib.import_module(
                         f"..{reader_name}", "DataDriver.DataDriver"
                     )
-                    reader_class = getattr(reader_module, reader_name)
+                    reader_class = getattr(reader_module, str(reader_name))
         debug(f"[ DataDriver ] Reader Class: {reader_class}")
         return reader_class
 
     @staticmethod
-    def _get_reader_class_from_path(file_name):
+    def _get_reader_class_from_path(file_name: Path):
         debug(f"[ DataDriver ] Loading Reader from file {file_name}")
-        abs_path = os.path.abspath(file_name)
+        abs_path = str(file_name.resolve())
         importer = Importer("DataReader")
         debug(f"[ DataDriver ] Reader path: {abs_path}")
         reader = importer.import_class_or_module_by_path(abs_path)
         if not inspect.isclass(reader):
             message = f"Importing custom DataReader class from {abs_path} failed."
             raise ImportError(message)
         return reader
@@ -1691,111 +1688,112 @@
         reader = importer.import_class_or_module(reader_name)
         if not inspect.isclass(reader):
             message = f"Importing custom DataReader class {reader_name} failed."
             raise ImportError(message)
         return reader
 
     def _resolve_file_attribute(self) -> None:
+        configured_file = (
+            str(self.reader_config.file) if self.reader_config.file else self.reader_config.file
+        )
         if self.reader_config.file_search_strategy == "PATH":
-            if self.reader_config.reader_class and not self.reader_config.file:
+            if self.reader_config.reader_class and not configured_file:
                 return
             if self._check_valid_glob():
                 return
-            if (not self.reader_config.file) or (
-                "" == self.reader_config.file[: self.reader_config.file.rfind(".")]
-            ):
+            if (not configured_file) or (not configured_file[: configured_file.rfind(".")]):
                 self._set_data_file_to_suite_source()
             else:
                 self._check_if_file_exists_as_path_or_in_suite()
         elif self.reader_config.file_search_strategy == "REGEX":
             self._search_file_from_regex()
         elif self.reader_config.file_search_strategy == "NONE":
             pass  # If file_search_strategy is None, no validation of the input file is done. Use i.e. for SQL sources.
         else:
             raise ValueError(
                 f"file_search_strategy={self.reader_config.file_search_strategy} is not a valid value!"
             )
 
     def _set_data_file_to_suite_source(self):
+        suite_source = Path(self.suite_source)
         if not self.reader_config.file:
-            suite_path_as_data_file = f"{self.suite_source[:self.suite_source.rfind('.')]}.csv"
+            suite_path_as_data_file = suite_source.parent / f"{suite_source.stem}.csv"
         else:
-            suite_path = self.suite_source[: self.suite_source.rfind(".")]
             file_extension = self.reader_config.file[self.reader_config.file.rfind(".") :]
-            suite_path_as_data_file = f"{suite_path}{file_extension}"
-        if os.path.isfile(suite_path_as_data_file):
-            self.reader_config.file = suite_path_as_data_file
+            suite_path_as_data_file = suite_source.parent / f"{suite_source.stem}{file_extension}"
+        if suite_path_as_data_file.is_file():
+            self.reader_config.file = str(suite_path_as_data_file)
         else:
             raise FileNotFoundError(
                 f"File attribute was empty. "
                 f"Tried to find {suite_path_as_data_file} but file does not exist. "
                 f"If no file validation is required, set file_search_strategy=None."
             )
 
     def _check_if_file_exists_as_path_or_in_suite(self):
-        if not os.path.isfile(self.reader_config.file):
-            suite_dir = str(os.path.dirname(self.suite_source))
-            file_in_suite_dir = os.path.join(suite_dir, self.reader_config.file)
-            if os.path.isfile(file_in_suite_dir):
-                self.reader_config.file = file_in_suite_dir
+        if not Path(self.reader_config.file).is_file():
+            file_in_suite_dir = Path(self.suite_source).parent / self.reader_config.file
+            if file_in_suite_dir.is_file():
+                self.reader_config.file = str(file_in_suite_dir)
             else:
                 raise FileNotFoundError(
                     f"File attribute was not a full path. Tried to find {file_in_suite_dir} but file does not exist."
                 )
 
     def _check_valid_glob(self):
-        if not self.reader_config.reader_class == "glob_reader":
-            return
+        if self.reader_config.reader_class != "glob_reader":
+            return None
         if not glob(self.reader_config.file):
             raise FileNotFoundError(
                 f"Glob pattern did not find a file or folder. Glob pattern was: {self.reader_config.file}"
             )
         return True
 
     def _search_file_from_regex(self):
-        if os.path.isdir(self.reader_config.file):
-            for filename in os.listdir(self.reader_config.file):
-                if re.match(self.reader_config.file_regex, filename):
-                    self.reader_config.file = os.path.join(self.reader_config.file, filename)
+        file = Path(self.reader_config.file)
+        if file.is_dir():
+            for filename in Path(".").iterdir():
+                if re.match(self.reader_config.file_regex, str(filename)):
+                    self.reader_config.file = str(file / filename)
                     break
 
     def _handle_pabot(self, test_list):
         if (
             get_variable_value("${DYNAMICTEST}")
             or get_variable_value("${DYNAMICTESTS}")
             or not self.robot_options["test"]
             or not get_variable_value("${PABOTQUEUEINDEX}")
         ):
-            return
+            return None
         pabot_process_count = int(get_variable_value("${PABOTNUMBEROFPROCESSES}"))
         if not pabot_process_count:
             warn(
                 "You are using an incompatible version of Pabot! "
                 " '--testlevelsplit' is not supported between Pabot 1.2.1 and 1.10.1 with DataDriver"
             )
-            return
+            return None
         try:
             from pabot.pabotlib import Remote  # type: ignore
         except ImportError as e:
             debug(e)
-            return
+            return None
         pabotlib_url = get_variable_value("${PABOTLIBURI}")
         try:
             pabotlib = Remote(pabotlib_url)
             if not pabotlib:
                 raise ConnectionError
             self._create_pabot_queue(pabot_process_count, pabotlib, test_list)
         except (RuntimeError, ConnectionError) as e:
             error(e)
             error(
                 f"Unable to connect to PabotLib via '{pabotlib_url}'! "
                 f"Is PabotLib in use? Try 'pabot --pabotlib'"
             )
             error("Execution as been processes without --testlevelsplit")
-            return
+            return None
         pabotlib.run_keyword("ignore_execution", [get_variable_value("${CALLER_ID}")], {})
         return True
 
     def _create_pabot_queue(self, pabot_process_count, pabotlib, test_list):
         pabot_opt = self.reader_config.optimize_pabot
         if pabot_opt == PabotOpt.Atomic:
             self._add_test_to_pabot_queue(pabotlib, test_list)
@@ -1805,16 +1803,16 @@
             else:
                 partitioner = equally_partition_test_list
             for process_test_list in partitioner(test_list, pabot_process_count):
                 self._add_test_list_to_pabot_queue(pabotlib, process_test_list)
 
     def _add_test_list_to_pabot_queue(self, pabotlib, test_list):
         test_names = [f"{self.suite_name}.{test.name}" for test in test_list]
-        pabot_string = '|'.join(
-            [name.replace('\\', '\\\\').replace('|', '\\|') for name in test_names]
+        pabot_string = "|".join(
+            [name.replace("\\", "\\\\").replace("|", "\\|") for name in test_names]
         )
         pabotlib.run_keyword(
             "add_suite_to_execution_queue",
             [self.suite_name, [f"DYNAMICTESTS:{pabot_string}"]],
             {},
         )
 
@@ -1846,15 +1844,15 @@
         self.test.parent = self.template_test.parent
         self._replace_test_case_name()
         self._replace_test_case_keywords()
         self._add_test_case_tags()
         self._replace_test_case_doc()
 
     def _replace_test_case_name(self):
-        if self.test_case_data.test_case_name == "":
+        if not self.test_case_data.test_case_name:
             for variable_name in self.test_case_data.arguments:
                 self.test.name = self.test.name.replace(
                     variable_name, str(self.test_case_data.arguments[variable_name])
                 )
             self.test_case_data.test_case_name = self.test.name
         else:
             self.test.name = self.test_case_data.test_case_name
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/ReaderConfig.py` & `robotframework-datadriver-1.8.0/src/DataDriver/ReaderConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional, Any, Dict, List
+
+from typing import Any, Dict, List, Optional
 
 from robot.utils import DotDict  # type: ignore
 
 from .utils import PabotOpt, TagHandling
 
 
 class ReaderConfig:
@@ -40,15 +41,15 @@
         file_regex: Optional[str] = None,
         include: Optional[str] = None,
         exclude: Optional[str] = None,
         handle_template_tags: TagHandling = TagHandling.UnsetTags,
         list_separator: Optional[str] = ",",
         config_keyword: Optional[str] = None,
         optimize_pabot: PabotOpt = PabotOpt.Equal,
-        **kwargs
+        **kwargs,
     ):
 
         self.file = file
         self.encoding = encoding
         self.dialect = dialect
         self.delimiter = delimiter
         self.quotechar = quotechar
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/argument_utils.py` & `robotframework-datadriver-1.8.0/src/DataDriver/argument_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import sys
-
 from enum import IntEnum
 
 from robot.run import USAGE  # type: ignore
 from robot.utils.argumentparser import ArgumentParser  # type: ignore
 
 SINGLE_ARG_CHARACTERS = ".?hTX"
 
@@ -12,25 +11,28 @@
     ANALYZE_NEXT = 0
     ONE_KNOWN = 1
     TWO_KNOWN = 2
 
 
 def robot_options():
     arg_parser = ArgumentParser(
-        USAGE, auto_pythonpath=False, auto_argumentfile=True, env_options="ROBOT_OPTIONS"
+        USAGE,
+        auto_pythonpath=False,
+        auto_argumentfile=True,
+        env_options="ROBOT_OPTIONS",
     )
     valid_args = filter_args(arg_parser)
     return arg_parser.parse_args(valid_args)[0]
 
 
 def filter_args(arg_parser):
     short_opts = arg_parser._short_opts
     long_opts = arg_parser._long_opts
     arg_state = ArgumentState.ANALYZE_NEXT
-    valid_robot_args = list()
+    valid_robot_args = []
     for arg in sys.argv[1:]:
         if arg_state == ArgumentState.ANALYZE_NEXT:
             arg_state = get_argument_state(arg, short_opts, long_opts)
         if arg_state >= ArgumentState.ONE_KNOWN:
             valid_robot_args.append(arg)
             arg_state -= 1
     return valid_robot_args
@@ -49,16 +51,16 @@
             arg_state = ArgumentState.TWO_KNOWN
         elif arg[2:] in long_opts:
             arg_state = ArgumentState.ONE_KNOWN
     return arg_state
 
 
 def is_short_option(arg):
-    return len(arg) == 2 and arg[0] == "-"
+    return len(arg) == 2 and arg[0] == "-"  # noqa: PLR2004
 
 
 def is_long_option(arg):
-    return len(arg) > 2 and arg[:2] == "--"
+    return len(arg) > 2 and arg[:2] == "--"  # noqa: PLR2004
 
 
 def is_pabot_testlevelsplit():
     return "--testlevelsplit" in sys.argv
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/csv_reader.py` & `robotframework-datadriver-1.8.0/src/DataDriver/csv_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import csv
+from pathlib import Path
+
 from DataDriver.AbstractReaderClass import AbstractReaderClass
 
 
 class csv_reader(AbstractReaderClass):
     def get_data_from_source(self):
         self._register_dialects()
         self._read_file_to_data_table()
@@ -44,15 +46,15 @@
                 doublequote=True,
                 skipinitialspace=False,
                 lineterminator="\r\n",
                 quoting=csv.QUOTE_ALL,
             )
 
     def _read_file_to_data_table(self):
-        with open(self.file, "r", encoding=self.csv_encoding) as csvfile:
+        with Path(self.file).open(encoding=self.csv_encoding) as csvfile:
             reader = csv.reader(csvfile, self.csv_dialect)
             for row_index, row in enumerate(reader):
                 try:
                     if row_index == 0:
                         self._analyse_header(row)
                     else:
                         self._read_data_from_table(row)
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/generic_csv_reader.py` & `robotframework-datadriver-1.8.0/src/DataDriver/generic_csv_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import csv
+from pathlib import Path
+
 from DataDriver.AbstractReaderClass import AbstractReaderClass
 
 
 class generic_csv_reader(AbstractReaderClass):
     def get_data_from_source(self):
         self._register_dialects()
         self._read_file_to_data_table()
@@ -44,15 +46,15 @@
                 doublequote=True,
                 skipinitialspace=False,
                 lineterminator="\r\n",
                 quoting=csv.QUOTE_ALL,
             )
 
     def _read_file_to_data_table(self):
-        with open(self.file, "r", encoding=self.csv_encoding) as csvfile:
+        with Path(self.file).open(encoding=self.csv_encoding) as csvfile:
             reader = csv.reader(csvfile, self.csv_dialect)
             for row_index, row in enumerate(reader):
                 if row_index == 0:
                     row_of_variables = []
                     for cell in row:
                         row_of_variables.append(f"${{{cell.strip()}}}")
                     self._analyse_header(row_of_variables)
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/glob_reader.py` & `robotframework-datadriver-1.8.0/src/DataDriver/pict_reader.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,64 @@
-# Copyright 2021-  René Rohner
+# Copyright 2018-  René Rohner
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#
-# This Reader has initialy been created by Samual Montgomery-Blinn (https://github.com/montsamu)
-# Thanks for this contribution
 
 
-from os.path import normpath, basename, splitext, abspath, isfile, isdir
-from glob import glob
+import csv
+import os
+import time
+from pathlib import Path
+
+from DataDriver.utils import debug
+
+from .AbstractReaderClass import AbstractReaderClass, ReaderConfig
 
-from DataDriver.AbstractReaderClass import AbstractReaderClass
 
+class pict_reader(AbstractReaderClass):
+    def __init__(self, reader_config: ReaderConfig):
+        super().__init__(reader_config)
+        file = self.file or ""
+        self.pictout_file = f"{Path(file).stem}{time.monotonic()}.pictout"
 
-class glob_reader(AbstractReaderClass):
     def get_data_from_source(self):
-        self._read_glob_to_data_table()
+        self._register_dialect()
+        self._create_generated_file_from_model_file()
+        self._read_generated_file_to_dictionaries()
         return self.data_table
 
-    def _read_glob_to_data_table(self):
-        self._analyse_header(["*** Test Cases ***", self.kwargs.get("arg_name", "${file_name}")])
-        for match_path in sorted(glob(self.file)):
-            match_path = abspath(match_path).replace("\\", "/")
-            if isfile(match_path):
-                test_case_name = basename(splitext(match_path)[0])
-            elif isdir(match_path):
-                test_case_name = basename(normpath(match_path))
-            else:
-                test_case_name = match_path
-            self._read_data_from_table([test_case_name, match_path])
+    @staticmethod
+    def _register_dialect():
+        csv.register_dialect(
+            "PICT",
+            delimiter="\t",
+            skipinitialspace=False,
+            lineterminator="\r\n",
+            quoting=csv.QUOTE_NONE,
+        )
+
+    def _create_generated_file_from_model_file(self):
+        args = self.pict_options if hasattr(self, "pict_options") else ""
+        debug(f'pict "{self.file}" {args} > "{self.pictout_file}"')
+        os.system(f'pict "{self.file}" {args} > "{self.pictout_file}"')
+
+    def _read_generated_file_to_dictionaries(self):
+        with Path(self.pictout_file).open(encoding="utf_8") as csvfile:
+            reader = csv.reader(csvfile, "PICT")
+            for row_index, row in enumerate(reader):
+                if row_index == 0:
+                    row_of_variables = []
+                    for cell in row:
+                        row_of_variables.append(f"${{{cell}}}")
+                    self._analyse_header(row_of_variables)
+                else:
+                    self._read_data_from_table(row)
+        Path(self.pictout_file).unlink()
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/json_reader.py` & `robotframework-datadriver-1.8.0/src/DataDriver/json_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,17 @@
       "smoke"
     ],
     "documentation": "This is the doc"
   }
 ]
 """
 from json import load
+from pathlib import Path
+
 from .AbstractReaderClass import AbstractReaderClass
 from .ReaderConfig import TestCaseData
 
 
 class json_reader(AbstractReaderClass):
     def get_data_from_source(self):
-        with open(self.file, 'r', encoding="utf-8") as json_file:
+        with Path(self.file).open(encoding="utf-8") as json_file:
             return [TestCaseData(**test) for test in load(json_file)]
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/pict_reader.py` & `robotframework-datadriver-1.8.0/src/DataDriver/glob_reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,41 @@
-# Copyright 2018-  René Rohner
+# Copyright 2021-  René Rohner
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+# This Reader has initialy been created by Samual Montgomery-Blinn (https://github.com/montsamu)
+# Thanks for this contribution
 
 
-import csv
-import time
-import os
-from .AbstractReaderClass import AbstractReaderClass, ReaderConfig
-from DataDriver.utils import debug
+from glob import glob
+from pathlib import Path
 
+from DataDriver.AbstractReaderClass import AbstractReaderClass
 
-class pict_reader(AbstractReaderClass):
-    def __init__(self, reader_config: ReaderConfig):
-        super().__init__(reader_config)
-        file = self.file or ""
-        self.pictout_file = f"{os.path.splitext(file)[0]}{time.time()}.pictout"
 
+class glob_reader(AbstractReaderClass):
     def get_data_from_source(self):
-        self._register_dialect()
-        self._create_generated_file_from_model_file()
-        self._read_generated_file_to_dictionaries()
+        self._read_glob_to_data_table()
         return self.data_table
 
-    @staticmethod
-    def _register_dialect():
-        csv.register_dialect(
-            "PICT",
-            delimiter="\t",
-            skipinitialspace=False,
-            lineterminator="\r\n",
-            quoting=csv.QUOTE_NONE,
-        )
-
-    def _create_generated_file_from_model_file(self):
-        args = self.pict_options if hasattr(self, 'pict_options') else ''
-        debug(f'pict "{self.file}" {args} > "{self.pictout_file}"')
-        os.system(f'pict "{self.file}" {args} > "{self.pictout_file}"')
-
-    def _read_generated_file_to_dictionaries(self):
-        with open(self.pictout_file, "r", encoding="utf_8") as csvfile:
-            reader = csv.reader(csvfile, "PICT")
-            for row_index, row in enumerate(reader):
-                if row_index == 0:
-                    row_of_variables = []
-                    for cell in row:
-                        row_of_variables.append(f"${{{cell}}}")
-                    self._analyse_header(row_of_variables)
-                else:
-                    self._read_data_from_table(row)
-        os.remove(self.pictout_file)
+    def _read_glob_to_data_table(self):
+        self._analyse_header(["*** Test Cases ***", self.kwargs.get("arg_name", "${file_name}")])
+        for match_path in sorted(glob(self.file)):
+            path = Path(match_path).resolve()
+            path_as_posix = path.as_posix()
+            if path.is_file():
+                test_case_name = path.stem
+            elif path.is_dir():
+                test_case_name = path.name
+            else:
+                test_case_name = str(path_as_posix)
+            self._read_data_from_table([test_case_name, str(path_as_posix)])
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/rerunfailed.py` & `robotframework-datadriver-1.8.0/src/DataDriver/rerunfailed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Pre-run modifier that excludes tests that run PASS last time.
 """
 
-import os
 import re
+from pathlib import Path
 
 from robot.api import ExecutionResult, ResultVisitor, SuiteVisitor  # type: ignore
 from robot.running.model import Variable  # type: ignore
 
 
 class rerunfailed(SuiteVisitor):
     def __init__(self, original_output_xml):
-        if not os.path.isfile(original_output_xml):
+        if not Path(original_output_xml).is_file():
             raise FileNotFoundError(f"{original_output_xml} is no file")
         result = ExecutionResult(original_output_xml)
         results_visitor = DataDriverResultsVisitor()
         result.visit(results_visitor)
         self._failed_tests = results_visitor.failed_tests
 
     def start_suite(self, suite):
         """Remove tests that match the given pattern."""
         if self.has_no_tests(suite.name):
             suite.tests.clear()
-            return None
+            return
         if self._suite_is_data_driven(suite):
             dynamic_tests = Variable("@{DYNAMICTESTS}", self._failed_tests, suite.source)
             suite.resource.variables.append(dynamic_tests)
         else:
             suite.tests = [
                 t for t in suite.tests if f"{t.parent.name}.{t.name}" in self._failed_tests
             ]
@@ -34,24 +34,24 @@
         r = re.compile(f'^{re.escape(f"{name}.")}.*$')
         return not bool(list(filter(r.match, self._failed_tests)))
 
     def _suite_is_data_driven(self, suite):
         for resource in suite.resource.imports:
             if resource.name == "DataDriver":
                 return True
+        return None
 
     def end_suite(self, suite):
         """Remove suites that are empty after removing tests."""
         suite.suites = [s for s in suite.suites if s.test_count > 0]
 
     def visit_test(self, test):
         """Avoid visiting tests and their keywords to save a little time."""
-        pass
 
 
 class DataDriverResultsVisitor(ResultVisitor):
     def __init__(self):
-        self.failed_tests = list()
+        self.failed_tests = []
 
     def start_test(self, test):
         if test.status == "FAIL":
             self.failed_tests.append(f"{test.parent.name}.{test.name}")
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/search.py` & `robotframework-datadriver-1.8.0/src/DataDriver/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def search_variable(string, identifiers="$@&%*", ignore_errors=False):
     if not (isinstance(string, str) and "{" in string):
         return VariableMatch(string)
     return VariableSearcher(identifiers, ignore_errors).search(string)
 
 
-class VariableMatch(object):
+class VariableMatch:
     def __init__(self, string, identifier=None, base=None, items=(), start=-1, end=-1):
         self.string = string
         self.identifier = identifier
         self.base = base
         self.items = items
         self.start = start
         self.end = end
@@ -40,15 +40,15 @@
                 internal,
                 custom_unescaper=unescape_variable_syntax,
                 ignore_errors=ignore_errors,
             )
 
     @property
     def name(self):
-        return "%s{%s}" % (self.identifier, self.base) if self else None
+        return f"{self.identifier}{{{self.base}}}" if self else None
 
     @property
     def before(self):
         return self.string[: self.start] if self.identifier else self.string
 
     @property
     def match(self):
@@ -75,18 +75,18 @@
     def __bool__(self):
         return self.identifier is not None
 
     def __str__(self):
         if not self:
             return "<no match>"
         items = "".join("[%s]" % i for i in self.item) if self.items else ""
-        return "%s{%s}%s" % (self.identifier, self.base, items)
+        return f"{self.identifier}{{{self.base}}}{items}"
 
 
-class VariableSearcher(object):
+class VariableSearcher:
     def __init__(self, identifiers, ignore_errors=False):
         self.identifiers = identifiers
         self._ignore_errors = ignore_errors
         self.start = -1
         self.variable_chars = []
         self.item_chars = []
         self.items = []
@@ -194,16 +194,16 @@
             incomplete = "".join(self.variable_chars)
             raise VariableError("Variable '%s' was not closed properly." % incomplete)
         if state == self.item_state:
             variable = "".join(self.variable_chars)
             items = "".join("[%s]" % i for i in self.items)
             incomplete = "".join(self.item_chars)
             raise VariableError(
-                "Variable item '%s%s[%s' was not closed "
-                "properly." % (variable, items, incomplete)
+                "Variable item '{}{}[{}' was not closed "
+                "properly.".format(variable, items, incomplete)
             )
 
 
 def unescape_variable_syntax(item):
     def handle_escapes(match):
         escapes, text = match.groups()
         if len(escapes) % 2 == 1 and starts_with_variable_or_curly(text):
@@ -217,15 +217,15 @@
         return match and match.start == 0
 
     return re.sub(r"(\\+)(?=(.+))", handle_escapes, item)
 
 
 # TODO: This is pretty odd/ugly and used only in two places. Implement
 # something better or just remove altogether.
-class VariableIterator(object):
+class VariableIterator:
     def __init__(self, string, identifiers="$@&%*"):
         self._string = string
         self._identifiers = identifiers
 
     def __iter__(self):
         remaining = self._string
         while True:
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/utils.py` & `robotframework-datadriver-1.8.0/src/DataDriver/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 import re
-
 from enum import Enum, auto
-from robot.libraries.BuiltIn import BuiltIn  # type: ignore
+from typing import Any, List
+
 from robot.api import logger  # type: ignore
-from typing import List, Any
+from robot.libraries.BuiltIn import BuiltIn  # type: ignore
 
 from .argument_utils import is_pabot_testlevelsplit
 
 
 class Encodings(Enum):
     """
     Python comes with a number of codecs built-in,
@@ -33,15 +33,15 @@
     - cp1252
     - an ISO 8859 codeset
     - a Microsoft Windows code page, which is typically derived from an 8859 codeset, but replaces control characters with additional graphic characters
     - an IBM EBCDIC code page
     - an IBM PC code page, which is ASCII compatible
     """
 
-    ascii = auto()
+    ascii = auto()  # noqa: A003
     big5 = auto()
     big5hkscs = auto()
     cp037 = auto()
     cp273 = auto()
     cp424 = auto()
     cp437 = auto()
     cp500 = auto()
@@ -187,23 +187,23 @@
 def error(msg: Any, html: bool = False):
     logger.error(msg, html)
 
 
 def get_filter_dynamic_test_names():
     dynamic_test_list = get_variable_value("${DYNAMICTESTS}")
     if isinstance(dynamic_test_list, str):
-        test_names_esc = re.split(r'(?<!\\)(?:\\\\)*\|', dynamic_test_list)
-        return [name.replace('\\|', '|').replace('\\\\', '\\') for name in test_names_esc]
-    elif isinstance(dynamic_test_list, list):
+        test_names_esc = re.split(r"(?<!\\)(?:\\\\)*\|", dynamic_test_list)
+        return [name.replace("\\|", "|").replace("\\\\", "\\") for name in test_names_esc]
+    if isinstance(dynamic_test_list, list):
         return dynamic_test_list
-    else:
-        dynamic_test_name = get_variable_value("${DYNAMICTEST}")
-        if dynamic_test_name:
-            BuiltIn().set_suite_metadata("DataDriver", dynamic_test_name, True)
-            return [dynamic_test_name]
+    dynamic_test_name = get_variable_value("${DYNAMICTEST}")
+    if dynamic_test_name:
+        BuiltIn().set_suite_metadata("DataDriver", dynamic_test_name, True)
+        return [dynamic_test_name]
+    return None
 
 
 def is_pabot_dry_run():
     return is_pabot_testlevelsplit() and get_variable_value("${PABOTQUEUEINDEX}") == "-1"
 
 
 def get_variable_value(name: str):
@@ -216,26 +216,26 @@
 
 def _get_normalized_keyword(keyword: str):
     return keyword.lower().replace(" ", "").replace("_", "")
 
 
 def binary_partition_test_list(test_list: List, process_count: int):
     fractions = equally_partition_test_list(test_list, process_count)
-    return_list = list()
-    for i in range(int(math.sqrt(len(test_list) // process_count))):
+    return_list = []
+    for _i in range(int(math.sqrt(len(test_list) // process_count))):
         first, second = _partition_second_half(fractions)
         return_list.extend(first)
         fractions = second
     return_list.extend(fractions)
     return [test_name for test_name in return_list if test_name]
 
 
 def _partition_second_half(fractions):
     first = fractions[: len(fractions) // 2]
-    second = list()
+    second = []
     for sub_list in fractions[len(fractions) // 2 :]:
         sub_sub_list = equally_partition_test_list(sub_list, 2)
         second.extend(sub_sub_list)
     return first, second
 
 
 def equally_partition_test_list(test_list: List, fraction_count: int):
```

### Comparing `robotframework-datadriver-1.7.0/src/DataDriver/xlsx_reader.py` & `robotframework-datadriver-1.8.0/src/DataDriver/xlsx_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 try:
-    import pandas as pd  # type: ignore
     from math import nan  # type: ignore
-    import openpyxl  # type: ignore
-except ImportError:
+
+    import openpyxl  # type: ignore  # noqa: F401
+    import pandas as pd  # type: ignore
+except ImportError as err:
     raise ImportError(
         """Requirements (pandas, openpyxl) for XLSX support are not installed.
     Use 'pip install -U robotframework-datadriver[XLS]' to install XLSX support."""
-    )
+    ) from err
 from robot.utils import is_truthy  # type: ignore
 
 from .AbstractReaderClass import AbstractReaderClass
 
 
 class xlsx_reader(AbstractReaderClass):
     def get_data_from_source(self):
@@ -36,9 +37,9 @@
             except Exception as e:
                 e.row = row_index + 1
                 raise e
         return self.data_table
 
     def read_data_frame_from_file(self, dtype):
         return pd.read_excel(
-            self.file, sheet_name=self.sheet_name, dtype=dtype, engine="openpyxl"
+            self.file, sheet_name=self.sheet_name, dtype=dtype, engine="openpyxl", na_filter=False
         ).replace(nan, "", regex=True)
```

### Comparing `robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/PKG-INFO` & `robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: robotframework-datadriver
-Version: 1.7.0
+Version: 1.8.0
 Summary: A library for Data-Driven Testing.
 Home-page: https://github.com/Snooz82/robotframework-datadriver
 Author: René Rohner(Snooz82)
 Author-email: snooz@posteo.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Framework :: Robot Framework
-Requires-Python: >=3.6.15
+Requires-Python: >=3.7.12
 Description-Content-Type: text/x-rst
 Provides-Extra: xls
 License-File: LICENSE
 
 ===================================================
 DataDriver for Robot Framework®
 ===================================================
```

### Comparing `robotframework-datadriver-1.7.0/src/robotframework_datadriver.egg-info/SOURCES.txt` & `robotframework-datadriver-1.8.0/src/robotframework_datadriver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CONTRIBUTION.md
 COPYRIGHT.txt
 LICENSE
 MANIFEST.in
 Readme.rst
 create_readme.py
 dev-requirements.txt
+pyproject.toml
 setup.py
 atest/run_atest.bat
 atest/run_atest.sh
 atest/run_atest_pabot.bat
 atest/run_atest_pabot.sh
 atest/.mypy_cache/3.9/@plugins_snapshot.json
 atest/.mypy_cache/3.9/_ast.data.json
@@ -107,14 +108,15 @@
 atest/TestCases/custom_reader/dummy.txt
 atest/TestCases/custom_reader/file_search_strategy_none.robot
 atest/TestCases/custom_reader/jsonreader.robot
 atest/TestCases/custom_reader/with_path_and_file.robot
 atest/TestCases/performance/10.000.robot
 atest/TestCases/performance/10000.csv
 doc/DataDriver.html
+docs/index.html
 example/Login Tests/DataDriven.csv
 example/Login Tests/DataDriven.pict
 example/Login Tests/DataDriven.robot
 example/Login Tests/DataDriven.xls
 example/Login Tests/DataDriven.xlsx
 example/Login Tests/DataDriven_pict.robot
 example/Login Tests/DataDriven_regex.robot
```

