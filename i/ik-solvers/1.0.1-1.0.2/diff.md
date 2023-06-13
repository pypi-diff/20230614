# Comparing `tmp/ik_solvers-1.0.1.tar.gz` & `tmp/ik_solvers-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ik_solvers-1.0.1.tar", last modified: Sat Jun 10 19:30:59 2023, max compression
+gzip compressed data, was "ik_solvers-1.0.2.tar", last modified: Tue Jun 13 22:06:42 2023, max compression
```

## Comparing `ik_solvers-1.0.1.tar` & `ik_solvers-1.0.2.tar`

### file list

```diff
@@ -1,385 +1,401 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.649186 ik_solvers-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.601186 ik_solvers-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.605186 ik_solvers-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/.github/workflows/test-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-10 19:30:59.649186 ik_solvers-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.605186 ik_solvers-1.0.1/ik_solvers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-10 19:30:59.000000 ik_solvers-1.0.1/ik_solvers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-06-10 19:30:59.000000 ik_solvers-1.0.1/ik_solvers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:30:59.000000 ik_solvers-1.0.1/ik_solvers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 19:30:59.000000 ik_solvers-1.0.1/ik_solvers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 19:30:59.000000 ik_solvers-1.0.1/ik_solvers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.605186 ik_solvers-1.0.1/include/
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/include/ForwardDynamicsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/include/IKSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/include/SolverLoader.h
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/include/Utility.h
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/include/kdl_parser.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.601186 ik_solvers-1.0.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.605186 ik_solvers-1.0.1/lib/orocos_kdl/
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/INSTALL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.609186 ik_solvers-1.0.1/lib/orocos_kdl/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/cmake/CheckSTLContainers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/cmake/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/cmake/FindPkgConfig.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/cmake_uninstall.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.609186 ik_solvers-1.0.1/lib/orocos_kdl/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/README
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/README.Debian
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/docs
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/kdl.doc-base.EX
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/liborocos-kdl-dev.install
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/liborocos-kdl.install
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/manpage.1.ex
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/python-orocos-kdl.install
--rwxr-xr-x   0 runner    (1001) docker     (123)     3200 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/rules
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/debian/substvars
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.609186 ik_solvers-1.0.1/lib/orocos_kdl/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/doc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/doc/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/doc/tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.609186 ik_solvers-1.0.1/lib/orocos_kdl/doc/tex/
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/doc/tex/UserManual.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.613186 ik_solvers-1.0.1/lib/orocos_kdl/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/README
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/chainiksolverpos_lma_demo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/geometry.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/plotframe.m
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/trajectory_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/examples/visualize_trajectory.m
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/manifest.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.613186 ik_solvers-1.0.1/lib/orocos_kdl/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/kukaLWR_DHnew.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/kukaLWRtestDHnew.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/kukaLWRtestHCG.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/models.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/puma560.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/models/puma560test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/orocos_kdl-config-version.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/orocos_kdl-config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/orocos_kdl.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/package.xml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/rosdoc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.629186 ik_solvers-1.0.1/lib/orocos_kdl/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/TODO.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/articulatedbodyinertia.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/articulatedbodyinertia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chain.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chaindynparam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chaindynparam.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainexternalwrenchestimator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainexternalwrenchestimator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfdsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolverpos_recursive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolverpos_recursive.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolvervel_recursive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolvervel_recursive.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainhdsolver_vereshchagin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31869 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainhdsolver_vereshchagin.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_vereshchagin.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_vereshchagin.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_lma.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_lma.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr_jl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr_jl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_wdls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_wdls.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacdotsolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacdotsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacsolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc.inl
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc_io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frames.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    50153 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frames.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frames.inl
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frames_io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/frames_io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/framevel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/framevel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/framevel.inl
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/framevel_io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jacobian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jacobian.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntarray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntarray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayacc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayacc.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayvel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayvel.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntspaceinertiamatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/jntspaceinertiamatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/joint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/joint.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/kdl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/kinfam.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/kinfam_io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/kinfam_io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/motion.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_circle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_circle.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_composite.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_composite.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_cyclic_closed.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_cyclic_closed.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_line.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_point.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_point.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_roundedcomposite.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/path_roundedcomposite.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rigidbodyinertia.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rigidbodyinertia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation_sa.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation_sa.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rotationalinertia.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/rotationalinertia.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/segment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/segment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/solveri.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/stiffness.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_composite.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_composite.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_segment.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_segment.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_stationary.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_stationary.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/tree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/tree.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treefksolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treefksolverpos_recursive.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treefksolverpos_recursive.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeidsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_nr_jl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_nr_jl.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_online.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolvervel_wdls.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolvervel_wdls.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treejnttojacsolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/treejnttojacsolver.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.633186 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/error_stack.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/error_stack.h
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/hash_combine.h
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/header.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/kdl-config.h
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/ldl_solver_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/ldl_solver_eigen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall1d.h
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall1d_io.h
--rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall2d.h
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall2d_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rallNd.h
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/scoped_ptr.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_HH.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_HH.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_HH.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_HH.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_Macie.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_Macie.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/traits.h
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility.h
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility_io.cxx
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility_io.h
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_dirac.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_dirac.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_rect.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_rect.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_spline.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_spline.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_trap.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_trap.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_traphalf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_traphalf.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/orocos_kdl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32329 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/framestest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/framestest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/inertiatest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/inertiatest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/iotest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandottest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandottest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandoubletests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandoubletests.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobianframetests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobianframetests.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantests.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/kinfamtest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/kinfamtest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/rallnumbertest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/rframestest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/serialchaintest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    80493 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/solvertest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/solvertest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/test-runner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/toolkittest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/treeinvdyntest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/treeinvdyntest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/velocityprofiletest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/velocityprofiletest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/orocos_kdl/tests/zxxzxztest.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.601186 ik_solvers-1.0.1/lib/urdf_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/console_bridge/
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/console_bridge/console.h
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/console_bridge/console_bridge_export.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_exception/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_exception/exception.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/color.h
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/joint.h
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/link.h
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/model.h
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/pose.h
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/twist.h
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/model_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/twist.h
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_parser/exportdecl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_parser/urdf_parser.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_sensor/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_sensor/sensor.h
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_sensor/types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.637186 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_world/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_world/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/include/urdf_world/world.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.641186 ik_solvers-1.0.1/lib/urdf_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/check_urdf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/console.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/joint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/link.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/pose.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/twist.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/urdf_model_state.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/urdf_sensor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/urdf_to_graphviz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/src/world.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.641186 ik_solvers-1.0.1/lib/urdf_parser/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.641186 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.641186 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/gtest.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/gtest_main.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/internal_utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/libgtest.la.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.601186 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.641186 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/
--rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-death-test.h
--rw-r--r--   0 runner    (1001) docker     (123)    33126 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-matchers.h
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-message.h
--rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h
--rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h.pump
--rw-r--r--   0 runner    (1001) docker     (123)    35935 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-spi.h
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-test-part.h
--rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-typed-test.h
--rw-r--r--   0 runner    (1001) docker     (123)    94181 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest.h
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest_prod.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.645187 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.645187 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-printers.h
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest.h
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 runner    (1001) docker     (123)    61622 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-linked_ptr.h
--rw-r--r--   0 runner    (1001) docker     (123)   192179 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h.pump
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port-arch.h
--rw-r--r--   0 runner    (1001) docker     (123)    85257 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port.h
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-string.h
--rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h.pump
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h.pump
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.645187 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-all.cc
--rw-r--r--   0 runner    (1001) docker     (123)    62109 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-death-test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-filepath.cc
--rw-r--r--   0 runner    (1001) docker     (123)    47373 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-internal-inl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-matchers.cc
--rw-r--r--   0 runner    (1001) docker     (123)    48099 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-port.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-printers.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-test-part.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-typed-test.cc
--rw-r--r--   0 runner    (1001) docker     (123)   248867 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest_main.cc
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/memtest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/urdf_double_convert.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/urdf_unit_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/lib/urdf_parser/test/urdf_version_test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-10 19:30:59.649186 ik_solvers-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.649186 ik_solvers-1.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/src/ForwardDynamicsSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/src/IKSolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/src/pybindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 19:30:59.649186 ik_solvers-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-06-10 19:30:41.000000 ik_solvers-1.0.1/tests/ur10e.urdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.946317 ik_solvers-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.874311 ik_solvers-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.882311 ik_solvers-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/.github/workflows/test-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 22:06:42.946317 ik_solvers-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.882311 ik_solvers-1.0.2/ik_solvers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 22:06:42.000000 ik_solvers-1.0.2/ik_solvers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-06-13 22:06:42.000000 ik_solvers-1.0.2/ik_solvers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:06:42.000000 ik_solvers-1.0.2/ik_solvers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:06:42.000000 ik_solvers-1.0.2/ik_solvers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 22:06:42.000000 ik_solvers-1.0.2/ik_solvers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.882311 ik_solvers-1.0.2/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/include/ForwardDynamicsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/include/IKSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/include/SolverLoader.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/include/Utility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/include/kdl_parser.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.878311 ik_solvers-1.0.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.886312 ik_solvers-1.0.2/lib/orocos_kdl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24383 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/INSTALL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.886312 ik_solvers-1.0.2/lib/orocos_kdl/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/cmake/CheckSTLContainers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/cmake/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/cmake/FindPkgConfig.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/cmake_uninstall.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.886312 ik_solvers-1.0.2/lib/orocos_kdl/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/README
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/README.Debian
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/docs
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/kdl.doc-base.EX
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/liborocos-kdl-dev.install
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/liborocos-kdl.install
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/manpage.1.ex
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/python-orocos-kdl.install
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3200 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/debian/substvars
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.886312 ik_solvers-1.0.2/lib/orocos_kdl/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/doc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/doc/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/doc/tests.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.886312 ik_solvers-1.0.2/lib/orocos_kdl/doc/tex/
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/doc/tex/UserManual.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.890312 ik_solvers-1.0.2/lib/orocos_kdl/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/README
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/chainiksolverpos_lma_demo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/geometry.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/plotframe.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/trajectory_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/examples/visualize_trajectory.m
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/manifest.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.890312 ik_solvers-1.0.2/lib/orocos_kdl/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/kukaLWR_DHnew.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/kukaLWRtestDHnew.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/kukaLWRtestHCG.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/models.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/puma560.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/models/puma560test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/orocos_kdl-config-version.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/orocos_kdl-config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/orocos_kdl.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/package.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/rosdoc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.914314 ik_solvers-1.0.2/lib/orocos_kdl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/TODO.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/articulatedbodyinertia.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/articulatedbodyinertia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chain.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chaindynparam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chaindynparam.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainexternalwrenchestimator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainexternalwrenchestimator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfdsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolverpos_recursive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolverpos_recursive.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolvervel_recursive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolvervel_recursive.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainhdsolver_vereshchagin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31869 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainhdsolver_vereshchagin.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_vereshchagin.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_vereshchagin.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_lma.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_lma.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr_jl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr_jl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_wdls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_wdls.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacdotsolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacdotsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacsolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc_io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    50153 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frames.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frames.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frames_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/frames_io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/framevel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/framevel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/framevel.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/framevel_io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jacobian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jacobian.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntarray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntarray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayacc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayacc.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayvel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayvel.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntspaceinertiamatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/jntspaceinertiamatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/joint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/joint.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/kdl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/kinfam.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/kinfam_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/kinfam_io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/motion.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_circle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_circle.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_composite.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_composite.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_cyclic_closed.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_cyclic_closed.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_line.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_point.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_point.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_roundedcomposite.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/path_roundedcomposite.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rigidbodyinertia.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rigidbodyinertia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation_sa.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation_sa.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rotationalinertia.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/rotationalinertia.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/segment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/segment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/solveri.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/stiffness.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_composite.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_composite.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_segment.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_segment.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_stationary.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_stationary.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/tree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/tree.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treefksolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treefksolverpos_recursive.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treefksolverpos_recursive.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeidsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_nr_jl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_nr_jl.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_online.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolvervel_wdls.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolvervel_wdls.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treejnttojacsolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/treejnttojacsolver.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.922315 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/error_stack.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/error_stack.h
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/hash_combine.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/header.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/kdl-config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/ldl_solver_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/ldl_solver_eigen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall1d_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16639 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall2d.h
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall2d_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rallNd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/scoped_ptr.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_HH.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_HH.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_HH.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_HH.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_Macie.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_Macie.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/traits.h
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility_io.cxx
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility_io.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_dirac.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_dirac.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_rect.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_rect.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_spline.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_spline.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_trap.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_trap.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_traphalf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_traphalf.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/orocos_kdl/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32329 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/framestest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/framestest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/inertiatest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/inertiatest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/iotest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandottest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandottest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandoubletests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandoubletests.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobianframetests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobianframetests.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantests.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/kinfamtest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/kinfamtest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/rallnumbertest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/rframestest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/serialchaintest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    80493 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/solvertest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/solvertest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/test-runner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/toolkittest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/treeinvdyntest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/treeinvdyntest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/velocityprofiletest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/velocityprofiletest.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/orocos_kdl/tests/zxxzxztest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.878311 ik_solvers-1.0.2/lib/urdf_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/console_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/console_bridge/console.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/console_bridge/console_bridge_export.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_exception/exception.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/color.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/joint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/link.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/model.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/pose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/twist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/model_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/twist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_parser/exportdecl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_parser/urdf_parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_sensor/sensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_sensor/types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.926315 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_world/
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_world/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/include/urdf_world/world.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.930315 ik_solvers-1.0.2/lib/urdf_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/check_urdf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/console.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/joint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17741 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/link.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/pose.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/twist.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/urdf_model_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/urdf_sensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/urdf_to_graphviz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/src/world.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.930315 ik_solvers-1.0.2/lib/urdf_parser/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.930315 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.930315 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/gtest.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/gtest_main.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/internal_utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/libgtest.la.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.878311 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.934316 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/
+-rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-death-test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33126 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-matchers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-message.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22588 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h.pump
+-rw-r--r--   0 runner    (1001) docker     (123)    35935 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-spi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-test-part.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15881 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-typed-test.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94181 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest_pred_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest_prod.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.938316 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.938316 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-printers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-death-test-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-filepath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61622 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-internal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-linked_ptr.h
+-rw-r--r--   0 runner    (1001) docker     (123)   192179 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h.pump
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port-arch.h
+-rw-r--r--   0 runner    (1001) docker     (123)    85257 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-string.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h.pump
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h.pump
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.942316 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-all.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    62109 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-death-test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-filepath.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    47373 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-internal-inl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-matchers.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    48099 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-port.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-printers.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-test-part.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-typed-test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)   248867 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest_main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/memtest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/urdf_double_convert.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/urdf_unit_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/lib/urdf_parser/test/urdf_version_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 22:06:42.946317 ik_solvers-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.942316 ik_solvers-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/ForwardDynamicsSolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/IKSolver.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.942316 ik_solvers-1.0.2/src/PyIKSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyIKSolver/pybindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.942316 ik_solvers-1.0.2/src/PyKDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL/PyKDL.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL/PyKDL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL/dynamics.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL/frames.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL/framevel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28725 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL/kinfam.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.942316 ik_solvers-1.0.2/src/PyKDL_Parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/src/PyKDL_Parser/py_kdl_parser.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:42.946317 ik_solvers-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/PyKDLtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/dynamicstest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/framestest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/frameveltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/kinfamtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-06-13 22:06:17.000000 ik_solvers-1.0.2/tests/ur10e.urdf
```

### Comparing `ik_solvers-1.0.1/.github/workflows/python-publish.yml` & `ik_solvers-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/.github/workflows/test-build.yml` & `ik_solvers-1.0.2/.github/workflows/test-build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,16 @@
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         sudo apt-get install libeigen3-dev libtinyxml-dev
         python -m pip install --upgrade pip
         pip install build
+        pip install psutil
     - name: Build package
       run: python3 -m build --sdist --wheel --outdir dist/
     - name: Build and install package
       run: pip install .
     - name: Run tests
       run: |
         python3 -m unittest tests/test_solvers.py
+        python3 -m unittest tests/PyKDLtest.py
```

### Comparing `ik_solvers-1.0.1/.gitignore` & `ik_solvers-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/CMakeLists.txt` & `ik_solvers-1.0.2/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -27,42 +27,70 @@
 )
 set(LIB_HEADER_FILES
   include/Utility.h
   include/IKSolver.h
   include/ForwardDynamicsSolver.h
   include/kdl_parser.hpp
 )
+
 add_subdirectory(lib/urdf_parser)
 add_subdirectory(lib/orocos_kdl)
 
 get_target_property(KDL_HEADERS orocos-kdl PUBLIC_HEADER)
 file(GLOB KDL_UTIL_HPPS ${orocos_kdl_SOURCE_DIR}/src/utilities/[^.]*.h ${orocos_kdl_SOURCE_DIR}/src/utilities/[^.]*.hpp)
 
 file(COPY ${KDL_HEADERS} DESTINATION ${orocos_kdl_BINARY_DIR}/include/kdl)
 file(COPY ${KDL_UTIL_HPPS} DESTINATION ${orocos_kdl_BINARY_DIR}/include/kdl/utilities)
 
 pybind11_add_module(PyIKSolver
 ${LIB_SOURCE_FILES} 
 ${LIB_HEADER_FILES}
-src/pybindings.cpp
+src/PyIKSolver/pybindings.cpp
 )
+pybind11_add_module(PyKDL
+  src/PyKDL/PyKDL.h
+  src/PyKDL/PyKDL.cpp
+  src/PyKDL/frames.cpp
+  src/PyKDL/kinfam.cpp
+  src/PyKDL/framevel.cpp
+  src/PyKDL/dynamics.cpp)
+
+pybind11_add_module(PyKDL_Parser
+  src/PyKDL_Parser/py_kdl_parser.cpp)
 target_include_directories(PyIKSolver PRIVATE
 include 
 ${EIGEN3_INCLUDE_DIR}
 ${PYBIND11_INCLUDE_DIR} 
 ${orocos_kdl_BINARY_DIR}/include
 )
+target_include_directories(PyKDL PRIVATE
+${EIGEN3_INCLUDE_DIR}
+${PYBIND11_INCLUDE_DIR} 
+${orocos_kdl_BINARY_DIR}/include
+)
+target_include_directories(PyKDL_Parser PRIVATE
+include
+${EIGEN3_INCLUDE_DIR}
+${PYBIND11_INCLUDE_DIR} 
+${orocos_kdl_BINARY_DIR}/include
+)
 
 target_link_libraries(PyIKSolver PRIVATE
 urdf_parser
 orocos-kdl
 )
-
-get_target_property(inc_dirs PyIKSolver INCLUDE_DIRECTORIES)
-message("INCLUDE_DIRECTORIES = ${inc_dirs}")
+target_link_libraries(PyKDL PRIVATE
+orocos-kdl
+)
+target_link_libraries(PyKDL_Parser PRIVATE
+urdf_parser
+orocos-kdl
+)
+# get_target_property(inc_dirs PyIKSolver INCLUDE_DIRECTORIES)
+# message("INCLUDE_DIRECTORIES = ${inc_dirs}")
 
 # message(orocos_kdl_lib = ${orocos_kdl_BINARY_DIR})
 # message(orocos_kdl_headers = ${KDL_HEADERS})
 # configure_file(${KDL_HEADERS} ${orocos_kdl_BINARY_DIR}/include/kdl COPYONLY)
 # message(orocos_kdl_SOURCE_DIR = ${orocos_kdl_SOURCE_DIR})
```

### Comparing `ik_solvers-1.0.1/LICENSE` & `ik_solvers-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/README.md` & `ik_solvers-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/ik_solvers.egg-info/SOURCES.txt` & `ik_solvers-1.0.2/ik_solvers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -339,10 +339,23 @@
 lib/urdf_parser/test/gtest/src/gtest-printers.cc
 lib/urdf_parser/test/gtest/src/gtest-test-part.cc
 lib/urdf_parser/test/gtest/src/gtest-typed-test.cc
 lib/urdf_parser/test/gtest/src/gtest.cc
 lib/urdf_parser/test/gtest/src/gtest_main.cc
 src/ForwardDynamicsSolver.cpp
 src/IKSolver.cpp
-src/pybindings.cpp
+src/PyIKSolver/pybindings.cpp
+src/PyKDL/PyKDL.cpp
+src/PyKDL/PyKDL.h
+src/PyKDL/dynamics.cpp
+src/PyKDL/frames.cpp
+src/PyKDL/framevel.cpp
+src/PyKDL/kinfam.cpp
+src/PyKDL_Parser/py_kdl_parser.cpp
+tests/PyKDLtest.py
+tests/__init__.py
+tests/dynamicstest.py
+tests/framestest.py
+tests/frameveltest.py
+tests/kinfamtest.py
 tests/test_solvers.py
 tests/ur10e.urdf
```

### Comparing `ik_solvers-1.0.1/include/ForwardDynamicsSolver.h` & `ik_solvers-1.0.2/include/ForwardDynamicsSolver.h`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
               const KDL::JntArray& lower_pos_limits);
 
   private:
 
     //! Build a generic robot model for control
     bool buildGenericModel();
 
+    void boundAcc();
     // Forward dynamics
     std::shared_ptr<KDL::ChainJntToJacSolver> m_jnt_jacobian_solver;
     std::shared_ptr<KDL::ChainDynParam>       m_jnt_space_inertia_solver;
     KDL::Jacobian                               m_jnt_jacobian;
     KDL::JntSpaceInertiaMatrix                  m_jnt_space_inertia;
 
     // IK solver specific dynamic reconfigure
```

### Comparing `ik_solvers-1.0.1/include/IKSolver.h` & `ik_solvers-1.0.2/include/IKSolver.h`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
      * @param net_force The applied net force, expressed in the root frame
      *
      * @return A point holding positions, velocities and accelerations of each joint
      */
     virtual std::vector<double> getJointControlCmds(
         double period,
         const ctrl::Vector6D& net_force) = 0;
-    const std::vector<double> forwardKinematics(const std::vector<double>& joint_positions, const std::string& segment_name);
+    // const std::vector<double> forwardKinematics(const std::vector<double>& joint_positions, const std::string& segment_name);
 
     const std::vector<double> getEndEffectorPose6D() const;
     /**
      * @brief Get the current end effector pose of the simulated robot
      *
      * The last link in the chain from the init() function is taken as end
      * effector. If \ref setStartState() has been called immediately before,
```

### Comparing `ik_solvers-1.0.1/include/SolverLoader.h` & `ik_solvers-1.0.2/include/SolverLoader.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/include/Utility.h` & `ik_solvers-1.0.2/include/Utility.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/include/kdl_parser.hpp` & `ik_solvers-1.0.2/include/kdl_parser.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -179,10 +179,17 @@
 
 bool treeFromFile(const std::string & file, KDL::Tree & tree)
 {
   const urdf::ModelInterfaceSharedPtr robot_model = urdf::parseURDFFile(file);
   return kdl_parser::treeFromUrdfModel(*robot_model, tree);
 }
 
+KDL::Tree treeFromFile(const std::string& file)
+{
+  const urdf::ModelInterfaceSharedPtr robot_model = urdf::parseURDFFile(file);
+  KDL::Tree tree;
+  kdl_parser::treeFromUrdfModel(*robot_model, tree);
+  return tree;
+}
 
 
 }  // namespace kdl_parser
```

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/CMakeLists.txt` & `ik_solvers-1.0.2/lib/orocos_kdl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/COPYING` & `ik_solvers-1.0.2/lib/orocos_kdl/COPYING`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/INSTALL.md` & `ik_solvers-1.0.2/lib/orocos_kdl/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/cmake/CheckSTLContainers.cmake` & `ik_solvers-1.0.2/lib/orocos_kdl/cmake/CheckSTLContainers.cmake`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/cmake/FindEigen3.cmake` & `ik_solvers-1.0.2/lib/orocos_kdl/cmake/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/cmake/FindPkgConfig.cmake` & `ik_solvers-1.0.2/lib/orocos_kdl/cmake/FindPkgConfig.cmake`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/cmake_uninstall.cmake.in` & `ik_solvers-1.0.2/lib/orocos_kdl/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/debian/control` & `ik_solvers-1.0.2/lib/orocos_kdl/debian/control`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/debian/copyright` & `ik_solvers-1.0.2/lib/orocos_kdl/debian/copyright`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/debian/manpage.1.ex` & `ik_solvers-1.0.2/lib/orocos_kdl/debian/manpage.1.ex`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/debian/rules` & `ik_solvers-1.0.2/lib/orocos_kdl/debian/rules`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/doc/Doxyfile.in` & `ik_solvers-1.0.2/lib/orocos_kdl/doc/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/doc/tests.txt` & `ik_solvers-1.0.2/lib/orocos_kdl/doc/tests.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/doc/tex/UserManual.tex` & `ik_solvers-1.0.2/lib/orocos_kdl/doc/tex/UserManual.tex`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/examples/chainiksolverpos_lma_demo.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/examples/chainiksolverpos_lma_demo.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/examples/geometry.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/examples/geometry.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/examples/trajectory_example.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/examples/trajectory_example.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/examples/visualize_trajectory.m` & `ik_solvers-1.0.2/lib/orocos_kdl/examples/visualize_trajectory.m`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/manifest.xml` & `ik_solvers-1.0.2/lib/orocos_kdl/manifest.xml`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/CMakeLists.txt` & `ik_solvers-1.0.2/lib/orocos_kdl/models/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/kukaLWR_DHnew.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/models/kukaLWR_DHnew.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/kukaLWRtestDHnew.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/models/kukaLWRtestDHnew.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/kukaLWRtestHCG.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/models/kukaLWRtestHCG.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/models.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/models/models.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/puma560.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/models/puma560.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/models/puma560test.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/models/puma560test.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/orocos_kdl-config.cmake.in` & `ik_solvers-1.0.2/lib/orocos_kdl/orocos_kdl-config.cmake.in`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/package.xml` & `ik_solvers-1.0.2/lib/orocos_kdl/package.xml`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/CMakeLists.txt` & `ik_solvers-1.0.2/lib/orocos_kdl/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/articulatedbodyinertia.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/articulatedbodyinertia.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/articulatedbodyinertia.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/articulatedbodyinertia.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chain.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chain.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chain.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chain.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chaindynparam.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chaindynparam.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chaindynparam.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chaindynparam.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainexternalwrenchestimator.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainexternalwrenchestimator.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainexternalwrenchestimator.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainexternalwrenchestimator.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfdsolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfdsolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfdsolver_recursive_newton_euler.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolverpos_recursive.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolverpos_recursive.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolverpos_recursive.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolverpos_recursive.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolvervel_recursive.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolvervel_recursive.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainfksolvervel_recursive.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainfksolvervel_recursive.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainhdsolver_vereshchagin.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainhdsolver_vereshchagin.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainhdsolver_vereshchagin.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainhdsolver_vereshchagin.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_recursive_newton_euler.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_vereshchagin.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_vereshchagin.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainidsolver_vereshchagin.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainidsolver_vereshchagin.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_lma.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_lma.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_lma.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_lma.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr_jl.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr_jl.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolverpos_nr_jl.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolverpos_nr_jl.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_givens.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_pinv_nso.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_wdls.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_wdls.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainiksolvervel_wdls.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainiksolvervel_wdls.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacdotsolver.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacdotsolver.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacdotsolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacdotsolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacsolver.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacsolver.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/chainjnttojacsolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/chainjnttojacsolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/config.h.in` & `ik_solvers-1.0.2/lib/orocos_kdl/src/config.h.in`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc.inl` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc.inl`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frameacc_io.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frameacc_io.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frames.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frames.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frames.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frames.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frames.inl` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frames.inl`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frames_io.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frames_io.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/frames_io.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/frames_io.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/framevel.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/framevel.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/framevel.inl` & `ik_solvers-1.0.2/lib/orocos_kdl/src/framevel.inl`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/framevel_io.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/framevel_io.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jacobian.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jacobian.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jacobian.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jacobian.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntarray.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntarray.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntarray.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntarray.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayacc.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayacc.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayacc.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayacc.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayvel.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayvel.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntarrayvel.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntarrayvel.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntspaceinertiamatrix.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntspaceinertiamatrix.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/jntspaceinertiamatrix.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/jntspaceinertiamatrix.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/joint.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/joint.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/joint.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/joint.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/kdl.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/kdl.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/kinfam.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/kinfam.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/kinfam_io.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/kinfam_io.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/kinfam_io.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/kinfam_io.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/motion.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/motion.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_circle.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_circle.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_circle.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_circle.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_composite.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_composite.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_composite.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_composite.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_cyclic_closed.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_cyclic_closed.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_cyclic_closed.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_cyclic_closed.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_line.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_line.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_line.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_line.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_point.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_point.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_point.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_point.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_roundedcomposite.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_roundedcomposite.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/path_roundedcomposite.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/path_roundedcomposite.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rigidbodyinertia.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rigidbodyinertia.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rigidbodyinertia.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rigidbodyinertia.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation_sa.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation_sa.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rotational_interpolation_sa.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rotational_interpolation_sa.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rotationalinertia.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rotationalinertia.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/rotationalinertia.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/rotationalinertia.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/segment.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/segment.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/segment.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/segment.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/solveri.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/solveri.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/stiffness.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/stiffness.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_composite.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_composite.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_composite.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_composite.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_segment.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_segment.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_segment.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_segment.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_stationary.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_stationary.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/trajectory_stationary.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/trajectory_stationary.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/tree.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/tree.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/tree.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/tree.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treefksolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treefksolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treefksolverpos_recursive.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treefksolverpos_recursive.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treefksolverpos_recursive.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treefksolverpos_recursive.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeidsolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeidsolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeidsolver_recursive_newton_euler.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_nr_jl.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_nr_jl.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_nr_jl.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_nr_jl.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_online.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_online.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolverpos_online.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolverpos_online.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolvervel_wdls.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolvervel_wdls.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treeiksolvervel_wdls.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treeiksolvervel_wdls.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treejnttojacsolver.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treejnttojacsolver.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/treejnttojacsolver.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/treejnttojacsolver.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/error.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/error.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/error_stack.cxx` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/error_stack.cxx`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/error_stack.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/error_stack.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/hash_combine.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/hash_combine.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/header.txt` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/header.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/kdl-config.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/kdl-config.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/ldl_solver_eigen.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/ldl_solver_eigen.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/ldl_solver_eigen.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/ldl_solver_eigen.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall1d.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall1d.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall1d_io.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall1d_io.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall2d.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall2d.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rall2d_io.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rall2d_io.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/rallNd.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/rallNd.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/scoped_ptr.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/scoped_ptr.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_HH.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_HH.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_HH.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_HH.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_HH.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_HH.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_HH.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_HH.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_Macie.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_Macie.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/svd_eigen_Macie.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/svd_eigen_Macie.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/traits.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/traits.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility.cxx` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility.cxx`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility_io.cxx` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility_io.cxx`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/utilities/utility_io.h` & `ik_solvers-1.0.2/lib/orocos_kdl/src/utilities/utility_io.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_dirac.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_dirac.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_dirac.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_dirac.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_rect.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_rect.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_rect.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_rect.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_spline.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_spline.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_spline.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_spline.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_trap.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_trap.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_trap.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_trap.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_traphalf.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_traphalf.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/src/velocityprofile_traphalf.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/src/velocityprofile_traphalf.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/CMakeLists.txt` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/framestest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/framestest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/framestest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/framestest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/inertiatest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/inertiatest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/iotest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/iotest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandottest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandottest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandottest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandottest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiandoubletests.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiandoubletests.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobianframetests.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobianframetests.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/jacobiantests.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/jacobiantests.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/kinfamtest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/kinfamtest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/kinfamtest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/kinfamtest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/rallnumbertest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/rallnumbertest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/rframestest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/rframestest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/serialchaintest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/serialchaintest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/solvertest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/solvertest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/solvertest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/solvertest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/test-runner.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/test-runner.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/toolkittest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/toolkittest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/treeinvdyntest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/treeinvdyntest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/treeinvdyntest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/treeinvdyntest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/velocityprofiletest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/velocityprofiletest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/velocityprofiletest.hpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/velocityprofiletest.hpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/orocos_kdl/tests/zxxzxztest.cpp` & `ik_solvers-1.0.2/lib/orocos_kdl/tests/zxxzxztest.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/CMakeLists.txt` & `ik_solvers-1.0.2/lib/urdf_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/console_bridge/console.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/console_bridge/console.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/console_bridge/console_bridge_export.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/console_bridge/console_bridge_export.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_exception/exception.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_exception/exception.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/color.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/color.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/joint.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/joint.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/link.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/link.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/model.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/model.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/pose.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/pose.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/twist.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/twist.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/types.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/types.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model/utils.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model/utils.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/model_state.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/model_state.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/twist.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/twist.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_model_state/types.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_model_state/types.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_parser/exportdecl.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_parser/exportdecl.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_parser/urdf_parser.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_parser/urdf_parser.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_sensor/sensor.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_sensor/sensor.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_sensor/types.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_sensor/types.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_world/types.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_world/types.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/include/urdf_world/world.h` & `ik_solvers-1.0.2/lib/urdf_parser/include/urdf_world/world.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/check_urdf.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/check_urdf.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/console.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/console.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/joint.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/joint.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/link.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/link.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/model.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/model.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/pose.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/pose.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/twist.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/twist.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/urdf_model_state.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/urdf_model_state.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/urdf_sensor.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/urdf_sensor.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/urdf_to_graphviz.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/urdf_to_graphviz.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/src/world.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/src/world.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/CMakeLists.txt` & `ik_solvers-1.0.2/lib/urdf_parser/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/cmake/internal_utils.cmake` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/cmake/internal_utils.cmake`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-death-test.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-death-test.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-matchers.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-matchers.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-message.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-message.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h.pump` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-param-test.h.pump`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-printers.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-spi.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-test-part.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-test-part.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest-typed-test.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest-typed-test.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest_pred_impl.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest_pred_impl.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/gtest_prod.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/gtest_prod.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/README.md` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/README.md`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-port.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-port.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-printers.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/custom/gtest.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-death-test-internal.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-death-test-internal.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-filepath.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-filepath.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-internal.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-internal.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-linked_ptr.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-linked_ptr.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h.pump` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util-generated.h.pump`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-param-util.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port-arch.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port-arch.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-port.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-string.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-string.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h.pump` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-tuple.h.pump`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h.pump` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/include/gtest/internal/gtest-type-util.h.pump`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-all.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-death-test.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-death-test.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-filepath.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-filepath.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-internal-inl.h` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-internal-inl.h`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-matchers.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-matchers.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-port.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-port.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-printers.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-printers.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-test-part.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-test-part.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest-typed-test.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest-typed-test.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/gtest/src/gtest_main.cc` & `ik_solvers-1.0.2/lib/urdf_parser/test/gtest/src/gtest_main.cc`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/urdf_double_convert.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/test/urdf_double_convert.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/urdf_unit_test.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/test/urdf_unit_test.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/lib/urdf_parser/test/urdf_version_test.cpp` & `ik_solvers-1.0.2/lib/urdf_parser/test/urdf_version_test.cpp`

 * *Files identical despite different names*

### Comparing `ik_solvers-1.0.1/setup.py` & `ik_solvers-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def __init__(self, user=False):
         self.user = user
 
     def __str__(self):
         import pybind11
         return pybind11.get_include(self.user)
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 
 setup(
     name="ik_solvers",
     version=__version__,
     author="Zongyao Yi",
     author_email="zongyao.yi@dfki.de",
```

### Comparing `ik_solvers-1.0.1/src/ForwardDynamicsSolver.cpp` & `ik_solvers-1.0.2/src/ForwardDynamicsSolver.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
     // Compute joint jacobian
     m_jnt_jacobian_solver->JntToJac(m_current_positions,m_jnt_jacobian);
 
     // Compute joint accelerations according to: \f$ \ddot{q} = H^{-1} ( J^T f) \f$
     m_current_accelerations.data = m_jnt_space_inertia.data.inverse() * m_jnt_jacobian.data.transpose() * net_force;
 
+    boundAcc();
     // Numerical time integration with the Euler forward method
     m_current_positions.data = m_last_positions.data + m_last_velocities.data * period;
     m_current_velocities.data = m_last_velocities.data + m_current_accelerations.data * period;
     m_current_velocities.data *= 0.9;  // 10 % global damping against unwanted null space motion.
                                        // Will cause exponential slow-down without input.
 
     // Make sure positions stay in allowed margins
@@ -123,14 +124,29 @@
     // Update for the next cycle
     m_last_positions = m_current_positions;
     m_last_velocities = m_current_velocities;
 
     return control_cmd;
   }
 
+  void ForwardDynamicsSolver::boundAcc()
+  {
+    for (int i = 0; i < m_number_joints; ++i)
+    {
+      if (std::isnan(m_lower_pos_limits(i)) || std::isnan(m_upper_pos_limits(i)))
+      {
+        // Joint marked as continuous.
+        continue;
+      }
+      if ((m_current_positions(i) > (m_upper_pos_limits(i) - 0.1)) &&  m_current_accelerations(i) > 0)
+        m_current_accelerations(i) = -0.01;
+      if((m_current_positions(i) < (m_lower_pos_limits(i) + 0.1)) && m_current_accelerations(i) < 0)
+        m_current_accelerations(i) = 0.01;
+    }
+  }
 
   bool ForwardDynamicsSolver::init(const KDL::Chain& chain,
                                    const KDL::JntArray& upper_pos_limits,
                                    const KDL::JntArray& lower_pos_limits)
   {
     IKSolver::init(chain, upper_pos_limits, lower_pos_limits);
```

### Comparing `ik_solvers-1.0.1/src/IKSolver.cpp` & `ik_solvers-1.0.2/src/IKSolver.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -67,34 +67,15 @@
     return pose;
   }
 
   const KDL::Frame& IKSolver::getEndEffectorPose() const
   {
     return m_end_effector_pose;
   }
-  const std::vector<double> IKSolver::forwardKinematics(const std::vector<double>& joint_positions, const std::string& segment_name)
-  {
-    KDL::JntArray j_pos(m_number_joints);
-    KDL::Frame segment_pose;
-    std::vector<double> segment_pose_6d;
-    for(int i = 0; i < m_number_joints; i++)
-    {
-      j_pos(i) = joint_positions[i];
-    }
-    m_fk_pos_solver->JntToCart(j_pos, segment_pose);
-    auto pos = segment_pose.p;
-    auto rot = segment_pose.M.GetRot();
-    segment_pose_6d.push_back(pos.x());
-    segment_pose_6d.push_back(pos.y());
-    segment_pose_6d.push_back(pos.z());
-    segment_pose_6d.push_back(rot.x());
-    segment_pose_6d.push_back(rot.y());
-    segment_pose_6d.push_back(rot.z());
-    return segment_pose_6d;
-  }
+
   const ctrl::Vector6D& IKSolver::getEndEffectorVel() const
   {
     return m_end_effector_vel;
   }
 
   const KDL::JntArray& IKSolver::getPositions() const
   {
@@ -143,16 +124,22 @@
     for (int i = 0; i < m_number_joints; ++i)
     {
       if (std::isnan(m_lower_pos_limits(i)) || std::isnan(m_upper_pos_limits(i)))
       {
         // Joint marked as continuous.
         continue;
       }
-      m_current_positions(i) = ctrl::clip(
-          m_current_positions(i),m_lower_pos_limits(i),m_upper_pos_limits(i));
+      if ((m_current_positions(i) > m_upper_pos_limits(i)) 
+      && (m_current_velocities(i) > 0))
+        m_current_velocities(i) = -0.1;
+      if((m_current_positions(i) < m_lower_pos_limits(i)) 
+      && (m_current_velocities(i) < 0))
+        m_current_velocities(i) = 0.1;
+      // m_current_positions(i) = ctrl::clip(
+      //     m_current_positions(i),m_lower_pos_limits(i),m_upper_pos_limits(i));
     }
   }
   bool IKSolver::setStartState(const std::vector<double>& joint_positions, const std::vector<double>& joint_velocities)
   {
     // Copy into internal buffers.
     for (size_t i = 0; i < joint_positions.size(); ++i)
     {
```

### Comparing `ik_solvers-1.0.1/src/pybindings.cpp` & `ik_solvers-1.0.2/src/PyIKSolver/pybindings.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/eigen.h>
 // #include <SolverLoader.h>
 #include <IKSolver.h>
 #include <ForwardDynamicsSolver.h>
 #include <kdl_parser.hpp>
+#include <kdl/treefksolverpos_recursive.hpp>
+#include <sstream>
 
-#define IKSolver_VERSION_STRING "1.0.1"
+#define IKSolver_VERSION_STRING "1.0.2"
 namespace py = pybind11;
 using namespace ik_solvers;
+using namespace KDL;
 
 namespace ik_solvers
 {
     std::shared_ptr<IKSolver> load(
     const std::string ik_solver_name, 
     const std::string urdf_file_path,
     const std::string robot_base_link,
@@ -87,34 +90,37 @@
             py::arg("joint_limits_lower"),
             py::arg("joint_limits_upper"),
             py::call_guard<py::gil_scoped_release>()
         );
 
         py::class_<IKSolver, IKSolverPy, std::shared_ptr<IKSolver>>(m, "IKSolver")
             .def(py::init<>())
+            .def("init", 
+                &IKSolver::init,
+                py::arg("chain"),
+                py::arg("upper_pos_limits"),
+                py::arg("lower_pos_limits"),
+                py::call_guard<py::gil_scoped_release>())
             .def("setStartState", 
                 &IKSolver::setStartState,
                 py::arg("joint_positions"),
                 py::arg("joint_velocities"),
                 py::call_guard<py::gil_scoped_release>())
-            .def("forwardKinematics",
-                &IKSolver::forwardKinematics,
-                py::arg("joint_positions"),
-                py::arg("segment_name"),
-                py::call_guard<py::gil_scoped_release>())
             .def("getEndEffectorPose", 
-                &IKSolver::getEndEffectorPose6D,
+                &IKSolver::getEndEffectorPose,
                 py::call_guard<py::gil_scoped_release>())
             .def("updateKinematics", &IKSolver::updateKinematics,
                 py::call_guard<py::gil_scoped_release>())
             .def("getJointControlCmds",&IKSolver::getJointControlCmds,
                 py::arg("period"),
                 py::arg("net_force"),
                 py::call_guard<py::gil_scoped_release>())
             .def("synchronizeJointPositions", &IKSolver::synchronizeJointPositions,
                 py::arg("joint_positions"),
-                py::call_guard<py::gil_scoped_release>());
+                py::call_guard<py::gil_scoped_release>())
+            .def("getPositions", &IKSolver::getPositions);
         
-        py::class_<ForwardDynamicsSolver, IKSolver, ForwardDynamicsSolverPy, std::shared_ptr<ForwardDynamicsSolver>>(m, "ForwardDynamicsSolver");
+        py::class_<ForwardDynamicsSolver, IKSolver, ForwardDynamicsSolverPy, std::shared_ptr<ForwardDynamicsSolver>>(m, "ForwardDynamicsSolver")
+            .def(py::init<>());
     }
 
 }
```

### Comparing `ik_solvers-1.0.1/tests/test_solvers.py` & `ik_solvers-1.0.2/tests/test_solvers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 import unittest
 class TestLoad(unittest.TestCase):
     def test_load(self):
         urdf_file = os.path.join(os.path.dirname(__file__), "ur10e.urdf")
         try:
-            from ik_solvers import PyIKSolver
-            ik_solver = PyIKSolver.load("forward_dynamics",urdf_file,"base_link","ft_sensor",[-3.14,-3.14,-3.14,-3.14,-3.14,-3.14], [3.14,3.14,3.14,3.14,3.14,3.14])
+            from ik_solvers import PyIKSolver, PyKDL, PyKDL_Parser
+            base_link = "base_link"
+            eef_link = "ft_sensor"
+            robot_chain = PyKDL_Parser.treeFromFile(urdf_file).getChain(base_link, eef_link)
+            ik_solver = PyIKSolver.ForwardDynamicsSolver()
+            ik_solver.init(robot_chain, PyKDL.JntArray(6), PyKDL.JntArray(6))
+            # ik_solver = PyIKSolver.load("forward_dynamics",urdf_file,"base_link","ft_sensor",[-3.14,-3.14,-3.14,-3.14,-3.14,-3.14], [3.14,3.14,3.14,3.14,3.14,3.14])
             ik_solver.setStartState([0,0,0,0,0,0],[0,0,0,0,0,0])
         except Exception as e:
             self.fail(f"PyIKSolver.load() raised Exception: {e.msg}")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ik_solvers-1.0.1/tests/ur10e.urdf` & `ik_solvers-1.0.2/tests/ur10e.urdf`

 * *Files identical despite different names*

