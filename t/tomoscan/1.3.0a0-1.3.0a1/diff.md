# Comparing `tmp/tomoscan-1.3.0a0.tar.gz` & `tmp/tomoscan-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomoscan-1.3.0a0.tar", last modified: Tue May  2 07:43:22 2023, max compression
+gzip compressed data, was "tomoscan-1.3.0a1.tar", last modified: Wed Jun 14 12:56:44 2023, max compression
```

## Comparing `tomoscan-1.3.0a0.tar` & `tomoscan-1.3.0a1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/
--rw-r--r--   0 payno    (81067) soft      (3401)     1253 2021-08-04 06:21:11.000000 tomoscan-1.3.0a0/LICENSE
--rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)      609 2023-03-08 13:26:14.000000 tomoscan-1.3.0a0/README.md
--rw-r--r--   0 payno    (81067) soft      (3401)     1213 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/setup.cfg
--rw-r--r--   0 payno    (81067) soft      (3401)     1486 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/setup.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.192546 tomoscan-1.3.0a0/tomoscan/
--rw-r--r--   0 payno    (81067) soft      (3401)       67 2022-03-24 14:18:52.000000 tomoscan-1.3.0a0/tomoscan/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/
--rw-r--r--   0 payno    (81067) soft      (3401)     1992 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)      263 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/edfscan.py
--rw-r--r--   0 payno    (81067) soft      (3401)      266 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/hdf5scan.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/identifier/
--rw-r--r--   0 payno    (81067) soft      (3401)     1765 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2926 2022-12-02 15:31:48.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/edfidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5467 2023-03-30 07:26:18.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/folderidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5781 2023-03-30 07:26:20.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/hdf5Identifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2302 2022-12-02 15:31:48.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/jp2kidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2732 2023-03-30 07:20:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/rawidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3621 2023-03-30 07:26:24.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/tiffidentifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2436 2023-03-30 07:19:36.000000 tomoscan-1.3.0a0/tomoscan/esrf/identifier/url_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)      254 2023-02-20 15:01:41.000000 tomoscan-1.3.0a0/tomoscan/esrf/mock.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/scan/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2023-02-08 14:54:26.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    43737 2023-03-30 14:34:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/edfscan.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/
--rw-r--r--   0 payno    (81067) soft      (3401)      118 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    25256 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/edfframereducer.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8542 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
--rw-r--r--   0 payno    (81067) soft      (3401)    58032 2023-05-02 07:34:41.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/hdf5scan.py
--rw-r--r--   0 payno    (81067) soft      (3401)    37157 2023-04-28 09:11:19.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/mock.py
--rw-r--r--   0 payno    (81067) soft      (3401)    22716 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/scan/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)      257 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/esrf/utils.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.200546 tomoscan-1.3.0a0/tomoscan/esrf/volume/
--rw-r--r--   0 payno    (81067) soft      (3401)     1637 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5369 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/edfvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)    18937 2023-04-28 14:23:39.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/hdf5volume.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8775 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/jp2kvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3035 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/mock.py
--rw-r--r--   0 payno    (81067) soft      (3401)    17047 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/rawvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)    15152 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/singleframebase.py
--rw-r--r--   0 payno    (81067) soft      (3401)    17517 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/tiffvolume.py
--rw-r--r--   0 payno    (81067) soft      (3401)     9222 2023-05-02 07:34:38.000000 tomoscan-1.3.0a0/tomoscan/esrf/volume/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)    10003 2023-04-28 09:02:37.000000 tomoscan-1.3.0a0/tomoscan/factory.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3757 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/framereducerbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2434 2023-02-01 10:03:58.000000 tomoscan-1.3.0a0/tomoscan/identifier.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6006 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/io.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.200546 tomoscan-1.3.0a0/tomoscan/nexus/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a0/tomoscan/nexus/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.200546 tomoscan-1.3.0a0/tomoscan/nexus/paths/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)      831 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxdetector.py
--rw-r--r--   0 payno    (81067) soft      (3401)      406 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxinstrument.py
--rw-r--r--   0 payno    (81067) soft      (3401)      250 2023-02-01 10:03:58.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxmonitor.py
--rw-r--r--   0 payno    (81067) soft      (3401)      540 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxsample.py
--rw-r--r--   0 payno    (81067) soft      (3401)      276 2023-01-10 13:59:36.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxsource.py
--rw-r--r--   0 payno    (81067) soft      (3401)    11151 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/nexus/paths/nxtomo.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5438 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/normalization.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3214 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/progress.py
--rw-r--r--   0 payno    (81067) soft      (3401)    66281 2023-03-31 07:57:09.000000 tomoscan-1.3.0a0/tomoscan/scanbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)      303 2022-08-12 07:51:29.000000 tomoscan-1.3.0a0/tomoscan/scanfactory.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8224 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/serie.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/tomoscan/test/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-12-06 12:48:08.000000 tomoscan-1.3.0a0/tomoscan/test/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)      266 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/conftest.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1732 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_framereducerbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)      451 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_hdf5_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2850 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_io.py
--rw-r--r--   0 payno    (81067) soft      (3401)     7466 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_normalization.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2013 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_progress.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8976 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_scanbase.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4569 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_scanfactory.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6223 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_serie.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1611 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_tomoobject.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3704 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)    11616 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_validator.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1502 2022-12-06 12:48:08.000000 tomoscan-1.3.0a0/tomoscan/test/test_version.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2909 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_volume_base.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6186 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/test_volume_utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8574 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/test/utils.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2341 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/tomoobject.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/tomoscan/unitsystem/
--rw-r--r--   0 payno    (81067) soft      (3401)     1657 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2447 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/electriccurrentsystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3270 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/energysystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     6542 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/metricsystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3165 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/timesystem.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1846 2022-12-02 15:31:48.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/unit.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1975 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/unitsystem/voltagesystem.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.204546 tomoscan-1.3.0a0/tomoscan/utils/
--rw-r--r--   0 payno    (81067) soft      (3401)      175 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1120 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/decorator.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2976 2023-01-05 08:34:39.000000 tomoscan-1.3.0a0/tomoscan/utils/geometry.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2666 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/hdf5.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1512 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/io.py
--rw-r--r--   0 payno    (81067) soft      (3401)     8884 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/utils/volume.py
--rw-r--r--   0 payno    (81067) soft      (3401)    17014 2023-03-30 07:18:03.000000 tomoscan-1.3.0a0/tomoscan/validator.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4346 2023-05-02 07:43:05.000000 tomoscan-1.3.0a0/tomoscan/version.py
--rw-r--r--   0 payno    (81067) soft      (3401)    19307 2023-05-02 07:34:38.000000 tomoscan-1.3.0a0/tomoscan/volumebase.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-02 07:43:22.196546 tomoscan-1.3.0a0/tomoscan.egg-info/
--rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)     2741 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/SOURCES.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/dependency_links.txt
--rw-r--r--   0 payno    (81067) soft      (3401)      300 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/requires.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        9 2023-05-02 07:43:21.000000 tomoscan-1.3.0a0/tomoscan.egg-info/top_level.txt
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1253 2021-08-04 06:21:11.000000 tomoscan-1.3.0a1/LICENSE
+-rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/PKG-INFO
+-rw-r--r--   0 payno    (81067) soft      (3401)      609 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/README.md
+-rw-r--r--   0 payno    (81067) soft      (3401)     1213 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/setup.cfg
+-rw-r--r--   0 payno    (81067) soft      (3401)     1486 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/setup.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.402967 tomoscan-1.3.0a1/tomoscan/
+-rw-r--r--   0 payno    (81067) soft      (3401)       67 2022-03-24 14:18:52.000000 tomoscan-1.3.0a1/tomoscan/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1992 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      263 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/edfscan.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      266 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/hdf5scan.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/identifier/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1765 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2926 2022-12-02 15:31:48.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/edfidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5467 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/folderidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5781 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/hdf5Identifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2302 2022-12-02 15:31:48.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/jp2kidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2732 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/rawidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3621 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/tiffidentifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2436 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/identifier/url_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      254 2023-02-20 15:01:41.000000 tomoscan-1.3.0a1/tomoscan/esrf/mock.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/scan/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2023-02-08 14:54:26.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    44250 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/edfscan.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/
+-rw-r--r--   0 payno    (81067) soft      (3401)      118 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    25256 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/edfframereducer.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8542 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    57936 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/hdf5scan.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    37157 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/mock.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    22716 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/scan/utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      257 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/utils.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/esrf/volume/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1637 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5369 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/edfvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    19300 2023-06-02 06:46:29.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/hdf5volume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8962 2023-05-26 12:33:10.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/jp2kvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3035 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/mock.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    17047 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/rawvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    15152 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/singleframebase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    17517 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/tiffvolume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     9222 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/esrf/volume/utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    10032 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/factory.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3757 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/framereducerbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2434 2023-02-01 10:03:58.000000 tomoscan-1.3.0a1/tomoscan/identifier.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6006 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/io.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.406967 tomoscan-1.3.0a1/tomoscan/nexus/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a1/tomoscan/nexus/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.410967 tomoscan-1.3.0a1/tomoscan/nexus/paths/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-05-03 11:55:01.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      831 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxdetector.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      406 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxinstrument.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      250 2023-02-01 10:03:58.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxmonitor.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      540 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxsample.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      276 2023-01-10 13:59:36.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxsource.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    11151 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/nexus/paths/nxtomo.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5438 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/normalization.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3214 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/progress.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    67019 2023-06-01 12:30:05.000000 tomoscan-1.3.0a1/tomoscan/scanbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      303 2022-08-12 07:51:29.000000 tomoscan-1.3.0a1/tomoscan/scanfactory.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8224 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/serie.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.410967 tomoscan-1.3.0a1/tomoscan/test/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2022-12-06 12:48:08.000000 tomoscan-1.3.0a1/tomoscan/test/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      266 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/conftest.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1732 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_framereducerbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)      451 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_hdf5_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2850 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_io.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     7466 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_normalization.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2013 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_progress.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8996 2023-06-01 12:30:05.000000 tomoscan-1.3.0a1/tomoscan/test/test_scanbase.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     4569 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_scanfactory.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6223 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_serie.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1611 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_tomoobject.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3704 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    11616 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_validator.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1502 2022-12-06 12:48:08.000000 tomoscan-1.3.0a1/tomoscan/test/test_version.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2933 2023-05-26 12:33:10.000000 tomoscan-1.3.0a1/tomoscan/test/test_volume_base.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6186 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/test_volume_utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8574 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/test/utils.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2341 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/tomoobject.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.410967 tomoscan-1.3.0a1/tomoscan/unitsystem/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1657 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2447 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/electriccurrentsystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3270 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/energysystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     6542 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/metricsystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3165 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/timesystem.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1846 2022-12-02 15:31:48.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/unit.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1975 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/unitsystem/voltagesystem.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.414967 tomoscan-1.3.0a1/tomoscan/utils/
+-rw-r--r--   0 payno    (81067) soft      (3401)      175 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1120 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/decorator.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2976 2023-01-05 08:34:39.000000 tomoscan-1.3.0a1/tomoscan/utils/geometry.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2666 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/hdf5.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1512 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/io.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     8884 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/utils/volume.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    17014 2023-05-26 12:33:07.000000 tomoscan-1.3.0a1/tomoscan/validator.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     4346 2023-06-14 12:56:34.000000 tomoscan-1.3.0a1/tomoscan/version.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    21351 2023-06-14 12:55:34.000000 tomoscan-1.3.0a1/tomoscan/volumebase.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-06-14 12:56:44.402967 tomoscan-1.3.0a1/tomoscan.egg-info/
+-rw-r--r--   0 payno    (81067) soft      (3401)      953 2023-06-14 12:56:43.000000 tomoscan-1.3.0a1/tomoscan.egg-info/PKG-INFO
+-rw-r--r--   0 payno    (81067) soft      (3401)     2741 2023-06-14 12:56:44.000000 tomoscan-1.3.0a1/tomoscan.egg-info/SOURCES.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-06-14 12:56:43.000000 tomoscan-1.3.0a1/tomoscan.egg-info/dependency_links.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)      300 2023-06-14 12:56:44.000000 tomoscan-1.3.0a1/tomoscan.egg-info/requires.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)        9 2023-06-14 12:56:44.000000 tomoscan-1.3.0a1/tomoscan.egg-info/top_level.txt
```

### Comparing `tomoscan-1.3.0a0/LICENSE` & `tomoscan-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/PKG-INFO` & `tomoscan-1.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a0
+Version: 1.3.0a1
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a0/README.md` & `tomoscan-1.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/setup.cfg` & `tomoscan-1.3.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/setup.py` & `tomoscan-1.3.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/__init__.py` & `tomoscan-1.3.0a1/tomoscan/esrf/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/__init__.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/edfidentifier.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/edfidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/folderidentifier.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/folderidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/hdf5Identifier.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/hdf5Identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/jp2kidentifier.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/jp2kidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/rawidentifier.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/rawidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/tiffidentifier.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/tiffidentifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/identifier/url_utils.py` & `tomoscan-1.3.0a1/tomoscan/esrf/identifier/url_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/scan/edfscan.py` & `tomoscan-1.3.0a1/tomoscan/esrf/scan/edfscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -713,14 +713,41 @@
         """
 
         :return: instrument name
         """
         return None
 
     @property
+    @docstring(TomoScanBase.title)
+    def title(self) -> Union[None, str]:
+        """
+
+        :return: title
+        """
+        return None
+
+    @property
+    @docstring(TomoScanBase.source_name)
+    def source_name(self) -> Union[None, str]:
+        """
+
+        :return: source name
+        """
+        return None
+
+    @property
+    @docstring(TomoScanBase.source_type)
+    def source_type(self) -> Union[None, str]:
+        """
+
+        :return: source type
+        """
+        return None
+
+    @property
     @docstring(TomoScanBase.distance)
     def distance(self) -> Union[None, float]:
         if self.__distance is None:
             self.__distance = EDFTomoScan.retrieve_information(
                 self.path,
                 dataset_basename=self.dataset_basename,
                 ref_file=None,
```

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/edfframereducer.py` & `tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/edfframereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/scan/framereducer/hdf5framereducer.py` & `tomoscan-1.3.0a1/tomoscan/esrf/scan/framereducer/hdf5framereducer.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/scan/hdf5scan.py` & `tomoscan-1.3.0a1/tomoscan/esrf/scan/hdf5scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,17 +205,14 @@
         self._end_time = None
         self._x_translations = None
         self._y_translations = None
         self._z_translations = None
         self._nexus_paths = None
         self._nexus_version = None
         self._user_nx_version = nx_version
-        self._source_type = None
-        self._source_name = None
-        self._instrument_name = None
 
     @staticmethod
     def get_master_file(scan_path):
         if os.path.isfile(scan_path):
             master_file = scan_path
         else:
             master_file = os.path.join(scan_path, os.path.basename(scan_path))
@@ -235,17 +232,14 @@
         self._x_pixel_size = None
         self._y_pixel_size = None
         self._x_magnified_pixel_size = None
         self._y_magnified_pixel_size = None
         self._distance = None
         self._fov = None
         self._source = None
-        self._source_type = None
-        self._source_name = None
-        self._instrument_name = None
         self._energy = None
         self._x_flipped = None
         self._y_flipped = None
         super().clear_caches()
 
     def clear_frames_caches(self):
         self._projections_compacted = None
@@ -421,14 +415,18 @@
             self._source = Source(
                 name=self.source_name,
                 type=self.source_type,
             )
         return self._source
 
     @property
+    def title(self):
+        return self._get_generic_key("_title", self.nexus_path.NAME_PATH)
+
+    @property
     def source_name(self):
         return self._get_generic_key("_source_name", self.nexus_path.SOURCE_NAME)
 
     @property
     def source_type(self):
         return self._get_generic_key("_source_type", self.nexus_path.SOURCE_TYPE)
```

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/scan/mock.py` & `tomoscan-1.3.0a1/tomoscan/esrf/scan/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/scan/utils.py` & `tomoscan-1.3.0a1/tomoscan/esrf/scan/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/__init__.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/edfvolume.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/edfvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/hdf5volume.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/hdf5volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 __authors__ = ["H. Payno", "P. Paleo"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
 import logging
 import os
-from typing import Optional
+from typing import Union, Optional
 
 import h5py
 import numpy
 from silx.io.dictdump import dicttonx, nxtodict
 from silx.io.url import DataUrl
 from silx.utils.deprecation import deprecated_warning
 
@@ -325,15 +325,15 @@
         if store:
             self.data = data
 
         return data
 
     def get_slice(
         self,
-        index=None,
+        index: Union[int, str] = None,
         axis=None,
         xy=None,
         xz=None,
         yz=None,
         url: Optional[DataUrl] = None,
     ):
         if xy is yz is xz is None and (index is None or axis is None):
@@ -368,14 +368,24 @@
             )
             if axis is None and index is None:
                 axis = 2
                 index = yz
             else:
                 raise ValueError("several axis (previously xy, xz, yz requested")
 
+        if isinstance(index, str):
+            if index == "first":
+                index = 0
+            elif index == "middle":
+                index = self.get_volume_shape()[axis] // 2
+            elif index == "last":
+                index = -1
+            else:
+                raise ValueError(f"index '{index}' is not handled")
+
         if self.data is not None:
             return self.select(volume=self.data, axis=axis, index=index)
         else:
             url = url or self.data_url
             if url is None:
                 raise ValueError(
                     "Cannot get data_url. An url should be provided. Don't know where to save this."
```

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/jp2kvolume.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/jp2kvolume.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,26 @@
         self._psnr = psnr
         self.setup_multithread_encoding(n_threads=n_threads)
 
     @property
     def cratios(self) -> Optional[list]:
         return self._cratios
 
+    @cratios.setter
+    def cratios(self, cratios: Optional[list]):
+        self._cratios = cratios
+
     @property
     def psnr(self) -> Optional[list]:
         return self._psnr
 
+    @psnr.setter
+    def psnr(self, psnr: Optional[list]):
+        self._psnr = psnr
+
     @docstring(VolumeSingleFrameBase)
     def save_frame(self, frame, file_name, scheme):
         if not has_glymur:
             raise RuntimeError(_MISSING_GLYMUR_MSG)
 
         if scheme == "glymur":
             glymur.Jp2k(file_name, data=frame, psnr=self.psnr, cratios=self.cratios)
```

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/mock.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/mock.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/rawvolume.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/rawvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/singleframebase.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/singleframebase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/tiffvolume.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/tiffvolume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/esrf/volume/utils.py` & `tomoscan-1.3.0a1/tomoscan/esrf/volume/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/factory.py` & `tomoscan-1.3.0a1/tomoscan/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         :param str identifier: identifier of the TomoScanBase
         :raises: TypeError if identifier is not a str
         :raises: ValueError if identifier cannot be converted back to an instance of TomoScanBase
         """
         if not isinstance(identifier, (str, BaseIdentifier)):
             raise TypeError(
-                f"identifier is expected to be a str or an instance of {BaseIdentifier} not {type(identifier)}"
+                f"identifier is expected to be a str or an instance of {BaseIdentifier} not {type(identifier)}. {type(identifier)} provided"
             )
 
         # step 1: convert identifier to an instance of BaseIdentifier if necessary
         if isinstance(identifier, str):
             info = urlparse(identifier)
             paths = split_path(info.path)
             scheme = info.scheme
```

### Comparing `tomoscan-1.3.0a0/tomoscan/framereducerbase.py` & `tomoscan-1.3.0a1/tomoscan/framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/identifier.py` & `tomoscan-1.3.0a1/tomoscan/identifier.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/io.py` & `tomoscan-1.3.0a1/tomoscan/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/nexus/paths/nxdetector.py` & `tomoscan-1.3.0a1/tomoscan/nexus/paths/nxdetector.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/nexus/paths/nxsample.py` & `tomoscan-1.3.0a1/tomoscan/nexus/paths/nxsample.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/nexus/paths/nxtomo.py` & `tomoscan-1.3.0a1/tomoscan/nexus/paths/nxtomo.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/normalization.py` & `tomoscan-1.3.0a1/tomoscan/normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/progress.py` & `tomoscan-1.3.0a1/tomoscan/progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/scanbase.py` & `tomoscan-1.3.0a1/tomoscan/scanbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,22 @@
 
     @staticmethod
     def split_data_and_metadata(my_dict):
         metadata = ReducedFramesInfos().load_from_dict(my_dict)
         data = ReducedFramesInfos.pop_info_keys(my_dict)
         return data, metadata
 
+    def __str__(self):
+        return "\n".join(
+            [
+                f"machine_electric_current {self.machine_electric_current}",
+                f"count_time {self.count_time}",
+            ]
+        )
+
 
 class TomoScanBase(TomoObject):
     """
     Base Class representing a scan.
     It is used to obtain core information regarding an aquisition like
     projections, dark and flat field...
 
@@ -273,19 +281,27 @@
         """monitor of the intensity during acquisition. Can be a diode
         for example"""
         self._source = None
         self._intensity_normalization = IntensityNormalization()
         """Extra information for normalization"""
         self._electric_current = None
         self._count_time = None
+        self._source_type = None
+        self._source_name = None
+        self._instrument_name = None
+        self._title = None
 
     def clear_caches(self):
         """clear caches. Might be call if some data changed after
         first read of data or metadata"""
         self._notify_ffc_rsc_missing = True
+        self._source_type = None
+        self._source_name = None
+        self._instrument_name = None
+        self._title = None
         self.clear_frames_caches()
 
     def clear_frames_caches(self):
         self._alignment_projections = None
         self._flats_weights = None
         self._projections = None
 
@@ -612,14 +628,26 @@
         if not isinstance(current, (type(None), tuple)):
             raise TypeError(
                 f"current is expected to be None or a tuple. Not {type(current)}"
             )
         self._electric_current = current
 
     @property
+    def title(self):
+        raise NotImplementedError("Base class")
+
+    @property
+    def source_name(self):
+        raise NotImplementedError("Base class")
+
+    @property
+    def source_type(self):
+        raise NotImplementedError("Base class")
+
+    @property
     def x_flipped(self) -> bool:
         """
         return True if  the frames are flip through x
         """
         raise NotImplementedError("Base class")
 
     @property
```

### Comparing `tomoscan-1.3.0a0/tomoscan/serie.py` & `tomoscan-1.3.0a1/tomoscan/serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_framereducerbase.py` & `tomoscan-1.3.0a1/tomoscan/test/test_framereducerbase.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_io.py` & `tomoscan-1.3.0a1/tomoscan/test/test_io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_normalization.py` & `tomoscan-1.3.0a1/tomoscan/test/test_normalization.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_progress.py` & `tomoscan-1.3.0a1/tomoscan/test/test_progress.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_scanbase.py` & `tomoscan-1.3.0a1/tomoscan/test/test_scanbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,7 +254,9 @@
     new_infos.load_from_dict(my_dict)
     assert new_infos.to_dict() == my_dict
 
     with pytest.raises(TypeError):
         new_infos.count_time = 12
     with pytest.raises(TypeError):
         new_infos.machine_electric_current = 12
+
+    str(new_infos)
```

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_scanfactory.py` & `tomoscan-1.3.0a1/tomoscan/test/test_scanfactory.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_serie.py` & `tomoscan-1.3.0a1/tomoscan/test/test_serie.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_tomoobject.py` & `tomoscan-1.3.0a1/tomoscan/test/test_tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_utils.py` & `tomoscan-1.3.0a1/tomoscan/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_validator.py` & `tomoscan-1.3.0a1/tomoscan/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_version.py` & `tomoscan-1.3.0a1/tomoscan/test/test_version.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_volume_base.py` & `tomoscan-1.3.0a1/tomoscan/test/test_volume_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,9 +79,9 @@
     with pytest.raises(NotImplementedError):
         volume_base.browse_data_urls()
 
     volume_base.position = (0, 1, 2)
     assert isinstance(volume_base.position, tuple)
     assert volume_base.position == (0, 1, 2)
 
-    volume_base.pixel_size = 12.3
-    assert volume_base.pixel_size == 12.3
+    volume_base.voxel_size = (12.3, 2.5, 6.9)
+    assert volume_base.voxel_size == (12.3, 2.5, 6.9)
```

### Comparing `tomoscan-1.3.0a0/tomoscan/test/test_volume_utils.py` & `tomoscan-1.3.0a1/tomoscan/test/test_volume_utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/test/utils.py` & `tomoscan-1.3.0a1/tomoscan/test/utils.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/tomoobject.py` & `tomoscan-1.3.0a1/tomoscan/tomoobject.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/__init__.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/electriccurrentsystem.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/electriccurrentsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/energysystem.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/energysystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/metricsystem.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/metricsystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/timesystem.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/timesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/unit.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/unit.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/unitsystem/voltagesystem.py` & `tomoscan-1.3.0a1/tomoscan/unitsystem/voltagesystem.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/utils/decorator.py` & `tomoscan-1.3.0a1/tomoscan/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/utils/geometry.py` & `tomoscan-1.3.0a1/tomoscan/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/utils/hdf5.py` & `tomoscan-1.3.0a1/tomoscan/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/utils/io.py` & `tomoscan-1.3.0a1/tomoscan/utils/io.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/utils/volume.py` & `tomoscan-1.3.0a1/tomoscan/utils/volume.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/validator.py` & `tomoscan-1.3.0a1/tomoscan/validator.py`

 * *Files identical despite different names*

### Comparing `tomoscan-1.3.0a0/tomoscan/version.py` & `tomoscan-1.3.0a1/tomoscan/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 3
 MICRO = 0
 RELEV = "alpha"  # <16
-SERIAL = 0  # <16
+SERIAL = 1  # <16
 
 date = __date__
 
 
 _version_info = namedtuple(
     "version_info", ["major", "minor", "micro", "releaselevel", "serial"]
 )
```

### Comparing `tomoscan-1.3.0a0/tomoscan/volumebase.py` & `tomoscan-1.3.0a1/tomoscan/volumebase.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,28 +27,30 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "27/01/2022"
 
 
 from typing import Optional, Union
-
+import logging
 import numpy
 from silx.io.url import DataUrl
 from silx.math.combo import (  # pylint: disable=E0611 (not found from the pyx file)
     min_max,
 )
-from silx.utils.deprecation import deprecated_warning
+from silx.utils.deprecation import deprecated, deprecated_warning
 
 from tomoscan.identifier import VolumeIdentifier
 from tomoscan.scanbase import TomoScanBase
 from tomoscan.tomoobject import TomoObject
 from tomoscan.unitsystem.metricsystem import MetricSystem
 from tomoscan.utils import BoundingBox1D, BoundingBox3D
 
+_logger = logging.getLogger(__name__)
+
 
 class VolumeBase(TomoObject):
     """
     context: we aim at having a common way of saving and loading volumes through the tomotools suite.
     The goal is to aim handling of volumes when creating them or doing some operations with those like stitching...
 
     :param DataUlr url: url of the volume. Could be path to a master file if we can provide one per each volume. Otherwise could be a pattern of edf files or tiff file with a data range
@@ -154,15 +156,15 @@
             )
         if isinstance(data, numpy.ndarray) and data.ndim != 3:
             raise ValueError(f"data is expected to be 3D and not {data.ndim}D.")
         self._data = data
 
     def get_slice(
         self,
-        index=None,
+        index: Union[str, int] = None,
         axis=None,
         xy=None,
         xz=None,
         yz=None,
         url: Optional[DataUrl] = None,
     ):
         if xy is yz is xz is axis is None:
@@ -171,14 +173,23 @@
         if self.data is None:
             # fixme: must be redefined by inheriting classes.
             # for example for single base frame we are simply loading the full volume instead of retrieving the
             # file. This is a bottleneck especially for xy slice because all the files are loaded instead of one
             # in the worst case.
             self.load_data(url=url, store=True)
 
+        if isinstance(index, str):
+            if index == "middle":
+                index = self.get_volume_shape()[axis] // 2
+            elif index == "first":
+                index = 0
+            elif index == "last":
+                index = -1
+
+        print("index is", index)
         if self.data is not None:
             return self.select(
                 volume=self.data, xy=xy, xz=xz, yz=yz, axis=axis, index=index
             )
         else:
             return None
 
@@ -236,16 +247,18 @@
     def _insure_reconstruction_dict_exists(ddict):
         if "processing_options" not in ddict:
             ddict["processing_options"] = {}
         if "reconstruction" not in ddict["processing_options"]:
             ddict["processing_options"]["reconstruction"] = {}
 
     @property
-    def position(self) -> tuple:
-        """position are provided as a tuple using the same reference for axis as the volume data"""
+    def position(self) -> Optional[tuple]:
+        """position are provided as a tuple using the same reference for axis as the volume data.
+        position is returned as (axis_0_pos, axis_1_pos, axis_2_pos). Can also be see as (z_position, y_position, x_position)
+        """
         metadata = self.metadata or self.load_metadata()
         position = (
             metadata.get("processing_options", {})
             .get("reconstruction", {})
             .get("position", None)
         )
         if position is None:
@@ -259,75 +272,111 @@
             self.metadata = {}
         self._insure_reconstruction_dict_exists(self.metadata)
         self.metadata["processing_options"]["reconstruction"]["position"] = numpy.array(
             position
         )
 
     @property
+    @deprecated(replacement="voxel_size", since_version="1.3.0")
     def pixel_size(self):
+        return self.voxel_size
+
+    @pixel_size.setter
+    @deprecated(replacement="voxel_size", since_version="1.3.0")
+    def pixel_size(self, pixel_size) -> None:
+        if numpy.isscalar(pixel_size):
+            pixel_size = [pixel_size] * 3
+            _logger.warning(
+                "pixel_size is expected to be a tuple. Conversion will be removed soon. Please update your code"
+            )
+        self.voxel_size = pixel_size
+
+    @property
+    def voxel_size(self) -> Optional[tuple]:
+        """
+        voxel size as (axis 0 dim - aka z, axis 1 dim - aka y, axis 2 dim aka z)
+        """
         metadata = self.metadata or self.load_metadata()
-        pixel_size = (
+
+        voxel_size = (
             metadata.get("processing_options", {})
             .get("reconstruction", {})
-            .get("pixel_size_cm", None)
+            .get("voxel_size_cm", None)
         )
-        if pixel_size is not None:
-            return pixel_size * MetricSystem.CENTIMETER.value
+        if voxel_size is None:
+            # ensure backward compatibility with old volumes (before nabu 2023.1)
+            # try fall back on pixel_size_cm for old volumes
+            voxel_size = (
+                metadata.get("processing_options", {})
+                .get("reconstruction", {})
+                .get("pixel_size_cm", None)
+            )
+            if voxel_size is not None:
+                voxel_size = (voxel_size, voxel_size, voxel_size)
+
+        if voxel_size is not None:
+            if numpy.isscalar(voxel_size):
+                # be safer and handle the case voxel size is a scalar
+                voxel_size = [voxel_size] * 3
+            return tuple(numpy.array(voxel_size) * MetricSystem.CENTIMETER.value)
         return None
 
-    @pixel_size.setter
-    def pixel_size(self, pixel_size) -> None:
+    @voxel_size.setter
+    def voxel_size(self, voxel_size: tuple) -> None:
         if self.metadata is None:
             self.metadata = {}
+        if numpy.isscalar(voxel_size):
+            raise TypeError("voxel is expected to be a tuple of three values")
         self._insure_reconstruction_dict_exists(self.metadata)
-        self.metadata["processing_options"]["reconstruction"]["pixel_size_cm"] = (
-            pixel_size / MetricSystem.CENTIMETER.value
+        self.metadata["processing_options"]["reconstruction"]["voxel_size_cm"] = (
+            numpy.array(voxel_size) / MetricSystem.CENTIMETER.value
         )
 
     def get_volume_shape(self):
         raise NotImplementedError("Base class")
 
     def get_bounding_box(self, axis: Optional[Union[str, int]] = None):
         if axis is None:
-            x_bb = self.get_bounding_box(axis="x")
-            y_bb = self.get_bounding_box(axis="y")
-            z_bb = self.get_bounding_box(axis="z")
+            x_bb = self.get_bounding_box(axis=2)
+            y_bb = self.get_bounding_box(axis=1)
+            z_bb = self.get_bounding_box(axis=0)
             return BoundingBox3D(
                 (z_bb.min, y_bb.min, x_bb.min),
                 (z_bb.max, y_bb.max, x_bb.max),
             )
 
         position = self.position
         shape = self.get_volume_shape()
         # TODO: does it make sense that pixel size is a scalar ?
-        pixel_size = self.pixel_size
+        voxel_size = self.voxel_size
         missing = []
         if position is None:
             missing.append("position")
         if shape is None:
             missing.append("shape")
             raise ValueError("Unable to find volume shape")
-        if pixel_size is None:
+        if voxel_size is None:
             missing.append("pixel_size")
 
         if len(missing) > 0:
             raise ValueError(
                 f"Unable to get bounding box. Missing information: {'; '.join(missing)}"
             )
         assert axis is not None
-        if axis == "x":
-            idx = 2
-        elif axis == "y":
-            idx = 1
-        elif axis == "z":
-            idx = 0
-        else:
-            raise ValueError(f"axis '{axis}' is not handled")
-        min_pos_in_meter = position[idx] - pixel_size * shape[idx] / 2.0
-        max_pos_in_meter = position[idx] + pixel_size * shape[idx] / 2.0
+        if isinstance(axis, str):
+            if axis == "x":
+                axis = 2
+            elif axis == "y":
+                axis = 1
+            elif axis == "z":
+                axis = 0
+            else:
+                raise ValueError(f"axis '{axis}' is not handled")
+        min_pos_in_meter = position[axis] - voxel_size[axis] * shape[axis] / 2.0
+        max_pos_in_meter = position[axis] + voxel_size[axis] * shape[axis] / 2.0
         return BoundingBox1D(min_pos_in_meter, max_pos_in_meter)
 
     def get_min_max(self) -> tuple:
         """
         compute min max of the volume. Can take some time but avoid to load the full volume in memory
         """
         if self.data is not None:
```

### Comparing `tomoscan-1.3.0a0/tomoscan.egg-info/PKG-INFO` & `tomoscan-1.3.0a1/tomoscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomoscan
-Version: 1.3.0a0
+Version: 1.3.0a1
 Summary: "utilitary to access tomography data at esrf"
 Home-page: https://gitlab.esrf.fr/tomotools/tomoscan
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Project-URL: Bug Tracker, https://gitlab.esrf.fr/tomotools/tomoscan/-/issues
 Classifier: Intended Audience :: Education
```

### Comparing `tomoscan-1.3.0a0/tomoscan.egg-info/SOURCES.txt` & `tomoscan-1.3.0a1/tomoscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

