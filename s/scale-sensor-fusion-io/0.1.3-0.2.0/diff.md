# Comparing `tmp/scale_sensor_fusion_io-0.1.3.tar.gz` & `tmp/scale_sensor_fusion_io-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_sensor_fusion_io-0.1.3.tar", max compression
+gzip compressed data, was "scale_sensor_fusion_io-0.2.0.tar", max compression
```

## Comparing `scale_sensor_fusion_io-0.1.3.tar` & `scale_sensor_fusion_io-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     2945 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.3/docs/README.md
--rw-r--r--   0        0        0      883 2023-06-02 23:19:18.152535 scale_sensor_fusion_io-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       98 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/__init__.py
--rw-r--r--   0        0        0       52 2023-05-25 07:12:37.457890 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/loaders/__init__.py
--rw-r--r--   0        0        0     2716 2023-05-22 20:30:40.190095 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/loaders/bs5_loader.py
--rw-r--r--   0        0        0     3088 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/loaders/sfs_loader.py
--rw-r--r--   0        0        0       19 2023-06-02 02:48:06.569388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/model_converters/__init__.py
--rw-r--r--   0        0        0     8163 2023-06-02 16:33:35.150043 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/model_converters/sfs.py
--rw-r--r--   0        0        0       96 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/__init__.py
--rw-r--r--   0        0        0      456 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/__init__.py
--rw-r--r--   0        0        0      512 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/attributes.py
--rw-r--r--   0        0        0      626 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/box_2d.py
--rw-r--r--   0        0        0     1129 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/cuboid.py
--rw-r--r--   0        0        0      520 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/event.py
--rw-r--r--   0        0        0      690 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/labeled_points.py
--rw-r--r--   0        0        0      924 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
--rw-r--r--   0        0        0      425 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/object.py
--rw-r--r--   0        0        0      638 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/polygon.py
--rw-r--r--   0        0        0      509 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/common.py
--rw-r--r--   0        0        0      109 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/paths/__init__.py
--rw-r--r--   0        0        0      291 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/paths/attribute_path.py
--rw-r--r--   0        0        0     5350 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/paths/cuboid_path.py
--rw-r--r--   0        0        0    16186 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/paths/pose_path.py
--rw-r--r--   0        0        0      577 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/scene.py
--rw-r--r--   0        0        0      253 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/__init__.py
--rw-r--r--   0        0        0       94 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/camera/__init__.py
--rw-r--r--   0        0        0     6340 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
--rw-r--r--   0        0        0      310 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
--rw-r--r--   0        0        0      896 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
--rw-r--r--   0        0        0       27 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
--rw-r--r--   0        0        0      931 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
--rw-r--r--   0        0        0       28 2023-05-22 20:07:37.040396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/radar/__init__.py
--rw-r--r--   0        0        0      825 2023-05-22 20:08:31.168592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
--rw-r--r--   0        0        0        0 2023-03-29 20:56:32.935581 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/py.typed
--rw-r--r--   0        0        0       91 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/spec/__init__.py
--rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/spec/sfs/__init__.py
--rw-r--r--   0        0        0     7837 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/spec/sfs/types.py
--rw-r--r--   0        0        0       21 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/spec/v5/__init__.py
--rw-r--r--   0        0        0     3001 2023-05-22 20:08:31.172592 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/spec/v5/types.py
--rw-r--r--   0        0        0        0 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/utils/__init__.py
--rw-r--r--   0        0        0     2005 2023-05-22 20:07:37.044396 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/utils/downsample.py
--rw-r--r--   0        0        0     2730 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/utils/generate_video.py
--rw-r--r--   0        0        0      899 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/__init__.py
--rw-r--r--   0        0        0     1069 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
--rw-r--r--   0        0        0      297 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/README.md
--rw-r--r--   0        0        0      135 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
--rw-r--r--   0        0        0      502 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/config.py
--rw-r--r--   0        0        0     7388 2023-06-02 02:48:06.841389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/core.py
--rw-r--r--   0        0        0       90 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/data.py
--rw-r--r--   0        0        0     1121 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
--rw-r--r--   0        0        0     2949 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
--rw-r--r--   0        0        0     8189 2023-06-02 02:48:06.837389 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/types.py
--rw-r--r--   0        0        0     2802 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/error.py
--rw-r--r--   0        0        0      965 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/helpers.py
--rw-r--r--   0        0        0       19 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/parser/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-02 02:48:06.573388 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/parser/sfs.py
--rw-r--r--   0        0        0     9039 2023-06-02 23:22:54.941509 scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/validate.py
--rw-r--r--   0        0        0     3756 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2945 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/docs/README.md
+-rw-r--r--   0        0        0      938 2023-06-13 19:55:58.611076 scale_sensor_fusion_io-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-21 17:25:32.493004 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/loaders/__init__.py
+-rw-r--r--   0        0        0     2716 2023-05-04 20:10:30.275131 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/loaders/bs5_loader.py
+-rw-r--r--   0        0        0     3088 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/loaders/sfs_loader.py
+-rw-r--r--   0        0        0       19 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/model_converters/__init__.py
+-rw-r--r--   0        0        0     8163 2023-06-02 18:09:01.052673 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/model_converters/sfs.py
+-rw-r--r--   0        0        0     3349 2023-06-13 19:55:58.611076 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/Pose.py
+-rw-r--r--   0        0        0       96 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/__init__.py
+-rw-r--r--   0        0        0      456 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/attributes.py
+-rw-r--r--   0        0        0      626 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/box_2d.py
+-rw-r--r--   0        0        0     1129 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/cuboid.py
+-rw-r--r--   0        0        0      520 2023-05-05 15:35:42.316417 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/event.py
+-rw-r--r--   0        0        0      690 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/labeled_points.py
+-rw-r--r--   0        0        0      924 2023-05-09 02:31:38.889679 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/localization_adjustment.py
+-rw-r--r--   0        0        0      425 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/object.py
+-rw-r--r--   0        0        0      638 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/polygon.py
+-rw-r--r--   0        0        0      509 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/common.py
+-rw-r--r--   0        0        0      109 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/paths/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/paths/attribute_path.py
+-rw-r--r--   0        0        0     5350 2023-05-01 16:05:39.349378 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/paths/cuboid_path.py
+-rw-r--r--   0        0        0    16186 2023-06-14 08:40:18.734552 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/paths/pose_path.py
+-rw-r--r--   0        0        0      577 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/scene.py
+-rw-r--r--   0        0        0      253 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/__init__.py
+-rw-r--r--   0        0        0       94 2023-04-19 22:28:02.352690 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/camera/__init__.py
+-rw-r--r--   0        0        0     6340 2023-05-24 16:46:54.391775 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py
+-rw-r--r--   0        0        0      310 2023-05-09 20:54:40.857630 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/camera/camera_intrinsics.py
+-rw-r--r--   0        0        0      896 2023-05-09 20:55:12.405738 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py
+-rw-r--r--   0        0        0       27 2023-04-19 22:28:02.352690 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/lidar/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-05 15:35:42.316417 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py
+-rw-r--r--   0        0        0       28 2023-04-19 22:28:02.352690 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/radar/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-09 21:28:41.008175 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py
+-rw-r--r--   0        0        0        0 2023-03-31 01:21:32.524089 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/py.typed
+-rw-r--r--   0        0        0       91 2023-05-04 20:10:30.275131 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/spec/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-21 17:25:32.513004 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/spec/sfs/__init__.py
+-rw-r--r--   0        0        0     9659 2023-06-12 23:16:43.148200 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/spec/sfs/types.py
+-rw-r--r--   0        0        0       21 2023-04-21 17:25:32.513004 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/spec/v5/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-14 08:41:24.950160 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/spec/v5/types.py
+-rw-r--r--   0        0        0        0 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/utils/__init__.py
+-rw-r--r--   0        0        0     2005 2023-05-01 16:02:07.346861 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/utils/downsample.py
+-rw-r--r--   0        0        0     2730 2023-06-09 22:05:31.823018 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/utils/generate_video.py
+-rw-r--r--   0        0        0      899 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-25 18:02:56.996415 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/LICENSE
+-rw-r--r--   0        0        0      297 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/README.md
+-rw-r--r--   0        0        0      135 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/config.py
+-rw-r--r--   0        0        0     7388 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/core.py
+-rw-r--r--   0        0        0       90 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/data.py
+-rw-r--r--   0        0        0     1121 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py
+-rw-r--r--   0        0        0     2949 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py
+-rw-r--r--   0        0        0     8189 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/types.py
+-rw-r--r--   0        0        0     2802 2023-06-01 00:34:19.596311 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/error.py
+-rw-r--r--   0        0        0      965 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/helpers.py
+-rw-r--r--   0        0        0       19 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/parser/__init__.py
+-rw-r--r--   0        0        0     7530 2023-05-25 18:02:57.000414 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/parser/sfs.py
+-rw-r--r--   0        0        0     9584 2023-06-05 17:16:28.436716 scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/validate.py
+-rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 scale_sensor_fusion_io-0.2.0/PKG-INFO
```

### Comparing `scale_sensor_fusion_io-0.1.3/docs/README.md` & `scale_sensor_fusion_io-0.2.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/pyproject.toml` & `scale_sensor_fusion_io-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale_sensor_fusion_io"
-version = "0.1.3"
+version = "0.2.0"
 description = "Library for working with timestamp-based sensor fusion scenes"
 authors = [
     "Michael Choi <michael.choi@scale.com>", 
     "Rodrigo Belfiore <rodrigo.belfiore@scale.com>"
 ]
 readme = ["docs/README.md"]
 
@@ -13,14 +13,16 @@
 numpy = "^1.22.4"
 ujson = "^5.7.0"
 pandas = "^2.0.0"
 scipy = "^1.10.1"
 dacite2 = "^2.0.0"
 scale-json-binary = "^0.0.7"
 typing-extensions = "^4.5.0"
+pyquaternion = "^0.9.9"
+pandas-stubs = "^2.0.2.230605"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.991"
 types-ujson = "^5.7.0"
 pytest = "^7.2.2"
 
 [[tool.poetry.source]]
```

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/loaders/bs5_loader.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/loaders/bs5_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/loaders/sfs_loader.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/loaders/sfs_loader.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/model_converters/sfs.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/model_converters/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/attributes.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/attributes.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/box_2d.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/box_2d.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/cuboid.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/cuboid.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/event.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/event.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/labeled_points.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/labeled_points.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/localization_adjustment.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/localization_adjustment.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/annotations/polygon.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/annotations/polygon.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/paths/cuboid_path.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/paths/cuboid_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/paths/pose_path.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/paths/pose_path.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/scene.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/scene.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/camera/camera_distortion.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/camera/camera_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/lidar/lidar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/models/sensors/radar/radar_sensor.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/spec/sfs/types.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/spec/sfs/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -209,43 +209,85 @@
     type: Literal["attributes"] = "attributes"
     parent_id: Optional[AnnotationID] = None
     attributes: Optional[List[AttributePath]] = None
     sensor_attributes: Optional[List[AttributePath]] = None
 
 
 @dataclass
-class Box2DPath:
+class AnnotationPath:
     timestamps: List[int]
-    values: List[List[float]]  # left, top, width, height
+    values: List[List[float]]
+
+
+@dataclass
+class Point2DAnnotation:
+    id: AnnotationID
+    sensor_id: SensorID
+    path: AnnotationPath  # values: [x, y]
+    type: Literal["point_2d"] = "point_2d"
+    parent_id: Optional[AnnotationID] = None
+    stationary: Optional[bool] = False
+    label: Optional[str] = None
+    attributes: Optional[List[AttributePath]] = None
 
 
 @dataclass
 class Box2DAnnotation:
     id: AnnotationID
     sensor_id: SensorID
-    path: Box2DPath
-    type: Literal["box"] = "box"
+    path: AnnotationPath  # values: [left, top, width, height]
+    type: Literal["box_2d"] = "box_2d"
+    parent_id: Optional[AnnotationID] = None
+    stationary: Optional[bool] = False
+    label: Optional[str] = None
+    attributes: Optional[List[AttributePath]] = None
+
+
+class Polyline2DAnnotation:
+    id: AnnotationID
+    sensor_id: SensorID
+    path: AnnotationPath  # x_0, y_0, x_1, y_1, ..., x_n, y_n
+    type: Literal["polyline_2d"] = "polyline_2d"
     parent_id: Optional[AnnotationID] = None
     stationary: Optional[bool] = False
     label: Optional[str] = None
     attributes: Optional[List[AttributePath]] = None
 
 
 @dataclass
-class PolygonPath:
-    timestamps: List[int]
-    values: List[List[float]]  # x_0, y_0, x_1, y_1, ..., x_n, y_n
+class Polygon2DAnnotation:
+    id: AnnotationID
+    sensor_id: SensorID
+    path: AnnotationPath  # x_0, y_0, x_1, y_1, ..., x_n, y_n
+    type: Literal["polygon_2d"] = "polygon_2d"
+    parent_id: Optional[AnnotationID] = None
+    stationary: Optional[bool] = False
+    label: Optional[str] = None
+    attributes: Optional[List[AttributePath]] = None
+
+
+@dataclass
+class PolylineAnnotation:
+    id: AnnotationID
+    sensor_id: SensorID
+    path: AnnotationPath  # x_0, y_0, z_0, x_1, y_1, z_1, ..., x_n, y_n, z_n
+    type: Literal["polyline"] = "polyline"
+    is_closed: Optional[bool] = None
+    parent_id: Optional[AnnotationID] = None
+    stationary: Optional[bool] = False
+    label: Optional[str] = None
+    attributes: Optional[List[AttributePath]] = None
 
 
 @dataclass
-class PolygonAnnotation:
+class PointAnnotation:
     id: AnnotationID
     sensor_id: SensorID
-    path: PolygonPath
-    type: Literal["polygon"] = "polygon"
+    path: AnnotationPath  # x, y, z
+    type: Literal["point"] = "point"
     parent_id: Optional[AnnotationID] = None
     stationary: Optional[bool] = False
     label: Optional[str] = None
     attributes: Optional[List[AttributePath]] = None
 
 
 @dataclass
@@ -284,29 +326,48 @@
     id: AnnotationID
     poses: PosePath
     type: Literal["localization_adjustment"] = "localization_adjustment"
     parent_id: Optional[AnnotationID] = None
 
 
 @dataclass
+class LinkAnnotation:
+    id: AnnotationID
+    sensor_id: SensorID
+    label: str
+    is_bidirectional: bool
+    from_id: AnnotationID
+    to_id: AnnotationID
+    type: Literal["link"] = "link"
+    parent_id: Optional[AnnotationID] = None
+    attributes: Optional[List[AttributePath]] = None
+
+
+@dataclass
 class ObjectAnnotation:
     id: AnnotationID
     type: Literal["object"] = "object"
     parent_id: Optional[AnnotationID] = None
     label: Optional[str] = None
     attributes: Optional[List[AttributePath]] = None
 
 
 Sensor = Union[CameraSensor, LidarSensor, RadarSensor, OdometrySensor, PointsSensor]
 
 Annotation = Union[
     CuboidAnnotation,
     AttributesAnnotation,
     Box2DAnnotation,
-    PolygonAnnotation,
+    Point2DAnnotation,
+    Polyline2DAnnotation,
+    Polygon2DAnnotation,
+    Polyline2DAnnotation,
+    PolylineAnnotation,
+    PointAnnotation,
+    LinkAnnotation,
     LabeledPointsAnnotation,
     LocalizationAdjustmentAnnotation,
     ObjectAnnotation,
 ]
 
 # Define Scene dataclass
```

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/utils/downsample.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/utils/downsample.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/utils/generate_video.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/utils/generate_video.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/__init__.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/LICENSE` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/LICENSE`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/core.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/core.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/dataclasses.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/dacite_internal/types.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/dacite_internal/types.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/error.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/error.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/helpers.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/helpers.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/parser/sfs.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/parser/sfs.py`

 * *Files identical despite different names*

### Comparing `scale_sensor_fusion_io-0.1.3/scale_sensor_fusion_io/validation/validate.py` & `scale_sensor_fusion_io-0.2.0/scale_sensor_fusion_io/validation/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,23 +165,32 @@
                 if frame_num < len(sensor.frames) - 1
                 else None
             )
 
             min_points_ts = np.min(frame.points.timestamps)
             max_points_ts = np.max(frame.points.timestamps)
 
-            if (
-                frame.timestamp > min_points_ts
-                or next_frame_ts
-                and max_points_ts > next_frame_ts
-            ):
+            # NOTE: this is the correct validation, but it is too strict for now. We can add this back as a warning once we support warnings vs errors
+            # if (
+            #     frame.timestamp > min_points_ts
+            #     or next_frame_ts
+            #     and max_points_ts > next_frame_ts
+            # ):
+            #     error_details.append(
+            #         ErrorDetails.from_msg(
+            #             f"point timestamps (range {min_points_ts} -> {max_points_ts}) must be included within consecutive frame timestamps (range {frame.timestamp} -> {next_frame_ts})",
+            #             path=["frames", frame_num, "points"],
+            #         )
+            #     )
+
+            # Simpler check: frame timestamp must be less the min point timestamp
+            if frame.timestamp > min_points_ts:
                 error_details.append(
                     ErrorDetails.from_msg(
-                        f"point timestamps (range {min_points_ts} -> {max_points_ts}) must be included within consecutive frame timestamps (range {frame.timestamp} -> {next_frame_ts})",
-                        path=["frames", frame_num, "points"],
+                        f"frame timestamp ({frame.timestamp}) must be less than min point timestamp ({min_points_ts})",
                     )
                 )
 
     if len(error_details) > 0:
         return DataValidationError(details=error_details)
 
     return None
```

### Comparing `scale_sensor_fusion_io-0.1.3/PKG-INFO` & `scale_sensor_fusion_io-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: scale-sensor-fusion-io
-Version: 0.1.3
+Version: 0.2.0
 Summary: Library for working with timestamp-based sensor fusion scenes
 Author: Michael Choi
 Author-email: michael.choi@scale.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dacite2 (>=2.0.0,<3.0.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
+Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
 Requires-Dist: scale-json-binary (>=0.0.7,<0.0.8)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # sensor-fusion-io
```

