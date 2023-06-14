# Comparing `tmp/pyincore-1.8.0.tar.gz` & `tmp/pyincore-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyincore-1.8.0.tar", last modified: Tue Nov 15 21:03:47 2022, max compression
+gzip compressed data, was "pyincore-1.9.0.tar", last modified: Tue Mar 14 16:05:41 2023, max compression
```

## Comparing `pyincore-1.8.0.tar` & `pyincore-1.9.0.tar`

### file list

```diff
@@ -1,183 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.136713 pyincore-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-11-15 21:03:11.000000 pyincore-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-15 21:03:11.000000 pyincore-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-11-15 21:03:47.136713 pyincore-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-11-15 21:03:11.000000 pyincore-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/bridgedamage/
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/bridgedamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16241 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/bridgedamage/bridgedamage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/bridgedamage/bridgeutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/buildingdamage/
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingdamage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16054 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingdamage/buildingdamage.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingdamage/buildingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/buildingeconloss/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingeconloss/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7278 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingeconloss/buildingeconloss.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/buildingfunctionality/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingfunctionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10722 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingfunctionality/buildingfunctionality.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/buildingportfolio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingportfolio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/BuildingDamage.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/BuildingData.py
--rw-r--r--   0 runner    (1001) docker     (121)    38490 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/BuildingPortfolioRecoveryAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/capitalshocks/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/capitalshocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4625 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/capitalshocks/capitalshocks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/combinedwindwavesurgebuildingdamage/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/combinedwindwavesurgebuildingdamage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5116 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/combinedwindwavesurgebuildingdamage/combinedwindwavesurgebuildingdamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/cumulativebuildingdamage/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/cumulativebuildingdamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8767 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/cumulativebuildingdamage/cumulativebuildingdamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/epfdamage/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epfdamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17794 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epfdamage/epfdamage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epfdamage/epfutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore/analyses/epfrestoration/
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epfrestoration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11556 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epfrestoration/epfrestoration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epfrestoration/epfrestorationutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/epnfunctionality/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epnfunctionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7787 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epnfunctionality/epnfunctionality.py
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/epnfunctionality/epnfunctionalityutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/example/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/example/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3389 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/example/exampleanalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/housingrecovery/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingrecovery/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17454 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingrecovery/housingrecovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     5711 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingrecovery/housingrecoveryutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/housingrecoverysequential/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingrecoverysequential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19740 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingrecoverysequential/housingrecoverysequential.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/housingunitallocation/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingunitallocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13453 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/housingunitallocation/housingunitallocation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/joplincge/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplincge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30316 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplincge/equationlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    78047 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplincge/joplincge.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplincge/outputfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/joplinempiricalrestoration/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplinempiricalrestoration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8584 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplinempiricalrestoration/joplinempiricalrestoration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/joplinempiricalrestoration/joplinempirrestor_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/meandamage/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/meandamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8964 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/meandamage/meandamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/montecarlofailureprobability/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/montecarlofailureprobability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13992 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/montecarlofailureprobability/montecarlofailureprobability.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/multiobjectiveretrofitoptimization/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/multiobjectiveretrofitoptimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    74302 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/multiobjectiveretrofitoptimization/multiobjectiveretrofitoptimization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/ncifunctionality/
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/ncifunctionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20741 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/ncifunctionality/ncifunctionality.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/nonstructbuildingdamage/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/nonstructbuildingdamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20366 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingdamage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2953 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/pipelinedamage/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinedamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12587 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinedamage/pipelinedamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/pipelinedamagerepairrate/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinedamagerepairrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18918 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinedamagerepairrate/pipelinedamagerepairrate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinedamagerepairrate/pipelineutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/pipelinefunctionality/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinefunctionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6259 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinefunctionality/pipelinefunctionality.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.128713 pyincore-1.8.0/pyincore/analyses/pipelinerestoration/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinerestoration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/pipelinerestoration/pipelinerestoration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/populationdislocation/
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/populationdislocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10041 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/populationdislocation/populationdislocation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8053 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/populationdislocation/populationdislocationutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/residentialbuildingrecovery/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/residentialbuildingrecovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25752 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/residentialbuildingrecovery/residentialbuildingrecovery.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/roaddamage/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/roaddamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16067 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/roaddamage/roaddamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/seasidecge/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/seasidecge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33512 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/seasidecge/equationlib.py
--rw-r--r--   0 runner    (1001) docker     (121)    84786 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/seasidecge/seasidecge.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/socialvulnerability/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/socialvulnerability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6408 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/socialvulnerability/socialvulnerability.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/tornadoepndamage/
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/tornadoepndamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27933 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/tornadoepndamage/tornadoepndamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/transportationrecovery/
--rw-r--r--   0 runner    (1001) docker     (121)     6125 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/WIPW.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7523 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9704 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/post_disaster_long_term_solution.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/test_transportation_recovery.py
--rw-r--r--   0 runner    (1001) docker     (121)    12173 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/transportationrecovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     5335 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/transportationrecovery/transportationrecoveryutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/waterfacilitydamage/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/waterfacilitydamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18751 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/waterfacilitydamage/waterfacilitydamage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/waterfacilityrestoration/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/waterfacilityrestoration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11590 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestoration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestorationutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/analyses/wfnfunctionality/
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/wfnfunctionality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9385 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/wfnfunctionality/wfnfunctionality.py
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/analyses/wfnfunctionality/wfnfunctionalityutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    10791 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/baseanalysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    15875 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    14839 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/dataservice.py
--rw-r--r--   0 runner    (1001) docker     (121)    10714 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    21993 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/dfr3service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/fragilityservice.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/globals.py
--rw-r--r--   0 runner    (1001) docker     (121)    33562 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/hazardservice.py
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.132713 pyincore-1.8.0/pyincore/models/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7239 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/dfr3curve.py
--rw-r--r--   0 runner    (1001) docker     (121)    15115 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/fragilitycurveset.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/mappingset.py
--rw-r--r--   0 runner    (1001) docker     (121)     6289 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/networkdataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3993 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/repaircurveset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4149 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/models/restorationcurveset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/networkdata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/repairservice.py
--rw-r--r--   0 runner    (1001) docker     (121)     2314 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/restorationservice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/spaceservice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.136713 pyincore-1.8.0/pyincore/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25095 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/analysisutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    10663 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/cgeoutputprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)    14253 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/dataprocessutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/datasetutil.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/evaluateexpression.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.136713 pyincore-1.8.0/pyincore/utils/expressioneval/
--rw-r--r--   0 runner    (1001) docker     (121)    25282 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/expressioneval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9186 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/geoutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    19587 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/networkutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    25388 2022-11-15 21:03:11.000000 pyincore-1.8.0/pyincore/utils/popdisloutputprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 21:03:47.124713 pyincore-1.8.0/pyincore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-11-15 21:03:47.000000 pyincore-1.8.0/pyincore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6469 2022-11-15 21:03:47.000000 pyincore-1.8.0/pyincore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 21:03:47.000000 pyincore-1.8.0/pyincore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-15 21:03:47.000000 pyincore-1.8.0/pyincore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-15 21:03:47.000000 pyincore-1.8.0/pyincore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 21:03:47.136713 pyincore-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-11-15 21:03:11.000000 pyincore-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.934340 pyincore-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-14 16:05:07.000000 pyincore-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-14 16:05:07.000000 pyincore-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-14 16:05:41.934340 pyincore-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-03-14 16:05:07.000000 pyincore-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.902340 pyincore-1.9.0/pyincore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.906340 pyincore-1.9.0/pyincore/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.906340 pyincore-1.9.0/pyincore/analyses/bridgedamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/bridgedamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/bridgedamage/bridgedamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/bridgedamage/bridgeutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.906340 pyincore-1.9.0/pyincore/analyses/buildingdamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingdamage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16054 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingdamage/buildingdamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingdamage/buildingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.906340 pyincore-1.9.0/pyincore/analyses/buildingeconloss/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingeconloss/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7397 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingeconloss/buildingeconloss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.910340 pyincore-1.9.0/pyincore/analyses/buildingfunctionality/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingfunctionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingfunctionality/buildingfunctionality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.910340 pyincore-1.9.0/pyincore/analyses/buildingportfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingportfolio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.910340 pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/BuildingDamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/BuildingData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38490 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/BuildingPortfolioRecoveryAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.910340 pyincore-1.9.0/pyincore/analyses/capitalshocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/capitalshocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/capitalshocks/capitalshocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.910340 pyincore-1.9.0/pyincore/analyses/combinedwindwavesurgebuildingdamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/combinedwindwavesurgebuildingdamage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9025 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/combinedwindwavesurgebuildingdamage/combinedwindwavesurgebuildingdamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.914340 pyincore-1.9.0/pyincore/analyses/combinedwindwavesurgebuildingloss/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/combinedwindwavesurgebuildingloss/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10683 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/combinedwindwavesurgebuildingloss/combinedwindwavesurgebuildingloss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.914340 pyincore-1.9.0/pyincore/analyses/cumulativebuildingdamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/cumulativebuildingdamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/cumulativebuildingdamage/cumulativebuildingdamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.914340 pyincore-1.9.0/pyincore/analyses/epfdamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epfdamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17794 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epfdamage/epfdamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epfdamage/epfutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.914340 pyincore-1.9.0/pyincore/analyses/epfrestoration/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epfrestoration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epfrestoration/epfrestoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epfrestoration/epfrestorationutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.918340 pyincore-1.9.0/pyincore/analyses/epnfunctionality/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epnfunctionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epnfunctionality/epnfunctionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/epnfunctionality/epnfunctionalityutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.918340 pyincore-1.9.0/pyincore/analyses/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/example/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3389 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/example/exampleanalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.918340 pyincore-1.9.0/pyincore/analyses/housingrecovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingrecovery/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17454 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingrecovery/housingrecovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingrecovery/housingrecoveryutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.918340 pyincore-1.9.0/pyincore/analyses/housingrecoverysequential/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingrecoverysequential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21479 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingrecoverysequential/housingrecoverysequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.918340 pyincore-1.9.0/pyincore/analyses/housingunitallocation/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingunitallocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/housingunitallocation/housingunitallocation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.922340 pyincore-1.9.0/pyincore/analyses/joplincge/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplincge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30316 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplincge/equationlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77981 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplincge/joplincge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplincge/outputfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.922340 pyincore-1.9.0/pyincore/analyses/joplinempiricalrestoration/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplinempiricalrestoration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8584 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplinempiricalrestoration/joplinempiricalrestoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/joplinempiricalrestoration/joplinempirrestor_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.922340 pyincore-1.9.0/pyincore/analyses/meandamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/meandamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/meandamage/meandamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.922340 pyincore-1.9.0/pyincore/analyses/montecarlofailureprobability/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/montecarlofailureprobability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/montecarlofailureprobability/montecarlofailureprobability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.922340 pyincore-1.9.0/pyincore/analyses/multiobjectiveretrofitoptimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/multiobjectiveretrofitoptimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74302 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/multiobjectiveretrofitoptimization/multiobjectiveretrofitoptimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/ncifunctionality/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/ncifunctionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20741 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/ncifunctionality/ncifunctionality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/nonstructbuildingdamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/nonstructbuildingdamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20366 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingdamage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/pipelinedamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinedamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinedamage/pipelinedamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/pipelinedamagerepairrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinedamagerepairrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18918 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinedamagerepairrate/pipelinedamagerepairrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinedamagerepairrate/pipelineutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/pipelinefunctionality/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinefunctionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinefunctionality/pipelinefunctionality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/pipelinerestoration/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinerestoration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/pipelinerestoration/pipelinerestoration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/populationdislocation/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/populationdislocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/populationdislocation/populationdislocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/populationdislocation/populationdislocationutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/residentialbuildingrecovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/residentialbuildingrecovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25752 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/residentialbuildingrecovery/residentialbuildingrecovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/roaddamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/roaddamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/roaddamage/roaddamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/saltlakecge/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/saltlakecge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/saltlakecge/equationlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/saltlakecge/outputfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88470 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/saltlakecge/saltlakecge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/saltlakecge/saltlakeoutput.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.926340 pyincore-1.9.0/pyincore/analyses/seasidecge/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/seasidecge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33512 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/seasidecge/equationlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84786 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/seasidecge/seasidecge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/analyses/socialvulnerability/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/socialvulnerability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/socialvulnerability/socialvulnerability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/analyses/tornadoepndamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/tornadoepndamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27933 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/tornadoepndamage/tornadoepndamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/analyses/transportationrecovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/WIPW.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/post_disaster_long_term_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/test_transportation_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/transportationrecovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/transportationrecovery/transportationrecoveryutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/analyses/waterfacilitydamage/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/waterfacilitydamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18751 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/waterfacilitydamage/waterfacilitydamage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/analyses/waterfacilityrestoration/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/waterfacilityrestoration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestoration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestorationutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/analyses/wfnfunctionality/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/wfnfunctionality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/wfnfunctionality/wfnfunctionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/analyses/wfnfunctionality/wfnfunctionalityutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/baseanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15875 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/dataservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21993 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/dfr3service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/fragilityservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33562 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/hazardservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.930340 pyincore-1.9.0/pyincore/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/dfr3curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/fragilitycurveset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/mappingset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6289 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/networkdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/repaircurveset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/models/restorationcurveset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/networkdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/repairservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/restorationservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/spaceservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.934340 pyincore-1.9.0/pyincore/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25095 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/analysisutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/cgeoutputprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/dataprocessutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/datasetutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/evaluateexpression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.934340 pyincore-1.9.0/pyincore/utils/expressioneval/
+-rw-r--r--   0 runner    (1001) docker     (123)    25282 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/expressioneval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/geoutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/hhrsoutputprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/networkutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25388 2023-03-14 16:05:07.000000 pyincore-1.9.0/pyincore/utils/popdisloutputprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.906340 pyincore-1.9.0/pyincore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-14 16:05:41.000000 pyincore-1.9.0/pyincore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-03-14 16:05:41.000000 pyincore-1.9.0/pyincore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 16:05:41.000000 pyincore-1.9.0/pyincore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-14 16:05:41.000000 pyincore-1.9.0/pyincore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-14 16:05:41.000000 pyincore-1.9.0/pyincore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 16:05:41.934340 pyincore-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-14 16:05:07.000000 pyincore-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 16:05:41.934340 pyincore-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-14 16:05:07.000000 pyincore-1.9.0/tests/test_format.py
```

### Comparing `pyincore-1.8.0/LICENSE` & `pyincore-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/PKG-INFO` & `pyincore-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyincore
-Version: 1.8.0
+Version: 1.9.0
 Summary: IN-CORE analysis tool python package
 Home-page: https://incore.ncsa.illinois.edu
 License: Mozilla Public License v2.0
 Project-URL: Bug Reports, https://github.com/IN-CORE/pyincore/issues
 Project-URL: Source, https://github.com/IN-CORE/pyincore
 Keywords: infrastructure,resilience,hazards,data discovery,IN-CORE,earthquake,tsunami,tornado,hurricane,dislocation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyincore-1.8.0/README.rst` & `pyincore-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/__init__.py` & `pyincore-1.9.0/pyincore/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pyincore.fragilityservice import FragilityService
 from pyincore.repairservice import RepairService
 from pyincore.restorationservice import RestorationService
 from pyincore.spaceservice import SpaceService
 from pyincore.utils.analysisutil import AnalysisUtil
 from pyincore.utils.popdisloutputprocess import PopDislOutputProcess
 from pyincore.utils.cgeoutputprocess import CGEOutputProcess
+from pyincore.utils.hhrsoutputprocess import HHRSOutputProcess
 from pyincore.dataset import Dataset, InventoryDataset, DamageRatioDataset
 from pyincore.models.fragilitycurveset import FragilityCurveSet
 from pyincore.models.repaircurveset import RepairCurveSet
 from pyincore.models.restorationcurveset import RestorationCurveSet
 from pyincore.models.dfr3curve import DFR3Curve
 from pyincore.models.mappingset import MappingSet
 from pyincore.models.mapping import Mapping
```

### Comparing `pyincore-1.8.0/pyincore/analyses/bridgedamage/bridgedamage.py` & `pyincore-1.9.0/pyincore/analyses/bridgedamage/bridgedamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/bridgedamage/bridgeutil.py` & `pyincore-1.9.0/pyincore/analyses/bridgedamage/bridgeutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/buildingdamage/buildingdamage.py` & `pyincore-1.9.0/pyincore/analyses/buildingdamage/buildingdamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/buildingdamage/buildingutil.py` & `pyincore-1.9.0/pyincore/analyses/buildingdamage/buildingutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/buildingeconloss/buildingeconloss.py` & `pyincore-1.9.0/pyincore/analyses/buildingeconloss/buildingeconloss.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,20 @@
         if self.infl_factor is None:
             self.infl_factor = 0.0
 
         # Building dataset
         bldg_set = self.get_input_dataset("buildings").get_inventory_reader()
 
         # Occupancy type of the exposure
-        occ_multiplier = self.get_input_dataset("occupancy_multiplier").get_csv_reader()
-        occ_mult_df = pd.DataFrame(occ_multiplier)
+        occ_multiplier = self.get_input_dataset("occupancy_multiplier")
+        if occ_multiplier is not None:
+            occ_multiplier = occ_multiplier.get_csv_reader()
+            occ_mult_df = pd.DataFrame(occ_multiplier)
+        else:
+            occ_mult_df = None
 
         try:
             prop_select = []
             for bldg_item in list(bldg_set):
                 guid = bldg_item["properties"]["guid"]
                 appr_bldg = bldg_item["properties"]["appr_bldg"]
                 year_built = bldg_item["properties"]["year_built"]
@@ -108,15 +112,15 @@
             # Occupancy multipliers are in percentages, convert to multiplication factors
             occ_mult_df["Multiplier"] = (occ_mult_df["Multiplier"].astype(float) / 100.0) + 1.0
 
             occ_mult_df = occ_mult_df.rename(columns={"Occupancy": "occ_type"})
             dmg_set_df = pd.merge(dmg_set_df, occ_mult_df, how="left", left_on="occ_type",
                                   right_on="occ_type", sort=True, copy=True)
         else:
-            dmg_set_df = dmg_set_df["Multiplier"] = 1.0
+            dmg_set_df["Multiplier"] = 1.0
 
         return dmg_set_df
 
     def get_spec(self):
         """Get specifications of the building damage analysis.
 
         Returns:
```

### Comparing `pyincore-1.8.0/pyincore/analyses/buildingfunctionality/buildingfunctionality.py` & `pyincore-1.9.0/pyincore/analyses/buildingfunctionality/buildingfunctionality.py`

 * *Files 15% similar despite different names*

```diff
@@ -104,19 +104,17 @@
 
         poles_dataset = self.get_input_dataset("poles_damage_mcs_samples")
         if poles_dataset is not None:
             poles_df = poles_dataset.get_dataframe_from_csv().set_index("guid")
         else:
             poles_df = None
 
-        # All three above needs to be present at the same time or none
-        if not all(epf is None for epf in [interdependency_dict, substations_df, poles_df]) \
-                and not all(epf is not None for epf in [interdependency_dict, substations_df, poles_df]):
-            raise ValueError("To consider electric power availability in the analysis, please provide pole damage "
-                             "samples, substation damage samples, and interdependency.")
+        if (poles_dataset is not None or substations_dataset is not None) and interdependency_dataset is None:
+            raise ValueError("Please provide interdependency table if pole or substation damage is "
+                             "considered in the building functionality calculation.")
 
         functionality_probabilities = []
         functionality_samples = []
         for building_guid in buildings_df.index:
             building_guid, sample, probability = self.functionality(building_guid, buildings_df, substations_df,
                                                                     poles_df,
                                                                     interdependency_dict)
@@ -164,38 +162,61 @@
             print(building_mc_samples)
             return {building_guid: -1}
 
         # if building is defined in the interdependency lookup table
         if interdependency is not None:
 
             if building_guid in interdependency.keys():
-                substations_mc_samples = substations.loc[interdependency[building_guid]["substations_guid"]]
-                poles_mc_samples = poles.loc[interdependency[building_guid]["poles_guid"]]
-
-                substation_list = []
-                try:
-                    substation_list = substations_mc_samples["failure"].split(",")
-                except IndexError:
-                    print("error with substations")
-                    print(interdependency[building_guid]["substations_guid"])
-                    return {building_guid: -1}
-
-                pole_list = []
-                try:
-                    pole_list = poles_mc_samples["failure"].split(",")
-                except IndexError:
-                    print("error with poles")
-                    print(interdependency[building_guid]["poles_guid"])
-                    return {building_guid: -1}
-
-                functionality_samples = [BuildingFunctionality._calc_functionality_samples(building_sample,
-                                                                                           substation_sample,
-                                                                                           pole_sample)
-                                         for building_sample, substation_sample, pole_sample in
-                                         zip(building_list, substation_list, pole_list)]
+                if substations is not None:
+                    substations_mc_samples = substations.loc[interdependency[building_guid]["substations_guid"]]
+                    substation_list = []
+                    try:
+                        substation_list = substations_mc_samples["failure"].split(",")
+                    except IndexError:
+                        print("error with substations")
+                        print(interdependency[building_guid]["substations_guid"])
+                        return {building_guid: -1}
+                else:
+                    substation_list = None
+
+                if poles is not None:
+                    poles_mc_samples = poles.loc[interdependency[building_guid]["poles_guid"]]
+                    pole_list = []
+                    try:
+                        pole_list = poles_mc_samples["failure"].split(",")
+                    except IndexError:
+                        print("error with poles")
+                        print(interdependency[building_guid]["poles_guid"])
+                        return {building_guid: -1}
+                else:
+                    pole_list = None
+
+                if substation_list is not None and pole_list is not None:
+                    functionality_samples = [BuildingFunctionality._calc_functionality_samples(building_sample,
+                                                                                               substation_sample,
+                                                                                               pole_sample)
+                                             for building_sample, substation_sample, pole_sample in
+                                             zip(building_list, substation_list, pole_list)]
+                elif substation_list is not None:
+                    functionality_samples = [BuildingFunctionality._calc_functionality_samples(building_sample,
+                                                                                               substation_sample,
+                                                                                               None)
+                                             for building_sample, substation_sample in
+                                             zip(building_list, substation_list)]
+                elif pole_list is not None:
+                    functionality_samples = [BuildingFunctionality._calc_functionality_samples(building_sample,
+                                                                                               None,
+                                                                                               pole_sample)
+                                             for building_sample, pole_sample in
+                                             zip(building_list, pole_list)]
+                else:
+                    functionality_samples = [BuildingFunctionality._calc_functionality_samples(building_sample,
+                                                                                               None,
+                                                                                               None)
+                                             for building_sample in building_list]
                 probability = BuildingFunctionality._calc_functionality_probability(functionality_samples)
                 return building_guid, ",".join([str(sample) for sample in functionality_samples]), probability
 
             else:
                 return building_guid, "NA", "NA"
 
         # else if only building MC failure is available
@@ -208,16 +229,16 @@
     @staticmethod
     def _calc_functionality_samples(building_sample, substation_sample=None, pole_sample=None):
         """ This function is subject to change. For now, buildings have a 1-to-1 relationship with
         substations and poles, so it suffices to check that the poles and substations are up.
 
         Args:
             building_sample (str): Monte Carlo samples of building functionality.
-            substation_sample (str): Monte Carlo samples of substation functionality.
-            pole_sample (str): Monte Carlo samples of pole functionality.
+            substation_sample (str|None): Monte Carlo samples of substation functionality.
+            pole_sample (str|None): Monte Carlo samples of pole functionality.
 
         Returns:
             int: 1 if building is functional, 0 otherwise
 
         """
         if building_sample == "1" and (substation_sample == "1" or substation_sample is None) \
                 and (pole_sample == "1" or pole_sample is None):
```

### Comparing `pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/BuildingData.py` & `pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/BuildingData.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/buildingportfolio/recovery/BuildingPortfolioRecoveryAnalysis.py` & `pyincore-1.9.0/pyincore/analyses/buildingportfolio/recovery/BuildingPortfolioRecoveryAnalysis.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/capitalshocks/capitalshocks.py` & `pyincore-1.9.0/pyincore/analyses/capitalshocks/capitalshocks.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/cumulativebuildingdamage/cumulativebuildingdamage.py` & `pyincore-1.9.0/pyincore/analyses/cumulativebuildingdamage/cumulativebuildingdamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/epfdamage/epfdamage.py` & `pyincore-1.9.0/pyincore/analyses/epfdamage/epfdamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/epfdamage/epfutil.py` & `pyincore-1.9.0/pyincore/analyses/epfdamage/epfutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/epfrestoration/epfrestoration.py` & `pyincore-1.9.0/pyincore/analyses/epfrestoration/epfrestoration.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/epfrestoration/epfrestorationutil.py` & `pyincore-1.9.0/pyincore/analyses/epfrestoration/epfrestorationutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/epnfunctionality/epnfunctionality.py` & `pyincore-1.9.0/pyincore/analyses/epnfunctionality/epnfunctionality.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/epnfunctionality/epnfunctionalityutil.py` & `pyincore-1.9.0/pyincore/analyses/epnfunctionality/epnfunctionalityutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/example/exampleanalysis.py` & `pyincore-1.9.0/pyincore/analyses/example/exampleanalysis.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/housingrecovery/housingrecovery.py` & `pyincore-1.9.0/pyincore/analyses/housingrecovery/housingrecovery.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/housingrecovery/housingrecoveryutil.py` & `pyincore-1.9.0/pyincore/analyses/housingrecovery/housingrecoveryutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/housingrecoverysequential/housingrecoverysequential.py` & `pyincore-1.9.0/pyincore/analyses/housingrecoverysequential/housingrecoverysequential.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright (c) 2021 University of Illinois and others. All rights reserved.
 #
 # This program and the accompanying materials are made available under the
 # terms of the Mozilla Public License v2.0 which accompanies this distribution,
 # and is available at https://www.mozilla.org/en-US/MPL/2.0/
-from pyincore import BaseAnalysis
+from pyincore import BaseAnalysis, AnalysisUtil
 
 import numpy as np
 import pandas as pd
+import concurrent.futures
+from itertools import repeat
 
 
 class HousingRecoverySequential(BaseAnalysis):
     """
     This analysis computes the series of household recovery states given a population
     dislocation dataset, a transition probability matrix (TPM) and an initial state vector.
 
@@ -87,27 +89,23 @@
     def run(self):
         """Execute the HHRS analysis using parameters and input data."""
         # Read parameters
         t_delta = self.get_parameter('t_delta')
         t_final = self.get_parameter('t_final')
 
         # Load population block data from IN-CORE
-        pop_dis_selectors = ['guid', 'huid', 'blockid',
-                             'numprec', 'race', 'hispan',
-                             'ownershp', 'randincome', 'dislocated']
+        pop_dis_selectors = ['guid', 'huid', 'blockid', 'race', 'hispan', 'ownershp', 'dislocated']
         households_csv = self.get_input_dataset('population_dislocation_block').get_csv_reader()
         households_df = (pd.DataFrame(households_csv))[pop_dis_selectors]
 
         # Perform  conversions across the dataset from object type into the appropriate type
         households_df['blockid'] = households_df['blockid'].astype('int64')
-        households_df['numprec'] = households_df['numprec'].astype(int)
         households_df['race'] = pd.to_numeric(households_df['race'])
         households_df['hispan'] = pd.to_numeric(households_df['hispan'])
         households_df['ownershp'] = pd.to_numeric(households_df['ownershp'])
-        households_df['randincome'] = pd.to_numeric(households_df['randincome'])
         households_df['dislocated'] = (households_df['dislocated'] == 'True')
 
         # Load the transition probability matrix from IN-CORE
         tpm_csv = self.get_input_dataset("tpm").get_csv_reader()
         tpm = pd.DataFrame(list(tpm_csv))
 
         # Make sure all columns have numeric values
@@ -118,27 +116,76 @@
         tpm[:, 0] = np.around(tpm[:, 0], 3)
 
         # Load the initial stage probability vector
         initial_prob_csv = self.get_input_dataset("initial_stage_probabilities").get_csv_reader()
         initial_prob = pd.DataFrame(list(initial_prob_csv))
         initial_prob['value'] = pd.to_numeric(initial_prob['value'])
 
+        # Obtain the number of CPUs (cores) to execute the analysis with
+        user_defined_cpu = 4
+
+        if not self.get_parameter("num_cpu") is None and self.get_parameter("num_cpu") > 0:
+            user_defined_cpu = self.get_parameter("num_cpu")
+
+        num_workers = AnalysisUtil.determine_parallelism_locally(self, len(households_df), user_defined_cpu)
+
+        # Chop dataset into `num_size` chunks
+        max_chunk_size = int(np.ceil(len(households_df)/num_workers))
+
+        households_df_list = list(
+            map(lambda x: households_df[x * max_chunk_size:x * max_chunk_size + max_chunk_size],
+                list(range(num_workers)))
+        )
+
         # Run the analysis
-        self.housing_serial_recovery_model(t_delta, t_final, tpm, initial_prob, households_df)
+        result = self.hhrs_concurrent_future(self.housing_serial_recovery_model,
+                                                 num_workers,
+                                                 households_df_list,
+                                                 repeat(t_delta),
+                                                 repeat(t_final),
+                                                 repeat(tpm),
+                                                 repeat(initial_prob))
+
+        result_name = self.get_parameter("result_name")
+        self.set_result_csv_data("ds_result", result, name=result_name, source="dataframe")
+
+        return True
+
+    def hhrs_concurrent_future(self, function_name, parallelism, *args):
+        """Utilizes concurrent.future module.
+
+        Args:
+            function_name (function): The function to be parallelized.
+            parallelism (int): Number of workers in parallelization.
+            *args: All the arguments in order to pass into parameter function_name.
+
+        Returns:
+            pd.DataFrame: outcome DataFrame containing the results from the concurrent function.
+
+        """
+        output_ds = pd.DataFrame()
+
+        with concurrent.futures.ProcessPoolExecutor(max_workers=parallelism) as executor:
+            for ret in executor.map(function_name, *args):
+                output_ds = pd.concat([output_ds, ret], ignore_index=True)
 
-    def housing_serial_recovery_model(self, t_delta, t_final, tpm, initial_prob, households_df):
+        return output_ds
+
+    def housing_serial_recovery_model(self, households_df, t_delta, t_final, tpm, initial_prob):
         """Performs the computation of the model as indicated in Sutley and Hamide (2020).
 
         Args:
+            households_df (pd.DataFrame): Households with population dislocation data.
             t_delta (float): Time step size.
             t_final (float): Final time.
             tpm (np.Array): Transition probability matrix.
             initial_prob (pd.DataFrame): Initial probability Markov vector.
-            households_df (pd.DataFrame): Households with population dislocation data.
 
+        Returns:
+            pd.DataFrame: outcome of the HHRS model for a given household dataset.
         """
         seed = self.get_parameter('seed')
         rng = np.random.RandomState(seed)
         sv_result = self.get_input_dataset("sv_result").get_dataframe_from_csv(low_memory=False)
         # turn fips code to string for ease of matching
         sv_result["FIPS"] = sv_result["FIPS"].astype(str)
 
@@ -266,16 +313,15 @@
         result['Zone'] = households_df['Zone']
         result['SV'] = sv_scores
         column_names = [str(i) for i in range(1, stages + 1)]
 
         for i, c in enumerate(column_names):
             result[c] = markov_stages[i]
 
-        result_name = self.get_parameter("result_name")
-        self.set_result_csv_data("ds_result", result, name=result_name, source="dataframe")
+        return result
 
     @staticmethod
     def compute_social_vulnerability_zones(sv_result, households_df):
         """
         Compute the social vulnerability score based on dislocation attributes. Updates the dislocation dataset
         by adding a new `Zone` column and removing values with missing Zone.
 
@@ -348,14 +394,15 @@
         Returns:
             int: Number of regressions between a given time window.
 
         """
         regressions = 0
 
         # Check the previous timesteps between [lower, upper] prior to the current timestep.
+
         for t in range(lower, upper):
             if markov_stages[t][household] < markov_stages[t - 1][household]:
                 regressions += 1
 
         return regressions
 
     def get_spec(self):
@@ -389,14 +436,20 @@
                 },
                 {
                     'id': 'seed',
                     'required': False,
                     'description': 'Seed to ensure replication of the Markov Chain path'
                                    'in connection with Population Dislocation.',
                     'type': int
+                },
+                {
+                    'id': 'num_cpu',
+                    'required': False,
+                    'description': 'If using parallel execution, the number of cpus to request',
+                    'type': int
                 }
             ],
             'input_datasets': [
                 {
                     'id': 'population_dislocation_block',
                     'required': True,
                     'description': 'A csv file with population dislocation result '
@@ -412,20 +465,14 @@
                 },
                 {
                     'id': 'initial_stage_probabilities',
                     'required': True,
                     'description': 'initial mass probability function for stage 0 of the Markov Chain',
                     'type': 'incore:houseRecInitialStageProbability'
                 },
-                {
-                    'id': 'initial_stage_probabilities',
-                    'required': True,
-                    'description': 'initial mass probability function for stage 0 of the Markov Chain',
-                    'type': 'incore:houseRecInitialStageProbability'
-                },
                 {
                     'id': 'sv_result',
                     'required': True,
                     'description': 'A csv file with zones containing demographic factors'
                                    'qualified by a social vulnerability score',
                     'type': 'incore:socialVulnerabilityScore'
                 }
```

### Comparing `pyincore-1.8.0/pyincore/analyses/housingunitallocation/housingunitallocation.py` & `pyincore-1.9.0/pyincore/analyses/housingunitallocation/housingunitallocation.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/joplincge/equationlib.py` & `pyincore-1.9.0/pyincore/analyses/joplincge/equationlib.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/joplincge/joplincge.py` & `pyincore-1.9.0/pyincore/analyses/joplincge/joplincge.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,86 +55,86 @@
             'input_datasets': [
                 {
                     'id': 'SAM',
                     'required': True,
                     'description': 'Social accounting matrix (SAM) contains data for firms, '
                                    'households and government which are organized in a way to '
                                    'represent the interactions of all three entities in a typical economy.',
-                    'type': ['incore:JoplinCGEsam']
+                    'type': ['incore:CGEsam']
                 },
                 {
                     'id': 'BB',
                     'required': True,
                     'description': 'BB is a matrix which describes how investment in physical infrastructure is'
                                    ' transformed into functioning capital such as commercial and residential buildings.'
                                    ' These data are collected from the Bureau of Economic Analysis (BEA).',
-                    'type': ['incore:JoplinCGEbb']
+                    'type': ['incore:CGEbb']
                 },
                 {
                     'id': 'IOUT',
                     'required': True,
                     'description': 'IOUT is a matrix that describes the transfer of tax revenue collected by the local'
                                    ' government to help finance local government expenditures.',
-                    'type': ['incore:JoplinCGEiout']
+                    'type': ['incore:CGEiout']
                 },
                 {
                     'id': 'MISC',
                     'required': True,
                     'description': 'MISC is the name of a file that contains data for commercial sector employment'
                                    ' and physical capital. It also contains data for the number of households and'
                                    ' working households in the economy.',
-                    'type': ['incore:JoplinCGEmisc']
+                    'type': ['incore:CGEmisc']
                 },
                 {
                     'id': 'MISCH',
                     'required': True,
                     'description': 'MISCH is a file that contains elasticities for the supply of labor with'
                                    ' respect to paying income taxes.',
-                    'type': ['incore:JoplinCGEmisch']
+                    'type': ['incore:CGEmisch']
                 },
                 {
                     'id': 'LANDCAP',
                     'required': True,
                     'description': 'LANDCAP contains information regarding elasticity values for the response of '
                                    'changes in the price of physical capital with respect to the supply of investment.',
-                    'type': ['incore:JoplinCGElandcap']
+                    'type': ['incore:CGElandcap']
                 },
                 {
                     'id': 'EMPLOY',
                     'required': True,
                     'description': 'EMPLOY is a table name containing data for commercial sector employment.',
-                    'type': ['incore:JoplinCGEemploy']
+                    'type': ['incore:CGEemploy']
                 },
                 {
                     'id': 'IGTD',
                     'required': True,
                     'description': 'IGTD variable represents a matrix describing the transfer of taxes collected'
                                    ' to a variable which permits governments to spend the tax revenue on workers and'
                                    ' intermediate inputs.',
-                    'type': ['incore:JoplinCGEigtd']
+                    'type': ['incore:CGEigtd']
                 },
                 {
                     'id': 'TAUFF',
                     'required': True,
                     'description': 'TAUFF represents social security tax rates',
-                    'type': ['incore:JoplinCGEtauff']
+                    'type': ['incore:CGEtauff']
                 },
                 {
                     'id': 'JOBCR',
                     'required': True,
                     'description': 'JOBCR is a matrix describing the supply of workers'
                                    ' coming from each household group in the economy.',
-                    'type': ['incore:JoplinCGEjobcr']
+                    'type': ['incore:CGEjobcr']
                 },
                 {
                     'id': 'OUTCR',
                     'required': True,
                     'description': 'OUTCR is a matrix describing the number of workers who'
                                    ' live in Joplin but commute outside of town to work.',
-                    'type': ['incore:JoplinCGEoutcr']
+                    'type': ['incore:CGEoutcr']
                 },
                 {
                     'id': 'sector_shocks',
                     'required': True,
                     'description': 'Aggregation of building functionality states to capital shocks per sector',
                     'type': ['incore:capitalShocks']
                 }
```

### Comparing `pyincore-1.8.0/pyincore/analyses/joplincge/outputfunctions.py` & `pyincore-1.9.0/pyincore/analyses/joplincge/outputfunctions.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/joplinempiricalrestoration/joplinempiricalrestoration.py` & `pyincore-1.9.0/pyincore/analyses/joplinempiricalrestoration/joplinempiricalrestoration.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/joplinempiricalrestoration/joplinempirrestor_util.py` & `pyincore-1.9.0/pyincore/analyses/joplinempiricalrestoration/joplinempirrestor_util.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/meandamage/meandamage.py` & `pyincore-1.9.0/pyincore/analyses/meandamage/meandamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/montecarlofailureprobability/montecarlofailureprobability.py` & `pyincore-1.9.0/pyincore/analyses/montecarlofailureprobability/montecarlofailureprobability.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/multiobjectiveretrofitoptimization/multiobjectiveretrofitoptimization.py` & `pyincore-1.9.0/pyincore/analyses/multiobjectiveretrofitoptimization/multiobjectiveretrofitoptimization.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/ncifunctionality/ncifunctionality.py` & `pyincore-1.9.0/pyincore/analyses/ncifunctionality/ncifunctionality.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingdamage.py` & `pyincore-1.9.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingdamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingutil.py` & `pyincore-1.9.0/pyincore/analyses/nonstructbuildingdamage/nonstructbuildingutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/pipelinedamage/pipelinedamage.py` & `pyincore-1.9.0/pyincore/analyses/pipelinedamage/pipelinedamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/pipelinedamagerepairrate/pipelinedamagerepairrate.py` & `pyincore-1.9.0/pyincore/analyses/pipelinedamagerepairrate/pipelinedamagerepairrate.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/pipelinedamagerepairrate/pipelineutil.py` & `pyincore-1.9.0/pyincore/analyses/pipelinedamagerepairrate/pipelineutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/pipelinefunctionality/pipelinefunctionality.py` & `pyincore-1.9.0/pyincore/analyses/pipelinefunctionality/pipelinefunctionality.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/pipelinerestoration/pipelinerestoration.py` & `pyincore-1.9.0/pyincore/analyses/pipelinerestoration/pipelinerestoration.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/populationdislocation/populationdislocation.py` & `pyincore-1.9.0/pyincore/analyses/populationdislocation/populationdislocation.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/populationdislocation/populationdislocationutil.py` & `pyincore-1.9.0/pyincore/analyses/populationdislocation/populationdislocationutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/residentialbuildingrecovery/residentialbuildingrecovery.py` & `pyincore-1.9.0/pyincore/analyses/residentialbuildingrecovery/residentialbuildingrecovery.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/roaddamage/roaddamage.py` & `pyincore-1.9.0/pyincore/analyses/roaddamage/roaddamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/seasidecge/equationlib.py` & `pyincore-1.9.0/pyincore/analyses/seasidecge/equationlib.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/seasidecge/seasidecge.py` & `pyincore-1.9.0/pyincore/analyses/seasidecge/seasidecge.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/socialvulnerability/socialvulnerability.py` & `pyincore-1.9.0/pyincore/analyses/socialvulnerability/socialvulnerability.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/tornadoepndamage/tornadoepndamage.py` & `pyincore-1.9.0/pyincore/analyses/tornadoepndamage/tornadoepndamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/WIPW.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/WIPW.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/__init__.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/nsga2.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/post_disaster_long_term_solution.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/post_disaster_long_term_solution.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/test_transportation_recovery.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/test_transportation_recovery.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/transportationrecovery.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/transportationrecovery.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/transportationrecovery/transportationrecoveryutil.py` & `pyincore-1.9.0/pyincore/analyses/transportationrecovery/transportationrecoveryutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/waterfacilitydamage/waterfacilitydamage.py` & `pyincore-1.9.0/pyincore/analyses/waterfacilitydamage/waterfacilitydamage.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestoration.py` & `pyincore-1.9.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestoration.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestorationutil.py` & `pyincore-1.9.0/pyincore/analyses/waterfacilityrestoration/waterfacilityrestorationutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/wfnfunctionality/wfnfunctionality.py` & `pyincore-1.9.0/pyincore/analyses/wfnfunctionality/wfnfunctionality.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/analyses/wfnfunctionality/wfnfunctionalityutil.py` & `pyincore-1.9.0/pyincore/analyses/wfnfunctionality/wfnfunctionalityutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/baseanalysis.py` & `pyincore-1.9.0/pyincore/baseanalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,28 +237,28 @@
         if not (dataset.data_type is dataset_spec['type']):
             is_valid = False
             err_msg = 'dataset type does not match'
         return is_valid, err_msg
 
     """ convenience function(s) for setting result data as a csv """
 
-    def set_result_csv_data(self, result_id, result_data, name, source='file'):
+    def set_result_csv_data(self, result_id, result_data, name, source='file', index=False):
         if name is None:
             name = self.spec["name"] + "-result"
 
         if not name.endswith(".csv"):
             name = name + ".csv"
 
         dataset_type = self.output_datasets[result_id]["spec"]["type"]
         dataset = None
 
         if source == 'file':
             dataset = Dataset.from_csv_data(result_data, name, dataset_type)
         elif source == 'dataframe':
-            dataset = Dataset.from_dataframe(result_data, name, dataset_type)
+            dataset = Dataset.from_dataframe(result_data, name, dataset_type, index)
 
         self.set_output_dataset(result_id, dataset)
 
     def set_result_json_data(self, result_id, result_data, name, source='file'):
         if name is None:
             name = self.spec["name"] + "-result"
```

### Comparing `pyincore-1.8.0/pyincore/client.py` & `pyincore-1.9.0/pyincore/client.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/dataservice.py` & `pyincore-1.9.0/pyincore/dataservice.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/dataset.py` & `pyincore-1.9.0/pyincore/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,27 +104,28 @@
                     "fileDescriptors": [],
                     "id": file_path}
         instance = cls(metadata)
         instance.local_file_path = file_path
         return instance
 
     @classmethod
-    def from_dataframe(cls, dataframe, name, data_type):
+    def from_dataframe(cls, dataframe, name, data_type, index=False):
         """Get Dataset from Panda's DataFrame.
 
         Args:
             dataframe (obj): Panda's DataFrame.
             name (str): filename.
             data_type (str): Incore data type, e.g. incore:xxxx or ergo:xxxx
+            index (bool): Store the index column
 
         Returns:
             obj: Dataset from file.
 
         """
-        dataframe.to_csv(name, index=False)
+        dataframe.to_csv(name, index=index)
         return Dataset.from_file(name, data_type)
 
     @classmethod
     def from_csv_data(cls, result_data, name, data_type):
         """Get Dataset from CSV data.
 
         Args:
```

### Comparing `pyincore-1.8.0/pyincore/dfr3service.py` & `pyincore-1.9.0/pyincore/dfr3service.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/fragilityservice.py` & `pyincore-1.9.0/pyincore/fragilityservice.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/globals.py` & `pyincore-1.9.0/pyincore/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from logging import config as logging_config
 
 import logging
 import os
 import shutil
 
-PACKAGE_VERSION = "1.8.0"
+PACKAGE_VERSION = "1.9.0"
 
 INCORE_API_PROD_URL = "https://incore.ncsa.illinois.edu"
 INCORE_API_DEV_URL = "https://incore-dev.ncsa.illinois.edu"
 
 KEYCLOAK_AUTH_PATH = "/auth/realms/In-core/protocol/openid-connect/token"
 KEYCLOAK_USERINFO_PATH = "/auth/realms/In-core/protocol/openid-connect/userinfo"
 CLIENT_ID = "react-auth"
```

### Comparing `pyincore-1.8.0/pyincore/hazardservice.py` & `pyincore-1.9.0/pyincore/hazardservice.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/logging.ini` & `pyincore-1.9.0/pyincore/logging.ini`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/dfr3curve.py` & `pyincore-1.9.0/pyincore/models/dfr3curve.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/fragilitycurveset.py` & `pyincore-1.9.0/pyincore/models/fragilitycurveset.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/mapping.py` & `pyincore-1.9.0/pyincore/models/mapping.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/mappingset.py` & `pyincore-1.9.0/pyincore/models/mappingset.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/networkdataset.py` & `pyincore-1.9.0/pyincore/models/networkdataset.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/repaircurveset.py` & `pyincore-1.9.0/pyincore/models/repaircurveset.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/models/restorationcurveset.py` & `pyincore-1.9.0/pyincore/models/restorationcurveset.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/networkdata.py` & `pyincore-1.9.0/pyincore/networkdata.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/repairservice.py` & `pyincore-1.9.0/pyincore/repairservice.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/restorationservice.py` & `pyincore-1.9.0/pyincore/restorationservice.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/analysisutil.py` & `pyincore-1.9.0/pyincore/utils/analysisutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/cgeoutputprocess.py` & `pyincore-1.9.0/pyincore/utils/cgeoutputprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,34 +8,35 @@
 import pandas as pd
 
 
 class CGEOutputProcess:
     """This class converts csv results outputs of Joplin CGE analysis to json format."""
 
     @staticmethod
-    def get_cge_household_count(household_count, household_count_path=None, filename_json=None):
+    def get_cge_household_count(household_count, household_count_path=None, filename_json=None,
+                                income_categories=("HH1", "HH2", "HH3", "HH4", "HH5")):
         """Calculate income results from the output files of the Joplin CGE analysis and convert the results
         to json format.
         {
             "beforeEvent": {"HH1": 3611, "HH2": 5997.0, "HH3": 7544.1, "HH4": 2394.1, "HH5": 793.0},
             "afterEvent": {"HH1": 3588, "HH2": 5929.8, "HH3": 7324.1, "HH4": 2207.5, "HH5": 766.4},
             "%_change": {"HH1": -0.6369, "HH2": -1.1, "HH3": -2.92, "HH4": -7.8, "HH5": -3.35}
         }
 
         Args:
             household_count (obj): IN-CORE dataset for CGE household count result.
             household_count_path (obj): A fallback for the case that household count object of CGE is not provided.
                  For example a user wants to directly pass in csv files, a path to CGE household count result.
             filename_json (str): Path and name to save json output file in. E.g "cge_total_household_count.json"
+            income_categories (list): A list of income categories to partition the data
 
         Returns:
             obj: CGE total household count. A JSON of the total household count results ordered by category.
 
         """
-        income_categories = ["HH1", "HH2", "HH3", "HH4", "HH5"]
 
         if household_count_path:
             household_group_count = pd.read_csv(household_count_path)
         else:
             household_group_count = household_count.get_dataframe_from_csv()
 
         before_values = household_group_count["HH0"]
@@ -52,39 +53,40 @@
             else:
                 pct_change[income_categories[i]] = None
 
         cge_total_household_count = {"beforeEvent": before_event, "afterEvent": after_event, "%_change": pct_change}
 
         if filename_json:
             with open(filename_json, "w") as outfile:
-                json.dump(cge_total_household_count, outfile)
+                json.dump(cge_total_household_count, outfile, indent=2)
         # Serializing json
         return json.dumps(cge_total_household_count)
 
     @staticmethod
-    def get_cge_gross_income(gross_income, gross_income_path=None, filename_json=None):
+    def get_cge_gross_income(gross_income, gross_income_path=None, filename_json=None,
+                             income_categories=("HH1", "HH2", "HH3", "HH4", "HH5")):
         """Calculate household gross income results from the output files of the Joplin CGE analysis
         and convert the results to json format.
         {
             "beforeEvent": {"HH1": 13, "HH2": 153.5, "HH3": 453.1, "HH4": 438.9, "HH5": 125.0},
             "afterEvent": {"HH1": 13, "HH2": 152.5, "HH3": 445.6, "HH4": 432.9, "HH5": 124.5},
             "%_change": {"HH1": -0, "HH2": -x.x, "HH3": -x.x, "HH4": -x.x, "HH5": -x.x}
         }
 
         Args:
             gross_income (obj): IN-CORE dataset for CGE household gross income result.
             gross_income_path (obj): A fallback for the case that gross_income object of CGE is not provided.
                  For example a user wants to directly pass in csv files, a path to CGE gross income result.
             filename_json (str): Path and name to save json output file in. E.g "cge_total_house_income.json"
+            income_categories (list): A list of income categories to partition the data
 
         Returns:
             obj: CGE total house income. A JSON of the total household income results ordered by category.
 
         """
-        income_categories = ["HH1", "HH2", "HH3", "HH4", "HH5"]
 
         if gross_income_path:
             household_income = pd.read_csv(gross_income_path)
         else:
             household_income = gross_income.get_dataframe_from_csv()
 
         before_values = household_income["Y0"]
@@ -101,22 +103,21 @@
             else:
                 pct_change[income_categories[i]] = None
 
         cge_total_household_income = {"beforeEvent": before_event, "afterEvent": after_event, "%_change": pct_change}
 
         if filename_json:
             with open(filename_json, "w") as outfile:
-                json.dump(cge_total_household_income, outfile)
+                json.dump(cge_total_household_income, outfile, indent=2)
         # Serializing json
         return json.dumps(cge_total_household_income)
 
     @staticmethod
-    def get_cge_employment(pre_demand, post_demand,
-                           pre_demand_path=None, post_demand_path=None,
-                           filename_json=None):
+    def get_cge_employment(pre_demand, post_demand, pre_demand_path=None, post_demand_path=None,
+                           filename_json=None, demand_categories=("GOODS", "TRADE", "OTHER")):
         """Calculate employment results from the output files of the Joplin CGE analysis and convert the results
         to json format. The value is a sum of L1, L2 and L3 Labor groups numbers.
         {
             "afterEvent": {
                 "Goods": 6680,
                 "Trade": 8876,
                 "Other": 23767
@@ -131,34 +132,30 @@
             pre_demand_path (obj): A fallback for the case that pre_disaster_demand_factor_path object
                 of CGE is not provided. For example a user wants to directly pass in csv files, a path to CGE
                 household count result.
             post_demand_path (obj): A fallback for the case that post_disaster_demand_factor_path object
                 of CGE is not provided. For example a user wants to directly pass in csv files, a path to CGE
                 household count result.
             filename_json (str): Path and name to save json output file in. E.g "cge_employment.json"
+            demand_categories (list): demand categories to partition data with.
 
         Returns:
             obj: CGE total employment. A JSON of the employment results ordered by category.
 
         """
-        demand_categories = ["Goods", "Trade", "Other"]
 
         if pre_demand_path and post_demand_path:
             pre_disaster_demand = pd.read_csv(pre_demand_path)
             post_disaster_demand = pd.read_csv(post_demand_path)
         else:
             pre_disaster_demand = pre_demand.get_dataframe_from_csv()
             post_disaster_demand = post_demand.get_dataframe_from_csv()
 
-        before_values = [pre_disaster_demand["GOODS"].sum(),
-                         pre_disaster_demand["TRADE"].sum(),
-                         pre_disaster_demand["OTHER"].sum()]
-        after_values = [post_disaster_demand["GOODS"].sum(),
-                        post_disaster_demand["TRADE"].sum(),
-                        post_disaster_demand["OTHER"].sum()]
+        before_values = [pre_disaster_demand[demand_category].sum() for demand_category in demand_categories]
+        after_values = [post_disaster_demand[demand_category].sum() for demand_category in demand_categories]
 
         before_event = {}
         after_event = {}
         pct_change = {}
         for i in range(len(demand_categories)):
             before_event[demand_categories[i]] = before_values[i]
             after_event[demand_categories[i]] = after_values[i]
@@ -167,42 +164,44 @@
             else:
                 pct_change[demand_categories[i]] = None
 
         cge_employment = {"beforeEvent": before_event, "afterEvent": after_event, "%_change": pct_change}
 
         if filename_json:
             with open(filename_json, "w") as outfile:
-                json.dump(cge_employment, outfile)
+                json.dump(cge_employment, outfile, indent=2)
         # Serializing json
         return json.dumps(cge_employment)
 
     @staticmethod
-    def get_cge_domestic_supply(domestic_supply, domestic_supply_path=None, filename_json=None):
+    def get_cge_domestic_supply(domestic_supply, domestic_supply_path=None, filename_json=None,
+                                supply_categories=("Goods", "Trade", "Other", "HS1", "HS2", "HS3")):
         """Calculate domestic supply results from the output files of the Joplin CGE analysis and convert the results
         to json format.
         {
             "afterEvent": {"Goods": 662.3, "Trade": 209.0, "Other": 254.1,
                            "HS1": 22.0, "HS2": 1337.1, "HS3": 466.2},
             "beforeEvent": {"Goods": 662.3, "Trade": 209.0, "Other": 254.1,
                             "HS1": 22.0, "HS2": 1337.1, "HS3": 466.2},
             "%_change": {"Goods": -1.1, "Trade":  -1.1, "Other":  -1.1,
                             "HS1":  -1.1, "HS2":  -1.1, "HS3":  -1.1}
         }
 
         Args:
             domestic_supply (obj): IN-CORE dataset for CGE domestic supply result.
+            supply_categories (list): demand categories to partition data with.
             domestic_supply_path (obj): A fallback for the case that domestic supply object of CGE is not provided.
                  For example a user wants to directly pass in csv files, a path to CGE household count result.
             filename_json (str): Path and name to save json output file in. E.g "cge_domestic_supply"
 
         Returns:
             obj: CGE total domestic supply. A JSON of the total domestic supply results ordered by category.
 
         """
-        supply_categories = ["Goods", "Trade", "Other", "HS1", "HS2", "HS3"]
+
         if domestic_supply_path:
             sector_supply = pd.read_csv(domestic_supply_path)
         else:
             sector_supply = domestic_supply.get_dataframe_from_csv()
 
         before_values = sector_supply["DS0"]
         after_values = sector_supply["DSL"]
@@ -218,10 +217,10 @@
             else:
                 pct_change[supply_categories[i]] = None
 
         cge_domestic_supply = {"beforeEvent": before_event, "afterEvent": after_event, "%_change": pct_change}
 
         if filename_json:
             with open(filename_json, "w") as outfile:
-                json.dump(cge_domestic_supply, outfile)
+                json.dump(cge_domestic_supply, outfile, indent=2)
         # Serializing json
         return json.dumps(cge_domestic_supply)
```

### Comparing `pyincore-1.8.0/pyincore/utils/dataprocessutil.py` & `pyincore-1.9.0/pyincore/utils/dataprocessutil.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 
 class DataProcessUtil:
 
     @staticmethod
     def get_mapped_result_from_analysis(client, inventory_id: str, dmg_result_dataset,
                                         bldg_func_dataset, archetype_mapping_id: str,
-                                        groupby_col_name: str = "max_state"):
+                                        groupby_col_name: str = "max_state", arch_col='archetype'
+                                        ):
         """Use this if you want to load results directly from the output files of the analysis, than storing the results
         to data service and loading from there using ids.
         It takes the static inputs: inventory & archetypes as dataset ids. The result inputs are taken as
         Dataset class objects, which are created by reading the output result files.
 
         Args:
             client: Service client with authentication info
@@ -29,47 +30,49 @@
             bldg_func_dataset: Incore dataset for building func dataset
             archetype_mapping_id: Mapping id dataset for archetype
 
         Returns:
             dmg_ret_json: JSON of the damage state results ordered by cluster and category.
             func_ret_json: JSON of the building functionality results ordered by cluster and category.
             mapped_df: Dataframe of max damage state
+            arch_col: column name for the archetype to perform the merge
 
         """
         bldg_inv = Dataset.from_data_service(inventory_id, DataService(client))
         inventory = pd.DataFrame(gpd.read_file(bldg_inv.local_file_path))
 
         dmg_result = dmg_result_dataset.get_dataframe_from_csv()
 
         bldg_func_df = bldg_func_dataset.get_dataframe_from_csv()
         bldg_func_df.rename(columns={'building_guid': 'guid'}, inplace=True)
 
         arch_mapping = Dataset.from_data_service(archetype_mapping_id, DataService(client)).get_dataframe_from_csv()
 
         max_state_df = DataProcessUtil.get_max_damage_state(dmg_result)
         dmg_ret_json = DataProcessUtil.create_mapped_dmg_result(inventory, max_state_df, arch_mapping,
-                                                                groupby_col_name)
-        func_ret_json = DataProcessUtil.create_mapped_func_result(inventory, bldg_func_df, arch_mapping)
+                                                                groupby_col_name, arch_col)
+        func_ret_json = DataProcessUtil.create_mapped_func_result(inventory, bldg_func_df, arch_mapping, arch_col)
 
         return dmg_ret_json, func_ret_json, max_state_df
 
     @staticmethod
     def get_mapped_result_from_dataset_id(client, inventory_id: str, dmg_result_id: str, bldg_func_id,
                                           archetype_mapping_id: str,
-                                          groupby_col_name: str = "max_state"):
+                                          groupby_col_name: str = "max_state", arch_col='archetype'):
         """Use this if your damage results are already stored in the data service and you have their dataset ids.
         All the inputs (except groupby_col_name) are dataset ids.
 
         Args:
             client: Service client with authentication info
             inventory_id: Inventory dataset id
             dmg_result_id: Damage result dataset id
             bldg_func_id: Incore dataset for building func id
             archetype_mapping_id: Mapping id dataset for archetype
             groupby_col_name: column name to group by, default to max_state
+            arch_col: column name for the archetype to perform the merge
 
         Returns:
             dmg_ret_json: JSON of the damage state results ordered by cluster and category.
             func_ret_json: JSON of the building functionality results ordered by cluster and category.
             max_state_df: Dataframe of max damage state
 
         """
@@ -84,33 +87,34 @@
         bldg_func_df.rename(columns={'building_guid': 'guid'}, inplace=True)
 
         archtype_mapping_dataset = Dataset.from_data_service(archetype_mapping_id, DataService(client))
         arch_mapping = archtype_mapping_dataset.get_dataframe_from_csv()
 
         max_state_df = DataProcessUtil.get_max_damage_state(dmg_result)
         dmg_ret_json = DataProcessUtil.create_mapped_dmg_result(inventory, max_state_df, arch_mapping,
-                                                                groupby_col_name)
-        func_ret_json = DataProcessUtil.create_mapped_func_result(inventory, bldg_func_df, arch_mapping)
+                                                                groupby_col_name, arch_col)
+        func_ret_json = DataProcessUtil.create_mapped_func_result(inventory, bldg_func_df, arch_mapping, arch_col)
 
         return dmg_ret_json, func_ret_json, max_state_df
 
     @staticmethod
     def get_mapped_result_from_path(inventory_path: str, dmg_result_path: str,
                                     func_result_path: str,
                                     archetype_mapping_path: str,
-                                    groupby_col_name: str):
+                                    groupby_col_name: str, arch_col='archetype'):
         """
 
         Args:
             inventory_path: Path to the zip file containing the inventory
                     example: /Users/myuser/5f9091df3e86721ed82f701d.zip
             dmg_result_path: Path to the damage result output file
             func_result_path: Path to the bldg functionality result output file
             archetype_mapping_path: Path to the arechetype mappings
             groupby_col_name: column name to group by, default to max_state
+            arch_col: column name for the archetype to perform the merge
 
         Returns:
             dmg_ret_json: JSON of the damage state results ordered by cluster and category.
             func_ret_json: JSON of the building functionality results ordered by cluster and category.
             mapped_df: Dataframe of max damage state
 
         """
@@ -118,36 +122,37 @@
         dmg_result = pd.read_csv(dmg_result_path)
         bldg_func_df = pd.read_csv(func_result_path)
         bldg_func_df.rename(columns={'building_guid': 'guid'}, inplace=True)
         arch_mapping = pd.read_csv(archetype_mapping_path)
 
         max_state_df = DataProcessUtil.get_max_damage_state(dmg_result)
         dmg_ret_json = DataProcessUtil.create_mapped_dmg_result(inventory, max_state_df, arch_mapping,
-                                                                groupby_col_name)
+                                                                groupby_col_name, arch_col)
 
-        func_ret_json = DataProcessUtil.create_mapped_func_result(inventory, bldg_func_df, arch_mapping)
+        func_ret_json = DataProcessUtil.create_mapped_func_result(inventory, bldg_func_df, arch_mapping, arch_col)
 
         return dmg_ret_json, func_ret_json, max_state_df
 
     @staticmethod
-    def create_mapped_dmg_result(inventory, dmg_result, arch_mapping, groupby_col_name="max_state"):
+    def create_mapped_dmg_result(inventory, dmg_result, arch_mapping, groupby_col_name="max_state",
+                                 arch_col='archetype'):
         """
 
         Args:
             inventory: dataframe represent inventory
             dmg_result: dmg_result that need to merge with inventory and be grouped
-            arch_mapping: Path to the arechetype mappings
+            arch_mapping: Path to the archetype mappings
 
         Returns:
             ret_json: JSON of the results ordered by cluster and category.
 
         """
         dmg_states = dmg_result[groupby_col_name].unique().tolist()  # get unique damage states
         dmg_merged = pd.merge(inventory, dmg_result, on='guid')
-        mapped_df = pd.merge(dmg_merged, arch_mapping, on='archetype')
+        mapped_df = pd.merge(dmg_merged, arch_mapping, on=arch_col)
         unique_categories = arch_mapping.groupby(by=['cluster', 'category'], sort=False).count().reset_index()
 
         group_by = mapped_df.groupby(by=[groupby_col_name, 'cluster', 'category']).count().reset_index()
         group_by = group_by.loc[:, ['guid', groupby_col_name, 'cluster', 'category']]
         group_by.rename(columns={'guid': 'count'}, inplace=True)
 
         pivot = group_by.pivot_table(values='count', index=['cluster', 'category'], columns=groupby_col_name,
@@ -170,29 +175,30 @@
         category_records = result_by_category.to_json(orient="records")
         json_by_cluster = json.loads(cluster_records)
         json_by_category = json.loads(category_records)
 
         return {"by_cluster": json_by_cluster, "by_category": json_by_category}
 
     @staticmethod
-    def create_mapped_func_result(inventory, bldg_func, arch_mapping):
+    def create_mapped_func_result(inventory, bldg_func, arch_mapping, arch_col='archetype'):
         """
 
         Args:
             inventory: dataframe represent inventory
             bldg_func: building func dataset
-            arch_mapping: Path to the arechetype mappings
+            arch_mapping: Path to the archetype mappings
+            arch_col: archetype column to use for the clustering
 
         Returns:
             ret_json: JSON of the results ordered by cluster and category.
 
         """
         func_state = ["percent_functional", "percent_non_functional", "num_functional", "num_non_functional"]
         func_merged = pd.merge(inventory, bldg_func, on='guid')
-        mapped_df = pd.merge(func_merged, arch_mapping, on='archetype')
+        mapped_df = pd.merge(func_merged, arch_mapping, on=arch_col)
         unique_categories = arch_mapping.groupby(by=['category'], sort=False, as_index=False).count()['category']
         unique_cluster = arch_mapping.groupby(by=['cluster', 'category'], sort=False, as_index=False).count()[[
             'cluster', 'category']]
 
         # group by cluster
         result_by_cluster = mapped_df.groupby(by=['cluster', 'category'], sort=False, as_index=False).agg(
             {'guid': 'count',
```

### Comparing `pyincore-1.8.0/pyincore/utils/datasetutil.py` & `pyincore-1.9.0/pyincore/utils/datasetutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/evaluateexpression.py` & `pyincore-1.9.0/pyincore/utils/evaluateexpression.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/expressioneval/__init__.py` & `pyincore-1.9.0/pyincore/utils/expressioneval/__init__.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/geoutil.py` & `pyincore-1.9.0/pyincore/utils/geoutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/networkutil.py` & `pyincore-1.9.0/pyincore/utils/networkutil.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore/utils/popdisloutputprocess.py` & `pyincore-1.9.0/pyincore/utils/popdisloutputprocess.py`

 * *Files identical despite different names*

### Comparing `pyincore-1.8.0/pyincore.egg-info/PKG-INFO` & `pyincore-1.9.0/pyincore.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyincore
-Version: 1.8.0
+Version: 1.9.0
 Summary: IN-CORE analysis tool python package
 Home-page: https://incore.ncsa.illinois.edu
 License: Mozilla Public License v2.0
 Project-URL: Bug Reports, https://github.com/IN-CORE/pyincore/issues
 Project-URL: Source, https://github.com/IN-CORE/pyincore
 Keywords: infrastructure,resilience,hazards,data discovery,IN-CORE,earthquake,tsunami,tornado,hurricane,dislocation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyincore-1.8.0/pyincore.egg-info/SOURCES.txt` & `pyincore-1.9.0/pyincore.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 pyincore/analyses/buildingportfolio/recovery/BuildingData.py
 pyincore/analyses/buildingportfolio/recovery/BuildingPortfolioRecoveryAnalysis.py
 pyincore/analyses/buildingportfolio/recovery/__init__.py
 pyincore/analyses/capitalshocks/__init__.py
 pyincore/analyses/capitalshocks/capitalshocks.py
 pyincore/analyses/combinedwindwavesurgebuildingdamage/__init__.py
 pyincore/analyses/combinedwindwavesurgebuildingdamage/combinedwindwavesurgebuildingdamage.py
+pyincore/analyses/combinedwindwavesurgebuildingloss/__init__.py
+pyincore/analyses/combinedwindwavesurgebuildingloss/combinedwindwavesurgebuildingloss.py
 pyincore/analyses/cumulativebuildingdamage/__init__.py
 pyincore/analyses/cumulativebuildingdamage/cumulativebuildingdamage.py
 pyincore/analyses/epfdamage/__init__.py
 pyincore/analyses/epfdamage/epfdamage.py
 pyincore/analyses/epfdamage/epfutil.py
 pyincore/analyses/epfrestoration/__init__.py
 pyincore/analyses/epfrestoration/epfrestoration.py
@@ -91,14 +93,19 @@
 pyincore/analyses/populationdislocation/__init__.py
 pyincore/analyses/populationdislocation/populationdislocation.py
 pyincore/analyses/populationdislocation/populationdislocationutil.py
 pyincore/analyses/residentialbuildingrecovery/__init__.py
 pyincore/analyses/residentialbuildingrecovery/residentialbuildingrecovery.py
 pyincore/analyses/roaddamage/__init__.py
 pyincore/analyses/roaddamage/roaddamage.py
+pyincore/analyses/saltlakecge/__init__.py
+pyincore/analyses/saltlakecge/equationlib.py
+pyincore/analyses/saltlakecge/outputfunctions.py
+pyincore/analyses/saltlakecge/saltlakecge.py
+pyincore/analyses/saltlakecge/saltlakeoutput.py
 pyincore/analyses/seasidecge/__init__.py
 pyincore/analyses/seasidecge/equationlib.py
 pyincore/analyses/seasidecge/seasidecge.py
 pyincore/analyses/socialvulnerability/__init__.py
 pyincore/analyses/socialvulnerability/socialvulnerability.py
 pyincore/analyses/tornadoepndamage/__init__.py
 pyincore/analyses/tornadoepndamage/tornadoepndamage.py
@@ -128,10 +135,12 @@
 pyincore/utils/__init__.py
 pyincore/utils/analysisutil.py
 pyincore/utils/cgeoutputprocess.py
 pyincore/utils/dataprocessutil.py
 pyincore/utils/datasetutil.py
 pyincore/utils/evaluateexpression.py
 pyincore/utils/geoutil.py
+pyincore/utils/hhrsoutputprocess.py
 pyincore/utils/networkutil.py
 pyincore/utils/popdisloutputprocess.py
-pyincore/utils/expressioneval/__init__.py
+pyincore/utils/expressioneval/__init__.py
+tests/test_format.py
```

### Comparing `pyincore-1.8.0/setup.py` & `pyincore-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This program and the accompanying materials are made available under the
 # terms of the Mozilla Public License v2.0 which accompanies this distribution,
 # and is available at https://www.mozilla.org/en-US/MPL/2.0/
 
 from setuptools import setup, find_packages
 
 # version number of pyincore
-version = '1.8.0'
+version = '1.9.0'
 
 with open("README.rst", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name='pyincore',
     version=version,
```

