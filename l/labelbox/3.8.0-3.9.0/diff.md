# Comparing `tmp/labelbox-3.8.0.tar.gz` & `tmp/labelbox-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labelbox-3.8.0.tar", last modified: Fri Oct 22 13:26:54 2021, max compression
+gzip compressed data, was "labelbox-3.9.0.tar", last modified: Sat Nov 13 01:01:27 2021, max compression
```

## Comparing `labelbox-3.8.0.tar` & `labelbox-3.9.0.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.668896 labelbox-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-22 13:26:42.000000 labelbox-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-10-22 13:26:42.000000 labelbox-3.8.0/LICENSES
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2021-10-22 13:26:54.668896 labelbox-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5167 2021-10-22 13:26:42.000000 labelbox-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox/
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26722 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox/data/annotation_types/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2697 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox/data/annotation_types/classification/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)    10860 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox/data/annotation_types/data/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/data/base_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/data/raster.py
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/data/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     5428 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/data/video.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox/data/annotation_types/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/mask.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/geometry/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     7653 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/label.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/annotation_types/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/metrics/scalar.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/ner.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/annotation_types/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/metrics/confusion_matrix/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/confusion_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13762 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/confusion_matrix/calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3774 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/confusion_matrix/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     6982 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/group.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/metrics/iou/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/iou/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11522 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/iou/calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/metrics/iou/iou.py
--rw-r--r--   0 runner    (1001) docker     (121)     5544 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/serialization/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/serialization/coco/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     6070 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     8124 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/instance_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/panoptic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      259 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/coco/path.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3538 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/feature.py
--rw-r--r--   0 runner    (1001) docker     (121)     9577 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     8824 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/data/serialization/ndjson/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7964 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5723 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     4583 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     7479 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/data/serialization/ndjson/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.664896 labelbox-3.8.0/labelbox/orm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3629 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/orm/comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)    10993 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/orm/db_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    14192 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/orm/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    17183 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/orm/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.668896 labelbox-3.8.0/labelbox/schema/
--rw-r--r--   0 runner    (1001) docker     (121)      706 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22943 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/annotation_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/asset_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)    29709 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/bulk_import_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3929 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/data_row.py
--rw-r--r--   0 runner    (1001) docker     (121)    18148 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/data_row_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    17475 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/iam_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/invite.py
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/labeling_frontend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/model_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    12155 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/ontology.py
--rw-r--r--   0 runner    (1001) docker     (121)     6796 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/organization.py
--rw-r--r--   0 runner    (1001) docker     (121)    29600 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/review.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     5268 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/schema/webhook.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-10-22 13:26:42.000000 labelbox-3.8.0/labelbox/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-22 13:26:54.660896 labelbox-3.8.0/labelbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2021-10-22 13:26:54.000000 labelbox-3.8.0/labelbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3775 2021-10-22 13:26:54.000000 labelbox-3.8.0/labelbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-22 13:26:54.000000 labelbox-3.8.0/labelbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-10-22 13:26:54.000000 labelbox-3.8.0/labelbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-22 13:26:54.000000 labelbox-3.8.0/labelbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-22 13:26:54.668896 labelbox-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1476 2021-10-22 13:26:42.000000 labelbox-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.521441 labelbox-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-11-13 01:01:13.000000 labelbox-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-11-13 01:01:13.000000 labelbox-3.9.0/LICENSES
+-rw-r--r--   0 runner    (1001) docker     (121)     5827 2021-11-13 01:01:27.521441 labelbox-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5167 2021-11-13 01:01:13.000000 labelbox-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox/
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36114 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox/data/annotation_types/
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2697 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox/data/annotation_types/classification/
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10860 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox/data/annotation_types/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/data/base_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6864 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/data/raster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3005 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/data/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5428 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/data/video.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox/data/annotation_types/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4315 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/mask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1421 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2128 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/geometry/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7653 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/label.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/annotation_types/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1245 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/metrics/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/ner.py
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/annotation_types/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2450 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)      137 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/metrics/confusion_matrix/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/confusion_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13762 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/confusion_matrix/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3774 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/confusion_matrix/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6982 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/metrics/iou/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/iou/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11522 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/iou/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3939 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/metrics/iou/iou.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5544 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/serialization/
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/serialization/coco/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6070 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8124 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/instance_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7644 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/panoptic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      259 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/coco/path.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5658 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3538 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      835 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/feature.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9577 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8824 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/data/serialization/ndjson/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7964 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5723 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4583 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7479 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/data/serialization/ndjson/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.517441 labelbox-3.9.0/labelbox/orm/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3629 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/orm/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10993 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/orm/db_object.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14192 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/orm/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17183 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/orm/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.521441 labelbox-3.9.0/labelbox/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22943 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/annotation_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/asset_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29709 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/bulk_import_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3929 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/data_row.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18288 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/data_row_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17633 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/iam_integration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/invite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2676 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1259 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/labeling_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8552 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/model_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12411 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6796 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/organization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34276 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/review.py
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3735 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5268 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/schema/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2021-11-13 01:01:13.000000 labelbox-3.9.0/labelbox/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 01:01:27.513441 labelbox-3.9.0/labelbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5827 2021-11-13 01:01:27.000000 labelbox-3.9.0/labelbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3775 2021-11-13 01:01:27.000000 labelbox-3.9.0/labelbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 01:01:27.000000 labelbox-3.9.0/labelbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2021-11-13 01:01:27.000000 labelbox-3.9.0/labelbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-13 01:01:27.000000 labelbox-3.9.0/labelbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-13 01:01:27.521441 labelbox-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1476 2021-11-13 01:01:13.000000 labelbox-3.9.0/setup.py
```

### Comparing `labelbox-3.8.0/LICENSE` & `labelbox-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/LICENSES` & `labelbox-3.9.0/LICENSES`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/PKG-INFO` & `labelbox-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbox
-Version: 3.8.0
+Version: 3.9.0
 Summary: Labelbox Python API
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: engineering@labelbox.com
 License: UNKNOWN
 Keywords: labelbox
 Platform: UNKNOWN
```

### Comparing `labelbox-3.8.0/README.md` & `labelbox-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/__init__.py` & `labelbox-3.9.0/labelbox/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name = "labelbox"
-__version__ = "3.8.0"
+__version__ = "3.9.0"
 
 from labelbox.schema.project import Project
 from labelbox.client import Client
 from labelbox.schema.model import Model
 from labelbox.schema.bulk_import_request import BulkImportRequest
 from labelbox.schema.annotation_import import MALPredictionImport, MEAPredictionImport, LabelImport
 from labelbox.schema.dataset import Dataset
@@ -12,12 +12,12 @@
 from labelbox.schema.review import Review
 from labelbox.schema.user import User
 from labelbox.schema.organization import Organization
 from labelbox.schema.task import Task
 from labelbox.schema.labeling_frontend import LabelingFrontend
 from labelbox.schema.asset_attachment import AssetAttachment
 from labelbox.schema.webhook import Webhook
-from labelbox.schema.ontology import Ontology, OntologyBuilder, Classification, Option, Tool
+from labelbox.schema.ontology import Ontology, OntologyBuilder, Classification, Option, Tool, FeatureSchema
 from labelbox.schema.role import Role, ProjectRole
 from labelbox.schema.invite import Invite, InviteLimit
 from labelbox.schema.data_row_metadata import DataRowMetadataOntology
 from labelbox.schema.model_run import ModelRun
```

### Comparing `labelbox-3.8.0/labelbox/client.py` & `labelbox-3.9.0/labelbox/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,25 +13,20 @@
 import requests.exceptions
 
 import labelbox.exceptions
 from labelbox import utils
 from labelbox import __version__ as SDK_VERSION
 from labelbox.orm import query
 from labelbox.orm.db_object import DbObject
+from labelbox.orm.model import Entity
 from labelbox.pagination import PaginatedCollection
-from labelbox.schema.project import Project
-from labelbox.schema.dataset import Dataset
-from labelbox.schema.data_row import DataRow
-from labelbox.schema.model import Model
-from labelbox.schema.user import User
-from labelbox.schema.organization import Organization
 from labelbox.schema.data_row_metadata import DataRowMetadataOntology
-from labelbox.schema.labeling_frontend import LabelingFrontend
 from labelbox.schema.iam_integration import IAMIntegration
 from labelbox.schema import role
+from labelbox.schema.ontology import Tool, Classification
 
 logger = logging.getLogger(__name__)
 
 _LABELBOX_API_KEY = "LABELBOX_API_KEY"
 
 
 class Client:
@@ -197,15 +192,15 @@
                 for path_elem in path:
                     obj = obj.get(path_elem, {})
                 if obj in keywords:
                     return error
             return None
 
         def get_error_status_code(error):
-            return error["extensions"]["exception"]["status"]
+            return error["extensions"]["exception"].get("status")
 
         if check_errors(["AUTHENTICATION_ERROR"], "extensions",
                         "code") is not None:
             raise labelbox.exceptions.AuthenticationError("Invalid API key")
 
         authorization_error = check_errors(["AUTHORIZATION_ERROR"],
                                            "extensions", "code")
@@ -238,14 +233,26 @@
         resource_not_found_error = check_errors(["RESOURCE_NOT_FOUND"],
                                                 "extensions", "code")
         if resource_not_found_error is not None:
             # Return None and let the caller methods raise an exception
             # as they already know which resource type and ID was requested
             return None
 
+        resource_conflict_error = check_errors(["RESOURCE_CONFLICT"],
+                                               "extensions", "code")
+        if resource_conflict_error is not None:
+            raise labelbox.exceptions.ResourceConflict(
+                resource_conflict_error["message"])
+
+        malformed_request_error = check_errors(["MALFORMED_REQUEST"],
+                                               "extensions", "code")
+        if malformed_request_error is not None:
+            raise labelbox.exceptions.MalformedQueryException(
+                malformed_request_error["message"])
+
         # A lot of different error situations are now labeled serverside
         # as INTERNAL_SERVER_ERROR, when they are actually client errors.
         # TODO: fix this in the server API
         internal_server_error = check_errors(["INTERNAL_SERVER_ERROR"],
                                              "extensions", "code")
         if internal_server_error is not None:
             message = internal_server_error.get("message")
@@ -259,16 +266,22 @@
                                          "extensions", "code")
         if not_allowed_error is not None:
             message = not_allowed_error.get("message")
             raise labelbox.exceptions.OperationNotAllowedException(message)
 
         if len(errors) > 0:
             logger.warning("Unparsed errors on query execution: %r", errors)
+            messages = list(
+                map(
+                    lambda x: {
+                        "message": x["message"],
+                        "code": x["extensions"]["code"]
+                    }, errors))
             raise labelbox.exceptions.LabelboxError("Unknown error: %s" %
-                                                    str(errors))
+                                                    str(messages))
 
         # if we do return a proper error code, and didn't catch this above
         # reraise
         # this mainly catches a 401 for API access disabled for free tier
         # TODO: need to unify API errors to handle things more uniformly
         # in the SDK
         if response.status_code != requests.codes.ok:
@@ -392,45 +405,45 @@
             project_id (str): Unique ID of the Project.
         Returns:
             The sought Project.
         Raises:
             labelbox.exceptions.ResourceNotFoundError: If there is no
                 Project with the given ID.
         """
-        return self._get_single(Project, project_id)
+        return self._get_single(Entity.Project, project_id)
 
     def get_dataset(self, dataset_id):
         """ Gets a single Dataset with the given ID.
 
             >>> dataset = client.get_dataset("<dataset_id>")
 
         Args:
             dataset_id (str): Unique ID of the Dataset.
         Returns:
             The sought Dataset.
         Raises:
             labelbox.exceptions.ResourceNotFoundError: If there is no
                 Dataset with the given ID.
         """
-        return self._get_single(Dataset, dataset_id)
+        return self._get_single(Entity.Dataset, dataset_id)
 
     def get_user(self):
         """ Gets the current User database object.
 
             >>> user = client.get_user()
         """
-        return self._get_single(User, None)
+        return self._get_single(Entity.User, None)
 
     def get_organization(self):
         """ Gets the Organization DB object of the current user.
 
             >>> organization = client.get_organization()
 
         """
-        return self._get_single(Organization, None)
+        return self._get_single(Entity.Organization, None)
 
     def _get_all(self, db_object_type, where, filter_deleted=True):
         """ Fetches all the objects of the given type the user has access to.
 
         Args:
             db_object_type (type): DbObject subclass.
             where (Comparison, LogicalOperation or None): The `where` clause
@@ -455,41 +468,41 @@
 
         Args:
             where (Comparison, LogicalOperation or None): The `where` clause
                 for filtering.
         Returns:
             An iterable of Projects (typically a PaginatedCollection).
         """
-        return self._get_all(Project, where)
+        return self._get_all(Entity.Project, where)
 
     def get_datasets(self, where=None):
         """ Fetches one or more datasets.
 
             >>> datasets = client.get_datasets(where=(Dataset.name == "<dataset_name>") & (Dataset.description == "<dataset_description>"))
 
         Args:
             where (Comparison, LogicalOperation or None): The `where` clause
                 for filtering.
         Returns:
             An iterable of Datasets (typically a PaginatedCollection).
         """
-        return self._get_all(Dataset, where)
+        return self._get_all(Entity.Dataset, where)
 
     def get_labeling_frontends(self, where=None):
         """ Fetches all the labeling frontends.
 
             >>> frontend = client.get_labeling_frontends(where=LabelingFrontend.name == "Editor")
 
         Args:
             where (Comparison, LogicalOperation or None): The `where` clause
                 for filtering.
         Returns:
             An iterable of LabelingFrontends (typically a PaginatedCollection).
         """
-        return self._get_all(LabelingFrontend, where)
+        return self._get_all(Entity.LabelingFrontend, where)
 
     def _create(self, db_object_type, data):
         """ Creates an object on the server. Attribute values are
             passed as keyword arguments:
 
         Args:
             db_object_type (type): A DbObjectType subtype.
@@ -528,31 +541,33 @@
             **kwargs: Keyword arguments with Dataset attribute values.
         Returns:
             A new Dataset object.
         Raises:
             InvalidAttributeError: If the Dataset type does not contain
                 any of the attribute names given in kwargs.
         """
-        dataset = self._create(Dataset, kwargs)
+        dataset = self._create(Entity.Dataset, kwargs)
 
         if iam_integration == IAMIntegration._DEFAULT:
             iam_integration = self.get_organization(
             ).get_default_iam_integration()
 
         if iam_integration is None:
             return dataset
 
-        if not isinstance(iam_integration, IAMIntegration):
-            raise TypeError(
-                f"iam integration must be a reference an `IAMIntegration` object. Found {type(iam_integration)}"
-            )
-
-        if not iam_integration.valid:
-            raise ValueError("Integration is not valid. Please select another.")
         try:
+            if not isinstance(iam_integration, IAMIntegration):
+                raise TypeError(
+                    f"iam integration must be a reference an `IAMIntegration` object. Found {type(iam_integration)}"
+                )
+
+            if not iam_integration.valid:
+                raise ValueError(
+                    "Integration is not valid. Please select another.")
+
             self.execute(
                 """mutation setSignerForDatasetPyApi($signerId: ID!, $datasetId: ID!) {
                     setSignerForDataset(data: { signerId: $signerId}, where: {id: $datasetId}){id}}
                 """, {
                     'signerId': iam_integration.uid,
                     'datasetId': dataset.uid
                 })
@@ -581,15 +596,15 @@
             **kwargs: Keyword arguments with Project attribute values.
         Returns:
             A new Project object.
         Raises:
             InvalidAttributeError: If the Project type does not contain
                 any of the attribute names given in kwargs.
         """
-        return self._create(Project, kwargs)
+        return self._create(Entity.Project, kwargs)
 
     def get_roles(self):
         """
         Returns:
             Roles: Provides information on available roles within an organization.
             Roles are used for user management.
         """
@@ -598,15 +613,15 @@
     def get_data_row(self, data_row_id):
         """
 
         Returns:
             DataRow: returns a single data row given the data row id
         """
 
-        return self._get_single(DataRow, data_row_id)
+        return self._get_single(Entity.DataRow, data_row_id)
 
     def get_data_row_metadata_ontology(self):
         """
 
         Returns:
             DataRowMetadataOntology: The ontology for Data Row Metadata for an organization
 
@@ -622,28 +637,28 @@
             model_id (str): Unique ID of the Model.
         Returns:
             The sought Model.
         Raises:
             labelbox.exceptions.ResourceNotFoundError: If there is no
                 Model with the given ID.
         """
-        return self._get_single(Model, model_id)
+        return self._get_single(Entity.Model, model_id)
 
     def get_models(self, where=None):
         """ Fetches all the models the user has access to.
 
             >>> models = client.get_models(where=(Model.name == "<model_name>"))
 
         Args:
             where (Comparison, LogicalOperation or None): The `where` clause
                 for filtering.
         Returns:
             An iterable of Models (typically a PaginatedCollection).
         """
-        return self._get_all(Model, where, filter_deleted=False)
+        return self._get_all(Entity.Model, where, filter_deleted=False)
 
     def create_model(self, name, ontology_id):
         """ Creates a Model object on the server.
 
         >>> model = client.create_model(<model_name>, <ontology_id>)
 
         Args:
@@ -655,21 +670,21 @@
             InvalidAttributeError: If the Model type does not contain
                 any of the attribute names given in kwargs.
         """
         query_str = """mutation createModelPyApi($name: String!, $ontologyId: ID!){
             createModel(data: {name : $name, ontologyId : $ontologyId}){
                     %s
                 }
-            }""" % query.results_query_part(Model)
+            }""" % query.results_query_part(Entity.Model)
 
         result = self.execute(query_str, {
             "name": name,
             "ontologyId": ontology_id
         })
-        return Model(self, result['createModel'])
+        return Entity.Model(self, result['createModel'])
 
     def get_data_row_ids_for_external_ids(
             self, external_ids: List[str]) -> Dict[str, List[str]]:
         """
         Returns a list of data row ids for a list of external ids.
         There is a max of 1500 items returned at a time.
 
@@ -687,7 +702,197 @@
         for i in range(0, len(external_ids), max_ids_per_request):
             for row in self.execute(
                     query_str,
                 {'externalId_in': external_ids[i:i + max_ids_per_request]
                 })['externalIdsToDataRowIds']:
                 result[row['externalId']].append(row['dataRowId'])
         return result
+
+    def get_ontology(self, ontology_id):
+        """
+        Fetches an Ontology by id.
+
+        Args:
+            ontology_id (str): The id of the ontology to query for
+        Returns:
+            Ontology
+        """
+        return self._get_single(Entity.Ontology, ontology_id)
+
+    def get_ontologies(self, name_contains):
+        """
+        Fetches all ontologies with names that match the name_contains string.
+
+        Args:
+            name_contains (str): the string to search ontology names by
+        Returns:
+            PaginatedCollection of Ontologies with names that match `name_contains`
+        """
+        query_str = """query getOntologiesPyApi($search: String, $filter: OntologyFilter, $from : String, $first: PageSize){
+            ontologies(where: {filter: $filter, search: $search}, after: $from, first: $first){
+                nodes {%s}
+                nextCursor
+            }
+        }
+        """ % query.results_query_part(Entity.Ontology)
+        params = {'search': name_contains, 'filter': {'status': 'ALL'}}
+        return PaginatedCollection(self, query_str, params,
+                                   ['ontologies', 'nodes'], Entity.Ontology,
+                                   ['ontologies', 'nextCursor'])
+
+    def get_feature_schema(self, feature_schema_id):
+        """
+        Fetches a feature schema. Only supports top level feature schemas.
+
+        Args:
+            feature_schema_id (str): The id of the feature schema to query for
+        Returns:
+            FeatureSchema
+        """
+
+        query_str = """query rootSchemaNodePyApi($rootSchemaNodeWhere: RootSchemaNodeWhere!){
+              rootSchemaNode(where: $rootSchemaNodeWhere){%s}
+        }""" % query.results_query_part(Entity.FeatureSchema)
+        res = self.execute(
+            query_str,
+            {'rootSchemaNodeWhere': {
+                'featureSchemaId': feature_schema_id
+            }})['rootSchemaNode']
+        res['id'] = res['normalized']['featureSchemaId']
+        return Entity.FeatureSchema(self, res)
+
+    def get_feature_schemas(self, name_contains):
+        """
+        Fetches top level feature schemas with names that match the `name_contains` string
+
+        Args:
+            name_contains (str): the string to search top level feature schema names by
+        Returns:
+            PaginatedCollection of FeatureSchemas with names that match `name_contains`
+        """
+        query_str = """query rootSchemaNodesPyApi($search: String, $filter: RootSchemaNodeFilter, $from : String, $first: PageSize){
+            rootSchemaNodes(where: {filter: $filter, search: $search}, after: $from, first: $first){
+                nodes {%s}
+                nextCursor
+            }
+        }
+        """ % query.results_query_part(Entity.FeatureSchema)
+        params = {'search': name_contains, 'filter': {'status': 'ALL'}}
+
+        def rootSchemaPayloadToFeatureSchema(client, payload):
+            # Technically we are querying for a Schema Node.
+            # But the features are the same so we just grab the feature schema id
+            payload['id'] = payload['normalized']['featureSchemaId']
+            return Entity.FeatureSchema(client, payload)
+
+        return PaginatedCollection(self, query_str, params,
+                                   ['rootSchemaNodes', 'nodes'],
+                                   rootSchemaPayloadToFeatureSchema,
+                                   ['rootSchemaNodes', 'nextCursor'])
+
+    def create_ontology_from_feature_schemas(self, name, feature_schema_ids):
+        """
+        Creates an ontology from a list of feature schema ids
+
+        Args:
+            name (str): Name of the ontology
+            feature_schema_ids (List[str]): List of feature schema ids corresponding to
+                top level tools and classifications to include in the ontology
+        Returns:
+            The created Ontology
+        """
+        tools, classifications = [], []
+        for feature_schema_id in feature_schema_ids:
+            feature_schema = self.get_feature_schema(feature_schema_id)
+            tool = ['tool']
+            if 'tool' in feature_schema.normalized:
+                tool = feature_schema.normalized['tool']
+                try:
+                    Tool.Type(tool)
+                    tools.append(feature_schema.normalized)
+                except ValueError:
+                    raise ValueError(
+                        f"Tool `{tool}` not in list of supported tools.")
+            elif 'type' in feature_schema.normalized:
+                classification = feature_schema.normalized['type']
+                try:
+                    Classification.Type(classification)
+                    classifications.append(feature_schema.normalized)
+                except ValueError:
+                    raise ValueError(
+                        f"Classification `{classification}` not in list of supported classifications."
+                    )
+            else:
+                raise ValueError(
+                    "Neither `tool` or `classification` found in the normalized feature schema"
+                )
+        normalized = {'tools': tools, 'classifications': classifications}
+        return self.create_ontology(name, normalized)
+
+    def create_ontology(self, name, normalized):
+        """
+        Creates an ontology from normalized data
+            >>> normalized = {"tools" : [{'tool': 'polygon',  'name': 'cat', 'color': 'black'}], "classifications" : []}
+            >>> ontology = client.create_ontology("ontology-name", normalized)
+
+        Or use the ontology builder. It is especially useful for complex ontologies
+            >>> normalized = OntologyBuilder(tools=[Tool(tool=Tool.Type.BBOX, name="cat", color = 'black')]).asdict()
+            >>> ontology = client.create_ontology("ontology-name", normalized)
+
+        To reuse existing feature schemas, use `create_ontology_from_feature_schemas()`
+        More details can be found here:
+            https://github.com/Labelbox/labelbox-python/blob/develop/examples/basics/ontologies.ipynb
+
+        Args:
+            name (str): Name of the ontology
+            normalized (dict): A normalized ontology payload. See above for details.
+        Returns:
+            The created Ontology
+        """
+        query_str = """mutation upsertRootSchemaNodePyApi($data:  UpsertOntologyInput!){
+                           upsertOntology(data: $data){ %s }
+        } """ % query.results_query_part(Entity.Ontology)
+        params = {'data': {'name': name, 'normalized': json.dumps(normalized)}}
+        res = self.execute(query_str, params)
+        return Entity.Ontology(self, res['upsertOntology'])
+
+    def create_feature_schema(self, normalized):
+        """
+        Creates a feature schema from normalized data.
+            >>> normalized = {'tool': 'polygon',  'name': 'cat', 'color': 'black'}
+            >>> feature_schema = client.create_feature_schema(normalized)
+
+        Or use the Tool or Classification objects. It is especially useful for complex tools.
+            >>> normalized = Tool(tool=Tool.Type.BBOX, name="cat", color = 'black').asdict()
+            >>> feature_schema = client.create_feature_schema(normalized)
+
+        Subclasses are also supported
+            >>> normalized =  Tool(
+                    tool=Tool.Type.SEGMENTATION,
+                    name="cat",
+                    classifications=[
+                        Classification(
+                            class_type=Classification.Type.TEXT,
+                            instructions="name"
+                        )
+                    ]
+                )
+            >>> feature_schema = client.create_feature_schema(normalized)
+
+        More details can be found here:
+            https://github.com/Labelbox/labelbox-python/blob/develop/examples/basics/ontologies.ipynb
+
+        Args:
+            normalized (dict): A normalized tool or classification payload. See above for details
+        Returns:
+            The created FeatureSchema.
+        """
+        query_str = """mutation upsertRootSchemaNodePyApi($data:  UpsertRootSchemaNodeInput!){
+                        upsertRootSchemaNode(data: $data){ %s }
+        } """ % query.results_query_part(Entity.FeatureSchema)
+        normalized = {k: v for k, v in normalized.items() if v}
+        params = {'data': {'normalized': json.dumps(normalized)}}
+        res = self.execute(query_str, params)['upsertRootSchemaNode']
+        # Technically we are querying for a Schema Node.
+        # But the features are the same so we just grab the feature schema id
+        res['id'] = res['normalized']['featureSchemaId']
+        return Entity.FeatureSchema(self, res)
```

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/__init__.py` & `labelbox-3.9.0/labelbox/data/annotation_types/__init__.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/annotation.py` & `labelbox-3.9.0/labelbox/data/annotation_types/annotation.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/classification/classification.py` & `labelbox-3.9.0/labelbox/data/annotation_types/classification/classification.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,26 +25,38 @@
     - Because it inherits from FeatureSchema
         the option can be represented with either the name or feature_schema_id
     """
     extra: Dict[str, Any] = {}
 
 
 class Radio(BaseModel):
-    """ A classification with only one selected option allowed """
+    """ A classification with only one selected option allowed
+    
+    >>> Radio(answer = ClassificationAnswer(name = "dog"))
+
+    """
     answer: ClassificationAnswer
 
 
 class Checklist(_TempName):
-    """ A classification with many selected options allowed """
+    """ A classification with many selected options allowed
+
+    >>> Checklist(answer = [ClassificationAnswer(name = "cloudy")])
+
+    """
     name: Literal["checklist"] = "checklist"
     answer: List[ClassificationAnswer]
 
 
 class Text(BaseModel):
-    """ Free form text """
+    """ Free form text
+
+    >>> Text(answer = "some text answer") 
+
+    """
     answer: str
 
 
 class Dropdown(_TempName):
     """
     - A classification with many selected options allowed .
     - This is not currently compatible with MAL.
```

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/collection.py` & `labelbox-3.9.0/labelbox/data/annotation_types/collection.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/data/raster.py` & `labelbox-3.9.0/labelbox/data/annotation_types/data/raster.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/data/text.py` & `labelbox-3.9.0/labelbox/data/annotation_types/data/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 from pydantic import root_validator
 
 from .base_data import BaseData
 
 
 class TextData(BaseData):
     """
-    Represents text data
+    Represents text data. Requires arg file_path, text, or url
+
+    >>> TextData(text="") 
+
+    Args:
+        file_path (str)
+        text (str)
+        url (str)
     """
     file_path: Optional[str] = None
     text: Optional[str] = None
     url: Optional[str] = None
 
     @property
     def value(self) -> str:
```

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/data/video.py` & `labelbox-3.9.0/labelbox/data/annotation_types/data/video.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/feature.py` & `labelbox-3.9.0/labelbox/data/annotation_types/feature.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/geometry/geometry.py` & `labelbox-3.9.0/labelbox/data/annotation_types/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/geometry/line.py` & `labelbox-3.9.0/labelbox/data/annotation_types/geometry/point.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import List, Optional, Union, Tuple
+from typing import Optional, Tuple, Union
 
 import geojson
 import numpy as np
 import cv2
 
-from .point import Point
 from .geometry import Geometry
 
 
-class Line(Geometry):
-    """Line annotation
+class Point(Geometry):
+    """Point geometry
+
+    >>> Point(x=0, y=0)
 
     Args:
-        points (List[Point]): A list of `Point` geometries
+        x (float)
+        y (float)
 
     """
-    points: List[Point]
+    x: float
+    y: float
 
     @property
-    def geometry(self) -> geojson.MultiLineString:
-        return geojson.MultiLineString(
-            [[[point.x, point.y] for point in self.points]])
+    def geometry(self) -> geojson.Point:
+        return geojson.Point((self.x, self.y))
 
     def draw(self,
              height: Optional[int] = None,
              width: Optional[int] = None,
              canvas: Optional[np.ndarray] = None,
              color: Union[int, Tuple[int, int, int]] = (255, 255, 255),
-             thickness: int = 1) -> np.ndarray:
+             thickness: int = 10) -> np.ndarray:
         """
-        Draw the line onto a 3d mask
+        Draw the point onto a 3d mask
         Args:
             height (int): height of the mask
             width (int): width of the mask
-            thickness (int): How thick to draw the line
-            color (int): color for the line.
+            thickness (int): pixel radius of the point
+            color (int): color for the point.
                   RGB values by default but if a 2D canvas is provided this can set this to an int.
-            canvas (np.ndarry): Canvas for drawing line on.
+            canvas (np.ndarray): Canvas to draw the point on
         Returns:
-            numpy array representing the mask with the line drawn on it.
+            numpy array representing the mask with the point drawn on it.
         """
         canvas = self.get_or_create_canvas(height, width, canvas)
-        pts = np.array(self.geometry['coordinates']).astype(np.int32)
-        return cv2.polylines(canvas,
-                             pts,
-                             False,
-                             color=color,
-                             thickness=thickness)
+        return cv2.circle(canvas, (int(self.x), int(self.y)),
+                          radius=thickness,
+                          color=color,
+                          thickness=-1)
```

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/geometry/mask.py` & `labelbox-3.9.0/labelbox/data/annotation_types/geometry/mask.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/geometry/polygon.py` & `labelbox-3.9.0/labelbox/data/annotation_types/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/geometry/rectangle.py` & `labelbox-3.9.0/labelbox/data/annotation_types/geometry/rectangle.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/label.py` & `labelbox-3.9.0/labelbox/data/annotation_types/label.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/metrics/base.py` & `labelbox-3.9.0/labelbox/data/annotation_types/metrics/base.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/metrics/confusion_matrix.py` & `labelbox-3.9.0/labelbox/data/annotation_types/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/metrics/scalar.py` & `labelbox-3.9.0/labelbox/data/annotation_types/metrics/scalar.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/ner.py` & `labelbox-3.9.0/labelbox/data/annotation_types/ner.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/annotation_types/types.py` & `labelbox-3.9.0/labelbox/data/annotation_types/types.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/generator.py` & `labelbox-3.9.0/labelbox/data/generator.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/metrics/confusion_matrix/calculation.py` & `labelbox-3.9.0/labelbox/data/metrics/confusion_matrix/calculation.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/metrics/confusion_matrix/confusion_matrix.py` & `labelbox-3.9.0/labelbox/data/metrics/confusion_matrix/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/metrics/group.py` & `labelbox-3.9.0/labelbox/data/metrics/group.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/metrics/iou/calculation.py` & `labelbox-3.9.0/labelbox/data/metrics/iou/calculation.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/metrics/iou/iou.py` & `labelbox-3.9.0/labelbox/data/metrics/iou/iou.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/ontology.py` & `labelbox-3.9.0/labelbox/data/ontology.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/coco/annotation.py` & `labelbox-3.9.0/labelbox/data/serialization/coco/annotation.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/coco/converter.py` & `labelbox-3.9.0/labelbox/data/serialization/coco/converter.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/coco/image.py` & `labelbox-3.9.0/labelbox/data/serialization/coco/image.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/coco/instance_dataset.py` & `labelbox-3.9.0/labelbox/data/serialization/coco/instance_dataset.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/coco/panoptic_dataset.py` & `labelbox-3.9.0/labelbox/data/serialization/coco/panoptic_dataset.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/classification.py` & `labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/classification.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/converter.py` & `labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/converter.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/feature.py` & `labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/feature.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/label.py` & `labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/label.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/labelbox_v1/objects.py` & `labelbox-3.9.0/labelbox/data/serialization/labelbox_v1/objects.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/ndjson/base.py` & `labelbox-3.9.0/labelbox/data/serialization/ndjson/base.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/ndjson/classification.py` & `labelbox-3.9.0/labelbox/data/serialization/ndjson/classification.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/ndjson/converter.py` & `labelbox-3.9.0/labelbox/data/serialization/ndjson/converter.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/ndjson/label.py` & `labelbox-3.9.0/labelbox/data/serialization/ndjson/label.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/ndjson/metric.py` & `labelbox-3.9.0/labelbox/data/serialization/ndjson/metric.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/data/serialization/ndjson/objects.py` & `labelbox-3.9.0/labelbox/data/serialization/ndjson/objects.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/exceptions.py` & `labelbox-3.9.0/labelbox/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,19 @@
         """
         super().__init__("Resource '%s' not found for params: %r" %
                          (db_object_type.type_name(), params))
         self.db_object_type = db_object_type
         self.params = params
 
 
+class ResourceConflict(LabelboxError):
+    """Exception raised when a given resource conflicts with another. """
+    pass
+
+
 class ValidationFailedError(LabelboxError):
     """Exception raised for when a GraphQL query fails validation (query cost,
     etc.) E.g. a query that is too expensive, or depth is too deep.
     """
     pass
```

### Comparing `labelbox-3.8.0/labelbox/orm/comparison.py` & `labelbox-3.9.0/labelbox/orm/comparison.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/orm/db_object.py` & `labelbox-3.9.0/labelbox/orm/db_object.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/orm/model.py` & `labelbox-3.9.0/labelbox/orm/model.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/orm/query.py` & `labelbox-3.9.0/labelbox/orm/query.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/pagination.py` & `labelbox-3.9.0/labelbox/pagination.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/__init__.py` & `labelbox-3.9.0/labelbox/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/annotation_import.py` & `labelbox-3.9.0/labelbox/schema/annotation_import.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/asset_attachment.py` & `labelbox-3.9.0/labelbox/schema/asset_attachment.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/benchmark.py` & `labelbox-3.9.0/labelbox/schema/benchmark.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/bulk_import_request.py` & `labelbox-3.9.0/labelbox/schema/bulk_import_request.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/data_row.py` & `labelbox-3.9.0/labelbox/schema/data_row.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/data_row_metadata.py` & `labelbox-3.9.0/labelbox/schema/data_row_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     reserved: bool
     kind: DataRowMetadataKind
     options: Optional[List["DataRowMetadataSchema"]]
     parent: Optional[SchemaId]
 
     @property
     def id(self):
+        """ `DataRowMetadataSchema.id is being deprecated after version 3.9 
+            in favor of DataRowMetadataSchema.uid`
+        """
         warnings.warn("`id` is being deprecated in favor of `uid`")
         return self.uid
 
 
 DataRowMetadataSchema.update_forward_refs()
 
 Embedding: Type[List[float]] = conlist(float, min_items=128, max_items=128)
```

### Comparing `labelbox-3.8.0/labelbox/schema/dataset.py` & `labelbox-3.9.0/labelbox/schema/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,19 @@
         if len(data_rows) > 1:
             logger.warning(
                 f"More than one data_row has the provided external_id : `%s`. Use function data_rows_for_external_id to fetch all",
                 external_id)
         return data_rows[0]
 
     def export_data_rows(self, timeout_seconds=120):
-        """ Returns a generator that produces all data rows that are currently attached to this dataset.
+        """ Returns a generator that produces all data rows that are currently
+        attached to this dataset.
+
+        Note: For efficiency, the data are cached for 30 minutes. Newly created data rows will not appear
+        until the end of the cache period.
 
         Args:
             timeout_seconds (float): Max waiting time, in seconds.
         Returns:
             Generator that yields DataRow objects belonging to this dataset.
         Raises:
             LabelboxError: if the export fails or is unable to download within the specified time.
```

### Comparing `labelbox-3.8.0/labelbox/schema/enums.py` & `labelbox-3.9.0/labelbox/schema/enums.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/iam_integration.py` & `labelbox-3.9.0/labelbox/schema/iam_integration.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/invite.py` & `labelbox-3.9.0/labelbox/schema/invite.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/label.py` & `labelbox-3.9.0/labelbox/schema/label.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/labeling_frontend.py` & `labelbox-3.9.0/labelbox/schema/labeling_frontend.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/model.py` & `labelbox-3.9.0/labelbox/schema/model.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/model_run.py` & `labelbox-3.9.0/labelbox/schema/model_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,17 @@
         return PaginatedCollection(
             self.client, query_str, {'modelRunId': self.uid},
             ['annotationGroups', 'nodes'],
             lambda client, res: ModelRunDataRow(client, self.model_id, res),
             ['annotationGroups', 'pageInfo', 'endCursor'])
 
     def annotation_groups(self):
+        """ `ModelRun.annotation_groups is being deprecated after version 3.9 
+            in favor of ModelRun.model_run_data_rows`
+        """
         warnings.warn(
             "`ModelRun.annotation_groups` is being deprecated in favor of `ModelRun.model_run_data_rows`"
         )
         return self.model_run_data_rows()
 
     def delete(self):
         """ Deletes specified model run.
@@ -177,14 +180,17 @@
             data_row_ids_param)
         self.client.execute(query_str, {
             model_run_id_param: self.uid,
             data_row_ids_param: data_row_ids
         })
 
     def delete_annotation_groups(self, data_row_ids):
+        """ `ModelRun.delete_annotation_groups is being deprecated after version 3.9 
+            in favor of ModelRun.delete_model_run_data_rows`
+        """
         warnings.warn(
             "`ModelRun.delete_annotation_groups` is being deprecated in favor of `ModelRun.delete_model_run_data_rows`"
         )
         return self.delete_model_run_data_rows(data_row_ids)
 
 
 class ModelRunDataRow(DbObject):
```

### Comparing `labelbox-3.8.0/labelbox/schema/ontology.py` & `labelbox-3.9.0/labelbox/schema/ontology.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 from labelbox.orm.db_object import DbObject
 from labelbox.orm.model import Field, Relationship
 
 FeatureSchemaId: Type[str] = constr(min_length=25, max_length=25)
 SchemaId: Type[str] = constr(min_length=25, max_length=25)
 
 
+class FeatureSchema(DbObject):
+    name = Field.String("name")
+    color = Field.String("name")
+    normalized = Field.Json("normalized")
+
+
 @dataclass
 class Option:
     """
     An option is a possible answer within a Classification object in
     a Project's ontology.
 
     To instantiate, only the "value" parameter needs to be passed in.
@@ -336,14 +342,18 @@
                 self.tools[index].color = '#%02x%02x%02x' % rgb_color
 
     @classmethod
     def from_project(cls, project: "project.Project"):
         ontology = project.ontology().normalized
         return cls.from_dict(ontology)
 
+    @classmethod
+    def from_ontology(cls, ontology: Ontology):
+        return cls.from_dict(ontology.normalized)
+
     def add_tool(self, tool: Tool):
         if tool.name in (t.name for t in self.tools):
             raise InconsistentOntologyException(
                 f"Duplicate tool name '{tool.name}'. ")
         self.tools.append(tool)
 
     def add_classification(self, classification: Classification):
```

### Comparing `labelbox-3.8.0/labelbox/schema/organization.py` & `labelbox-3.9.0/labelbox/schema/organization.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/project.py` & `labelbox-3.9.0/labelbox/schema/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,57 @@
+import enum
 import json
-import time
 import logging
+import time
+import warnings
 from collections import namedtuple
 from datetime import datetime, timezone
 from pathlib import Path
-from typing import Dict, Union, Iterable
+from typing import Dict, Union, Iterable, List, Optional
 from urllib.parse import urlparse
-import requests
+
 import ndjson
+import requests
 
 from labelbox import utils
-from labelbox.schema.data_row import DataRow
-from labelbox.orm import query
-from labelbox.schema.bulk_import_request import BulkImportRequest
 from labelbox.exceptions import InvalidQueryError, LabelboxError
+from labelbox.orm import query
 from labelbox.orm.db_object import DbObject, Updateable, Deletable
 from labelbox.orm.model import Entity, Field, Relationship
 from labelbox.pagination import PaginatedCollection
+from labelbox.schema.bulk_import_request import BulkImportRequest
+from labelbox.schema.data_row import DataRow
 
 try:
     datetime.fromisoformat  # type: ignore[attr-defined]
 except AttributeError:
     from backports.datetime_fromisoformat import MonkeyPatch
+
     MonkeyPatch.patch_fromisoformat()
 
 try:
     from labelbox.data.serialization import LBV1Converter
 except ImportError:
     pass
 
 logger = logging.getLogger(__name__)
 
+MAX_QUEUE_BATCH_SIZE = 1000
+
+
+class QueueMode(enum.Enum):
+    Batch = "Batch"
+    Dataset = "Dataset"
+
+
+class QueueErrors(enum.Enum):
+    InvalidDataRowType = 'InvalidDataRowType'
+    AlreadyInProject = 'AlreadyInProject'
+    HasAttachedLabel = 'HasAttachedLabel'
+
 
 class Project(DbObject, Updateable, Deletable):
     """ A Project is a container that includes a labeling frontend, an ontology,
     datasets and labels.
 
     Attributes:
         name (str)
@@ -75,14 +92,22 @@
         "LabelingFrontendOptions", False, "labeling_frontend_options")
     labeling_parameter_overrides = Relationship.ToMany(
         "LabelingParameterOverride", False, "labeling_parameter_overrides")
     webhooks = Relationship.ToMany("Webhook", False)
     benchmarks = Relationship.ToMany("Benchmark", False)
     ontology = Relationship.ToOne("Ontology", True)
 
+    def update(self, **kwargs):
+
+        mode: Optional[QueueMode] = kwargs.pop("queue_mode", None)
+        if mode:
+            self._update_queue_mode(mode)
+
+        return super().update(**kwargs)
+
     def members(self):
         """ Fetch all current members for this project
 
         Returns:
             A `PaginatedCollection of `ProjectMember`s
 
         """
@@ -393,41 +418,173 @@
         query_str = """query ProjectReviewMetricsPyApi($%s: ID!){
             project(where: {id:$%s})
             {reviewMetrics {labelAggregate(netScore: %s) {count}}}
         }""" % (id_param, id_param, net_score_literal)
         res = self.client.execute(query_str, {id_param: self.uid})
         return res["project"]["reviewMetrics"]["labelAggregate"]["count"]
 
+    def setup_editor(self, ontology):
+        """
+        Sets up the project using the Pictor editor.
+
+        Args:
+            ontology (Ontology): The ontology to attach to the project
+        """
+        labeling_frontend = next(
+            self.client.get_labeling_frontends(
+                where=Entity.LabelingFrontend.name == "Editor"))
+        self.labeling_frontend.connect(labeling_frontend)
+
+        LFO = Entity.LabelingFrontendOptions
+        self.client._create(
+            LFO, {
+                LFO.project:
+                    self,
+                LFO.labeling_frontend:
+                    labeling_frontend,
+                LFO.customization_options:
+                    json.dumps({
+                        "tools": [],
+                        "classifications": []
+                    })
+            })
+
+        query_str = """mutation ConnectOntologyPyApi($projectId: ID!, $ontologyId: ID!){
+            project(where: {id: $projectId}) {connectOntology(ontologyId: $ontologyId) {id}}}"""
+        self.client.execute(query_str, {
+            'ontologyId': ontology.uid,
+            'projectId': self.uid
+        })
+        timestamp = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
+        self.update(setup_complete=timestamp)
+
     def setup(self, labeling_frontend, labeling_frontend_options):
         """ Finalizes the Project setup.
 
         Args:
             labeling_frontend (LabelingFrontend): Which UI to use to label the
                 data.
             labeling_frontend_options (dict or str): Labeling frontend options,
                 a.k.a. project ontology. If given a `dict` it will be converted
                 to `str` using `json.dumps`.
         """
-        organization = self.client.get_organization()
+
         if not isinstance(labeling_frontend_options, str):
             labeling_frontend_options = json.dumps(labeling_frontend_options)
 
         self.labeling_frontend.connect(labeling_frontend)
 
         LFO = Entity.LabelingFrontendOptions
-        labeling_frontend_options = self.client._create(
+        self.client._create(
             LFO, {
                 LFO.project: self,
                 LFO.labeling_frontend: labeling_frontend,
                 LFO.customization_options: labeling_frontend_options
             })
 
         timestamp = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%M:%SZ")
         self.update(setup_complete=timestamp)
 
+    def queue(self, data_row_ids: List[str]):
+        """Add Data Rows to the Project queue"""
+
+        method = "submitBatchOfDataRows"
+        return self._post_batch(method, data_row_ids)
+
+    def dequeue(self, data_row_ids: List[str]):
+        """Remove Data Rows from the Project queue"""
+
+        method = "removeBatchOfDataRows"
+        return self._post_batch(method, data_row_ids)
+
+    def _post_batch(self, method, data_row_ids: List[str]):
+        """Post batch methods"""
+
+        if self.queue_mode() != QueueMode.Batch:
+            raise ValueError("Project must be in batch mode")
+
+        if len(data_row_ids) > MAX_QUEUE_BATCH_SIZE:
+            raise ValueError(
+                f"Batch exceeds max size of {MAX_QUEUE_BATCH_SIZE}, consider breaking it into parts"
+            )
+
+        query = """mutation %sPyApi($projectId: ID!, $dataRowIds: [ID!]!) {
+              project(where: {id: $projectId}) {
+                %s(data: {dataRowIds: $dataRowIds}) {
+                  dataRows {
+                    dataRowId
+                    error
+                  }
+                }
+              }
+            }
+        """ % (method, method)
+
+        res = self.client.execute(query, {
+            "projectId": self.uid,
+            "dataRowIds": data_row_ids
+        })["project"][method]["dataRows"]
+
+        # TODO: figure out error messaging
+        if len(data_row_ids) == len(res):
+            raise ValueError("No dataRows were submitted successfully")
+
+        if len(data_row_ids) > 0:
+            warnings.warn("Some Data Rows were not submitted successfully")
+
+        return res
+
+    def _update_queue_mode(self, mode: QueueMode) -> QueueMode:
+
+        if self.queue_mode() == mode:
+            return mode
+
+        if mode == QueueMode.Batch:
+            status = "ENABLED"
+        elif mode == QueueMode.Dataset:
+            status = "DISABLED"
+        else:
+            raise ValueError(
+                "Must provide either `BATCH` or `DATASET` as a mode")
+
+        query_str = """mutation %s($projectId: ID!, $status: TagSetStatusInput!) {
+              project(where: {id: $projectId}) {
+                 setTagSetStatus(input: {tagSetStatus: $status}) {
+                    tagSetStatus
+                }
+            }
+        }
+        """ % "setTagSetStatusPyApi"
+
+        self.client.execute(query_str, {
+            'projectId': self.uid,
+            'status': status
+        })
+
+        return mode
+
+    def queue_mode(self):
+
+        query_str = """query %s($projectId: ID!) {
+              project(where: {id: $projectId}) {
+                 tagSetStatus
+            }
+        }
+        """ % "GetTagSetStatusPyApi"
+
+        status = self.client.execute(
+            query_str, {'projectId': self.uid})["project"]["tagSetStatus"]
+
+        if status == "ENABLED":
+            return QueueMode.Batch
+        elif status == "DISABLED":
+            return QueueMode.Dataset
+        else:
+            raise ValueError("Status not known")
+
     def validate_labeling_parameter_overrides(self, data):
         for idx, row in enumerate(data):
             if len(row) != 3:
                 raise TypeError(
                     f"Data must be a list of tuples containing a DataRow, priority (int), num_labels (int). Found {len(row)} items. Index: {idx}"
                 )
             data_row, priority, num_labels = row
```

### Comparing `labelbox-3.8.0/labelbox/schema/review.py` & `labelbox-3.9.0/labelbox/schema/review.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/role.py` & `labelbox-3.9.0/labelbox/schema/role.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/task.py` & `labelbox-3.9.0/labelbox/schema/task.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/user.py` & `labelbox-3.9.0/labelbox/schema/user.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/schema/webhook.py` & `labelbox-3.9.0/labelbox/schema/webhook.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox/utils.py` & `labelbox-3.9.0/labelbox/utils.py`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/labelbox.egg-info/PKG-INFO` & `labelbox-3.9.0/labelbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelbox
-Version: 3.8.0
+Version: 3.9.0
 Summary: Labelbox Python API
 Home-page: https://labelbox.com
 Author: Labelbox
 Author-email: engineering@labelbox.com
 License: UNKNOWN
 Keywords: labelbox
 Platform: UNKNOWN
```

### Comparing `labelbox-3.8.0/labelbox.egg-info/SOURCES.txt` & `labelbox-3.9.0/labelbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labelbox-3.8.0/setup.py` & `labelbox-3.9.0/setup.py`

 * *Files identical despite different names*

