# Comparing `tmp/stim-1.9.dev1656756326.tar.gz` & `tmp/stim-1.9.dev1657429876.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stim-1.9.dev1656756326.tar", last modified: Sat Jul  2 10:29:34 2022, max compression
+gzip compressed data, was "stim-1.9.dev1657429876.tar", last modified: Sun Jul 10 05:33:53 2022, max compression
```

## Comparing `stim-1.9.dev1656756326.tar` & `stim-1.9.dev1657429876.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.463694 stim-1.9.dev1656756326/
--rw-r--r--   0 runner     (501) staff       (20)    11357 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      103 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     4190 2022-07-02 10:29:34.463274 stim-1.9.dev1656756326/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3846 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.328868 stim-1.9.dev1656756326/glue/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.334960 stim-1.9.dev1656756326/glue/python/
--rw-r--r--   0 runner     (501) staff       (20)     3846 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/glue/python/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.329250 stim-1.9.dev1656756326/glue/python/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.337001 stim-1.9.dev1656756326/glue/python/src/stim/
--rw-r--r--   0 runner     (501) staff       (20)     2357 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/glue/python/src/stim/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)   201734 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/glue/python/src/stim/__init__.pyi
--rw-r--r--   0 runner     (501) staff       (20)      134 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/glue/python/src/stim/_main_argv.py
--rw-r--r--   0 runner     (501) staff       (20)      109 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-02 10:29:34.463807 stim-1.9.dev1656756326/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3649 2022-07-02 10:07:06.000000 stim-1.9.dev1656756326/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.339565 stim-1.9.dev1656756326/src/
--rw-r--r--   0 runner     (501) staff       (20)      701 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/main.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.349900 stim-1.9.dev1656756326/src/stim/
--rw-r--r--   0 runner     (501) staff       (20)    10123 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/arg_parse.cc
--rw-r--r--   0 runner     (501) staff       (20)     9242 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/arg_parse.h
--rw-r--r--   0 runner     (501) staff       (20)    11209 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/arg_parse.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     6036 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/benchmark_main.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)      627 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/benchmark_util.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     3973 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/benchmark_util.perf.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.367228 stim-1.9.dev1656756326/src/stim/circuit/
--rw-r--r--   0 runner     (501) staff       (20)    47320 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.cc
--rw-r--r--   0 runner     (501) staff       (20)    15456 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.h
--rw-r--r--   0 runner     (501) staff       (20)     1431 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    74537 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1080 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    36126 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.test.cc
--rw-r--r--   0 runner     (501) staff       (20)      977 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit.test.h
--rw-r--r--   0 runner     (501) staff       (20)     5342 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit_gate_target.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)      996 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit_gate_target.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     5902 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit_instruction.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1668 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit_instruction.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     4617 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit_repeat_block.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1155 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/circuit_repeat_block.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     5472 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data.cc
--rw-r--r--   0 runner     (501) staff       (20)     9837 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data.h
--rw-r--r--   0 runner     (501) staff       (20)     1198 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     3280 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    13456 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_annotations.cc
--rw-r--r--   0 runner     (501) staff       (20)     2093 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_blocks.cc
--rw-r--r--   0 runner     (501) staff       (20)    14084 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_collapsing.cc
--rw-r--r--   0 runner     (501) staff       (20)    10531 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_controlled.cc
--rw-r--r--   0 runner     (501) staff       (20)     3221 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_hada.cc
--rw-r--r--   0 runner     (501) staff       (20)    11977 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_noisy.cc
--rw-r--r--   0 runner     (501) staff       (20)     3588 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_pauli.cc
--rw-r--r--   0 runner     (501) staff       (20)     2483 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_period_3.cc
--rw-r--r--   0 runner     (501) staff       (20)     5635 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_period_4.cc
--rw-r--r--   0 runner     (501) staff       (20)     6624 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_pp.cc
--rw-r--r--   0 runner     (501) staff       (20)     3517 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_data_swaps.cc
--rw-r--r--   0 runner     (501) staff       (20)     5748 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_target.cc
--rw-r--r--   0 runner     (501) staff       (20)     2307 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_target.h
--rw-r--r--   0 runner     (501) staff       (20)     6040 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/circuit/gate_target.test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.374011 stim-1.9.dev1656756326/src/stim/dem/
--rw-r--r--   0 runner     (501) staff       (20)    31371 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model.cc
--rw-r--r--   0 runner     (501) staff       (20)     7894 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model.h
--rw-r--r--   0 runner     (501) staff       (20)    36715 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)      901 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    25490 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     8077 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model_instruction.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1437 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model_instruction.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     3686 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model_repeat_block.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1159 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model_repeat_block.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     8395 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model_target.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1221 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/dem/detector_error_model_target.pybind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.381882 stim-1.9.dev1656756326/src/stim/gen/
--rw-r--r--   0 runner     (501) staff       (20)     2887 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/circuit_gen_main.cc
--rw-r--r--   0 runner     (501) staff       (20)      249 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/circuit_gen_main.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/circuit_gen_main.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4061 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/circuit_gen_params.cc
--rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/circuit_gen_params.h
--rw-r--r--   0 runner     (501) staff       (20)     4762 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/circuit_gen_params.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     7920 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_color_code.cc
--rw-r--r--   0 runner     (501) staff       (20)      256 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_color_code.h
--rw-r--r--   0 runner     (501) staff       (20)     4373 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_color_code.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     3753 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_rep_code.cc
--rw-r--r--   0 runner     (501) staff       (20)      250 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_rep_code.h
--rw-r--r--   0 runner     (501) staff       (20)     2356 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_rep_code.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    13501 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_surface_code.cc
--rw-r--r--   0 runner     (501) staff       (20)      262 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_surface_code.h
--rw-r--r--   0 runner     (501) staff       (20)     9269 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/gen/gen_surface_code.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    46890 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/help.cc
--rw-r--r--   0 runner     (501) staff       (20)      808 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/help.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.394611 stim-1.9.dev1656756326/src/stim/io/
--rw-r--r--   0 runner     (501) staff       (20)     1735 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record.cc
--rw-r--r--   0 runner     (501) staff       (20)     2117 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record.h
--rw-r--r--   0 runner     (501) staff       (20)     1377 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4259 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_batch.cc
--rw-r--r--   0 runner     (501) staff       (20)     3858 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_batch.h
--rw-r--r--   0 runner     (501) staff       (20)     2210 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_batch.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     3508 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_batch_writer.cc
--rw-r--r--   0 runner     (501) staff       (20)     2859 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_batch_writer.h
--rw-r--r--   0 runner     (501) staff       (20)     1276 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_batch_writer.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    13034 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_reader.cc
--rw-r--r--   0 runner     (501) staff       (20)    14427 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_reader.h
--rw-r--r--   0 runner     (501) staff       (20)     4085 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_reader.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    24778 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_reader.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     8042 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_writer.cc
--rw-r--r--   0 runner     (501) staff       (20)     4038 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_writer.h
--rw-r--r--   0 runner     (501) staff       (20)    14152 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/measure_record_writer.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1218 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/raii_file.cc
--rw-r--r--   0 runner     (501) staff       (20)      899 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/raii_file.h
--rw-r--r--   0 runner     (501) staff       (20)    16114 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/read_write.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1163 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/read_write.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     1409 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/sparse_shot.cc
--rw-r--r--   0 runner     (501) staff       (20)     1325 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/sparse_shot.h
--rw-r--r--   0 runner     (501) staff       (20)     1350 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/sparse_shot.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    16245 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/stim_data_formats.cc
--rw-r--r--   0 runner     (501) staff       (20)      558 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/io/stim_data_formats.h
--rw-r--r--   0 runner     (501) staff       (20)    13925 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/main_namespaced.cc
--rw-r--r--   0 runner     (501) staff       (20)      822 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/main_namespaced.h
--rw-r--r--   0 runner     (501) staff       (20)     5958 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/main_namespaced.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    23484 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/main_namespaced.test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.411879 stim-1.9.dev1656756326/src/stim/mem/
--rw-r--r--   0 runner     (501) staff       (20)      772 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/bit_ref.cc
--rw-r--r--   0 runner     (501) staff       (20)     2520 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/bit_ref.h
--rw-r--r--   0 runner     (501) staff       (20)     2434 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/bit_ref.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4103 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/fixed_cap_vector.h
--rw-r--r--   0 runner     (501) staff       (20)     3256 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/fixed_cap_vector.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     6232 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/monotonic_buffer.h
--rw-r--r--   0 runner     (501) staff       (20)     1486 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/monotonic_buffer.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     5590 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/pointer_range.h
--rw-r--r--   0 runner     (501) staff       (20)    10193 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.cc
--rw-r--r--   0 runner     (501) staff       (20)     7148 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.h
--rw-r--r--   0 runner     (501) staff       (20)     1215 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     6374 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4564 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits.cc
--rw-r--r--   0 runner     (501) staff       (20)     6109 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits.h
--rw-r--r--   0 runner     (501) staff       (20)     1340 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     8004 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     3921 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits_range_ref.cc
--rw-r--r--   0 runner     (501) staff       (20)    12929 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits_range_ref.h
--rw-r--r--   0 runner     (501) staff       (20)    10063 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_bits_range_ref.test.cc
--rw-r--r--   0 runner     (501) staff       (20)      623 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat.cc
--rw-r--r--   0 runner     (501) staff       (20)      831 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat.h
--rw-r--r--   0 runner     (501) staff       (20)     1254 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     2541 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     3658 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat_avx2.h
--rw-r--r--   0 runner     (501) staff       (20)     4289 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat_polyfill.h
--rw-r--r--   0 runner     (501) staff       (20)     3485 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_compat_sse2.h
--rw-r--r--   0 runner     (501) staff       (20)     1522 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_util.cc
--rw-r--r--   0 runner     (501) staff       (20)     1519 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_util.h
--rw-r--r--   0 runner     (501) staff       (20)     5551 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/simd_util.test.cc
--rw-r--r--   0 runner     (501) staff       (20)      633 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.cc
--rw-r--r--   0 runner     (501) staff       (20)     6646 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.h
--rw-r--r--   0 runner     (501) staff       (20)     1355 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     6750 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4622 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/probability_util.cc
--rw-r--r--   0 runner     (501) staff       (20)     2196 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/probability_util.h
--rw-r--r--   0 runner     (501) staff       (20)     2881 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/probability_util.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     2460 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/probability_util.test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.416576 stim-1.9.dev1656756326/src/stim/py/
--rw-r--r--   0 runner     (501) staff       (20)     3511 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/base.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1720 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/base.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    12498 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/compiled_detector_sampler.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     2182 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/compiled_detector_sampler.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    11708 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/compiled_measurement_sampler.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     2038 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/compiled_measurement_sampler.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     1655 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/march.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)      210 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/march.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     9912 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/py/stim.pybind.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.417075 stim-1.9.dev1656756326/src/stim/search/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.424801 stim-1.9.dev1656756326/src/stim/search/graphlike/
--rw-r--r--   0 runner     (501) staff       (20)     3666 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/algo.cc
--rw-r--r--   0 runner     (501) staff       (20)     1883 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/algo.h
--rw-r--r--   0 runner     (501) staff       (20)     1520 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/algo.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)     5967 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/algo.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1598 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/edge.cc
--rw-r--r--   0 runner     (501) staff       (20)     1173 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/edge.h
--rw-r--r--   0 runner     (501) staff       (20)     1299 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/edge.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4535 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/graph.cc
--rw-r--r--   0 runner     (501) staff       (20)     1664 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/graph.h
--rw-r--r--   0 runner     (501) staff       (20)     5946 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/graph.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1247 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/node.cc
--rw-r--r--   0 runner     (501) staff       (20)     1241 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/node.h
--rw-r--r--   0 runner     (501) staff       (20)     1214 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/node.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     3824 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/search_state.cc
--rw-r--r--   0 runner     (501) staff       (20)     1717 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/search_state.h
--rw-r--r--   0 runner     (501) staff       (20)     5135 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/graphlike/search_state.test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.432382 stim-1.9.dev1656756326/src/stim/search/hyper/
--rw-r--r--   0 runner     (501) staff       (20)     4075 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/algo.cc
--rw-r--r--   0 runner     (501) staff       (20)     3726 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/algo.h
--rw-r--r--   0 runner     (501) staff       (20)     6614 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/algo.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1780 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/edge.cc
--rw-r--r--   0 runner     (501) staff       (20)     1145 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/edge.h
--rw-r--r--   0 runner     (501) staff       (20)     1220 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/edge.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2764 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/graph.cc
--rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/graph.h
--rw-r--r--   0 runner     (501) staff       (20)     3834 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/graph.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1187 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/node.cc
--rw-r--r--   0 runner     (501) staff       (20)     1061 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/node.h
--rw-r--r--   0 runner     (501) staff       (20)     1202 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/node.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     2584 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/search_state.cc
--rw-r--r--   0 runner     (501) staff       (20)     1319 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/search_state.h
--rw-r--r--   0 runner     (501) staff       (20)     2764 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/hyper/search_state.test.cc
--rw-r--r--   0 runner     (501) staff       (20)      741 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/search/search.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.450869 stim-1.9.dev1656756326/src/stim/simulators/
--rw-r--r--   0 runner     (501) staff       (20)     8303 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/detection_simulator.cc
--rw-r--r--   0 runner     (501) staff       (20)     3491 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/detection_simulator.h
--rw-r--r--   0 runner     (501) staff       (20)    13068 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/detection_simulator.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    58776 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.cc
--rw-r--r--   0 runner     (501) staff       (20)    19400 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.h
--rw-r--r--   0 runner     (501) staff       (20)     2487 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    93794 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    13244 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_matcher.cc
--rw-r--r--   0 runner     (501) staff       (20)     4113 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_matcher.h
--rw-r--r--   0 runner     (501) staff       (20)    12959 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/error_matcher.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    22561 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.cc
--rw-r--r--   0 runner     (501) staff       (20)     6766 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.h
--rw-r--r--   0 runner     (501) staff       (20)     3090 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    35644 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    14238 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/matched_error.cc
--rw-r--r--   0 runner     (501) staff       (20)     7006 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/matched_error.h
--rw-r--r--   0 runner     (501) staff       (20)    23934 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/matched_error.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)      774 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/matched_error.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)     8918 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/matched_error.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    12594 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.cc
--rw-r--r--   0 runner     (501) staff       (20)     5802 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.h
--rw-r--r--   0 runner     (501) staff       (20)    17795 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     2894 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    17916 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.test.cc
--rw-r--r--   0 runner     (501) staff       (20)    38340 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.cc
--rw-r--r--   0 runner     (501) staff       (20)    14965 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.h
--rw-r--r--   0 runner     (501) staff       (20)     1192 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    52297 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1014 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    65265 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     8122 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/vector_simulator.cc
--rw-r--r--   0 runner     (501) staff       (20)     3151 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/vector_simulator.h
--rw-r--r--   0 runner     (501) staff       (20)     9602 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/simulators/vector_simulator.test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.459754 stim-1.9.dev1656756326/src/stim/stabilizers/
--rw-r--r--   0 runner     (501) staff       (20)     4476 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.cc
--rw-r--r--   0 runner     (501) staff       (20)     4282 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.h
--rw-r--r--   0 runner     (501) staff       (20)     1513 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    30578 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)     1991 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    11945 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     4715 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string_ref.cc
--rw-r--r--   0 runner     (501) staff       (20)     5004 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string_ref.h
--rw-r--r--   0 runner     (501) staff       (20)    22011 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau.cc
--rw-r--r--   0 runner     (501) staff       (20)     8555 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau.h
--rw-r--r--   0 runner     (501) staff       (20)     1599 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau.perf.cc
--rw-r--r--   0 runner     (501) staff       (20)    41401 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau.pybind.cc
--rw-r--r--   0 runner     (501) staff       (20)      757 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau.pybind.h
--rw-r--r--   0 runner     (501) staff       (20)    42286 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     5334 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau_specialized_prepend.cc
--rw-r--r--   0 runner     (501) staff       (20)     4495 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau_transposed_raii.cc
--rw-r--r--   0 runner     (501) staff       (20)     1925 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/stabilizers/tableau_transposed_raii.h
--rw-r--r--   0 runner     (501) staff       (20)     1601 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/str_util.h
--rw-r--r--   0 runner     (501) staff       (20)     1076 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/str_util.test.cc
--rw-r--r--   0 runner     (501) staff       (20)     1641 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/test_util.test.cc
--rw-r--r--   0 runner     (501) staff       (20)      957 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim/test_util.test.h
--rw-r--r--   0 runner     (501) staff       (20)      614 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim.cc
--rw-r--r--   0 runner     (501) staff       (20)     2329 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim.h
--rw-r--r--   0 runner     (501) staff       (20)      925 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim.test.cc
--rw-r--r--   0 runner     (501) staff       (20)      798 2022-07-02 10:07:05.000000 stim-1.9.dev1656756326/src/stim_included_twice.test.cc
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-02 10:29:34.462625 stim-1.9.dev1656756326/stim.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     4190 2022-07-02 10:29:34.000000 stim-1.9.dev1656756326/stim.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     8665 2022-07-02 10:29:34.000000 stim-1.9.dev1656756326/stim.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-02 10:29:34.000000 stim-1.9.dev1656756326/stim.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       52 2022-07-02 10:29:34.000000 stim-1.9.dev1656756326/stim.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2022-07-02 10:29:34.000000 stim-1.9.dev1656756326/stim.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        5 2022-07-02 10:29:34.000000 stim-1.9.dev1656756326/stim.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.679581 stim-1.9.dev1657429876/
+-rw-r--r--   0 runner     (501) staff       (20)    11357 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      103 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     4208 2022-07-10 05:33:53.678445 stim-1.9.dev1657429876/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3846 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.486415 stim-1.9.dev1657429876/glue/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.493692 stim-1.9.dev1657429876/glue/python/
+-rw-r--r--   0 runner     (501) staff       (20)     3846 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/glue/python/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.486935 stim-1.9.dev1657429876/glue/python/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.496379 stim-1.9.dev1657429876/glue/python/src/stim/
+-rw-r--r--   0 runner     (501) staff       (20)     2357 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/glue/python/src/stim/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)   204702 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/glue/python/src/stim/__init__.pyi
+-rw-r--r--   0 runner     (501) staff       (20)      134 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/glue/python/src/stim/_main_argv.py
+-rw-r--r--   0 runner     (501) staff       (20)      109 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-10 05:33:53.679733 stim-1.9.dev1657429876/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3667 2022-07-10 05:11:44.000000 stim-1.9.dev1657429876/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.499211 stim-1.9.dev1657429876/src/
+-rw-r--r--   0 runner     (501) staff       (20)      701 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/main.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.510907 stim-1.9.dev1657429876/src/stim/
+-rw-r--r--   0 runner     (501) staff       (20)    10123 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/arg_parse.cc
+-rw-r--r--   0 runner     (501) staff       (20)     9242 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/arg_parse.h
+-rw-r--r--   0 runner     (501) staff       (20)    11209 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/arg_parse.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6036 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/benchmark_main.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)      627 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/benchmark_util.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3973 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/benchmark_util.perf.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.529210 stim-1.9.dev1657429876/src/stim/circuit/
+-rw-r--r--   0 runner     (501) staff       (20)    47320 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.cc
+-rw-r--r--   0 runner     (501) staff       (20)    15456 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.h
+-rw-r--r--   0 runner     (501) staff       (20)     1431 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    74455 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    36126 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      977 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit.test.h
+-rw-r--r--   0 runner     (501) staff       (20)     5342 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit_gate_target.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      996 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit_gate_target.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     5902 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit_instruction.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1668 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit_instruction.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     4617 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit_repeat_block.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1155 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/circuit_repeat_block.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     5472 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data.cc
+-rw-r--r--   0 runner     (501) staff       (20)     9837 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data.h
+-rw-r--r--   0 runner     (501) staff       (20)     1198 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3280 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13456 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_annotations.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2093 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_blocks.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14084 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_collapsing.cc
+-rw-r--r--   0 runner     (501) staff       (20)    10531 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_controlled.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3221 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_hada.cc
+-rw-r--r--   0 runner     (501) staff       (20)    11977 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_noisy.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3588 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_pauli.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2483 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_period_3.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5635 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_period_4.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6624 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_pp.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3517 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_data_swaps.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5748 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_target.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2307 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_target.h
+-rw-r--r--   0 runner     (501) staff       (20)     6040 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/circuit/gate_target.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.535206 stim-1.9.dev1657429876/src/stim/dem/
+-rw-r--r--   0 runner     (501) staff       (20)    31371 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7894 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model.h
+-rw-r--r--   0 runner     (501) staff       (20)    36713 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      901 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    25490 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8077 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model_instruction.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1437 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model_instruction.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     3686 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model_repeat_block.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1159 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model_repeat_block.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     8395 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model_target.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1221 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/dem/detector_error_model_target.pybind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.542345 stim-1.9.dev1657429876/src/stim/gen/
+-rw-r--r--   0 runner     (501) staff       (20)     2887 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/circuit_gen_main.cc
+-rw-r--r--   0 runner     (501) staff       (20)      249 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/circuit_gen_main.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/circuit_gen_main.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4061 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/circuit_gen_params.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/circuit_gen_params.h
+-rw-r--r--   0 runner     (501) staff       (20)     4762 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/circuit_gen_params.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7920 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_color_code.cc
+-rw-r--r--   0 runner     (501) staff       (20)      256 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_color_code.h
+-rw-r--r--   0 runner     (501) staff       (20)     4373 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_color_code.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3753 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_rep_code.cc
+-rw-r--r--   0 runner     (501) staff       (20)      250 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_rep_code.h
+-rw-r--r--   0 runner     (501) staff       (20)     2356 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_rep_code.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13501 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_surface_code.cc
+-rw-r--r--   0 runner     (501) staff       (20)      262 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_surface_code.h
+-rw-r--r--   0 runner     (501) staff       (20)     9269 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/gen/gen_surface_code.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    46890 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/help.cc
+-rw-r--r--   0 runner     (501) staff       (20)      808 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/help.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.556611 stim-1.9.dev1657429876/src/stim/io/
+-rw-r--r--   0 runner     (501) staff       (20)     1735 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2117 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record.h
+-rw-r--r--   0 runner     (501) staff       (20)     1377 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4259 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_batch.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3858 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_batch.h
+-rw-r--r--   0 runner     (501) staff       (20)     2210 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_batch.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3508 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_batch_writer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2859 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_batch_writer.h
+-rw-r--r--   0 runner     (501) staff       (20)     1276 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_batch_writer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13034 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_reader.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14427 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_reader.h
+-rw-r--r--   0 runner     (501) staff       (20)     4085 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_reader.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    24778 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_reader.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8042 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_writer.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4038 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_writer.h
+-rw-r--r--   0 runner     (501) staff       (20)    14152 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/measure_record_writer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/raii_file.cc
+-rw-r--r--   0 runner     (501) staff       (20)      899 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/raii_file.h
+-rw-r--r--   0 runner     (501) staff       (20)    16178 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/read_write.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1163 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/read_write.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     1409 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/sparse_shot.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1325 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/sparse_shot.h
+-rw-r--r--   0 runner     (501) staff       (20)     1350 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/sparse_shot.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    16245 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/stim_data_formats.cc
+-rw-r--r--   0 runner     (501) staff       (20)      558 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/io/stim_data_formats.h
+-rw-r--r--   0 runner     (501) staff       (20)    13925 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/main_namespaced.cc
+-rw-r--r--   0 runner     (501) staff       (20)      822 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/main_namespaced.h
+-rw-r--r--   0 runner     (501) staff       (20)     5958 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/main_namespaced.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    23484 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/main_namespaced.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.577181 stim-1.9.dev1657429876/src/stim/mem/
+-rw-r--r--   0 runner     (501) staff       (20)      772 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/bit_ref.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/bit_ref.h
+-rw-r--r--   0 runner     (501) staff       (20)     2434 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/bit_ref.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4103 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/fixed_cap_vector.h
+-rw-r--r--   0 runner     (501) staff       (20)     3256 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/fixed_cap_vector.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6232 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/monotonic_buffer.h
+-rw-r--r--   0 runner     (501) staff       (20)     1486 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/monotonic_buffer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5590 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/pointer_range.h
+-rw-r--r--   0 runner     (501) staff       (20)    10193 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7148 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.h
+-rw-r--r--   0 runner     (501) staff       (20)     1215 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6374 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4564 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6109 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits.h
+-rw-r--r--   0 runner     (501) staff       (20)     1340 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8004 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3921 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits_range_ref.cc
+-rw-r--r--   0 runner     (501) staff       (20)    12929 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits_range_ref.h
+-rw-r--r--   0 runner     (501) staff       (20)    10063 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_bits_range_ref.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      623 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat.cc
+-rw-r--r--   0 runner     (501) staff       (20)      831 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat.h
+-rw-r--r--   0 runner     (501) staff       (20)     1254 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2541 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3658 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat_avx2.h
+-rw-r--r--   0 runner     (501) staff       (20)     4289 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat_polyfill.h
+-rw-r--r--   0 runner     (501) staff       (20)     3485 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_compat_sse2.h
+-rw-r--r--   0 runner     (501) staff       (20)     1522 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_util.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1519 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     5551 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/simd_util.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      633 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6646 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.h
+-rw-r--r--   0 runner     (501) staff       (20)     1355 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6750 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4622 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/probability_util.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2196 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/probability_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     2881 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/probability_util.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2460 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/probability_util.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.581599 stim-1.9.dev1657429876/src/stim/py/
+-rw-r--r--   0 runner     (501) staff       (20)     3511 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/base.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1720 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/base.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    12489 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/compiled_detector_sampler.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2182 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/compiled_detector_sampler.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    11714 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/compiled_measurement_sampler.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2038 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/compiled_measurement_sampler.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     1655 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/march.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      210 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/march.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    10346 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/py/stim.pybind.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.582041 stim-1.9.dev1657429876/src/stim/search/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.590213 stim-1.9.dev1657429876/src/stim/search/graphlike/
+-rw-r--r--   0 runner     (501) staff       (20)     3666 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/algo.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1883 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/algo.h
+-rw-r--r--   0 runner     (501) staff       (20)     1520 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/algo.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5967 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/algo.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1598 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/edge.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/edge.h
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/edge.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4535 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/graph.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1664 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/graph.h
+-rw-r--r--   0 runner     (501) staff       (20)     5946 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/graph.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1247 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/node.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1241 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/node.h
+-rw-r--r--   0 runner     (501) staff       (20)     1214 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/node.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3824 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/search_state.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1717 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/search_state.h
+-rw-r--r--   0 runner     (501) staff       (20)     5135 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/graphlike/search_state.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.600026 stim-1.9.dev1657429876/src/stim/search/hyper/
+-rw-r--r--   0 runner     (501) staff       (20)     4075 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/algo.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3726 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/algo.h
+-rw-r--r--   0 runner     (501) staff       (20)     6614 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/algo.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1780 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/edge.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1145 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/edge.h
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/edge.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2764 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/graph.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/graph.h
+-rw-r--r--   0 runner     (501) staff       (20)     3834 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/graph.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1187 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/node.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1061 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/node.h
+-rw-r--r--   0 runner     (501) staff       (20)     1202 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/node.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2584 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/search_state.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1319 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/search_state.h
+-rw-r--r--   0 runner     (501) staff       (20)     2764 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/hyper/search_state.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      741 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/search/search.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.624861 stim-1.9.dev1657429876/src/stim/simulators/
+-rw-r--r--   0 runner     (501) staff       (20)     8303 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/detection_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3491 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/detection_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)    13068 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/detection_simulator.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    58776 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.cc
+-rw-r--r--   0 runner     (501) staff       (20)    19400 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.h
+-rw-r--r--   0 runner     (501) staff       (20)     2487 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    93794 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    13244 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_matcher.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4113 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_matcher.h
+-rw-r--r--   0 runner     (501) staff       (20)    12959 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/error_matcher.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    22561 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)     6766 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)     3090 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    35644 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14238 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/matched_error.cc
+-rw-r--r--   0 runner     (501) staff       (20)     7006 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/matched_error.h
+-rw-r--r--   0 runner     (501) staff       (20)    23934 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/matched_error.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      774 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/matched_error.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)     8918 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/matched_error.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    12594 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5802 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.h
+-rw-r--r--   0 runner     (501) staff       (20)    17724 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2894 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    17916 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)    38340 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)    14965 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)     1192 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    56623 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1014 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    65265 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8122 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/vector_simulator.cc
+-rw-r--r--   0 runner     (501) staff       (20)     3151 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/vector_simulator.h
+-rw-r--r--   0 runner     (501) staff       (20)     9602 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/simulators/vector_simulator.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.674483 stim-1.9.dev1657429876/src/stim/stabilizers/
+-rw-r--r--   0 runner     (501) staff       (20)     4476 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4282 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.h
+-rw-r--r--   0 runner     (501) staff       (20)     1513 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    30578 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1991 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    11945 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4715 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string_ref.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5004 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string_ref.h
+-rw-r--r--   0 runner     (501) staff       (20)    22011 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau.cc
+-rw-r--r--   0 runner     (501) staff       (20)     8555 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau.h
+-rw-r--r--   0 runner     (501) staff       (20)     1599 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau.perf.cc
+-rw-r--r--   0 runner     (501) staff       (20)    41497 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau.pybind.cc
+-rw-r--r--   0 runner     (501) staff       (20)      757 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau.pybind.h
+-rw-r--r--   0 runner     (501) staff       (20)    42286 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     5334 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau_specialized_prepend.cc
+-rw-r--r--   0 runner     (501) staff       (20)     4495 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau_transposed_raii.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1925 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/stabilizers/tableau_transposed_raii.h
+-rw-r--r--   0 runner     (501) staff       (20)     1601 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/str_util.h
+-rw-r--r--   0 runner     (501) staff       (20)     1076 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/str_util.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)     1641 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/test_util.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      957 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim/test_util.test.h
+-rw-r--r--   0 runner     (501) staff       (20)      614 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim.cc
+-rw-r--r--   0 runner     (501) staff       (20)     2329 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim.h
+-rw-r--r--   0 runner     (501) staff       (20)      925 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim.test.cc
+-rw-r--r--   0 runner     (501) staff       (20)      798 2022-07-10 05:11:43.000000 stim-1.9.dev1657429876/src/stim_included_twice.test.cc
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-10 05:33:53.677970 stim-1.9.dev1657429876/stim.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     4208 2022-07-10 05:33:53.000000 stim-1.9.dev1657429876/stim.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8665 2022-07-10 05:33:53.000000 stim-1.9.dev1657429876/stim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-10 05:33:53.000000 stim-1.9.dev1657429876/stim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       52 2022-07-10 05:33:53.000000 stim-1.9.dev1657429876/stim.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2022-07-10 05:33:53.000000 stim-1.9.dev1657429876/stim.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2022-07-10 05:33:53.000000 stim-1.9.dev1657429876/stim.egg-info/top_level.txt
```

### Comparing `stim-1.9.dev1656756326/LICENSE` & `stim-1.9.dev1657429876/LICENSE`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/PKG-INFO` & `stim-1.9.dev1657429876/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stim
-Version: 1.9.dev1656756326
-Summary: A fast quantum stabilizer circuit simulator.
+Version: 1.9.dev1657429876
+Summary: A fast library for analyzing with quantum stabilizer circuits.
 Home-page: https://github.com/quantumlib/stim
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `stim-1.9.dev1656756326/README.md` & `stim-1.9.dev1657429876/README.md`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/glue/python/README.md` & `stim-1.9.dev1657429876/glue/python/README.md`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/glue/python/src/stim/__init__.py` & `stim-1.9.dev1657429876/glue/python/src/stim/__init__.py`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/glue/python/src/stim/__init__.pyi` & `stim-1.9.dev1657429876/glue/python/src/stim/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
     Examples:
         >>> import stim
         >>> c = stim.Circuit()
         >>> c.append("X", 0)
         >>> c.append("M", 0)
         >>> c.compile_sampler().sample(shots=1)
-        array([[1]], dtype=uint8)
+        array([[ True]])
 
         >>> stim.Circuit('''
         ...    H 0
         ...    CNOT 0 1
         ...    M 0 1
         ...    DETECTOR rec[-1] rec[-2]
         ... ''').compile_detector_sampler().sample(shots=1)
-        array([[0]], dtype=uint8)
+        array([[False]])
 
     """
     def __add__(self, second: stim.Circuit) -> stim.Circuit:
         """Creates a circuit by appending two circuits.
 
         Examples:
             >>> import stim
@@ -400,15 +400,15 @@
             ...    H 0
             ...    CNOT 0 1
             ...    M 0 1
             ...    DETECTOR rec[-1] rec[-2]
             ... ''')
             >>> s = c.compile_detector_sampler()
             >>> s.sample(shots=1)
-            array([[0]], dtype=uint8)
+            array([[False]])
         """
     def compile_m2d_converter(self, *, skip_reference_sample: bool = False) -> stim.CompiledMeasurementsToDetectionEventsConverter:
         """Returns an object that can efficiently convert measurements into detection events for the given circuit.
 
         The converter uses a noiseless reference sample, collected from the circuit using stim's Tableau simulator
         during initialization of the converter, as a baseline for determining what the expected value of a detector
         is.
@@ -481,15 +481,15 @@
             >>> import stim
             >>> c = stim.Circuit('''
             ...    X 2
             ...    M 0 1 2
             ... ''')
             >>> s = c.compile_sampler()
             >>> s.sample(shots=1)
-            array([[0, 0, 1]], dtype=uint8)
+            array([[False, False,  True]])
         """
     def copy(self) -> stim.Circuit:
         """Returns a copy of the circuit. An independent circuit with the same contents.
 
         Examples:
             >>> import stim
 
@@ -626,15 +626,15 @@
         Returns:
             A `stim.Circuit` with the same instructions in the same order,
             but with loops flattened into repeated instructions and with
             all coordinate shifts inlined.
 
         Examples:
             >>> import stim
-            >>> circuit = stim.Circuit('''
+            >>> stim.Circuit('''
             ...     REPEAT 5 {
             ...         MR 0 1
             ...         DETECTOR(0, 0) rec[-2]
             ...         DETECTOR(1, 0) rec[-1]
             ...         SHIFT_COORDS(0, 1)
             ...     }
             ... ''').flattened()
@@ -1063,28 +1063,26 @@
             >>> import tempfile
             >>> c = stim.Circuit('H 5\nX 0')
 
             >>> with tempfile.TemporaryDirectory() as tmpdir:
             ...     path = tmpdir + '/tmp.stim'
             ...     with open(path, 'w') as f:
             ...         c.to_file(f)
-            ...     with open(path, 'w') as f:
+            ...     with open(path) as f:
             ...         contents = f.read()
             >>> contents
-            H 5
-            X 0
+            'H 5\nX 0\n'
 
             >>> with tempfile.TemporaryDirectory() as tmpdir:
             ...     path = tmpdir + '/tmp.stim'
             ...     c.to_file(path)
-            ...     with open(path, 'w') as f:
+            ...     with open(path) as f:
             ...         contents = f.read()
             >>> contents
-            H 5
-            X 0
+            'H 5\nX 0\n'
         """
     def without_noise(self) -> stim.Circuit:
         """Returns a copy of the circuit with all noise processes removed.
 
         Pure noise instructions, such as X_ERROR and DEPOLARIZE2, are not
         included in the result.
 
@@ -1093,21 +1091,21 @@
 
         Returns:
             A `stim.Circuit` with the same instructions except all noise
             processes have been removed.
 
         Examples:
             >>> import stim
-            >>> circuit = stim.Circuit('''
+            >>> stim.Circuit('''
             ...     X_ERROR(0.25) 0
             ...     CNOT 0 1
             ...     M(0.125) 0
             ... ''').without_noise()
             stim.Circuit('''
-                CNOT 0 1
+                CX 0 1
                 M 0
             ''')
         """
 class CircuitErrorLocation:
     """Describes the location of an error mechanism from a stim circuit.
     """
     def __init__(self, *, tick_offset: int, flipped_pauli_product: List[stim.GateTargetWithCoords], flipped_measurement: object, instruction_targets: stim.CircuitTargetsInsideInstruction, stack_frames: List[stim.CircuitErrorLocationStackFrame]) -> None:
@@ -1368,15 +1366,15 @@
             ...    CNOT 0 1
             ...    X_ERROR(1.0) 0
             ...    M 0 1
             ...    DETECTOR rec[-1] rec[-2]
             ... ''')
             >>> s = c.compile_detector_sampler()
             >>> s.sample(shots=1)
-            array([[1]], dtype=uint8)
+            array([[ True]])
         """
     def __repr__(self) -> str:
         """Returns text that is a valid python expression evaluating to an equivalent `stim.CompiledDetectorSampler`.
         """
     def sample(self, shots: int, *, prepend_observables: bool = False, append_observables: bool = False) -> np.ndarray[bool]:
         """Returns a numpy array containing a batch of detector samples from the circuit.
 
@@ -1504,15 +1502,15 @@
             >>> import stim
             >>> c = stim.Circuit('''
             ...    X 0   2 3
             ...    M 0 1 2 3
             ... ''')
             >>> s = c.compile_sampler()
             >>> s.sample(shots=1)
-            array([[1, 0, 1, 1]], dtype=uint8)
+            array([[ True, False,  True,  True]])
         """
     def __repr__(self) -> str:
         """Returns text that is a valid python expression evaluating to an equivalent `stim.CompiledMeasurementSampler`.
         """
     def sample(self, shots: int) -> np.ndarray[bool]:
         """Returns a numpy array containing a batch of measurement samples from the circuit.
 
@@ -1520,15 +1518,15 @@
             >>> import stim
             >>> c = stim.Circuit('''
             ...    X 0   2 3
             ...    M 0 1 2 3
             ... ''')
             >>> s = c.compile_sampler()
             >>> s.sample(shots=1)
-            array([[1, 0, 1, 1]], dtype=uint8)
+            array([[ True, False,  True,  True]])
 
         Args:
             shots: The number of times to sample every measurement in the circuit.
 
         Returns:
             A numpy array with `dtype=uint8` and `shape=(shots, num_measurements)`.
             The bit for measurement `m` in shot `s` is at `result[s, m]`.
@@ -1679,23 +1677,21 @@
             ...                            [1, 0]], dtype=np.bool8),
             ...     separate_observables=True,
             ... )
             >>> dets
             array([[False, False],
                    [False, False],
                    [False, False],
-                   [ True, False],
-                   [False, False],
+                   [False,  True],
                    [False, False]])
             >>> obs
             array([[False],
                    [False],
                    [False],
                    [ True],
-                   [False],
                    [False]])
         """
     def convert_file(self, *, measurements_filepath: str, measurements_format: str = '01', sweep_bits_filepath: str = None, sweep_bits_format: str = '01', detection_events_filepath: str, detection_events_format: str = '01', append_observables: bool = False, obs_out_filepath: str = None, obs_out_format: str = '01') -> None:
         """Reads measurement data from a file, converts it, and writes the detection events to another file.
 
         Args:
             measurements_filepath: A file containing measurement data to be converted.
@@ -2536,26 +2532,26 @@
             >>> import tempfile
             >>> c = stim.DetectorErrorModel('error(0.25) D2 D3')
 
             >>> with tempfile.TemporaryDirectory() as tmpdir:
             ...     path = tmpdir + '/tmp.stim'
             ...     with open(path, 'w') as f:
             ...         c.to_file(f)
-            ...     with open(path, 'w') as f:
+            ...     with open(path) as f:
             ...         contents = f.read()
             >>> contents
-            error(0.25) D2 D3
+            'error(0.25) D2 D3\n'
 
             >>> with tempfile.TemporaryDirectory() as tmpdir:
             ...     path = tmpdir + '/tmp.stim'
             ...     c.to_file(path)
-            ...     with open(path, 'w') as f:
+            ...     with open(path) as f:
             ...         contents = f.read()
             >>> contents
-            error(0.25) D2 D3
+            'error(0.25) D2 D3\n'
         """
 class ExplainedError:
     """Describes the location of an error mechanism from a stim circuit.
     """
     def __init__(self, *, dem_error_terms: List[stim.DemTargetWithCoords], circuit_error_locations: List[stim.CircuitErrorLocation]) -> None:
         """Creates a stim.ExplainedError.
         """
@@ -3716,15 +3712,16 @@
             >>> t1 = stim.Tableau.random(4)
             >>> t2 = stim.Tableau.random(4)
             >>> t3 = t1.then(t2)
             >>> p = stim.PauliString.random(4)
             >>> t3(p) == t2(t1(p))
             True
         """
-    def to_unitary_matrix(self, *, endian: str) -> np.ndarray[np.float32]:
+    def to_unitary_matrix(self, *, endian: str) -> np.ndarray[np.complex64]:
+
         """Converts the tableau into a unitary matrix.
 
         Args:
             endian:
                 "little": The first qubit is the least significant (corresponds
                     to an offset of 1 in the state vector).
                 "big": The first qubit is the most significant (corresponds
@@ -3930,14 +3927,26 @@
             ],
             zs=[
                 stim.PauliString("+X_"),
                 stim.PauliString("+XZ"),
             ],
         )
     """
+    def c_xyz(self, *targets) -> None:
+        """Applies a C_XYZ gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+        """
+    def c_zyx(self, *targets) -> None:
+        """Applies a C_ZYX gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+        """
     def canonical_stabilizers(self) -> List[stim.PauliString]:
         """Returns a list of the stabilizers of the simulator's current state in a standard form.
 
         Two simulators have the same canonical stabilizers if and only if their current quantum state is equal
         (and tracking the same number of qubits).
 
         The canonical form is computed as follows:
@@ -4055,14 +4064,22 @@
             >>> s.do(stim.Circuit("M 0"))
             >>> s.current_measurement_record()
             [False, True, True]
 
         Returns:
             A list of booleans containing the result of every measurement performed by the simulator so far.
         """
+    def cx(self, *targets) -> None:
+        """Applies a controlled X gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+                Applies the gate to the first two targets, then the next two targets, and so forth.
+                There must be an even number of targets.
+        """
     def cy(self, *targets) -> None:
         """Applies a controlled Y gate to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
                 Applies the gate to the first two targets, then the next two targets, and so forth.
                 There must be an even number of targets.
@@ -4121,14 +4138,15 @@
     def do_pauli_string(self, pauli_string: stim.PauliString) -> None:
         """Applies the paulis from a pauli string to the simulator's state.
 
         Args:
             pauli_string: A stim.PauliString containing Paulis to apply.
 
         Examples:
+            >>> import stim
             >>> s = stim.TableauSimulator()
             >>> s.do_pauli_string(stim.PauliString("IXYZ"))
             >>> s.measure_many(0, 1, 2, 3)
             [False, True, True, False]
         """
     def do_tableau(self, tableau: stim.Tableau, targets: List[int]) -> None:
         """Applies a custom tableau operation to qubits in the simulator.
@@ -4141,15 +4159,15 @@
             targets: The indices of the qubits to operate on.
 
         Examples:
             >>> import stim
             >>> sim = stim.TableauSimulator()
             >>> sim.h(1)
             >>> sim.h_yz(2)
-            >>> [str(sim.peek_block(k)) for k in range(4)]
+            >>> [str(sim.peek_bloch(k)) for k in range(4)]
             ['+Z', '+X', '+Y', '+Z']
             >>> rot3 = stim.Tableau.from_conjugated_generators(
             ...     xs=[
             ...         stim.PauliString("_X_"),
             ...         stim.PauliString("__X"),
             ...         stim.PauliString("X__"),
             ...     ],
@@ -4157,33 +4175,39 @@
             ...         stim.PauliString("_Z_"),
             ...         stim.PauliString("__Z"),
             ...         stim.PauliString("Z__"),
             ...     ],
             ... )
 
             >>> sim.do_tableau(rot3, [1, 2, 3])
-            >>> [str(sim.peek_block(k)) for k in range(4)]
+            >>> [str(sim.peek_bloch(k)) for k in range(4)]
             ['+Z', '+Z', '+X', '+Y']
 
             >>> sim.do_tableau(rot3, [1, 2, 3])
-            >>> [str(sim.peek_block(k)) for k in range(4)]
+            >>> [str(sim.peek_bloch(k)) for k in range(4)]
             ['+Z', '+Y', '+Z', '+X']
         """
     def h(self, *targets) -> None:
         """Applies a Hadamard gate to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
         """
     def h_xy(self, *targets) -> None:
         """Applies a variant of the Hadamard gate that swaps the X and Y axes to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
         """
+    def h_xz(self, *targets) -> None:
+        """Applies a Hadamard gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+        """
     def h_yz(self, *targets) -> None:
         """Applies a variant of the Hadamard gate that swaps the Y and Z axes to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
         """
     def iswap(self, *targets) -> None:
@@ -4273,14 +4297,30 @@
 
         Args:
             *targets: The indices of the qubits to measure.
 
         Returns:
             The measurement results as a list of bools.
         """
+    @property
+    def num_qubits(self) -> int:
+        """Returns the number of qubits currently being tracked by the simulator's internal state.
+
+        Note that the number of qubits being tracked will implicitly increase if qubits beyond
+        the current limit are touched. Untracked qubits are always assumed to be in the |0> state.
+
+        Examples:
+            >>> import stim
+            >>> s = stim.TableauSimulator()
+            >>> s.num_qubits
+            0
+            >>> s.h(2)
+            >>> s.num_qubits
+            3
+        """
     def peek_bloch(self, target: int) -> stim.PauliString:
         """Returns the current bloch vector of the qubit, represented as a stim.PauliString.
 
         This is a non-physical operation. It reports information about the qubit without disturbing it.
 
         Args:
             target: The qubit to peek at.
@@ -4371,15 +4411,15 @@
             >>> s = stim.TableauSimulator()
             >>> s.reset_z(0)
             >>> s.peek_x(0)
             0
             >>> s.reset_x(0)
             >>> s.peek_x(0)
             1
-            >>> s.Z(0)
+            >>> s.z(0)
             >>> s.peek_x(0)
             -1
         """
     def peek_y(self, target: int) -> int:
         """Returns the expected value of a qubit's Y observable (which will always be -1, 0, or +1).
 
         This is a non-physical operation.
@@ -4398,15 +4438,15 @@
             >>> s = stim.TableauSimulator()
             >>> s.reset_z(0)
             >>> s.peek_y(0)
             0
             >>> s.reset_y(0)
             >>> s.peek_y(0)
             1
-            >>> s.Z(0)
+            >>> s.z(0)
             >>> s.peek_y(0)
             -1
         """
     def peek_z(self, target: int) -> int:
         """Returns the expected value of a qubit's Z observable (which will always be -1, 0, or +1).
 
         This is a non-physical operation.
@@ -4425,15 +4465,15 @@
             >>> s = stim.TableauSimulator()
             >>> s.reset_x(0)
             >>> s.peek_z(0)
             0
             >>> s.reset_z(0)
             >>> s.peek_z(0)
             1
-            >>> s.X(0)
+            >>> s.x(0)
             >>> s.peek_z(0)
             -1
         """
     def postselect_x(self, targets: Union[int, Iterable[int]], *, desired_value: bool) -> None:
 
         """Postselects qubits in the X basis, or raises an exception.
 
@@ -4498,58 +4538,58 @@
 
         Args:
             *targets: The indices of the qubits to reset.
 
         Example:
             >>> import stim
             >>> s = stim.TableauSimulator()
-            >>> s.X(0)
+            >>> s.x(0)
             >>> s.reset(0)
             >>> s.peek_bloch(0)
-            +Z
+            stim.PauliString("+Z")
         """
     def reset_x(self, *targets) -> None:
         """Resets qubits to the |+> state.
 
         Args:
             *targets: The indices of the qubits to reset.
 
         Example:
             >>> import stim
             >>> s = stim.TableauSimulator()
             >>> s.reset_x(0)
             >>> s.peek_bloch(0)
-            +X
+            stim.PauliString("+X")
         """
     def reset_y(self, *targets) -> None:
         """Resets qubits to the |i> state.
 
         Args:
             *targets: The indices of the qubits to reset.
 
         Example:
             >>> import stim
             >>> s = stim.TableauSimulator()
             >>> s.reset_y(0)
             >>> s.peek_bloch(0)
-            +Y
+            stim.PauliString("+Y")
         """
     def reset_z(self, *targets) -> None:
         """Resets qubits to the |0> state.
 
         Args:
             *targets: The indices of the qubits to reset.
 
         Example:
             >>> import stim
             >>> s = stim.TableauSimulator()
-            >>> s.H(0)
+            >>> s.h(0)
             >>> s.reset_z(0)
             >>> s.peek_bloch(0)
-            +Z
+            stim.PauliString("+Z")
         """
     def s(self, *targets) -> None:
         """Applies a SQRT_Z gate to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
         """
@@ -4630,15 +4670,16 @@
         """
     def sqrt_y_dag(self, *targets) -> None:
         """Applies a SQRT_Y_DAG gate to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
         """
-    def state_vector(self, *, endian: str = 'little') -> np.ndarray[np.float32]:
+    def state_vector(self, *, endian: str = 'little') -> np.ndarray[np.complex64]:
+
         """Returns a wavefunction that satisfies the stabilizers of the simulator's current state.
 
         This function takes O(n * 2**n) time and O(2**n) space, where n is the number of qubits. The computation is
         done by initialization a random state vector and iteratively projecting it into the +1 eigenspace of each
         stabilizer of the state. The state is then canonicalized so that zero values are actually exactly 0, and so
         that the first non-zero entry is positive.
 
@@ -4652,15 +4693,15 @@
         Returns:
             A `numpy.ndarray[numpy.complex64]` of computational basis amplitudes.
 
             If the result is in little endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
             the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_0, the
             qubit with index 1 is storing the bit b_1, etc.
 
-            If the result is in little endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
+            If the result is in big endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
             the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_{n-1}, the
             qubit with index 1 is storing the bit b_{n-2}, etc.
 
         Examples:
             >>> import stim
             >>> import numpy as np
             >>> s = stim.TableauSimulator()
@@ -4745,14 +4786,38 @@
         """
     def z(self, *targets) -> None:
         """Applies a Pauli Z gate to the simulator's state.
 
         Args:
             *targets: The indices of the qubits to target with the gate.
         """
+    def zcx(self, *targets) -> None:
+        """Applies a controlled X gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+                Applies the gate to the first two targets, then the next two targets, and so forth.
+                There must be an even number of targets.
+        """
+    def zcy(self, *targets) -> None:
+        """Applies a controlled Y gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+                Applies the gate to the first two targets, then the next two targets, and so forth.
+                There must be an even number of targets.
+        """
+    def zcz(self, *targets) -> None:
+        """Applies a controlled Z gate to the simulator's state.
+
+        Args:
+            *targets: The indices of the qubits to target with the gate.
+                Applies the gate to the first two targets, then the next two targets, and so forth.
+                There must be an even number of targets.
+        """
 def main(*, command_line_args: List[str]) -> int:
     """Runs the command line tool version of stim on the given arguments.
 
     Note that by default any input will be read from stdin, any output
     will print to stdout (as opposed to being intercepted). For most
     commands, you can use arguments like `--out` to write to a file
     instead of stdout and `--in` to read from a file instead of stdin.
@@ -4763,21 +4828,30 @@
     Raises:
         A large variety of errors, depending on what you are doing and
         how it failed! Beware that many errors are caught by the main
         method itself and printed to stderr, with the only indication
         that something went wrong being the return code.
 
     Example:
-        >>> stim.main(command_line_args=[
-        ...     "gen",
-        ...     "--code=repetition_code",
-        ...     "--task=memory",
-        ...     "--rounds=1000",
-        ...     "--distance=2",
-        ... ])
+        >>> import stim
+        >>> import tempfile
+        >>> with tempfile.TemporaryDirectory() as d:
+        ...     path = f'{d}/tmp.out'
+        ...     return_code = stim.main(command_line_args=[
+        ...         "gen",
+        ...         "--code=repetition_code",
+        ...         "--task=memory",
+        ...         "--rounds=1000",
+        ...         "--distance=2",
+        ...         "--out",
+        ...         path,
+        ...     ])
+        ...     assert return_code == 0
+        ...     with open(path) as f:
+        ...         print(f.read(), end='')
         # Generated repetition_code circuit.
         # task: memory
         # rounds: 1000
         # distance: 2
         # before_round_data_depolarization: 0
         # before_measure_flip_probability: 0
         # after_reset_flip_probability: 0
@@ -4840,25 +4914,25 @@
 
     Examples:
         >>> import stim
         >>> import pathlib
         >>> import tempfile
         >>> with tempfile.TemporaryDirectory() as d:
         ...     path = pathlib.Path(d) / 'shots'
-        ...     with open(path) as f:
+        ...     with open(path, 'w') as f:
         ...         print("0000", file=f)
         ...         print("0101", file=f)
         ...
         ...     read = stim.read_shot_data_file(
         ...         path=str(path),
         ...         format='01',
         ...         num_measurements=4)
         >>> read
-        [[False False False False]
-         [False  True False  True]]
+        array([[False, False, False, False],
+               [False,  True, False,  True]])
     """
 def target_combiner() -> stim.GateTarget:
     """Returns a target combiner (`*` in circuit files) that can be used as an operation target.
     """
 def target_inv(qubit_index: int) -> stim.GateTarget:
     """Returns a target flagged as inverted that can be passed into Circuit.append_operation
     For example, the '!1' in 'M 0 !1 2' is qubit 1 flagged as inverted,
@@ -4959,14 +5033,15 @@
             Note that this only refers to observables *in the given shot data*, not to
             observables from the original circuit that was sampled.
 
     Examples:
         >>> import stim
         >>> import pathlib
         >>> import tempfile
+        >>> import numpy as np
         >>> with tempfile.TemporaryDirectory() as d:
         ...     path = pathlib.Path(d) / 'shots'
         ...     shot_data = np.array([
         ...         [0, 1, 0],
         ...         [0, 1, 1],
         ...     ], dtype=np.bool8)
         ...
```

### Comparing `stim-1.9.dev1656756326/setup.py` & `stim-1.9.dev1657429876/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 MUX_SOURCE_FILES = glob.glob("src/**/march.pybind.cc", recursive=True)
 TEST_FILES = glob.glob("src/**/*.test.cc", recursive=True)
 PERF_FILES = glob.glob("src/**/*.perf.cc", recursive=True)
 MAIN_FILES = glob.glob("src/**/main.cc", recursive=True)
 HEADER_FILES = glob.glob("src/**/*.h", recursive=True)
 RELEVANT_SOURCE_FILES = sorted(set(ALL_SOURCE_FILES) - set(TEST_FILES + PERF_FILES + MAIN_FILES + MUX_SOURCE_FILES))
 
-version = '1.9.dev1656756326'
+version = '1.9.dev1657429876'
 
 common_compile_args = [
     '-std=c++11',
     '-fno-strict-aliasing',
     '-O3',
     '-g0',
     f'-DVERSION_INFO={version}',
@@ -87,15 +87,15 @@
 setup(
     name='stim',
     version=version,
     author='Craig Gidney',
     author_email='craig.gidney@gmail.com',
     url='https://github.com/quantumlib/stim',
     license='Apache 2',
-    description='A fast quantum stabilizer circuit simulator.',
+    description='A fast library for analyzing with quantum stabilizer circuits.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     ext_modules=[
         stim_detect_machine_architecture,
         stim_polyfill,
         stim_sse2,
         stim_avx2,
```

### Comparing `stim-1.9.dev1656756326/src/main.cc` & `stim-1.9.dev1657429876/src/main.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/arg_parse.cc` & `stim-1.9.dev1657429876/src/stim/arg_parse.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/arg_parse.h` & `stim-1.9.dev1657429876/src/stim/arg_parse.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/arg_parse.test.cc` & `stim-1.9.dev1657429876/src/stim/arg_parse.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/benchmark_main.perf.cc` & `stim-1.9.dev1657429876/src/stim/benchmark_main.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/benchmark_util.perf.cc` & `stim-1.9.dev1657429876/src/stim/benchmark_util.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/benchmark_util.perf.h` & `stim-1.9.dev1657429876/src/stim/benchmark_util.perf.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.h` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.perf.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.pybind.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -152,23 +152,23 @@
 
             Examples:
                 >>> import stim
                 >>> c = stim.Circuit()
                 >>> c.append("X", 0)
                 >>> c.append("M", 0)
                 >>> c.compile_sampler().sample(shots=1)
-                array([[1]], dtype=uint8)
+                array([[ True]])
 
                 >>> stim.Circuit('''
                 ...    H 0
                 ...    CNOT 0 1
                 ...    M 0 1
                 ...    DETECTOR rec[-1] rec[-2]
                 ... ''').compile_detector_sampler().sample(shots=1)
-                array([[0]], dtype=uint8)
+                array([[False]])
 
         )DOC")
             .data());
 
     pybind_circuit_repeat_block(m);
     pybind_circuit_gate_target(m);
     pybind_circuit_instruction(m);
@@ -350,15 +350,15 @@
                 >>> import stim
                 >>> c = stim.Circuit('''
                 ...    X 2
                 ...    M 0 1 2
                 ... ''')
                 >>> s = c.compile_sampler()
                 >>> s.sample(shots=1)
-                array([[0, 0, 1]], dtype=uint8)
+                array([[False, False,  True]])
         )DOC")
             .data());
 
     c.def(
         "compile_m2d_converter",
         &py_init_compiled_measurements_to_detection_events_converter,
         pybind11::kw_only(),
@@ -435,15 +435,15 @@
                 ...    H 0
                 ...    CNOT 0 1
                 ...    M 0 1
                 ...    DETECTOR rec[-1] rec[-2]
                 ... ''')
                 >>> s = c.compile_detector_sampler()
                 >>> s.sample(shots=1)
-                array([[0]], dtype=uint8)
+                array([[False]])
         )DOC")
             .data());
 
     c.def(
         "clear",
         &Circuit::clear,
         clean_doc_string(u8R"DOC(
@@ -1028,28 +1028,26 @@
                 >>> import tempfile
                 >>> c = stim.Circuit('H 5\nX 0')
 
                 >>> with tempfile.TemporaryDirectory() as tmpdir:
                 ...     path = tmpdir + '/tmp.stim'
                 ...     with open(path, 'w') as f:
                 ...         c.to_file(f)
-                ...     with open(path, 'w') as f:
+                ...     with open(path) as f:
                 ...         contents = f.read()
                 >>> contents
-                H 5
-                X 0
+                'H 5\nX 0\n'
 
                 >>> with tempfile.TemporaryDirectory() as tmpdir:
                 ...     path = tmpdir + '/tmp.stim'
                 ...     c.to_file(path)
-                ...     with open(path, 'w') as f:
+                ...     with open(path) as f:
                 ...         contents = f.read()
                 >>> contents
-                H 5
-                X 0
+                'H 5\nX 0\n'
         )DOC")
             .data());
 
     c.def(
         "__len__",
         [](const Circuit &self) {
             return self.operations.size();
@@ -1645,21 +1643,21 @@
 
             Returns:
                 A `stim.Circuit` with the same instructions except all noise
                 processes have been removed.
 
             Examples:
                 >>> import stim
-                >>> circuit = stim.Circuit('''
+                >>> stim.Circuit('''
                 ...     X_ERROR(0.25) 0
                 ...     CNOT 0 1
                 ...     M(0.125) 0
                 ... ''').without_noise()
                 stim.Circuit('''
-                    CNOT 0 1
+                    CX 0 1
                     M 0
                 ''')
         )DOC")
             .data());
 
     c.def(
         "flattened",
@@ -1670,15 +1668,15 @@
             Returns:
                 A `stim.Circuit` with the same instructions in the same order,
                 but with loops flattened into repeated instructions and with
                 all coordinate shifts inlined.
 
             Examples:
                 >>> import stim
-                >>> circuit = stim.Circuit('''
+                >>> stim.Circuit('''
                 ...     REPEAT 5 {
                 ...         MR 0 1
                 ...         DETECTOR(0, 0) rec[-2]
                 ...         DETECTOR(1, 0) rec[-1]
                 ...         SHIFT_COORDS(0, 1)
                 ...     }
                 ... ''').flattened()
```

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.pybind.h` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.test.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit.test.h` & `stim-1.9.dev1657429876/src/stim/circuit/circuit.test.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit_gate_target.pybind.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit_gate_target.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit_gate_target.pybind.h` & `stim-1.9.dev1657429876/src/stim/circuit/circuit_gate_target.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit_instruction.pybind.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit_instruction.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit_instruction.pybind.h` & `stim-1.9.dev1657429876/src/stim/circuit/circuit_instruction.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit_repeat_block.pybind.cc` & `stim-1.9.dev1657429876/src/stim/circuit/circuit_repeat_block.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/circuit_repeat_block.pybind.h` & `stim-1.9.dev1657429876/src/stim/circuit/circuit_repeat_block.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data.h` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data.perf.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data.test.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_annotations.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_annotations.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_blocks.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_blocks.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_collapsing.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_collapsing.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_controlled.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_controlled.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_hada.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_hada.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_noisy.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_noisy.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_pauli.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_pauli.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_period_3.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_period_3.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_period_4.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_period_4.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_pp.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_pp.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_data_swaps.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_data_swaps.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_target.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_target.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_target.h` & `stim-1.9.dev1657429876/src/stim/circuit/gate_target.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/circuit/gate_target.test.cc` & `stim-1.9.dev1657429876/src/stim/circuit/gate_target.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model.cc` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model.h` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model.pybind.cc` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model.pybind.cc`

 * *Files 0% similar despite different names*

```diff
@@ -902,22 +902,22 @@
                 >>> import tempfile
                 >>> c = stim.DetectorErrorModel('error(0.25) D2 D3')
 
                 >>> with tempfile.TemporaryDirectory() as tmpdir:
                 ...     path = tmpdir + '/tmp.stim'
                 ...     with open(path, 'w') as f:
                 ...         c.to_file(f)
-                ...     with open(path, 'w') as f:
+                ...     with open(path) as f:
                 ...         contents = f.read()
                 >>> contents
-                error(0.25) D2 D3
+                'error(0.25) D2 D3\n'
 
                 >>> with tempfile.TemporaryDirectory() as tmpdir:
                 ...     path = tmpdir + '/tmp.stim'
                 ...     c.to_file(path)
-                ...     with open(path, 'w') as f:
+                ...     with open(path) as f:
                 ...         contents = f.read()
                 >>> contents
-                error(0.25) D2 D3
+                'error(0.25) D2 D3\n'
         )DOC")
             .data());
 }
```

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model.pybind.h` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model.test.cc` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model_instruction.pybind.cc` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model_instruction.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model_instruction.pybind.h` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model_instruction.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model_repeat_block.pybind.cc` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model_repeat_block.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model_repeat_block.pybind.h` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model_repeat_block.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model_target.pybind.cc` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model_target.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/dem/detector_error_model_target.pybind.h` & `stim-1.9.dev1657429876/src/stim/dem/detector_error_model_target.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/circuit_gen_main.cc` & `stim-1.9.dev1657429876/src/stim/gen/circuit_gen_main.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/circuit_gen_main.test.cc` & `stim-1.9.dev1657429876/src/stim/gen/circuit_gen_main.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/circuit_gen_params.cc` & `stim-1.9.dev1657429876/src/stim/gen/circuit_gen_params.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/circuit_gen_params.h` & `stim-1.9.dev1657429876/src/stim/gen/circuit_gen_params.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/circuit_gen_params.test.cc` & `stim-1.9.dev1657429876/src/stim/gen/circuit_gen_params.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/gen_color_code.cc` & `stim-1.9.dev1657429876/src/stim/gen/gen_color_code.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/gen_color_code.test.cc` & `stim-1.9.dev1657429876/src/stim/gen/gen_color_code.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/gen_rep_code.cc` & `stim-1.9.dev1657429876/src/stim/gen/gen_rep_code.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/gen_rep_code.test.cc` & `stim-1.9.dev1657429876/src/stim/gen/gen_rep_code.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/gen_surface_code.cc` & `stim-1.9.dev1657429876/src/stim/gen/gen_surface_code.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/gen/gen_surface_code.test.cc` & `stim-1.9.dev1657429876/src/stim/gen/gen_surface_code.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/help.cc` & `stim-1.9.dev1657429876/src/stim/help.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/help.h` & `stim-1.9.dev1657429876/src/stim/help.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record.h` & `stim-1.9.dev1657429876/src/stim/io/measure_record.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record.test.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_batch.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_batch.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_batch.h` & `stim-1.9.dev1657429876/src/stim/io/measure_record_batch.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_batch.test.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_batch.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_batch_writer.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_batch_writer.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_batch_writer.h` & `stim-1.9.dev1657429876/src/stim/io/measure_record_batch_writer.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_batch_writer.test.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_batch_writer.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_reader.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_reader.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_reader.h` & `stim-1.9.dev1657429876/src/stim/io/measure_record_reader.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_reader.perf.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_reader.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_reader.test.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_reader.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_writer.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_writer.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_writer.h` & `stim-1.9.dev1657429876/src/stim/io/measure_record_writer.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/measure_record_writer.test.cc` & `stim-1.9.dev1657429876/src/stim/io/measure_record_writer.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/raii_file.cc` & `stim-1.9.dev1657429876/src/stim/io/raii_file.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/raii_file.h` & `stim-1.9.dev1657429876/src/stim/io/raii_file.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/read_write.pybind.cc` & `stim-1.9.dev1657429876/src/stim/io/read_write.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -290,25 +290,25 @@
 
             Examples:
                 >>> import stim
                 >>> import pathlib
                 >>> import tempfile
                 >>> with tempfile.TemporaryDirectory() as d:
                 ...     path = pathlib.Path(d) / 'shots'
-                ...     with open(path) as f:
+                ...     with open(path, 'w') as f:
                 ...         print("0000", file=f)
                 ...         print("0101", file=f)
                 ...
                 ...     read = stim.read_shot_data_file(
                 ...         path=str(path),
                 ...         format='01',
                 ...         num_measurements=4)
                 >>> read
-                [[False False False False]
-                 [False  True False  True]]
+                array([[False, False, False, False],
+                       [False,  True, False,  True]])
         )DOC")
             .data());
 
     m.def(
         "write_shot_data_file",
         &write_shot_data_file,
         pybind11::kw_only(),
@@ -337,14 +337,15 @@
                     Note that this only refers to observables *in the given shot data*, not to
                     observables from the original circuit that was sampled.
 
             Examples:
                 >>> import stim
                 >>> import pathlib
                 >>> import tempfile
+                >>> import numpy as np
                 >>> with tempfile.TemporaryDirectory() as d:
                 ...     path = pathlib.Path(d) / 'shots'
                 ...     shot_data = np.array([
                 ...         [0, 1, 0],
                 ...         [0, 1, 1],
                 ...     ], dtype=np.bool8)
                 ...
```

### Comparing `stim-1.9.dev1656756326/src/stim/io/read_write.pybind.h` & `stim-1.9.dev1657429876/src/stim/io/read_write.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/sparse_shot.cc` & `stim-1.9.dev1657429876/src/stim/io/sparse_shot.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/sparse_shot.h` & `stim-1.9.dev1657429876/src/stim/io/sparse_shot.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/sparse_shot.test.cc` & `stim-1.9.dev1657429876/src/stim/io/sparse_shot.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/stim_data_formats.cc` & `stim-1.9.dev1657429876/src/stim/io/stim_data_formats.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/io/stim_data_formats.h` & `stim-1.9.dev1657429876/src/stim/io/stim_data_formats.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/main_namespaced.cc` & `stim-1.9.dev1657429876/src/stim/main_namespaced.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/main_namespaced.h` & `stim-1.9.dev1657429876/src/stim/main_namespaced.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/main_namespaced.perf.cc` & `stim-1.9.dev1657429876/src/stim/main_namespaced.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/main_namespaced.test.cc` & `stim-1.9.dev1657429876/src/stim/main_namespaced.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/bit_ref.cc` & `stim-1.9.dev1657429876/src/stim/mem/bit_ref.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/bit_ref.h` & `stim-1.9.dev1657429876/src/stim/mem/bit_ref.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/bit_ref.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/bit_ref.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/fixed_cap_vector.h` & `stim-1.9.dev1657429876/src/stim/mem/fixed_cap_vector.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/fixed_cap_vector.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/fixed_cap_vector.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/monotonic_buffer.h` & `stim-1.9.dev1657429876/src/stim/mem/monotonic_buffer.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/monotonic_buffer.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/monotonic_buffer.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/pointer_range.h` & `stim-1.9.dev1657429876/src/stim/mem/pointer_range.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.perf.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bit_table.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bit_table.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits.perf.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits_range_ref.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits_range_ref.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits_range_ref.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits_range_ref.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_bits_range_ref.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_bits_range_ref.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat.perf.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat_avx2.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat_avx2.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat_polyfill.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat_polyfill.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_compat_sse2.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_compat_sse2.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_util.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_util.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_util.h` & `stim-1.9.dev1657429876/src/stim/mem/simd_util.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/simd_util.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/simd_util.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.cc` & `stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.h` & `stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.perf.cc` & `stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/mem/sparse_xor_vec.test.cc` & `stim-1.9.dev1657429876/src/stim/mem/sparse_xor_vec.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/probability_util.cc` & `stim-1.9.dev1657429876/src/stim/probability_util.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/probability_util.h` & `stim-1.9.dev1657429876/src/stim/probability_util.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/probability_util.perf.cc` & `stim-1.9.dev1657429876/src/stim/probability_util.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/probability_util.test.cc` & `stim-1.9.dev1657429876/src/stim/probability_util.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/py/base.pybind.cc` & `stim-1.9.dev1657429876/src/stim/py/base.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/py/base.pybind.h` & `stim-1.9.dev1657429876/src/stim/py/base.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/py/compiled_detector_sampler.pybind.cc` & `stim-1.9.dev1657429876/src/stim/py/compiled_detector_sampler.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 ...    CNOT 0 1
                 ...    X_ERROR(1.0) 0
                 ...    M 0 1
                 ...    DETECTOR rec[-1] rec[-2]
                 ... ''')
                 >>> s = c.compile_detector_sampler()
                 >>> s.sample(shots=1)
-                array([[1]], dtype=uint8)
+                array([[ True]])
         )DOC")
             .data());
 
     c.def(
         "sample",
         &CompiledDetectorSampler::sample,
         pybind11::arg("shots"),
```

### Comparing `stim-1.9.dev1656756326/src/stim/py/compiled_detector_sampler.pybind.h` & `stim-1.9.dev1657429876/src/stim/py/compiled_detector_sampler.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/py/compiled_measurement_sampler.pybind.cc` & `stim-1.9.dev1657429876/src/stim/py/compiled_measurement_sampler.pybind.cc`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
                 >>> import stim
                 >>> c = stim.Circuit('''
                 ...    X 0   2 3
                 ...    M 0 1 2 3
                 ... ''')
                 >>> s = c.compile_sampler()
                 >>> s.sample(shots=1)
-                array([[1, 0, 1, 1]], dtype=uint8)
+                array([[ True, False,  True,  True]])
         )DOC")
             .data());
 
     c.def(
         "sample",
         &CompiledMeasurementSampler::sample,
         pybind11::arg("shots"),
@@ -173,15 +173,15 @@
                 >>> import stim
                 >>> c = stim.Circuit('''
                 ...    X 0   2 3
                 ...    M 0 1 2 3
                 ... ''')
                 >>> s = c.compile_sampler()
                 >>> s.sample(shots=1)
-                array([[1, 0, 1, 1]], dtype=uint8)
+                array([[ True, False,  True,  True]])
 
             Args:
                 shots: The number of times to sample every measurement in the circuit.
 
             Returns:
                 A numpy array with `dtype=uint8` and `shape=(shots, num_measurements)`.
                 The bit for measurement `m` in shot `s` is at `result[s, m]`.
```

### Comparing `stim-1.9.dev1656756326/src/stim/py/compiled_measurement_sampler.pybind.h` & `stim-1.9.dev1657429876/src/stim/py/compiled_measurement_sampler.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/py/march.pybind.cc` & `stim-1.9.dev1657429876/src/stim/py/march.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/py/stim.pybind.cc` & `stim-1.9.dev1657429876/src/stim/py/stim.pybind.cc`

 * *Files 3% similar despite different names*

```diff
@@ -232,21 +232,30 @@
             Raises:
                 A large variety of errors, depending on what you are doing and
                 how it failed! Beware that many errors are caught by the main
                 method itself and printed to stderr, with the only indication
                 that something went wrong being the return code.
 
             Example:
-                >>> stim.main(command_line_args=[
-                ...     "gen",
-                ...     "--code=repetition_code",
-                ...     "--task=memory",
-                ...     "--rounds=1000",
-                ...     "--distance=2",
-                ... ])
+                >>> import stim
+                >>> import tempfile
+                >>> with tempfile.TemporaryDirectory() as d:
+                ...     path = f'{d}/tmp.out'
+                ...     return_code = stim.main(command_line_args=[
+                ...         "gen",
+                ...         "--code=repetition_code",
+                ...         "--task=memory",
+                ...         "--rounds=1000",
+                ...         "--distance=2",
+                ...         "--out",
+                ...         path,
+                ...     ])
+                ...     assert return_code == 0
+                ...     with open(path) as f:
+                ...         print(f.read(), end='')
                 # Generated repetition_code circuit.
                 # task: memory
                 # rounds: 1000
                 # distance: 2
                 # before_round_data_depolarization: 0
                 # before_measure_flip_probability: 0
                 # after_reset_flip_probability: 0
```

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/algo.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/algo.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/algo.h` & `stim-1.9.dev1657429876/src/stim/search/graphlike/algo.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/algo.perf.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/algo.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/algo.test.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/algo.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/edge.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/edge.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/edge.h` & `stim-1.9.dev1657429876/src/stim/search/graphlike/edge.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/edge.test.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/edge.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/graph.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/graph.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/graph.h` & `stim-1.9.dev1657429876/src/stim/search/graphlike/graph.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/graph.test.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/graph.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/node.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/node.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/node.h` & `stim-1.9.dev1657429876/src/stim/search/graphlike/node.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/node.test.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/node.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/search_state.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/search_state.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/search_state.h` & `stim-1.9.dev1657429876/src/stim/search/graphlike/search_state.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/graphlike/search_state.test.cc` & `stim-1.9.dev1657429876/src/stim/search/graphlike/search_state.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/algo.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/algo.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/algo.h` & `stim-1.9.dev1657429876/src/stim/search/hyper/algo.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/algo.test.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/algo.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/edge.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/edge.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/edge.h` & `stim-1.9.dev1657429876/src/stim/search/hyper/edge.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/edge.test.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/edge.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/graph.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/graph.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/graph.h` & `stim-1.9.dev1657429876/src/stim/search/hyper/graph.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/graph.test.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/graph.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/node.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/node.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/node.h` & `stim-1.9.dev1657429876/src/stim/search/hyper/node.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/node.test.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/node.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/search_state.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/search_state.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/search_state.h` & `stim-1.9.dev1657429876/src/stim/search/hyper/search_state.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/hyper/search_state.test.cc` & `stim-1.9.dev1657429876/src/stim/search/hyper/search_state.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/search/search.h` & `stim-1.9.dev1657429876/src/stim/search/search.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/detection_simulator.cc` & `stim-1.9.dev1657429876/src/stim/simulators/detection_simulator.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/detection_simulator.h` & `stim-1.9.dev1657429876/src/stim/simulators/detection_simulator.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/detection_simulator.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/detection_simulator.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.cc` & `stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.h` & `stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.perf.cc` & `stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_analyzer.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/error_analyzer.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_matcher.cc` & `stim-1.9.dev1657429876/src/stim/simulators/error_matcher.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_matcher.h` & `stim-1.9.dev1657429876/src/stim/simulators/error_matcher.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/error_matcher.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/error_matcher.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.cc` & `stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.h` & `stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.perf.cc` & `stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/frame_simulator.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/frame_simulator.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/matched_error.cc` & `stim-1.9.dev1657429876/src/stim/simulators/matched_error.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/matched_error.h` & `stim-1.9.dev1657429876/src/stim/simulators/matched_error.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/matched_error.pybind.cc` & `stim-1.9.dev1657429876/src/stim/simulators/matched_error.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/matched_error.pybind.h` & `stim-1.9.dev1657429876/src/stim/simulators/matched_error.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/matched_error.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/matched_error.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.cc` & `stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.h` & `stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.pybind.cc` & `stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -339,23 +339,21 @@
                 ...                            [1, 0]], dtype=np.bool8),
                 ...     separate_observables=True,
                 ... )
                 >>> dets
                 array([[False, False],
                        [False, False],
                        [False, False],
-                       [ True, False],
-                       [False, False],
+                       [False,  True],
                        [False, False]])
                 >>> obs
                 array([[False],
                        [False],
                        [False],
                        [ True],
-                       [False],
                        [False]])
         )DOC")
             .data());
 
     c.def(
         "__repr__",
         &CompiledMeasurementsToDetectionEventsConverter::repr,
```

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.pybind.h` & `stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/measurements_to_detection_events.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/measurements_to_detection_events.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.cc` & `stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.h` & `stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.perf.cc` & `stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.pybind.cc` & `stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.pybind.cc`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,15 @@
             bool readonly = true;
             return pybind11::array_t<float>(
                 pybind11::buffer_info(ptr, itemsize, format, shape.size(), shape, stride, readonly));
         },
         pybind11::kw_only(),
         pybind11::arg("endian") = "little",
         clean_doc_string(u8R"DOC(
+            @signature def state_vector(self, *, endian: str = 'little') -> np.ndarray[np.complex64]:
             Returns a wavefunction that satisfies the stabilizers of the simulator's current state.
 
             This function takes O(n * 2**n) time and O(2**n) space, where n is the number of qubits. The computation is
             done by initialization a random state vector and iteratively projecting it into the +1 eigenspace of each
             stabilizer of the state. The state is then canonicalized so that zero values are actually exactly 0, and so
             that the first non-zero entry is positive.
 
@@ -239,15 +240,15 @@
             Returns:
                 A `numpy.ndarray[numpy.complex64]` of computational basis amplitudes.
 
                 If the result is in little endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
                 the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_0, the
                 qubit with index 1 is storing the bit b_1, etc.
 
-                If the result is in little endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
+                If the result is in big endian order then the amplitude at offset b_0 + b_1*2 + b_2*4 + ... + b_{n-1}*2^{n-1} is
                 the amplitude for the computational basis state where the qubit with index 0 is storing the bit b_{n-1}, the
                 qubit with index 1 is storing the bit b_{n-2}, etc.
 
             Examples:
                 >>> import stim
                 >>> import numpy as np
                 >>> s = stim.TableauSimulator()
@@ -381,14 +382,15 @@
         clean_doc_string(u8R"DOC(
             Applies the paulis from a pauli string to the simulator's state.
 
             Args:
                 pauli_string: A stim.PauliString containing Paulis to apply.
 
             Examples:
+                >>> import stim
                 >>> s = stim.TableauSimulator()
                 >>> s.do_pauli_string(stim.PauliString("IXYZ"))
                 >>> s.measure_many(0, 1, 2, 3)
                 [False, True, True, False]
         )DOC")
             .data());
 
@@ -448,15 +450,15 @@
                 targets: The indices of the qubits to operate on.
 
             Examples:
                 >>> import stim
                 >>> sim = stim.TableauSimulator()
                 >>> sim.h(1)
                 >>> sim.h_yz(2)
-                >>> [str(sim.peek_block(k)) for k in range(4)]
+                >>> [str(sim.peek_bloch(k)) for k in range(4)]
                 ['+Z', '+X', '+Y', '+Z']
                 >>> rot3 = stim.Tableau.from_conjugated_generators(
                 ...     xs=[
                 ...         stim.PauliString("_X_"),
                 ...         stim.PauliString("__X"),
                 ...         stim.PauliString("X__"),
                 ...     ],
@@ -464,19 +466,19 @@
                 ...         stim.PauliString("_Z_"),
                 ...         stim.PauliString("__Z"),
                 ...         stim.PauliString("Z__"),
                 ...     ],
                 ... )
 
                 >>> sim.do_tableau(rot3, [1, 2, 3])
-                >>> [str(sim.peek_block(k)) for k in range(4)]
+                >>> [str(sim.peek_bloch(k)) for k in range(4)]
                 ['+Z', '+Z', '+X', '+Y']
 
                 >>> sim.do_tableau(rot3, [1, 2, 3])
-                >>> [str(sim.peek_block(k)) for k in range(4)]
+                >>> [str(sim.peek_bloch(k)) for k in range(4)]
                 ['+Z', '+Y', '+Z', '+X']
         )DOC")
             .data());
 
     c.def(
         "h",
         [](PyTableauSimulator &self, pybind11::args args) {
@@ -487,14 +489,53 @@
 
             Args:
                 *targets: The indices of the qubits to target with the gate.
         )DOC")
             .data());
 
     c.def(
+        "h_xz",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.H_XZ(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a Hadamard gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+        )DOC")
+            .data());
+
+    c.def(
+        "c_xyz",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.C_XYZ(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a C_XYZ gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+        )DOC")
+            .data());
+
+    c.def(
+        "c_zyx",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.C_ZYX(args_to_targets(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a C_ZYX gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+        )DOC")
+            .data());
+
+    c.def(
         "h_xy",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.H_XY(args_to_targets(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a variant of the Hadamard gate that swaps the X and Y axes to the simulator's state.
 
@@ -690,14 +731,44 @@
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
+        "zcx",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCX(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled X gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
+        "cx",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCX(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled X gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
         "cz",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.ZCZ(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a controlled Z gate to the simulator's state.
 
@@ -705,14 +776,29 @@
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
+        "zcz",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCZ(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled Z gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
         "cy",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.ZCY(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies a controlled Y gate to the simulator's state.
 
@@ -720,14 +806,29 @@
                 *targets: The indices of the qubits to target with the gate.
                     Applies the gate to the first two targets, then the next two targets, and so forth.
                     There must be an even number of targets.
         )DOC")
             .data());
 
     c.def(
+        "zcy",
+        [](PyTableauSimulator &self, pybind11::args args) {
+            self.ZCY(args_to_target_pairs(self, args));
+        },
+        clean_doc_string(u8R"DOC(
+            Applies a controlled Y gate to the simulator's state.
+
+            Args:
+                *targets: The indices of the qubits to target with the gate.
+                    Applies the gate to the first two targets, then the next two targets, and so forth.
+                    There must be an even number of targets.
+        )DOC")
+            .data());
+
+    c.def(
         "xcx",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.XCX(args_to_target_pairs(self, args));
         },
         clean_doc_string(u8R"DOC(
             Applies an X-controlled X gate to the simulator's state.
 
@@ -823,18 +924,18 @@
 
             Args:
                 *targets: The indices of the qubits to reset.
 
             Example:
                 >>> import stim
                 >>> s = stim.TableauSimulator()
-                >>> s.X(0)
+                >>> s.x(0)
                 >>> s.reset(0)
                 >>> s.peek_bloch(0)
-                +Z
+                stim.PauliString("+Z")
         )DOC")
             .data());
 
     c.def(
         "reset_x",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.reset_x(args_to_targets(self, args));
@@ -846,15 +947,15 @@
                 *targets: The indices of the qubits to reset.
 
             Example:
                 >>> import stim
                 >>> s = stim.TableauSimulator()
                 >>> s.reset_x(0)
                 >>> s.peek_bloch(0)
-                +X
+                stim.PauliString("+X")
         )DOC")
             .data());
 
     c.def(
         "reset_y",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.reset_y(args_to_targets(self, args));
@@ -866,15 +967,15 @@
                 *targets: The indices of the qubits to reset.
 
             Example:
                 >>> import stim
                 >>> s = stim.TableauSimulator()
                 >>> s.reset_y(0)
                 >>> s.peek_bloch(0)
-                +Y
+                stim.PauliString("+Y")
         )DOC")
             .data());
 
     c.def(
         "reset_z",
         [](PyTableauSimulator &self, pybind11::args args) {
             self.reset_z(args_to_targets(self, args));
@@ -884,18 +985,18 @@
 
             Args:
                 *targets: The indices of the qubits to reset.
 
             Example:
                 >>> import stim
                 >>> s = stim.TableauSimulator()
-                >>> s.H(0)
+                >>> s.h(0)
                 >>> s.reset_z(0)
                 >>> s.peek_bloch(0)
-                +Z
+                stim.PauliString("+Z")
         )DOC")
             .data());
 
     c.def(
         "peek_x",
         [](PyTableauSimulator &self, uint32_t target) -> int8_t {
             self.ensure_large_enough_for_qubits(target + 1);
@@ -921,15 +1022,15 @@
                 >>> s = stim.TableauSimulator()
                 >>> s.reset_z(0)
                 >>> s.peek_x(0)
                 0
                 >>> s.reset_x(0)
                 >>> s.peek_x(0)
                 1
-                >>> s.Z(0)
+                >>> s.z(0)
                 >>> s.peek_x(0)
                 -1
         )DOC")
             .data());
 
     c.def(
         "peek_y",
@@ -957,15 +1058,15 @@
                 >>> s = stim.TableauSimulator()
                 >>> s.reset_z(0)
                 >>> s.peek_y(0)
                 0
                 >>> s.reset_y(0)
                 >>> s.peek_y(0)
                 1
-                >>> s.Z(0)
+                >>> s.z(0)
                 >>> s.peek_y(0)
                 -1
         )DOC")
             .data());
 
     c.def(
         "peek_z",
@@ -993,15 +1094,15 @@
                 >>> s = stim.TableauSimulator()
                 >>> s.reset_x(0)
                 >>> s.peek_z(0)
                 0
                 >>> s.reset_z(0)
                 >>> s.peek_z(0)
                 1
-                >>> s.X(0)
+                >>> s.x(0)
                 >>> s.peek_z(0)
                 -1
         )DOC")
             .data());
 
     c.def(
         "peek_bloch",
@@ -1232,14 +1333,36 @@
                     The postselection failed. One of the qubits was in a state
                     orthogonal to the desired state, so it was literally
                     impossible for a measurement of the qubit to return the
                     desired result.
         )DOC")
             .data());
 
+    c.def_property_readonly(
+        "num_qubits",
+        [](const PyTableauSimulator &self) -> size_t {
+            return self.inv_state.num_qubits;
+        },
+        clean_doc_string(u8R"DOC(
+            Returns the number of qubits currently being tracked by the simulator's internal state.
+
+            Note that the number of qubits being tracked will implicitly increase if qubits beyond
+            the current limit are touched. Untracked qubits are always assumed to be in the |0> state.
+
+            Examples:
+                >>> import stim
+                >>> s = stim.TableauSimulator()
+                >>> s.num_qubits
+                0
+                >>> s.h(2)
+                >>> s.num_qubits
+                3
+        )DOC")
+            .data());
+
     c.def(
         "set_num_qubits",
         [](PyTableauSimulator &self, uint32_t new_num_qubits) {
             self.set_num_qubits(new_num_qubits);
         },
         pybind11::arg("new_num_qubits"),
         clean_doc_string(u8R"DOC(
```

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.pybind.h` & `stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/tableau_simulator.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/tableau_simulator.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/vector_simulator.cc` & `stim-1.9.dev1657429876/src/stim/simulators/vector_simulator.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/vector_simulator.h` & `stim-1.9.dev1657429876/src/stim/simulators/vector_simulator.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/simulators/vector_simulator.test.cc` & `stim-1.9.dev1657429876/src/stim/simulators/vector_simulator.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.h` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.perf.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.pybind.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.pybind.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.pybind.h` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string.test.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string_ref.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string_ref.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/pauli_string_ref.h` & `stim-1.9.dev1657429876/src/stim/stabilizers/pauli_string_ref.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau.h` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau.perf.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau.perf.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau.pybind.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau.pybind.cc`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
             bool readonly = true;
             return pybind11::array_t<float>(
                 pybind11::buffer_info(ptr, itemsize, format, shape.size(), shape, stride, readonly));
         },
         pybind11::kw_only(),
         pybind11::arg("endian"),
         clean_doc_string(u8R"DOC(
+            @signature def to_unitary_matrix(self, *, endian: str) -> np.ndarray[np.complex64]:
             Converts the tableau into a unitary matrix.
 
             Args:
                 endian:
                     "little": The first qubit is the least significant (corresponds
                         to an offset of 1 in the state vector).
                     "big": The first qubit is the most significant (corresponds
```

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau.pybind.h` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau.pybind.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau.test.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau_specialized_prepend.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau_specialized_prepend.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau_transposed_raii.cc` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau_transposed_raii.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/stabilizers/tableau_transposed_raii.h` & `stim-1.9.dev1657429876/src/stim/stabilizers/tableau_transposed_raii.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/str_util.h` & `stim-1.9.dev1657429876/src/stim/str_util.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/str_util.test.cc` & `stim-1.9.dev1657429876/src/stim/str_util.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/test_util.test.cc` & `stim-1.9.dev1657429876/src/stim/test_util.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim/test_util.test.h` & `stim-1.9.dev1657429876/src/stim/test_util.test.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim.cc` & `stim-1.9.dev1657429876/src/stim.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim.h` & `stim-1.9.dev1657429876/src/stim.h`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim.test.cc` & `stim-1.9.dev1657429876/src/stim.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/src/stim_included_twice.test.cc` & `stim-1.9.dev1657429876/src/stim_included_twice.test.cc`

 * *Files identical despite different names*

### Comparing `stim-1.9.dev1656756326/stim.egg-info/PKG-INFO` & `stim-1.9.dev1657429876/stim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: stim
-Version: 1.9.dev1656756326
-Summary: A fast quantum stabilizer circuit simulator.
+Version: 1.9.dev1657429876
+Summary: A fast library for analyzing with quantum stabilizer circuits.
 Home-page: https://github.com/quantumlib/stim
 Author: Craig Gidney
 Author-email: craig.gidney@gmail.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
```

### Comparing `stim-1.9.dev1656756326/stim.egg-info/SOURCES.txt` & `stim-1.9.dev1657429876/stim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

