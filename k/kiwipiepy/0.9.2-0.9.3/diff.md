# Comparing `tmp/kiwipiepy-0.9.2.tar.gz` & `tmp/kiwipiepy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwipiepy-0.9.2.tar", last modified: Tue Jan 19 17:02:39 2021, max compression
+gzip compressed data, was "kiwipiepy-0.9.3.tar", last modified: Sat Jun  5 17:55:08 2021, max compression
```

## Comparing `kiwipiepy-0.9.2.tar` & `kiwipiepy-0.9.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.353694 kiwipiepy-0.9.2/
--rw-r--r--   0 root         (0) root         (0)      831 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      144 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      929 2021-01-19 17:02:39.353694 kiwipiepy-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17736 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.337694 kiwipiepy-0.9.2/kiwipiepy/
--rw-r--r--   0 root         (0) root         (0)     1818 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/kiwipiepy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      179 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/kiwipiepy/__main__.py
--rw-r--r--   0 root         (0) root         (0)       21 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/kiwipiepy/_version.py
--rw-r--r--   0 root         (0) root         (0)    20516 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/kiwipiepy/documentation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.337694 kiwipiepy-0.9.2/kiwipiepy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      929 2021-01-19 17:02:39.000000 kiwipiepy-0.9.2/kiwipiepy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1531 2021-01-19 17:02:39.000000 kiwipiepy-0.9.2/kiwipiepy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 17:02:39.000000 kiwipiepy-0.9.2/kiwipiepy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2021-01-19 17:02:39.000000 kiwipiepy-0.9.2/kiwipiepy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2021-01-19 17:02:39.000000 kiwipiepy-0.9.2/kiwipiepy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.333694 kiwipiepy-0.9.2/mimalloc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.341694 kiwipiepy-0.9.2/mimalloc/include/
--rw-r--r--   0 root         (0) root         (0)    14175 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/include/mimalloc-atomic.h
--rw-r--r--   0 root         (0) root         (0)    29451 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/include/mimalloc-internal.h
--rw-r--r--   0 root         (0) root         (0)     2996 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/include/mimalloc-new-delete.h
--rw-r--r--   0 root         (0) root         (0)     3052 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/include/mimalloc-override.h
--rw-r--r--   0 root         (0) root         (0)    21163 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/include/mimalloc-types.h
--rw-r--r--   0 root         (0) root         (0)    26879 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/include/mimalloc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.345694 kiwipiepy-0.9.2/mimalloc/src/
--rw-r--r--   0 root         (0) root         (0)     9807 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/alloc-aligned.c
--rw-r--r--   0 root         (0) root         (0)     7274 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/alloc-override-osx.c
--rw-r--r--   0 root         (0) root         (0)    12063 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/alloc-override.c
--rw-r--r--   0 root         (0) root         (0)     5396 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/alloc-posix.c
--rw-r--r--   0 root         (0) root         (0)    30425 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/alloc.c
--rw-r--r--   0 root         (0) root         (0)    15392 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/arena.c
--rw-r--r--   0 root         (0) root         (0)     9516 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/bitmap.inc.c
--rw-r--r--   0 root         (0) root         (0)    18818 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/heap.c
--rw-r--r--   0 root         (0) root         (0)    20095 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/init.c
--rw-r--r--   0 root         (0) root         (0)    17648 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/options.c
--rw-r--r--   0 root         (0) root         (0)    46106 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/os.c
--rw-r--r--   0 root         (0) root         (0)    12678 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/page-queue.c
--rw-r--r--   0 root         (0) root         (0)    32699 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/page.c
--rw-r--r--   0 root         (0) root         (0)    11610 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/random.c
--rw-r--r--   0 root         (0) root         (0)    20512 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/region.c
--rw-r--r--   0 root         (0) root         (0)    55589 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/segment.c
--rw-r--r--   0 root         (0) root         (0)     1142 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/static.c
--rw-r--r--   0 root         (0) root         (0)    20977 2021-01-19 17:02:38.000000 kiwipiepy-0.9.2/mimalloc/src/stats.c
--rw-r--r--   0 root         (0) root         (0)       38 2021-01-19 17:02:39.353694 kiwipiepy-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2502 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.345694 kiwipiepy-0.9.2/src/
--rw-r--r--   0 root         (0) root         (0)    27898 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/src/KiwiPy.cpp
--rw-r--r--   0 root         (0) root         (0)    16734 2021-01-19 17:02:13.000000 kiwipiepy-0.9.2/src/PyDoc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 17:02:39.353694 kiwipiepy-0.9.2/src/core/
--rw-r--r--   0 root         (0) root         (0)     4825 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/BakedMap.hpp
--rw-r--r--   0 root         (0) root         (0)     2101 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KFeatureTestor.cpp
--rw-r--r--   0 root         (0) root         (0)      584 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KFeatureTestor.h
--rw-r--r--   0 root         (0) root         (0)     7031 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KForm.cpp
--rw-r--r--   0 root         (0) root         (0)     3089 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KForm.h
--rw-r--r--   0 root         (0) root         (0)    15890 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KModelMgr.cpp
--rw-r--r--   0 root         (0) root         (0)     2398 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KModelMgr.h
--rw-r--r--   0 root         (0) root         (0)     7556 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KNLangModel.cpp
--rw-r--r--   0 root         (0) root         (0)     6912 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KNLangModel.h
--rw-r--r--   0 root         (0) root         (0)    11136 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KTrie.cpp
--rw-r--r--   0 root         (0) root         (0)     1457 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KTrie.h
--rw-r--r--   0 root         (0) root         (0)    14449 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KWordDetector.cpp
--rw-r--r--   0 root         (0) root         (0)     7787 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KWordDetector.h
--rw-r--r--   0 root         (0) root         (0)    24520 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/Kiwi.cpp
--rw-r--r--   0 root         (0) root         (0)     4026 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/Kiwi.h
--rw-r--r--   0 root         (0) root         (0)     2133 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/KiwiHeader.h
--rw-r--r--   0 root         (0) root         (0)     4178 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/PatternMatcher.cpp
--rw-r--r--   0 root         (0) root         (0)      782 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/PatternMatcher.h
--rw-r--r--   0 root         (0) root         (0)     2840 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/ThreadPool.h
--rw-r--r--   0 root         (0) root         (0)     3505 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/Trie.hpp
--rw-r--r--   0 root         (0) root         (0)     5857 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/Utils.cpp
--rw-r--r--   0 root         (0) root         (0)     3072 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/Utils.h
--rw-r--r--   0 root         (0) root         (0)      548 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/logPoisson.h
--rw-r--r--   0 root         (0) root         (0)    12843 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/pattern.hpp
--rw-r--r--   0 root         (0) root         (0)     2845 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/serializer.cpp
--rw-r--r--   0 root         (0) root         (0)     5189 2021-01-19 17:02:36.000000 kiwipiepy-0.9.2/src/core/serializer.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.682192 kiwipiepy-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)      831 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      144 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      912 2021-06-05 17:55:08.682192 kiwipiepy-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17736 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.674192 kiwipiepy-0.9.3/kiwipiepy/
+-rw-r--r--   0 root         (0) root         (0)     1818 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/kiwipiepy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      179 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/kiwipiepy/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/kiwipiepy/_version.py
+-rw-r--r--   0 root         (0) root         (0)    20624 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/kiwipiepy/documentation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.674192 kiwipiepy-0.9.3/kiwipiepy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      912 2021-06-05 17:55:08.000000 kiwipiepy-0.9.3/kiwipiepy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1531 2021-06-05 17:55:08.000000 kiwipiepy-0.9.3/kiwipiepy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-06-05 17:55:08.000000 kiwipiepy-0.9.3/kiwipiepy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2021-06-05 17:55:08.000000 kiwipiepy-0.9.3/kiwipiepy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2021-06-05 17:55:08.000000 kiwipiepy-0.9.3/kiwipiepy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.674192 kiwipiepy-0.9.3/mimalloc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.674192 kiwipiepy-0.9.3/mimalloc/include/
+-rw-r--r--   0 root         (0) root         (0)    14175 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/include/mimalloc-atomic.h
+-rw-r--r--   0 root         (0) root         (0)    29451 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/include/mimalloc-internal.h
+-rw-r--r--   0 root         (0) root         (0)     2996 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/include/mimalloc-new-delete.h
+-rw-r--r--   0 root         (0) root         (0)     3052 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/include/mimalloc-override.h
+-rw-r--r--   0 root         (0) root         (0)    21163 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/include/mimalloc-types.h
+-rw-r--r--   0 root         (0) root         (0)    26879 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/include/mimalloc.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.678192 kiwipiepy-0.9.3/mimalloc/src/
+-rw-r--r--   0 root         (0) root         (0)     9807 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/alloc-aligned.c
+-rw-r--r--   0 root         (0) root         (0)     7274 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/alloc-override-osx.c
+-rw-r--r--   0 root         (0) root         (0)    12063 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/alloc-override.c
+-rw-r--r--   0 root         (0) root         (0)     5396 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/alloc-posix.c
+-rw-r--r--   0 root         (0) root         (0)    30425 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/alloc.c
+-rw-r--r--   0 root         (0) root         (0)    15392 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/arena.c
+-rw-r--r--   0 root         (0) root         (0)     9516 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/bitmap.inc.c
+-rw-r--r--   0 root         (0) root         (0)    18818 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/heap.c
+-rw-r--r--   0 root         (0) root         (0)    20095 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/init.c
+-rw-r--r--   0 root         (0) root         (0)    17648 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/options.c
+-rw-r--r--   0 root         (0) root         (0)    46106 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/os.c
+-rw-r--r--   0 root         (0) root         (0)    12678 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/page-queue.c
+-rw-r--r--   0 root         (0) root         (0)    32699 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/page.c
+-rw-r--r--   0 root         (0) root         (0)    11610 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/random.c
+-rw-r--r--   0 root         (0) root         (0)    20512 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/region.c
+-rw-r--r--   0 root         (0) root         (0)    55589 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/segment.c
+-rw-r--r--   0 root         (0) root         (0)     1142 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/static.c
+-rw-r--r--   0 root         (0) root         (0)    20977 2021-06-05 17:55:07.000000 kiwipiepy-0.9.3/mimalloc/src/stats.c
+-rw-r--r--   0 root         (0) root         (0)       38 2021-06-05 17:55:08.682192 kiwipiepy-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2502 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.678192 kiwipiepy-0.9.3/src/
+-rw-r--r--   0 root         (0) root         (0)    27898 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/src/KiwiPy.cpp
+-rw-r--r--   0 root         (0) root         (0)    16734 2021-06-05 17:54:48.000000 kiwipiepy-0.9.3/src/PyDoc.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-05 17:55:08.682192 kiwipiepy-0.9.3/src/core/
+-rw-r--r--   0 root         (0) root         (0)     4825 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/BakedMap.hpp
+-rw-r--r--   0 root         (0) root         (0)     2101 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KFeatureTestor.cpp
+-rw-r--r--   0 root         (0) root         (0)      584 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KFeatureTestor.h
+-rw-r--r--   0 root         (0) root         (0)     7031 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KForm.cpp
+-rw-r--r--   0 root         (0) root         (0)     3089 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KForm.h
+-rw-r--r--   0 root         (0) root         (0)    15961 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KModelMgr.cpp
+-rw-r--r--   0 root         (0) root         (0)     2398 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KModelMgr.h
+-rw-r--r--   0 root         (0) root         (0)     7556 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KNLangModel.cpp
+-rw-r--r--   0 root         (0) root         (0)     6912 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KNLangModel.h
+-rw-r--r--   0 root         (0) root         (0)    11136 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KTrie.cpp
+-rw-r--r--   0 root         (0) root         (0)     1457 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KTrie.h
+-rw-r--r--   0 root         (0) root         (0)    14449 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KWordDetector.cpp
+-rw-r--r--   0 root         (0) root         (0)     7787 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KWordDetector.h
+-rw-r--r--   0 root         (0) root         (0)    24520 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/Kiwi.cpp
+-rw-r--r--   0 root         (0) root         (0)     4026 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/Kiwi.h
+-rw-r--r--   0 root         (0) root         (0)     2133 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/KiwiHeader.h
+-rw-r--r--   0 root         (0) root         (0)     4178 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/PatternMatcher.cpp
+-rw-r--r--   0 root         (0) root         (0)      782 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/PatternMatcher.h
+-rw-r--r--   0 root         (0) root         (0)     2840 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/ThreadPool.h
+-rw-r--r--   0 root         (0) root         (0)     3505 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/Trie.hpp
+-rw-r--r--   0 root         (0) root         (0)     5857 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/Utils.cpp
+-rw-r--r--   0 root         (0) root         (0)     3072 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/Utils.h
+-rw-r--r--   0 root         (0) root         (0)      548 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/logPoisson.h
+-rw-r--r--   0 root         (0) root         (0)    12843 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/pattern.hpp
+-rw-r--r--   0 root         (0) root         (0)     2845 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/serializer.cpp
+-rw-r--r--   0 root         (0) root         (0)     5189 2021-06-05 17:55:04.000000 kiwipiepy-0.9.3/src/core/serializer.hpp
```

### Comparing `kiwipiepy-0.9.2/LICENSE.txt` & `kiwipiepy-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/PKG-INFO` & `kiwipiepy-0.9.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: kiwipiepy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Kiwi, the Korean Tokenizer for Python
 Home-page: https://github.com/bab2min/kiwipiepy
 Author: bab2min
 Author-email: bab2min@gmail.com
 License: LGPL v3 License
-Description: kiwipiepy
-        ----------
-        kiwipiepy is a python version package of Kiwi(Korean Intelligent Word Identifier) which is a morphological analyzer for Korean.
-        
-        https://github.com/bab2min/kiwipiepy 
 Keywords: Korean morphological analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
+License-File: LICENSE.txt
+
+kiwipiepy
+----------
+kiwipiepy is a python version package of Kiwi(Korean Intelligent Word Identifier) which is a morphological analyzer for Korean.
+
+https://github.com/bab2min/kiwipiepy 
+
```

### Comparing `kiwipiepy-0.9.2/README.md` & `kiwipiepy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/kiwipiepy/__init__.py` & `kiwipiepy-0.9.3/kiwipiepy/__init__.py`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/kiwipiepy/documentation.rst` & `kiwipiepy-0.9.3/kiwipiepy/documentation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Kiwipiepy란?
 ============
 Kiwipiepy는 한국어 형태소 분석기인 Kiwi(Korean Intelligent Word Identifier)의 Python 모듈입니다. 
 C++로 작성되었고 다른 패키지에 의존성이 없으므로 C++ 컴파일이 가능한 환경이라면 어디에서나 Kiwipiepy를 사용 가능합니다.
 
-현재 Kiwipiepy의 최신 버전은 0.9.2입니다.
 
 .. image:: https://badge.fury.io/py/kiwipiepy.svg
 
 시작하기
 --------
 pip를 이용해 쉽게 설치할 수 있습니다. (https://pypi.org/project/kiwipiepy/)
 
@@ -312,15 +311,18 @@
 <tr><td>W_MENTION</td><td>멘션(@abcd)<sup>*</sup></td></tr>
 </table>
 
 <sup>*</sup> 세종 품사 태그와 다른 독자적인 태그입니다.
 
 역사
 ----
-* 0.9.2 (2021-01-20)
+* 0.9.3 (2021-06-06)
+    * Linux 환경에서 특정 단어가 포함된 텍스트를 분석할 때 크래시가 발생하던 문제를 수정했습니다.
+    
+* 0.9.2 (2020-12-03)
     * 0.9.1에서 제대로 수정되지 않은 mimalloc 충돌 문제를 수정했습니다.
     * 형태소 분석 모델을 분리하여 패키징하는 기능을 추가했습니다. 용량 문제로 업로드 못했던 대용량 모델을 차차 추가해나갈 예정입니다.
 
 * 0.9.1 (2020-12-03)
     * kiwipiepy가 다른 Python 패키지와 함께 사용될 경우 종종 mimalloc이 충돌하는 문제를 해결했습니다.
 
 * 0.9.0 (2020-11-26)
```

### Comparing `kiwipiepy-0.9.2/kiwipiepy.egg-info/PKG-INFO` & `kiwipiepy-0.9.3/kiwipiepy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: kiwipiepy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Kiwi, the Korean Tokenizer for Python
 Home-page: https://github.com/bab2min/kiwipiepy
 Author: bab2min
 Author-email: bab2min@gmail.com
 License: LGPL v3 License
-Description: kiwipiepy
-        ----------
-        kiwipiepy is a python version package of Kiwi(Korean Intelligent Word Identifier) which is a morphological analyzer for Korean.
-        
-        https://github.com/bab2min/kiwipiepy 
 Keywords: Korean morphological analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
+License-File: LICENSE.txt
+
+kiwipiepy
+----------
+kiwipiepy is a python version package of Kiwi(Korean Intelligent Word Identifier) which is a morphological analyzer for Korean.
+
+https://github.com/bab2min/kiwipiepy 
+
```

### Comparing `kiwipiepy-0.9.2/kiwipiepy.egg-info/SOURCES.txt` & `kiwipiepy-0.9.3/kiwipiepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/include/mimalloc-atomic.h` & `kiwipiepy-0.9.3/mimalloc/include/mimalloc-atomic.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/include/mimalloc-internal.h` & `kiwipiepy-0.9.3/mimalloc/include/mimalloc-internal.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/include/mimalloc-new-delete.h` & `kiwipiepy-0.9.3/mimalloc/include/mimalloc-new-delete.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/include/mimalloc-override.h` & `kiwipiepy-0.9.3/mimalloc/include/mimalloc-override.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/include/mimalloc-types.h` & `kiwipiepy-0.9.3/mimalloc/include/mimalloc-types.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/include/mimalloc.h` & `kiwipiepy-0.9.3/mimalloc/include/mimalloc.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/alloc-aligned.c` & `kiwipiepy-0.9.3/mimalloc/src/alloc-aligned.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/alloc-override-osx.c` & `kiwipiepy-0.9.3/mimalloc/src/alloc-override-osx.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/alloc-override.c` & `kiwipiepy-0.9.3/mimalloc/src/alloc-override.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/alloc-posix.c` & `kiwipiepy-0.9.3/mimalloc/src/alloc-posix.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/alloc.c` & `kiwipiepy-0.9.3/mimalloc/src/alloc.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/arena.c` & `kiwipiepy-0.9.3/mimalloc/src/arena.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/bitmap.inc.c` & `kiwipiepy-0.9.3/mimalloc/src/bitmap.inc.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/heap.c` & `kiwipiepy-0.9.3/mimalloc/src/heap.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/init.c` & `kiwipiepy-0.9.3/mimalloc/src/init.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/options.c` & `kiwipiepy-0.9.3/mimalloc/src/options.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/os.c` & `kiwipiepy-0.9.3/mimalloc/src/os.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/page-queue.c` & `kiwipiepy-0.9.3/mimalloc/src/page-queue.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/page.c` & `kiwipiepy-0.9.3/mimalloc/src/page.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/random.c` & `kiwipiepy-0.9.3/mimalloc/src/random.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/region.c` & `kiwipiepy-0.9.3/mimalloc/src/region.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/segment.c` & `kiwipiepy-0.9.3/mimalloc/src/segment.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/static.c` & `kiwipiepy-0.9.3/mimalloc/src/static.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/mimalloc/src/stats.c` & `kiwipiepy-0.9.3/mimalloc/src/stats.c`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/setup.py` & `kiwipiepy-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/KiwiPy.cpp` & `kiwipiepy-0.9.3/src/KiwiPy.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/PyDoc.h` & `kiwipiepy-0.9.3/src/PyDoc.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/BakedMap.hpp` & `kiwipiepy-0.9.3/src/core/BakedMap.hpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KFeatureTestor.cpp` & `kiwipiepy-0.9.3/src/core/KFeatureTestor.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KFeatureTestor.h` & `kiwipiepy-0.9.3/src/core/KFeatureTestor.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KForm.cpp` & `kiwipiepy-0.9.3/src/core/KForm.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KForm.h` & `kiwipiepy-0.9.3/src/core/KForm.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KModelMgr.cpp` & `kiwipiepy-0.9.3/src/core/KModelMgr.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,17 @@
 	trieRoot.reserve(baseTrieSize + extraTrieSize);
 	trieRoot.resize((size_t)KPOSTag::DEFAULT_TAG_SIZE + 1); // preserve places for root node + default tag morphemes
 	for (size_t i = 1; i <= (size_t)KPOSTag::DEFAULT_TAG_SIZE; ++i)
 	{
 		trieRoot[i].val = &forms[i - 1];
 	}
 
-	for (size_t i = (size_t)KPOSTag::DEFAULT_TAG_SIZE; i < forms.size(); ++i)
+	forms.emplace_back(); // add sentry for last value
+
+	for (size_t i = (size_t)KPOSTag::DEFAULT_TAG_SIZE; i < forms.size() - 1; ++i)
 	{
 		auto& f = forms[i];
 		if (f.candidate.empty()) continue;
 		size_t realSize = f.form.size();
 		if (trieRoot.capacity() < trieRoot.size() + realSize)
 		{
 			trieRoot.reserve(max(trieRoot.size() + realSize, trieRoot.capacity() + trieRoot.capacity() / 4));
```

#### encoding

```diff
@@ -1 +1 @@
-iso-8859-1
+utf-8
```

### Comparing `kiwipiepy-0.9.2/src/core/KModelMgr.h` & `kiwipiepy-0.9.3/src/core/KModelMgr.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KNLangModel.cpp` & `kiwipiepy-0.9.3/src/core/KNLangModel.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KNLangModel.h` & `kiwipiepy-0.9.3/src/core/KNLangModel.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KTrie.cpp` & `kiwipiepy-0.9.3/src/core/KTrie.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KTrie.h` & `kiwipiepy-0.9.3/src/core/KTrie.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KWordDetector.cpp` & `kiwipiepy-0.9.3/src/core/KWordDetector.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KWordDetector.h` & `kiwipiepy-0.9.3/src/core/KWordDetector.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/Kiwi.cpp` & `kiwipiepy-0.9.3/src/core/Kiwi.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -877,15 +877,15 @@
 void Kiwi::clearCache()
 {
 
 }
 
 const char* Kiwi::getVersion()
 {
-	return "0.9.1";
+	return "0.9.3";
 }
 
 std::u16string Kiwi::toU16(const std::string & str)
 {
 	return utf8_to_utf16(str);
 }
```

### Comparing `kiwipiepy-0.9.2/src/core/Kiwi.h` & `kiwipiepy-0.9.3/src/core/Kiwi.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/KiwiHeader.h` & `kiwipiepy-0.9.3/src/core/KiwiHeader.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/PatternMatcher.cpp` & `kiwipiepy-0.9.3/src/core/PatternMatcher.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/PatternMatcher.h` & `kiwipiepy-0.9.3/src/core/PatternMatcher.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/ThreadPool.h` & `kiwipiepy-0.9.3/src/core/ThreadPool.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/Trie.hpp` & `kiwipiepy-0.9.3/src/core/Trie.hpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/Utils.cpp` & `kiwipiepy-0.9.3/src/core/Utils.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/Utils.h` & `kiwipiepy-0.9.3/src/core/Utils.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/logPoisson.h` & `kiwipiepy-0.9.3/src/core/logPoisson.h`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/pattern.hpp` & `kiwipiepy-0.9.3/src/core/pattern.hpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/serializer.cpp` & `kiwipiepy-0.9.3/src/core/serializer.cpp`

 * *Files identical despite different names*

### Comparing `kiwipiepy-0.9.2/src/core/serializer.hpp` & `kiwipiepy-0.9.3/src/core/serializer.hpp`

 * *Files identical despite different names*

