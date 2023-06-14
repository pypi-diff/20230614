# Comparing `tmp/pyflowline-0.2.2.tar.gz` & `tmp/pyflowline-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflowline-0.2.2.tar", last modified: Mon Mar 20 22:54:40 2023, max compression
+gzip compressed data, was "pyflowline-0.2.4.tar", last modified: Wed Jun 14 19:40:31 2023, max compression
```

## Comparing `pyflowline-0.2.2.tar` & `pyflowline-0.2.4.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-20 22:54:30.000000 pyflowline-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-03-20 22:54:30.000000 pyflowline-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-20 22:54:30.000000 pyflowline-0.2.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-03-20 22:54:30.000000 pyflowline-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-20 22:54:30.000000 pyflowline-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-20 22:54:40.773635 pyflowline-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.749634 pyflowline-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (123)    67244 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/after_loop.png
--rw-r--r--   0 runner    (1001) docker     (123)    64320 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/after_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)    66495 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/basic_element.png
--rw-r--r--   0 runner    (1001) docker     (123)    76858 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/before_loop.png
--rw-r--r--   0 runner    (1001) docker     (123)    68959 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/before_merge.png
--rw-r--r--   0 runner    (1001) docker     (123)    69874 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/data_mode.png
--rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/disconnect_flowline.png
--rw-r--r--   0 runner    (1001) docker     (123)   146717 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/find_vertex.png
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/flow_direction.png
--rw-r--r--   0 runner    (1001) docker     (123)   252712 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/flow_direction_matrix.png
--rw-r--r--   0 runner    (1001) docker     (123)   525380 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/hexagon.png
--rw-r--r--   0 runner    (1001) docker     (123)   628942 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/hexagon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (123)   524174 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/lat_lon.png
--rw-r--r--   0 runner    (1001) docker     (123)   734342 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/lat_lon_intersect.png
--rw-r--r--   0 runner    (1001) docker     (123)    45168 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/merge_flowline.png
--rw-r--r--   0 runner    (1001) docker     (123)  1191889 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/meshes.png
--rw-r--r--   0 runner    (1001) docker     (123)    47724 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/remove_loop.png
--rw-r--r--   0 runner    (1001) docker     (123)   596253 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/remove_loop_matrix.png
--rw-r--r--   0 runner    (1001) docker     (123)    93563 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/simplification01.png
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/small_river.png
--rw-r--r--   0 runner    (1001) docker     (123)   148387 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/sqaure_intersect.png
--rw-r--r--   0 runner    (1001) docker     (123)    61180 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/square.png
--rw-r--r--   0 runner    (1001) docker     (123)    46783 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/structure_pyflowline.png
--rw-r--r--   0 runner    (1001) docker     (123)   160993 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/figures/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/source/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/algorithm/algorithm.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/api/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/source/application/
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/application/application.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/source/data/
--rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/data/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/docs/source/installation/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/installation/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/references.rst
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/support.rst
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-20 22:54:30.000000 pyflowline-0.2.2/docs/source/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.761634 pyflowline-0.2.2/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-20 22:54:30.000000 pyflowline-0.2.2/examples/create_model_condfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/check_head_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/find_index_in_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/gdal_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/longlat_to_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/auxiliary/text_reader_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/connection/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/connection/connect_disconnect_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/cython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/direction/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/direction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/direction/correct_flowline_direction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/index/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/index/define_stream_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/index/define_stream_segment_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/intersect/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/intersect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline/algorithms/loop/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/loop/remove_flowline_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.769635 pyflowline-0.2.2/pyflowline/algorithms/merge/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/merge/merge_flowline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.769635 pyflowline-0.2.2/pyflowline/algorithms/simplification/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/simplification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/simplification/remove_duplicate_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/simplification/remove_returning_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/simplification/remove_small_river.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.769635 pyflowline-0.2.2/pyflowline/algorithms/split/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/split/find_flowline_confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/split/find_flowline_vertex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/split/split_by_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/split/split_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/algorithms/split/split_flowline_to_edge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/classes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/_hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    41412 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)    47766 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/basin.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/confluence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/hexagon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/latlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/link.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/mpas.py
--rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/pycase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/square.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/tin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/classes/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/convert_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/convert_flowline_to_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/export_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/export_vertex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/read_flowline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/read_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/formats/read_nhdplus_flowline_shapefile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/dggrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/dggrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/dggrid/create_dggrid_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/hexagon/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/hexagon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/hexagon/create_hexagon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/latlon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/latlon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/latlon/create_latlon_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/mpas/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/mpas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/mpas/create_mpas_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/square/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/square/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/square/create_square_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.773635 pyflowline-0.2.2/pyflowline/mesh/tin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/tin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/mesh/tin/create_tin_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/pyflowline_create_template_configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyflowline/pyflowline_read_model_configuration_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:54:40.765634 pyflowline-0.2.2/pyflowline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-03-20 22:54:40.000000 pyflowline-0.2.2/pyflowline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-03-20 22:54:40.000000 pyflowline-0.2.2/pyflowline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 22:54:40.000000 pyflowline-0.2.2/pyflowline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-20 22:54:40.000000 pyflowline-0.2.2/pyflowline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-20 22:54:40.000000 pyflowline-0.2.2/pyflowline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-20 22:54:30.000000 pyflowline-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-20 22:54:40.777635 pyflowline-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-20 22:54:30.000000 pyflowline-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-14 19:40:18.000000 pyflowline-0.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-14 19:40:18.000000 pyflowline-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-14 19:40:18.000000 pyflowline-0.2.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-14 19:40:18.000000 pyflowline-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-14 19:40:18.000000 pyflowline-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-14 19:40:31.866621 pyflowline-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-14 19:40:18.000000 pyflowline-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.838619 pyflowline-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.846619 pyflowline-0.2.4/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    67244 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/after_loop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64320 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/after_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66495 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/basic_element.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76858 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/before_loop.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68959 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/before_merge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69874 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/data_mode.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16482 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/disconnect_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146717 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/find_vertex.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/flow_direction.png
+-rw-r--r--   0 runner    (1001) docker     (123)   252712 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/flow_direction_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)   525380 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/hexagon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   628942 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/hexagon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (123)   524174 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/lat_lon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   734342 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/lat_lon_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45168 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/merge_flowline.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1191889 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/meshes.png
+-rw-r--r--   0 runner    (1001) docker     (123)    47724 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/remove_loop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   596253 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/remove_loop_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93563 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/simplification01.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/small_river.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148387 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/sqaure_intersect.png
+-rw-r--r--   0 runner    (1001) docker     (123)    61180 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46783 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/structure_pyflowline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160993 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/figures/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/algorithm/algorithm.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/api/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/application/application.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/data/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/docs/source/installation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/installation/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/references.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-14 19:40:18.000000 pyflowline-0.2.4/docs/source/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-14 19:40:18.000000 pyflowline-0.2.4/examples/create_model_condfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/pyflowline/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/check_head_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_index_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_vertex_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/auxiliary/longlat_to_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/connection/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/connection/connect_disconnect_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/direction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/direction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/direction/correct_flowline_direction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/index/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/index/define_stream_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/index/define_stream_segment_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.854620 pyflowline-0.2.4/pyflowline/algorithms/intersect/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8167 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/loop/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/loop/remove_flowline_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/merge/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/merge/merge_flowline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/simplification/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_duplicate_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_duplicate_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_returning_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_small_river.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.858620 pyflowline-0.2.4/pyflowline/algorithms/split/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/split_by_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline_to_edge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.862620 pyflowline-0.2.4/pyflowline/classes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/_hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47953 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/basin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/confluence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/hexagon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/latlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/mpas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40205 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/pycase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/square.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/tin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/classes/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/convert_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/convert_flowline_to_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/export_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/export_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/read_flowline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/read_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/formats/read_nhdplus_flowline_shapefile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/dggrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/dggrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/dggrid/create_dggrid_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/hexagon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/hexagon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17396 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/hexagon/create_hexagon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/latlon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/latlon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/latlon/create_latlon_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/mpas/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/mpas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/mpas/create_mpas_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/square/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/square/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/square/create_square_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/pyflowline/mesh/tin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/tin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/mesh/tin/create_tin_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/pyflowline_create_template_configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyflowline/pyflowline_read_model_configuration_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.850620 pyflowline-0.2.4/pyflowline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 19:40:31.000000 pyflowline-0.2.4/pyflowline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 19:40:18.000000 pyflowline-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-14 19:40:31.866621 pyflowline-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-14 19:40:18.000000 pyflowline-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:40:31.866621 pyflowline-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 19:40:18.000000 pyflowline-0.2.4/tests/test_installation.py
```

### Comparing `pyflowline-0.2.2/CONTRIBUTING.rst` & `pyflowline-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/LICENSE.md` & `pyflowline-0.2.4/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,28 @@
-PyFlowline
+BSD 3-Clause License
 
-A mesh-independent river network generator for hydrologic models.
-        
-Copyright © 2022, Battelle Memorial Institute
+Copyright (c) 2022, Battelle Memorial Institute
 
-1. Battelle Memorial Institute (hereinafter Battelle) hereby grants permission to any person or entity lawfully obtaining a copy of this software and associated documentation files (hereinafter “the Software”) to redistribute and use the Software in source and binary forms, with or without modification. Such person or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and may permit others to do so, subject to the following conditions:
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimers.
-
-* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
-
-* Other than as used herein, neither the name Battelle Memorial Institute or Battelle may be used in any form whatsoever without the express written consent of Battelle.
-
-2. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL BATTELLE OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyflowline-0.2.2/PKG-INFO` & `pyflowline-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.2.2
-Summary: A mesh independent river network generator for hydrologic models
+Version: 0.2.4
+Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -15,32 +15,49 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: visualization
-License-File: LICENSE.md
+License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 ### PyFlowline
 
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
+[![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models. 
 
 PyFlowline is mesh independent, meaning you can apply it to both structured (e.g., traditional rectangle mesh, latitude-longitude, hexagon) and unstructured mesh systems (e.g., Triangulated Irregular Network (TIN) mesh and Model for Prediction Across Scales (MPAS) mesh).
 
 This package generates the mesh cell-based conceptual river networks using the following steps:
 
 1. `Flowline simplification`: PyFlowline checks the vector dataset and corrects undesired flowlines, such as braided rivers.
 2. `Mesh generation`: PyFlowline generates structured meshes (e.g., rectangle, hexagon) or imports user-provided unstructured meshes into the PyFlowline-compatible GEOJSON format.
 3. `Topological relationship reconstruction`: PyFlowline reconstructs the topological relationship using the mesh and flowline intersections.
 
+
+### Dependency
+
+PyFlowline depends on the following packages
+
+1. `numpy`
+2. `gdal`
+3. `netCDF4`
+4. `shapely`
+
+PyFlowline also has three optional dependency packages
+
+1. `cython` for performance 
+2. `matplotlin` for visualization
+3. `cartopy` for visulization
+
 ### Quickstart
 
 Please refer to the [quickstart documentation](https://pyflowline.readthedocs.io/en/latest/quickstart.html) for details on how to get started using the PyFlowline package.
 
 ### Installation
 
 Please refer to the [official documentation](https://pyflowline.readthedocs.io/) for details on how to install the PyFlowline package.
@@ -51,14 +68,16 @@
 
 ### Acknowledgment
 
 This work was supported by the Earth System Model Development program areas of the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research as part of the multi-program, collaborative Integrated Coastal Modeling (ICoM) project and the Interdisciplinary Research for Arctic Coastal Environments (InteRFACE) project.
 
 ### License
 
+BSD 3-Clause License
+
 Copyright © 2022, Battelle Memorial Institute
 
 1. Battelle Memorial Institute (hereinafter Battelle) hereby grants permission to any person or entity lawfully obtaining a copy of this software and associated documentation files (hereinafter “the Software”) to redistribute and use the Software in source and binary forms, with or without modification. Such person or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software and may permit others to do so, subject to the following conditions:
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimers.
 
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
@@ -67,11 +86,11 @@
 
 2. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL BATTELLE OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ### References
 
 Several publications describe the algorithms used in `PyFlowline` in detail. If you make use of `PyFlowline` in your work, please consider including a reference to the following:
 
-* Liao. C. Cooper, M (2022) Pyflowline: a mesh independent river network generator for hydrologic models. Zenodo.
+* Liao. C. Cooper, M (2022) Pyflowline: a mesh-independent river network generator for hydrologic models. Zenodo.
 https://doi.org/10.5281/zenodo.6407299
 
 * Liao, C., Zhou, T., Xu, D., Cooper, M. G., Engwirda, D., Li, H.-Y., & Leung, L. R. (2023). Topological relationship-based flow direction modeling: Mesh-independent river networks representation. Journal of Advances in Modeling Earth Systems, 15, e2022MS003089. https://doi.org/10.1029/2022MS003089
```

### Comparing `pyflowline-0.2.2/docs/Makefile` & `pyflowline-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/after_loop.png` & `pyflowline-0.2.4/docs/figures/after_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/after_merge.png` & `pyflowline-0.2.4/docs/figures/after_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/basic_element.png` & `pyflowline-0.2.4/docs/figures/basic_element.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/before_loop.png` & `pyflowline-0.2.4/docs/figures/before_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/before_merge.png` & `pyflowline-0.2.4/docs/figures/before_merge.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/data_mode.png` & `pyflowline-0.2.4/docs/figures/data_mode.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/disconnect_flowline.png` & `pyflowline-0.2.4/docs/figures/disconnect_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/find_vertex.png` & `pyflowline-0.2.4/docs/figures/find_vertex.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/flow_direction.png` & `pyflowline-0.2.4/docs/figures/flow_direction.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/flow_direction_matrix.png` & `pyflowline-0.2.4/docs/figures/flow_direction_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/hexagon.png` & `pyflowline-0.2.4/docs/figures/hexagon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/hexagon_intersect.png` & `pyflowline-0.2.4/docs/figures/hexagon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/lat_lon.png` & `pyflowline-0.2.4/docs/figures/lat_lon.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/lat_lon_intersect.png` & `pyflowline-0.2.4/docs/figures/lat_lon_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/merge_flowline.png` & `pyflowline-0.2.4/docs/figures/merge_flowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/meshes.png` & `pyflowline-0.2.4/docs/figures/meshes.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/remove_loop.png` & `pyflowline-0.2.4/docs/figures/remove_loop.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/remove_loop_matrix.png` & `pyflowline-0.2.4/docs/figures/remove_loop_matrix.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/simplification01.png` & `pyflowline-0.2.4/docs/figures/simplification01.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/small_river.png` & `pyflowline-0.2.4/docs/figures/small_river.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/sqaure_intersect.png` & `pyflowline-0.2.4/docs/figures/sqaure_intersect.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/square.png` & `pyflowline-0.2.4/docs/figures/square.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/structure_pyflowline.png` & `pyflowline-0.2.4/docs/figures/structure_pyflowline.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/figures/workflow.png` & `pyflowline-0.2.4/docs/figures/workflow.png`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/make.bat` & `pyflowline-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/algorithm/algorithm.rst` & `pyflowline-0.2.4/docs/source/algorithm/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/api/api.rst` & `pyflowline-0.2.4/docs/source/api/api.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/application/application.rst` & `pyflowline-0.2.4/docs/source/application/application.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/conf.py` & `pyflowline-0.2.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/data/data.rst` & `pyflowline-0.2.4/docs/source/data/data.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/faq.rst` & `pyflowline-0.2.4/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/glossary.rst` & `pyflowline-0.2.4/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/index.rst` & `pyflowline-0.2.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/docs/source/installation/installation.rst` & `pyflowline-0.2.4/docs/source/installation/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -50,7 +50,24 @@
 
 * `numpy`
 * `gdal`
 * `netCDF4`
 * `shapely`
 
 
+=============
+Visualization
+=============
+
+PyFlowline only provides experimental support for visualization through the optional `matplotlib` and `cartopy` packages.
+
+You need to manually speicify these packages during the installation process
+
+    conda install -c conda-forge pyflowline matplotlib cartopy
+
+"""
+
+or install manually after the installation of PyFlowline:
+
+    conda install -c conda-forge matplotlib cartopy
+
+
```

### Comparing `pyflowline-0.2.2/docs/source/quickstart.rst` & `pyflowline-0.2.4/docs/source/quickstart.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #####################
 Quickstart
 #####################
 
 Users can run a PyFlowline simulation in the following steps:
 
 1. Create a new Python environment using Conda, and activate the new environment.
-2. Clone the latest PyFlowline repository from https://github.com/changliao1025/pyflowline. 
-3. Install the dependency packages using conda.
+2. Install the package using `conda install -c conda-forge pyflowline`. Conda will automatically install all the required dependencies.
+3. Clone the latest PyFlowline repository from https://github.com/changliao1025/pyflowline. 
 4. Download the additional large MPAS mesh file `lnd_cull_mesh.nc` from https://github.com/changliao1025/pyflowline/releases/tag/0.2.0 and move it under the `data/susquehanna/input` folder.
 5. Open the `examples/susquehanna/pyflowline_susquehanna_mpas.json` file and change `sWorkspace_output` to the full path to the directory where you want to save the output (e.g. `/full/path/to/pyflowline/data/susquehanna/output`), change `"sFilename_mesh_netcdf"` to the full path to `lnd_cull_mesh.nc`, `"sFilename_mesh_boundary"` to the full path to `data/susquehanna/input/mesh_boundary_buffer.geojson`, and `"sFilename_basins"` to the full path to `examples/susquehanna/pyflowline_susquehanna_basins.json`.
 6. Open the `examples/susquehanna/pyflowline_susquehanna_basins.json` file and change `"sFilename_flowline_filter"` to the full path to `data/susquehanna/input/flowline.geojson`. Ignore the other settings in these json files for now.
-7. Open the preferred Python IDE (Visual Studio Code recommended) and run the  `examples/susquehanna/run_simulation_mpas.py` Python script. Optionally, you can also run the `notebooks/mpas_notebook.ipynb` notebook.
+7. Open the preferred Python IDE (Visual Studio Code recommended) and run the  `examples/susquehanna/run_simulation_mpas.py` Python script. Optionally, you can also run the `notebooks/mpas_example.ipynb` notebook.
 8. You should produce a list of model outputs in the `data/susquehanna/output` folder or the user-specified output folder.
 
 If you encounter any issues, refer to the FAQ or submit a GitHub issue (https://github.com/changliao1025/pyflowline/issues).
```

### Comparing `pyflowline-0.2.2/docs/source/readme.rst` & `pyflowline-0.2.4/docs/source/readme.rst`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/examples/create_model_condfiguration.py` & `pyflowline-0.2.4/examples/create_model_condfiguration.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py` & `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/calculate_area_of_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import numpy as np
 from osgeo import ogr, osr
 import importlib
 
 from shapely.ops import polygonize
-from pyflowline.algorithms.auxiliary.gdal_functions import  calculate_angle_betwen_vertex_normal
-from pyflowline.algorithms.auxiliary.gdal_functions import calculate_polygon_area
+
 from pyflowline.algorithms.auxiliary.find_index_in_list import find_list_in_list 
 
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_angle_betwen_vertex_normal
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
+
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import find_vertex_in_list
 else:
     from pyflowline.algorithms.auxiliary.find_vertex_in_list import find_vertex_in_list
```

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/auxiliary/check_head_water.py` & `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/check_head_water.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/auxiliary/find_index_in_list.py` & `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_index_in_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,16 +167,14 @@
     if iFlag_exist == 1:
         pass
     else:
         aVertex_in.append(pVertex_in)
         pass
 
     return aVertex_in, iFlag_exist
-
-
 def find_list_in_list(aList_in, pList_in):
     c = copy.deepcopy(pList_in)
     c.sort()
     nList = len(aList_in)
     iFlag = 0
     for i in range(nList):
         a = aList_in[i]
```

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/auxiliary/find_vertex_in_list.py` & `pyflowline-0.2.4/pyflowline/algorithms/auxiliary/find_vertex_in_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 def find_vertex_in_list(aVertex_in, pVertex_in, dThreshold_in=1.0E-6):
     """[find the index of a vertex in a list]
 
     Args:
         aVertex_in ([type]): [description]
         pVertex_in ([type]): [description]
```

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/connection/connect_disconnect_flowline.py` & `pyflowline-0.2.4/pyflowline/algorithms/connection/connect_disconnect_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/direction/correct_flowline_direction.py` & `pyflowline-0.2.4/pyflowline/algorithms/direction/correct_flowline_direction.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     for i in range(nFlowline):
         pFlowline = aFlowline_in[i]
         iFlag_dam = pFlowline.iFlag_dam
         iStream_order = pFlowline.iStream_order
         pVertex_start = pFlowline.pVertex_start
         pVertex_end = pFlowline.pVertex_end
         dDiatance = pVertex_end.calculate_distance( pVertex_outlet_in )   
-        if iFlag_first ==1:
+        if iFlag_first == 1:
             dDiatance_min = dDiatance                
             lIndex_outlet = i            
             iFlag_first=0    
         else:            
             if  dDiatance < dDiatance_min:
                 dDiatance_min = dDiatance
                 #found it
```

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/index/define_stream_order.py` & `pyflowline-0.2.4/pyflowline/algorithms/index/define_stream_order.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py` & `pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_flowline.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,18 +62,19 @@
     aVertex_intersect=list()
     #for i in range (nfeature_mesh):
     for pFeature_flowline_a in pLayer_flowline_a:
        
         #pFeature_mesh= pLayer_mesh.GetFeature(i)
         pGeometry_flowline_a = pFeature_flowline_a.GetGeometryRef() 
         npoint = pFeature_flowline_a.GetPointCount()
-        aCoords = list()
+        aCoords_gcs = list()
         for i in range(0, npoint):                   
             pt = pFeature_flowline_a.GetPoint(i)
-            aCoords.append( [ pt[0], pt[1]])               
+            aCoords_gcs.append( [ pt[0], pt[1]])         
+
         aCoords_gcs= np.array(aCoords_gcs)       
 
         if (iFlag_transform ==1): #projections are different
             pGeometry_flowline_a.Transform(transform)
 
         if (pGeometry_flowline_a.IsValid()):
             pass
```

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py` & `pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py` & `pyflowline-0.2.4/pyflowline/algorithms/intersect/intersect_flowline_with_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/loop/remove_flowline_loop.py` & `pyflowline-0.2.4/pyflowline/algorithms/loop/remove_flowline_loop.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/merge/merge_flowline.py` & `pyflowline-0.2.4/pyflowline/algorithms/merge/merge_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/simplification/remove_returning_flowline.py` & `pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_returning_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/simplification/remove_small_river.py` & `pyflowline-0.2.4/pyflowline/algorithms/simplification/remove_small_river.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/split/find_flowline_confluence.py` & `pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_confluence.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/split/find_flowline_vertex.py` & `pyflowline-0.2.4/pyflowline/algorithms/split/find_flowline_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/split/split_by_length.py` & `pyflowline-0.2.4/pyflowline/algorithms/split/split_by_length.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/split/split_flowline.py` & `pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/algorithms/split/split_flowline_to_edge.py` & `pyflowline-0.2.4/pyflowline/algorithms/split/split_flowline_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/classes/_hpc.py` & `pyflowline-0.2.4/pyflowline/classes/_hpc.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/classes/basin.py` & `pyflowline-0.2.4/pyflowline/classes/basin.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pyflowline.formats.read_flowline import read_flowline_geojson
 from pyflowline.formats.read_nhdplus_flowline_shapefile import  read_nhdplus_flowline_geojson_attribute
 from pyflowline.formats.read_nhdplus_flowline_shapefile import extract_nhdplus_flowline_shapefile_by_attribute
 from pyflowline.formats.read_nhdplus_flowline_shapefile import track_nhdplus_flowline
 from pyflowline.formats.convert_flowline_to_geojson import convert_flowline_to_geojson
 from pyflowline.formats.export_flowline import export_flowline_to_geojson
 from pyflowline.formats.export_vertex import export_vertex_to_geojson
-from pyflowline.algorithms.auxiliary.text_reader_string import text_reader_string
+from pyflowline.external.pyearth.toolbox.reader.text_reader_string import text_reader_string
 
 
 
 from pyflowline.algorithms.split.find_flowline_vertex import find_flowline_vertex
 from pyflowline.algorithms.split.find_flowline_confluence import find_flowline_confluence
 from pyflowline.algorithms.split.split_flowline import split_flowline
 from pyflowline.algorithms.split.split_flowline_to_edge import split_flowline_to_edge
@@ -359,15 +359,15 @@
             nFlowline_after = len(aFlowline_basin_filtered)
             print('Basin ',  self.sBasinID, ' has dam', nFlowline_before, nFlowline_after)
             ptimer.stop()
         else:
             print('Basin ',  self.sBasinID, ' has no dam')
             sFilename_flowline_filter = self.sFilename_flowline_filter
             aFlowline_basin_filtered, pSpatial_reference = read_flowline_geojson( sFilename_flowline_filter ) 
-            aVertex_filtered = find_flowline_vertex(aFlowline_basin_filtered)  
+            #aVertex_filtered = find_flowline_vertex(aFlowline_basin_filtered)  
     
             pass
         sys.stdout.flush()
         if self.iFlag_disconnected == 1:
             #not used anymore                
             #aThreshold = np.full(2, 300.0, dtype=float)
             #aFlowline_basin_filtered = connect_disconnect_flowline(aFlowline_basin_filtered, aVertex, aThreshold)
@@ -391,33 +391,40 @@
         ptimer.stop()
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_vertex_without_confluence_before_intersect.geojson'
             sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             export_vertex_to_geojson( aVertex, sFilename_out)
         
         ptimer.start()
-        nFlowline_before = len(aFlowline_basin_filtered)
-        aFlowline_basin_simplified = split_flowline(aFlowline_basin_filtered, aVertex)
-        nFlowline_after = len(aFlowline_basin_simplified)
+        try:
+            nFlowline_before = len(aFlowline_basin_filtered)
+            aFlowline_basin_simplified = split_flowline(aFlowline_basin_filtered, aVertex)
+            nFlowline_after = len(aFlowline_basin_simplified)
+        except:
+            print(nFlowline_before)
         ptimer.stop()
         print('Basin ',  self.sBasinID, 'split flowline', nFlowline_before, nFlowline_after)
         if self.iFlag_debug ==1:
             sFilename_out = 'flowline_split_by_point_before_intersect.geojson'
             sFilename_out = os.path.join(sWorkspace_output_basin, sFilename_out)
             export_flowline_to_geojson(aFlowline_basin_simplified, sFilename_out)
         #use location to find outlet
         point= dict()   
         point['dLongitude_degree'] = self.dLongitude_outlet_degree
         point['dLatitude_degree'] = self.dLatitude_outlet_degree
         pVertex_outlet=pyvertex(point)
 
         ptimer.start()
-        nFlowline_before = len(aFlowline_basin_simplified)
-        aFlowline_basin_simplified = correct_flowline_direction(aFlowline_basin_simplified,  pVertex_outlet )
-        nFlowline_after = len(aFlowline_basin_simplified)
+        try:
+            nFlowline_before = len(aFlowline_basin_simplified)        
+            aFlowline_basin_simplified = correct_flowline_direction(aFlowline_basin_simplified,  pVertex_outlet )
+            nFlowline_after = len(aFlowline_basin_simplified)
+        except:
+            print(nFlowline_before)
+            
         ptimer.stop()
         
         print('Basin ',  self.sBasinID, 'flow direction', nFlowline_before, nFlowline_after)
         sys.stdout.flush()
         pVertex_outlet = aFlowline_basin_simplified[0].pVertex_end
         self.pVertex_outlet = pVertex_outlet
         if self.iFlag_debug ==1:
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/confluence.py` & `pyflowline-0.2.4/pyflowline/classes/confluence.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.flowline import pyflowline
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import calculate_angle_betwen_vertex
 else:
-    from pyflowline.algorithms.auxiliary.gdal_functions import  calculate_angle_betwen_vertex
+    from pyflowline.external.pyearth.gis.gdal.gdal_functions import  calculate_angle_betwen_vertex
 
 class ConfluenceClassEncoder(JSONEncoder):
     """Confluence Class Encoder
 
     Args:
         JSONEncoder (_type_): _description_
     """
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/edge.py` & `pyflowline-0.2.4/pyflowline/classes/edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from pyflowline.algorithms.split.split_by_length import split_edge_by_length
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import calculate_angle_betwen_vertex
     from pyflowline.algorithms.cython.kernel import calculate_distance_to_plane
 else:
-    from pyflowline.algorithms.auxiliary.gdal_functions import  calculate_angle_betwen_vertex
-    from pyflowline.algorithms.auxiliary.gdal_functions import calculate_distance_to_plane
+    from pyflowline.external.pyearth.gis.gdal.gdal_functions import  calculate_angle_betwen_vertex
+    from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_distance_to_plane
 
 class EdgeClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/flowline.py` & `pyflowline-0.2.4/pyflowline/classes/flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/classes/hexagon.py` & `pyflowline-0.2.4/pyflowline/classes/hexagon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.algorithms.auxiliary.gdal_functions import calculate_polygon_area
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
 
 class HexagonClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/latlon.py` & `pyflowline-0.2.4/pyflowline/classes/latlon.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.algorithms.auxiliary.gdal_functions import calculate_polygon_area
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
 
 class LatlonClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/link.py` & `pyflowline-0.2.4/pyflowline/classes/link.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/classes/mpas.py` & `pyflowline-0.2.4/pyflowline/classes/mpas.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.algorithms.auxiliary.gdal_functions import calculate_polygon_area
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
 
 class MpasClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/pycase.py` & `pyflowline-0.2.4/pyflowline/classes/pycase.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 from pyflowline.classes.latlon import pylatlon
 from pyflowline.classes.square import pysquare
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.basin import pybasin
 from pyflowline.classes.flowline import pyflowline
 from pyflowline.classes.edge import pyedge
 from pyflowline.formats.read_mesh import read_mesh_json, read_mesh_json_w_topology
-from pyflowline.algorithms.auxiliary.gdal_functions import reproject_coordinates
-from pyflowline.algorithms.auxiliary.gdal_functions  import degree_to_meter
-from pyflowline.algorithms.auxiliary.gdal_functions  import meter_to_degree
-from pyflowline.algorithms.auxiliary.gdal_functions import retrieve_geotiff_metadata
-from pyflowline.algorithms.auxiliary.gdal_functions import read_mesh_boundary
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates
+from pyflowline.external.pyearth.gis.gdal.gdal_functions  import degree_to_meter
+from pyflowline.external.pyearth.gis.gdal.gdal_functions  import meter_to_degree
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import retrieve_geotiff_metadata
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import read_mesh_boundary
 from pyflowline.mesh.hexagon.create_hexagon_mesh import create_hexagon_mesh
 from pyflowline.mesh.latlon.create_latlon_mesh import create_latlon_mesh
 from pyflowline.mesh.square.create_square_mesh import create_square_mesh
 from pyflowline.mesh.mpas.create_mpas_mesh import create_mpas_mesh
 from pyflowline.mesh.tin.create_tin_mesh import create_tin_mesh
 
 pDate = datetime.datetime.today()
@@ -71,14 +71,15 @@
     """
     iCase_index= 0
     
     sMesh_type = 1
     iFlag_standalone=1
     iFlag_flowline = 1
     iFlag_global = 0
+    iFlag_antarctic = 0
     iFlag_multiple_outlet = 0
     iFlag_mesh_boundary = 0
     #iFlag_use_shapefile_extent=1
     iFlag_use_mesh_dem=0
     iFlag_save_mesh = 0
     iFlag_simplification = 1 #user can turn on/off
     iFlag_create_mesh=1
@@ -162,14 +163,17 @@
         else:
             #without iFlag_flowline the model is a mesh generator
             self.iFlag_flowline=1
         
         if 'iFlag_global' in aConfig_in:
             self.iFlag_global             = int(aConfig_in[ 'iFlag_global'])
 
+        if 'iFlag_antarctic' in aConfig_in:
+            self.iFlag_antarctic             = int(aConfig_in[ 'iFlag_antarctic'])    
+
         if 'iFlag_mesh_boundary' in aConfig_in:
             self.iFlag_mesh_boundary             = int(aConfig_in[ 'iFlag_mesh_boundary'])
         else:
             self.iFlag_mesh_boundary=0
         
         if 'iFlag_multiple_outlet' in aConfig_in:
             self.iFlag_multiple_outlet             = int(aConfig_in[ 'iFlag_multiple_outlet'])  
@@ -397,22 +401,27 @@
                 aOutlet.append(pBasin.pVertex_outlet)
             
             self.aFlowline_simplified = aFlowline_out
               
 
         return aFlowline_out
     
-    def mesh_generation(self):
+    def mesh_generation(self, iFlag_antarctic_in=None):
         """
         The mesh generation operation
 
         Returns:
             list [pycell]: A list of cell object
         """
         print('Start mesh generation.')
+        if iFlag_antarctic_in is None:
+            iFlag_antarctic = 0
+        else:
+            iFlag_antarctic = iFlag_antarctic_in
+
         aCell_out = list()  
         if self.iFlag_create_mesh ==1:
             iFlag_global =  self.iFlag_global
             iMesh_type = self.iMesh_type
             iFlag_save_mesh = self.iFlag_save_mesh
             iFlag_rotation = self.iFlag_rotation
             iFlag_mesh_boundary = self.iFlag_mesh_boundary
@@ -568,41 +577,42 @@
                             iFlag_use_mesh_dem = self.iFlag_use_mesh_dem
                             sFilename_mesh_netcdf = self.sFilename_mesh_netcdf                            
                             dLatitude_top    = self.dLatitude_top   
                             dLatitude_bot    = self.dLatitude_bot   
                             dLongitude_left  = self.dLongitude_left 
                             dLongitude_right = self.dLongitude_right
 
-                            if iFlag_mesh_boundary ==1:
-                                #create a polygon based on 
-                                #read boundary 
-                                pBoundary = read_mesh_boundary(self.sFilename_mesh_boundary)
-
-                                aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, \
-                                  pBoundary,       sFilename_mesh_netcdf,      sFilename_mesh)
+                            if iFlag_antarctic ==1:                                                             
+                                aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, 
+                                            sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in )
                                 pass
                             else:
-                                pRing = ogr.Geometry(ogr.wkbLinearRing)
-                                pRing.AddPoint(dLongitude_left, dLatitude_top)
-                                pRing.AddPoint(dLongitude_right, dLatitude_top)
-                                pRing.AddPoint(dLongitude_right, dLatitude_bot)
-                                pRing.AddPoint(dLongitude_left, dLatitude_bot)
-                                pRing.AddPoint(dLongitude_left, dLatitude_top)
-                                pBoundary = ogr.Geometry(ogr.wkbPolygon)
-                                pBoundary.AddGeometry(pRing)
-                                pBoundary_rec = loads( pBoundary.ExportToWkt() )
-
-                                #old method using rectange
-                                #aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, \
-                                #  dLongitude_left, dLongitude_right,  dLatitude_top, dLatitude_bot, \
-                                #        sFilename_mesh_netcdf,      sFilename_mesh)
-
-                                #new method using polygon object
-                                aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, \
-                                  pBoundary_rec,       sFilename_mesh_netcdf,      sFilename_mesh)
+
+                                if iFlag_mesh_boundary ==1:
+                                    #create a polygon based on 
+                                    #read boundary 
+                                    pBoundary = read_mesh_boundary(self.sFilename_mesh_boundary)
+
+                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, 
+                                       sFilename_mesh_netcdf,  sFilename_mesh, iFlag_antarctic_in=iFlag_antarctic_in, pBoundary_in = pBoundary)
+                                    pass
+                                else:
+                                    pRing = ogr.Geometry(ogr.wkbLinearRing)
+                                    pRing.AddPoint(dLongitude_left, dLatitude_top)
+                                    pRing.AddPoint(dLongitude_right, dLatitude_top)
+                                    pRing.AddPoint(dLongitude_right, dLatitude_bot)
+                                    pRing.AddPoint(dLongitude_left, dLatitude_bot)
+                                    pRing.AddPoint(dLongitude_left, dLatitude_top)
+                                    pBoundary = ogr.Geometry(ogr.wkbPolygon)
+                                    pBoundary.AddGeometry(pRing)
+                                    pBoundary_rec = loads( pBoundary.ExportToWkt() )
+                                  
+                                    #new method using polygon object
+                                    aMpas = create_mpas_mesh(iFlag_global, iFlag_use_mesh_dem, iFlag_save_mesh, \
+                                           sFilename_mesh_netcdf, sFilename_mesh, iFlag_antarctic_in= iFlag_antarctic_in, pBoundary_in = pBoundary_rec  )
                             return aMpas
                         else:
                             if iMesh_type ==5: #tin this one need to be updated because central location issue
                                 #tin edge
                                 dArea = np.power(dResolution_meter,2.0)
                                 dLength_edge = np.sqrt(  4.0 * dArea /  np.sqrt(3.0) )  
                                 dX_shift = 0.5 * dLength_edge
@@ -763,15 +773,15 @@
             aCell = self.mesh_generation()
             if self.iFlag_intersect ==1:
                 aCell_out, a, b = self.reconstruct_topological_relationship(aCell)
             else:
                 pass
         else:
             #only mesh generator
-            aCell = self.mesh_generation()
+            aCell = self.mesh_generation(iFlag_antarctic_in= self.iFlag_antarctic)
             self.aCell = aCell      
             aCell_out = aCell
         
         return aCell_out
 
     def evaluate(self):
         """
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/square.py` & `pyflowline-0.2.4/pyflowline/classes/square.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from json import JSONEncoder
 import numpy as np
 from pyflowline.classes.vertex import pyvertex
 from pyflowline.classes.edge import pyedge
 from pyflowline.classes.cell import pycell
 from pyflowline.classes.flowline import pyflowline
-from pyflowline.algorithms.auxiliary.gdal_functions import calculate_polygon_area
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import calculate_polygon_area
 
 class SquareClassEncoder(JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.float32):
             return float(obj)
```

### Comparing `pyflowline-0.2.2/pyflowline/classes/timer.py` & `pyflowline-0.2.4/pyflowline/classes/timer.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/classes/tin.py` & `pyflowline-0.2.4/pyflowline/classes/tin.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/classes/vertex.py` & `pyflowline-0.2.4/pyflowline/classes/vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/convert_attributes.py` & `pyflowline-0.2.4/pyflowline/formats/convert_attributes.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/convert_coordinates.py` & `pyflowline-0.2.4/pyflowline/formats/convert_coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.classes.square import pysquare
 from pyflowline.classes.latlon import pylatlon
 from pyflowline.classes.mpas import pympas
 from pyflowline.classes.tin import pytin
 
-from pyflowline.algorithms.auxiliary.gdal_functions import reproject_coordinates
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates
 
 def convert_gcs_coordinates_to_cell(iMesh_type_in, \
     dLongitude_center_in, \
     dLatitude_center_in, \
         aCoordinates_gcs_in):
 
     npoint = len(aCoordinates_gcs_in)
```

### Comparing `pyflowline-0.2.2/pyflowline/formats/convert_flowline_to_geojson.py` & `pyflowline-0.2.4/pyflowline/formats/convert_flowline_to_geojson.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/export_flowline.py` & `pyflowline-0.2.4/pyflowline/formats/export_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/export_mesh.py` & `pyflowline-0.2.4/pyflowline/formats/export_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/export_vertex.py` & `pyflowline-0.2.4/pyflowline/formats/export_vertex.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/read_flowline.py` & `pyflowline-0.2.4/pyflowline/formats/read_flowline.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/read_mesh.py` & `pyflowline-0.2.4/pyflowline/formats/read_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/formats/read_nhdplus_flowline_shapefile.py` & `pyflowline-0.2.4/pyflowline/formats/read_nhdplus_flowline_shapefile.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/mesh/dggrid/create_dggrid_case.py` & `pyflowline-0.2.4/pyflowline/mesh/dggrid/create_dggrid_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 import sys, os, stat
 import numpy as np
 from pathlib import Path
 from shutil import copy2
 import subprocess
 import datetime
 
+from pyflowline.external.pyearth.system.define_global_variables import *
 
 pDate = datetime.datetime.today()
 sDate_default = "{:04d}".format(pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
 
-def create_dggrid_case( iCase_index, \
-    iResolution_index ,\
-        sGrid_type,\
-            sDate_in = None, \
+def create_dggrid_mesh( iCase_index, 
+    iResolution_index ,
+        sGrid_type,
+            sDate_in = None, 
         sFilename_crop_shapefile_in =None ):
 
     sCase = "{:03d}".format( iCase_index )
     sResolution = "{:02d}".format( iResolution_index )
 
     if sDate_in is not None:
         sDate = sDate_in
```

### Comparing `pyflowline-0.2.2/pyflowline/mesh/hexagon/create_hexagon_mesh.py` & `pyflowline-0.2.4/pyflowline/mesh/hexagon/create_hexagon_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import os
 import numpy as np
 from osgeo import ogr, osr
 from shapely.wkt import loads
 from pyflowline.classes.hexagon import pyhexagon
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 from pyflowline.algorithms.auxiliary.find_index_in_list import check_if_duplicates
-from pyflowline.algorithms.auxiliary.gdal_functions import reproject_coordinates_batch
+
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates_batch
 
 def create_hexagon_mesh(iFlag_rotation_in, 
         dX_left_in, dY_bot_in, 
         dResolution_meter_in, 
         ncolumn_in, 
         nrow_in,
         pPolygon_in,
```

### Comparing `pyflowline-0.2.2/pyflowline/mesh/latlon/create_latlon_mesh.py` & `pyflowline-0.2.4/pyflowline/mesh/latlon/create_latlon_mesh.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/mesh/mpas/create_mpas_mesh.py` & `pyflowline-0.2.4/pyflowline/mesh/mpas/create_mpas_mesh.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,46 +7,60 @@
 from shapely.wkt import loads
 from pyflowline.formats.convert_attributes import convert_gcs_attributes_to_cell
 
 iFlag_cython = importlib.util.find_spec("cython") 
 if iFlag_cython is not None:
     from pyflowline.algorithms.cython.kernel import convert_360_to_180
 else:
-    from pyflowline.algorithms.auxiliary.gdal_functions import convert_360_to_180
+    from pyflowline.external.pyearth.gis.gdal.gdal_functions import convert_360_to_180
 
 def create_mpas_mesh(iFlag_global_in, 
     iFlag_use_mesh_dem, 
     iFlag_save_mesh_in, 
-    pPolygon_in, 
+    
     sFilename_mesh_netcdf_in, 
-    sFilename_output_in): 
+    sFilename_output_in,
+    iFlag_antarctic_in=None,
+    pBoundary_in = None): 
     """
     Create a MPAS mesh
 
     Args:
         iFlag_global_in (int): _description_
         iFlag_use_mesh_dem (int): _description_
         iFlag_save_mesh_in (int): _description_
-        pPolygon_in (_type_): _description_
+        pBoundary_in (_type_): _description_
         sFilename_mesh_netcdf_in (_type_): _description_
         sFilename_output_in (_type_): _description_
 
     Returns:
         _type_: _description_
     """
+
+    if iFlag_antarctic_in is None:
+        iFlag_antarctic=0
+    else:
+        iFlag_antarctic=iFlag_antarctic_in
+
+    if pBoundary_in is None:
+        pBoundary = None
+    else:
+        pBoundary = pBoundary_in
        
     if (os.path.exists(sFilename_mesh_netcdf_in)):
         pass
     else:
         print('Mesh file does not exist!')
         return
     
     if os.path.exists(sFilename_output_in):  
         os.remove(sFilename_output_in)
 
+    iFlag_remove_ice = 0
+
     pDatasets_in = Dataset(sFilename_mesh_netcdf_in)
 
     netcdf_format = pDatasets_in.file_format
     pDriver_geojson = ogr.GetDriverByName('GeoJSON')     
     pSpatial_reference_gcs = osr.SpatialReference()  
     pSpatial_reference_gcs.ImportFromEPSG(4326)    # WGS84 lat/lon    
     #geojson
@@ -180,99 +194,130 @@
     aIce_thickness = ice_thickness0[:]
     aCellArea = areaCell0[:]
     aDcEdge = dcEdge0[:]
     aBed_elevation_profile = bed_elevation_profile0[:]  #elevation    
     ncell = len(aIndexToCellID) 
     aMpas = list()
     for i in range(ncell):
+        #center
         dLat = convert_360_to_180 (aLatitudeCell[i])
         dLon = convert_360_to_180 (aLongitudeCell[i])
-        pCenter = ogr.Geometry(ogr.wkbPoint)
-        pCenter.AddPoint(dLon, dLat)
-        pCenter1 = loads( pCenter.ExportToWkt() )
-        
-        
-        iFlag = pCenter1.within(pPolygon_in)
+
+        #vertex
+        aCellOnCellIndex = np.array(aCellsOnCell[i,:])
+        aEdgesOnCellIndex = np.array(aEdgesOnCell[i,:])
+        aVertexOnCellIndex = np.array(aVertexOnCell[i,:])
+        dummy0 = np.where(aVertexOnCellIndex > 0)
+        aVertexIndex = aVertexOnCellIndex[dummy0]
+        dummy1 = np.where(aEdgesOnCellIndex > 0)
+        aEdgeIndex= aEdgesOnCellIndex[dummy1]
+        dummy2 = np.where(aCellOnCellIndex > 0)
+        aNeighborIndex= (aCellOnCellIndex[dummy2]).astype(int)
+        aVertexIndexOnEdge = np.array(aVertexOnEdge0[aEdgeIndex-1,:]).astype((int))
+        aLonVertex = aLongitudeVertex[aVertexIndex-1]
+        aLatVertex = aLatitudeVertex[aVertexIndex-1]
+        nVertex = len(aLonVertex)
+
+        if iFlag_antarctic == 1:
+            #if it is antarctic, we dont need the boundary
+            if dLat < -60:
+                iFlag = True
+            else:  
+                iFlag = False
+            pass
+        else:
+            #we will check vertex insteaf of center
+            iFlag = False
+            for j in range(nVertex):
+                x1 = convert_360_to_180(aLonVertex[j])
+                y1 = aLatVertex[j]                
+                pVertex = ogr.Geometry(ogr.wkbPoint)
+                pVertex.AddPoint(x1, y1)
+                pVertex1 = loads( pVertex.ExportToWkt() )   
+                iFlag = pVertex1.within(pBoundary)
+                if iFlag == True:
+                    break
+                else:
+                    continue
+                
+            pass 
+
+
         if ( iFlag == True ):
             #get cell edge
             lCellID = int(aIndexToCellID[i])
             dElevation_mean = float(aBed_elevation[i])
             dElevation_profile0 = float(aBed_elevation_profile[i,0])
             dThickness_ice = float( aIce_thickness[i] )
             dArea = float(aCellArea[i])
-            if dThickness_ice > 0:
-                continue
-            else:
-                aCellOnCellIndex = np.array(aCellsOnCell[i,:])
-                aEdgesOnCellIndex = np.array(aEdgesOnCell[i,:])
-                aVertexOnCellIndex = np.array(aVertexOnCell[i,:])
-                dummy0 = np.where(aVertexOnCellIndex > 0)
-                aVertexIndex = aVertexOnCellIndex[dummy0]
-                dummy1 = np.where(aEdgesOnCellIndex > 0)
-                aEdgeIndex= aEdgesOnCellIndex[dummy1]
-                dummy2 = np.where(aCellOnCellIndex > 0)
-                aNeighborIndex= (aCellOnCellIndex[dummy2]).astype(int)
-                aVertexIndexOnEdge = np.array(aVertexOnEdge0[aEdgeIndex-1,:]).astype((int))
-                aLonVertex = aLongitudeVertex[aVertexIndex-1]
-                aLatVertex = aLatitudeVertex[aVertexIndex-1]
-                nVertex = len(aLonVertex)
-                ring = ogr.Geometry(ogr.wkbLinearRing)
-                aCoords = np.full((nVertex,2), -9999.0, dtype=float)
-
-                for j in range(nVertex):
-                    x1 = convert_360_to_180(aLonVertex[j])
-                    y1 = aLatVertex[j]      
-                    ring.AddPoint(x1, y1)
-                    aCoords[j,0] = x1
-                    aCoords[j,1] = y1
+            if iFlag_remove_ice == 1:
+                if dThickness_ice > 0 :
+                    continue
+                else:
                     pass
-
-                if iFlag_save_mesh_in ==1:
-                    x1 = convert_360_to_180(aLonVertex[0])
-                    y1 = aLatVertex[0]
-                    ring.AddPoint(x1, y1) #double check            
-                    pPolygon = ogr.Geometry(ogr.wkbPolygon)
-                    pPolygon.AddGeometry(ring)
-                    pFeature.SetGeometry(pPolygon)
-                    pFeature.SetField("id", int(lCellID) )
-                    pFeature.SetField("lon", dLon )
-                    pFeature.SetField("lat", dLat )
-                    pFeature.SetField("area", dArea )
-                    if iFlag_use_mesh_dem == 1:
-                        pFeature.SetField("elev", dElevation_mean )
-                        pFeature.SetField("elev0", dElevation_profile0 )
-
-                    pLayer.CreateFeature(pFeature)
-
-                pmpas = convert_gcs_attributes_to_cell(4, dLon, dLat, aCoords, aVertexIndex, aEdgeIndex, aVertexIndexOnEdge)               
-                pmpas.dArea = dArea
-                pmpas.calculate_edge_length()
-                pmpas.dLength_flowline = pmpas.dLength_edge #Default
-                pmpas.lCellID = lCellID
-                pmpas.dElevation_mean  = dElevation_mean
-                pmpas.dElevation_profile0 = dElevation_profile0
-                pmpas.aNeighbor=aNeighborIndex
-                pmpas.nNeighbor=len(aNeighborIndex)
-                pmpas.aNeighbor_land=aNeighborIndex
-                pmpas.nNeighbor_land=len(aNeighborIndex)
-                aDistance=list()
-                for i in range(pmpas.nNeighbor):
-                    lNeighborID = pmpas.aNeighbor[i]
-                    #find shared edge
-                    lEdgeID= aEdgeIndex[i]                    
-                    #lIndex = aIndexToEdgeID[lEdgeID-1]
-                    lIndex = lEdgeID-1
-                    dDistance = aDcEdge[lIndex]
-                    aDistance.append(dDistance)
-                    pass
-
-                pmpas.aNeighbor_distance = aDistance
-                aMpas.append(pmpas)
-                #get vertex
-
+            else:
+                pass
+            
+            ring = ogr.Geometry(ogr.wkbLinearRing)
+            aCoords = np.full((nVertex,2), -9999.0, dtype=float)
+            
+            for j in range(nVertex):
+                x1 = convert_360_to_180(aLonVertex[j])
+                y1 = aLatVertex[j]      
+                ring.AddPoint(x1, y1)
+                aCoords[j,0] = x1
+                aCoords[j,1] = y1
+                pass
+
+            if iFlag_save_mesh_in ==1:
+                x1 = convert_360_to_180(aLonVertex[0])
+                y1 = aLatVertex[0]
+                ring.AddPoint(x1, y1) #double check            
+                pPolygon = ogr.Geometry(ogr.wkbPolygon)
+                pPolygon.AddGeometry(ring)
+                pFeature.SetGeometry(pPolygon)
+                pFeature.SetField("id", int(lCellID) )
+                pFeature.SetField("lon", dLon )
+                pFeature.SetField("lat", dLat )
+                pFeature.SetField("area", dArea )
+                if iFlag_use_mesh_dem == 1:
+                    pFeature.SetField("elev", dElevation_mean )
+                    pFeature.SetField("elev0", dElevation_profile0 )
+                pLayer.CreateFeature(pFeature)
+
+            pmpas = convert_gcs_attributes_to_cell(4, dLon, dLat, aCoords, aVertexIndex, aEdgeIndex, aVertexIndexOnEdge)               
+            pmpas.dArea = dArea
+            pmpas.calculate_edge_length()
+            pmpas.dLength_flowline = pmpas.dLength_edge #Default
+            pmpas.lCellID = lCellID
+            pmpas.dElevation_mean  = dElevation_mean
+            pmpas.dElevation_profile0 = dElevation_profile0
+            pmpas.aNeighbor=aNeighborIndex
+            pmpas.nNeighbor=len(aNeighborIndex)
+            pmpas.aNeighbor_land=aNeighborIndex
+            pmpas.nNeighbor_land=len(aNeighborIndex)
+            aDistance=list()
+            for i in range(pmpas.nNeighbor):
+                lNeighborID = pmpas.aNeighbor[i]
+                #find shared edge
+                lEdgeID= aEdgeIndex[i]                    
+                #lIndex = aIndexToEdgeID[lEdgeID-1]
+                lIndex = lEdgeID-1
+                dDistance = aDcEdge[lIndex]
+                aDistance.append(dDistance)
+                pass
+            pmpas.aNeighbor_distance = aDistance
+            aMpas.append(pmpas)
+            #get vertex
+        else:
+            #if dLat< -54:
+            #    print(dLon, dLat)
+            #else:
+            #    pass
+            pass
         pass
 
     #for maps we need to clean some cell because they were not actually in the domain
 
     if iFlag_global_in == 1:
         aMpas_out = aMpas
     else:
```

### Comparing `pyflowline-0.2.2/pyflowline/mesh/square/create_square_mesh.py` & `pyflowline-0.2.4/pyflowline/mesh/square/create_square_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 #we will use gdal api for most operations
 import os
 from osgeo import ogr, osr
 import numpy as np
 from shapely.wkt import loads
 from pyflowline.classes.square import pysquare
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
-from pyflowline.algorithms.auxiliary.gdal_functions import  reproject_coordinates_batch
+
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import  reproject_coordinates_batch
 
 def create_square_mesh(dX_left_in, dY_bot_in, dResolution_meter_in, ncolumn_in, nrow_in, pPolygon_in,
     sFilename_output_in, sFilename_spatial_reference_in):   
     """
     _summary_
 
     Args:
```

### Comparing `pyflowline-0.2.2/pyflowline/mesh/tin/create_tin_mesh.py` & `pyflowline-0.2.4/pyflowline/mesh/tin/create_tin_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from osgeo import ogr, osr
 from shapely.wkt import loads
 from pyflowline.classes.tin import pytin
 
 from pyflowline.formats.convert_coordinates import convert_pcs_coordinates_to_cell
 from pyflowline.formats.convert_coordinates import convert_gcs_coordinates_to_cell
 from pyflowline.algorithms.auxiliary.find_index_in_list import check_if_duplicates
-from pyflowline.algorithms.auxiliary.gdal_functions import reproject_coordinates_batch
+
+from pyflowline.external.pyearth.gis.gdal.gdal_functions import reproject_coordinates_batch
 
 def create_tin_mesh(dX_left_in, dY_bot_in, dResolution_meter_in, ncolumn_in, nrow_in, pPolygon_in,
 sFilename_output_in, sFilename_spatial_reference_in):
      
     
     if os.path.exists(sFilename_output_in): 
         #delete it if it exists
```

### Comparing `pyflowline-0.2.2/pyflowline/pyflowline_create_template_configuration_file.py` & `pyflowline-0.2.4/pyflowline/pyflowline_create_template_configuration_file.py`

 * *Files identical despite different names*

### Comparing `pyflowline-0.2.2/pyflowline/pyflowline_read_model_configuration_file.py` & `pyflowline-0.2.4/pyflowline/pyflowline_read_model_configuration_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from pathlib import Path
 import datetime
 import json
 from pyflowline.classes.pycase import flowlinecase
 pDate = datetime.datetime.today()
 sDate_default = "{:04d}".format(pDate.year) + "{:02d}".format(pDate.month) + "{:02d}".format(pDate.day)
 
-def pyflowline_read_model_configuration_file(sFilename_configuration_in,   \
-    iFlag_standalone_in= None, \
-        iFlag_use_mesh_dem_in=None, \
-        iCase_index_in=None,   \
-            dResolution_degree_in = None,  \
-            dResolution_meter_in = None,  \
-                sMesh_type_in = None,  \
-                sModel_in = None, \
-                    sDate_in = None,\
+def pyflowline_read_model_configuration_file(sFilename_configuration_in,   
+    iFlag_standalone_in= None, 
+        iFlag_use_mesh_dem_in=None, 
+        iCase_index_in=None,   
+            dResolution_degree_in = None,  
+            dResolution_meter_in = None,  
+                sMesh_type_in = None,  
+                sModel_in = None, 
+                    sDate_in = None,
                     sWorkspace_output_in = None):
     """read a model configuration
 
     Args:
         sFilename_configuration_in (str): _description_
         iFlag_standalone_in (int, optional): _description_. Defaults to None.
         iFlag_use_mesh_dem_in (int, optional): _description_. Defaults to None.
```

### Comparing `pyflowline-0.2.2/pyflowline.egg-info/PKG-INFO` & `pyflowline-0.2.4/pyflowline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyflowline
-Version: 0.2.2
-Summary: A mesh independent river network generator for hydrologic models
+Version: 0.2.4
+Summary: A mesh-independent river network generator for hydrologic models
 Home-page: https://github.com/changliao1025/pyflowline
 Author: Chang Liao
 Author-email: chang.liao@pnnl.gov
 License: custom
 Keywords: Earth Science
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -15,32 +15,49 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: visualization
-License-File: LICENSE.md
+License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 ### PyFlowline
 
 [![DOI](https://zenodo.org/badge/368338554.svg)](https://zenodo.org/badge/latestdoi/368338554)
+[![Downloads](https://static.pepy.tech/badge/pyflowline)](https://pepy.tech/project/pyflowline)
 
 PyFlowline: a mesh-independent river network generator for hydrologic models. 
 
 PyFlowline is mesh independent, meaning you can apply it to both structured (e.g., traditional rectangle mesh, latitude-longitude, hexagon) and unstructured mesh systems (e.g., Triangulated Irregular Network (TIN) mesh and Model for Prediction Across Scales (MPAS) mesh).
 
 This package generates the mesh cell-based conceptual river networks using the following steps:
 
 1. `Flowline simplification`: PyFlowline checks the vector dataset and corrects undesired flowlines, such as braided rivers.
 2. `Mesh generation`: PyFlowline generates structured meshes (e.g., rectangle, hexagon) or imports user-provided unstructured meshes into the PyFlowline-compatible GEOJSON format.
 3. `Topological relationship reconstruction`: PyFlowline reconstructs the topological relationship using the mesh and flowline intersections.
 
+
+### Dependency
+
+PyFlowline depends on the following packages
+
+1. `numpy`
+2. `gdal`
+3. `netCDF4`
+4. `shapely`
+
+PyFlowline also has three optional dependency packages
+
+1. `cython` for performance 
+2. `matplotlin` for visualization
+3. `cartopy` for visulization
+
 ### Quickstart
 
 Please refer to the [quickstart documentation](https://pyflowline.readthedocs.io/en/latest/quickstart.html) for details on how to get started using the PyFlowline package.
 
 ### Installation
 
 Please refer to the [official documentation](https://pyflowline.readthedocs.io/) for details on how to install the PyFlowline package.
@@ -51,14 +68,16 @@
 
 ### Acknowledgment
 
 This work was supported by the Earth System Model Development program areas of the U.S. Department of Energy, Office of Science, Office of Biological and Environmental Research as part of the multi-program, collaborative Integrated Coastal Modeling (ICoM) project and the Interdisciplinary Research for Arctic Coastal Environments (InteRFACE) project.
 
 ### License
 
+BSD 3-Clause License
+
 Copyright © 2022, Battelle Memorial Institute
 
 1. Battelle Memorial Institute (hereinafter Battelle) hereby grants permission to any person or entity lawfully obtaining a copy of this software and associated documentation files (hereinafter “the Software”) to redistribute and use the Software in source and binary forms, with or without modification. Such person or entity may use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software and may permit others to do so, subject to the following conditions:
 
 * Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimers.
 
 * Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
@@ -67,11 +86,11 @@
 
 2. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL BATTELLE OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 ### References
 
 Several publications describe the algorithms used in `PyFlowline` in detail. If you make use of `PyFlowline` in your work, please consider including a reference to the following:
 
-* Liao. C. Cooper, M (2022) Pyflowline: a mesh independent river network generator for hydrologic models. Zenodo.
+* Liao. C. Cooper, M (2022) Pyflowline: a mesh-independent river network generator for hydrologic models. Zenodo.
 https://doi.org/10.5281/zenodo.6407299
 
 * Liao, C., Zhou, T., Xu, D., Cooper, M. G., Engwirda, D., Li, H.-Y., & Leung, L. R. (2023). Topological relationship-based flow direction modeling: Mesh-independent river networks representation. Journal of Advances in Modeling Earth Systems, 15, e2022MS003089. https://doi.org/10.1029/2022MS003089
```

### Comparing `pyflowline-0.2.2/pyflowline.egg-info/SOURCES.txt` & `pyflowline-0.2.4/pyflowline.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
-LICENSE.md
+LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 docs/make.bat
 docs/figures/after_loop.png
 docs/figures/after_merge.png
@@ -62,17 +62,15 @@
 pyflowline.egg-info/top_level.txt
 pyflowline/algorithms/__init__.py
 pyflowline/algorithms/auxiliary/__init__.py
 pyflowline/algorithms/auxiliary/calculate_area_of_difference.py
 pyflowline/algorithms/auxiliary/check_head_water.py
 pyflowline/algorithms/auxiliary/find_index_in_list.py
 pyflowline/algorithms/auxiliary/find_vertex_in_list.py
-pyflowline/algorithms/auxiliary/gdal_functions.py
 pyflowline/algorithms/auxiliary/longlat_to_3d.py
-pyflowline/algorithms/auxiliary/text_reader_string.py
 pyflowline/algorithms/connection/__init__.py
 pyflowline/algorithms/connection/connect_disconnect_flowline.py
 pyflowline/algorithms/cython/__init__.py
 pyflowline/algorithms/cython/setup.py
 pyflowline/algorithms/direction/__init__.py
 pyflowline/algorithms/direction/correct_flowline_direction.py
 pyflowline/algorithms/index/__init__.py
@@ -123,18 +121,19 @@
 pyflowline/formats/export_mesh.py
 pyflowline/formats/export_vertex.py
 pyflowline/formats/read_flowline.py
 pyflowline/formats/read_mesh.py
 pyflowline/formats/read_nhdplus_flowline_shapefile.py
 pyflowline/mesh/__init__.py
 pyflowline/mesh/dggrid/__init__.py
-pyflowline/mesh/dggrid/create_dggrid_case.py
+pyflowline/mesh/dggrid/create_dggrid_mesh.py
 pyflowline/mesh/hexagon/__init__.py
 pyflowline/mesh/hexagon/create_hexagon_mesh.py
 pyflowline/mesh/latlon/__init__.py
 pyflowline/mesh/latlon/create_latlon_mesh.py
 pyflowline/mesh/mpas/__init__.py
 pyflowline/mesh/mpas/create_mpas_mesh.py
 pyflowline/mesh/square/__init__.py
 pyflowline/mesh/square/create_square_mesh.py
 pyflowline/mesh/tin/__init__.py
-pyflowline/mesh/tin/create_tin_mesh.py
+pyflowline/mesh/tin/create_tin_mesh.py
+tests/test_installation.py
```

### Comparing `pyflowline-0.2.2/setup.py` & `pyflowline-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import subprocess
 import shutil
 
 from setuptools import setup, find_packages, Command
 
 NAME = "pyflowline"
 DESCRIPTION = \
-    "A mesh independent river network generator for hydrologic models"
+    "A mesh-independent river network generator for hydrologic models"
 AUTHOR = "Chang Liao"
 AUTHOR_EMAIL = "chang.liao@pnnl.gov"
 URL = "https://github.com/changliao1025/pyflowline"
-VERSION = "0.2.2"
+VERSION = "0.2.4"
 REQUIRES_PYTHON = ">=3.8.0"
 KEYWORDS = "Earth Science"
 
 REQUIRED = [
     "numpy", 
     "gdal",
     "netCDF4",
@@ -57,10 +57,10 @@
     python_requires=REQUIRES_PYTHON,
     keywords=KEYWORDS,
     url=URL,
     packages=find_packages(),
     install_requires=REQUIRED,
     classifiers=CLASSIFY,
     extras_require={
-        'visualization': ['matplotlib', 'cartopy>=0.21.0']
+        'visualization': ['cython', 'matplotlib', 'cartopy>=0.21.0']
     }
 )
```

