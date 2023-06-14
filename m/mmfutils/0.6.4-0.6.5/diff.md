# Comparing `tmp/mmfutils-0.6.4.tar.gz` & `tmp/mmfutils-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmfutils-0.6.4.tar", max compression
+gzip compressed data, was "mmfutils-0.6.5.tar", max compression
```

## Comparing `mmfutils-0.6.4.tar` & `mmfutils-0.6.5.tar`

### file list

```diff
@@ -1,41 +1,178 @@
--rw-r--r--   0        0        0     1504 2023-03-14 02:37:07.428202 mmfutils-0.6.4/LICENSE.txt
--rw-r--r--   0        0        0      448 2023-03-14 02:37:07.430312 mmfutils-0.6.4/description.md
--rw-r--r--   0        0        0     5146 2023-05-25 09:52:09.462298 mmfutils-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     1071 2023-03-23 10:20:06.591896 mmfutils-0.6.4/src/mmfutils/__init__.py
--rw-r--r--   0        0        0    16856 2023-03-23 10:20:06.592165 mmfutils-0.6.4/src/mmfutils/containers.py
--rw-r--r--   0        0        0    25514 2023-03-23 10:20:06.592490 mmfutils-0.6.4/src/mmfutils/contexts.py
--rw-r--r--   0        0        0     3616 2023-03-14 02:37:07.443437 mmfutils-0.6.4/src/mmfutils/debugging.py
--rw-r--r--   0        0        0     7062 2023-03-14 02:37:07.443639 mmfutils-0.6.4/src/mmfutils/interface.py
--rw-r--r--   0        0        0        0 2023-03-14 02:37:07.443792 mmfutils-0.6.4/src/mmfutils/math/__init__.py
--rw-r--r--   0        0        0      242 2023-03-14 02:37:07.444002 mmfutils-0.6.4/src/mmfutils/math/bases/__init__.py
--rw-r--r--   0        0        0    51198 2023-03-23 10:20:06.592908 mmfutils-0.6.4/src/mmfutils/math/bases/bases.py
--rw-r--r--   0        0        0     5861 2023-03-14 02:37:07.444568 mmfutils-0.6.4/src/mmfutils/math/bases/interfaces.py
--rw-r--r--   0        0        0     3646 2023-05-25 09:45:38.840475 mmfutils-0.6.4/src/mmfutils/math/bases/utils.py
--rw-r--r--   0        0        0    14266 2023-03-14 02:37:07.445487 mmfutils-0.6.4/src/mmfutils/math/bessel.py
--rw-r--r--   0        0        0     7476 2023-03-14 02:37:07.445736 mmfutils-0.6.4/src/mmfutils/math/differentiate.py
--rw-r--r--   0        0        0    20573 2023-03-14 02:37:07.446021 mmfutils-0.6.4/src/mmfutils/math/integrate/__init__.py
--rw-r--r--   0        0        0   918653 2023-03-14 02:37:07.449156 mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.c
--rw-r--r--   0        0        0      918 2023-03-14 02:37:07.449431 mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.pyx
--rw-r--r--   0        0        0      657 2023-03-14 02:37:07.450074 mmfutils-0.6.4/src/mmfutils/math/linalg.py
--rw-r--r--   0        0        0     1916 2023-03-14 02:37:07.450271 mmfutils-0.6.4/src/mmfutils/math/special.py
--rw-r--r--   0        0        0     1624 2023-03-14 02:37:07.451256 mmfutils-0.6.4/src/mmfutils/math/wigner.py
--rw-r--r--   0        0        0     2159 2023-03-14 02:37:07.451445 mmfutils-0.6.4/src/mmfutils/optimize.py
--rw-r--r--   0        0        0     8944 2023-03-14 02:37:07.451659 mmfutils-0.6.4/src/mmfutils/parallel.py
--rw-r--r--   0        0        0      177 2023-03-14 02:37:07.451870 mmfutils-0.6.4/src/mmfutils/performance/__init__.py
--rw-r--r--   0        0        0     4282 2023-03-14 02:37:07.452102 mmfutils-0.6.4/src/mmfutils/performance/blas.py
--rw-r--r--   0        0        0     9777 2023-03-14 02:37:07.452369 mmfutils-0.6.4/src/mmfutils/performance/fft.py
--rw-r--r--   0        0        0      976 2023-03-14 02:37:07.452583 mmfutils-0.6.4/src/mmfutils/performance/numexpr.py
--rw-r--r--   0        0        0     1053 2023-03-14 02:37:07.452796 mmfutils-0.6.4/src/mmfutils/performance/threads.py
--rw-r--r--   0        0        0      421 2023-03-14 02:37:07.453039 mmfutils-0.6.4/src/mmfutils/plot/__init__.py
--rw-r--r--   0        0        0     6957 2023-05-25 09:45:38.840755 mmfutils-0.6.4/src/mmfutils/plot/animation.py
--rw-r--r--   0        0        0    37324 2023-03-14 02:37:07.453620 mmfutils-0.6.4/src/mmfutils/plot/cmaps.py
--rw-r--r--   0        0        0     6925 2023-03-23 10:20:06.593151 mmfutils-0.6.4/src/mmfutils/plot/colors.py
--rw-r--r--   0        0        0     4921 2023-03-14 02:37:07.454080 mmfutils-0.6.4/src/mmfutils/plot/contour.py
--rw-r--r--   0        0        0     4431 2023-03-14 02:37:07.454298 mmfutils-0.6.4/src/mmfutils/plot/errors.py
--rw-r--r--   0        0        0     2474 2023-03-27 18:52:24.066912 mmfutils-0.6.4/src/mmfutils/plot/histogram.py
--rw-r--r--   0        0        0    26375 2023-03-14 02:37:07.454584 mmfutils-0.6.4/src/mmfutils/plot/publish.py
--rw-r--r--   0        0        0     1706 2023-03-14 02:37:07.454796 mmfutils-0.6.4/src/mmfutils/plot/rasterize.py
--rw-r--r--   0        0        0        0 2023-03-14 02:37:07.455018 mmfutils-0.6.4/src/mmfutils/solve/__init__.py
--rw-r--r--   0        0        0    28204 2023-03-23 10:20:06.593467 mmfutils-0.6.4/src/mmfutils/solve/broyden.py
--rw-r--r--   0        0        0     1302 2023-03-14 02:37:07.456161 mmfutils-0.6.4/src/mmfutils/testing.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 mmfutils-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1504 2022-02-01 20:15:10.000000 mmfutils-0.6.5/LICENSE
+-rw-r--r--   0        0        0     1504 2022-08-11 21:12:19.647920 mmfutils-0.6.5/LICENSE.txt
+-rw-r--r--   0        0        0      448 2022-02-03 17:07:03.000000 mmfutils-0.6.5/description.md
+-rw-r--r--   0        0        0     5557 2023-05-30 08:52:09.903519 mmfutils-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1071 2022-12-23 03:02:16.395658 mmfutils-0.6.5/src/mmfutils/__init__.py
+-rw-r--r--   0        0        0    16856 2022-12-23 03:32:04.362045 mmfutils-0.6.5/src/mmfutils/containers.py
+-rw-r--r--   0        0        0    25514 2022-12-26 20:44:28.096310 mmfutils-0.6.5/src/mmfutils/contexts.py
+-rw-r--r--   0        0        0     3616 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/debugging.py
+-rw-r--r--   0        0        0     7062 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/interface.py
+-rw-r--r--   0        0        0        0 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/__init__.py
+-rw-r--r--   0        0        0      157 2022-12-23 05:28:59.610913 mmfutils-0.6.5/src/mmfutils/math/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      173 2023-05-25 08:21:06.721234 mmfutils-0.6.5/src/mmfutils/math/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      151 2022-12-22 09:31:48.784327 mmfutils-0.6.5/src/mmfutils/math/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      155 2022-12-22 09:22:10.706488 mmfutils-0.6.5/src/mmfutils/math/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      155 2022-12-22 09:14:44.924318 mmfutils-0.6.5/src/mmfutils/math/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    12947 2022-12-23 05:28:59.615252 mmfutils-0.6.5/src/mmfutils/math/__pycache__/bessel.cpython-310.pyc
+-rw-r--r--   0        0        0    19380 2023-05-25 08:21:06.726495 mmfutils-0.6.5/src/mmfutils/math/__pycache__/bessel.cpython-311.pyc
+-rw-r--r--   0        0        0    12818 2022-12-22 09:31:48.788430 mmfutils-0.6.5/src/mmfutils/math/__pycache__/bessel.cpython-37.pyc
+-rw-r--r--   0        0        0    12791 2022-12-22 09:22:10.710350 mmfutils-0.6.5/src/mmfutils/math/__pycache__/bessel.cpython-38.pyc
+-rw-r--r--   0        0        0    12771 2022-12-22 09:14:44.928553 mmfutils-0.6.5/src/mmfutils/math/__pycache__/bessel.cpython-39.pyc
+-rw-r--r--   0        0        0     8146 2022-12-23 05:29:09.322556 mmfutils-0.6.5/src/mmfutils/math/__pycache__/differentiate.cpython-310.pyc
+-rw-r--r--   0        0        0    10857 2023-05-25 08:21:15.385099 mmfutils-0.6.5/src/mmfutils/math/__pycache__/differentiate.cpython-311.pyc
+-rw-r--r--   0        0        0     8145 2022-12-22 09:31:56.235089 mmfutils-0.6.5/src/mmfutils/math/__pycache__/differentiate.cpython-37.pyc
+-rw-r--r--   0        0        0     8136 2022-12-22 09:22:19.118339 mmfutils-0.6.5/src/mmfutils/math/__pycache__/differentiate.cpython-38.pyc
+-rw-r--r--   0        0        0     8144 2022-12-22 09:14:44.995859 mmfutils-0.6.5/src/mmfutils/math/__pycache__/differentiate.cpython-39.pyc
+-rw-r--r--   0        0        0     1001 2022-12-23 05:29:15.405512 mmfutils-0.6.5/src/mmfutils/math/__pycache__/linalg.cpython-310.pyc
+-rw-r--r--   0        0        0     1471 2023-05-25 08:21:19.987096 mmfutils-0.6.5/src/mmfutils/math/__pycache__/linalg.cpython-311.pyc
+-rw-r--r--   0        0        0      991 2022-12-22 09:32:05.719485 mmfutils-0.6.5/src/mmfutils/math/__pycache__/linalg.cpython-37.pyc
+-rw-r--r--   0        0        0     1001 2022-12-22 09:22:29.313309 mmfutils-0.6.5/src/mmfutils/math/__pycache__/linalg.cpython-38.pyc
+-rw-r--r--   0        0        0      997 2022-12-22 09:14:45.316791 mmfutils-0.6.5/src/mmfutils/math/__pycache__/linalg.cpython-39.pyc
+-rw-r--r--   0        0        0     2156 2022-12-23 05:29:15.406677 mmfutils-0.6.5/src/mmfutils/math/__pycache__/special.cpython-310.pyc
+-rw-r--r--   0        0        0     3273 2023-05-25 08:21:19.989268 mmfutils-0.6.5/src/mmfutils/math/__pycache__/special.cpython-311.pyc
+-rw-r--r--   0        0        0     2171 2022-12-22 09:32:05.720703 mmfutils-0.6.5/src/mmfutils/math/__pycache__/special.cpython-37.pyc
+-rw-r--r--   0        0        0     2164 2022-12-22 09:22:29.314552 mmfutils-0.6.5/src/mmfutils/math/__pycache__/special.cpython-38.pyc
+-rw-r--r--   0        0        0     2164 2022-12-22 09:14:45.317942 mmfutils-0.6.5/src/mmfutils/math/__pycache__/special.cpython-39.pyc
+-rw-r--r--   0        0        0     1701 2022-12-23 05:29:15.407862 mmfutils-0.6.5/src/mmfutils/math/__pycache__/wigner.cpython-310.pyc
+-rw-r--r--   0        0        0     2622 2023-05-25 08:21:19.991392 mmfutils-0.6.5/src/mmfutils/math/__pycache__/wigner.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2022-12-22 09:32:05.721939 mmfutils-0.6.5/src/mmfutils/math/__pycache__/wigner.cpython-37.pyc
+-rw-r--r--   0        0        0     1699 2022-12-22 09:22:29.315684 mmfutils-0.6.5/src/mmfutils/math/__pycache__/wigner.cpython-38.pyc
+-rw-r--r--   0        0        0     1699 2022-12-22 09:14:45.319069 mmfutils-0.6.5/src/mmfutils/math/__pycache__/wigner.cpython-39.pyc
+-rw-r--r--   0        0        0      242 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/bases/__init__.py
+-rw-r--r--   0        0        0      323 2022-12-23 05:29:18.223414 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      418 2023-05-25 08:21:21.974403 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      356 2022-12-22 09:32:07.936312 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      362 2022-12-22 09:22:31.639635 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      321 2022-12-22 09:14:45.346009 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    36053 2023-05-08 03:37:37.128250 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/bases.cpython-310.pyc
+-rw-r--r--   0        0        0    58530 2023-05-30 08:00:29.565807 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/bases.cpython-311.pyc
+-rw-r--r--   0        0        0    36461 2023-05-16 06:31:15.599513 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/bases.cpython-37.pyc
+-rw-r--r--   0        0        0    36436 2023-05-16 06:33:34.723451 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/bases.cpython-38.pyc
+-rw-r--r--   0        0        0    36329 2023-05-16 06:35:56.870572 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/bases.cpython-39.pyc
+-rw-r--r--   0        0        0     7806 2022-12-23 05:29:18.228912 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/interfaces.cpython-310.pyc
+-rw-r--r--   0        0        0     9312 2023-05-25 08:21:21.979989 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/interfaces.cpython-311.pyc
+-rw-r--r--   0        0        0     7747 2022-12-22 09:32:07.942667 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/interfaces.cpython-37.pyc
+-rw-r--r--   0        0        0     7833 2022-12-22 09:22:31.647392 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/interfaces.cpython-38.pyc
+-rw-r--r--   0        0        0     7836 2022-12-22 09:14:45.351362 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/interfaces.cpython-39.pyc
+-rw-r--r--   0        0        0     3992 2023-05-25 09:46:30.802682 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     5614 2023-05-25 09:47:43.058509 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4127 2023-05-25 10:08:24.608664 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0     4052 2023-05-25 10:09:32.681103 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-05-25 09:45:22.204263 mmfutils-0.6.5/src/mmfutils/math/bases/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    51199 2023-05-30 08:00:25.698228 mmfutils-0.6.5/src/mmfutils/math/bases/bases.py
+-rw-r--r--   0        0        0    51691 2022-09-02 21:32:00.358613 mmfutils-0.6.5/src/mmfutils/math/bases/bases.py.orig
+-rw-r--r--   0        0        0     5861 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/bases/interfaces.py
+-rw-r--r--   0        0        0     3646 2023-05-25 09:44:38.336805 mmfutils-0.6.5/src/mmfutils/math/bases/utils.py
+-rw-r--r--   0        0        0    14266 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/bessel.py
+-rw-r--r--   0        0        0     7476 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/differentiate.py
+-rw-r--r--   0        0        0    20573 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/integrate/__init__.py
+-rw-r--r--   0        0        0    18566 2022-12-23 05:29:09.325001 mmfutils-0.6.5/src/mmfutils/math/integrate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    27067 2023-05-25 08:21:15.389004 mmfutils-0.6.5/src/mmfutils/math/integrate/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    18533 2022-12-22 09:31:56.239365 mmfutils-0.6.5/src/mmfutils/math/integrate/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0    18574 2022-12-22 09:22:19.121387 mmfutils-0.6.5/src/mmfutils/math/integrate/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    18496 2022-12-22 09:14:44.998159 mmfutils-0.6.5/src/mmfutils/math/integrate/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0   918653 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/integrate/_ssum_cython.c
+-rw-r--r--   0        0        0      918 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/integrate/_ssum_cython.pyx
+-rw-r--r--   0        0        0      657 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/linalg.py
+-rw-r--r--   0        0        0     1916 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/special.py
+-rw-r--r--   0        0        0     1624 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/math/wigner.py
+-rw-r--r--   0        0        0     2159 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/optimize.py
+-rw-r--r--   0        0        0     8944 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/parallel.py
+-rw-r--r--   0        0        0      177 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/performance/__init__.py
+-rw-r--r--   0        0        0      346 2022-12-23 05:29:15.408249 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-05-25 08:21:19.992076 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      340 2022-12-22 09:32:05.722339 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      344 2022-12-22 09:22:29.316212 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      344 2022-12-22 09:14:45.319495 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3663 2022-12-23 05:29:18.278492 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/blas.cpython-310.pyc
+-rw-r--r--   0        0        0     6459 2023-05-25 08:21:22.058946 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/blas.cpython-311.pyc
+-rw-r--r--   0        0        0     4441 2022-12-22 09:32:07.960830 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/blas.cpython-37.pyc
+-rw-r--r--   0        0        0     3941 2022-12-22 09:22:31.665491 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/blas.cpython-38.pyc
+-rw-r--r--   0        0        0     3915 2022-12-22 09:14:45.366159 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/blas.cpython-39.pyc
+-rw-r--r--   0        0        0     7311 2022-12-23 05:29:15.409551 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/fft.cpython-310.pyc
+-rw-r--r--   0        0        0    19044 2023-05-30 08:34:46.408896 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/fft.cpython-311.pyc
+-rw-r--r--   0        0        0     7795 2022-12-22 09:32:05.723662 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/fft.cpython-37.pyc
+-rw-r--r--   0        0        0     7628 2022-12-22 09:22:29.317537 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/fft.cpython-38.pyc
+-rw-r--r--   0        0        0     7641 2022-12-22 09:14:45.320679 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/fft.cpython-39.pyc
+-rw-r--r--   0        0        0      867 2022-12-23 05:29:18.281064 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/numexpr.cpython-310.pyc
+-rw-r--r--   0        0        0     1311 2023-05-25 08:21:22.061489 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/numexpr.cpython-311.pyc
+-rw-r--r--   0        0        0      849 2022-12-22 09:32:07.963878 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/numexpr.cpython-37.pyc
+-rw-r--r--   0        0        0      857 2022-12-22 09:22:31.668423 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/numexpr.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-12-22 09:14:45.368844 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/numexpr.cpython-39.pyc
+-rw-r--r--   0        0        0     1051 2022-12-23 05:29:15.410007 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/threads.cpython-310.pyc
+-rw-r--r--   0        0        0     1556 2023-05-25 08:21:19.995491 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/threads.cpython-311.pyc
+-rw-r--r--   0        0        0     1035 2022-12-22 09:32:05.724107 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/threads.cpython-37.pyc
+-rw-r--r--   0        0        0     1039 2022-12-22 09:22:29.317960 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/threads.cpython-38.pyc
+-rw-r--r--   0        0        0     1035 2022-12-22 09:14:45.321132 mmfutils-0.6.5/src/mmfutils/performance/__pycache__/threads.cpython-39.pyc
+-rw-r--r--   0        0        0     4282 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/performance/blas.py
+-rw-r--r--   0        0        0    14421 2023-05-30 08:34:43.820331 mmfutils-0.6.5/src/mmfutils/performance/fft.py
+-rw-r--r--   0        0        0      976 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/performance/numexpr.py
+-rw-r--r--   0        0        0     1053 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/performance/threads.py
+-rw-r--r--   0        0        0      421 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/plot/__init__.py
+-rw-r--r--   0        0        0      555 2022-12-23 05:29:19.200778 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      684 2023-05-25 08:21:22.665988 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      577 2022-12-22 09:32:08.122299 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      583 2022-12-22 09:22:31.991272 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      553 2022-12-22 09:14:45.667220 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5151 2023-05-25 09:46:31.113646 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/animation.cpython-310.pyc
+-rw-r--r--   0        0        0     7932 2023-05-25 09:47:43.384988 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/animation.cpython-311.pyc
+-rw-r--r--   0        0        0     5085 2023-05-25 10:08:24.646728 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/animation.cpython-37.pyc
+-rw-r--r--   0        0        0     5104 2023-05-25 10:09:32.992642 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/animation.cpython-38.pyc
+-rw-r--r--   0        0        0     5130 2023-05-25 09:45:22.504830 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/animation.cpython-39.pyc
+-rw-r--r--   0        0        0    46086 2022-12-23 05:29:21.407072 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/cmaps.cpython-310.pyc
+-rw-r--r--   0        0        0    59317 2023-05-25 08:21:23.809490 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/cmaps.cpython-311.pyc
+-rw-r--r--   0        0        0    43943 2022-12-22 09:32:10.470157 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/cmaps.cpython-37.pyc
+-rw-r--r--   0        0        0    43983 2022-12-22 09:22:34.368435 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/cmaps.cpython-38.pyc
+-rw-r--r--   0        0        0    39914 2022-12-22 09:14:46.283857 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/cmaps.cpython-39.pyc
+-rw-r--r--   0        0        0     5951 2022-12-23 05:29:21.398566 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/colors.cpython-310.pyc
+-rw-r--r--   0        0        0     9490 2023-05-25 08:21:23.801918 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/colors.cpython-311.pyc
+-rw-r--r--   0        0        0     5906 2022-12-23 04:14:52.711923 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/colors.cpython-37.pyc
+-rw-r--r--   0        0        0     5941 2022-12-23 04:15:59.416259 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/colors.cpython-38.pyc
+-rw-r--r--   0        0        0     6011 2022-12-23 04:17:05.338447 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/colors.cpython-39.pyc
+-rw-r--r--   0        0        0     4757 2022-12-23 05:29:21.414554 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/contour.cpython-310.pyc
+-rw-r--r--   0        0        0     9318 2023-05-25 08:21:23.816282 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/contour.cpython-311.pyc
+-rw-r--r--   0        0        0     4719 2022-12-22 09:32:10.477009 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/contour.cpython-37.pyc
+-rw-r--r--   0        0        0     4763 2022-12-22 09:22:34.374493 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/contour.cpython-38.pyc
+-rw-r--r--   0        0        0     4754 2022-12-22 09:14:46.324006 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/contour.cpython-39.pyc
+-rw-r--r--   0        0        0     3030 2022-12-23 05:29:22.422448 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/errors.cpython-310.pyc
+-rw-r--r--   0        0        0     6404 2023-05-25 08:21:24.714303 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     2948 2022-12-22 09:32:11.504747 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/errors.cpython-37.pyc
+-rw-r--r--   0        0        0     2959 2022-12-22 09:22:35.147528 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/errors.cpython-38.pyc
+-rw-r--r--   0        0        0     2990 2022-12-22 09:14:46.340944 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0    20263 2022-12-23 05:29:25.349177 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/publish.cpython-310.pyc
+-rw-r--r--   0        0        0    31881 2023-05-25 08:21:27.966444 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0        0        0    20166 2022-12-22 09:32:13.271775 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/publish.cpython-37.pyc
+-rw-r--r--   0        0        0    20214 2022-12-22 09:22:37.948690 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/publish.cpython-38.pyc
+-rw-r--r--   0        0        0    20228 2022-12-22 09:14:46.473758 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/publish.cpython-39.pyc
+-rw-r--r--   0        0        0     2187 2022-12-23 05:29:22.419547 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/rasterize.cpython-310.pyc
+-rw-r--r--   0        0        0     3230 2023-05-25 08:21:24.707452 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/rasterize.cpython-311.pyc
+-rw-r--r--   0        0        0     2147 2022-12-22 09:32:11.503116 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/rasterize.cpython-37.pyc
+-rw-r--r--   0        0        0     2173 2022-12-22 09:22:35.142076 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/rasterize.cpython-38.pyc
+-rw-r--r--   0        0        0     2181 2022-12-22 09:14:46.335118 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/rasterize.cpython-39.pyc
+-rw-r--r--   0        0        0      182 2022-12-23 05:29:25.353266 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/sparkline.cpython-310.pyc
+-rw-r--r--   0        0        0      208 2023-05-25 08:21:27.971562 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/sparkline.cpython-311.pyc
+-rw-r--r--   0        0        0      176 2022-12-22 09:32:13.276909 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/sparkline.cpython-37.pyc
+-rw-r--r--   0        0        0      180 2022-12-22 09:22:37.952144 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/sparkline.cpython-38.pyc
+-rw-r--r--   0        0        0      180 2022-12-22 09:14:46.477746 mmfutils-0.6.5/src/mmfutils/plot/__pycache__/sparkline.cpython-39.pyc
+-rw-r--r--   0        0        0     6957 2023-05-25 09:44:38.337096 mmfutils-0.6.5/src/mmfutils/plot/animation.py
+-rw-r--r--   0        0        0    37324 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/plot/cmaps.py
+-rw-r--r--   0        0        0     6925 2022-12-23 04:14:39.493015 mmfutils-0.6.5/src/mmfutils/plot/colors.py
+-rw-r--r--   0        0        0     4921 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/plot/contour.py
+-rw-r--r--   0        0        0     4431 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/plot/errors.py
+-rw-r--r--   0        0        0    26375 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/plot/publish.py
+-rw-r--r--   0        0        0     1706 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/plot/rasterize.py
+-rw-r--r--   0        0        0       19 2022-02-03 18:03:02.000000 mmfutils-0.6.5/src/mmfutils/plot/sparkline.py
+-rw-r--r--   0        0        0        0 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/solve/__init__.py
+-rw-r--r--   0        0        0      158 2022-12-23 05:29:25.354086 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      174 2023-05-25 08:21:27.972523 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      152 2022-12-22 09:32:13.277814 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0      156 2022-12-22 09:22:37.953184 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      156 2022-12-22 09:14:46.478522 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    25745 2022-12-23 05:29:25.357782 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/broyden.cpython-310.pyc
+-rw-r--r--   0        0        0    40862 2023-05-25 08:21:27.977038 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/broyden.cpython-311.pyc
+-rw-r--r--   0        0        0    25830 2022-12-22 10:15:24.426687 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/broyden.cpython-37.pyc
+-rw-r--r--   0        0        0    25864 2022-12-22 21:47:33.115877 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/broyden.cpython-38.pyc
+-rw-r--r--   0        0        0    25835 2022-12-22 10:15:13.527762 mmfutils-0.6.5/src/mmfutils/solve/__pycache__/broyden.cpython-39.pyc
+-rw-r--r--   0        0        0    28204 2022-12-22 10:14:40.380573 mmfutils-0.6.5/src/mmfutils/solve/broyden.py
+-rw-r--r--   0        0        0     1302 2022-02-03 17:07:03.000000 mmfutils-0.6.5/src/mmfutils/testing.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 mmfutils-0.6.5/PKG-INFO
```

### Comparing `mmfutils-0.6.4/LICENSE.txt` & `mmfutils-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/pyproject.toml` & `mmfutils-0.6.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mmfutils"
-version = "0.6.4"
+version = "0.6.5"
 description = "Small set of utilities: containers and interfaces."
 authors = ["Michael McNeil Forbes <michael.forbes+python@gmail.com>"]
 license = "BSD-3"
 readme = "description.md"
 repository = "https://alum.mit.edu/www/mforbes/hg/forbes-group/mmfutils"
 documentation = "http://mmfutils.readthedocs.org"
 classifiers = [
@@ -30,15 +30,18 @@
 numba = [
     {version = ">=0.56.4", python = "<3.8", optional = true},
     {version = ">=0.57.0", python = ">=3.8", optional = true}
 ]
 numexpr = {version = ">=2.8.1", optional = true}
 persist = {version = ">=3.0", optional = true}
 psutil = {version = ">=5.9.1", optional = true}
-pyFFTW = {version = ">=0.13.0", optional = true}
+pyFFTW = [
+    {version = "==0.13.1", python = ">=3.8", optional = true},
+    {version = "==0.13.0", python = "<3.8", optional = true}
+]
 pytest = {version = ">=7.1.2", optional = true}
 pytest-cov = {version = ">=3.0.0", optional = true}
 #docutils = {version = ">=0.20.1", optional = true}
 docutils = {version = ">=0.18.1", optional = true}
 sphinx-rtd-theme = {version = ">=1.2.1", optional = true}
 sphinxcontrib-zopeext = {version = ">=0.3.2", optional = true}
 uncertainties = {version = ">=3.1.5", optional = true}
@@ -128,22 +131,28 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 ######################################################################
 # PyTest
 [tool.pytest.ini_options]
-testpaths = [ "src/mmfutils", "tests" ]
+# Note: see the discussion in https://github.com/pytest-dev/pytest/issues/2042
+# If your doctests are installed, then you should provide the module here (mmfutils)
+# and add --pyargs to the options below.  Otherwise, you will get ImportMismatchError
+# for the doctests.
+testpaths = [ "mmfutils", "tests" ]
+#testpaths = [ "src/mmfutils", "tests" ]
 markers = [
     # mark test as a benchmark.  (Might be slow, or platform dependent)
     "bench",
     # mark test as slow.
     "slow",
 ]
 addopts = [
+    "--pyargs",
     "-m not bench",
     "--doctest-modules",
     "--cov",
     "--cov-report=html",
     "--cov-fail-under=80",
     "--no-cov-on-fail",
     "--cov-append",
```

### Comparing `mmfutils-0.6.4/src/mmfutils/__init__.py` & `mmfutils-0.6.5/src/mmfutils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/containers.py` & `mmfutils-0.6.5/src/mmfutils/containers.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/contexts.py` & `mmfutils-0.6.5/src/mmfutils/contexts.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/debugging.py` & `mmfutils-0.6.5/src/mmfutils/debugging.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/interface.py` & `mmfutils-0.6.5/src/mmfutils/interface.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/bases/bases.py` & `mmfutils-0.6.5/src/mmfutils/math/bases/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -1070,15 +1070,15 @@
         shape_xyz = n.shape[:-1] + (Ny, Nz)
         rs = np.sqrt(y.ravel()[bcast_y] ** 2 + z[bcast_z] ** 2)
         n_xyz = (abs(self.Psi(np.sqrt(n), (x, rs.ravel()))) ** 2).reshape(shape_xyz)
         n_2D = 2 * np.trapz(n_xyz, z, axis=-1)
         return n_2D
 
 
-'''
+r'''
 Incomplete!
 @implementer(IBasis, IBasisKx)
 class SphericalDVRBasis(ObjectBase, BasisMixin):
     r"""3D Spherical DVR basis.
 
     This represents 3-dimensional problems with spherical symmetry.
```

### Comparing `mmfutils-0.6.4/src/mmfutils/math/bases/interfaces.py` & `mmfutils-0.6.5/src/mmfutils/math/bases/interfaces.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/bases/utils.py` & `mmfutils-0.6.5/src/mmfutils/math/bases/utils.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/bessel.py` & `mmfutils-0.6.5/src/mmfutils/math/bessel.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/differentiate.py` & `mmfutils-0.6.5/src/mmfutils/math/differentiate.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/integrate/__init__.py` & `mmfutils-0.6.5/src/mmfutils/math/integrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.c` & `mmfutils-0.6.5/src/mmfutils/math/integrate/_ssum_cython.c`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/integrate/_ssum_cython.pyx` & `mmfutils-0.6.5/src/mmfutils/math/integrate/_ssum_cython.pyx`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/linalg.py` & `mmfutils-0.6.5/src/mmfutils/math/linalg.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/special.py` & `mmfutils-0.6.5/src/mmfutils/math/special.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/math/wigner.py` & `mmfutils-0.6.5/src/mmfutils/math/wigner.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/optimize.py` & `mmfutils-0.6.5/src/mmfutils/optimize.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/parallel.py` & `mmfutils-0.6.5/src/mmfutils/parallel.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/performance/blas.py` & `mmfutils-0.6.5/src/mmfutils/performance/blas.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/performance/fft.py` & `mmfutils-0.6.5/src/mmfutils/performance/fft.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,24 +16,36 @@
     done
 
 Note: The FFTW library does not work with negative indices for axis.
 Indices should first be normalized by ``inds % len(shape)``.
 """
 import functools
 import itertools
+import timeit
 import warnings
 
 import numpy.fft
 import numpy as np
 
 from .threads import SET_THREAD_HOOKS
 
 del numpy
 
-__all__ = ["fft", "ifft", "fftn", "ifftn", "fftfreq", "resample"]
+__all__ = [
+    "fft",
+    "ifft",
+    "fftn",
+    "ifftn",
+    "get_fft",
+    "get_ifft",
+    "get_fftn",
+    "get_ifftn",
+    "fftfreq",
+    "resample",
+]
 
 
 # Numpy versions with a default axis specified
 def fft_numpy(Phi, axis=-1):
     return np.fft.fft(Phi, axis=axis)
 
 
@@ -248,24 +260,172 @@
             planner_effort=_PLANNER_EFFORT,
             overwrite_input=overwrite_input,
             auto_align_input=auto_align_input,
             auto_contiguous=auto_contiguous,
             avoid_copy=avoid_copy,
         )
 
-    fft = fft_pyfftw
-    ifft = ifft_pyfftw
-    fftn = fftn_pyfftw
-    ifftn = ifftn_pyfftw
 except ImportError:  # pragma: nocover
     warnings.warn("Could not import pyfftw... falling back to numpy")
-    fft = fft_numpy
-    ifft = ifft_numpy
-    fftn = fftn_numpy
-    ifftn = ifftn_numpy
+    get_fft_pyfftw = None
+    get_ifft_pyfftw = None
+    get_fftn_pyfftw = None
+    get_ifft_pyfftw = None
+
+
+def _get_best(ffts, a, repeat=3, number=1):
+    """Measure the performance of the ffts and return the best.
+
+    The first entry should be the fastest (pyfftw), and a warning is raised if it is not.
+    """
+    if len(ffts) == 1:
+        return ffts[0]
+
+    assert len(ffts) == 2
+    assert np.allclose(ffts[0](a), ffts[1](a))
+    times = [
+        min(
+            timeit.repeat(
+                "_fft(a)", number=number, repeat=repeat, globals=dict(_fft=_fft, a=a)
+            )
+        )
+        for _fft in ffts
+    ]
+    ind = np.argmin(times)
+    if ind != 0:
+        msg = [
+            f"Numpy fft {times[0]/times[-1]:.1f}x faster than pyfftw.",
+            f"(dtype={a.dtype}, shape={a.shape})",
+            "Check that it is properly compiled/selected.",
+        ]
+        warnings.warn(" ".join(msg))
+    return ffts[ind]
+
+
+def get_fft(a, n=None, axis=-1, repeat=3, number=1, **kw):
+    """Return the fastest function to compute the fft.
+
+    Arguments
+    ---------
+    repeat, number : int
+        Uses :func:`timeit.repeat` to compare versions (if pyfftw is defined).
+
+    Other arguments are as for :func:`numpy.fft.fft`.
+    """
+    ffts = []
+    if get_fft_pyfftw:
+        ffts.append(get_fft_pyfftw(a=a, n=n, axis=axis, **kw))
+    ffts.append(functools.partial(np.fft.fft, n=n, axis=axis))
+    return _get_best(ffts, a, repeat=3, number=1)
+
+
+def get_ifft(a, n=None, axis=-1, repeat=3, number=1, **kw):
+    """Return the fastest function to compute the ifft.
+
+    Arguments
+    ---------
+    repeat, number : int
+        Uses :func:`timeit.repeat` to compare versions (if pyfftw is defined).
+
+    Other arguments are as for :func:`numpy.fft.ifft`.
+    """
+    ffts = []
+    if get_ifft_pyfftw:
+        ffts.append(get_ifft_pyfftw(a=a, n=n, axis=axis, **kw))
+    ffts.append(functools.partial(np.fft.ifft, n=n, axis=axis))
+    return _get_best(ffts, a, repeat=3, number=1)
+
+
+def get_fftn(a, s=None, axes=None, repeat=3, number=1, **kw):
+    """Return the fastest function to compute the fftn.
+
+    Arguments
+    ---------
+    repeat, number : int
+        Uses :func:`timeit.repeat` to compare versions (if pyfftw is defined).
+
+    Other arguments are as for :func:`numpy.fft.fftn`.
+    """
+    ffts = []
+    if get_fftn_pyfftw:
+        ffts.append(get_fftn_pyfftw(a=a, s=s, axes=axes, **kw))
+    ffts.append(functools.partial(np.fft.fftn, s=s, axes=axes))
+    return _get_best(ffts, a, repeat=3, number=1)
+
+
+def get_ifftn(a, s=None, axes=None, repeat=3, number=1, **kw):
+    """Return the fastest function to compute the ifftn.
+
+    Arguments
+    ---------
+    repeat, number : int
+        Uses :func:`timeit.repeat` to compare versions (if pyfftw is defined).
+
+    Other arguments are as for :func:`numpy.fft.ifftn`.
+    """
+    ffts = []
+    if get_ifftn_pyfftw:
+        ffts.append(get_ifftn_pyfftw(a=a.copy(), s=s, axes=axes, **kw))
+    ffts.append(functools.partial(np.fft.ifftn, s=s, axes=axes))
+    return _get_best(ffts, a, repeat=3, number=1)
+
+
+_fft_cache = dict()
+
+
+def fft(a, n=None, axis=-1):
+    """High-performance replacement for :func:`numpy.fft.fft`"""
+    # return get_fft(a=a, n=n, axis=axis)(a)
+    key = ("fft", a.dtype, a.shape, n, axis)
+    if key not in _fft_cache:
+        _fft_cache[key] = get_fft(a=a, n=n, axis=axis)
+    res = _fft_cache[key](a)
+    if not res.flags["OWNDATA"]:
+        res = res.copy()
+    return res
+
+
+def ifft(a, n=None, axis=-1):
+    """High-performance replacement for :func:`numpy.fft.ifft`"""
+    # return get_ifft(a=a, n=n, axis=axis)(a)
+    key = ("ifft", a.dtype, a.shape, n, axis)
+    if key not in _fft_cache:
+        _fft_cache[key] = get_ifft(a=a, n=n, axis=axis)
+    res = _fft_cache[key](a)
+    if not res.flags["OWNDATA"]:
+        res = res.copy()
+    return res
+
+
+def fftn(a, s=None, axes=None):
+    """High-performance replacement for :func:`numpy.fft.fftn`"""
+    # return get_fftn(a=a, s=s, axes=axes)(a)
+    if axes is not None:
+        axes = tuple(axes)
+    key = ("fftn", a.dtype, a.shape, s, axes)
+    if key not in _fft_cache:
+        _fft_cache[key] = get_fftn(a=a, s=s, axes=axes)
+    res = _fft_cache[key](a)
+    if not res.flags["OWNDATA"]:
+        res = res.copy()
+    return res
+
+
+def ifftn(a, s=None, axes=None):
+    """High-performance replacement for :func:`numpy.fft.ifftn`"""
+    # return get_ifftn(a=a, s=s, axes=axes)(a)
+    if axes is not None:
+        axes = tuple(axes)
+    key = ("ifftn", a.dtype, a.shape, s, axes)
+    if key not in _fft_cache:
+        _fft_cache[key] = get_ifftn(a=a, s=s, axes=axes)
+    res = _fft_cache[key](a)
+    if not res.flags["OWNDATA"]:
+        res = res.copy()
+    return res
 
 
 def resample(f, N):
     """Resample f to a new grid of size N.
 
     This uses the FFT to resample the function `f` on a new grid with `N`
     points.  Note: this assumes that the function `f` is periodic.  Resampling
```

### Comparing `mmfutils-0.6.4/src/mmfutils/performance/numexpr.py` & `mmfutils-0.6.5/src/mmfutils/performance/numexpr.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/performance/threads.py` & `mmfutils-0.6.5/src/mmfutils/performance/threads.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/animation.py` & `mmfutils-0.6.5/src/mmfutils/plot/animation.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/cmaps.py` & `mmfutils-0.6.5/src/mmfutils/plot/cmaps.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/colors.py` & `mmfutils-0.6.5/src/mmfutils/plot/colors.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/contour.py` & `mmfutils-0.6.5/src/mmfutils/plot/contour.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/errors.py` & `mmfutils-0.6.5/src/mmfutils/plot/errors.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/publish.py` & `mmfutils-0.6.5/src/mmfutils/plot/publish.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/plot/rasterize.py` & `mmfutils-0.6.5/src/mmfutils/plot/rasterize.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/solve/broyden.py` & `mmfutils-0.6.5/src/mmfutils/solve/broyden.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/src/mmfutils/testing.py` & `mmfutils-0.6.5/src/mmfutils/testing.py`

 * *Files identical despite different names*

### Comparing `mmfutils-0.6.4/PKG-INFO` & `mmfutils-0.6.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmfutils
-Version: 0.6.4
+Version: 0.6.5
 Summary: Small set of utilities: containers and interfaces.
 Home-page: https://alum.mit.edu/www/mforbes/hg/forbes-group/mmfutils
 License: BSD-3
 Author: Michael McNeil Forbes
 Author-email: michael.forbes+python@gmail.com
 Requires-Python: >=3.7.13,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -33,15 +33,16 @@
 Requires-Dist: numba (>=0.56.4) ; (python_version < "3.8") and (extra == "test")
 Requires-Dist: numba (>=0.57.0) ; (python_version >= "3.8") and (extra == "test")
 Requires-Dist: numexpr (>=2.8.1) ; extra == "all" or extra == "test"
 Requires-Dist: numpy (>=1.20.2,<1.22.0) ; (python_version < "3.8") and (extra == "doc")
 Requires-Dist: numpy (>=1.23.5) ; (python_version >= "3.8") and (extra == "doc")
 Requires-Dist: persist (>=3.0) ; extra == "test"
 Requires-Dist: psutil (>=5.9.1) ; extra == "test"
-Requires-Dist: pyFFTW (>=0.13.0) ; extra == "all" or extra == "test"
+Requires-Dist: pyFFTW (==0.13.0) ; (python_version < "3.8") and (extra == "all" or extra == "test")
+Requires-Dist: pyFFTW (==0.13.1) ; (python_version >= "3.8") and (extra == "all" or extra == "test")
 Requires-Dist: pytest (>=7.1.2) ; extra == "test"
 Requires-Dist: pytest-cov (>=3.0.0) ; extra == "test"
 Requires-Dist: pytest-rerunfailures (>=11.1.2) ; extra == "test"
 Requires-Dist: scipy (>=1.10.1) ; (python_version >= "3.11") and (extra == "all" or extra == "test")
 Requires-Dist: scipy (>=1.7.3) ; (python_version >= "3.7" and python_version < "3.8") and (extra == "all" or extra == "test")
 Requires-Dist: scipy (>=1.8.1) ; (python_version >= "3.8") and (extra == "all" or extra == "test")
 Requires-Dist: sphinx-rtd-theme (>=1.2.1)
```

