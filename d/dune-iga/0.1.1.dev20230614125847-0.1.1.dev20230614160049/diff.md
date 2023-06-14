# Comparing `tmp/dune-iga-0.1.1.dev20230614125847.tar.gz` & `tmp/dune-iga-0.1.1.dev20230614160049.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-iga-0.1.1.dev20230614125847.tar", last modified: Wed Jun 14 12:58:48 2023, max compression
+gzip compressed data, was "dune-iga-0.1.1.dev20230614160049.tar", last modified: Wed Jun 14 16:00:50 2023, max compression
```

## Comparing `dune-iga-0.1.1.dev20230614125847.tar` & `dune-iga-0.1.1.dev20230614160049.tar`

### file list

```diff
@@ -1,147 +1,150 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.395870 dune-iga-0.1.1.dev20230614125847/
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.clang-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.375870 dune-iga-0.1.1.dev20230614125847/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      435 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1758 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2245 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     1728 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/reuseLint.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3142 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/.reuse/
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1332 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/LICENSES/
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-14 12:58:48.395870 dune-iga-0.1.1.dev20230614125847/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/cmake/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/FormatTarget/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/FormatTarget/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      843 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/AddClipperLibFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      826 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/AddEarCutFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/AddnLohmannJsonFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/cmake/modules/DuneIgaMacros.cmake
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.379870 dune-iga-0.1.1.dev20230614125847/dune/
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.383870 dune-iga-0.1.1.dev20230614125847/dune/iga/
--rw-r--r--   0 root         (0) root         (0)      808 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9152 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/bsplinealgorithms.hh
--rw-r--r--   0 root         (0) root         (0)     2017 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/controlpoint.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.383870 dune-iga-0.1.1.dev20230614125847/dune/iga/geometry/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/geometry/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6073 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/geometry/closestpointprojection.hh
--rw-r--r--   0 root         (0) root         (0)     2804 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/geometry/geohelper.hh
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/gridcapabilities.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.383870 dune-iga-0.1.1.dev20230614125847/dune/iga/io/
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/io/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.383870 dune-iga-0.1.1.dev20230614125847/dune/iga/io/ibra/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/io/ibra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    10369 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/io/ibra/ibrageometry.hh
--rw-r--r--   0 root         (0) root         (0)     7806 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/io/ibra/ibrareader.hh
--rw-r--r--   0 root         (0) root         (0)     8239 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/io/igadatacollector.hh
--rw-r--r--   0 root         (0) root         (0)    30652 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsalgorithms.hh
--rw-r--r--   0 root         (0) root         (0)    29306 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsbasis.hh
--rw-r--r--   0 root         (0) root         (0)    18305 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgeometry.hh
--rw-r--r--   0 root         (0) root         (0)    11629 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgrid.hh
--rw-r--r--   0 root         (0) root         (0)    13111 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridentity.hh
--rw-r--r--   0 root         (0) root         (0)     3063 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridindexsets.hh
--rw-r--r--   0 root         (0) root         (0)     3957 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridleafiterator.hh
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridtraits.hh
--rw-r--r--   0 root         (0) root         (0)     1285 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsidset.hh
--rw-r--r--   0 root         (0) root         (0)     7882 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsintersection.hh
--rw-r--r--   0 root         (0) root         (0)     9302 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsleafgridview.hh
--rw-r--r--   0 root         (0) root         (0)     9447 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbslocalgeometry.hh
--rw-r--r--   0 root         (0) root         (0)    36685 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbspatch.hh
--rw-r--r--   0 root         (0) root         (0)     1454 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbspatchdata.hh
--rw-r--r--   0 root         (0) root         (0)     9061 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/nurbspatchgeometry.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.387870 dune-iga-0.1.1.dev20230614125847/dune/iga/test/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.387870 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)     5772 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/element.ibra
--rw-r--r--   0 root         (0) root         (0)     7222 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/element_trim.ibra
--rw-r--r--   0 root         (0) root         (0)     7396 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra
--rw-r--r--   0 root         (0) root         (0)     7665 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/infty_pwh.ibra
--rw-r--r--   0 root         (0) root         (0)     6209 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/nurbs_1.ibra
--rw-r--r--   0 root         (0) root         (0)     6704 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/pipe_trim.ibra
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/plate_quarter.ibra
--rw-r--r--   0 root         (0) root         (0)    10170 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/schale_trim.ibra
--rw-r--r--   0 root         (0) root         (0)    12176 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/shell-hole.ibra
--rw-r--r--   0 root         (0) root         (0)     7146 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/shell.ibra
--rw-r--r--   0 root         (0) root         (0)     7688 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/surface-hole.ibra
--rw-r--r--   0 root         (0) root         (0)    60433 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/surface-multihole.ibra
--rw-r--r--   0 root         (0) root         (0)    45902 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/gridTests.cc
--rw-r--r--   0 root         (0) root         (0)    17532 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/test/trimmedGridTests.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.387870 dune-iga-0.1.1.dev20230614125847/dune/iga/trim/
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/trim/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4636 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/trim/nurbstrimboundary.hh
--rw-r--r--   0 root         (0) root         (0)    37350 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/trim/nurbstrimmer.hh
--rw-r--r--   0 root         (0) root         (0)    14597 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/trim/trimmedelementrepresentation.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.387870 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/
--rw-r--r--   0 root         (0) root         (0)      328 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/fillquadraturerule.hh
--rw-r--r--   0 root         (0) root         (0)     2326 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/igahelpers.hh
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/linearalgebra.hh
--rw-r--r--   0 root         (0) root         (0)    22061 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/mdnet.hh
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/iga/utils/typetraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.387870 dune-iga-0.1.1.dev20230614125847/dune/python/
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/dune/python/iga/
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6314 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/iga/grid.hh
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/iga/gridenums.hh
--rw-r--r--   0 root         (0) root         (0)     3951 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/iga/nurbspatchdata.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/dune/python/test/
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4969 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/test/poisson.py
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/test/readGrid.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune/python/test/setpath.py.in
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune-iga.pc.in
--rw-r--r--   0 root         (0) root         (0)      325 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/dune.module
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/python/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/python/dune/
--rw-r--r--   0 root         (0) root         (0)      179 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/python/dune/iga/
--rw-r--r--   0 root         (0) root         (0)      610 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/__init__.py
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/_iga.cc
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/_igagrids.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/_nurbspatchdata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/python/dune/iga/basis/
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3577 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/python/dune/iga/basis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.391870 dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-14 12:58:48.000000 dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3532 2023-06-14 12:58:48.000000 dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 12:58:48.000000 dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-14 12:58:48.000000 dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 12:58:48.000000 dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 12:58:48.395870 dune-iga-0.1.1.dev20230614125847/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      889 2023-06-14 12:58:47.000000 dune-iga-0.1.1.dev20230614125847/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.395870 dune-iga-0.1.1.dev20230614125847/src/
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 12:58:48.395870 dune-iga-0.1.1.dev20230614125847/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)      228 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/auxiliaryFiles/kirchhoff_plate.parset
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/auxiliaryFiles/linear2dsolid.parset
--rw-r--r--   0 root         (0) root         (0)     7688 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/auxiliaryFiles/surface-hole.ibra
--rw-r--r--   0 root         (0) root         (0)     6609 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/kirchhoff_plate.cc
--rw-r--r--   0 root         (0) root         (0)    13589 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/kirchhoffplate.hh
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/linear2dsolid.cc
--rw-r--r--   0 root         (0) root         (0)    15691 2023-06-14 12:58:40.000000 dune-iga-0.1.1.dev20230614125847/src/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.269451 dune-iga-0.1.1.dev20230614160049/
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.clang-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.237450 dune-iga-0.1.1.dev20230614160049/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1758 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/reuseLint.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-14 16:00:50.269451 dune-iga-0.1.1.dev20230614160049/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/cmake/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/FormatTarget/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/FormatTarget/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      843 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/AddClipperLibFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      826 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/AddEarCutFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/AddnLohmannJsonFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/cmake/modules/DuneIgaMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.245451 dune-iga-0.1.1.dev20230614160049/dune/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.249451 dune-iga-0.1.1.dev20230614160049/dune/iga/
+-rw-r--r--   0 root         (0) root         (0)      808 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9152 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/bsplinealgorithms.hh
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/controlpoint.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.253451 dune-iga-0.1.1.dev20230614160049/dune/iga/geometry/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/geometry/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6073 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/geometry/closestpointprojection.hh
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/geometry/geohelper.hh
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/gridcapabilities.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.253451 dune-iga-0.1.1.dev20230614160049/dune/iga/io/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/io/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.253451 dune-iga-0.1.1.dev20230614160049/dune/iga/io/ibra/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/io/ibra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    10369 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/io/ibra/ibrageometry.hh
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/io/ibra/ibrareader.hh
+-rw-r--r--   0 root         (0) root         (0)     8239 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/io/igadatacollector.hh
+-rw-r--r--   0 root         (0) root         (0)    30652 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsalgorithms.hh
+-rw-r--r--   0 root         (0) root         (0)    29306 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsbasis.hh
+-rw-r--r--   0 root         (0) root         (0)    18305 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgeometry.hh
+-rw-r--r--   0 root         (0) root         (0)    11629 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgrid.hh
+-rw-r--r--   0 root         (0) root         (0)    13111 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridentity.hh
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridindexsets.hh
+-rw-r--r--   0 root         (0) root         (0)     3957 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridleafiterator.hh
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridtraits.hh
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsidset.hh
+-rw-r--r--   0 root         (0) root         (0)     7882 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsintersection.hh
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsleafgridview.hh
+-rw-r--r--   0 root         (0) root         (0)     9447 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbslocalgeometry.hh
+-rw-r--r--   0 root         (0) root         (0)    36685 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbspatch.hh
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbspatchdata.hh
+-rw-r--r--   0 root         (0) root         (0)     9061 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/nurbspatchgeometry.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.253451 dune-iga-0.1.1.dev20230614160049/dune/iga/test/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.257451 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)     5772 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/element.ibra
+-rw-r--r--   0 root         (0) root         (0)     7222 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/element_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)     7396 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/infty_pwh.ibra
+-rw-r--r--   0 root         (0) root         (0)     6209 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/nurbs_1.ibra
+-rw-r--r--   0 root         (0) root         (0)     6704 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/pipe_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/plate_quarter.ibra
+-rw-r--r--   0 root         (0) root         (0)    10170 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/schale_trim.ibra
+-rw-r--r--   0 root         (0) root         (0)    12176 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/shell-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)     7146 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/shell.ibra
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/surface-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)    60433 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/surface-multihole.ibra
+-rw-r--r--   0 root         (0) root         (0)    45902 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/gridTests.cc
+-rw-r--r--   0 root         (0) root         (0)    17532 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/test/trimmedGridTests.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.257451 dune-iga-0.1.1.dev20230614160049/dune/iga/trim/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/trim/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/trim/nurbstrimboundary.hh
+-rw-r--r--   0 root         (0) root         (0)    37350 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/trim/nurbstrimmer.hh
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/trim/trimmedelementrepresentation.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.261451 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/fillquadraturerule.hh
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/igahelpers.hh
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/linearalgebra.hh
+-rw-r--r--   0 root         (0) root         (0)    22061 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/mdnet.hh
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/iga/utils/typetraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.261451 dune-iga-0.1.1.dev20230614160049/dune/python/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.261451 dune-iga-0.1.1.dev20230614160049/dune/python/iga/
+-rw-r--r--   0 root         (0) root         (0)      290 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/iga/boundarypatch.hh
+-rw-r--r--   0 root         (0) root         (0)     6314 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/iga/grid.hh
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/iga/gridenums.hh
+-rw-r--r--   0 root         (0) root         (0)     3951 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/iga/nurbspatchdata.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.261451 dune-iga-0.1.1.dev20230614160049/dune/python/test/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/test/Poisson.vtu
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/test/poisson.py
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/test/readGrid.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune/python/test/setpath.py.in
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune-iga.pc.in
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/dune.module
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.261451 dune-iga-0.1.1.dev20230614160049/python/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.265451 dune-iga-0.1.1.dev20230614160049/python/dune/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.265451 dune-iga-0.1.1.dev20230614160049/python/dune/iga/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      375 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/_iga.cc
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/_igagrids.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/_nurbspatchdata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.265451 dune-iga-0.1.1.dev20230614160049/python/dune/iga/basis/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/basis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/python/dune/iga/boundarypatch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.265451 dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-14 16:00:50.000000 dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3627 2023-06-14 16:00:50.000000 dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 16:00:50.000000 dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-14 16:00:50.000000 dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-14 16:00:50.000000 dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 16:00:50.269451 dune-iga-0.1.1.dev20230614160049/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      889 2023-06-14 16:00:49.000000 dune-iga-0.1.1.dev20230614160049/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.265451 dune-iga-0.1.1.dev20230614160049/src/
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:00:50.269451 dune-iga-0.1.1.dev20230614160049/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)      228 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/auxiliaryFiles/kirchhoff_plate.parset
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/auxiliaryFiles/linear2dsolid.parset
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/auxiliaryFiles/surface-hole.ibra
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/kirchhoff_plate.cc
+-rw-r--r--   0 root         (0) root         (0)    13589 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/kirchhoffplate.hh
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/linear2dsolid.cc
+-rw-r--r--   0 root         (0) root         (0)    15691 2023-06-14 16:00:42.000000 dune-iga-0.1.1.dev20230614160049/src/linearElastic.hh
```

### Comparing `dune-iga-0.1.1.dev20230614125847/.clang-format` & `dune-iga-0.1.1.dev20230614160049/.clang-format`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/.github/workflows/debian-coverage.yml` & `dune-iga-0.1.1.dev20230614160049/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/.github/workflows/debian.yml` & `dune-iga-0.1.1.dev20230614160049/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/.github/workflows/releasePythonPackage.yml` & `dune-iga-0.1.1.dev20230614160049/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/.github/workflows/scripts/release.py` & `dune-iga-0.1.1.dev20230614160049/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/.github/workflows/style.yml` & `dune-iga-0.1.1.dev20230614160049/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/CMakeLists.txt` & `dune-iga-0.1.1.dev20230614160049/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/LICENSES/CC0-1.0.txt` & `dune-iga-0.1.1.dev20230614160049/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/LICENSES/LGPL-3.0-or-later.txt` & `dune-iga-0.1.1.dev20230614160049/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/PKG-INFO` & `dune-iga-0.1.1.dev20230614160049/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-iga
-Version: 0.1.1.dev20230614125847
+Version: 0.1.1.dev20230614160049
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

### Comparing `dune-iga-0.1.1.dev20230614125847/README.md` & `dune-iga-0.1.1.dev20230614160049/README.md`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/FormatTarget/CMakeLists.txt` & `dune-iga-0.1.1.dev20230614160049/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/FormatTarget/CPM.cmake` & `dune-iga-0.1.1.dev20230614160049/cmake/FormatTarget/CPM.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/modules/AddAutoDiffFlags.cmake` & `dune-iga-0.1.1.dev20230614160049/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/modules/AddClipperLibFlags.cmake` & `dune-iga-0.1.1.dev20230614160049/cmake/modules/AddClipperLibFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/modules/AddEarCutFlags.cmake` & `dune-iga-0.1.1.dev20230614160049/cmake/modules/AddEarCutFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/modules/AddEigenFlags.cmake` & `dune-iga-0.1.1.dev20230614160049/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/cmake/modules/AddnLohmannJsonFlags.cmake` & `dune-iga-0.1.1.dev20230614160049/cmake/modules/AddnLohmannJsonFlags.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/config.h.cmake` & `dune-iga-0.1.1.dev20230614160049/config.h.cmake`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/CMakeLists.txt` & `dune-iga-0.1.1.dev20230614160049/dune/iga/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/bsplinealgorithms.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/bsplinealgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/controlpoint.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/controlpoint.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/geometry/closestpointprojection.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/geometry/closestpointprojection.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/geometry/geohelper.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/geometry/geohelper.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/gridcapabilities.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/gridcapabilities.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/io/ibra/ibrageometry.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/io/ibra/ibrageometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/io/ibra/ibrareader.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/io/ibra/ibrareader.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/io/igadatacollector.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/io/igadatacollector.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsalgorithms.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsalgorithms.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsbasis.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsbasis.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgeometry.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgrid.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgrid.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridentity.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridentity.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridindexsets.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridindexsets.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridleafiterator.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridleafiterator.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsgridtraits.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsgridtraits.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsidset.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsidset.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsintersection.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsintersection.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbsleafgridview.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbsleafgridview.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbslocalgeometry.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbslocalgeometry.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbspatch.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbspatch.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbspatchdata.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbspatchdata.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/nurbspatchgeometry.h` & `dune-iga-0.1.1.dev20230614160049/dune/iga/nurbspatchgeometry.h`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/CMakeLists.txt` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/element.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/element.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/element_trim.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/element_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/element_trim_xb.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/infty_pwh.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/infty_pwh.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/nurbs_1.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/nurbs_1.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/pipe_trim.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/pipe_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/plate_quarter.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/plate_quarter.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/schale_trim.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/schale_trim.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/shell-hole.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/shell-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/shell.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/shell.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/surface-hole.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/surface-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/auxiliaryFiles/surface-multihole.ibra` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/auxiliaryFiles/surface-multihole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/gridTests.cc` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/gridTests.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/test/trimmedGridTests.cc` & `dune-iga-0.1.1.dev20230614160049/dune/iga/test/trimmedGridTests.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/trim/nurbstrimboundary.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/trim/nurbstrimboundary.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/trim/nurbstrimmer.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/trim/nurbstrimmer.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/trim/trimmedelementrepresentation.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/trim/trimmedelementrepresentation.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/utils/concepts.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/utils/fillquadraturerule.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/utils/fillquadraturerule.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/utils/igahelpers.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/utils/igahelpers.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/utils/linearalgebra.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/utils/linearalgebra.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/iga/utils/mdnet.hh` & `dune-iga-0.1.1.dev20230614160049/dune/iga/utils/mdnet.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/python/iga/grid.hh` & `dune-iga-0.1.1.dev20230614160049/dune/python/iga/grid.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/python/iga/nurbspatchdata.hh` & `dune-iga-0.1.1.dev20230614160049/dune/python/iga/nurbspatchdata.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/python/test/poisson.py` & `dune-iga-0.1.1.dev20230614160049/dune/python/test/poisson.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import math
 from scipy.sparse import lil_matrix
 import scipy as sp
 import dune.geometry
 import dune.grid
 from dune.iga import reader as readeriga
 from dune.iga.basis import defaultGlobalBasis, Power, Lagrange, Nurbs
-from dune.iga import IGAGrid
+from dune.iga import IGAGrid, boundaryPatch
 from dune.grid import gridFunction
 from dune.common import FieldVector
 import os
 
 os.environ["ALUGRID_VERBOSITY_LEVEL"] = "0"
 
 # f(x) = 1
@@ -127,14 +127,19 @@
 ############################### START ########################################
 
 # create a trimmed grid from file
 reader = (readeriga.json, "../../iga/test/auxiliaryFiles/element_trim_xb.ibra")
 
 gridView = IGAGrid(reader, dimgrid=2, dimworld=2)
 gridView.hierarchicalGrid.globalRefine(2)
+
+neumannVertices = np.zeros(gridView.size(2), dtype=bool)
+
+boundaryPatch = boundaryPatch(gridView, neumannVertices)
+
 basis = defaultGlobalBasis(gridView, Nurbs())
 
 # compute A and b
 A, b = globalAssembler(basis)
 
 # convert A to Compressed Sparse Column format
 Acsc = A.tocsc()
```

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/python/test/readGrid.py` & `dune-iga-0.1.1.dev20230614160049/dune/python/test/readGrid.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/dune/python/test/setpath.py.in` & `dune-iga-0.1.1.dev20230614160049/dune/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/python/dune/iga/CMakeLists.txt` & `dune-iga-0.1.1.dev20230614160049/python/dune/iga/CMakeLists.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # SPDX-FileCopyrightText: 2023 The dune-iga developers
 # mueller@ibb.uni-stuttgart.de SPDX-License-Identifier: LGPL-3.0-or-later
 add_subdirectory(basis)
 
-add_python_targets(iga __init__ _igagrids _nurbspatchdata)
+add_python_targets(iga __init__ _igagrids _nurbspatchdata boundarypatch)
 
 dune_add_pybind11_module(NAME _iga)
- set_property(TARGET _iga PROPERTY LINK_LIBRARIES dunecommon dunegeometry
- PkgConfig::Clipper2Lib nlohmann_json::nlohmann_json earcut_hpp::earcut_hpp
- APPEND)
+set_property(
+  TARGET _iga
+  PROPERTY LINK_LIBRARIES dunecommon dunegeometry PkgConfig::Clipper2Lib
+           nlohmann_json::nlohmann_json earcut_hpp::earcut_hpp
+  APPEND)
 target_link_libraries(_iga PUBLIC PkgConfig::Clipper2Lib)
- target_compile_definitions(_iga PUBLIC ENABLE_CLIPPERLIB2=1)
+target_compile_definitions(_iga PUBLIC ENABLE_CLIPPERLIB2=1)
 
 if(SKBUILD)
   install(TARGETS _iga LIBRARY DESTINATION python/dune/iga)
 endif()
```

### Comparing `dune-iga-0.1.1.dev20230614125847/python/dune/iga/_igagrids.py` & `dune-iga-0.1.1.dev20230614160049/python/dune/iga/_igagrids.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/python/dune/iga/_nurbspatchdata.py` & `dune-iga-0.1.1.dev20230614160049/python/dune/iga/_nurbspatchdata.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/python/dune/iga/basis/__init__.py` & `dune-iga-0.1.1.dev20230614160049/python/dune/iga/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/PKG-INFO` & `dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-iga
-Version: 0.1.1.dev20230614125847
+Version: 0.1.1.dev20230614160049
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

### Comparing `dune-iga-0.1.1.dev20230614125847/python/dune_iga.egg-info/SOURCES.txt` & `dune-iga-0.1.1.dev20230614160049/python/dune_iga.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -82,28 +82,31 @@
 dune/iga/utils/fillquadraturerule.hh
 dune/iga/utils/igahelpers.hh
 dune/iga/utils/linearalgebra.hh
 dune/iga/utils/mdnet.hh
 dune/iga/utils/typetraits.hh
 dune/python/CMakeLists.txt
 dune/python/iga/CMakeLists.txt
+dune/python/iga/boundarypatch.hh
 dune/python/iga/grid.hh
 dune/python/iga/gridenums.hh
 dune/python/iga/nurbspatchdata.hh
 dune/python/test/CMakeLists.txt
+dune/python/test/Poisson.vtu
 dune/python/test/poisson.py
 dune/python/test/readGrid.py
 dune/python/test/setpath.py.in
 python/CMakeLists.txt
 python/dune/CMakeLists.txt
 python/dune/iga/CMakeLists.txt
 python/dune/iga/__init__.py
 python/dune/iga/_iga.cc
 python/dune/iga/_igagrids.py
 python/dune/iga/_nurbspatchdata.py
+python/dune/iga/boundarypatch.py
 python/dune/iga/basis/CMakeLists.txt
 python/dune/iga/basis/__init__.py
 python/dune_iga.egg-info/PKG-INFO
 python/dune_iga.egg-info/SOURCES.txt
 python/dune_iga.egg-info/dependency_links.txt
 python/dune_iga.egg-info/requires.txt
 python/dune_iga.egg-info/top_level.txt
```

### Comparing `dune-iga-0.1.1.dev20230614125847/setup.py` & `dune-iga-0.1.1.dev20230614160049/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 # build _iga
 # cd /tmp/dune-iga
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/dune-iga
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-duneigaVersion = "0.1.1.dev20230614125847"
+duneigaVersion = "0.1.1.dev20230614160049"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = duneigaVersion
 
 setup(**metadata)
```

### Comparing `dune-iga-0.1.1.dev20230614125847/src/CMakeLists.txt` & `dune-iga-0.1.1.dev20230614160049/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/src/auxiliaryFiles/surface-hole.ibra` & `dune-iga-0.1.1.dev20230614160049/src/auxiliaryFiles/surface-hole.ibra`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/src/kirchhoff_plate.cc` & `dune-iga-0.1.1.dev20230614160049/src/kirchhoff_plate.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/src/kirchhoffplate.hh` & `dune-iga-0.1.1.dev20230614160049/src/kirchhoffplate.hh`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/src/linear2dsolid.cc` & `dune-iga-0.1.1.dev20230614160049/src/linear2dsolid.cc`

 * *Files identical despite different names*

### Comparing `dune-iga-0.1.1.dev20230614125847/src/linearElastic.hh` & `dune-iga-0.1.1.dev20230614160049/src/linearElastic.hh`

 * *Files identical despite different names*

