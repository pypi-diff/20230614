# Comparing `tmp/coretex-1.0.4.tar.gz` & `tmp/coretex-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.4.tar", last modified: Tue Jun  6 12:02:51 2023, max compression
+gzip compressed data, was "coretex-1.0.5.tar", last modified: Tue Jun  6 20:30:46 2023, max compression
```

## Comparing `coretex-1.0.4.tar` & `coretex-1.0.5.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.483449 coretex-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-06 12:02:39.000000 coretex-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-06 12:02:51.483449 coretex-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-06 12:02:39.000000 coretex-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-06 12:02:39.000000 coretex-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:02:51.483449 coretex-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.459448 coretex-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.463448 coretex-1.0.4/src/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/cache/cache_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/codable/descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/coretex/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/coretex/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/coretex/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/coretex/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.471448 coretex-1.0.4/src/coretex/coretex/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.471448 coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.471448 coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.471448 coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.471448 coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/network_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.471448 coretex-1.0.4/src/coretex/coretex/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/executing_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/experiment/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/experiment/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/model/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.475448 coretex-1.0.4/src/coretex/coretex/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.479448 coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.479448 coretex-1.0.4/src/coretex/coretex/space/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/space/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/space/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/coretex/space/space_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.479448 coretex-1.0.4/src/coretex/folder_management/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/folder_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.479448 coretex-1.0.4/src/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/logging/log_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.479448 coretex-1.0.4/src/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/requests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/networking/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.483449 coretex-1.0.4/src/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.483449 coretex-1.0.4/src/coretex/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/project/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/project/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/project/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/project/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.483449 coretex-1.0.4/src/coretex/qiime2/
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.483449 coretex-1.0.4/src/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.483449 coretex-1.0.4/src/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/utils/console_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 12:02:39.000000 coretex-1.0.4/src/coretex/utils/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:51.467448 coretex-1.0.4/src/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-06 12:02:51.000000 coretex-1.0.4/src/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-06 12:02:51.000000 coretex-1.0.4/src/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:02:51.000000 coretex-1.0.4/src/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 12:02:51.000000 coretex-1.0.4/src/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 12:02:51.000000 coretex-1.0.4/src/coretex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.633864 coretex-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-06-06 20:30:35.000000 coretex-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-06 20:30:46.633864 coretex-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-06-06 20:30:35.000000 coretex-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-06 20:30:35.000000 coretex-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:30:46.633864 coretex-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.609864 coretex-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.613864 coretex-1.0.5/src/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.613864 coretex-1.0.5/src/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.613864 coretex-1.0.5/src/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.613864 coretex-1.0.5/src/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.613864 coretex-1.0.5/src/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.617864 coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.621864 coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.621864 coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/network_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.621864 coretex-1.0.5/src/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/executing_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.621864 coretex-1.0.5/src/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.621864 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/experiment/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.625864 coretex-1.0.5/src/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/project/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/project/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.629864 coretex-1.0.5/src/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.633864 coretex-1.0.5/src/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-06 20:30:35.000000 coretex-1.0.5/src/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:30:46.613864 coretex-1.0.5/src/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-06 20:30:46.000000 coretex-1.0.5/src/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-06-06 20:30:46.000000 coretex-1.0.5/src/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:30:46.000000 coretex-1.0.5/src/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 20:30:46.000000 coretex-1.0.5/src/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:30:46.000000 coretex-1.0.5/src/coretex.egg-info/top_level.txt
```

### Comparing `coretex-1.0.4/LICENSE` & `coretex-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/PKG-INFO` & `coretex-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
-Author-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
+Author-email: Duško Mirković <dmirkovic@coretex.ai>
+Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `coretex-1.0.4/README.md` & `coretex-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/pyproject.toml` & `coretex-1.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [project]
 name = "coretex"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
+  { name="Duško Mirković", email="dmirkovic@coretex.ai" }
+]
+maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Igor Perić", email="igor@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
   { name="Darko Zarić", email="dzaric@coretex.ai" },
   { name="Bogdan Tintor", email="btintor@coretex.ai" },
   { name="Alex Maslennikov", email="alex@coretex.ai" },
 ]
```

### Comparing `coretex-1.0.4/src/coretex/__init__.py` & `coretex-1.0.5/src/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/_configuration.py` & `coretex-1.0.5/src/coretex/_configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/_logger.py` & `coretex-1.0.5/src/coretex/_logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/cache/__init__.py` & `coretex-1.0.5/src/coretex/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/cache/cache_module.py` & `coretex-1.0.5/src/coretex/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/codable/__init__.py` & `coretex-1.0.5/src/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/codable/codable.py` & `coretex-1.0.5/src/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/codable/descriptor.py` & `coretex-1.0.5/src/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/__init__.py` & `coretex-1.0.5/src/coretex/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/annotation/__init__.py` & `coretex-1.0.5/src/coretex/coretex/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/annotation/image/__init__.py` & `coretex-1.0.5/src/coretex/coretex/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/annotation/image/bbox.py` & `coretex-1.0.5/src/coretex/coretex/annotation/image/bbox.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/annotation/image/classes_format.py` & `coretex-1.0.5/src/coretex/coretex/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/annotation/image/coretex_format.py` & `coretex-1.0.5/src/coretex/coretex/annotation/image/coretex_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/__init__.py` & `coretex-1.0.5/src/coretex/coretex/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/base_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converter_processor_factory.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/__init__.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/create_ml_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/label_me_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/__init__.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/instance_extractor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/pascal/shared.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/pascal/shared.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/conversion/converters/yolo_converter.py` & `coretex-1.0.5/src/coretex/coretex/conversion/converters/yolo_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/__init__.py` & `coretex-1.0.5/src/coretex/coretex/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/__init__.py` & `coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/base.py` & `coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/__init__.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/base.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/local_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/network_dataset.py` & `coretex-1.0.5/src/coretex/coretex/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/dataset/utils.py` & `coretex-1.0.5/src/coretex/coretex/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/__init__.py` & `coretex-1.0.5/src/coretex/coretex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/artifact.py` & `coretex-1.0.5/src/coretex/coretex/experiment/artifact.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/executing_experiment.py` & `coretex-1.0.5/src/coretex/coretex/experiment/executing_experiment.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/experiment.py` & `coretex-1.0.5/src/coretex/coretex/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/__init__.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/metric.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/metric_factory.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/metric_type.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/metrics/utils.py` & `coretex-1.0.5/src/coretex/coretex/experiment/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/parameters.py` & `coretex-1.0.5/src/coretex/coretex/experiment/parameters.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/experiment/status.py` & `coretex-1.0.5/src/coretex/coretex/experiment/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/model/__init__.py` & `coretex-1.0.5/src/coretex/coretex/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/model/model.py` & `coretex-1.0.5/src/coretex/coretex/model/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/__init__.py` & `coretex-1.0.5/src/coretex/coretex/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/any_local_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/__init__.py` & `coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/custom_sample/__init__.py` & `coretex-1.0.5/src/coretex/coretex/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/custom_sample/custom_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/custom_sample/custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.5/src/coretex/coretex/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_sample/__init__.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_sample/image_format.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_sample/image_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_sample/image_sample_data.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_sample/local_image_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/local_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/network_sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/network_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/sample/sample.py` & `coretex-1.0.5/src/coretex/coretex/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/space/__init__.py` & `coretex-1.0.5/src/coretex/coretex/space/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/space/base.py` & `coretex-1.0.5/src/coretex/coretex/space/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/space/project.py` & `coretex-1.0.5/src/coretex/coretex/space/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/space/space.py` & `coretex-1.0.5/src/coretex/coretex/space/space.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/coretex/space/space_task.py` & `coretex-1.0.5/src/coretex/coretex/space/space_task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/folder_management/__init__.py` & `coretex-1.0.5/src/coretex/folder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/folder_management/folder_manager.py` & `coretex-1.0.5/src/coretex/folder_management/folder_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/logging/__init__.py` & `coretex-1.0.5/src/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/logging/log.py` & `coretex-1.0.5/src/coretex/logging/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/logging/log_severity.py` & `coretex-1.0.5/src/coretex/logging/log_severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/logging/logger.py` & `coretex-1.0.5/src/coretex/logging/logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/__init__.py` & `coretex-1.0.5/src/coretex/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/chunk_upload_session.py` & `coretex-1.0.5/src/coretex/networking/chunk_upload_session.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/file_data.py` & `coretex-1.0.5/src/coretex/networking/file_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/network_manager.py` & `coretex-1.0.5/src/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/network_manager_base.py` & `coretex-1.0.5/src/coretex/networking/network_manager_base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/network_object.py` & `coretex-1.0.5/src/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/network_response.py` & `coretex-1.0.5/src/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/request_type.py` & `coretex-1.0.5/src/coretex/networking/request_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/requests_manager.py` & `coretex-1.0.5/src/coretex/networking/requests_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/networking/user_data.py` & `coretex-1.0.5/src/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/nlp/__init__.py` & `coretex-1.0.5/src/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/nlp/text.py` & `coretex-1.0.5/src/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/nlp/token.py` & `coretex-1.0.5/src/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/nlp/transcriber.py` & `coretex-1.0.5/src/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/nlp/transcription.py` & `coretex-1.0.5/src/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/nlp/utils.py` & `coretex-1.0.5/src/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/project/__init__.py` & `coretex-1.0.5/src/coretex/project/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/project/base.py` & `coretex-1.0.5/src/coretex/project/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/project/calculate_metrics.py` & `coretex-1.0.5/src/coretex/project/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/project/heartbeat.py` & `coretex-1.0.5/src/coretex/project/heartbeat.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/project/local.py` & `coretex-1.0.5/src/coretex/project/local.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/project/remote.py` & `coretex-1.0.5/src/coretex/project/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/qiime2/__init__.py` & `coretex-1.0.5/src/coretex/qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/qiime2/utils.py` & `coretex-1.0.5/src/coretex/qiime2/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/threading/__init__.py` & `coretex-1.0.5/src/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/threading/threaded_data_processor.py` & `coretex-1.0.5/src/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/utils/__init__.py` & `coretex-1.0.5/src/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/utils/console_progress_bar.py` & `coretex-1.0.5/src/coretex/utils/console_progress_bar.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/utils/date.py` & `coretex-1.0.5/src/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/utils/file.py` & `coretex-1.0.5/src/coretex/utils/file.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex/utils/number.py` & `coretex-1.0.5/src/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.4/src/coretex.egg-info/PKG-INFO` & `coretex-1.0.5/src/coretex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
-Author-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
+Author-email: Duško Mirković <dmirkovic@coretex.ai>
+Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `coretex-1.0.4/src/coretex.egg-info/SOURCES.txt` & `coretex-1.0.5/src/coretex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

