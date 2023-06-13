# Comparing `tmp/chiapos-1.0.8.tar.gz` & `tmp/chiapos-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiapos-1.0.8.tar", last modified: Sun Jan  9 02:41:00 2022, max compression
+gzip compressed data, was "chiapos-1.0.9.tar", last modified: Tue Feb  1 05:09:02 2022, max compression
```

## Comparing `chiapos-1.0.8.tar` & `chiapos-1.0.9.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.881820 chiapos-1.0.8/
--rw-r--r--   0 runner     (501) staff       (20)      428 2022-01-09 02:40:34.000000 chiapos-1.0.8/.clang-format
--rw-r--r--   0 runner     (501) staff       (20)       97 2022-01-09 02:40:34.000000 chiapos-1.0.8/.dockerignore
--rw-r--r--   0 runner     (501) staff       (20)       56 2022-01-09 02:40:34.000000 chiapos-1.0.8/.flake8
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.795487 chiapos-1.0.8/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.810372 chiapos-1.0.8/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     3009 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/build-aarch64.yml
--rw-r--r--   0 runner     (501) staff       (20)     3124 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/build-m1-wheel.yml
--rw-r--r--   0 runner     (501) staff       (20)     2719 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/build-test-cplusplus.yml
--rw-r--r--   0 runner     (501) staff       (20)     4684 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner     (501) staff       (20)     1382 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/doc-html-pdf.yml
--rw-r--r--   0 runner     (501) staff       (20)     1883 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/manual-plot.yml
--rw-r--r--   0 runner     (501) staff       (20)     1252 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/plot-k27-no-bitfield.yaml
--rw-r--r--   0 runner     (501) staff       (20)     1232 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/plot-k27.yaml
--rwxr-xr-x   0 runner     (501) staff       (20)     1330 2022-01-09 02:40:34.000000 chiapos-1.0.8/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner     (501) staff       (20)      316 2022-01-09 02:40:34.000000 chiapos-1.0.8/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     5765 2022-01-09 02:40:34.000000 chiapos-1.0.8/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)      583 2022-01-09 02:40:34.000000 chiapos-1.0.8/Dockerfile
--rw-r--r--   0 runner     (501) staff       (20)    11357 2022-01-09 02:40:34.000000 chiapos-1.0.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     4195 2022-01-09 02:41:00.881385 chiapos-1.0.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3833 2022-01-09 02:40:34.000000 chiapos-1.0.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.812560 chiapos-1.0.8/chiapos.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     4195 2022-01-09 02:41:00.000000 chiapos-1.0.8/chiapos.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4740 2022-01-09 02:41:00.000000 chiapos-1.0.8/chiapos.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-01-09 02:41:00.000000 chiapos-1.0.8/chiapos.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-01-09 02:41:00.000000 chiapos-1.0.8/chiapos.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        8 2022-01-09 02:41:00.000000 chiapos-1.0.8/chiapos.egg-info/top_level.txt
--rwxr-xr-x   0 runner     (501) staff       (20)       41 2022-01-09 02:40:34.000000 chiapos-1.0.8/docker-build.sh
--rwxr-xr-x   0 runner     (501) staff       (20)       57 2022-01-09 02:40:34.000000 chiapos-1.0.8/docker-test.sh
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.818832 chiapos-1.0.8/documents/
--rw-r--r--   0 runner     (501) staff       (20)      398 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/README.txt
--rw-r--r--   0 runner     (501) staff       (20)   224153 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/bucket_graph.pdf
--rw-r--r--   0 runner     (501) staff       (20)   116670 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/code_documentation.pdf
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.822151 chiapos-1.0.8/documents/images/
--rw-r--r--   0 runner     (501) staff       (20)    13861 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/images/aesctr.png
--rw-r--r--   0 runner     (501) staff       (20)    62757 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/images/beyondhellman.png
--rw-r--r--   0 runner     (501) staff       (20)    67446 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/images/beyondhellman2.png
--rw-r--r--   0 runner     (501) staff       (20)   146667 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/images/pointerformat.png
--rw-r--r--   0 runner     (501) staff       (20)    40389 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/images/proofofspace.png
--rw-r--r--   0 runner     (501) staff       (20)  1368315 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/proof_of_space.html
--rw-r--r--   0 runner     (501) staff       (20)    75263 2022-01-09 02:40:34.000000 chiapos-1.0.8/documents/proof_of_space.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.830400 chiapos-1.0.8/hellman_example/
--rw-r--r--   0 runner     (501) staff       (20)    85217 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/Hellman attacks.pdf
--rw-r--r--   0 runner     (501) staff       (20)      353 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/Makefile
--rw-r--r--   0 runner     (501) staff       (20)    10179 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/aes.hpp
--rw-r--r--   0 runner     (501) staff       (20)    22632 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/bits.hpp
--rw-r--r--   0 runner     (501) staff       (20)    15920 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/calculate_bucket.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8358 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/cli.cpp
--rw-r--r--   0 runner     (501) staff       (20)    41970 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/cxxopts.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6187 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/encoding.hpp
--rw-r--r--   0 runner     (501) staff       (20)    13236 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/hellman.hpp
--rw-r--r--   0 runner     (501) staff       (20)    13016 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/picosha2.hpp
--rw-r--r--   0 runner     (501) staff       (20)    78714 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/plotter_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2766 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/pos_constants.hpp
--rw-r--r--   0 runner     (501) staff       (20)    28580 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/prover_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)      433 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/readme.md
--rw-r--r--   0 runner     (501) staff       (20)    34630 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/sort_on_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6605 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/util.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5474 2022-01-09 02:40:34.000000 chiapos-1.0.8/hellman_example/verifier.hpp
--rw-r--r--   0 runner     (501) staff       (20)      343 2022-01-09 02:40:34.000000 chiapos-1.0.8/lgtm.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.798787 chiapos-1.0.8/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.831761 chiapos-1.0.8/lib/FiniteStateEntropy/
--rw-r--r--   0 runner     (501) staff       (20)     1293 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     3636 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.797137 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.832183 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.833109 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE/
--rw-r--r--   0 runner     (501) staff       (20)    10066 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
--rw-r--r--   0 runner     (501) staff       (20)     1414 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
--rw-r--r--   0 runner     (501) staff       (20)     2821 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.833552 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
--rw-r--r--   0 runner     (501) staff       (20)     8930 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.834386 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/libfse/
--rw-r--r--   0 runner     (501) staff       (20)     1414 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
--rw-r--r--   0 runner     (501) staff       (20)    10601 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
--rw-r--r--   0 runner     (501) staff       (20)     5026 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.843263 chiapos-1.0.8/lib/FiniteStateEntropy/lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.844113 chiapos-1.0.8/lib/FiniteStateEntropy/lib/Archives/
--rw-r--r--   0 runner     (501) staff       (20)     2928 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/Archives/hufx6.h
--rw-r--r--   0 runner     (501) staff       (20)    18735 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
--rw-r--r--   0 runner     (501) staff       (20)     1579 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/README.md
--rw-r--r--   0 runner     (501) staff       (20)    18204 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/bitstream.h
--rw-r--r--   0 runner     (501) staff       (20)     3919 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/compiler.h
--rw-r--r--   0 runner     (501) staff       (20)     1912 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/debug.c
--rw-r--r--   0 runner     (501) staff       (20)     4605 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/debug.h
--rw-r--r--   0 runner     (501) staff       (20)     9599 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/entropy_common.c
--rw-r--r--   0 runner     (501) staff       (20)     4375 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/error_private.h
--rw-r--r--   0 runner     (501) staff       (20)     2434 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/error_public.h
--rw-r--r--   0 runner     (501) staff       (20)    32982 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/fse.h
--rw-r--r--   0 runner     (501) staff       (20)    11446 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/fseU16.c
--rw-r--r--   0 runner     (501) staff       (20)     3570 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/fseU16.h
--rw-r--r--   0 runner     (501) staff       (20)    27523 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/fse_compress.c
--rw-r--r--   0 runner     (501) staff       (20)    11179 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/fse_decompress.c
--rw-r--r--   0 runner     (501) staff       (20)     7926 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/hist.c
--rw-r--r--   0 runner     (501) staff       (20)     4327 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/hist.h
--rw-r--r--   0 runner     (501) staff       (20)    19479 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/huf.h
--rw-r--r--   0 runner     (501) staff       (20)    32593 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/huf_compress.c
--rw-r--r--   0 runner     (501) staff       (20)    45802 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/huf_decompress.c
--rw-r--r--   0 runner     (501) staff       (20)    11394 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/lib/mem.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.853124 chiapos-1.0.8/lib/FiniteStateEntropy/programs/
--rw-r--r--   0 runner     (501) staff       (20)    18092 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/COPYING
--rw-r--r--   0 runner     (501) staff       (20)      287 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/README.md
--rw-r--r--   0 runner     (501) staff       (20)    29002 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/bench.c
--rw-r--r--   0 runner     (501) staff       (20)     1455 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/bench.h
--rw-r--r--   0 runner     (501) staff       (20)    12301 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/commandline.c
--rw-r--r--   0 runner     (501) staff       (20)     4444 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/cpu.h
--rw-r--r--   0 runner     (501) staff       (20)    22894 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fileio.c
--rw-r--r--   0 runner     (501) staff       (20)     2073 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fileio.h
--rw-r--r--   0 runner     (501) staff       (20)    19607 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fseDist.c
--rw-r--r--   0 runner     (501) staff       (20)     1608 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fseDist.h
--rw-r--r--   0 runner     (501) staff       (20)    44827 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fullbench.c
--rw-r--r--   0 runner     (501) staff       (20)    20262 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fuzzer.c
--rw-r--r--   0 runner     (501) staff       (20)    14122 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
--rw-r--r--   0 runner     (501) staff       (20)    13406 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/fuzzerU16.c
--rw-r--r--   0 runner     (501) staff       (20)     4406 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/probaGenerator.c
--rw-r--r--   0 runner     (501) staff       (20)    28510 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/xxhash.c
--rw-r--r--   0 runner     (501) staff       (20)    12352 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/xxhash.h
--rw-r--r--   0 runner     (501) staff       (20)    68887 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/zlibh.c
--rw-r--r--   0 runner     (501) staff       (20)     4817 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/FiniteStateEntropy/programs/zlibh.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.853603 chiapos-1.0.8/lib/include/
--rw-r--r--   0 runner     (501) staff       (20)    13016 2022-01-09 02:40:34.000000 chiapos-1.0.8/lib/include/picosha2.hpp
--rw-r--r--   0 runner     (501) staff       (20)       37 2022-01-09 02:40:34.000000 chiapos-1.0.8/mypi.ini
--rw-r--r--   0 runner     (501) staff       (20)      194 2022-01-09 02:40:34.000000 chiapos-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.854016 chiapos-1.0.8/python-bindings/
--rw-r--r--   0 runner     (501) staff       (20)     6452 2022-01-09 02:40:34.000000 chiapos-1.0.8/python-bindings/chiapos.cpp
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-01-09 02:41:00.881948 chiapos-1.0.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     7006 2022-01-09 02:40:34.000000 chiapos-1.0.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.868111 chiapos-1.0.8/src/
--rw-r--r--   0 runner     (501) staff       (20)    21159 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b17phase2.hpp
--rw-r--r--   0 runner     (501) staff       (20)    21395 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b17phase3.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8685 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b17phase4.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11996 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b17sort_manager.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.873411 chiapos-1.0.8/src/b3/
--rw-r--r--   0 runner     (501) staff       (20)    26722 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3.c
--rw-r--r--   0 runner     (501) staff       (20)     1759 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3.h
--rw-r--r--   0 runner     (501) staff       (20)    12411 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_avx2.c
--rw-r--r--   0 runner     (501) staff       (20)    65803 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_avx2_x86-64_unix.S
--rw-r--r--   0 runner     (501) staff       (20)    47960 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_avx512.c
--rw-r--r--   0 runner     (501) staff       (20)    89081 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_avx512_x86-64_unix.S
--rw-r--r--   0 runner     (501) staff       (20)     6764 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_dispatch.c
--rw-r--r--   0 runner     (501) staff       (20)     8423 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_impl.h
--rw-r--r--   0 runner     (501) staff       (20)     6078 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_portable.c
--rw-r--r--   0 runner     (501) staff       (20)    20772 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_sse41.c
--rw-r--r--   0 runner     (501) staff       (20)    60859 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/b3/blake3_sse41_x86-64_unix.S
--rw-r--r--   0 runner     (501) staff       (20)     2144 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/bitfield.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2223 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/bitfield_index.hpp
--rw-r--r--   0 runner     (501) staff       (20)    19655 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/bits.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11224 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/calculate_bucket.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4292 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/chacha8.c
--rw-r--r--   0 runner     (501) staff       (20)      431 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/chacha8.h
--rw-r--r--   0 runner     (501) staff       (20)     1104 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/chia_filesystem.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11257 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/cli.cpp
--rw-r--r--   0 runner     (501) staff       (20)    16417 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     7635 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/encoding.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4427 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/entry_sizes.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1449 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/exceptions.hpp
--rw-r--r--   0 runner     (501) staff       (20)    32661 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/phase1.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11324 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/phase2.hpp
--rw-r--r--   0 runner     (501) staff       (20)    23014 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/phase3.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8587 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/phase4.hpp
--rw-r--r--   0 runner     (501) staff       (20)      799 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/phases.hpp
--rw-r--r--   0 runner     (501) staff       (20)    18848 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/plotter_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3819 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/pos_constants.hpp
--rw-r--r--   0 runner     (501) staff       (20)      284 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/progress.hpp
--rw-r--r--   0 runner     (501) staff       (20)    28981 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/prover_disk.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3272 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/quicksort.hpp
--rw-r--r--   0 runner     (501) staff       (20)    11844 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/sort_manager.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1853 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/threading.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4253 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/uniformsort.hpp
--rw-r--r--   0 runner     (501) staff       (20)    10882 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/util.hpp
--rw-r--r--   0 runner     (501) staff       (20)     6193 2022-01-09 02:40:34.000000 chiapos-1.0.8/src/verifier.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.876125 chiapos-1.0.8/tests/
--rw-r--r--   0 runner     (501) staff       (20)       31 2022-01-09 02:40:34.000000 chiapos-1.0.8/tests/.flake8
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-01-09 02:40:34.000000 chiapos-1.0.8/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6367 2022-01-09 02:40:34.000000 chiapos-1.0.8/tests/plot-resources.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2022-01-09 02:40:34.000000 chiapos-1.0.8/tests/test-main.cpp
--rw-r--r--   0 runner     (501) staff       (20)    36230 2022-01-09 02:40:34.000000 chiapos-1.0.8/tests/test.cpp
--rw-r--r--   0 runner     (501) staff       (20)     5403 2022-01-09 02:40:34.000000 chiapos-1.0.8/tests/test_python_bindings.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.877069 chiapos-1.0.8/tools/
--rwxr-xr-x   0 runner     (501) staff       (20)      879 2022-01-09 02:40:34.000000 chiapos-1.0.8/tools/disk.gnuplot
--rw-r--r--   0 runner     (501) staff       (20)      864 2022-01-09 02:40:34.000000 chiapos-1.0.8/tools/parse_disk.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-01-09 02:41:00.880784 chiapos-1.0.8/uint128_t/
--rw-r--r--   0 runner     (501) staff       (20)     1108 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     1385 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1124 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/endianness.h
--rw-r--r--   0 runner     (501) staff       (20)      203 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/uint128_t.build
--rw-r--r--   0 runner     (501) staff       (20)    13671 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner     (501) staff       (20)      180 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/uint128_t.h
--rw-r--r--   0 runner     (501) staff       (20)    19685 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/uint128_t.include
--rw-r--r--   0 runner     (501) staff       (20)      653 2022-01-09 02:40:34.000000 chiapos-1.0.8/uint128_t/uint128_t_config.include
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.065206 chiapos-1.0.9/
+-rw-r--r--   0 runner     (501) staff       (20)      428 2022-02-01 05:08:30.000000 chiapos-1.0.9/.clang-format
+-rw-r--r--   0 runner     (501) staff       (20)       97 2022-02-01 05:08:30.000000 chiapos-1.0.9/.dockerignore
+-rw-r--r--   0 runner     (501) staff       (20)       56 2022-02-01 05:08:30.000000 chiapos-1.0.9/.flake8
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.977973 chiapos-1.0.9/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.992634 chiapos-1.0.9/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     3009 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-aarch64.yml
+-rw-r--r--   0 runner     (501) staff       (20)     3124 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-m1-wheel.yml
+-rw-r--r--   0 runner     (501) staff       (20)     2719 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-test-cplusplus.yml
+-rw-r--r--   0 runner     (501) staff       (20)     4684 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1382 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/doc-html-pdf.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1883 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/manual-plot.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1252 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/plot-k27-no-bitfield.yaml
+-rw-r--r--   0 runner     (501) staff       (20)     1232 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/plot-k27.yaml
+-rwxr-xr-x   0 runner     (501) staff       (20)     1330 2022-02-01 05:08:30.000000 chiapos-1.0.9/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner     (501) staff       (20)      316 2022-02-01 05:08:30.000000 chiapos-1.0.9/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     5765 2022-02-01 05:08:30.000000 chiapos-1.0.9/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)      583 2022-02-01 05:08:30.000000 chiapos-1.0.9/Dockerfile
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2022-02-01 05:08:30.000000 chiapos-1.0.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     4195 2022-02-01 05:09:02.064738 chiapos-1.0.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3833 2022-02-01 05:08:30.000000 chiapos-1.0.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.994817 chiapos-1.0.9/chiapos.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     4195 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4740 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        8 2022-02-01 05:09:01.000000 chiapos-1.0.9/chiapos.egg-info/top_level.txt
+-rwxr-xr-x   0 runner     (501) staff       (20)       41 2022-02-01 05:08:30.000000 chiapos-1.0.9/docker-build.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)       57 2022-02-01 05:08:30.000000 chiapos-1.0.9/docker-test.sh
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.001801 chiapos-1.0.9/documents/
+-rw-r--r--   0 runner     (501) staff       (20)      398 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/README.txt
+-rw-r--r--   0 runner     (501) staff       (20)   224153 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/bucket_graph.pdf
+-rw-r--r--   0 runner     (501) staff       (20)   116670 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/code_documentation.pdf
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.005189 chiapos-1.0.9/documents/images/
+-rw-r--r--   0 runner     (501) staff       (20)    13861 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/aesctr.png
+-rw-r--r--   0 runner     (501) staff       (20)    62757 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/beyondhellman.png
+-rw-r--r--   0 runner     (501) staff       (20)    67446 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/beyondhellman2.png
+-rw-r--r--   0 runner     (501) staff       (20)   146667 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/pointerformat.png
+-rw-r--r--   0 runner     (501) staff       (20)    40389 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/images/proofofspace.png
+-rw-r--r--   0 runner     (501) staff       (20)  1368315 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/proof_of_space.html
+-rw-r--r--   0 runner     (501) staff       (20)    75263 2022-02-01 05:08:30.000000 chiapos-1.0.9/documents/proof_of_space.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.013658 chiapos-1.0.9/hellman_example/
+-rw-r--r--   0 runner     (501) staff       (20)    85217 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/Hellman attacks.pdf
+-rw-r--r--   0 runner     (501) staff       (20)      353 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)    10179 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/aes.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    22632 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/bits.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    15920 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/calculate_bucket.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8358 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/cli.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    41970 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/cxxopts.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6187 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/encoding.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    13236 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/hellman.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    13016 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/picosha2.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    78714 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/plotter_disk.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2766 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/pos_constants.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    28580 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/prover_disk.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      433 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/readme.md
+-rw-r--r--   0 runner     (501) staff       (20)    34630 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/sort_on_disk.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6605 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/util.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5474 2022-02-01 05:08:30.000000 chiapos-1.0.9/hellman_example/verifier.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      343 2022-02-01 05:08:30.000000 chiapos-1.0.9/lgtm.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.981036 chiapos-1.0.9/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.014940 chiapos-1.0.9/lib/FiniteStateEntropy/
+-rw-r--r--   0 runner     (501) staff       (20)     1293 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:01.979475 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.015366 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.016303 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/
+-rw-r--r--   0 runner     (501) staff       (20)    10066 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
+-rw-r--r--   0 runner     (501) staff       (20)     1414 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
+-rw-r--r--   0 runner     (501) staff       (20)     2821 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.016728 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
+-rw-r--r--   0 runner     (501) staff       (20)     8930 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.017677 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/
+-rw-r--r--   0 runner     (501) staff       (20)     1414 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
+-rw-r--r--   0 runner     (501) staff       (20)    10601 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
+-rw-r--r--   0 runner     (501) staff       (20)     5026 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.026654 chiapos-1.0.9/lib/FiniteStateEntropy/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.027611 chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/
+-rw-r--r--   0 runner     (501) staff       (20)     2928 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6.h
+-rw-r--r--   0 runner     (501) staff       (20)    18735 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
+-rw-r--r--   0 runner     (501) staff       (20)     1579 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    18204 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/bitstream.h
+-rw-r--r--   0 runner     (501) staff       (20)     3919 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/compiler.h
+-rw-r--r--   0 runner     (501) staff       (20)     1912 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.c
+-rw-r--r--   0 runner     (501) staff       (20)     4605 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.h
+-rw-r--r--   0 runner     (501) staff       (20)     9599 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/entropy_common.c
+-rw-r--r--   0 runner     (501) staff       (20)     4375 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_private.h
+-rw-r--r--   0 runner     (501) staff       (20)     2434 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_public.h
+-rw-r--r--   0 runner     (501) staff       (20)    32982 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse.h
+-rw-r--r--   0 runner     (501) staff       (20)    11446 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.c
+-rw-r--r--   0 runner     (501) staff       (20)     3570 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.h
+-rw-r--r--   0 runner     (501) staff       (20)    27523 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_compress.c
+-rw-r--r--   0 runner     (501) staff       (20)    11179 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_decompress.c
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.c
+-rw-r--r--   0 runner     (501) staff       (20)     4327 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.h
+-rw-r--r--   0 runner     (501) staff       (20)    19479 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf.h
+-rw-r--r--   0 runner     (501) staff       (20)    32593 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_compress.c
+-rw-r--r--   0 runner     (501) staff       (20)    45802 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_decompress.c
+-rw-r--r--   0 runner     (501) staff       (20)    11394 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/lib/mem.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.036744 chiapos-1.0.9/lib/FiniteStateEntropy/programs/
+-rw-r--r--   0 runner     (501) staff       (20)    18092 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/COPYING
+-rw-r--r--   0 runner     (501) staff       (20)      287 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    29002 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.c
+-rw-r--r--   0 runner     (501) staff       (20)     1455 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.h
+-rw-r--r--   0 runner     (501) staff       (20)    12301 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/commandline.c
+-rw-r--r--   0 runner     (501) staff       (20)     4444 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/cpu.h
+-rw-r--r--   0 runner     (501) staff       (20)    22894 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.c
+-rw-r--r--   0 runner     (501) staff       (20)     2073 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.h
+-rw-r--r--   0 runner     (501) staff       (20)    19607 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.c
+-rw-r--r--   0 runner     (501) staff       (20)     1608 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.h
+-rw-r--r--   0 runner     (501) staff       (20)    44827 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fullbench.c
+-rw-r--r--   0 runner     (501) staff       (20)    20262 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzer.c
+-rw-r--r--   0 runner     (501) staff       (20)    14122 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
+-rw-r--r--   0 runner     (501) staff       (20)    13406 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerU16.c
+-rw-r--r--   0 runner     (501) staff       (20)     4406 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/probaGenerator.c
+-rw-r--r--   0 runner     (501) staff       (20)    28510 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.c
+-rw-r--r--   0 runner     (501) staff       (20)    12352 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.h
+-rw-r--r--   0 runner     (501) staff       (20)    68887 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.c
+-rw-r--r--   0 runner     (501) staff       (20)     4817 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.037165 chiapos-1.0.9/lib/include/
+-rw-r--r--   0 runner     (501) staff       (20)    13016 2022-02-01 05:08:30.000000 chiapos-1.0.9/lib/include/picosha2.hpp
+-rw-r--r--   0 runner     (501) staff       (20)       37 2022-02-01 05:08:30.000000 chiapos-1.0.9/mypi.ini
+-rw-r--r--   0 runner     (501) staff       (20)      194 2022-02-01 05:08:30.000000 chiapos-1.0.9/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.037596 chiapos-1.0.9/python-bindings/
+-rw-r--r--   0 runner     (501) staff       (20)     6452 2022-02-01 05:08:30.000000 chiapos-1.0.9/python-bindings/chiapos.cpp
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-02-01 05:09:02.065398 chiapos-1.0.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     7006 2022-02-01 05:08:30.000000 chiapos-1.0.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.051625 chiapos-1.0.9/src/
+-rw-r--r--   0 runner     (501) staff       (20)    21159 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17phase2.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    21395 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17phase3.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8685 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17phase4.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    11996 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b17sort_manager.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.056936 chiapos-1.0.9/src/b3/
+-rw-r--r--   0 runner     (501) staff       (20)    26722 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3.c
+-rw-r--r--   0 runner     (501) staff       (20)     1759 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3.h
+-rw-r--r--   0 runner     (501) staff       (20)    12411 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx2.c
+-rw-r--r--   0 runner     (501) staff       (20)    65803 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx2_x86-64_unix.S
+-rw-r--r--   0 runner     (501) staff       (20)    47960 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx512.c
+-rw-r--r--   0 runner     (501) staff       (20)    89081 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_avx512_x86-64_unix.S
+-rw-r--r--   0 runner     (501) staff       (20)     6764 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_dispatch.c
+-rw-r--r--   0 runner     (501) staff       (20)     8423 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_impl.h
+-rw-r--r--   0 runner     (501) staff       (20)     6078 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_portable.c
+-rw-r--r--   0 runner     (501) staff       (20)    20772 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_sse41.c
+-rw-r--r--   0 runner     (501) staff       (20)    60859 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/b3/blake3_sse41_x86-64_unix.S
+-rw-r--r--   0 runner     (501) staff       (20)     2144 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/bitfield.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2223 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/bitfield_index.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    19655 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/bits.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    11224 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/calculate_bucket.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4292 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/chacha8.c
+-rw-r--r--   0 runner     (501) staff       (20)      431 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/chacha8.h
+-rw-r--r--   0 runner     (501) staff       (20)     1104 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/chia_filesystem.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    11257 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/cli.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    16417 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/disk.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     7635 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/encoding.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4427 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/entry_sizes.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1449 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/exceptions.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    32661 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase1.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    11324 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase2.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    23014 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase3.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8587 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phase4.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      799 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/phases.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    19237 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/plotter_disk.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3819 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/pos_constants.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      284 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/progress.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    28981 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/prover_disk.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3272 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/quicksort.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    11844 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/sort_manager.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1853 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/threading.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4253 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/uniformsort.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    10882 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/util.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     6193 2022-02-01 05:08:30.000000 chiapos-1.0.9/src/verifier.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.059710 chiapos-1.0.9/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       31 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/.flake8
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6367 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/plot-resources.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/test-main.cpp
+-rw-r--r--   0 runner     (501) staff       (20)    36230 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/test.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     5403 2022-02-01 05:08:30.000000 chiapos-1.0.9/tests/test_python_bindings.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.060519 chiapos-1.0.9/tools/
+-rwxr-xr-x   0 runner     (501) staff       (20)      879 2022-02-01 05:08:30.000000 chiapos-1.0.9/tools/disk.gnuplot
+-rw-r--r--   0 runner     (501) staff       (20)      864 2022-02-01 05:08:30.000000 chiapos-1.0.9/tools/parse_disk.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-02-01 05:09:02.064131 chiapos-1.0.9/uint128_t/
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     1385 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1124 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/endianness.h
+-rw-r--r--   0 runner     (501) staff       (20)      203 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.build
+-rw-r--r--   0 runner     (501) staff       (20)    13671 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      180 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.h
+-rw-r--r--   0 runner     (501) staff       (20)    19685 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t.include
+-rw-r--r--   0 runner     (501) staff       (20)      653 2022-02-01 05:08:30.000000 chiapos-1.0.9/uint128_t/uint128_t_config.include
```

### Comparing `chiapos-1.0.8/.github/workflows/build-aarch64.yml` & `chiapos-1.0.9/.github/workflows/build-aarch64.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/build-m1-wheel.yml` & `chiapos-1.0.9/.github/workflows/build-m1-wheel.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/build-test-cplusplus.yml` & `chiapos-1.0.9/.github/workflows/build-test-cplusplus.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/build-wheels.yml` & `chiapos-1.0.9/.github/workflows/build-wheels.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/doc-html-pdf.yml` & `chiapos-1.0.9/.github/workflows/doc-html-pdf.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/manual-plot.yml` & `chiapos-1.0.9/.github/workflows/manual-plot.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/plot-k27-no-bitfield.yaml` & `chiapos-1.0.9/.github/workflows/plot-k27-no-bitfield.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/plot-k27.yaml` & `chiapos-1.0.9/.github/workflows/plot-k27.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/.github/workflows/stale-issue.yml` & `chiapos-1.0.9/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/CMakeLists.txt` & `chiapos-1.0.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/Dockerfile` & `chiapos-1.0.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/LICENSE` & `chiapos-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/PKG-INFO` & `chiapos-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 1.0.8
+Version: 1.0.9
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `chiapos-1.0.8/README.md` & `chiapos-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/chiapos.egg-info/PKG-INFO` & `chiapos-1.0.9/chiapos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 1.0.8
+Version: 1.0.9
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `chiapos-1.0.8/chiapos.egg-info/SOURCES.txt` & `chiapos-1.0.9/chiapos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/bucket_graph.pdf` & `chiapos-1.0.9/documents/bucket_graph.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/code_documentation.pdf` & `chiapos-1.0.9/documents/code_documentation.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/images/aesctr.png` & `chiapos-1.0.9/documents/images/aesctr.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/images/beyondhellman.png` & `chiapos-1.0.9/documents/images/beyondhellman.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/images/beyondhellman2.png` & `chiapos-1.0.9/documents/images/beyondhellman2.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/images/pointerformat.png` & `chiapos-1.0.9/documents/images/pointerformat.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/images/proofofspace.png` & `chiapos-1.0.9/documents/images/proofofspace.png`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/proof_of_space.html` & `chiapos-1.0.9/documents/proof_of_space.html`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/documents/proof_of_space.md` & `chiapos-1.0.9/documents/proof_of_space.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/Hellman attacks.pdf` & `chiapos-1.0.9/hellman_example/Hellman attacks.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/aes.hpp` & `chiapos-1.0.9/hellman_example/aes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/bits.hpp` & `chiapos-1.0.9/hellman_example/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/calculate_bucket.hpp` & `chiapos-1.0.9/hellman_example/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/cli.cpp` & `chiapos-1.0.9/hellman_example/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/cxxopts.hpp` & `chiapos-1.0.9/hellman_example/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/encoding.hpp` & `chiapos-1.0.9/hellman_example/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/hellman.hpp` & `chiapos-1.0.9/hellman_example/hellman.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/picosha2.hpp` & `chiapos-1.0.9/hellman_example/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/plotter_disk.hpp` & `chiapos-1.0.9/hellman_example/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/pos_constants.hpp` & `chiapos-1.0.9/hellman_example/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/prover_disk.hpp` & `chiapos-1.0.9/hellman_example/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/sort_on_disk.hpp` & `chiapos-1.0.9/hellman_example/sort_on_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/util.hpp` & `chiapos-1.0.9/hellman_example/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/hellman_example/verifier.hpp` & `chiapos-1.0.9/hellman_example/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/LICENSE` & `chiapos-1.0.9/lib/FiniteStateEntropy/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/README.md` & `chiapos-1.0.9/lib/FiniteStateEntropy/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj` & `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc` & `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln` & `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj` & `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc` & `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj` & `chiapos-1.0.9/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt` & `chiapos-1.0.9/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/Archives/hufx6.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/README.md` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/bitstream.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/bitstream.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/compiler.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/compiler.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/debug.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/debug.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/debug.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/entropy_common.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/entropy_common.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/error_private.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_private.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/error_public.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/error_public.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/fse.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/fseU16.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/fseU16.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fseU16.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/fse_compress.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/fse_decompress.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/hist.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/hist.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/hist.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/huf.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/huf_compress.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/huf_decompress.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/lib/mem.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/lib/mem.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/COPYING` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/COPYING`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/bench.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/bench.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/bench.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/commandline.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/commandline.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/cpu.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/cpu.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fileio.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fileio.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fseDist.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fseDist.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fseDist.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fullbench.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fullbench.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fuzzer.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzer.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fuzzerHuff0.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerHuff0.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/fuzzerU16.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/fuzzerU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/probaGenerator.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/probaGenerator.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/xxhash.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/xxhash.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/xxhash.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/zlibh.c` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/FiniteStateEntropy/programs/zlibh.h` & `chiapos-1.0.9/lib/FiniteStateEntropy/programs/zlibh.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/lib/include/picosha2.hpp` & `chiapos-1.0.9/lib/include/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/python-bindings/chiapos.cpp` & `chiapos-1.0.9/python-bindings/chiapos.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/setup.py` & `chiapos-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b17phase2.hpp` & `chiapos-1.0.9/src/b17phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b17phase3.hpp` & `chiapos-1.0.9/src/b17phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b17phase4.hpp` & `chiapos-1.0.9/src/b17phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b17sort_manager.hpp` & `chiapos-1.0.9/src/b17sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3.c` & `chiapos-1.0.9/src/b3/blake3.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3.h` & `chiapos-1.0.9/src/b3/blake3.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_avx2.c` & `chiapos-1.0.9/src/b3/blake3_avx2.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_avx2_x86-64_unix.S` & `chiapos-1.0.9/src/b3/blake3_avx2_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_avx512.c` & `chiapos-1.0.9/src/b3/blake3_avx512.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_avx512_x86-64_unix.S` & `chiapos-1.0.9/src/b3/blake3_avx512_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_dispatch.c` & `chiapos-1.0.9/src/b3/blake3_dispatch.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_impl.h` & `chiapos-1.0.9/src/b3/blake3_impl.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_portable.c` & `chiapos-1.0.9/src/b3/blake3_portable.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_sse41.c` & `chiapos-1.0.9/src/b3/blake3_sse41.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/b3/blake3_sse41_x86-64_unix.S` & `chiapos-1.0.9/src/b3/blake3_sse41_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/bitfield.hpp` & `chiapos-1.0.9/src/bitfield.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/bitfield_index.hpp` & `chiapos-1.0.9/src/bitfield_index.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/bits.hpp` & `chiapos-1.0.9/src/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/calculate_bucket.hpp` & `chiapos-1.0.9/src/calculate_bucket.hpp`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -205,16 +205,16 @@
     inline FxCalculator(uint8_t k, uint8_t table_index)
     {
         this->k_ = k;
         this->table_index_ = table_index;
 
         this->rmap.resize(kBC);
         if (!initialized) {
-            initialized = true;
             load_tables();
+            initialized = true;
         }
     }
 
     inline ~FxCalculator() = default;
 
     // Disable copying
     FxCalculator(const FxCalculator&) = delete;
```

### Comparing `chiapos-1.0.8/src/chacha8.c` & `chiapos-1.0.9/src/chacha8.c`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/chia_filesystem.hpp` & `chiapos-1.0.9/src/chia_filesystem.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/cli.cpp` & `chiapos-1.0.9/src/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/disk.hpp` & `chiapos-1.0.9/src/disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/encoding.hpp` & `chiapos-1.0.9/src/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/entry_sizes.hpp` & `chiapos-1.0.9/src/entry_sizes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/exceptions.hpp` & `chiapos-1.0.9/src/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/phase1.hpp` & `chiapos-1.0.9/src/phase1.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/phase2.hpp` & `chiapos-1.0.9/src/phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/phase3.hpp` & `chiapos-1.0.9/src/phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/phase4.hpp` & `chiapos-1.0.9/src/phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/phases.hpp` & `chiapos-1.0.9/src/phases.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/plotter_disk.hpp` & `chiapos-1.0.9/src/plotter_disk.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #include <semaphore.h>
 #include <sys/resource.h>
 #include <unistd.h>
 #endif
 
 #include <math.h>
 #include <stdio.h>
+#include <sys/stat.h>
 
 #include <algorithm>
 #include <fstream>
 #include <iostream>
 #include <map>
 #include <string>
 #include <vector>
@@ -366,15 +367,21 @@
         }
 
         bool bCopied = false;
         bool bRenamed = false;
         Timer copy;
         do {
             std::error_code ec;
-            if (tmp_2_filename.parent_path() == final_filename.parent_path()) {
+            struct stat tmp2_stat, final_stat;
+            int rc;
+            rc = ::stat(reinterpret_cast<const char *>(tmp_2_filename.c_str()), &tmp2_stat);
+            if (rc == 0)
+                rc = ::stat(reinterpret_cast<const char *>(final_filename.parent_path().c_str()), &final_stat);
+            if ((rc == 0 && tmp2_stat.st_dev == final_stat.st_dev) ||
+                tmp_2_filename.parent_path() == final_filename.parent_path()) {
                 fs::rename(tmp_2_filename, final_filename, ec);
                 if (ec.value() != 0) {
                     std::cout << "Could not rename " << tmp_2_filename << " to " << final_filename
                               << ". Error " << ec.message() << ". Retrying in five minutes."
                               << std::endl;
                 } else {
                     bRenamed = true;
```

### Comparing `chiapos-1.0.8/src/pos_constants.hpp` & `chiapos-1.0.9/src/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/prover_disk.hpp` & `chiapos-1.0.9/src/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/quicksort.hpp` & `chiapos-1.0.9/src/quicksort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/sort_manager.hpp` & `chiapos-1.0.9/src/sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/threading.hpp` & `chiapos-1.0.9/src/threading.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/uniformsort.hpp` & `chiapos-1.0.9/src/uniformsort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/util.hpp` & `chiapos-1.0.9/src/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/src/verifier.hpp` & `chiapos-1.0.9/src/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/tests/plot-resources.py` & `chiapos-1.0.9/tests/plot-resources.py`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/tests/test-main.cpp` & `chiapos-1.0.9/tests/test-main.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/tests/test.cpp` & `chiapos-1.0.9/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/tests/test_python_bindings.py` & `chiapos-1.0.9/tests/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/tools/disk.gnuplot` & `chiapos-1.0.9/tools/disk.gnuplot`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/tools/parse_disk.py` & `chiapos-1.0.9/tools/parse_disk.py`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/uint128_t/LICENSE` & `chiapos-1.0.9/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/uint128_t/README.md` & `chiapos-1.0.9/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/uint128_t/endianness.h` & `chiapos-1.0.9/uint128_t/endianness.h`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/uint128_t/uint128_t.cpp` & `chiapos-1.0.9/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/uint128_t/uint128_t.include` & `chiapos-1.0.9/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chiapos-1.0.8/uint128_t/uint128_t_config.include` & `chiapos-1.0.9/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

