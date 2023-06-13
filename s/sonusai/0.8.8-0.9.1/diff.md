# Comparing `tmp/sonusai-0.8.8.tar.gz` & `tmp/sonusai-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonusai-0.8.8.tar", max compression
+gzip compressed data, was "sonusai-0.9.1.tar", max compression
```

## Comparing `sonusai-0.8.8.tar` & `sonusai-0.9.1.tar`

### file list

```diff
@@ -1,84 +1,176 @@
--rw-r--r--   0        0        0      864 2021-07-20 01:11:41.000000 sonusai-0.8.8/README.rst
--rw-r--r--   0        0        0     1127 2022-11-02 20:37:00.000000 sonusai-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     1505 2022-10-14 17:31:47.000000 sonusai-0.8.8/sonusai/__init__.py
--rwxr-xr-x   0        0        0     3595 2022-08-09 21:23:58.000000 sonusai-0.8.8/sonusai/aawscd_probwrite.py
--rw-r--r--   0        0        0    13953 2022-10-19 19:36:27.000000 sonusai-0.8.8/sonusai/data/genmixdb.yml
--rw-r--r--   0        0        0  1920044 2021-12-21 18:48:45.000000 sonusai-0.8.8/sonusai/data/whitenoise.wav
--rw-r--r--   0        0        0      291 2022-10-14 20:54:03.000000 sonusai-0.8.8/sonusai/data_generator/__init__.py
--rw-r--r--   0        0        0     6630 2022-10-20 18:27:03.000000 sonusai-0.8.8/sonusai/data_generator/keras_from_h5.py
--rw-r--r--   0        0        0     5789 2022-10-31 15:55:30.000000 sonusai-0.8.8/sonusai/data_generator/keras_from_mixdb.py
--rw-r--r--   0        0        0     4978 2022-10-19 20:19:54.000000 sonusai-0.8.8/sonusai/data_generator/sequence_from_h5.py
--rw-r--r--   0        0        0      981 2022-10-19 20:20:58.000000 sonusai-0.8.8/sonusai/data_generator/utils.py
--rw-r--r--   0        0        0    10153 2022-11-01 19:44:02.000000 sonusai-0.8.8/sonusai/evaluate.py
--rw-r--r--   0        0        0     9461 2022-10-31 20:32:13.000000 sonusai-0.8.8/sonusai/genft.py
--rw-r--r--   0        0        0     9588 2022-10-31 20:32:13.000000 sonusai-0.8.8/sonusai/genmix.py
--rw-r--r--   0        0        0    27730 2022-10-31 20:32:13.000000 sonusai-0.8.8/sonusai/genmixdb.py
--rw-r--r--   0        0        0    18005 2022-10-05 20:04:39.000000 sonusai-0.8.8/sonusai/gentcst.py
--rw-r--r--   0        0        0     2650 2022-10-13 04:31:20.000000 sonusai-0.8.8/sonusai/keras_onnx.py
--rw-r--r--   0        0        0     9212 2022-10-17 20:42:32.000000 sonusai-0.8.8/sonusai/keras_predict.py
--rw-r--r--   0        0        0    11515 2022-10-19 20:03:59.000000 sonusai-0.8.8/sonusai/keras_train.py
--rw-r--r--   0        0        0     8238 2022-11-01 19:44:02.000000 sonusai-0.8.8/sonusai/lsdb.py
--rw-r--r--   0        0        0     2393 2022-10-31 18:51:33.000000 sonusai-0.8.8/sonusai/main.py
--rw-r--r--   0        0        0      631 2022-09-09 14:39:10.000000 sonusai-0.8.8/sonusai/metrics/__init__.py
--rw-r--r--   0        0        0     3927 2022-10-13 17:19:27.000000 sonusai-0.8.8/sonusai/metrics/calculate_class_weights.py
--rw-r--r--   0        0        0     3196 2022-10-13 19:22:06.000000 sonusai-0.8.8/sonusai/metrics/calculate_optimal_thresholds.py
--rw-r--r--   0        0        0      938 2022-05-11 15:57:59.000000 sonusai-0.8.8/sonusai/metrics/calculate_sample_weights.py
--rw-r--r--   0        0        0     3138 2022-10-11 04:54:25.000000 sonusai-0.8.8/sonusai/metrics/class_summary.py
--rw-r--r--   0        0        0     3751 2022-10-11 04:54:56.000000 sonusai-0.8.8/sonusai/metrics/confusion_matrix_summary.py
--rw-r--r--   0        0        0    12965 2022-10-13 19:22:06.000000 sonusai-0.8.8/sonusai/metrics/one_hot.py
--rw-r--r--   0        0        0     5242 2022-11-01 19:38:41.000000 sonusai-0.8.8/sonusai/metrics/snr_summary.py
--rw-r--r--   0        0        0     5231 2022-10-31 15:55:31.000000 sonusai-0.8.8/sonusai/mixture/__init__.py
--rw-r--r--   0        0        0     8453 2022-10-19 20:14:46.000000 sonusai-0.8.8/sonusai/mixture/active_truth_class_balancing.py
--rw-r--r--   0        0        0    11754 2022-10-31 18:39:47.000000 sonusai-0.8.8/sonusai/mixture/audio_db.py
--rw-r--r--   0        0        0     8814 2022-10-11 03:36:35.000000 sonusai-0.8.8/sonusai/mixture/augmentation.py
--rw-r--r--   0        0        0      644 2022-09-14 01:06:01.000000 sonusai-0.8.8/sonusai/mixture/balance.py
--rw-r--r--   0        0        0     2356 2022-10-11 04:36:39.000000 sonusai-0.8.8/sonusai/mixture/class_count.py
--rw-r--r--   0        0        0    18797 2022-11-01 19:44:02.000000 sonusai-0.8.8/sonusai/mixture/config.py
--rw-r--r--   0        0        0     1020 2022-09-14 01:06:49.000000 sonusai-0.8.8/sonusai/mixture/constants.py
--rw-r--r--   0        0        0     1081 2022-09-14 01:06:53.000000 sonusai-0.8.8/sonusai/mixture/dataclasses_sonusai.py
--rw-r--r--   0        0        0     7482 2022-11-02 20:40:10.000000 sonusai-0.8.8/sonusai/mixture/feature.py
--rw-r--r--   0        0        0     1335 2022-08-09 21:05:21.000000 sonusai-0.8.8/sonusai/mixture/log_duration_and_sizes.py
--rw-r--r--   0        0        0     1803 2022-09-13 01:08:15.000000 sonusai-0.8.8/sonusai/mixture/mapped_snr_f.py
--rw-r--r--   0        0        0    11150 2022-10-11 01:22:29.000000 sonusai-0.8.8/sonusai/mixture/mixdb.py
--rw-r--r--   0        0        0     5940 2022-10-11 04:39:11.000000 sonusai-0.8.8/sonusai/mixture/process.py
--rw-r--r--   0        0        0      622 2022-08-09 20:32:22.000000 sonusai-0.8.8/sonusai/mixture/segment.py
--rw-r--r--   0        0        0     1395 2022-10-11 01:05:33.000000 sonusai-0.8.8/sonusai/mixture/segsnr.py
--rw-r--r--   0        0        0     3729 2022-08-24 18:58:32.000000 sonusai-0.8.8/sonusai/mixture/target_class_balancing.py
--rw-r--r--   0        0        0     6909 2022-09-30 19:43:01.000000 sonusai-0.8.8/sonusai/mixture/targets.py
--rw-r--r--   0        0        0     9730 2022-11-01 22:24:11.000000 sonusai-0.8.8/sonusai/mixture/truth.py
--rw-r--r--   0        0        0     6745 2022-11-01 16:37:26.000000 sonusai-0.8.8/sonusai/mkwav.py
--rw-r--r--   0        0        0     8682 2022-10-21 17:47:53.000000 sonusai-0.8.8/sonusai/onnx_predict.py
--rw-r--r--   0        0        0    16847 2022-11-01 19:39:34.000000 sonusai-0.8.8/sonusai/plot.py
--rw-r--r--   0        0        0      474 2022-07-22 19:34:58.000000 sonusai-0.8.8/sonusai/queries/__init__.py
--rw-r--r--   0        0        0     9337 2022-10-11 04:57:36.000000 sonusai-0.8.8/sonusai/queries/queries.py
--rwxr-xr-x   0        0        0    58096 2022-11-01 23:15:56.000000 sonusai-0.8.8/sonusai/speech_enh.py
--rw-r--r--   0        0        0    14769 2022-10-11 01:38:14.000000 sonusai-0.8.8/sonusai/tplot.py
--rw-r--r--   0        0        0     2201 2022-11-01 19:34:47.000000 sonusai-0.8.8/sonusai/utils/__init__.py
--rw-r--r--   0        0        0      852 2022-10-13 05:26:48.000000 sonusai-0.8.8/sonusai/utils/braced_glob.py
--rw-r--r--   0        0        0     1322 2022-08-09 20:43:15.000000 sonusai-0.8.8/sonusai/utils/calculate_input_shape.py
--rw-r--r--   0        0        0      405 2022-10-05 19:29:04.000000 sonusai-0.8.8/sonusai/utils/create_ts_name.py
--rw-r--r--   0        0        0      388 2022-07-09 21:26:55.000000 sonusai-0.8.8/sonusai/utils/dataclass_from_dict.py
--rw-r--r--   0        0        0      254 2022-08-09 20:43:35.000000 sonusai-0.8.8/sonusai/utils/dbfs.py
--rw-r--r--   0        0        0     5551 2022-08-09 20:45:16.000000 sonusai-0.8.8/sonusai/utils/engineering_number.py
--rw-r--r--   0        0        0      784 2022-08-25 12:41:30.000000 sonusai-0.8.8/sonusai/utils/get_label_names.py
--rw-r--r--   0        0        0      203 2022-04-15 16:49:07.000000 sonusai-0.8.8/sonusai/utils/grouper.py
--rw-r--r--   0        0        0      279 2022-04-07 22:57:46.000000 sonusai-0.8.8/sonusai/utils/human_readable_size.py
--rw-r--r--   0        0        0     6685 2022-10-31 18:42:48.000000 sonusai-0.8.8/sonusai/utils/keras_utils.py
--rw-r--r--   0        0        0      311 2022-11-01 19:34:34.000000 sonusai-0.8.8/sonusai/utils/numeric_conversion.py
--rw-r--r--   0        0        0     2971 2022-10-28 20:04:11.000000 sonusai-0.8.8/sonusai/utils/onnx_utils.py
--rw-r--r--   0        0        0     2005 2022-10-04 18:35:20.000000 sonusai-0.8.8/sonusai/utils/parallel.py
--rw-r--r--   0        0        0     2039 2022-08-09 23:00:09.000000 sonusai-0.8.8/sonusai/utils/parallel_tqdm.py
--rw-r--r--   0        0        0     2888 2022-10-11 01:10:16.000000 sonusai-0.8.8/sonusai/utils/print_mixture_details.py
--rw-r--r--   0        0        0     1089 2022-09-08 19:52:17.000000 sonusai-0.8.8/sonusai/utils/ranges.py
--rw-r--r--   0        0        0      392 2022-10-04 20:31:09.000000 sonusai-0.8.8/sonusai/utils/read_mixture_data.py
--rw-r--r--   0        0        0     1021 2022-10-04 20:31:09.000000 sonusai-0.8.8/sonusai/utils/read_predict_data.py
--rw-r--r--   0        0        0     7349 2022-10-13 20:13:40.000000 sonusai-0.8.8/sonusai/utils/reshape.py
--rw-r--r--   0        0        0      260 2022-04-07 22:57:46.000000 sonusai-0.8.8/sonusai/utils/seconds_to_hms.py
--rw-r--r--   0        0        0     6833 2022-10-05 18:32:03.000000 sonusai-0.8.8/sonusai/utils/stratified_shuffle_split.py
--rw-r--r--   0        0        0      220 2022-08-09 20:54:37.000000 sonusai-0.8.8/sonusai/utils/to_numpy_array.py
--rw-r--r--   0        0        0      881 2022-04-15 16:49:06.000000 sonusai-0.8.8/sonusai/utils/trim_docstring.py
--rw-r--r--   0        0        0      409 2022-11-01 16:31:50.000000 sonusai-0.8.8/sonusai/utils/wave.py
--rw-r--r--   0        0        0      282 2022-04-07 22:57:46.000000 sonusai-0.8.8/sonusai/utils/yes_or_no.py
--rw-r--r--   0        0        0      625 2022-08-09 21:41:16.000000 sonusai-0.8.8/sonusai/vars.py
--rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 sonusai-0.8.8/setup.py
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 sonusai-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      864 2021-07-20 01:11:41.000000 sonusai-0.9.1/README.rst
+-rw-r--r--   0        0        0     1127 2022-11-07 18:07:16.000000 sonusai-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-09-14 01:19:11.000000 sonusai-0.9.1/sonusai/.DS_Store
+-rw-r--r--   0        0        0     1505 2022-10-14 17:31:47.000000 sonusai-0.9.1/sonusai/__init__.py
+-rwxr-xr-x   0        0        0     3595 2022-08-09 21:23:58.000000 sonusai-0.9.1/sonusai/aawscd_probwrite.py
+-rw-r--r--   0        0        0    14065 2022-11-07 16:41:12.000000 sonusai-0.9.1/sonusai/data/genmixdb.yml
+-rw-r--r--   0        0        0  1920044 2021-12-21 18:48:45.000000 sonusai-0.9.1/sonusai/data/whitenoise.wav
+-rw-r--r--   0        0        0      291 2022-10-14 20:54:03.000000 sonusai-0.9.1/sonusai/data_generator/__init__.py
+-rw-r--r--   0        0        0      446 2022-10-14 20:54:04.000000 sonusai-0.9.1/sonusai/data_generator/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4956 2022-11-07 16:29:00.000000 sonusai-0.9.1/sonusai/data_generator/__pycache__/keras_from_h5.cpython-38.pyc
+-rw-r--r--   0        0        0     4317 2022-11-07 16:29:00.000000 sonusai-0.9.1/sonusai/data_generator/__pycache__/keras_from_mixdb.cpython-38.pyc
+-rw-r--r--   0        0        0     3639 2022-10-19 20:21:10.000000 sonusai-0.9.1/sonusai/data_generator/__pycache__/sequence_from_h5.cpython-38.pyc
+-rw-r--r--   0        0        0     1146 2022-10-19 20:21:11.000000 sonusai-0.9.1/sonusai/data_generator/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     6632 2022-11-07 16:04:52.000000 sonusai-0.9.1/sonusai/data_generator/keras_from_h5.py
+-rw-r--r--   0        0        0     5791 2022-11-07 16:07:08.000000 sonusai-0.9.1/sonusai/data_generator/keras_from_mixdb.py
+-rw-r--r--   0        0        0     4978 2022-10-19 20:19:54.000000 sonusai-0.9.1/sonusai/data_generator/sequence_from_h5.py
+-rw-r--r--   0        0        0      981 2022-10-19 20:20:58.000000 sonusai-0.9.1/sonusai/data_generator/utils.py
+-rw-r--r--   0        0        0    10155 2022-11-07 16:07:22.000000 sonusai-0.9.1/sonusai/evaluate.py
+-rw-r--r--   0        0        0     9278 2022-11-07 21:51:20.000000 sonusai-0.9.1/sonusai/genft.py
+-rw-r--r--   0        0        0     9588 2022-10-31 20:32:13.000000 sonusai-0.9.1/sonusai/genmix.py
+-rw-r--r--   0        0        0    27521 2022-11-07 21:50:37.000000 sonusai-0.9.1/sonusai/genmixdb.py
+-rw-r--r--   0        0        0    18005 2022-10-05 20:04:39.000000 sonusai-0.9.1/sonusai/gentcst.py
+-rw-r--r--   0        0        0     2650 2022-10-13 04:31:20.000000 sonusai-0.9.1/sonusai/keras_onnx.py
+-rw-r--r--   0        0        0     9212 2022-10-17 20:42:32.000000 sonusai-0.9.1/sonusai/keras_predict.py
+-rw-r--r--   0        0        0    11515 2022-10-19 20:03:59.000000 sonusai-0.9.1/sonusai/keras_train.py
+-rw-r--r--   0        0        0     8240 2022-11-07 16:08:11.000000 sonusai-0.9.1/sonusai/lsdb.py
+-rw-r--r--   0        0        0     2393 2022-10-31 18:51:33.000000 sonusai-0.9.1/sonusai/main.py
+-rw-r--r--   0        0        0      631 2022-09-09 14:39:10.000000 sonusai-0.9.1/sonusai/metrics/__init__.py
+-rw-r--r--   0        0        0      834 2022-01-11 21:05:04.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0      753 2022-09-12 19:05:56.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1041 2022-01-07 09:03:29.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/averages.cpython-36.pyc
+-rw-r--r--   0        0        0     1027 2022-02-03 16:00:13.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/averages.cpython-38.pyc
+-rw-r--r--   0        0        0      741 2022-01-11 21:05:04.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_class_weights.cpython-36.pyc
+-rw-r--r--   0        0        0     3267 2022-10-13 17:21:53.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_class_weights.cpython-38.pyc
+-rw-r--r--   0        0        0     1641 2022-01-11 21:05:04.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_metrics.cpython-36.pyc
+-rw-r--r--   0        0        0     1583 2022-04-01 03:54:51.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     2223 2022-10-13 19:22:17.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_optimal_thresholds.cpython-38.pyc
+-rw-r--r--   0        0        0      512 2022-01-11 21:05:04.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_sample_weights.cpython-36.pyc
+-rw-r--r--   0        0        0      977 2022-05-11 18:02:59.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/calculate_sample_weights.cpython-38.pyc
+-rw-r--r--   0        0        0     2661 2022-10-11 05:15:48.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/class_summary.cpython-38.pyc
+-rw-r--r--   0        0        0     2535 2022-10-11 05:15:48.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/confusion_matrix_summary.cpython-38.pyc
+-rw-r--r--   0        0        0     1116 2021-12-31 18:06:31.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/confusion_matrix_to_string.cpython-36.pyc
+-rw-r--r--   0        0        0     1121 2022-03-02 19:44:50.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/confusion_matrix_to_string.cpython-38.pyc
+-rw-r--r--   0        0        0      435 2021-12-31 18:06:31.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/format_confusion_matrix.cpython-36.pyc
+-rw-r--r--   0        0        0      423 2022-03-02 19:44:50.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/format_confusion_matrix.cpython-38.pyc
+-rw-r--r--   0        0        0     1597 2022-01-06 22:07:24.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/generate_snr_summary.cpython-36.pyc
+-rw-r--r--   0        0        0     1638 2022-03-02 19:44:50.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/generate_snr_summary.cpython-38.pyc
+-rw-r--r--   0        0        0     2471 2022-01-11 01:31:39.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/generate_summary.cpython-36.pyc
+-rw-r--r--   0        0        0     2614 2022-02-03 16:00:13.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/generate_summary.cpython-38.pyc
+-rw-r--r--   0        0        0     1750 2022-01-11 21:05:04.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/one_hot.cpython-36.pyc
+-rw-r--r--   0        0        0     6752 2022-10-13 19:22:17.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/one_hot.cpython-38.pyc
+-rw-r--r--   0        0        0     3473 2022-11-01 19:44:19.000000 sonusai-0.9.1/sonusai/metrics/__pycache__/snr_summary.cpython-38.pyc
+-rw-r--r--   0        0        0     3927 2022-10-13 17:19:27.000000 sonusai-0.9.1/sonusai/metrics/calculate_class_weights.py
+-rw-r--r--   0        0        0     3196 2022-10-13 19:22:06.000000 sonusai-0.9.1/sonusai/metrics/calculate_optimal_thresholds.py
+-rw-r--r--   0        0        0      938 2022-05-11 15:57:59.000000 sonusai-0.9.1/sonusai/metrics/calculate_sample_weights.py
+-rw-r--r--   0        0        0     3138 2022-10-11 04:54:25.000000 sonusai-0.9.1/sonusai/metrics/class_summary.py
+-rw-r--r--   0        0        0     3751 2022-10-11 04:54:56.000000 sonusai-0.9.1/sonusai/metrics/confusion_matrix_summary.py
+-rw-r--r--   0        0        0    12965 2022-10-13 19:22:06.000000 sonusai-0.9.1/sonusai/metrics/one_hot.py
+-rw-r--r--   0        0        0     5242 2022-11-01 19:38:41.000000 sonusai-0.9.1/sonusai/metrics/snr_summary.py
+-rw-r--r--   0        0        0     5336 2022-11-07 21:49:44.000000 sonusai-0.9.1/sonusai/mixture/__init__.py
+-rw-r--r--   0        0        0     1350 2022-01-13 21:48:57.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     4506 2022-11-07 21:54:38.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2266 2022-01-13 21:48:57.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/audio_db.cpython-36.pyc
+-rw-r--r--   0        0        0     8181 2022-11-07 16:28:59.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/audio_db.cpython-38.pyc
+-rw-r--r--   0        0        0     6624 2022-10-11 03:37:32.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/augmentation.cpython-38.pyc
+-rw-r--r--   0        0        0      614 2022-09-14 01:22:04.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/balance.cpython-38.pyc
+-rw-r--r--   0        0        0     2107 2022-10-11 04:39:39.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/class_count.cpython-38.pyc
+-rw-r--r--   0        0        0    11283 2022-11-07 16:45:25.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0     1112 2022-11-07 15:48:12.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0        0        0     1217 2022-09-14 01:22:04.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/dataclasses_sonusai.cpython-38.pyc
+-rw-r--r--   0        0        0      558 2022-07-09 21:23:51.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/estimate_audio_length.cpython-38.pyc
+-rw-r--r--   0        0        0     5816 2022-11-07 16:42:57.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/feature.cpython-38.pyc
+-rw-r--r--   0        0        0     1025 2022-07-09 21:23:51.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/generate_segsnr.cpython-38.pyc
+-rw-r--r--   0        0        0     1179 2022-07-09 21:23:51.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/get_mixtures_from_mixid.cpython-38.pyc
+-rw-r--r--   0        0        0      829 2022-07-09 21:23:51.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/get_targets_for_truth_index.cpython-38.pyc
+-rw-r--r--   0        0        0     2501 2022-07-09 21:23:52.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/input_files.cpython-38.pyc
+-rw-r--r--   0        0        0      789 2022-07-09 21:23:52.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/load_mixdb.cpython-38.pyc
+-rw-r--r--   0        0        0      755 2022-07-09 21:23:52.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/load_mixid.cpython-38.pyc
+-rw-r--r--   0        0        0     1154 2022-08-09 21:25:00.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/log_duration_and_sizes.cpython-38.pyc
+-rw-r--r--   0        0        0     1676 2022-09-13 01:08:21.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/mapped_snr_f.cpython-38.pyc
+-rw-r--r--   0        0        0    11924 2022-11-07 21:54:38.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/mixdb.cpython-38.pyc
+-rw-r--r--   0        0        0     4063 2022-07-09 21:23:52.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/mixture_data.cpython-38.pyc
+-rw-r--r--   0        0        0     3351 2022-10-11 04:39:39.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/process.cpython-38.pyc
+-rw-r--r--   0        0        0     1172 2022-08-09 21:25:00.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/segment.cpython-38.pyc
+-rw-r--r--   0        0        0     1129 2022-11-07 16:28:59.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/segsnr.cpython-38.pyc
+-rw-r--r--   0        0        0     2791 2022-08-25 12:27:45.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/target_class_balancing.cpython-38.pyc
+-rw-r--r--   0        0        0     5022 2022-10-03 13:13:19.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/targets.cpython-38.pyc
+-rw-r--r--   0        0        0     6915 2022-11-07 21:54:38.000000 sonusai-0.9.1/sonusai/mixture/__pycache__/truth.cpython-38.pyc
+-rw-r--r--   0        0        0     8453 2022-10-19 20:14:46.000000 sonusai-0.9.1/sonusai/mixture/active_truth_class_balancing.py
+-rw-r--r--   0        0        0    11758 2022-11-07 16:05:13.000000 sonusai-0.9.1/sonusai/mixture/audio_db.py
+-rw-r--r--   0        0        0     8814 2022-10-11 03:36:35.000000 sonusai-0.9.1/sonusai/mixture/augmentation.py
+-rw-r--r--   0        0        0      644 2022-09-14 01:06:01.000000 sonusai-0.9.1/sonusai/mixture/balance.py
+-rw-r--r--   0        0        0     2356 2022-10-11 04:36:39.000000 sonusai-0.9.1/sonusai/mixture/class_count.py
+-rw-r--r--   0        0        0    18537 2022-11-07 16:45:16.000000 sonusai-0.9.1/sonusai/mixture/config.py
+-rw-r--r--   0        0        0      978 2022-11-04 11:35:41.000000 sonusai-0.9.1/sonusai/mixture/constants.py
+-rw-r--r--   0        0        0     1081 2022-09-14 01:06:53.000000 sonusai-0.9.1/sonusai/mixture/dataclasses_sonusai.py
+-rw-r--r--   0        0        0     7845 2022-11-07 16:42:57.000000 sonusai-0.9.1/sonusai/mixture/feature.py
+-rw-r--r--   0        0        0     1335 2022-08-09 21:05:21.000000 sonusai-0.9.1/sonusai/mixture/log_duration_and_sizes.py
+-rw-r--r--   0        0        0     1803 2022-09-13 01:08:15.000000 sonusai-0.9.1/sonusai/mixture/mapped_snr_f.py
+-rw-r--r--   0        0        0    12321 2022-11-07 21:49:27.000000 sonusai-0.9.1/sonusai/mixture/mixdb.py
+-rw-r--r--   0        0        0     5940 2022-10-11 04:39:11.000000 sonusai-0.9.1/sonusai/mixture/process.py
+-rw-r--r--   0        0        0      622 2022-08-09 20:32:22.000000 sonusai-0.9.1/sonusai/mixture/segment.py
+-rw-r--r--   0        0        0     1431 2022-11-07 16:06:45.000000 sonusai-0.9.1/sonusai/mixture/segsnr.py
+-rw-r--r--   0        0        0     3729 2022-08-24 18:58:32.000000 sonusai-0.9.1/sonusai/mixture/target_class_balancing.py
+-rw-r--r--   0        0        0     6909 2022-09-30 19:43:01.000000 sonusai-0.9.1/sonusai/mixture/targets.py
+-rw-r--r--   0        0        0    10846 2022-11-07 19:10:48.000000 sonusai-0.9.1/sonusai/mixture/truth.py
+-rw-r--r--   0        0        0     6745 2022-11-01 16:37:26.000000 sonusai-0.9.1/sonusai/mkwav.py
+-rw-r--r--   0        0        0     8682 2022-10-21 17:47:53.000000 sonusai-0.9.1/sonusai/onnx_predict.py
+-rw-r--r--   0        0        0    16847 2022-11-01 19:39:34.000000 sonusai-0.9.1/sonusai/plot.py
+-rw-r--r--   0        0        0      474 2022-07-22 19:34:58.000000 sonusai-0.9.1/sonusai/queries/__init__.py
+-rw-r--r--   0        0        0      512 2022-07-22 21:30:41.000000 sonusai-0.9.1/sonusai/queries/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7007 2022-10-11 05:15:48.000000 sonusai-0.9.1/sonusai/queries/__pycache__/queries.cpython-38.pyc
+-rw-r--r--   0        0        0     9337 2022-10-11 04:57:36.000000 sonusai-0.9.1/sonusai/queries/queries.py
+-rw-r--r--   0        0        0       61 2022-11-07 19:10:48.000000 sonusai-0.9.1/sonusai/scratch.py
+-rwxr-xr-x   0        0        0    58027 2022-11-07 16:26:47.000000 sonusai-0.9.1/sonusai/speech_enh.py
+-rw-r--r--   0        0        0    14769 2022-10-11 01:38:14.000000 sonusai-0.9.1/sonusai/tplot.py
+-rw-r--r--   0        0        0     2201 2022-11-01 19:34:47.000000 sonusai-0.9.1/sonusai/utils/__init__.py
+-rw-r--r--   0        0        0      608 2022-01-11 21:14:24.000000 sonusai-0.9.1/sonusai/utils/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0        0        0     2365 2022-11-01 19:44:18.000000 sonusai-0.9.1/sonusai/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1247 2022-10-13 05:27:12.000000 sonusai-0.9.1/sonusai/utils/__pycache__/braced_glob.cpython-38.pyc
+-rw-r--r--   0        0        0     1329 2022-11-07 16:43:29.000000 sonusai-0.9.1/sonusai/utils/__pycache__/calculate_input_shape.cpython-38.pyc
+-rw-r--r--   0        0        0      516 2022-10-06 13:04:31.000000 sonusai-0.9.1/sonusai/utils/__pycache__/create_ts_name.cpython-38.pyc
+-rw-r--r--   0        0        0      823 2022-07-10 23:26:33.000000 sonusai-0.9.1/sonusai/utils/__pycache__/dataclass_from_dict.cpython-38.pyc
+-rw-r--r--   0        0        0      578 2022-08-09 21:25:00.000000 sonusai-0.9.1/sonusai/utils/__pycache__/dbfs.cpython-38.pyc
+-rw-r--r--   0        0        0     5355 2022-08-09 21:25:00.000000 sonusai-0.9.1/sonusai/utils/__pycache__/engineering_number.cpython-38.pyc
+-rw-r--r--   0        0        0      961 2022-08-25 12:44:35.000000 sonusai-0.9.1/sonusai/utils/__pycache__/get_label_names.cpython-38.pyc
+-rw-r--r--   0        0        0      530 2022-04-15 16:54:27.000000 sonusai-0.9.1/sonusai/utils/__pycache__/grouper.cpython-38.pyc
+-rw-r--r--   0        0        0      461 2021-12-31 18:53:36.000000 sonusai-0.9.1/sonusai/utils/__pycache__/human_readable_size.cpython-36.pyc
+-rw-r--r--   0        0        0      484 2022-04-08 12:41:11.000000 sonusai-0.9.1/sonusai/utils/__pycache__/human_readable_size.cpython-38.pyc
+-rw-r--r--   0        0        0     4232 2022-10-31 18:45:52.000000 sonusai-0.9.1/sonusai/utils/__pycache__/keras_utils.cpython-38.pyc
+-rw-r--r--   0        0        0      589 2022-11-01 19:44:18.000000 sonusai-0.9.1/sonusai/utils/__pycache__/numeric_conversion.cpython-38.pyc
+-rw-r--r--   0        0        0     2527 2022-10-28 20:51:31.000000 sonusai-0.9.1/sonusai/utils/__pycache__/onnx_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2010 2022-10-04 18:35:31.000000 sonusai-0.9.1/sonusai/utils/__pycache__/parallel.cpython-38.pyc
+-rw-r--r--   0        0        0     2090 2022-08-13 18:59:14.000000 sonusai-0.9.1/sonusai/utils/__pycache__/parallel_tqdm.cpython-38.pyc
+-rw-r--r--   0        0        0     2723 2022-11-07 21:54:38.000000 sonusai-0.9.1/sonusai/utils/__pycache__/print_mixture_details.cpython-38.pyc
+-rw-r--r--   0        0        0     1524 2022-09-08 19:52:28.000000 sonusai-0.9.1/sonusai/utils/__pycache__/ranges.cpython-38.pyc
+-rw-r--r--   0        0        0      586 2022-10-04 20:57:11.000000 sonusai-0.9.1/sonusai/utils/__pycache__/read_mixture_data.cpython-38.pyc
+-rw-r--r--   0        0        0     1057 2022-01-11 21:05:05.000000 sonusai-0.9.1/sonusai/utils/__pycache__/read_predict_data.cpython-36.pyc
+-rw-r--r--   0        0        0      965 2022-10-04 20:57:11.000000 sonusai-0.9.1/sonusai/utils/__pycache__/read_predict_data.cpython-38.pyc
+-rw-r--r--   0        0        0     4356 2022-10-13 20:44:55.000000 sonusai-0.9.1/sonusai/utils/__pycache__/reshape.cpython-38.pyc
+-rw-r--r--   0        0        0      475 2022-04-08 12:41:13.000000 sonusai-0.9.1/sonusai/utils/__pycache__/seconds_to_hms.cpython-38.pyc
+-rw-r--r--   0        0        0     4901 2022-10-05 18:35:51.000000 sonusai-0.9.1/sonusai/utils/__pycache__/stratified_shuffle_split.cpython-38.pyc
+-rw-r--r--   0        0        0      449 2022-08-09 21:25:00.000000 sonusai-0.9.1/sonusai/utils/__pycache__/to_numpy_array.cpython-38.pyc
+-rw-r--r--   0        0        0      660 2022-01-06 22:07:28.000000 sonusai-0.9.1/sonusai/utils/__pycache__/trim_docstring.cpython-36.pyc
+-rw-r--r--   0        0        0      678 2022-04-15 16:54:27.000000 sonusai-0.9.1/sonusai/utils/__pycache__/trim_docstring.cpython-38.pyc
+-rw-r--r--   0        0        0      624 2022-11-01 16:46:39.000000 sonusai-0.9.1/sonusai/utils/__pycache__/wave.cpython-38.pyc
+-rw-r--r--   0        0        0      406 2021-12-31 18:53:36.000000 sonusai-0.9.1/sonusai/utils/__pycache__/yes_or_no.cpython-36.pyc
+-rw-r--r--   0        0        0      438 2022-04-08 12:41:13.000000 sonusai-0.9.1/sonusai/utils/__pycache__/yes_or_no.cpython-38.pyc
+-rw-r--r--   0        0        0      852 2022-10-13 05:26:48.000000 sonusai-0.9.1/sonusai/utils/braced_glob.py
+-rw-r--r--   0        0        0     1423 2022-11-07 16:42:57.000000 sonusai-0.9.1/sonusai/utils/calculate_input_shape.py
+-rw-r--r--   0        0        0      405 2022-10-05 19:29:04.000000 sonusai-0.9.1/sonusai/utils/create_ts_name.py
+-rw-r--r--   0        0        0      388 2022-07-09 21:26:55.000000 sonusai-0.9.1/sonusai/utils/dataclass_from_dict.py
+-rw-r--r--   0        0        0      254 2022-08-09 20:43:35.000000 sonusai-0.9.1/sonusai/utils/dbfs.py
+-rw-r--r--   0        0        0     5551 2022-08-09 20:45:16.000000 sonusai-0.9.1/sonusai/utils/engineering_number.py
+-rw-r--r--   0        0        0      784 2022-08-25 12:41:30.000000 sonusai-0.9.1/sonusai/utils/get_label_names.py
+-rw-r--r--   0        0        0      203 2022-04-15 16:49:07.000000 sonusai-0.9.1/sonusai/utils/grouper.py
+-rw-r--r--   0        0        0      279 2022-04-07 22:57:46.000000 sonusai-0.9.1/sonusai/utils/human_readable_size.py
+-rw-r--r--   0        0        0     6685 2022-10-31 18:42:48.000000 sonusai-0.9.1/sonusai/utils/keras_utils.py
+-rw-r--r--   0        0        0      311 2022-11-01 19:34:34.000000 sonusai-0.9.1/sonusai/utils/numeric_conversion.py
+-rw-r--r--   0        0        0     2971 2022-10-28 20:04:11.000000 sonusai-0.9.1/sonusai/utils/onnx_utils.py
+-rw-r--r--   0        0        0     2005 2022-10-04 18:35:20.000000 sonusai-0.9.1/sonusai/utils/parallel.py
+-rw-r--r--   0        0        0     2039 2022-08-09 23:00:09.000000 sonusai-0.9.1/sonusai/utils/parallel_tqdm.py
+-rw-r--r--   0        0        0     2904 2022-11-07 21:53:30.000000 sonusai-0.9.1/sonusai/utils/print_mixture_details.py
+-rw-r--r--   0        0        0     1089 2022-09-08 19:52:17.000000 sonusai-0.9.1/sonusai/utils/ranges.py
+-rw-r--r--   0        0        0      392 2022-10-04 20:31:09.000000 sonusai-0.9.1/sonusai/utils/read_mixture_data.py
+-rw-r--r--   0        0        0     1021 2022-10-04 20:31:09.000000 sonusai-0.9.1/sonusai/utils/read_predict_data.py
+-rw-r--r--   0        0        0     7349 2022-10-13 20:13:40.000000 sonusai-0.9.1/sonusai/utils/reshape.py
+-rw-r--r--   0        0        0      260 2022-04-07 22:57:46.000000 sonusai-0.9.1/sonusai/utils/seconds_to_hms.py
+-rw-r--r--   0        0        0     6833 2022-10-05 18:32:03.000000 sonusai-0.9.1/sonusai/utils/stratified_shuffle_split.py
+-rw-r--r--   0        0        0      220 2022-08-09 20:54:37.000000 sonusai-0.9.1/sonusai/utils/to_numpy_array.py
+-rw-r--r--   0        0        0      881 2022-04-15 16:49:06.000000 sonusai-0.9.1/sonusai/utils/trim_docstring.py
+-rw-r--r--   0        0        0      409 2022-11-01 16:31:50.000000 sonusai-0.9.1/sonusai/utils/wave.py
+-rw-r--r--   0        0        0      282 2022-04-07 22:57:46.000000 sonusai-0.9.1/sonusai/utils/yes_or_no.py
+-rw-r--r--   0        0        0      517 2022-11-07 16:09:07.000000 sonusai-0.9.1/sonusai/vars.py
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 sonusai-0.9.1/setup.py
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 sonusai-0.9.1/PKG-INFO
```

### Comparing `sonusai-0.8.8/README.rst` & `sonusai-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/pyproject.toml` & `sonusai-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sonusai"
-version = "0.8.8"
+version = "0.9.1"
 description = "Framework for building deep neural network models for sound, speech, and voice AI"
 authors = ["Chris Eddington <chris@aaware.com>", "Jason Calderwood <jason@aaware.com>"]
 maintainers = ["Chris Eddington <chris@aaware.com>", "Jason Calderwood <jason@aaware.com>"]
 homepage = "https://aaware.com"
 license = "GPL-3.0-only"
 readme = "README.rst"
 include = ["sonusai/data/genmixdb.yml", "sonusai/data/whitenoise.wav"]
```

### Comparing `sonusai-0.8.8/sonusai/__init__.py` & `sonusai-0.9.1/sonusai/__init__.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/aawscd_probwrite.py` & `sonusai-0.9.1/sonusai/aawscd_probwrite.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/data/genmixdb.yml` & `sonusai-0.9.1/sonusai/data/genmixdb.yml`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,25 @@
 # Output file name; "${config}" will be expanded to the name of the local config
 # file
 output: "${config}"
 
 # Feature to use
 feature: ""
 
-# Transform frame size
-frame_size: "${frame_size}"
+# Forward transform config
+ftransform:
+  N: 256
+  R: 64
+  ttype: stft-olsa-hanns
+
+# Inverse transform config
+itransform:
+  N: 256
+  R: 64
+  ttype: stft-olsa-hanns
 
 # Targets list
 #
 # Required field:
 #
 #   'name'
 #                     File name. May be one of the following:
```

### Comparing `sonusai-0.8.8/sonusai/data/whitenoise.wav` & `sonusai-0.9.1/sonusai/data/whitenoise.wav`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/data_generator/keras_from_h5.py` & `sonusai-0.9.1/sonusai/data_generator/keras_from_h5.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 datasets = ['feature', 'truth_f']
                 for dataset in datasets:
                     if dataset not in f:
                         raise SonusAIError(f'Could not find "{dataset}" in {filename}')
 
         fs = get_feature_stats(feature=self.mixdb.feature,
                                num_classes=self.mixdb.num_classes,
-                               frame_size=self.mixdb.frame_size)
+                               frame_size=self.mixdb.ftransform.R)
 
         self.stride = fs.stride
         self.num_bands = fs.num_bands
         self.num_classes = self.mixdb.num_classes
         self.mrecords = None
         self.mixture_frame_segments = None
         self.batch_frame_segments = None
```

### Comparing `sonusai-0.8.8/sonusai/data_generator/keras_from_mixdb.py` & `sonusai-0.9.1/sonusai/data_generator/keras_from_mixdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.add1ch = add1ch
         self.shuffle = shuffle
         self.raw_target_audios = get_raw_audios(self.mixdb)
         self.augmented_noise_audios = get_augmented_noise_audios(self.mixdb)
 
         fs = get_feature_stats(feature=self.mixdb.feature,
                                num_classes=self.mixdb.num_classes,
-                               frame_size=self.mixdb.frame_size)
+                               frame_size=self.mixdb.ftransform.R)
 
         self.stride = fs.stride
         self.num_bands = fs.num_bands
         self.num_classes = self.mixdb.num_classes
         self.mixtures = None
         self.mixture_frame_segments = None
         self.batch_frame_segments = None
```

### Comparing `sonusai-0.8.8/sonusai/data_generator/sequence_from_h5.py` & `sonusai-0.9.1/sonusai/data_generator/sequence_from_h5.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/data_generator/utils.py` & `sonusai-0.9.1/sonusai/data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/evaluate.py` & `sonusai-0.9.1/sonusai/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     if fdiff < 0:
         predict = predict[0:fdiff, :]
         logger.info(f'Predict has more feature-frames than truth, trimming predict to match.')
 
     # Check segsnr, input is always in transform frames
     compute_segsnr = False
     if len(segsnr) > 0:
-        segsnr_feature_frames = segsnr.shape[0] / (mixdb.feature_step_samples / mixdb.frame_size)
+        segsnr_feature_frames = segsnr.shape[0] / (mixdb.feature_step_samples / mixdb.ftransform.R)
         if segsnr_feature_frames == truth.shape[0]:
             compute_segsnr = True
         else:
             logger.warning('segsnr length does not match truth, ignoring.')
 
     # Check pred_thr array or scalar and return final scalar pred_thr value
     if not mixdb.truth_mutex:
```

### Comparing `sonusai-0.8.8/sonusai/genft.py` & `sonusai-0.9.1/sonusai/genft.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
 
 def _process_mixture(mixid: int) -> None:
     from os.path import join
 
     import h5py
 
+    from sonusai.mixture import add_feature_truth_to_h5
     from sonusai.mixture import get_mixid_padded_name
     from sonusai.mixture import get_mixture_metadata
 
     mixdb = MP_DICT['mixdb']
     compute_segsnr = MP_DICT['compute_segsnr']
     mixid_padded_name = get_mixid_padded_name(mixdb, mixid)
     output_base = join(MP_DICT['output_dir'], mixid_padded_name)
@@ -129,25 +130,19 @@
                                          raw_target_audios=MP_DICT['raw_target_audios'],
                                          augmented_noise_audios=MP_DICT['augmented_noise_audios'],
                                          mixture=mixture_t,
                                          truth_t=truth_t,
                                          segsnr_t=segsnr_t,
                                          compute_segsnr=compute_segsnr)
 
-        datasets = ['feature', 'truth_f', 'segsnr']
-        for dataset in datasets:
-            if dataset in f:
-                del f[dataset]
-
-        f.create_dataset(name='feature', data=feature, dtype=np.single)
-        f.create_dataset(name='truth_f',
-                         data=truth_f,
-                         dtype=np.csingle if np.iscomplex(truth_f).any() else np.single)
-        if compute_segsnr:
-            f.create_dataset(name='segsnr', data=segsnr, dtype=np.single)
+        add_feature_truth_to_h5(file=f,
+                                feature=feature,
+                                truth_f=truth_f,
+                                segsnr=segsnr,
+                                save_segsnr=compute_segsnr)
 
     with open(file=output_base + '.txt', mode='w') as f:
         f.write(get_mixture_metadata(mixdb, mixdb.mixtures[mixid]))
 
 
 def main():
     import time
@@ -200,26 +195,26 @@
 
     logger.info(f'\nLoad mixture database from {mixdb_name}')
     mixdb = load_mixdb(name=mixdb_name)
     mixid = convert_mixids_to_list(mixdb, mixid)
 
     total_samples = sum([sub.samples for sub in [mixdb.mixtures[m] for m in mixid]])
     duration = total_samples / sonusai.mixture.SAMPLE_RATE
-    total_transform_frames = total_samples // mixdb.frame_size
+    total_transform_frames = total_samples // mixdb.ftransform.R
     total_feature_frames = total_samples // mixdb.feature_step_samples
 
     logger.info('')
     logger.info(f'Found {len(mixid):,} mixtures to process')
     logger.info(f'{total_samples:,} samples, '
                 f'{total_transform_frames:,} transform frames, '
                 f'{total_feature_frames:,} feature frames')
 
     check_audio_files_exist(mixdb)
 
-    fg = FeatureGenerator(frame_size=mixdb.frame_size,
+    fg = FeatureGenerator(frame_size=mixdb.ftransform.R,
                           feature_mode=mixdb.feature,
                           num_classes=mixdb.num_classes,
                           truth_mutex=mixdb.truth_mutex)
 
     MP_DICT['mixdb'] = mixdb
     MP_DICT['output_dir'] = output_dir
     MP_DICT['raw_target_audios'] = get_raw_audios(mixdb)
```

### Comparing `sonusai-0.8.8/sonusai/genmix.py` & `sonusai-0.9.1/sonusai/genmix.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/genmixdb.py` & `sonusai-0.9.1/sonusai/genmixdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,29 +233,30 @@
     truth_mutex = config['truth_mode'] == 'mutex'
 
     if truth_mutex and any(mixup > 1 for mixup in mixups):
         raise SonusAIError(f'Mutex truth mode is not compatible with mixup')
 
     fs = get_feature_stats(feature=config['feature'],
                            num_classes=config['num_classes'],
-                           frame_size=config['frame_size'])
+                           frame_size=config['ftransform'].R)
 
     augmented_targets = get_augmented_targets(target_files, target_augmentations)
 
     mixdb = MixtureDatabase(
         class_balancing=config['class_balancing'],
         class_balancing_augmentation=dataclass_from_dict(Augmentation, config['class_balancing_augmentation']),
         class_labels=config['class_labels'],
         class_weights_threshold=get_class_weights_threshold(config),
         exhaustive_noise=config['exhaustive_noise'],
         feature=config['feature'],
         feature_samples=fs.feature_samples,
         feature_step_samples=fs.feature_step_samples,
         first_cba_index=len(target_augmentations),
-        frame_size=config['frame_size'],
+        ftransform=config['ftransform'],
+        itransform=config['itransform'],
         mixtures=[],
         noise_augmentations=noise_augmentations,
         noises=noise_files,
         num_classes=config['num_classes'],
         random_snrs=config['random_snrs'],
         seed=config['seed'],
         snrs=config['snrs'],
@@ -530,14 +531,15 @@
 
 def _process_mixture(mixid: int) -> MRecord:
     from os.path import join
 
     import h5py
 
     from sonusai.genft import genft
+    from sonusai.mixture import add_feature_truth_to_h5
     from sonusai.mixture import get_mixid_padded_name
     from sonusai.mixture import get_mixture_metadata
     from sonusai.mixture import process_mixture
 
     mrecord = MP_DICT['mixdb'].mixtures[mixid]
 
     (mrecord,
@@ -570,28 +572,22 @@
                                              raw_target_audios=MP_DICT['raw_target_audios'],
                                              augmented_noise_audios=MP_DICT['augmented_noise_audios'],
                                              mixture=mixture,
                                              truth_t=truth_t,
                                              compute_segsnr=MP_DICT['save_segsnr'])
 
             with h5py.File(output_base + '.h5', 'a') as f:
-                datasets = ['feature', 'truth_f', 'segsnr']
-                for dataset in datasets:
-                    if dataset in f:
-                        del f[dataset]
-
-                f.create_dataset(name='feature', data=feature, dtype=np.single)
-                f.create_dataset(name='truth_f',
-                                 data=truth_f,
-                                 dtype=np.csingle if np.iscomplex(truth_f).any() else np.single)
-                if MP_DICT['save_segsnr']:
-                    f.create_dataset(name='segsnr', data=segsnr, dtype=np.single)
+                add_feature_truth_to_h5(file=f,
+                                        feature=feature,
+                                        truth_f=truth_f,
+                                        segsnr=segsnr,
+                                        save_segsnr=MP_DICT['save_segsnr'])
 
         with open(file=output_base + '.txt', mode='w') as f:
-            f.write(get_mixture_metadata(MP_DICT['mixdb'], MP_DICT['mixdb'].mixtures[mixid]))
+            f.write(get_mixture_metadata(MP_DICT['mixdb'], mrecord))
 
     return mrecord
 
 
 def main():
     import time
     from os import makedirs
```

### Comparing `sonusai-0.8.8/sonusai/gentcst.py` & `sonusai-0.9.1/sonusai/gentcst.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/keras_onnx.py` & `sonusai-0.9.1/sonusai/keras_onnx.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/keras_predict.py` & `sonusai-0.9.1/sonusai/keras_predict.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/keras_train.py` & `sonusai-0.9.1/sonusai/keras_train.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/lsdb.py` & `sonusai-0.9.1/sonusai/lsdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if f_frames != t_frames:
             logger.warn(f'Number of feature frames, {f_frames} does not match number of truth frames, {t_frames}.')
 
     total_samples = sum([sub.samples for sub in mixdb.mixtures])
     total_duration = total_samples / SAMPLE_RATE
     fs = get_feature_stats(feature=mixdb.feature,
                            num_classes=mixdb.num_classes,
-                           frame_size=mixdb.frame_size)
+                           frame_size=mixdb.ftransform.R)
 
     logger.info(f'{"Mixtures":{desc_len}} {len(mixdb.mixtures)}')
     logger.info(f'{"Duration":{desc_len}} {seconds_to_hms(seconds=total_duration)}')
     logger.info(f'{"Targets":{desc_len}} {len(mixdb.targets)}')
     logger.info(f'{"Target augmentations":{desc_len}} {len(mixdb.target_augmentations)}')
     logger.info(f'{"Noise augmentations":{desc_len}} {len(mixdb.noise_augmentations)}')
     logger.info(f'{"Noises":{desc_len}} {len(mixdb.noises)}')
```

### Comparing `sonusai-0.8.8/sonusai/main.py` & `sonusai-0.9.1/sonusai/main.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/__init__.py` & `sonusai-0.9.1/sonusai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/calculate_class_weights.py` & `sonusai-0.9.1/sonusai/metrics/calculate_class_weights.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/calculate_optimal_thresholds.py` & `sonusai-0.9.1/sonusai/metrics/calculate_optimal_thresholds.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/calculate_sample_weights.py` & `sonusai-0.9.1/sonusai/metrics/calculate_sample_weights.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/class_summary.py` & `sonusai-0.9.1/sonusai/metrics/class_summary.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/confusion_matrix_summary.py` & `sonusai-0.9.1/sonusai/metrics/confusion_matrix_summary.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/one_hot.py` & `sonusai-0.9.1/sonusai/metrics/one_hot.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/metrics/snr_summary.py` & `sonusai-0.9.1/sonusai/metrics/snr_summary.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/__init__.py` & `sonusai-0.9.1/sonusai/mixture/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 from sonusai.mixture.config import tokenized_expandvars
 from sonusai.mixture.config import update_config_from_file
 from sonusai.mixture.config import update_config_from_hierarchy
 from sonusai.mixture.config import update_truth_settings
 from sonusai.mixture.constants import BIT_DEPTH
 from sonusai.mixture.constants import CHANNEL_COUNT
 from sonusai.mixture.constants import DEFAULT_CONFIG
-from sonusai.mixture.constants import DEFAULT_FRAME_SIZE
 from sonusai.mixture.constants import DEFAULT_NOISE
 from sonusai.mixture.constants import FLOAT_BYTES
 from sonusai.mixture.constants import RAND_PATTERN
 from sonusai.mixture.constants import REQUIRED_CONFIGS
 from sonusai.mixture.constants import SAMPLE_BYTES
 from sonusai.mixture.constants import SAMPLE_RATE
 from sonusai.mixture.constants import VALID_AUGMENTATIONS
@@ -58,15 +57,18 @@
 from sonusai.mixture.mixdb import AugmentedTargets
 from sonusai.mixture.mixdb import MRecord
 from sonusai.mixture.mixdb import MRecords
 from sonusai.mixture.mixdb import MixtureDatabase
 from sonusai.mixture.mixdb import MixtureIDs
 from sonusai.mixture.mixdb import TargetFile
 from sonusai.mixture.mixdb import TargetFiles
+from sonusai.mixture.mixdb import TransformConfig
+from sonusai.mixture.mixdb import TruthFunctionConfig
 from sonusai.mixture.mixdb import TruthSettings
+from sonusai.mixture.mixdb import add_feature_truth_to_h5
 from sonusai.mixture.mixdb import convert_json_to_mixdb
 from sonusai.mixture.mixdb import convert_mixids_to_list
 from sonusai.mixture.mixdb import evaluate_random_rule
 from sonusai.mixture.mixdb import get_class_weights_threshold
 from sonusai.mixture.mixdb import get_feature_frames_in_mrecord
 from sonusai.mixture.mixdb import get_file_frame_segments
 from sonusai.mixture.mixdb import get_mixid_padded_name
```

### Comparing `sonusai-0.8.8/sonusai/mixture/active_truth_class_balancing.py` & `sonusai-0.9.1/sonusai/mixture/active_truth_class_balancing.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/audio_db.py` & `sonusai-0.9.1/sonusai/mixture/audio_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
         augmented_noise_audios = get_augmented_noise_audios(mixdb)
 
     target_file_index = mrecord.target_file_index
     target_augmentation_index = mrecord.target_augmentation_index
     if len(target_file_index) != len(target_augmentation_index):
         raise SonusAIError('target_file_index and target_augmentation_index are not the same length')
 
-    if mrecord.samples % mixdb.frame_size != 0:
-        raise SonusAIError(f'Number of samples in mixture is not a multiple of {mixdb.frame_size}')
+    if mrecord.samples % mixdb.ftransform.R != 0:
+        raise SonusAIError(f'Number of samples in mixture is not a multiple of {mixdb.ftransform.R}')
 
     targets = []
     for idx in range(len(target_file_index)):
         target_augmentation = mixdb.target_augmentations[target_augmentation_index[idx]]
 
         target = apply_augmentation(audio_in=raw_target_audios[target_file_index[idx]],
                                     augmentation=target_augmentation,
```

### Comparing `sonusai-0.8.8/sonusai/mixture/augmentation.py` & `sonusai-0.9.1/sonusai/mixture/augmentation.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/balance.py` & `sonusai-0.9.1/sonusai/mixture/balance.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/class_count.py` & `sonusai-0.9.1/sonusai/mixture/class_count.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/config.py` & `sonusai-0.9.1/sonusai/mixture/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,26 @@
 from typing import Union
 
 from sonusai.mixture.mixdb import NoiseFiles
 from sonusai.mixture.mixdb import TargetFiles
 
 
 def raw_load_config(name: str) -> Dict:
-    """Load YAML file with SonusAI variable substitution."""
+    """Load YAML file."""
     import yaml
 
+    from sonusai.mixture.mixdb import TransformConfig
+
     with open(file=name, mode='r') as f:
         config = yaml.safe_load(f)
 
-    return config_variable_substitution(config)
-
-
-def config_variable_substitution(config: Dict) -> Dict:
-    """Find custom SonusAI variables in given dictionary and substitute their values in place."""
-    import json
-
-    from sonusai.mixture import DEFAULT_FRAME_SIZE
+    for key in ['ftransform', 'itransform']:
+        if key in config:
+            config[key] = TransformConfig(**config[key])
 
-    result = json.dumps(config)
-    result = result.replace('"${frame_size}"', str(DEFAULT_FRAME_SIZE))
-    config = json.loads(result)
     return config
 
 
 def get_default_config() -> Dict:
     """Load default SonusAI config."""
     from sonusai import SonusAIError
     from sonusai.mixture import DEFAULT_CONFIG
```

### Comparing `sonusai-0.8.8/sonusai/mixture/constants.py` & `sonusai-0.9.1/sonusai/mixture/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 REQUIRED_CONFIGS = [
     'class_balancing',
     'class_balancing_augmentation',
     'class_labels',
     'class_weights_threshold',
     'exhaustive_noise',
     'feature',
-    'frame_size',
     'noise_augmentations',
     'noises',
     'num_classes',
     'random_snrs',
     'seed',
     'snrs',
     'target_augmentations',
@@ -28,11 +27,10 @@
 VALID_AUGMENTATIONS = ['normalize', 'gain', 'pitch', 'tempo', 'eq1', 'eq2', 'eq3', 'lpf', 'count', 'mixup']
 RAND_PATTERN = re.compile(r'rand\(([-+]?(\d+(\.\d*)?|\.\d+)),\s*([-+]?(\d+(\.\d*)?|\.\d+))\)')
 SAMPLE_RATE = 16000
 BIT_DEPTH = 16
 CHANNEL_COUNT = 1
 SAMPLE_BYTES = int(BIT_DEPTH / 8)
 FLOAT_BYTES = 4
-DEFAULT_FRAME_SIZE = 64
 
 DEFAULT_NOISE = os.path.join(sonusai.BASEDIR, 'data', 'whitenoise.wav')
 DEFAULT_CONFIG = os.path.join(sonusai.BASEDIR, 'data', 'genmixdb.yml')
```

### Comparing `sonusai-0.8.8/sonusai/mixture/dataclasses_sonusai.py` & `sonusai-0.9.1/sonusai/mixture/dataclasses_sonusai.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/feature.py` & `sonusai-0.9.1/sonusai/mixture/feature.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
 from os import PathLike
 from typing import List
 from typing import Union
 
 import numpy as np
 
-from sonusai.mixture import DEFAULT_FRAME_SIZE
 from sonusai.mixture.mixdb import MRecord
 from sonusai.mixture.mixdb import MixtureDatabase
 from sonusai.mixture.mixdb import MixtureIDs
+from sonusai.mixture.mixdb import TransformConfig
 
 MP_DICT = {}
 
 
 def _get_ft_from_dir_kernel(mixid: int) -> (np.ndarray, np.ndarray):
     """Get feature/truth for a given mixid from a directory containing genft data"""
     from os.path import join
@@ -44,28 +44,35 @@
 
     feature = np.vstack([result[i][0] for i in range(len(result))])
     truth_f = np.vstack([result[i][1] for i in range(len(result))])
 
     return feature, truth_f
 
 
-def get_feature_from_audio(audio: np.ndarray, feature: str) -> np.ndarray:
+def get_feature_from_audio(audio: np.ndarray, feature: str, ftransform: TransformConfig = None) -> np.ndarray:
     from sonusai.mixture import get_pad_length
     from sonusai.mixture import MRecord
 
     fs = get_feature_stats(feature=feature, num_classes=1)
     audio = np.pad(array=audio,
                    pad_width=(0, get_pad_length(len(audio), fs.feature_step_samples)),
                    mode='constant',
                    constant_values=0)
+
+    if ftransform is None:
+        from sonusai.mixture import get_default_config
+
+        config = get_default_config()
+        ftransform = TransformConfig(**config['ftransform'])
+
     mixdb = MixtureDatabase(feature=feature,
                             mixtures=[MRecord(samples=len(audio))],
                             feature_samples=fs.feature_samples,
                             feature_step_samples=fs.feature_step_samples,
-                            frame_size=DEFAULT_FRAME_SIZE,
+                            ftransform=ftransform,
                             num_classes=1,
                             truth_mutex=False,
                             truth_reduction_function='max')
     feature, _, _ = get_feature_and_truth_f(mixdb=mixdb,
                                             mrecord=mixdb.mixtures[0],
                                             mixture=audio,
                                             compute_truth=False)
@@ -117,18 +124,17 @@
                                          compute_truth=compute_truth,
                                          compute_segsnr=compute_segsnr,
                                          frame_based_segsnr=True)
 
     if len(mixture) != mrecord.samples:
         raise SonusAIError(f'Wrong number of samples in mixture')
 
-    fft = ForwardTransform(N=mixdb.frame_size * 4,
-                           R=mixdb.frame_size)
+    fft = ForwardTransform(N=mixdb.ftransform.N, R=mixdb.ftransform.R, ttype=mixdb.ftransform.ttype)
 
-    fg = FeatureGenerator(frame_size=mixdb.frame_size,
+    fg = FeatureGenerator(frame_size=fft.R,
                           feature_mode=mixdb.feature,
                           num_classes=mixdb.num_classes,
                           truth_mutex=mixdb.truth_mutex)
 
     transform_frames = get_transform_frames_in_mrecord(mixdb, mrecord)
     feature_frames = get_feature_frames_in_mrecord(mixdb, mrecord)
 
@@ -136,16 +142,16 @@
         truth_t = np.zeros((mrecord.samples, mixdb.num_classes), dtype=np.single)
 
     feature = np.empty((feature_frames, fg.stride, fg.num_bands), dtype=np.single)
     truth_f = np.empty((feature_frames, mixdb.num_classes), dtype=np.csingle)
 
     feature_frame = 0
     for transform_frame in range(transform_frames):
-        indices = slice(transform_frame * mixdb.frame_size,
-                        (transform_frame + 1) * mixdb.frame_size)
+        indices = slice(transform_frame * mixdb.ftransform.R,
+                        (transform_frame + 1) * mixdb.ftransform.R)
         fd = fft.execute(int16_to_float(mixture[indices]))
 
         fg.execute(fd, truth_reduction(truth_t[indices], mixdb.truth_reduction_function))
 
         if fg.eof():
             feature[feature_frame] = fg.feature()
             truth_f[feature_frame] = fg.truth()
@@ -167,22 +173,28 @@
     stride: int
     step: int
     decimation: int
 
 
 def get_feature_stats(feature: str,
                       num_classes: int,
-                      frame_size: int = DEFAULT_FRAME_SIZE) -> FeatureStats:
+                      frame_size: int = None) -> FeatureStats:
     import h5py
     from pyaaware import FeatureGenerator
 
     import sonusai
 
-    fg = FeatureGenerator(feature_mode=feature,
-                          frame_size=frame_size,
+    if frame_size is None:
+        from sonusai.mixture import get_default_config
+
+        config = get_default_config()
+        frame_size = config['ftransform'].R
+
+    fg = FeatureGenerator(frame_size=frame_size,
+                          feature_mode=feature,
                           num_classes=num_classes)
 
     transform_frame_ms = float(frame_size) / float(sonusai.mixture.SAMPLE_RATE / 1000)
 
     return FeatureStats(feature_ms=transform_frame_ms * fg.decimation * fg.stride,
                         feature_samples=frame_size * fg.decimation * fg.stride,
                         feature_step_ms=transform_frame_ms * fg.decimation * fg.step,
```

### Comparing `sonusai-0.8.8/sonusai/mixture/log_duration_and_sizes.py` & `sonusai-0.9.1/sonusai/mixture/log_duration_and_sizes.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/mapped_snr_f.py` & `sonusai-0.9.1/sonusai/mixture/mapped_snr_f.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/mixdb.py` & `sonusai-0.9.1/sonusai/mixture/mixdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
+import h5py
 import numpy as np
 
 from sonusai.mixture.dataclasses_sonusai import DataClassSonusAIMixin
 from sonusai.mixture.segment import Segment
 
 
 @dataclass(frozen=True)
@@ -91,27 +92,35 @@
 
 
 MRecords = List[MRecord]
 
 MixtureIDs = Union[str, int, List[int], range]
 
 
+@dataclass(frozen=True)
+class TransformConfig(DataClassSonusAIMixin):
+    N: int
+    R: int
+    ttype: str
+
+
 @dataclass
 class MixtureDatabase(DataClassSonusAIMixin):
     class_balancing: Optional[bool] = False
     class_balancing_augmentation: Optional[Augmentation] = None
     class_count: ClassCount = None
     class_labels: List[str] = None
     class_weights_threshold: List[float] = None
     exhaustive_noise: Optional[bool] = True
     feature: str = None
     feature_samples: int = None
     feature_step_samples: int = None
     first_cba_index: Optional[int] = None
-    frame_size: int = None
+    ftransform: TransformConfig = None
+    itransform: TransformConfig = None
     mixid_padding: Optional[int] = None
     mixtures: MRecords = None
     noise_augmentations: Augmentations = None
     noises: NoiseFiles = None
     num_classes: int = None
     random_snrs: Optional[List[str]] = None
     seed: Optional[int] = 0
@@ -119,14 +128,25 @@
     target_augmentations: Augmentations = None
     targets: TargetFiles = None
     truth_mutex: bool = None
     truth_reduction_function: str = None
     truth_settings: TruthSettings = None
 
 
+@dataclass(frozen=True)
+class TruthFunctionConfig(DataClassSonusAIMixin):
+    ftransform: TransformConfig
+    num_classes: int
+    mutex: bool
+    target_gain: float
+    index: Optional[List[int]] = None
+    function: Optional[str] = None
+    config: Optional[dict] = None
+
+
 def convert_json_to_mixdb(data: str) -> MixtureDatabase:
     import json
 
     return MixtureDatabase.from_dict(json.loads(data))
 
 
 def load_mixdb(name: str) -> MixtureDatabase:
@@ -155,15 +175,15 @@
 
 
 def get_samples_in_mixid(mixdb: MixtureDatabase, mixid: int) -> int:
     return mixdb.mixtures[mixid].samples
 
 
 def get_transform_frames_in_mrecord(mixdb: MixtureDatabase, mrecord: MRecord) -> int:
-    return mrecord.samples // mixdb.frame_size
+    return mrecord.samples // mixdb.ftransform.R
 
 
 def get_feature_frames_in_mrecord(mixdb: MixtureDatabase, mrecord: MRecord) -> int:
     return mrecord.samples // mixdb.feature_step_samples
 
 
 def get_class_weights_threshold(mixdb: Union[MixtureDatabase, Dict]) -> List[float]:
@@ -346,7 +366,24 @@
     metadata += f'random_snr: {mrecord.random_snr}\n'
     metadata += f'samples: {mrecord.samples}\n'
     metadata += f'target_snr_gain: {mrecord.target_snr_gain}\n'
     metadata += f'noise_snr_gain: {mrecord.noise_snr_gain}\n'
     metadata += f'class_count: {mrecord.class_count}\n'
 
     return metadata
+
+
+def add_feature_truth_to_h5(file: h5py.File,
+                            feature: np.ndarray,
+                            truth_f: np.ndarray,
+                            segsnr: np.ndarray,
+                            save_segsnr: bool = False) -> None:
+    datasets = ['feature', 'truth_f', 'segsnr']
+    for dataset in datasets:
+        if dataset in file:
+            del file[dataset]
+    file.create_dataset(name='feature', data=feature, dtype=np.single)
+    file.create_dataset(name='truth_f',
+                        data=truth_f,
+                        dtype=np.csingle if np.iscomplex(truth_f).any() else np.single)
+    if save_segsnr:
+        file.create_dataset(name='segsnr', data=segsnr, dtype=np.single)
```

### Comparing `sonusai-0.8.8/sonusai/mixture/process.py` & `sonusai-0.9.1/sonusai/mixture/process.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/segment.py` & `sonusai-0.9.1/sonusai/mixture/segment.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/target_class_balancing.py` & `sonusai-0.9.1/sonusai/mixture/target_class_balancing.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/targets.py` & `sonusai-0.9.1/sonusai/mixture/targets.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/mixture/truth.py` & `sonusai-0.9.1/sonusai/mixture/truth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 import numpy as np
 
 from sonusai.mixture.mixdb import MRecord
 from sonusai.mixture.mixdb import MixtureDatabase
+from sonusai.mixture.mixdb import TruthFunctionConfig
 
 
 def _strictly_decreasing(list_to_check: list) -> bool:
     return all(x > y for x, y in zip(list_to_check, list_to_check[1:]))
 
 
 def generate_truth(mixdb: MixtureDatabase,
@@ -25,199 +26,231 @@
 
     if not all(len(target_audio) == len(noise_audio) for target_audio in target_audios):
         raise SonusAIError('Lengths of target audio do not match length of noise audio')
 
     truth = np.zeros((mrecord.samples, mixdb.num_classes), dtype=np.csingle)
     for idx in range(len(target_audios)):
         for truth_setting in mixdb.targets[mrecord.target_file_index[idx]].truth_settings:
-            config = {
-                'index':       truth_setting.index,
-                'function':    truth_setting.function,
-                'config':      truth_setting.config,
-                'frame_size':  mixdb.frame_size,
-                'num_classes': mixdb.num_classes,
-                'mutex':       mixdb.truth_mutex,
-                'target_gain': mrecord.target_gain[idx] * mrecord.target_snr_gain
-            }
+            config = TruthFunctionConfig(
+                index=truth_setting.index,
+                function=truth_setting.function,
+                config=truth_setting.config,
+                ftransform=mixdb.ftransform,
+                num_classes=mixdb.num_classes,
+                mutex=mixdb.truth_mutex,
+                target_gain=mrecord.target_gain[idx] * mrecord.target_snr_gain
+            )
             truth += truth_function(target_audio=target_audios[idx], noise_audio=noise_audio, config=config)
 
     if np.isreal(truth).all():
         truth = np.single(np.real(truth))
     return truth
 
 
 def truth_function(target_audio: np.ndarray,
                    noise_audio: np.ndarray,
-                   config: dict) -> np.ndarray:
+                   config: TruthFunctionConfig) -> np.ndarray:
     import h5py
     from pyaaware import ForwardTransform
     from pyaaware import SED
 
     from sonusai import SonusAIError
     from sonusai.mixture.mapped_snr_f import calculate_mapped_snr_f
     from sonusai.utils.numeric_conversion import int16_to_float
 
-    truth = np.zeros((len(target_audio), config['num_classes']), dtype=np.single)
-    offsets = range(0, len(target_audio), config['frame_size'])
-    zero_based_indices = [x - 1 for x in config['index']]
-    target_fft = ForwardTransform(N=config['frame_size'] * 4, R=config['frame_size'])
-    noise_fft = ForwardTransform(N=config['frame_size'] * 4, R=config['frame_size'])
-
-    if config['function'] == 'sed':
-        if len(target_audio) % config['frame_size'] != 0:
-            raise SonusAIError(f'Number of samples in audio is not a multiple of {config["frame_size"]}')
+    ftransform = config.ftransform
+    frame_size = ftransform.R
+    truth = np.zeros((len(target_audio), config.num_classes), dtype=np.single)
+    offsets = range(0, len(target_audio), frame_size)
+    zero_based_indices = [x - 1 for x in config.index]
+    target_fft = ForwardTransform(N=ftransform.N, R=ftransform.R, ttype=ftransform.ttype)
+    noise_fft = ForwardTransform(N=ftransform.N, R=ftransform.R, ttype=ftransform.ttype)
+
+    if config.function == 'sed':
+        if len(target_audio) % frame_size != 0:
+            raise SonusAIError(f'Number of samples in audio is not a multiple of {frame_size}')
 
-        if 'config' not in config:
+        if config.config is None:
             raise SonusAIError('Truth function SED missing config')
 
         parameters = ['thresholds']
         for parameter in parameters:
-            if parameter not in config['config']:
+            if parameter not in config.config:
                 raise SonusAIError(f'Truth function SED config missing required parameter: {parameter}')
 
-        thresholds = config['config']['thresholds']
+        thresholds = config.config['thresholds']
         if not _strictly_decreasing(thresholds):
             raise SonusAIError(f'Truth function SED thresholds are not strictly decreasing: {thresholds}')
 
-        if config['target_gain'] == 0:
+        if config.target_gain == 0:
             return truth
 
         # SED wants 1-based indices
         sed = SED(thresholds=thresholds,
-                  index=config['index'],
-                  frame_size=config['frame_size'],
-                  num_classes=config['num_classes'],
-                  mutex=config['mutex'])
+                  index=config.index,
+                  frame_size=frame_size,
+                  num_classes=config.num_classes,
+                  mutex=config.mutex)
 
-        target_audio = np.int16(np.round(np.single(target_audio) / config['target_gain']))
+        target_audio = np.int16(np.round(np.single(target_audio) / config.target_gain))
         for offset in offsets:
-            indices = slice(offset, offset + config['frame_size'])
+            indices = slice(offset, offset + frame_size)
             new_truth = sed.execute(target_fft.energy_t(int16_to_float(target_audio[indices])))
             truth[indices] = np.reshape(new_truth, (1, len(new_truth)))
 
         return truth
 
-    elif config['function'] == 'file':
-        if 'config' not in config:
+    if config.function == 'file':
+        if config.config is None:
             raise SonusAIError('Truth function file missing config')
 
         parameters = ['file']
         for parameter in parameters:
-            if parameter not in config['config']:
+            if parameter not in config.config:
                 raise SonusAIError(f'Truth function file config missing required parameter: {parameter}')
 
-        with h5py.File(config['config']['file'], 'r') as f:
+        with h5py.File(config.config['file'], 'r') as f:
             truth_in = np.array(f['/truth_t'])
 
         if truth_in.ndim != 2:
             raise SonusAIError('Truth file data is not 2 dimensions')
 
         if truth_in.shape[0] != len(target_audio):
             raise SonusAIError('Truth file does not contain the right amount of samples')
 
-        if config['target_gain'] == 0:
+        if config.target_gain == 0:
             return truth
 
         if len(zero_based_indices) > 1:
             if len(zero_based_indices) != truth_in.shape[1]:
                 raise SonusAIError('Truth file does not contain the right amount of classes')
 
             truth[:, zero_based_indices] = truth_in
         else:
             index = zero_based_indices[0]
-            if index + truth_in.shape[1] > config['num_classes']:
+            if index + truth_in.shape[1] > config.num_classes:
                 raise SonusAIError('Truth file contains too many classes')
 
             truth[:, index:index + truth_in.shape[1]] = truth_in
 
         return truth
 
-    elif config['function'] == 'energy_t':
-        if config['target_gain'] == 0:
+    if config.function == 'energy_t':
+        if config.target_gain == 0:
             return truth
 
         for offset in offsets:
-            target_energy = target_fft.energy_t(int16_to_float(target_audio[offset:offset + config['frame_size']]))
-            truth[offset:offset + config['frame_size'], zero_based_indices] = np.single(target_energy)
+            target_energy = target_fft.energy_t(int16_to_float(target_audio[offset:offset + frame_size]))
+            truth[offset:offset + frame_size, zero_based_indices] = np.single(target_energy)
 
         return truth
 
-    elif config['function'] == 'target_f':
-        truth = np.zeros((len(target_audio), config['num_classes']), dtype=np.csingle)
-        if config['target_gain'] == 0:
+    if config.function == 'target_f':
+        truth = np.zeros((len(target_audio), config.num_classes), dtype=np.csingle)
+        if config.target_gain == 0:
             return truth
 
         for offset in offsets:
             target_f = np.csingle(
-                target_fft.execute(int16_to_float(target_audio[offset:offset + config['frame_size']])))
+                target_fft.execute(int16_to_float(target_audio[offset:offset + frame_size])))
 
-            indices = slice(offset, offset + config['frame_size'])
+            indices = slice(offset, offset + frame_size)
             for index in zero_based_indices:
                 truth[indices, index:index + target_fft.bins] = target_f
 
         return truth
 
-    elif config['function'] in ['energy_f', 'snr_f', 'mapped_snr_f']:
-        if config['target_gain'] == 0:
+    if config.function == 'crm':
+        truth = np.zeros((len(target_audio), config.num_classes), dtype=np.csingle)
+
+        if config.target_gain == 0:
+            return truth
+
+        for offset in offsets:
+            target_f = np.csingle(
+                target_fft.execute(int16_to_float(target_audio[offset:offset + frame_size])))
+            mixture_f = np.csingle(
+                noise_fft.execute(int16_to_float(noise_audio[offset:offset + frame_size]))) + target_f
+
+            crm = np.empty(target_f.shape, dtype=np.csingle)
+            with np.nditer(target_f, flags=['multi_index'], op_flags=['readwrite']) as it:
+                for _ in it:
+                    num = target_f[it.multi_index]
+                    den = mixture_f[it.multi_index]
+                    if num == 0:
+                        crm[it.multi_index] = 0
+                    elif den == 0:
+                        crm[it.multi_index] = complex(np.inf, np.inf)
+                    else:
+                        crm[it.multi_index] = num / den
+
+            indices = slice(offset, offset + frame_size)
+            for index in zero_based_indices:
+                truth[indices, index:index + target_fft.bins] = crm
+
+        return truth
+
+    if config.function in ['energy_f', 'snr_f', 'mapped_snr_f']:
+        if config.target_gain == 0:
             return truth
 
         snr_db_mean = None
         snr_db_std = None
-        if config['function'] == 'mapped_snr_f':
-            if 'config' not in config:
+        if config.function == 'mapped_snr_f':
+            if config.config is None:
                 raise SonusAIError('Truth function mapped SNR missing config')
 
             parameters = ['snr_db_mean', 'snr_db_std']
             for parameter in parameters:
-                if parameter not in config['config']:
+                if parameter not in config.config:
                     raise SonusAIError(f'Truth function mapped SNR config missing required parameter: {parameter}')
 
-            snr_db_mean = config['config']['snr_db_mean']
+            snr_db_mean = config.config['snr_db_mean']
             if len(snr_db_mean) != target_fft.bins:
                 raise SonusAIError(f'Truth function mapped SNR snr_db_mean does not have {target_fft.bins} elements')
 
-            snr_db_std = config['config']['snr_db_std']
+            snr_db_std = config.config['snr_db_std']
             if len(snr_db_std) != target_fft.bins:
                 raise SonusAIError(f'Truth function mapped SNR snr_db_std does not have {target_fft.bins} elements')
 
         for index in zero_based_indices:
-            if index + target_fft.bins > config['num_classes']:
+            if index + target_fft.bins > config.num_classes:
                 raise SonusAIError('Truth index exceeds the number of classes')
 
         for offset in offsets:
             target_energy = np.single(
-                target_fft.energy_f(int16_to_float(target_audio[offset:offset + config['frame_size']])))
-            if config['function'] in ['snr_f', 'mapped_snr_f']:
+                target_fft.energy_f(int16_to_float(target_audio[offset:offset + frame_size])))
+            if config.function in ['snr_f', 'mapped_snr_f']:
                 noise_energy = np.single(
-                    noise_fft.energy_f(int16_to_float(noise_audio[offset:offset + config['frame_size']])))
+                    noise_fft.energy_f(int16_to_float(noise_audio[offset:offset + frame_size])))
             else:
                 noise_energy = np.single(1)
 
-            indices = slice(offset, offset + config['frame_size'])
+            indices = slice(offset, offset + frame_size)
             for index in zero_based_indices:
                 old_err = np.seterr(divide='ignore', invalid='ignore')
                 tmp = target_energy / noise_energy
                 np.seterr(**old_err)
 
                 tmp = np.nan_to_num(tmp, nan=-np.inf, posinf=np.inf, neginf=-np.inf)
 
-                if config['function'] == 'mapped_snr_f':
+                if config.function == 'mapped_snr_f':
                     tmp = calculate_mapped_snr_f(tmp, snr_db_mean, snr_db_std)
 
                 truth[indices, index:index + target_fft.bins] = tmp
 
         return truth
 
-    elif config['function'] == 'phoneme':
+    if config.function == 'phoneme':
         # Read in .txt transcript and run a Python function to generate text grid data
         # (indicating which phonemes are active)
-        # Then generate truth based on this data and put in the correct classes based on config['index']
+        # Then generate truth based on this data and put in the correct classes based on config.index
         raise SonusAIError('Truth function phoneme is not supported yet')
 
-    raise SonusAIError(f'Unsupported truth function: {config["function"]}')
+    raise SonusAIError(f'Unsupported truth function: {config.function}')
 
 
 def get_truth_indices_for_mixid(mixdb: MixtureDatabase, mixid: int) -> List[int]:
     """Get a list of truth indices for a given mixid."""
 
     from sonusai.mixture.targets import get_truth_indices_for_target
```

### Comparing `sonusai-0.8.8/sonusai/mkwav.py` & `sonusai-0.9.1/sonusai/mkwav.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/onnx_predict.py` & `sonusai-0.9.1/sonusai/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/plot.py` & `sonusai-0.9.1/sonusai/plot.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/queries/queries.py` & `sonusai-0.9.1/sonusai/queries/queries.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/speech_enh.py` & `sonusai-0.9.1/sonusai/speech_enh.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,18 +583,17 @@
     import numpy as np
     from pyaaware import ForwardTransform
 
     from sonusai.mixture import get_feature_stats
     from sonusai.mixture import get_pad_length
     from sonusai.utils import int16_to_float
 
-    fs = get_feature_stats(feature_mode=feature_gen.feature_mode,
-                           frame_size=feature_gen.frame_size,
+    fs = get_feature_stats(feature=feature_gen.feature_mode,
                            num_classes=feature_gen.num_classes,
-                           truth_mutex=feature_gen.truth_mutex)
+                           frame_size=feature_gen.frame_size)
 
     audio = np.pad(array=audio,
                    pad_width=(0, get_pad_length(len(audio), fs.feature_step_samples)),
                    mode='constant',
                    constant_values=0)
 
     target_fft = ForwardTransform(N=feature_gen.frame_size * 4, R=feature_gen.frame_size)
```

### Comparing `sonusai-0.8.8/sonusai/tplot.py` & `sonusai-0.9.1/sonusai/tplot.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/__init__.py` & `sonusai-0.9.1/sonusai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/braced_glob.py` & `sonusai-0.9.1/sonusai/utils/braced_glob.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/calculate_input_shape.py` & `sonusai-0.9.1/sonusai/utils/calculate_input_shape.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import List
 
-from sonusai.mixture.constants import DEFAULT_FRAME_SIZE
-
 
 def calculate_input_shape(feature: str,
                           flatten: bool = False,
                           timesteps: int = 0,
                           add1ch: bool = False,
-                          frame_size=DEFAULT_FRAME_SIZE) -> List[int]:
+                          frame_size: int = None) -> List[int]:
     """
     Calculate input shape given feature and user-specified reshape parameters.
 
     Inputs:
         feature:     String defining the Aaware feature used in SonusAI, typically  mixdb.feature.
         flatten:     If true, flatten the 2D spectrogram from SxB to S*B.
         timesteps:   Pre-pend timesteps dimension if non-zero, size = timesteps.
         add1ch:      Append channel dimension of size 1, (channel last).
         frame_size:  The default SonusAI frame size should always be used for now.
     """
     from pyaaware import FeatureGenerator
 
+    if frame_size is None:
+        from sonusai.mixture import get_default_config
+
+        config = get_default_config()
+        frame_size = config['ftransform'].R
+
     # num_classes is irrelevant, set to 2
     fg = FeatureGenerator(frame_size=frame_size,
                           feature_mode=feature,
                           num_classes=2)
 
     if flatten:
         in_shape = [fg.stride * fg.num_bands]
```

### Comparing `sonusai-0.8.8/sonusai/utils/engineering_number.py` & `sonusai-0.9.1/sonusai/utils/engineering_number.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/get_label_names.py` & `sonusai-0.9.1/sonusai/utils/get_label_names.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/keras_utils.py` & `sonusai-0.9.1/sonusai/utils/keras_utils.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/onnx_utils.py` & `sonusai-0.9.1/sonusai/utils/onnx_utils.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/parallel.py` & `sonusai-0.9.1/sonusai/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/parallel_tqdm.py` & `sonusai-0.9.1/sonusai/utils/parallel_tqdm.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/print_mixture_details.py` & `sonusai-0.9.1/sonusai/utils/print_mixture_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             print_fn(f'  Truth settings:')
             for truth_setting in target.truth_settings:
                 print_fn(f'{"    Index":{desc_len}} {truth_setting.index}')
                 print_fn(f'{"    Function":{desc_len}} {truth_setting.function}')
                 print_fn(f'{"    Config":{desc_len}} {truth_setting.config}')
             print_fn(f'{"  Augmentation":{desc_len}} {target_augmentations[idx]}')
         print_fn(f'{"Samples":{desc_len}} {mixture.samples}')
-        print_fn(f'{"Features":{desc_len}} {get_feature_frames_in_mrecord(mixdb, mixid)}')
+        print_fn(f'{"Features":{desc_len}} {get_feature_frames_in_mrecord(mixdb, mixdb.mixtures[mixid])}')
         print_fn(f'{"Noise":{desc_len}} {noise.name}')
         noise_offset_percent = int(np.round(100 * mixture.noise_offset / float(noise.duration * SAMPLE_RATE)))
         print_fn(f'{"Noise offset":{desc_len}} {mixture.noise_offset} samples ({noise_offset_percent}%)')
         print_fn(f'{"SNR":{desc_len}} {mixture.snr} dB')
         print_fn(f'{"Target gain":{desc_len}} {mixture.target_gain}')
         print_fn(f'{"Target SNR gain":{desc_len}} {mixture.target_snr_gain}')
         print_fn(f'{"Noise SNR gain":{desc_len}} {mixture.noise_snr_gain}')
```

### Comparing `sonusai-0.8.8/sonusai/utils/ranges.py` & `sonusai-0.9.1/sonusai/utils/ranges.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/read_predict_data.py` & `sonusai-0.9.1/sonusai/utils/read_predict_data.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/reshape.py` & `sonusai-0.9.1/sonusai/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/stratified_shuffle_split.py` & `sonusai-0.9.1/sonusai/utils/stratified_shuffle_split.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/utils/trim_docstring.py` & `sonusai-0.9.1/sonusai/utils/trim_docstring.py`

 * *Files identical despite different names*

### Comparing `sonusai-0.8.8/sonusai/vars.py` & `sonusai-0.9.1/sonusai/vars.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 """
 
 
 def main():
     from docopt import docopt
 
     import sonusai
-    from sonusai.mixture import DEFAULT_FRAME_SIZE
     from sonusai.mixture import DEFAULT_NOISE
     from sonusai.utils import trim_docstring
 
     docopt(trim_docstring(__doc__), version=sonusai.__version__, options_first=True)
 
     print('Custom SonusAI variables:')
     print('')
     print(f'  ${{default_noise}}: {DEFAULT_NOISE}')
-    print(f'  ${{frame_size}}:    {DEFAULT_FRAME_SIZE}')
     print('')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `sonusai-0.8.8/setup.py` & `sonusai-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 entry_points = \
 {'console_scripts': ['aawscd_probwrite = sonusai.aawscd_probwrite:main',
                      'sonusai = sonusai.main:main']}
 
 setup_kwargs = {
     'name': 'sonusai',
-    'version': '0.8.8',
+    'version': '0.9.1',
     'description': 'Framework for building deep neural network models for sound, speech, and voice AI',
     'long_description': "Sonus AI: Framework for simplified creation of deep NN models for sound, speech, and voice AI\n\nSonus AI includes functions for pre-processing training and validation data and\ncreating performance metrics reports for key types of Keras models:\n- recurrent, convolutional, or a combination (i.e. RCNNs)\n- binary, multiclass single-label, multiclass multi-label, and regresssion\n- training with data augmentations:  noise mixing, pitch and time stretch, etc.\n\nSonus AI python functions are used by:\n - Aaware Inc. sonusai executable:  Easily create train/validation data, run prediction, evaluate model performance\n - Keras model scripts:             User python scripts for keras model creation, training, and prediction. These can use sonusai-specific data but also some general useful utilities for trainining rnn-based models like CRNN's, DSCRNN's, etc. in Keras\n",
     'author': 'Chris Eddington',
     'author_email': 'chris@aaware.com',
     'maintainer': 'Chris Eddington',
     'maintainer_email': 'chris@aaware.com',
     'url': 'https://aaware.com',
```

### Comparing `sonusai-0.8.8/PKG-INFO` & `sonusai-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonusai
-Version: 0.8.8
+Version: 0.9.1
 Summary: Framework for building deep neural network models for sound, speech, and voice AI
 Home-page: https://aaware.com
 License: GPL-3.0-only
 Author: Chris Eddington
 Author-email: chris@aaware.com
 Maintainer: Chris Eddington
 Maintainer-email: chris@aaware.com
```

