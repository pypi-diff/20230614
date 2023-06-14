# Comparing `tmp/libinsitu-1.4.tar.gz` & `tmp/libinsitu-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libinsitu-1.4.tar", last modified: Wed Mar 22 15:11:39 2023, max compression
+gzip compressed data, was "libinsitu-1.5.tar", last modified: Wed Jun 14 21:14:30 2023, max compression
```

## Comparing `libinsitu-1.4.tar` & `libinsitu-1.5.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.955687 libinsitu-1.4/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      152 2023-01-26 17:14:14.000000 libinsitu-1.4/.gitignore
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1703 2023-03-22 14:32:14.000000 libinsitu-1.4/.gitlab-ci.yml
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      645 2022-11-07 10:09:07.000000 libinsitu-1.4/.readthedocs.yaml
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2022-11-07 10:09:07.000000 libinsitu-1.4/LICENSE
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      123 2022-11-07 10:09:07.000000 libinsitu-1.4/MANIFEST.in
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      485 2023-02-27 11:33:04.000000 libinsitu-1.4/Makefile
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1836 2023-03-22 15:11:39.955687 libinsitu-1.4/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1279 2022-11-07 10:09:07.000000 libinsitu-1.4/README.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1359 2023-03-22 14:35:45.000000 libinsitu-1.4/RELEASE_NOTES.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1748 2022-11-07 10:09:07.000000 libinsitu-1.4/TODO.txt
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.939687 libinsitu-1.4/bin/
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      202 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/cat.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      204 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/check.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      205 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/diff.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      377 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/diff.sh
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      209 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/enrich-csv.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      204 2022-11-07 11:05:56.000000 libinsitu-1.4/bin/index.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      204 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/info.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      202 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/ls.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      201 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/qc.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      205 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/sync.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      208 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/transform.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      210 2022-11-07 10:09:07.000000 libinsitu-1.4/bin/update_meta.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.939687 libinsitu-1.4/docs/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      638 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/Makefile
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      804 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/make.bat
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       76 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/requirements.txt
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/_deps/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1136 2023-01-26 17:14:14.000000 libinsitu-1.4/docs/source/_deps/format_table.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/_deps/gitrep2/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       57 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      310 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/constants.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      198 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/exceptions.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3284 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/git.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3173 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/parser.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4249 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/remote.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2424 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/role.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1488 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_deps/gitrep2/setup.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.935687 libinsitu-1.4/docs/source/_static/
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/_static/css/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       90 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_static/css/custom.css
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/_static/img/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   319879 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/_static/img/web-interface.png
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/api/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      157 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/api/compute_qc_flags.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      206 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/api/dataframe_to_netcdf.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      617 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/api/index.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      505 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/api/netcdf_to_dataframe.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      156 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/api/visual_qc.md
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/docs/source/cli/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      606 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/cli/index.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7426 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/cli/ins-cat.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       92 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/cli/ins-info.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       86 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/cli/ins-qc.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      320 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/cli/ins-transform.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1686 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/conf.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    22043 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/conventions.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      783 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/data.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1945 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/index.md
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2406 2022-11-07 10:09:07.000000 libinsitu-1.4/docs/source/networks.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8653 2023-03-22 14:31:38.000000 libinsitu-1.4/docs/source/qc.md
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.943687 libinsitu-1.4/libinsitu/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      152 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       29 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/_version.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4421 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/catalog.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7716 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/cdl.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.947687 libinsitu-1.4/libinsitu/cli/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/cli/__init__.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     9895 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/cli/cat.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     1082 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/cli/check.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     4658 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/cli/diff.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)    11580 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/cli/enrich_csv.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7530 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/cli/index.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2105 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/cli/info.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     4132 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/cli/ls.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3190 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/cli/qc.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)    15104 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/cli/sync.py
--rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)    15899 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/cli/transform.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3703 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/cli/update_meta.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    24647 2023-03-22 14:46:57.000000 libinsitu-1.4/libinsitu/common.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.947687 libinsitu-1.4/libinsitu/handlers/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1144 2023-01-26 17:50:52.000000 libinsitu-1.4/libinsitu/handlers/ABOM.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1427 2023-01-26 17:50:55.000000 libinsitu-1.4/libinsitu/handlers/BSRN.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3102 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/handlers/ESMAP.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      636 2023-01-26 17:51:01.000000 libinsitu-1.4/libinsitu/handlers/IEA_PVPS.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      435 2023-01-26 17:51:05.000000 libinsitu-1.4/libinsitu/handlers/ISE_PVLive.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      506 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/handlers/METEO_FRANCE.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4137 2023-01-26 17:51:08.000000 libinsitu-1.4/libinsitu/handlers/NREL_MIDC.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      962 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/handlers/RAD.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1164 2023-01-26 17:51:11.000000 libinsitu-1.4/libinsitu/handlers/SAURAN.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1730 2023-01-26 17:51:14.000000 libinsitu-1.4/libinsitu/handlers/SKYNET.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4296 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/handlers/UniOregon_readdata.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/handlers/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7661 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/handlers/base_handler.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3232 2023-01-26 17:50:58.000000 libinsitu-1.4/libinsitu/handlers/enerMENA.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5272 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/log.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.947687 libinsitu-1.4/libinsitu/qc/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2023-01-12 17:09:12.000000 libinsitu-1.4/libinsitu/qc/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2728 2023-01-26 17:29:36.000000 libinsitu-1.4/libinsitu/qc/base_graphs.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.947687 libinsitu-1.4/libinsitu/qc/matplot/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6300 2023-01-26 17:22:56.000000 libinsitu-1.4/libinsitu/qc/matplot/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    20107 2023-02-21 15:38:31.000000 libinsitu-1.4/libinsitu/qc/matplot/graphs.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    15469 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/qc/qc_utils.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.947687 libinsitu-1.4/libinsitu/res/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8647 2023-02-21 15:34:41.000000 libinsitu-1.4/libinsitu/res/IEA_PVPS.cdl
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     9081 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/res/base.cdl
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1315 2022-11-07 11:05:56.000000 libinsitu-1.4/libinsitu/res/index.cdl
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4796 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/res/networks.csv
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.951687 libinsitu-1.4/libinsitu/res/station-info/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4346 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/ABOM.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    15198 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/BSRN.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4760 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/res/station-info/ESMAP.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    22272 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/IEA_PVPS.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8010 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/ISE_PVLive.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      337 2023-03-22 14:31:38.000000 libinsitu-1.4/libinsitu/res/station-info/METEO_FRANCE.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6057 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/res/station-info/NREL_MIDC.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5107 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/SAURAN.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1704 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/SKYNET.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1525 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/SOLRAD.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1227 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/res/station-info/SURFRAD.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/__init__.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1842 2022-11-07 10:09:07.000000 libinsitu-1.4/libinsitu/res/station-info/enerMENA.csv
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.951687 libinsitu-1.4/libinsitu/test/
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.939687 libinsitu-1.4/libinsitu/test/data/
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.951687 libinsitu-1.4/libinsitu/test/data/expected/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      178 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/test/data/expected/ABOM.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   297906 2023-01-26 18:03:15.000000 libinsitu-1.4/libinsitu/test/data/expected/BSRN-ILO-qc.png
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      633 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/test/data/expected/BSRN.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5904 2023-03-22 15:02:43.000000 libinsitu-1.4/libinsitu/test/end_to_end.py
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/test/out.csv
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1609 2023-01-26 17:14:14.000000 libinsitu-1.4/libinsitu/test/unit_tests.py
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.947687 libinsitu-1.4/libinsitu.egg-info/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1836 2023-03-22 15:11:39.000000 libinsitu-1.4/libinsitu.egg-info/PKG-INFO
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3317 2023-03-22 15:11:39.000000 libinsitu-1.4/libinsitu.egg-info/SOURCES.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2023-03-22 15:11:39.000000 libinsitu-1.4/libinsitu.egg-info/dependency_links.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      434 2023-03-22 15:11:39.000000 libinsitu-1.4/libinsitu.egg-info/entry_points.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      220 2023-03-22 15:11:39.000000 libinsitu-1.4/libinsitu.egg-info/requires.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       10 2023-03-22 15:11:39.000000 libinsitu-1.4/libinsitu.egg-info/top_level.txt
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.951687 libinsitu-1.4/notebooks/
-drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-03-22 15:11:39.955687 libinsitu-1.4/notebooks/data/
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  5050196 2023-01-16 16:49:57.000000 libinsitu-1.4/notebooks/data/sample-data.csv.gz
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  1933242 2023-01-16 16:49:57.000000 libinsitu-1.4/notebooks/read-data.ipynb
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  1687968 2023-02-16 16:13:12.000000 libinsitu-1.4/notebooks/visual-quality-check.ipynb
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       22 2023-01-26 17:14:14.000000 libinsitu-1.4/requirements-dev.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      302 2023-01-26 17:14:14.000000 libinsitu-1.4/requirements.txt
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       38 2023-03-22 15:11:39.955687 libinsitu-1.4/setup.cfg
--rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2663 2023-01-26 17:14:14.000000 libinsitu-1.4/setup.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.579900 libinsitu-1.5/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      152 2023-01-26 17:14:14.000000 libinsitu-1.5/.gitignore
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1703 2023-03-22 14:32:14.000000 libinsitu-1.5/.gitlab-ci.yml
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      645 2022-11-07 10:09:07.000000 libinsitu-1.5/.readthedocs.yaml
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1331 2022-11-07 10:09:07.000000 libinsitu-1.5/LICENSE
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      123 2022-11-07 10:09:07.000000 libinsitu-1.5/MANIFEST.in
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      485 2023-02-27 11:33:04.000000 libinsitu-1.5/Makefile
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1836 2023-06-14 21:14:30.579900 libinsitu-1.5/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1279 2022-11-07 10:09:07.000000 libinsitu-1.5/README.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1426 2023-06-14 21:14:14.000000 libinsitu-1.5/RELEASE_NOTES.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1748 2022-11-07 10:09:07.000000 libinsitu-1.5/TODO.txt
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.563900 libinsitu-1.5/bin/
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      202 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/cat.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      204 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/check.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      205 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/diff.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      377 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/diff.sh
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      209 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/enrich-csv.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      204 2022-11-07 11:05:56.000000 libinsitu-1.5/bin/index.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      204 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/info.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      202 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/ls.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      201 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/qc.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      205 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/sync.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      208 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/transform.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)      210 2022-11-07 10:09:07.000000 libinsitu-1.5/bin/update_meta.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.563900 libinsitu-1.5/docs/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      638 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/Makefile
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      804 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/make.bat
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       76 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/requirements.txt
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.563900 libinsitu-1.5/docs/source/
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.563900 libinsitu-1.5/docs/source/_deps/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1136 2023-01-26 17:14:14.000000 libinsitu-1.5/docs/source/_deps/format_table.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.563900 libinsitu-1.5/docs/source/_deps/gitrep2/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       57 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      310 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/constants.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      198 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/exceptions.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3284 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/git.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3173 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/parser.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4249 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/remote.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2424 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/role.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1488 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_deps/gitrep2/setup.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.559900 libinsitu-1.5/docs/source/_static/
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.563900 libinsitu-1.5/docs/source/_static/css/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       90 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_static/css/custom.css
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.567900 libinsitu-1.5/docs/source/_static/img/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   319879 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/_static/img/web-interface.png
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.567900 libinsitu-1.5/docs/source/api/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      157 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/api/compute_qc_flags.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      206 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/api/dataframe_to_netcdf.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      617 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/api/index.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      505 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/api/netcdf_to_dataframe.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      156 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/api/visual_qc.md
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.567900 libinsitu-1.5/docs/source/cli/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      606 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/cli/index.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7426 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/cli/ins-cat.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       92 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/cli/ins-info.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       86 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/cli/ins-qc.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      320 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/cli/ins-transform.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1686 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/conf.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    22043 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/conventions.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      783 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/data.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1945 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/index.md
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2406 2022-11-07 10:09:07.000000 libinsitu-1.5/docs/source/networks.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8653 2023-03-22 14:31:38.000000 libinsitu-1.5/docs/source/qc.md
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.567900 libinsitu-1.5/libinsitu/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      152 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       29 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/_version.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4421 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/catalog.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7681 2023-06-14 21:14:14.000000 libinsitu-1.5/libinsitu/cdl.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.567900 libinsitu-1.5/libinsitu/cli/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/cli/__init__.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     9895 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/cli/cat.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     1082 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/cli/check.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     4658 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/cli/diff.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)    11766 2023-06-14 21:14:14.000000 libinsitu-1.5/libinsitu/cli/enrich_csv.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7530 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/cli/index.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2105 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/cli/info.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)     4132 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/cli/ls.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3190 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/cli/qc.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)    15104 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/cli/sync.py
+-rwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)    17113 2023-06-14 21:14:14.000000 libinsitu-1.5/libinsitu/cli/transform.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3703 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/cli/update_meta.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    25084 2023-06-14 21:14:14.000000 libinsitu-1.5/libinsitu/common.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/handlers/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1144 2023-01-26 17:50:52.000000 libinsitu-1.5/libinsitu/handlers/ABOM.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1427 2023-01-26 17:50:55.000000 libinsitu-1.5/libinsitu/handlers/BSRN.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3102 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/handlers/ESMAP.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5757 2023-06-14 21:14:14.000000 libinsitu-1.5/libinsitu/handlers/GenericCSVHandler.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      636 2023-01-26 17:51:01.000000 libinsitu-1.5/libinsitu/handlers/IEA_PVPS.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      435 2023-01-26 17:51:05.000000 libinsitu-1.5/libinsitu/handlers/ISE_PVLive.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      506 2023-03-30 15:26:13.000000 libinsitu-1.5/libinsitu/handlers/METEO_FRANCE.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4137 2023-01-26 17:51:08.000000 libinsitu-1.5/libinsitu/handlers/NREL_MIDC.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      962 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/handlers/RAD.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1164 2023-01-26 17:51:11.000000 libinsitu-1.5/libinsitu/handlers/SAURAN.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1730 2023-01-26 17:51:14.000000 libinsitu-1.5/libinsitu/handlers/SKYNET.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4296 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/handlers/UniOregon_readdata.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1147 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/handlers/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     7850 2023-06-14 21:14:14.000000 libinsitu-1.5/libinsitu/handlers/base_handler.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3232 2023-01-26 17:50:58.000000 libinsitu-1.5/libinsitu/handlers/enerMENA.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5272 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/log.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/qc/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2023-01-12 17:09:12.000000 libinsitu-1.5/libinsitu/qc/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2728 2023-01-26 17:29:36.000000 libinsitu-1.5/libinsitu/qc/base_graphs.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/qc/matplot/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6300 2023-01-26 17:22:56.000000 libinsitu-1.5/libinsitu/qc/matplot/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    20107 2023-02-21 15:38:31.000000 libinsitu-1.5/libinsitu/qc/matplot/graphs.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    15469 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/qc/qc_utils.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/res/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     9081 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/res/base.cdl
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1315 2022-11-07 11:05:56.000000 libinsitu-1.5/libinsitu/res/index.cdl
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4796 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/res/networks.csv
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/res/station-info/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4346 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/ABOM.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    15198 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/BSRN.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     4760 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/res/station-info/ESMAP.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)    22272 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/IEA_PVPS.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     8010 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/ISE_PVLive.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      337 2023-03-22 14:31:38.000000 libinsitu-1.5/libinsitu/res/station-info/METEO_FRANCE.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     6057 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/res/station-info/NREL_MIDC.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5107 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/SAURAN.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1704 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/SKYNET.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1525 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/SOLRAD.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1227 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/res/station-info/SURFRAD.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/__init__.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1842 2022-11-07 10:09:07.000000 libinsitu-1.5/libinsitu/res/station-info/enerMENA.csv
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/test/
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.559900 libinsitu-1.5/libinsitu/test/data/
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.571900 libinsitu-1.5/libinsitu/test/data/expected/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      178 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/test/data/expected/ABOM.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)   297906 2023-01-26 18:03:15.000000 libinsitu-1.5/libinsitu/test/data/expected/BSRN-ILO-qc.png
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      633 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/test/data/expected/BSRN.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     5904 2023-03-22 15:02:43.000000 libinsitu-1.5/libinsitu/test/end_to_end.py
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        0 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/test/out.csv
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1609 2023-01-26 17:14:14.000000 libinsitu-1.5/libinsitu/test/unit_tests.py
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.567900 libinsitu-1.5/libinsitu.egg-info/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     1836 2023-06-14 21:14:30.000000 libinsitu-1.5/libinsitu.egg-info/PKG-INFO
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     3330 2023-06-14 21:14:30.000000 libinsitu-1.5/libinsitu.egg-info/SOURCES.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)        1 2023-06-14 21:14:30.000000 libinsitu-1.5/libinsitu.egg-info/dependency_links.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      434 2023-06-14 21:14:30.000000 libinsitu-1.5/libinsitu.egg-info/entry_points.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      220 2023-06-14 21:14:30.000000 libinsitu-1.5/libinsitu.egg-info/requires.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       10 2023-06-14 21:14:30.000000 libinsitu-1.5/libinsitu.egg-info/top_level.txt
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.575900 libinsitu-1.5/notebooks/
+drwxrwxr-x   0 rjolivet  (1000) rjolivet  (1000)        0 2023-06-14 21:14:30.575900 libinsitu-1.5/notebooks/data/
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  5050196 2023-01-16 16:49:57.000000 libinsitu-1.5/notebooks/data/sample-data.csv.gz
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  1933242 2023-01-16 16:49:57.000000 libinsitu-1.5/notebooks/read-data.ipynb
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)  1687968 2023-02-16 16:13:12.000000 libinsitu-1.5/notebooks/visual-quality-check.ipynb
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       22 2023-01-26 17:14:14.000000 libinsitu-1.5/requirements-dev.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)      302 2023-01-26 17:14:14.000000 libinsitu-1.5/requirements.txt
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)       38 2023-06-14 21:14:30.579900 libinsitu-1.5/setup.cfg
+-rw-rw-r--   0 rjolivet  (1000) rjolivet  (1000)     2663 2023-01-26 17:14:14.000000 libinsitu-1.5/setup.py
```

### Comparing `libinsitu-1.4/.gitlab-ci.yml` & `libinsitu-1.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/.readthedocs.yaml` & `libinsitu-1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/LICENSE` & `libinsitu-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/PKG-INFO` & `libinsitu-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libinsitu
-Version: 1.4
+Version: 1.5
 Summary: This library provides tools to transform solar irradiation data from various networks to uniform NetCDF files. It also provides tools to request and manipulate those NetCDF files
 Home-page: https://git.sophia.mines-paristech.fr/oie/libinsitu
 Author: OIE - Mines ParisTech
 Author-email: raphael.jolivet@mines-paristech.fr
 License: BSD
 Keywords: in-situ,solar,pv,irradiation,NetCDF,FAIR,meta-data
 Platform: UNKNOWN
```

### Comparing `libinsitu-1.4/README.md` & `libinsitu-1.5/README.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/RELEASE_NOTES.md` & `libinsitu-1.5/RELEASE_NOTES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+1.5: 
+* Added generic encoding from Excel and CSV in CLI commands
+
 1.4 :
 * Added function dataframe_to_netcdf() to encode NetCDF from an existing dataframe
 * Updated the Convention to include QC flags in it
 * Added filter on QC in netcdf_to_dataframe() and cat.py CLI command
 
 1.3.2 :
 * Fixed IEA_PVPS after updates of convention : Time -> time
```

### Comparing `libinsitu-1.4/TODO.txt` & `libinsitu-1.5/TODO.txt`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/Makefile` & `libinsitu-1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/make.bat` & `libinsitu-1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_deps/format_table.py` & `libinsitu-1.5/docs/source/_deps/format_table.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_deps/gitrep2/git.py` & `libinsitu-1.5/docs/source/_deps/gitrep2/git.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_deps/gitrep2/parser.py` & `libinsitu-1.5/docs/source/_deps/gitrep2/parser.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_deps/gitrep2/remote.py` & `libinsitu-1.5/docs/source/_deps/gitrep2/remote.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_deps/gitrep2/role.py` & `libinsitu-1.5/docs/source/_deps/gitrep2/role.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_deps/gitrep2/setup.py` & `libinsitu-1.5/docs/source/_deps/gitrep2/setup.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/_static/img/web-interface.png` & `libinsitu-1.5/docs/source/_static/img/web-interface.png`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/api/index.md` & `libinsitu-1.5/docs/source/api/index.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/cli/index.md` & `libinsitu-1.5/docs/source/cli/index.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/cli/ins-cat.md` & `libinsitu-1.5/docs/source/cli/ins-cat.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/conf.py` & `libinsitu-1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/conventions.md` & `libinsitu-1.5/docs/source/conventions.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/data.md` & `libinsitu-1.5/docs/source/data.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/index.md` & `libinsitu-1.5/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/networks.csv` & `libinsitu-1.5/docs/source/networks.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/docs/source/qc.md` & `libinsitu-1.5/docs/source/qc.md`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/catalog.py` & `libinsitu-1.5/libinsitu/catalog.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cdl.py` & `libinsitu-1.5/libinsitu/cdl.py`

 * *Files 6% similar despite different names*

```diff
@@ -214,24 +214,24 @@
     for varname, vardef in cdl.variables.items() :
         initVar(ncfile, vardef, dry_run, delete_attrs)
 
     # Update global attributes
     update_attributes(ncfile, cdl.global_attributes, dry_run, delete_attrs)
 
 
-def init_nc(netcdf, properties, data_vars=DATA_VARS, dry_run=False, delete_attrs=False) :
+def init_nc(netcdf, properties, data_vars=DATA_VARS, dry_run=False, delete_attrs=False, custom_cdl=None) :
 
-    try:
-        # Try to load custom CDL first
-        custom_name = properties.get("Network_ID", "") + ".cdl"
-        cdl = parse_cdl(read_res(custom_name), properties)
-        info("Used custom CDL : %s" % custom_name)
+    # Read CDL from resource or custom file
+    if custom_cdl is None:
+        cdl_file = read_res(CDL_PATH)
+    else:
+        info("Using custom CDL file %s" % custom_cdl)
+        cdl_file = open(custom_cdl, "r")
 
-    except FileNotFoundError:
-        cdl = parse_cdl(read_res(CDL_PATH), properties)
+    cdl = parse_cdl(cdl_file, properties)
 
     # Ensures all requested data vars are defined
     missing_vars = set(data_var for data_var in data_vars if data_var not in cdl.variables)
     if len(missing_vars) > 0 :
         raise Exception("Unknown data vars : %s" % missing_vars)
 
     filtered_cdl = deepcopy(cdl)
```

### Comparing `libinsitu-1.4/libinsitu/cli/cat.py` & `libinsitu-1.5/libinsitu/cli/cat.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/check.py` & `libinsitu-1.5/libinsitu/cli/check.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/diff.py` & `libinsitu-1.5/libinsitu/cli/diff.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/enrich_csv.py` & `libinsitu-1.5/libinsitu/cli/enrich_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,24 +321,31 @@
 
     row["Timezone"] = "UTC%s%02d:%02d" % (sign, offset_min / 60, offset_min % 60)
 
 def enrich_coords(network, rows, nc_climate, ids=None) :
 
     tzFinder = TimezoneFinder()
 
-    for row in rows:
+    for i, row in enumerate(rows):
 
         if ids is not None and row["ID"] not in ids :
             continue
 
         lat = str2val(row["Latitude"])
         lon = str2val(row["Longitude"])
 
+        print("Processing ID %d. %d/%d" % (row["ID"], i, len(rows)))
+
+        print("Enrich  address")
         enrich_address(network, row, lat, lon)
+
+        print("Enrich  climate")
         enrich_climate(nc_climate, row, lat, lon)
+
+        print("Enrich  timezone")
         enrich_timezone(tzFinder, row, lat, lon)
 
     return rows
 
 
 def main_xls(xls_file, out_folder) :
```

### Comparing `libinsitu-1.4/libinsitu/cli/index.py` & `libinsitu-1.5/libinsitu/cli/index.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/info.py` & `libinsitu-1.5/libinsitu/cli/info.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/ls.py` & `libinsitu-1.5/libinsitu/cli/ls.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/qc.py` & `libinsitu-1.5/libinsitu/cli/qc.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/sync.py` & `libinsitu-1.5/libinsitu/cli/sync.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/cli/transform.py` & `libinsitu-1.5/libinsitu/cli/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os.path
 from os.path import basename, dirname
 from libinsitu import update_qc_flags
 from libinsitu.common import *
 from libinsitu.cdl import *
 from libinsitu.common import _prepare_properties
 from libinsitu.handlers import HANDLERS, InSituHandler, listNetworks
+from libinsitu.handlers.GenericCSVHandler import GenericCSVHandler
 from libinsitu.log import debug, info, warning, logger, LogContext, error
 import argparse
 
 
 DONE_SUFFIX = '.done'
 ERR_SUFFIX = '.err'
 
@@ -60,34 +61,57 @@
     if len(in_files) == 0:
         warning("No input file found")
         sys.exit(0)
 
     return in_files
 
 
-def process_network(network, station_id, out_filename, args) :
+def process_network(network, station_id, args) :
 
-    # Get properties for this station
-    properties = getProperties(network, station_id)
+    if args.mapping :
 
+        if not args.metadata :
+            raise Exception("Missing file path for custom station metadata")
 
-    handler : InSituHandler = HANDLERS[network](properties)
+        properties = getCustomProperties(
+            network,
+            station_id,
+            args.metadata)
+
+        handler = GenericCSVHandler(properties, args.mapping)
+    else:
+
+        # Check network
+        all_networks = listNetworks()
+        if not network in all_networks:
+            raise Exception("Bad Network %s. Should be one of %s" % (network, str(all_networks)))
+
+        # Get all properties
+        properties = getProperties(
+            network,
+            station_id)
+
+        handler : InSituHandler = HANDLERS[network](properties)
 
     in_files = list_files(args.in_files, handler)
 
-    new = not os.path.exists(out_filename)
+    new = not os.path.exists(args.out)
 
     # If file exists, put it in read only until we process an input file, to avoid changing its mtime
     mode = "w" if new else "r"
-    ncfile = Dataset(out_filename, mode=mode)
+    ncfile = Dataset(args.out, mode=mode)
 
     if new :
         # Nc File does not exist ==> create it
-        info("File '%s' was not there. Initializing it.", out_filename)
-        init_nc(ncfile, properties, [])
+        info("File '%s' was not there. Initializing it.", args.out)
+        init_nc(
+            ncfile,
+            properties,
+            data_vars=[],
+            custom_cdl=args.cdl)
 
     min_date = None
     max_date = None
 
     # Loop on input files
     for infile in in_files :
 
@@ -107,23 +131,24 @@
                 if not new and args.incremental and os.path.exists(status_file) and older_than(infile, status_file):
                     info("File %s is older than status file %s : Skipping", infile, status_file)
                     continue
 
                 # First processed file ? reopen the file in write mode => this will update its mtime
                 if mode == "r" :
                     ncfile.close()
-                    ncfile = Dataset(out_filename, mode="a")
+                    ncfile = Dataset(args.out, mode="a")
                     mode = "a"
 
                 data = handler.read_chunk(infile)
 
                 chunk_start, chunk_end = process_chunck(
                     data, ncfile, properties,
                     check=args.check,
-                    strict_resolution=args.strict_resolution)
+                    strict_resolution=args.strict_resolution,
+                    custom_cdl=args.cdl)
 
                 # Store extent of update
                 min_date = nmin(chunk_start, min_date)
                 max_date = nmax(chunk_end, max_date)
 
                 # Incremental mode : touch status file
                 if args.incremental:
@@ -235,29 +260,31 @@
         network_name=None,
         latitude=None,
         longitude=None,
         elevation=None,
         process_qc=True,
         close=True,
         network_props = dict(),
-        station_props = dict()) :
+        station_props = dict(),
+        custom_cdl=None) :
     """
     Transforms a Dataframe of solar irradiance to a well encoded NetCDF file.
 
     :param data: The dataframe. It should contain GHI, DHI, BNI columns in W.m-2 and be indexed by UTC time (Datetime index)
     :param out_filename: Name of output file
     :param station_name: Station name. Can also be passed as 'Name' in station properties
     :param network_name: Network name. Can also be passed as 'Name' in network properties
     :param latitude: Station latitude. Can also be passed as 'Latitude' in station properties
     :param longitude: Station longitude. Can also be passed as 'Longitude' in station properties
     :param elevation: Station elevation.  Can also be passed as 'Elevation' in station properties
     :param process_qc: Process and embed QC flags (true be default)
     :param close: Close netcdf file at the end of process
     :param network_props: Dict of additional network properties (without `Network_` prefix), as used in base.cdl
     :param station_props: Dict of additional station properties (without `Station_` prefix) as used in base.cdl
+    :param custom_cdl: File path to custom schema.cdl file
     """
 
     properties = _prepare_properties(
         network_props,
         station_props)
 
     def update_props(key, value) :
@@ -285,28 +312,30 @@
 
     # Create file
     ncfile = Dataset(out_filename, mode="w")
     try :
         init_nc(ncfile, properties, [])
 
         # Transform data
-        process_chunck(data, ncfile, properties)
+        process_chunck(
+            data, ncfile, properties,
+            custom_cdl=custom_cdl)
 
         if process_qc :
             update_qc_flags(ncfile)
 
     finally:
         if close :
             ncfile.close()
         return ncfile
 
 
 
 
-def process_chunck(data, ncfile, properties, strict_resolution=False, check=False):
+def process_chunck(data, ncfile, properties, strict_resolution=False, check=False, custom_cdl=None):
 
     if data is None or len(data) == 0 :
         warning("Chunk is empty")
         return
 
     # Time resolution, in seconds
     resolution_s = getTimeResolution(ncfile)
@@ -324,15 +353,15 @@
 
     columns = list(data.columns)
 
     # Create vars if not present yet
     missing_vars = list(col for col in columns if not col in ncfile.variables)
     if len(missing_vars) > 0:
         info("Adding missing vars : %s", missing_vars)
-        init_nc(ncfile, properties, missing_vars)
+        init_nc(ncfile, properties, missing_vars, custom_cdl=custom_cdl)
 
     # Ensure all timestamps fall into resolution
     exact_idx = (times_sec % resolution_s) == 0
     nb_not_exact_times = len(times_sec) - np.sum(exact_idx)
     if nb_not_exact_times > 0:
 
         # Remove lines with wrong times
@@ -417,31 +446,38 @@
         raise argparse.ArgumentTypeError(f"{path} is not a valid folder")
 
 
 def parser() :
     parser = argparse.ArgumentParser(description='Transforms In-Situ data into NetCDF files')
     parser.add_argument('out', metavar='<out.nc>', type=str, help='Output file')
     parser.add_argument('in_files', metavar='<file|dir>', nargs='+', help='Input files or folders')
-    parser.add_argument('--network', '-n', help='Network name', required=True, choices=listNetworks())
+    parser.add_argument('--network', '-n', help='Network name', required=True)
     parser.add_argument('--station-id', '-s', metavar='<SID>', help='Station ID', required=True)
-    parser.add_argument('--incremental', '-i', default=False, action='store_true',
-                        help="Incremental mode, skipping input files having a '.done' status files")
-    parser.add_argument('--strict-resolution', '-sr', default=False, action='store_true',
-                        help="Skip chunks having a different resulution")
+    parser.add_argument('--mapping', '-m', metavar='<mapping.json>', help='Use a generic parser with custom mapping. Tu be used in conjonction with --metadata')
+    parser.add_argument('--metadata', '-md', metavar='<station-meta.csv>', help='Use custom station metadata for this network')
+    parser.add_argument('--cdl', metavar='<schema.cdl>', help="Use a custom CDL (NetCDF schema)")
+    parser.add_argument(
+        '--incremental', '-i', default=False, action='store_true',
+        help="Incremental mode, skipping input files having a '.done' status files")
+    parser.add_argument(
+        '--strict-resolution', '-sr', default=False, action='store_true',
+        help="Skip chunks having a different resulution")
     parser.add_argument('--no-qc', default=False, action='store_true', help="Do not compute QC flags")
     parser.add_argument('--check', '-c', default=False, action='store_true', help="Check potential override of data")
-    parser.add_argument('--status-folder', '-f', metavar='<folder>', type=dir_path,
-                        help='Separate folder for .done/.err files')
+    parser.add_argument(
+        '--status-folder', '-f',
+        metavar='<folder>', type=dir_path,
+        help='Separate folder for .done/.err files')
     return parser
 
 def main():
 
     args = parser().parse_args()
 
     network = args.network
     station_id  = args.station_id
 
     with LogContext(network=network, station_id=station_id):
-        process_network(network, station_id, args.out, args)
+        process_network(network, station_id, args)
 
 if __name__ == '__main__':
     main()
```

### Comparing `libinsitu-1.4/libinsitu/cli/update_meta.py` & `libinsitu-1.5/libinsitu/cli/update_meta.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/common.py` & `libinsitu-1.5/libinsitu/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,25 +137,28 @@
 TIME_FORMAT_SEC= '%Y-%m-%dT%H:%M:%S'
 
 STATION_START_DATA_ATTR = "time_coverage_start"
 
 SECOND = timedelta64(1, 's')
 CDL_PATH = "base.cdl"
 
-def parseCSV(res_path, key = "ID") :
+def parseCSV(res_path, key = "ID", resource=True) :
     """Generic parser """
     res = dict()
-    rows = DictReader(read_res(res_path))
+
+    file = read_res(res_path) if resource else open(res_path, 'r')
+    rows = DictReader(file)
     for row in rows:
 
         # Skip commented lines
         if "#" in row[key] :
             continue
 
-        res[row[key]] = {key: parse_value(val) for key, val in row.items()}
+        # We force ID to stay a String
+        res[row[key]] = {k: val if k == key else parse_value(val) for k, val in row.items()}
     return res
 
 def getStationsInfo(network) :
     """Read station info from CSV"""
     return parseCSV(STATION_INFO_PATTERN % network)
 
 def getNetworksInfo() :
@@ -170,16 +173,20 @@
     """ creates or update the time of a file """
     if os.path.exists(filename):
         os.utime(filename)
     else:
         with open(filename,'a') :
             pass
 
-def getStationInfo(network, station_id) :
-    stations = getStationsInfo(network)
+def getStationInfo(network, station_id, custom_file=None) :
+
+    if custom_file :
+        stations = parseCSV(custom_file, resource=False)
+    else:
+        stations = getStationsInfo(network)
     if not station_id in stations :
         raise Exception("Station %s not found in Station Info of %s" % (station_id, network))
     return stations[station_id]
 
 def getNetworkInfo(network) :
     networks = getNetworksInfo()
     if not network in networks :
@@ -787,14 +794,19 @@
 def getProperties(network_id, station_id) :
     """Gather Network_ and Station_ properties """
 
     return _prepare_properties(
         getNetworkInfo(network_id),
         getStationInfo(network_id, station_id))
 
+def getCustomProperties(network_id, station_id, custom_station_file) :
+    return _prepare_properties(
+        dict(),
+        getStationInfo(network_id, station_id, custom_file=custom_station_file))
+
 def qc_masks(df) :
     """Parse metadata of a QC bitmap and returns dict of flag name => mask"""
     attrs = df.attrs["variables"][QC_FLAGS_VAR]
     return {meaning: mask for meaning, mask in zip(
         attrs["flag_meanings"].split(),
         attrs["flag_masks"]
     )}
```

### Comparing `libinsitu-1.4/libinsitu/handlers/ABOM.py` & `libinsitu-1.5/libinsitu/handlers/ABOM.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/BSRN.py` & `libinsitu-1.5/libinsitu/handlers/BSRN.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/ESMAP.py` & `libinsitu-1.5/libinsitu/handlers/ESMAP.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/IEA_PVPS.py` & `libinsitu-1.5/libinsitu/handlers/IEA_PVPS.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/NREL_MIDC.py` & `libinsitu-1.5/libinsitu/handlers/NREL_MIDC.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/RAD.py` & `libinsitu-1.5/libinsitu/handlers/RAD.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/SAURAN.py` & `libinsitu-1.5/libinsitu/handlers/SAURAN.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/SKYNET.py` & `libinsitu-1.5/libinsitu/handlers/SKYNET.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/UniOregon_readdata.py` & `libinsitu-1.5/libinsitu/handlers/UniOregon_readdata.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/__init__.py` & `libinsitu-1.5/libinsitu/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/handlers/base_handler.py` & `libinsitu-1.5/libinsitu/handlers/base_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,18 @@
     """Filter and rename columns """
     data = data[list(mapping.keys())]
     return data.rename(columns=mapping)
 
 class InSituHandler :
     """ Virtual class to be implemented for each new network """
     
-    def __init__(self, properties, entries_extensions=[".txt"]):
+    def __init__(self, properties, entries_extensions=[".txt"], binary=False):
         self.properties = properties.copy()
         self.entries_extensions = entries_extensions # Used for zip archive : select the entries to process
+        self.binary = binary
 
         # Also adds lower case version of properties
         for key, val in properties.items() :
             if isinstance(val, str) :
                 self.properties[key.lower()] = val.lower()
 
 
@@ -42,15 +43,15 @@
         zip_entry= None
         if '!' in filename :
             filename, zip_entry = filename.split('!')
 
         if filename.endswith(".gz") :
             with open(filename, "rb") as f:
                 stream =  TextIOWrapper(GzipFile(fileobj=f), encoding=encoding)
-                return self._read_chunk(stream)
+                return self._read_chunk(stream, entryname=filename)
 
         elif filename.endswith('.zip'):  # check if file is a zipped (.zip) file
 
             with ZipFile(filename) as thezip :
 
                 names = thezip.namelist()
 
@@ -80,16 +81,21 @@
                 # Sort by time
                 dfs = sorted(dfs, key=lambda df : df.index[0])
 
                 return pd.concat(dfs)
 
 
         else :
-            with open(filename, "rt", encoding=encoding) as f :
-                return self._read_chunk(f)
+            if self.binary :
+                f = open(filename, "rb")
+            else:
+                f = open(filename, "rt", encoding=encoding)
+
+            with f :
+                return self._read_chunk(f, entryname=filename)
 
     @abstractmethod
     def pattern(self):
         """Should return a file pattern for input files.
 
         The following placeholders are supported :
         *: any string
```

### Comparing `libinsitu-1.4/libinsitu/handlers/enerMENA.py` & `libinsitu-1.5/libinsitu/handlers/enerMENA.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/log.py` & `libinsitu-1.5/libinsitu/log.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/qc/base_graphs.py` & `libinsitu-1.5/libinsitu/qc/base_graphs.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/qc/matplot/__init__.py` & `libinsitu-1.5/libinsitu/qc/matplot/__init__.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/qc/matplot/graphs.py` & `libinsitu-1.5/libinsitu/qc/matplot/graphs.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/qc/qc_utils.py` & `libinsitu-1.5/libinsitu/qc/qc_utils.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/base.cdl` & `libinsitu-1.5/libinsitu/res/base.cdl`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/index.cdl` & `libinsitu-1.5/libinsitu/res/index.cdl`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/networks.csv` & `libinsitu-1.5/libinsitu/res/networks.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/ABOM.csv` & `libinsitu-1.5/libinsitu/res/station-info/ABOM.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/BSRN.csv` & `libinsitu-1.5/libinsitu/res/station-info/BSRN.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/ESMAP.csv` & `libinsitu-1.5/libinsitu/res/station-info/ESMAP.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/IEA_PVPS.csv` & `libinsitu-1.5/libinsitu/res/station-info/IEA_PVPS.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/ISE_PVLive.csv` & `libinsitu-1.5/libinsitu/res/station-info/ISE_PVLive.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/NREL_MIDC.csv` & `libinsitu-1.5/libinsitu/res/station-info/NREL_MIDC.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/SAURAN.csv` & `libinsitu-1.5/libinsitu/res/station-info/SAURAN.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/SKYNET.csv` & `libinsitu-1.5/libinsitu/res/station-info/SKYNET.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/SOLRAD.csv` & `libinsitu-1.5/libinsitu/res/station-info/SOLRAD.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/SURFRAD.csv` & `libinsitu-1.5/libinsitu/res/station-info/SURFRAD.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/res/station-info/enerMENA.csv` & `libinsitu-1.5/libinsitu/res/station-info/enerMENA.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/test/data/expected/BSRN-ILO-qc.png` & `libinsitu-1.5/libinsitu/test/data/expected/BSRN-ILO-qc.png`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/test/data/expected/BSRN.csv` & `libinsitu-1.5/libinsitu/test/data/expected/BSRN.csv`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/test/end_to_end.py` & `libinsitu-1.5/libinsitu/test/end_to_end.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu/test/unit_tests.py` & `libinsitu-1.5/libinsitu/test/unit_tests.py`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/libinsitu.egg-info/PKG-INFO` & `libinsitu-1.5/libinsitu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libinsitu
-Version: 1.4
+Version: 1.5
 Summary: This library provides tools to transform solar irradiation data from various networks to uniform NetCDF files. It also provides tools to request and manipulate those NetCDF files
 Home-page: https://git.sophia.mines-paristech.fr/oie/libinsitu
 Author: OIE - Mines ParisTech
 Author-email: raphael.jolivet@mines-paristech.fr
 License: BSD
 Keywords: in-situ,solar,pv,irradiation,NetCDF,FAIR,meta-data
 Platform: UNKNOWN
```

### Comparing `libinsitu-1.4/libinsitu.egg-info/SOURCES.txt` & `libinsitu-1.5/libinsitu.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 libinsitu/cli/qc.py
 libinsitu/cli/sync.py
 libinsitu/cli/transform.py
 libinsitu/cli/update_meta.py
 libinsitu/handlers/ABOM.py
 libinsitu/handlers/BSRN.py
 libinsitu/handlers/ESMAP.py
+libinsitu/handlers/GenericCSVHandler.py
 libinsitu/handlers/IEA_PVPS.py
 libinsitu/handlers/ISE_PVLive.py
 libinsitu/handlers/METEO_FRANCE.py
 libinsitu/handlers/NREL_MIDC.py
 libinsitu/handlers/RAD.py
 libinsitu/handlers/SAURAN.py
 libinsitu/handlers/SKYNET.py
@@ -91,15 +92,14 @@
 libinsitu/handlers/base_handler.py
 libinsitu/handlers/enerMENA.py
 libinsitu/qc/__init__.py
 libinsitu/qc/base_graphs.py
 libinsitu/qc/qc_utils.py
 libinsitu/qc/matplot/__init__.py
 libinsitu/qc/matplot/graphs.py
-libinsitu/res/IEA_PVPS.cdl
 libinsitu/res/__init__.py
 libinsitu/res/base.cdl
 libinsitu/res/index.cdl
 libinsitu/res/networks.csv
 libinsitu/res/station-info/ABOM.csv
 libinsitu/res/station-info/BSRN.csv
 libinsitu/res/station-info/ESMAP.csv
```

### Comparing `libinsitu-1.4/notebooks/data/sample-data.csv.gz` & `libinsitu-1.5/notebooks/data/sample-data.csv.gz`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/notebooks/read-data.ipynb` & `libinsitu-1.5/notebooks/read-data.ipynb`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/notebooks/visual-quality-check.ipynb` & `libinsitu-1.5/notebooks/visual-quality-check.ipynb`

 * *Files identical despite different names*

### Comparing `libinsitu-1.4/setup.py` & `libinsitu-1.5/setup.py`

 * *Files identical despite different names*

