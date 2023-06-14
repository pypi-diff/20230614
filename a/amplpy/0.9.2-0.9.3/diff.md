# Comparing `tmp/amplpy-0.9.2.tar.gz` & `tmp/amplpy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amplpy-0.9.2.tar", last modified: Wed Apr  5 08:45:24 2023, max compression
+gzip compressed data, was "amplpy-0.9.3.tar", last modified: Fri Apr 21 13:44:29 2023, max compression
```

## Comparing `amplpy-0.9.2.tar` & `amplpy-0.9.3.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/
--rw-r--r--   0 vsts      (1001) docker     (122)     1527 2023-04-05 08:45:15.000000 amplpy-0.9.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)     3339 2023-04-05 08:45:24.904900 amplpy-0.9.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5032 2023-04-05 08:45:15.000000 amplpy-0.9.2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.892901 amplpy-0.9.2/amplpy/
--rw-r--r--   0 vsts      (1001) docker     (122)     1905 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    31506 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/ampl.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.892901 amplpy-0.9.2/amplpy/amplpython/
--rw-r--r--   0 vsts      (1001) docker     (122)      781 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/amplpython/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.892901 amplpy-0.9.2/amplpy/amplpython/cppinterface/
--rw-r--r--   0 vsts      (1001) docker     (122)     2210 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/amplpython.py
--rw-r--r--   0 vsts      (1001) docker     (122)  2657730 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.cxx
--rw-r--r--   0 vsts      (1001) docker     (122)     4969 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.892901 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/
--rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.896901 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/
--rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)    29663 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ampl.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5175 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/amplexception.h
--rw-r--r--   0 vsts      (1001) docker     (122)    19342 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/dataframe.h
--rw-r--r--   0 vsts      (1001) docker     (122)    39615 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/entity.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/entitymap.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4543 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/environment.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.896901 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/
--rw-r--r--   0 vsts      (1001) docker     (122)     8344 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/ampl_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)      775 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/arg.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2618 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/countediterator.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5231 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/dataframe_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)      979 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/declarations.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10323 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/entity_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16028 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/entitymap_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4099 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/environment_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)      785 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/error_information.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2591 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/errorinfo_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)    18593 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/format.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4536 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/instance_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3160 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/scopedarray.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2454 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/slice.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1245 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/tuple_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/variant_ep.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1026 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/errorhandler.h
--rw-r--r--   0 vsts      (1001) docker     (122)   128009 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/format.h
--rw-r--r--   0 vsts      (1001) docker     (122)    22617 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/instance.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1643 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/optional.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5138 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/output.h
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/runnable.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7468 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/string.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7978 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/tuple.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8783 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/variant.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.896901 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/
--rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/.gitignore
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.896901 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/aarch64/
--rw-r--r--   0 vsts      (1001) docker     (122)  1025216 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/aarch64/libampl.so
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.900900 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/
--rw-r--r--   0 vsts      (1001) docker     (122)   451072 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/ampl-2.0.12.dll
--rw-r--r--   0 vsts      (1001) docker     (122)    87566 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/ampl.lib
--rw-r--r--   0 vsts      (1001) docker     (122)  1309280 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/libampl.dylib
--rw-r--r--   0 vsts      (1001) docker     (122)   829592 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/libampl.so
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.900900 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/ppc64le/
--rw-r--r--   0 vsts      (1001) docker     (122)  1221728 2023-04-05 08:45:21.000000 amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/ppc64le/libampl.so
--rw-r--r--   0 vsts      (1001) docker     (122)      457 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6290 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/constraint.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13973 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7328 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/entity.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2859 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1102 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/errorhandler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1461 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2064 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/iterators.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.900900 amplpy-0.9.2/amplpy/modules/
--rw-r--r--   0 vsts      (1001) docker     (122)      507 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/modules/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/modules/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2519 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/objective.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6988 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/outputhandler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4159 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/parameter.py
--rw-r--r--   0 vsts      (1001) docker     (122)      851 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/runnable.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4079 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/set.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)     1417 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/TestBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      397 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/context.py
--rw-r--r--   0 vsts      (1001) docker     (122)       29 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/data.csv
--rw-r--r--   0 vsts      (1001) docker     (122)    12901 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/test_ampl.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10474 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/test_dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15744 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/test_entities.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1653 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/test_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9748 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/test_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests/test_properties.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/tests_camel/
--rw-r--r--   0 vsts      (1001) docker     (122)     1408 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/TestBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      397 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/context.py
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/data.csv
--rw-r--r--   0 vsts      (1001) docker     (122)    11264 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/test_ampl.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10266 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/test_dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14747 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/test_entities.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1609 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/test_environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8674 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/test_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2115 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tests_camel/test_properties.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/tools/
--rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/tools/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1523 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5246 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/variable.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/vendor/
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)     2758 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/CHANGELOG.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1522 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       57 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)      446 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/vendor/ampltools/
--rw-r--r--   0 vsts      (1001) docker     (122)      407 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/vendor/ampltools/modules/
--rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/modules/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       93 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/modules/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12304 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/modules/amplpypi.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3723 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/modules/commands.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6017 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/notebooks.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.904900 amplpy-0.9.2/amplpy/vendor/ampltools/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/TestBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      286 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3566 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_install.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1951 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_load.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2411 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_preload.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1751 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3228 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/ampltools/utils.py
--rwxr-xr-x   0 vsts      (1001) docker     (122)      333 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/bumpversion.sh
--rw-r--r--   0 vsts      (1001) docker     (122)      493 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/clear.sh
--rwxr-xr-x   0 vsts      (1001) docker     (122)      262 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/register.sh
--rw-r--r--   0 vsts      (1001) docker     (122)        8 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     1651 2023-04-05 08:45:15.000000 amplpy-0.9.2/amplpy/vendor/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-05 08:45:24.892901 amplpy-0.9.2/amplpy.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     3339 2023-04-05 08:45:24.000000 amplpy-0.9.2/amplpy.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4542 2023-04-05 08:45:24.000000 amplpy-0.9.2/amplpy.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-05 08:45:24.000000 amplpy-0.9.2/amplpy.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       32 2023-04-05 08:45:24.000000 amplpy-0.9.2/amplpy.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-04-05 08:45:24.000000 amplpy-0.9.2/amplpy.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-04-05 08:45:24.904900 amplpy-0.9.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     6313 2023-04-05 08:45:15.000000 amplpy-0.9.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1527 2023-04-21 13:44:23.000000 amplpy-0.9.3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     4168 2023-04-21 13:44:29.840483 amplpy-0.9.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5890 2023-04-21 13:44:23.000000 amplpy-0.9.3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.816482 amplpy-0.9.3/amplpy/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1905 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30660 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/ampl.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.820482 amplpy-0.9.3/amplpy/amplpython/
+-rw-r--r--   0 vsts      (1001) docker     (122)      781 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/amplpython/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.820482 amplpy-0.9.3/amplpy/amplpython/cppinterface/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2210 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/amplpython.py
+-rw-r--r--   0 vsts      (1001) docker     (122)  2657730 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.cxx
+-rw-r--r--   0 vsts      (1001) docker     (122)     4969 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.820482 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/
+-rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.824482 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/
+-rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)    29663 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ampl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5175 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/amplexception.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    19342 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/dataframe.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    39615 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/entity.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/entitymap.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4543 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/environment.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.828482 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/
+-rw-r--r--   0 vsts      (1001) docker     (122)     8344 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/ampl_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      775 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/arg.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2618 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/countediterator.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5231 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/dataframe_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      979 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/declarations.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10323 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/entity_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16028 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/entitymap_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4099 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/environment_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      785 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/error_information.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2591 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/errorinfo_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    18593 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/format.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4536 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/instance_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3160 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/scopedarray.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2454 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/slice.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1245 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/tuple_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/variant_ep.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1026 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/errorhandler.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   128009 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/format.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    22617 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/instance.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1643 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/optional.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5138 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/output.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/runnable.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7468 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/string.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7978 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/tuple.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8783 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/variant.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.828482 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/
+-rw-r--r--   0 vsts      (1001) docker     (122)       15 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/.gitignore
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.828482 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/aarch64/
+-rw-r--r--   0 vsts      (1001) docker     (122)  1025216 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/aarch64/libampl.so
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.832482 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/
+-rw-r--r--   0 vsts      (1001) docker     (122)   451072 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/ampl-2.0.12.dll
+-rw-r--r--   0 vsts      (1001) docker     (122)    87566 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/ampl.lib
+-rw-r--r--   0 vsts      (1001) docker     (122)  1309280 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/libampl.dylib
+-rw-r--r--   0 vsts      (1001) docker     (122)   829592 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/libampl.so
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.832482 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/ppc64le/
+-rw-r--r--   0 vsts      (1001) docker     (122)  1221728 2023-04-21 13:44:27.000000 amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/ppc64le/libampl.so
+-rw-r--r--   0 vsts      (1001) docker     (122)      457 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6255 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/constraint.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13651 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7294 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/entity.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2859 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1046 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/errorhandler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1461 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2064 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/iterators.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.836483 amplpy-0.9.3/amplpy/modules/
+-rw-r--r--   0 vsts      (1001) docker     (122)      507 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/modules/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/modules/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2484 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/objective.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6948 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/outputhandler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4090 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      714 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/runnable.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/set.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.836483 amplpy-0.9.3/amplpy/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1417 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/TestBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      397 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/context.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       29 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/data.csv
+-rw-r--r--   0 vsts      (1001) docker     (122)    12901 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/test_ampl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10474 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/test_dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15744 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/test_entities.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1653 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/test_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9748 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/test_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests/test_properties.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/amplpy/tests_camel/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1408 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/TestBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      397 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/context.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/data.csv
+-rw-r--r--   0 vsts      (1001) docker     (122)    11264 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/test_ampl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10266 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/test_dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14747 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/test_entities.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1609 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/test_environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8674 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/test_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2115 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tests_camel/test_properties.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/amplpy/tools/
+-rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/tools/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1523 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5211 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/variable.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/amplpy/vendor/
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)     2758 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1522 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       57 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)      446 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/amplpy/vendor/ampltools/
+-rw-r--r--   0 vsts      (1001) docker     (122)      407 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/amplpy/vendor/ampltools/modules/
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/modules/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       93 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/modules/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12304 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/modules/amplpypi.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3723 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/modules/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6017 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/notebooks.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.840483 amplpy-0.9.3/amplpy/vendor/ampltools/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/TestBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       24 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      286 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3566 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_install.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1951 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_load.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2411 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_preload.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1751 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3228 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/ampltools/utils.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      333 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/bumpversion.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)      493 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/clear.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      262 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/register.sh
+-rw-r--r--   0 vsts      (1001) docker     (122)        8 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1651 2023-04-21 13:44:23.000000 amplpy-0.9.3/amplpy/vendor/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-21 13:44:29.816482 amplpy-0.9.3/amplpy.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4168 2023-04-21 13:44:29.000000 amplpy-0.9.3/amplpy.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4542 2023-04-21 13:44:29.000000 amplpy-0.9.3/amplpy.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-21 13:44:29.000000 amplpy-0.9.3/amplpy.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       32 2023-04-21 13:44:29.000000 amplpy-0.9.3/amplpy.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-04-21 13:44:29.000000 amplpy-0.9.3/amplpy.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-04-21 13:44:29.840483 amplpy-0.9.3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     7142 2023-04-21 13:44:23.000000 amplpy-0.9.3/setup.py
```

### Comparing `amplpy-0.9.2/LICENSE` & `amplpy-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/PKG-INFO` & `amplpy-0.9.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplpy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python API for AMPL
 Home-page: http://ampl.com/
 Download-URL: https://github.com/ampl/amplpy
 Author: AMPL Optimization Inc.
 Author-email: devteam@ampl.com
 License: BSD-3
 Platform: any
@@ -50,14 +50,44 @@
 
 # Import in Python
 $ python
 >>> from amplpy import AMPL
 >>> ampl = AMPL() # instantiate AMPL object
 ```
 
+```python
+# Minimal example:
+from amplpy import AMPL
+import pandas as pd
+ampl = AMPL()
+ampl.eval(r"""
+    set A ordered;
+    param S{A, A};
+    param lb default 0;
+    param ub default 1;
+    var w{A} >= lb <= ub;
+    minimize portfolio_variance:
+        sum {i in A, j in A} w[i] * S[i, j] * w[j];
+    s.t. portfolio_weights:
+        sum {i in A} w[i] = 1;
+""")
+tickers, cov_matrix = # ... pre-process data in Python
+ampl.set["A"] = tickers
+ampl.param["S"] = pd.DataFrame(
+    cov_matrix, index=tickers, columns=tickers
+).unstack()
+ampl.option["solver"] = "gurobi"
+ampl.option["gurobi_options"] = "outlev=1"
+ampl.solve()
+assert ampl.get_value("solve_result") == "solved"
+sigma = ampl.get_value("sqrt(sum {i in A, j in A} w[i] * S[i, j] * w[j])")
+print(f"Volatility: {sigma*100:.1f}%")
+# ... post-process solution in Python
+```
+
 [[Documentation](https://amplpy.readthedocs.io/)] [[AMPL Modules for Python](https://dev.ampl.com/ampl/python/modules.html)] [[Available on Google Colab](https://colab.ampl.com/)] [[AMPL Community Edition](http://ampl.com/ce)]
 
 `amplpy` is an interface that allows developers to access the features of [AMPL](https://ampl.com) from within Python. For a quick introduction to AMPL see [Quick Introduction to AMPL](https://dev.ampl.com/ampl/introduction.html).
 
 In the same way that AMPL’s syntax matches naturally the mathematical description of the model, the input and output data matches naturally Python lists, sets, dictionaries, `pandas` and `numpy` objects.
 
 All model generation and solver interaction is handled directly by AMPL, which leads to great stability and speed; the library just acts as an intermediary, and the added overhead (in terms of memory and CPU usage) depends mostly on how much data is sent and read back from AMPL, the size of the expanded model as such is irrelevant.
```

### Comparing `amplpy-0.9.2/README.md` & `amplpy-0.9.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -11,16 +11,47 @@
 $ python -m amplpy.modules activate <license-uuid>
 
 # Import in Python
 $ python
 >>> from amplpy import AMPL
 >>> ampl = AMPL() # instantiate AMPL object
 ```
+```python
+# Minimal example:
+from amplpy import AMPL
+import pandas as pd
+ampl = AMPL()
+ampl.eval(r"""
+    set A ordered;
+    param S{A, A};
+    param lb default 0;
+    param ub default 1;
+    var w{A} >= lb <= ub;
+    minimize portfolio_variance:
+        sum {i in A, j in A} w[i] * S[i, j] * w[j];
+    s.t. portfolio_weights:
+        sum {i in A} w[i] = 1;
+""")
+tickers, cov_matrix = # ... pre-process data in Python
+ampl.set["A"] = tickers
+ampl.param["S"] = pd.DataFrame(
+    cov_matrix, index=tickers, columns=tickers
+).unstack()
+ampl.option["solver"] = "gurobi"
+ampl.option["gurobi_options"] = "outlev=1"
+ampl.solve()
+assert ampl.get_value("solve_result") == "solved"
+sigma = ampl.get_value("sqrt(sum {i in A, j in A} w[i] * S[i, j] * w[j])")
+print(f"Volatility: {sigma*100:.1f}%")
+# ... post-process solution in Python
+```
+
 
-[[Documentation](https://amplpy.readthedocs.io/)] [[AMPL Modules for Python](https://dev.ampl.com/ampl/python/modules.html)] [[Available on Google Colab](https://colab.ampl.com/)]
+
+[[Documentation](https://amplpy.readthedocs.io/)] [[AMPL Modules for Python](https://dev.ampl.com/ampl/python/modules.html)] [[AMPL on Streamlit](https://ampl.com/streamlit)] [[Available on Google Colab](https://colab.ampl.com/)]
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/amplpy?label=PyPI%20downloads)](https://pypistats.org/packages/amplpy)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/amplpy?label=Conda%20downloads)](https://anaconda.org/conda-forge/amplpy)
 [![Build Status](https://dev.azure.com/ampldev/amplpy/_apis/build/status/ampl.amplpy?branchName=master)](https://dev.azure.com/ampldev/amplpy/_build/latest?definitionId=9&branchName=test)
 [![build-and-test](https://github.com/ampl/amplpy/actions/workflows/build-and-test.yaml/badge.svg)](https://github.com/ampl/amplpy/actions/workflows/build-and-test.yaml)
 
 `amplpy` is an interface that allows developers to access the features of [AMPL](https://ampl.com) from within Python. For a quick introduction to AMPL see [Quick Introduction to AMPL](https://dev.ampl.com/ampl/introduction.html).
@@ -59,17 +90,18 @@
 - Conda-Forge: https://anaconda.org/conda-forge/amplpy
 
 ## Setup
 
 ### PyPI
 
 Install from the [PyPI repository](https://pypi.python.org/pypi/amplpy):
-    ```
-    python -m pip install amplpy
-    ```
+
+```
+python -m pip install amplpy
+```
 
 ### AMPL Modules for Python
 
 [AMPL and all Solvers are now available as Python Packages](https://dev.ampl.com/ampl/python/modules.html):
 
 - Install Python API for AMPL:
     ```
@@ -92,17 +124,18 @@
     >>> from amplpy import AMPL
     >>> ampl = AMPL() # instantiate AMPL object
     ```
 
 ### Conda
 
 Install from the [Conda repository](https://anaconda.org/conda-forge/amplpy):
-    ```
-    conda install -c conda-forge amplpy
-    ```
+
+```
+conda install -c conda-forge amplpy
+```
 
 ### Air-gapped installation
 
 For air-gapped installations we recomend the following:
 - Download on another machine the `.whl` file for the corresponding platform and python version from [pypi](https://pypi.org/project/amplpy/#files).
 - Install on the target machine with: `python -m pip install amplpy-version-python_version-*-platform.whl --no-deps`
```

### Comparing `amplpy-0.9.2/amplpy/__init__.py` & `amplpy-0.9.3/amplpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 try:
     from . import modules
 
     modules.preload()
 except Exception:
     pass
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 
 def _list_aliases():
     from inflection import camelize
 
     classes = [
         BaseClass,
```

### Comparing `amplpy-0.9.2/amplpy/ampl.py` & `amplpy-0.9.3/amplpy/ampl.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,54 +45,51 @@
 
 
 class AMPL(object):
     """An AMPL translator.
 
     An object of this class can be used to do the following tasks:
 
-    - Run AMPL code. See :func:`~amplpy.AMPL.eval` and
-      :func:`~amplpy.AMPL.eval_async` / :func:`~amplpy.AMPL.evalAsync`.
+    - Run AMPL code. See :func:`~amplpy.AMPL.eval`.
     - Read models and data from files. See :func:`~amplpy.AMPL.read`,
-      :func:`~amplpy.AMPL.read_data` / :func:`~amplpy.AMPL.readData`,
-      :func:`~amplpy.AMPL.read_async` / :func:`~amplpy.AMPL.readAsync`, and
-      :func:`~amplpy.AMPL.read_data_async` / :func:`~amplpy.AMPL.readDataAsync`.
+      :func:`~amplpy.AMPL.read_data`.
     - Solve optimization problems constructed from model and data (see
-      :func:`~amplpy.AMPL.solve` and :func:`~amplpy.AMPL.solve_async` / :func:`~amplpy.AMPL.solveAsync`).
+      :func:`~amplpy.AMPL.solve`).
     - Access single Elements of an optimization problem. See
-      :func:`~amplpy.AMPL.get_variable` / :func:`~amplpy.AMPL.getVariable`,
-      :func:`~amplpy.AMPL.get_constraint` / :func:`~amplpy.AMPL.getConstraint`,
-      :func:`~amplpy.AMPL.get_objective` / :func:`~amplpy.AMPL.getObjective`,
-      :func:`~amplpy.AMPL.get_set` / :func:`~amplpy.AMPL.getSet`,
-      and :func:`~amplpy.AMPL.get_parameter` / :func:`~amplpy.AMPL.getParameter`.
+      :func:`~amplpy.AMPL.get_variable`,
+      :func:`~amplpy.AMPL.get_constraint`,
+      :func:`~amplpy.AMPL.get_objective`,
+      :func:`~amplpy.AMPL.get_set`,
+      and :func:`~amplpy.AMPL.get_parameter`.
     - Access lists of available entities of an optimization problem. See
-      :func:`~amplpy.AMPL.get_variables` / :func:`~amplpy.AMPL.getVariables`,
-      :func:`~amplpy.AMPL.get_constraints` / :func:`~amplpy.AMPL.getConstraints`,
-      :func:`~amplpy.AMPL.get_objectives` / :func:`~amplpy.AMPL.getObjectives`,
-      :func:`~amplpy.AMPL.get_sets` / :func:`~amplpy.AMPL.getSets`,
-      and :func:`~amplpy.AMPL.get_parameters` / :func:`~amplpy.AMPL.getParameters`.
+      :func:`~amplpy.AMPL.get_variables`,
+      :func:`~amplpy.AMPL.get_constraints`,
+      :func:`~amplpy.AMPL.get_objectives`,
+      :func:`~amplpy.AMPL.get_sets`,
+      and :func:`~amplpy.AMPL.get_parameters`.
 
     Error handling is two-faced:
 
     - Errors coming from the underlying AMPL translator (e.g. syntax errors and
       warnings obtained calling the eval method) are handled by
       the :class:`~amplpy.ErrorHandler` which can be set and get via
-      :func:`~amplpy.AMPL.get_error_handler` / :func:`~amplpy.AMPL.getErrorHandler` and
-      :func:`~amplpy.AMPL.set_error_handler` / :func:`~amplpy.AMPL.setErrorHandler`.
+      :func:`~amplpy.AMPL.get_error_handler` and
+      :func:`~amplpy.AMPL.set_error_handler`.
     - Generic errors coming from misusing the API, which are detected in
       Python, are thrown as exceptions.
 
     The default implementation of the error handler throws exceptions on errors
     and prints to console on warnings.
 
     The output of every user interaction with the underlying translator is
     handled implementing the abstract class :class:`~amplpy.OutputHandler`.
     The (only) method is called at each block of output from the translator.
     The current output handler can be accessed and set via
-    :func:`~amplpy.AMPL.get_output_handler` / :func:`~amplpy.AMPL.getOutputHandler` and
-    :func:`~amplpy.AMPL.set_output_handler` / :func:`~amplpy.AMPL.setOutputHandler`.
+    :func:`~amplpy.AMPL.get_output_handler` and
+    :func:`~amplpy.AMPL.set_output_handler`.
     """
 
     def __init__(self, environment=None, langext=None):
         """
         Constructor:
         creates a new AMPL instance with the specified environment if provided.
```

### Comparing `amplpy-0.9.2/amplpy/amplpython/__init__.py` & `amplpy-0.9.3/amplpy/amplpython/__init__.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/amplpython.py` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/amplpython.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.cxx` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.cxx`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/amplpythonPYTHON_wrap.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ampl.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ampl.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/amplexception.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/amplexception.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/dataframe.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/dataframe.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/entity.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/entity.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/entitymap.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/entitymap.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/environment.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/environment.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/ampl_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/ampl_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/arg.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/arg.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/countediterator.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/countediterator.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/dataframe_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/dataframe_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/declarations.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/declarations.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/entity_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/entity_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/entitymap_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/entitymap_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/environment_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/environment_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/error_information.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/error_information.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/errorinfo_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/errorinfo_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/format.cc` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/format.cc`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/instance_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/instance_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/scopedarray.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/scopedarray.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/slice.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/slice.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/ep/tuple_ep.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/ep/tuple_ep.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/errorhandler.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/errorhandler.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/format.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/format.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/instance.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/instance.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/optional.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/optional.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/output.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/output.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/runnable.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/runnable.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/string.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/string.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/tuple.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/tuple.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/include/ampl/variant.h` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/include/ampl/variant.h`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/aarch64/libampl.so` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/aarch64/libampl.so`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/ampl-2.0.12.dll` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/ampl-2.0.12.dll`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/ampl.lib` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/ampl.lib`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/libampl.dylib` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/libampl.dylib`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/amd64/libampl.so` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/amd64/libampl.so`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/amplpython/cppinterface/lib/ppc64le/libampl.so` & `amplpy-0.9.3/amplpy/amplpython/cppinterface/lib/ppc64le/libampl.so`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/constraint.py` & `amplpy-0.9.3/amplpy/constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     a non-scalar constraint and if a method corresponding to a suffix which is
     not supported by the type of the constraint is called.
     A runtime error is thrown if any property of an entity which has been
     deleted from the underlying interpreter is accessed.
 
     To gain access to all the values in an entity (for all instances and all
     suffixes for that entities), see
-    :func:`~amplpy.Entity.get_values` / :func:`~amplpy.Entity.getValues`
+    :func:`~amplpy.Entity.get_values`
     and the :class:`~amplpy.DataFrame` class.
     """
 
     def __init__(self, _impl):
         Entity.__init__(self, _impl, Constraint)
 
     def is_logical(self):
```

### Comparing `amplpy-0.9.2/amplpy/dataframe.py` & `amplpy-0.9.3/amplpy/dataframe.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,33 +65,33 @@
         DataFrame objects should not be instantiated manually. For best performance
         using Python native types or Pandas Dataframes. The API takes care of the conversion
         for you in the most efficient way it finds.
 
     An object of this class can be used to do the following tasks:
 
     - Assign values to AMPL entities (once the DataFrame is populated, use
-      :func:`~amplpy.AMPL.set_data` / :func:`~amplpy.AMPL.setData` to assign its
+      :func:`~amplpy.AMPL.set_data` to assign its
       values to the modelling entities in its columns)
     - Get values from AMPL, decoupling the values from the AMPL entities they
       originate via
-      :func:`~amplpy.Entity.get_values` / :func:`~amplpy.Entity.getValues`.
+      :func:`~amplpy.Entity.get_values`.
 
     A DataFrame object can be created in various ways:
 
     - Get values from AMPL, decoupling the values from the AMPL entities they originate from
-      (via :func:`~amplpy.Entity.get_values` / :func:`~amplpy.Entity.getValues`)
-    - From Pandas dataframes with :func:`~amplpy.DataFrame.from_pandas` / :func:`~amplpy.DataFrame.fromPandas`
-    - From Numpy matrices with :func:`~amplpy.DataFrame.from_numpy` / :func:`~amplpy.DataFrame.fromNumpy`
-    - From Python dictionaries with :func:`~amplpy.DataFrame.from_dict` / :func:`~amplpy.DataFrame.fromDict`
+      (via :func:`~amplpy.Entity.get_values`)
+    - From Pandas dataframes with :func:`~amplpy.DataFrame.from_pandas`
+    - From Numpy matrices with :func:`~amplpy.DataFrame.from_numpy`
+    - From Python dictionaries with :func:`~amplpy.DataFrame.from_dict`
 
     and can be converted to various object types:
 
-    - Pandas dataframes with :func:`~amplpy.DataFrame.to_pandas` / :func:`~amplpy.DataFrame.toPandas`
-    - Python dictionary with :func:`~amplpy.DataFrame.to_dict` / :func:`~amplpy.DataFrame.toDict`
-    - Python list with :func:`~amplpy.DataFrame.to_list` / :func:`~amplpy.DataFrame.toList`
+    - Pandas dataframes with :func:`~amplpy.DataFrame.to_pandas`
+    - Python dictionary with :func:`~amplpy.DataFrame.to_dict`
+    - Python list with :func:`~amplpy.DataFrame.to_list`
     """
 
     def __init__(self, index, columns=tuple(), **kwargs):
         """
         Create a new DataFrame with specifed index and column headers.
 
         Args:
```

### Comparing `amplpy-0.9.2/amplpy/entity.py` & `amplpy-0.9.3/amplpy/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     entity or, if the corresponding declaration has an indexing expression, a
     mapping from keys to instances. In the derived classes, it has methods to
     access instance-level properties which can be used in case the represented
     entity is scalar.
 
     To gain access to all the values in an entity (for all instances and all
     suffixes for that entities), use the function
-    :func:`~amplpy.Entity.get_values` / :func:`~amplpy.Entity.getValues`.
+    :func:`~amplpy.Entity.get_values`.
 
-    The algebraic entities which currenty have an equivalent class in the API
+    The algebraic entities which currently have an equivalent class in the API
     are:
 
     - Variables (see :class:`~amplpy.Variable`)
     - Constraints (see :class:`~amplpy.Constraint`)
     - Objectives (see :class:`~amplpy.Objective`)
     - Sets (see :class:`~amplpy.Set`)
     - Parameters (see :class:`~amplpy.Parameter`)
```

### Comparing `amplpy-0.9.2/amplpy/environment.py` & `amplpy-0.9.3/amplpy/environment.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/errorhandler.py` & `amplpy-0.9.3/amplpy/errorhandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # -*- coding: utf-8 -*-
-from __future__ import print_function, absolute_import, division
+from __future__ import print_function
 
-# from builtins import map, range, object, zip, sorted
-# from past.builtins import basestring
+
+def display_error_message(exception, error=True):
+    msg = "\t" + str(exception).replace("\n", "\n\t")
+    if error:
+        print("Error:\n{:s}".format(msg))
+    else:
+        print("Warning:\n{:s}".format(msg))
 
 
 class ErrorHandler:
     """
     A basic interface for AMPL error handlers. If an application needs to
-    implement customised error handling, it must implement this interface and
+    implement customized error handling, it must implement this interface and
     then register an instance with the AMPL API using the
-    :func:`~amplpy.AMPL.set_error_handler` / :func:`~amplpy.AMPL.setErrorHandler` method.
-    The underlying AMPL
-    interpreter will then report all errors and warnings through this
-    interface as :class:`~amplpy.AMPLException` objects.
+    :func:`~amplpy.AMPL.set_error_handler` method.
+    The underlying AMPL interpreter will then report all errors and warnings
+    through this interface as :class:`~amplpy.AMPLException` objects.
     """
 
     def error(self, exception):
         """
         Receives notification of an error.
         """
-        msg = "\t" + str(exception).replace("\n", "\n\t")
-        print("Error:\n{:s}".format(msg))
+        display_error_message(exception)
         raise exception
 
     def warning(self, exception):
         """
         Receives notification of a warning.
         """
-        msg = "\t" + str(exception).replace("\n", "\n\t")
-        print("Warning:\n{:s}".format(msg))
+        display_error_message(exception, error=False)
```

### Comparing `amplpy-0.9.2/amplpy/exceptions.py` & `amplpy-0.9.3/amplpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/iterators.py` & `amplpy-0.9.3/amplpy/iterators.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/objective.py` & `amplpy-0.9.3/amplpy/objective.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     All these methods throw a TypeError if called for a non scalar
     objective and an RuntimeError if called on an entity which has been deleted
     in the underlying intepreter.
 
     To gain access to all the values in an entity (for all instances and all
     suffixes for that entities), see
-    :func:`~amplpy.Entity.get_values` / :func:`~amplpy.Entity.getValues`
+    :func:`~amplpy.Entity.get_values`
     and the :class:`~amplpy.DataFrame` class.
     """
 
     def __init__(self, _impl):
         Entity.__init__(self, _impl, Objective)
 
     def value(self):
```

### Comparing `amplpy-0.9.2/amplpy/outputhandler.py` & `amplpy-0.9.3/amplpy/outputhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class OutputHandler(amplpython.OutputHandler):
     """
     Interface to handle the outputs from the calls to any
     function that causes the underlying AMPL interpreter to display a message.
     If an application needs to
     implement customised output handling, it must implement this interface and
     then register an instance with the AMPL API using the
-    :func:`~amplpy.AMPL.set_output_handler` / :func:`~amplpy.AMPL.setOutputHandler`
+    :func:`~amplpy.AMPL.set_output_handler`
     method.
 
     Note that errors and warnings are not passed through this interface,
     see :class:`~amplpy.ErrorHandler` for more information.
     """
 
     def output(self, kind, msg):
```

### Comparing `amplpy-0.9.2/amplpy/parameter.py` & `amplpy-0.9.3/amplpy/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 class Parameter(Entity):
     """
     Represents an AMPL parameter. The values can be float or string (in case of
     symbolic parameters).
 
     Data can be assigned to the set using the methods
     :func:`~amplpy.Parameter.set` and
-    :func:`~amplpy.Parameter.set_values` / :func:`~amplpy.Parameter.setValues`
+    :func:`~amplpy.Parameter.set_values`
     or using
-    :func:`~amplpy.AMPL.set_data` / :func:`~amplpy.AMPL.setData`
+    :func:`~amplpy.AMPL.set_data`
     and an object of class :class:`~amplpy.DataFrame`.
     """
 
     def __init__(self, _impl):
         Entity.__init__(self, _impl, lambda it: it)
 
     def __setitem__(self, index, value):
```

### Comparing `amplpy-0.9.2/amplpy/set.py` & `amplpy-0.9.3/amplpy/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     In case of indexed sets, you can gain access to the instances using the
     operator [].
 
     All the accessors in this class throw an RuntimeError if the instance has
     been deleted in the underlying AMPL interpreter.
 
     Data can be assigned to the set using the methods
-    :func:`~amplpy.Set.set_values` / :func:`~amplpy.Set.setValues`
+    :func:`~amplpy.Set.set_values`
     (for non-indexed sets only) or using
-    :func:`~amplpy.AMPL.set_data` / :func:`~amplpy.AMPL.setData`
+    :func:`~amplpy.AMPL.set_data`
     and an object of class
     :class:`~amplpy.DataFrame`.
     """
 
     def __init__(self, _impl):
         Entity.__init__(self, _impl, Set)
```

### Comparing `amplpy-0.9.2/amplpy/tests/TestBase.py` & `amplpy-0.9.3/amplpy/tests/TestBase.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests/test_ampl.py` & `amplpy-0.9.3/amplpy/tests/test_ampl.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests/test_dataframe.py` & `amplpy-0.9.3/amplpy/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests/test_entities.py` & `amplpy-0.9.3/amplpy/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests/test_environment.py` & `amplpy-0.9.3/amplpy/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests/test_iterators.py` & `amplpy-0.9.3/amplpy/tests/test_iterators.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests/test_properties.py` & `amplpy-0.9.3/amplpy/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/TestBase.py` & `amplpy-0.9.3/amplpy/tests_camel/TestBase.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/test_ampl.py` & `amplpy-0.9.3/amplpy/tests_camel/test_ampl.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/test_dataframe.py` & `amplpy-0.9.3/amplpy/tests_camel/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/test_entities.py` & `amplpy-0.9.3/amplpy/tests_camel/test_entities.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/test_environment.py` & `amplpy-0.9.3/amplpy/tests_camel/test_environment.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/test_iterators.py` & `amplpy-0.9.3/amplpy/tests_camel/test_iterators.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tests_camel/test_properties.py` & `amplpy-0.9.3/amplpy/tests_camel/test_properties.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/tools/__init__.py` & `amplpy-0.9.3/amplpy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/utils.py` & `amplpy-0.9.3/amplpy/utils.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/variable.py` & `amplpy-0.9.3/amplpy/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     All these methods throw a TypeError if called for a non scalar
     objective and an RuntimeError if called on an entity which has been deleted
     in the underlying intepreter.
 
     To gain access to all the values in an entity (for all instances and all
     suffixes for that entities), see
-    :func:`~amplpy.Entity.get_values` / :func:`~amplpy.Entity.getValues`
+    :func:`~amplpy.Entity.get_values`
     and the :class:`~amplpy.DataFrame` class.
     """
 
     def __init__(self, _impl):
         Entity.__init__(self, _impl, Variable)
 
     def value(self):
```

### Comparing `amplpy-0.9.2/amplpy/vendor/CHANGELOG.md` & `amplpy-0.9.3/amplpy/vendor/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/LICENSE` & `amplpy-0.9.3/amplpy/vendor/LICENSE`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/modules/amplpypi.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/modules/amplpypi.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/modules/commands.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/modules/commands.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/notebooks.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/notebooks.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_install.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_load.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_preload.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/tests/test_run.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/ampltools/utils.py` & `amplpy-0.9.3/amplpy/vendor/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy/vendor/setup.py` & `amplpy-0.9.3/amplpy/vendor/setup.py`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/amplpy.egg-info/PKG-INFO` & `amplpy-0.9.3/amplpy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplpy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python API for AMPL
 Home-page: http://ampl.com/
 Download-URL: https://github.com/ampl/amplpy
 Author: AMPL Optimization Inc.
 Author-email: devteam@ampl.com
 License: BSD-3
 Platform: any
@@ -50,14 +50,44 @@
 
 # Import in Python
 $ python
 >>> from amplpy import AMPL
 >>> ampl = AMPL() # instantiate AMPL object
 ```
 
+```python
+# Minimal example:
+from amplpy import AMPL
+import pandas as pd
+ampl = AMPL()
+ampl.eval(r"""
+    set A ordered;
+    param S{A, A};
+    param lb default 0;
+    param ub default 1;
+    var w{A} >= lb <= ub;
+    minimize portfolio_variance:
+        sum {i in A, j in A} w[i] * S[i, j] * w[j];
+    s.t. portfolio_weights:
+        sum {i in A} w[i] = 1;
+""")
+tickers, cov_matrix = # ... pre-process data in Python
+ampl.set["A"] = tickers
+ampl.param["S"] = pd.DataFrame(
+    cov_matrix, index=tickers, columns=tickers
+).unstack()
+ampl.option["solver"] = "gurobi"
+ampl.option["gurobi_options"] = "outlev=1"
+ampl.solve()
+assert ampl.get_value("solve_result") == "solved"
+sigma = ampl.get_value("sqrt(sum {i in A, j in A} w[i] * S[i, j] * w[j])")
+print(f"Volatility: {sigma*100:.1f}%")
+# ... post-process solution in Python
+```
+
 [[Documentation](https://amplpy.readthedocs.io/)] [[AMPL Modules for Python](https://dev.ampl.com/ampl/python/modules.html)] [[Available on Google Colab](https://colab.ampl.com/)] [[AMPL Community Edition](http://ampl.com/ce)]
 
 `amplpy` is an interface that allows developers to access the features of [AMPL](https://ampl.com) from within Python. For a quick introduction to AMPL see [Quick Introduction to AMPL](https://dev.ampl.com/ampl/introduction.html).
 
 In the same way that AMPL’s syntax matches naturally the mathematical description of the model, the input and output data matches naturally Python lists, sets, dictionaries, `pandas` and `numpy` objects.
 
 All model generation and solver interaction is handled directly by AMPL, which leads to great stability and speed; the library just acts as an intermediary, and the added overhead (in terms of memory and CPU usage) depends mostly on how much data is sent and read back from AMPL, the size of the expanded model as such is irrelevant.
```

### Comparing `amplpy-0.9.2/amplpy.egg-info/SOURCES.txt` & `amplpy-0.9.3/amplpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amplpy-0.9.2/setup.py` & `amplpy-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""
+'''
 # AMPLPY: Python API for AMPL
 
 ```python
 # Install Python API for AMPL
 $ python -m pip install amplpy --upgrade
 
 # Install solver modules (e.g., HiGHS, CBC, Gurobi)
@@ -14,14 +14,44 @@
 
 # Import in Python
 $ python
 >>> from amplpy import AMPL
 >>> ampl = AMPL() # instantiate AMPL object
 ```
 
+```python
+# Minimal example:
+from amplpy import AMPL
+import pandas as pd
+ampl = AMPL()
+ampl.eval(r"""
+    set A ordered;
+    param S{A, A};
+    param lb default 0;
+    param ub default 1;
+    var w{A} >= lb <= ub;
+    minimize portfolio_variance:
+        sum {i in A, j in A} w[i] * S[i, j] * w[j];
+    s.t. portfolio_weights:
+        sum {i in A} w[i] = 1;
+""")
+tickers, cov_matrix = # ... pre-process data in Python
+ampl.set["A"] = tickers
+ampl.param["S"] = pd.DataFrame(
+    cov_matrix, index=tickers, columns=tickers
+).unstack()
+ampl.option["solver"] = "gurobi"
+ampl.option["gurobi_options"] = "outlev=1"
+ampl.solve()
+assert ampl.get_value("solve_result") == "solved"
+sigma = ampl.get_value("sqrt(sum {i in A, j in A} w[i] * S[i, j] * w[j])")
+print(f"Volatility: {sigma*100:.1f}%")
+# ... post-process solution in Python
+```
+
 [[Documentation](https://amplpy.readthedocs.io/)] [[AMPL Modules for Python](https://dev.ampl.com/ampl/python/modules.html)] [[Available on Google Colab](https://colab.ampl.com/)] [[AMPL Community Edition](http://ampl.com/ce)]
 
 `amplpy` is an interface that allows developers to access the features of [AMPL](https://ampl.com) from within Python. For a quick introduction to AMPL see [Quick Introduction to AMPL](https://dev.ampl.com/ampl/introduction.html).
 
 In the same way that AMPL’s syntax matches naturally the mathematical description of the model, the input and output data matches naturally Python lists, sets, dictionaries, `pandas` and `numpy` objects.
 
 All model generation and solver interaction is handled directly by AMPL, which leads to great stability and speed; the library just acts as an intermediary, and the added overhead (in terms of memory and CPU usage) depends mostly on how much data is sent and read back from AMPL, the size of the expanded model as such is irrelevant.
@@ -32,15 +62,15 @@
 
 - http://amplpy.readthedocs.io
 
 ## Repositories:
 
 * GitHub Repository: https://github.com/ampl/amplpy
 * PyPI Repository: https://pypi.python.org/pypi/amplpy
-"""
+'''
 from setuptools import setup, Extension
 import platform
 import sys
 import os
 
 OSTYPE = platform.system()
 ARCH = platform.processor() or platform.machine()
@@ -122,18 +152,18 @@
         #  cannot open input file '.obj' in build on distutils from Python 3.9
         # https://github.com/pypa/setuptools/issues/2417
         return []
 
 
 setup(
     name="amplpy",
-    version="0.9.2",
+    version="0.9.3",
     description="Python API for AMPL",
     long_description=__doc__,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     license="BSD-3",
     platforms="any",
     author="AMPL Optimization Inc.",
     author_email="devteam@ampl.com",
     url="http://ampl.com/",
     download_url="https://github.com/ampl/amplpy",
     classifiers=[
```

