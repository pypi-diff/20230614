# Comparing `tmp/hello2-1.9.2.tar.gz` & `tmp/hello2-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello2-1.9.2.tar", last modified: Thu Jun  8 12:24:13 2023, max compression
+gzip compressed data, was "hello2-1.9.3.tar", last modified: Wed Jun 14 04:15:39 2023, max compression
```

## Comparing `hello2-1.9.2.tar` & `hello2-1.9.3.tar`

### file list

```diff
@@ -1,203 +1,203 @@
--rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-1.9.2/.gitignore
--rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-1.9.2/.readthedocs.yaml
--rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-1.9.2/LICENSE
--rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-1.9.2/README.md
--rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-1.9.2/docs/Makefile
--rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-1.9.2/docs/make.bat
--rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-1.9.2/docs/requirements.txt
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.9.2/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.9.2/docs/source/_templates/.gitkeep
--rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-1.9.2/docs/source/conf.py
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-1.9.2/docs/source/hello.data.coco2yolo.rst
--rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-1.9.2/docs/source/hello.data.rst
--rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-1.9.2/docs/source/hello.experimental.albu.detection.rst
--rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-1.9.2/docs/source/hello.experimental.albu.rst
--rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-1.9.2/docs/source/hello.experimental.rst
--rw-r--r--   0        0        0      157 2023-04-20 14:38:58.196102 hello2-1.9.2/docs/source/hello.fiftyone.annotate.rst
--rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-1.9.2/docs/source/hello.fiftyone.brain.rst
--rw-r--r--   0        0        0      145 2023-05-04 10:28:37.375287 hello2-1.9.2/docs/source/hello.fiftyone.coco.rst
--rw-r--r--   0        0        0      165 2023-05-29 00:31:35.816394 hello2-1.9.2/docs/source/hello.fiftyone.coco_utils.rst
--rw-r--r--   0        0        0      160 2023-04-29 13:47:19.060767 hello2-1.9.2/docs/source/hello.fiftyone.connected.rst
--rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-1.9.2/docs/source/hello.fiftyone.copypaste.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-1.9.2/docs/source/hello.fiftyone.core.rst
--rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-1.9.2/docs/source/hello.fiftyone.dataset.rst
--rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-1.9.2/docs/source/hello.fiftyone.dataset_annotate.rst
--rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-1.9.2/docs/source/hello.fiftyone.dataset_detections.rst
--rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.dataset_segmentations.rst
--rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.dataset_yolov5.rst
--rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.dataset_zoo.rst
--rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.evaluate.rst
--rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.evaluate_detections.rst
--rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.evaluate_segmentations.rst
--rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-1.9.2/docs/source/hello.fiftyone.gen_examples.rst
--rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-1.9.2/docs/source/hello.fiftyone.mask_ignore.rst
--rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-1.9.2/docs/source/hello.fiftyone.miou.rst
--rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-1.9.2/docs/source/hello.fiftyone.patches.rst
--rw-r--r--   0        0        0      905 2023-05-29 00:31:35.816394 hello2-1.9.2/docs/source/hello.fiftyone.rst
--rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-1.9.2/docs/source/hello.fiftyone.tarinfo.rst
--rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-1.9.2/docs/source/hello.fiftyone.unique.rst
--rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-1.9.2/docs/source/hello.fiftyone.utils.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-1.9.2/docs/source/hello.fiftyone.video.rst
--rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-1.9.2/docs/source/hello.fiftyone.view.rst
--rw-r--r--   0        0        0      139 2023-04-29 13:47:19.090767 hello2-1.9.2/docs/source/hello.fvcore.core.rst
--rw-r--r--   0        0        0      234 2023-04-29 13:47:19.090767 hello2-1.9.2/docs/source/hello.fvcore.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-1.9.2/docs/source/hello.io.image.rst
--rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-1.9.2/docs/source/hello.io.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-1.9.2/docs/source/hello.io.utils.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-1.9.2/docs/source/hello.mmdet.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-1.9.2/docs/source/hello.mmdet.flop.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-1.9.2/docs/source/hello.mmdet.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.9.2/docs/source/hello.mmdet.log.rst
--rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-1.9.2/docs/source/hello.mmdet.plot.rst
--rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-1.9.2/docs/source/hello.mmdet.rst
--rw-r--r--   0        0        0      142 2023-05-29 00:31:35.816394 hello2-1.9.2/docs/source/hello.mmlab.mmdet3.rst
--rw-r--r--   0        0        0      139 2023-05-29 00:31:35.816394 hello2-1.9.2/docs/source/hello.mmlab.mmseg.rst
--rw-r--r--   0        0        0      253 2023-05-29 00:31:35.816394 hello2-1.9.2/docs/source/hello.mmlab.rst
--rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-1.9.2/docs/source/hello.mmseg.infer.rst
--rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.9.2/docs/source/hello.mmseg.log.rst
--rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-1.9.2/docs/source/hello.mmseg.lr.rst
--rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-1.9.2/docs/source/hello.mmseg.rst
--rw-r--r--   0        0        0      145 2023-04-20 14:38:58.266102 hello2-1.9.2/docs/source/hello.nanodet.infer.rst
--rw-r--r--   0        0        0      239 2023-04-20 14:38:58.266102 hello2-1.9.2/docs/source/hello.nanodet.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-1.9.2/docs/source/hello.onnx.export.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-1.9.2/docs/source/hello.onnx.infer.rst
--rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-1.9.2/docs/source/hello.onnx.rst
--rw-r--r--   0        0        0      415 2023-05-29 00:31:35.826394 hello2-1.9.2/docs/source/hello.rst
--rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-1.9.2/docs/source/hello.transforms.rst
--rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-1.9.2/docs/source/hello.transforms.transforms.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.9.2/docs/source/hello.utils.colors.rst
--rw-r--r--   0        0        0      145 2023-05-29 00:31:35.826394 hello2-1.9.2/docs/source/hello.utils.compare.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-1.9.2/docs/source/hello.utils.cuda.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-1.9.2/docs/source/hello.utils.importer.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-1.9.2/docs/source/hello.utils.plots.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.9.2/docs/source/hello.utils.points.rst
--rw-r--r--   0        0        0      365 2023-05-29 00:31:35.826394 hello2-1.9.2/docs/source/hello.utils.rst
--rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-1.9.2/docs/source/hello.utils.strtime.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-1.9.2/docs/source/hello.video.align.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.9.2/docs/source/hello.video.clip.rst
--rw-r--r--   0        0        0      145 2023-04-20 14:38:58.306102 hello2-1.9.2/docs/source/hello.video.fisheye.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.9.2/docs/source/hello.video.frames.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.9.2/docs/source/hello.video.info.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.9.2/docs/source/hello.video.resize.rst
--rw-r--r--   0        0        0      425 2023-04-20 14:38:58.296102 hello2-1.9.2/docs/source/hello.video.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-1.9.2/docs/source/hello.video.rtsp.rst
--rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-1.9.2/docs/source/hello.video.rtsp_pull.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.9.2/docs/source/hello.video.split.rst
--rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-1.9.2/docs/source/hello.video.unwarp.rst
--rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.9.2/docs/source/hello.video.utils.rst
--rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-1.9.2/docs/source/hello.x3m.config.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.9.2/docs/source/hello.x3m.preprocess.rst
--rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-1.9.2/docs/source/hello.x3m.rst
--rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.9.2/docs/source/hello.x3m.transforms.rst
--rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-1.9.2/docs/source/index.rst
--rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-1.9.2/docs/source/modules.rst
--rw-r--r--   0        0        0     3270 2023-06-06 04:22:36.459690 hello2-1.9.2/hello/README.md
--rw-r--r--   0        0        0      773 2023-06-08 12:22:26.096863 hello2-1.9.2/hello/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.2/hello/__main__.py
--rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-1.9.2/hello/data/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.2/hello/data/__main__.py
--rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-1.9.2/hello/data/coco2yolo.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.9.2/hello/experimental/__init__.py
--rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.9.2/hello/experimental/albu/__init__.py
--rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-1.9.2/hello/experimental/albu/detection.py
--rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-1.9.2/hello/fiftyone/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.2/hello/fiftyone/__main__.py
--rw-r--r--   0        0        0     4742 2023-05-30 03:46:30.923445 hello2-1.9.2/hello/fiftyone/annotate.py
--rw-r--r--   0        0        0    10588 2023-05-30 15:55:41.469982 hello2-1.9.2/hello/fiftyone/brain.py
--rw-r--r--   0        0        0     8233 2023-05-29 00:31:35.826394 hello2-1.9.2/hello/fiftyone/coco.py
--rw-r--r--   0        0        0     3945 2023-05-29 00:31:35.826394 hello2-1.9.2/hello/fiftyone/coco_utils.py
--rw-r--r--   0        0        0      912 2023-04-25 01:47:26.910695 hello2-1.9.2/hello/fiftyone/connected.py
--rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-1.9.2/hello/fiftyone/copypaste.py
--rw-r--r--   0        0        0    18009 2023-05-24 08:55:42.705839 hello2-1.9.2/hello/fiftyone/core.py
--rw-r--r--   0        0        0    20251 2023-06-01 06:34:06.690322 hello2-1.9.2/hello/fiftyone/dataset.py
--rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-1.9.2/hello/fiftyone/dataset_detections.py
--rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-1.9.2/hello/fiftyone/dataset_segmentations.py
--rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-1.9.2/hello/fiftyone/dataset_yolov5.py
--rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-1.9.2/hello/fiftyone/dataset_zoo.py
--rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-1.9.2/hello/fiftyone/evaluate.py
--rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-1.9.2/hello/fiftyone/evaluate_detections.py
--rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-1.9.2/hello/fiftyone/evaluate_segmentations.py
--rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-1.9.2/hello/fiftyone/examples/README.md
--rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-1.9.2/hello/fiftyone/examples/examples.py
--rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-1.9.2/hello/fiftyone/examples/utils.py
--rw-r--r--   0        0        0     3241 2023-05-19 07:54:24.980385 hello2-1.9.2/hello/fiftyone/gen_examples.py
--rw-r--r--   0        0        0     2328 2023-05-29 00:31:35.826394 hello2-1.9.2/hello/fiftyone/mask_ignore.py
--rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-1.9.2/hello/fiftyone/miou.py
--rw-r--r--   0        0        0      164 2023-06-08 07:23:27.040658 hello2-1.9.2/hello/fiftyone/novabot/README.md
--rw-r--r--   0        0        0     3213 2023-06-08 04:08:44.033126 hello2-1.9.2/hello/fiftyone/novabot/big_test.py
--rw-r--r--   0        0        0      816 2023-06-08 09:32:00.249026 hello2-1.9.2/hello/fiftyone/novabot/cal_data.py
--rw-r--r--   0        0        0     6017 2023-06-08 11:29:17.187533 hello2-1.9.2/hello/fiftyone/novabot/det_annotate.py
--rw-r--r--   0        0        0     4781 2023-06-08 11:29:00.497532 hello2-1.9.2/hello/fiftyone/novabot/det_clear.py
--rw-r--r--   0        0        0     1612 2023-06-08 09:53:10.788756 hello2-1.9.2/hello/fiftyone/novabot/seg_base.py
--rw-r--r--   0        0        0     2011 2023-06-08 10:00:00.688672 hello2-1.9.2/hello/fiftyone/novabot/tag_data.py
--rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-1.9.2/hello/fiftyone/patches.py
--rw-r--r--   0        0        0     9349 2023-06-08 12:22:21.066864 hello2-1.9.2/hello/fiftyone/tarinfo.py
--rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-1.9.2/hello/fiftyone/unique.py
--rw-r--r--   0        0        0     8090 2023-05-29 00:31:35.826394 hello2-1.9.2/hello/fiftyone/utils.py
--rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-1.9.2/hello/fiftyone/video.py
--rw-r--r--   0        0        0    10678 2023-06-05 03:32:36.498706 hello2-1.9.2/hello/fiftyone/view.py
--rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-1.9.2/hello/fvcore/README.md
--rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-1.9.2/hello/fvcore/__init__.py
--rw-r--r--   0        0        0     1080 2023-04-29 13:43:43.400786 hello2-1.9.2/hello/fvcore/core.py
--rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-1.9.2/hello/io/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-1.9.2/hello/io/image.py
--rw-r--r--   0        0        0      989 2023-05-29 00:31:35.826394 hello2-1.9.2/hello/io/utils.py
--rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-1.9.2/hello/mmdet/__init__.py
--rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-1.9.2/hello/mmdet/__main__.py
--rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-1.9.2/hello/mmdet/export.py
--rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-1.9.2/hello/mmdet/flop.py
--rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-1.9.2/hello/mmdet/infer.py
--rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-1.9.2/hello/mmdet/log.py
--rw-r--r--   0        0        0     5976 2023-04-12 11:23:04.178651 hello2-1.9.2/hello/mmdet/plot.py
--rw-r--r--   0        0        0      563 2023-05-12 07:19:19.396722 hello2-1.9.2/hello/mmlab/__init__.py
--rw-r--r--   0        0        0       67 2023-05-12 07:16:55.756771 hello2-1.9.2/hello/mmlab/__main__.py
--rw-r--r--   0        0        0      110 2023-05-12 07:26:47.136571 hello2-1.9.2/hello/mmlab/mmdet3.py
--rw-r--r--   0        0        0     6549 2023-05-15 09:18:13.003946 hello2-1.9.2/hello/mmlab/mmseg.py
--rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-1.9.2/hello/mmseg/__init__.py
--rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-1.9.2/hello/mmseg/__main__.py
--rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-1.9.2/hello/mmseg/infer.py
--rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-1.9.2/hello/mmseg/log.py
--rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-1.9.2/hello/mmseg/lr.py
--rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-1.9.2/hello/nanodet/__init__.py
--rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-1.9.2/hello/nanodet/__main__.py
--rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-1.9.2/hello/nanodet/infer.py
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.9.2/hello/onnx/__init__.py
--rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-1.9.2/hello/onnx/examples/README.md
--rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-1.9.2/hello/onnx/examples/test_sigmoid.py
--rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-1.9.2/hello/onnx/export.py
--rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-1.9.2/hello/onnx/infer.py
--rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-1.9.2/hello/transforms/README.md
--rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.9.2/hello/transforms/__init__.py
--rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-1.9.2/hello/transforms/transforms.py
--rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-1.9.2/hello/utils/__init__.py
--rw-r--r--   0        0        0     2133 2023-05-19 03:21:05.796070 hello2-1.9.2/hello/utils/colors.py
--rw-r--r--   0        0        0     1349 2023-05-29 00:31:35.826394 hello2-1.9.2/hello/utils/compare.py
--rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-1.9.2/hello/utils/cuda.py
--rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-1.9.2/hello/utils/importer.py
--rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-1.9.2/hello/utils/plots.py
--rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-1.9.2/hello/utils/points.py
--rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-1.9.2/hello/utils/strtime.py
--rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-1.9.2/hello/video/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.2/hello/video/__main__.py
--rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-1.9.2/hello/video/align.py
--rw-r--r--   0        0        0     6382 2023-05-17 04:07:48.740198 hello2-1.9.2/hello/video/clip.py
--rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-1.9.2/hello/video/fisheye.py
--rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-1.9.2/hello/video/info.py
--rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-1.9.2/hello/video/resize.py
--rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-1.9.2/hello/video/rtsp.py
--rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-1.9.2/hello/video/rtsp_pull.py
--rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-1.9.2/hello/video/split.py
--rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-1.9.2/hello/video/unwarp.py
--rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-1.9.2/hello/video/utils.py
--rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-1.9.2/hello/x3m/__init__.py
--rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.2/hello/x3m/__main__.py
--rw-r--r--   0        0        0     4846 2023-06-07 01:37:27.153419 hello2-1.9.2/hello/x3m/config.py
--rw-r--r--   0        0        0     5224 2023-06-08 07:56:20.720236 hello2-1.9.2/hello/x3m/nanodet/best_one.py
--rw-r--r--   0        0        0     3280 2023-06-06 08:46:57.526337 hello2-1.9.2/hello/x3m/preprocess.py
--rw-r--r--   0        0        0     6928 2022-06-27 01:46:45.026108 hello2-1.9.2/hello/x3m/transforms.py
--rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-1.9.2/hello_c/CMakeLists.txt
--rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-1.9.2/hello_c/README.md
--rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-1.9.2/hello_c/main.cpp
--rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-1.9.2/hello_c/trace_model.py
--rw-r--r--   0        0        0      787 2023-05-15 09:28:06.783743 hello2-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0      550 2022-11-04 08:45:52.036893 hello2-1.9.3/.gitignore
+-rw-r--r--   0        0        0      715 2022-11-04 17:06:29.116576 hello2-1.9.3/.readthedocs.yaml
+-rw-r--r--   0        0        0    11357 2022-06-27 01:46:45.026108 hello2-1.9.3/LICENSE
+-rw-r--r--   0        0        0      351 2022-12-20 05:58:10.658183 hello2-1.9.3/README.md
+-rw-r--r--   0        0        0      638 2022-11-04 13:36:31.980929 hello2-1.9.3/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-11-04 13:36:31.980929 hello2-1.9.3/docs/make.bat
+-rw-r--r--   0        0        0      163 2022-11-06 11:07:57.505182 hello2-1.9.3/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.9.3/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-06 11:07:57.505182 hello2-1.9.3/docs/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     1365 2022-11-06 12:23:09.043638 hello2-1.9.3/docs/source/conf.py
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.770149 hello2-1.9.3/docs/source/hello.data.coco2yolo.rst
+-rw-r--r--   0        0        0      231 2022-11-04 14:14:10.770149 hello2-1.9.3/docs/source/hello.data.rst
+-rw-r--r--   0        0        0      187 2022-12-14 01:38:29.403883 hello2-1.9.3/docs/source/hello.experimental.albu.detection.rst
+-rw-r--r--   0        0        0      283 2022-12-14 01:38:29.403883 hello2-1.9.3/docs/source/hello.experimental.albu.rst
+-rw-r--r--   0        0        0      260 2022-12-14 01:38:29.393883 hello2-1.9.3/docs/source/hello.experimental.rst
+-rw-r--r--   0        0        0      157 2023-04-20 14:38:58.196102 hello2-1.9.3/docs/source/hello.fiftyone.annotate.rst
+-rw-r--r--   0        0        0      148 2022-12-14 09:04:35.414160 hello2-1.9.3/docs/source/hello.fiftyone.brain.rst
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:37.375287 hello2-1.9.3/docs/source/hello.fiftyone.coco.rst
+-rw-r--r--   0        0        0      165 2023-05-29 00:31:35.816394 hello2-1.9.3/docs/source/hello.fiftyone.coco_utils.rst
+-rw-r--r--   0        0        0      160 2023-04-29 13:47:19.060767 hello2-1.9.3/docs/source/hello.fiftyone.connected.rst
+-rw-r--r--   0        0        0      160 2022-11-18 12:12:27.461051 hello2-1.9.3/docs/source/hello.fiftyone.copypaste.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.780149 hello2-1.9.3/docs/source/hello.fiftyone.core.rst
+-rw-r--r--   0        0        0      154 2022-11-04 14:14:10.780149 hello2-1.9.3/docs/source/hello.fiftyone.dataset.rst
+-rw-r--r--   0        0        0      183 2022-11-04 14:14:10.780149 hello2-1.9.3/docs/source/hello.fiftyone.dataset_annotate.rst
+-rw-r--r--   0        0        0      189 2022-11-04 14:14:10.780149 hello2-1.9.3/docs/source/hello.fiftyone.dataset_detections.rst
+-rw-r--r--   0        0        0      198 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.dataset_segmentations.rst
+-rw-r--r--   0        0        0      177 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.dataset_yolov5.rst
+-rw-r--r--   0        0        0      168 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.dataset_zoo.rst
+-rw-r--r--   0        0        0      157 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.evaluate.rst
+-rw-r--r--   0        0        0      192 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.evaluate_detections.rst
+-rw-r--r--   0        0        0      201 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.evaluate_segmentations.rst
+-rw-r--r--   0        0        0      171 2022-11-18 12:12:27.481051 hello2-1.9.3/docs/source/hello.fiftyone.gen_examples.rst
+-rw-r--r--   0        0        0      168 2022-11-18 12:12:27.481051 hello2-1.9.3/docs/source/hello.fiftyone.mask_ignore.rst
+-rw-r--r--   0        0        0      145 2022-11-04 14:14:10.790149 hello2-1.9.3/docs/source/hello.fiftyone.miou.rst
+-rw-r--r--   0        0        0      154 2022-11-18 12:12:27.481051 hello2-1.9.3/docs/source/hello.fiftyone.patches.rst
+-rw-r--r--   0        0        0      905 2023-05-29 00:31:35.816394 hello2-1.9.3/docs/source/hello.fiftyone.rst
+-rw-r--r--   0        0        0      154 2022-12-16 13:39:47.530383 hello2-1.9.3/docs/source/hello.fiftyone.tarinfo.rst
+-rw-r--r--   0        0        0      151 2022-11-04 14:14:10.800149 hello2-1.9.3/docs/source/hello.fiftyone.unique.rst
+-rw-r--r--   0        0        0      148 2022-11-22 16:10:13.239568 hello2-1.9.3/docs/source/hello.fiftyone.utils.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.800149 hello2-1.9.3/docs/source/hello.fiftyone.video.rst
+-rw-r--r--   0        0        0      145 2022-11-22 16:10:13.239568 hello2-1.9.3/docs/source/hello.fiftyone.view.rst
+-rw-r--r--   0        0        0      139 2023-04-29 13:47:19.090767 hello2-1.9.3/docs/source/hello.fvcore.core.rst
+-rw-r--r--   0        0        0      234 2023-04-29 13:47:19.090767 hello2-1.9.3/docs/source/hello.fvcore.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.800149 hello2-1.9.3/docs/source/hello.io.image.rst
+-rw-r--r--   0        0        0      237 2022-11-04 14:14:10.800149 hello2-1.9.3/docs/source/hello.io.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.810149 hello2-1.9.3/docs/source/hello.io.utils.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.810149 hello2-1.9.3/docs/source/hello.mmdet.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.810149 hello2-1.9.3/docs/source/hello.mmdet.flop.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.820149 hello2-1.9.3/docs/source/hello.mmdet.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.9.3/docs/source/hello.mmdet.log.rst
+-rw-r--r--   0        0        0      136 2022-11-25 07:45:47.915124 hello2-1.9.3/docs/source/hello.mmdet.plot.rst
+-rw-r--r--   0        0        0      312 2022-11-25 07:45:47.915124 hello2-1.9.3/docs/source/hello.mmdet.rst
+-rw-r--r--   0        0        0      142 2023-05-29 00:31:35.816394 hello2-1.9.3/docs/source/hello.mmlab.mmdet3.rst
+-rw-r--r--   0        0        0      139 2023-05-29 00:31:35.816394 hello2-1.9.3/docs/source/hello.mmlab.mmseg.rst
+-rw-r--r--   0        0        0      253 2023-05-29 00:31:35.816394 hello2-1.9.3/docs/source/hello.mmlab.rst
+-rw-r--r--   0        0        0      139 2022-11-07 02:04:44.756679 hello2-1.9.3/docs/source/hello.mmseg.infer.rst
+-rw-r--r--   0        0        0      133 2022-11-04 14:14:10.820149 hello2-1.9.3/docs/source/hello.mmseg.log.rst
+-rw-r--r--   0        0        0      130 2022-11-04 14:14:10.820149 hello2-1.9.3/docs/source/hello.mmseg.lr.rst
+-rw-r--r--   0        0        0      268 2022-11-07 02:04:44.756679 hello2-1.9.3/docs/source/hello.mmseg.rst
+-rw-r--r--   0        0        0      145 2023-04-20 14:38:58.266102 hello2-1.9.3/docs/source/hello.nanodet.infer.rst
+-rw-r--r--   0        0        0      239 2023-04-20 14:38:58.266102 hello2-1.9.3/docs/source/hello.nanodet.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.830149 hello2-1.9.3/docs/source/hello.onnx.export.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.830149 hello2-1.9.3/docs/source/hello.onnx.infer.rst
+-rw-r--r--   0        0        0      248 2022-11-04 14:14:10.830149 hello2-1.9.3/docs/source/hello.onnx.rst
+-rw-r--r--   0        0        0      415 2023-05-29 00:31:35.826394 hello2-1.9.3/docs/source/hello.rst
+-rw-r--r--   0        0        0      256 2022-11-04 14:14:10.840149 hello2-1.9.3/docs/source/hello.transforms.rst
+-rw-r--r--   0        0        0      169 2022-11-04 14:14:10.840149 hello2-1.9.3/docs/source/hello.transforms.transforms.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.9.3/docs/source/hello.utils.colors.rst
+-rw-r--r--   0        0        0      145 2023-05-29 00:31:35.826394 hello2-1.9.3/docs/source/hello.utils.compare.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.850149 hello2-1.9.3/docs/source/hello.utils.cuda.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.850149 hello2-1.9.3/docs/source/hello.utils.importer.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.850149 hello2-1.9.3/docs/source/hello.utils.plots.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.850149 hello2-1.9.3/docs/source/hello.utils.points.rst
+-rw-r--r--   0        0        0      365 2023-05-29 00:31:35.826394 hello2-1.9.3/docs/source/hello.utils.rst
+-rw-r--r--   0        0        0      145 2022-11-30 10:15:09.976399 hello2-1.9.3/docs/source/hello.utils.strtime.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.860149 hello2-1.9.3/docs/source/hello.video.align.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.9.3/docs/source/hello.video.clip.rst
+-rw-r--r--   0        0        0      145 2023-04-20 14:38:58.306102 hello2-1.9.3/docs/source/hello.video.fisheye.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.9.3/docs/source/hello.video.frames.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.860149 hello2-1.9.3/docs/source/hello.video.info.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.860149 hello2-1.9.3/docs/source/hello.video.resize.rst
+-rw-r--r--   0        0        0      425 2023-04-20 14:38:58.296102 hello2-1.9.3/docs/source/hello.video.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.870149 hello2-1.9.3/docs/source/hello.video.rtsp.rst
+-rw-r--r--   0        0        0      153 2022-11-29 06:30:33.931961 hello2-1.9.3/docs/source/hello.video.rtsp_pull.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.9.3/docs/source/hello.video.split.rst
+-rw-r--r--   0        0        0      142 2022-11-04 14:14:10.870149 hello2-1.9.3/docs/source/hello.video.unwarp.rst
+-rw-r--r--   0        0        0      139 2022-11-04 14:14:10.870149 hello2-1.9.3/docs/source/hello.video.utils.rst
+-rw-r--r--   0        0        0      136 2022-11-04 14:14:10.880149 hello2-1.9.3/docs/source/hello.x3m.config.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.9.3/docs/source/hello.x3m.preprocess.rst
+-rw-r--r--   0        0        0      272 2022-11-04 14:14:10.870149 hello2-1.9.3/docs/source/hello.x3m.rst
+-rw-r--r--   0        0        0      148 2022-11-04 14:14:10.880149 hello2-1.9.3/docs/source/hello.x3m.transforms.rst
+-rw-r--r--   0        0        0      572 2022-11-04 15:19:50.508765 hello2-1.9.3/docs/source/index.rst
+-rw-r--r--   0        0        0       52 2022-11-04 14:40:30.829573 hello2-1.9.3/docs/source/modules.rst
+-rw-r--r--   0        0        0     3270 2023-06-06 04:22:36.459690 hello2-1.9.3/hello/README.md
+-rw-r--r--   0        0        0      773 2023-06-14 04:12:49.144947 hello2-1.9.3/hello/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.3/hello/__main__.py
+-rw-r--r--   0        0        0      471 2022-11-06 13:38:11.482015 hello2-1.9.3/hello/data/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.3/hello/data/__main__.py
+-rw-r--r--   0        0        0     3426 2022-08-30 01:19:13.615222 hello2-1.9.3/hello/data/coco2yolo.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.9.3/hello/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-11 06:23:09.504528 hello2-1.9.3/hello/experimental/albu/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-11 06:23:09.504528 hello2-1.9.3/hello/experimental/albu/detection.py
+-rw-r--r--   0        0        0     1047 2022-11-06 13:38:17.442013 hello2-1.9.3/hello/fiftyone/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.3/hello/fiftyone/__main__.py
+-rw-r--r--   0        0        0     4742 2023-05-30 03:46:30.923445 hello2-1.9.3/hello/fiftyone/annotate.py
+-rw-r--r--   0        0        0    10588 2023-05-30 15:55:41.469982 hello2-1.9.3/hello/fiftyone/brain.py
+-rw-r--r--   0        0        0     8233 2023-05-29 00:31:35.826394 hello2-1.9.3/hello/fiftyone/coco.py
+-rw-r--r--   0        0        0     3945 2023-05-29 00:31:35.826394 hello2-1.9.3/hello/fiftyone/coco_utils.py
+-rw-r--r--   0        0        0      912 2023-04-25 01:47:26.910695 hello2-1.9.3/hello/fiftyone/connected.py
+-rw-r--r--   0        0        0       36 2022-11-18 04:25:30.455378 hello2-1.9.3/hello/fiftyone/copypaste.py
+-rw-r--r--   0        0        0    18009 2023-05-24 08:55:42.705839 hello2-1.9.3/hello/fiftyone/core.py
+-rw-r--r--   0        0        0    20251 2023-06-01 06:34:06.690322 hello2-1.9.3/hello/fiftyone/dataset.py
+-rw-r--r--   0        0        0     7502 2022-12-30 03:41:16.092249 hello2-1.9.3/hello/fiftyone/dataset_detections.py
+-rw-r--r--   0        0        0     5693 2022-12-30 03:45:01.362177 hello2-1.9.3/hello/fiftyone/dataset_segmentations.py
+-rw-r--r--   0        0        0     1402 2022-11-30 01:50:37.091070 hello2-1.9.3/hello/fiftyone/dataset_yolov5.py
+-rw-r--r--   0        0        0      889 2022-12-02 08:54:06.970245 hello2-1.9.3/hello/fiftyone/dataset_zoo.py
+-rw-r--r--   0        0        0     1169 2022-07-18 00:56:40.761934 hello2-1.9.3/hello/fiftyone/evaluate.py
+-rw-r--r--   0        0        0     5157 2023-03-07 04:04:15.369663 hello2-1.9.3/hello/fiftyone/evaluate_detections.py
+-rw-r--r--   0        0        0     4544 2023-03-07 04:04:11.609664 hello2-1.9.3/hello/fiftyone/evaluate_segmentations.py
+-rw-r--r--   0        0        0      103 2022-09-19 06:15:49.337504 hello2-1.9.3/hello/fiftyone/examples/README.md
+-rw-r--r--   0        0        0     2975 2022-11-30 01:46:25.831120 hello2-1.9.3/hello/fiftyone/examples/examples.py
+-rw-r--r--   0        0        0    12021 2023-01-09 09:33:51.046594 hello2-1.9.3/hello/fiftyone/examples/utils.py
+-rw-r--r--   0        0        0     3241 2023-05-19 07:54:24.980385 hello2-1.9.3/hello/fiftyone/gen_examples.py
+-rw-r--r--   0        0        0     2328 2023-05-29 00:31:35.826394 hello2-1.9.3/hello/fiftyone/mask_ignore.py
+-rw-r--r--   0        0        0     5683 2022-12-30 03:42:18.702230 hello2-1.9.3/hello/fiftyone/miou.py
+-rw-r--r--   0        0        0      164 2023-06-08 07:23:27.040658 hello2-1.9.3/hello/fiftyone/novabot/README.md
+-rw-r--r--   0        0        0     3835 2023-06-12 07:16:30.068768 hello2-1.9.3/hello/fiftyone/novabot/big_test.py
+-rw-r--r--   0        0        0      952 2023-06-14 03:36:33.145883 hello2-1.9.3/hello/fiftyone/novabot/cal_data.py
+-rw-r--r--   0        0        0     6250 2023-06-14 04:03:54.435176 hello2-1.9.3/hello/fiftyone/novabot/det_annotate.py
+-rw-r--r--   0        0        0     5309 2023-06-14 04:11:05.194991 hello2-1.9.3/hello/fiftyone/novabot/det_big_train.py
+-rw-r--r--   0        0        0     1669 2023-06-14 03:43:11.095705 hello2-1.9.3/hello/fiftyone/novabot/seg_base.py
+-rw-r--r--   0        0        0     2014 2023-06-14 03:46:04.785634 hello2-1.9.3/hello/fiftyone/novabot/tag_data.py
+-rw-r--r--   0        0        0     2639 2022-11-18 06:29:39.594231 hello2-1.9.3/hello/fiftyone/patches.py
+-rw-r--r--   0        0        0     9349 2023-06-08 12:22:21.066864 hello2-1.9.3/hello/fiftyone/tarinfo.py
+-rw-r--r--   0        0        0     4094 2023-03-15 08:42:32.674825 hello2-1.9.3/hello/fiftyone/unique.py
+-rw-r--r--   0        0        0     8090 2023-05-29 00:31:35.826394 hello2-1.9.3/hello/fiftyone/utils.py
+-rw-r--r--   0        0        0      781 2022-12-01 14:14:43.560707 hello2-1.9.3/hello/fiftyone/video.py
+-rw-r--r--   0        0        0    10678 2023-06-05 03:32:36.498706 hello2-1.9.3/hello/fiftyone/view.py
+-rw-r--r--   0        0        0      435 2022-10-20 14:18:34.575285 hello2-1.9.3/hello/fvcore/README.md
+-rw-r--r--   0        0        0        0 2022-11-04 14:49:06.729395 hello2-1.9.3/hello/fvcore/__init__.py
+-rw-r--r--   0        0        0     1080 2023-04-29 13:43:43.400786 hello2-1.9.3/hello/fvcore/core.py
+-rw-r--r--   0        0        0      135 2022-06-27 01:46:45.026108 hello2-1.9.3/hello/io/__init__.py
+-rw-r--r--   0        0        0     1382 2022-08-23 09:20:12.751790 hello2-1.9.3/hello/io/image.py
+-rw-r--r--   0        0        0      989 2023-05-29 00:31:35.826394 hello2-1.9.3/hello/io/utils.py
+-rw-r--r--   0        0        0      851 2022-11-25 07:46:45.875120 hello2-1.9.3/hello/mmdet/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-17 07:49:46.479528 hello2-1.9.3/hello/mmdet/__main__.py
+-rw-r--r--   0        0        0       97 2022-10-17 08:00:01.479443 hello2-1.9.3/hello/mmdet/export.py
+-rw-r--r--   0        0        0     1736 2022-10-20 16:17:29.762828 hello2-1.9.3/hello/mmdet/flop.py
+-rw-r--r--   0        0        0     5446 2023-03-03 15:16:46.611009 hello2-1.9.3/hello/mmdet/infer.py
+-rw-r--r--   0        0        0     3273 2023-04-11 07:00:00.274582 hello2-1.9.3/hello/mmdet/log.py
+-rw-r--r--   0        0        0     5976 2023-04-12 11:23:04.178651 hello2-1.9.3/hello/mmdet/plot.py
+-rw-r--r--   0        0        0      563 2023-05-12 07:19:19.396722 hello2-1.9.3/hello/mmlab/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-12 07:16:55.756771 hello2-1.9.3/hello/mmlab/__main__.py
+-rw-r--r--   0        0        0      110 2023-05-12 07:26:47.136571 hello2-1.9.3/hello/mmlab/mmdet3.py
+-rw-r--r--   0        0        0     6549 2023-05-15 09:18:13.003946 hello2-1.9.3/hello/mmlab/mmseg.py
+-rw-r--r--   0        0        0      645 2022-11-07 02:04:01.296693 hello2-1.9.3/hello/mmseg/__init__.py
+-rw-r--r--   0        0        0       67 2022-10-31 01:39:47.674470 hello2-1.9.3/hello/mmseg/__main__.py
+-rw-r--r--   0        0        0     6040 2022-11-09 01:29:31.447414 hello2-1.9.3/hello/mmseg/infer.py
+-rw-r--r--   0        0        0     2368 2023-04-11 07:03:55.124501 hello2-1.9.3/hello/mmseg/log.py
+-rw-r--r--   0        0        0     7006 2022-12-01 12:09:30.751861 hello2-1.9.3/hello/mmseg/lr.py
+-rw-r--r--   0        0        0      462 2023-03-29 08:04:38.934968 hello2-1.9.3/hello/nanodet/__init__.py
+-rw-r--r--   0        0        0       67 2023-03-29 08:03:09.784974 hello2-1.9.3/hello/nanodet/__main__.py
+-rw-r--r--   0        0        0     7410 2023-04-06 10:19:32.462564 hello2-1.9.3/hello/nanodet/infer.py
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.9.3/hello/onnx/__init__.py
+-rw-r--r--   0        0        0      213 2022-06-27 02:15:25.376085 hello2-1.9.3/hello/onnx/examples/README.md
+-rw-r--r--   0        0        0     1879 2022-06-27 01:46:45.026108 hello2-1.9.3/hello/onnx/examples/test_sigmoid.py
+-rw-r--r--   0        0        0     3024 2022-08-30 07:45:32.884923 hello2-1.9.3/hello/onnx/export.py
+-rw-r--r--   0        0        0     1707 2022-08-22 07:09:07.802604 hello2-1.9.3/hello/onnx/infer.py
+-rw-r--r--   0        0        0     1334 2022-11-21 14:14:37.239473 hello2-1.9.3/hello/transforms/README.md
+-rw-r--r--   0        0        0        0 2022-06-27 01:46:45.026108 hello2-1.9.3/hello/transforms/__init__.py
+-rw-r--r--   0        0        0     2655 2022-11-21 15:01:54.364062 hello2-1.9.3/hello/transforms/transforms.py
+-rw-r--r--   0        0        0        0 2022-07-20 06:21:09.967902 hello2-1.9.3/hello/utils/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-19 03:21:05.796070 hello2-1.9.3/hello/utils/colors.py
+-rw-r--r--   0        0        0     1349 2023-05-29 00:31:35.826394 hello2-1.9.3/hello/utils/compare.py
+-rw-r--r--   0        0        0     1815 2022-10-14 02:36:42.461531 hello2-1.9.3/hello/utils/cuda.py
+-rw-r--r--   0        0        0      356 2022-07-20 06:43:22.727885 hello2-1.9.3/hello/utils/importer.py
+-rw-r--r--   0        0        0      612 2022-08-23 06:44:50.231910 hello2-1.9.3/hello/utils/plots.py
+-rw-r--r--   0        0        0     2999 2022-11-06 13:40:43.281966 hello2-1.9.3/hello/utils/points.py
+-rw-r--r--   0        0        0      195 2022-11-30 01:25:21.821313 hello2-1.9.3/hello/utils/strtime.py
+-rw-r--r--   0        0        0     1135 2023-02-20 08:24:47.078416 hello2-1.9.3/hello/video/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.3/hello/video/__main__.py
+-rw-r--r--   0        0        0     3428 2022-11-06 13:15:37.862480 hello2-1.9.3/hello/video/align.py
+-rw-r--r--   0        0        0     6382 2023-05-17 04:07:48.740198 hello2-1.9.3/hello/video/clip.py
+-rw-r--r--   0        0        0     3290 2023-02-20 09:35:59.918194 hello2-1.9.3/hello/video/fisheye.py
+-rw-r--r--   0        0        0     1565 2022-11-06 13:15:49.722478 hello2-1.9.3/hello/video/info.py
+-rw-r--r--   0        0        0     3502 2022-11-06 13:15:55.532477 hello2-1.9.3/hello/video/resize.py
+-rw-r--r--   0        0        0     4716 2022-11-29 07:15:17.421543 hello2-1.9.3/hello/video/rtsp.py
+-rw-r--r--   0        0        0     5006 2022-11-29 08:00:32.141119 hello2-1.9.3/hello/video/rtsp_pull.py
+-rw-r--r--   0        0        0     3048 2022-11-11 09:35:15.036742 hello2-1.9.3/hello/video/split.py
+-rw-r--r--   0        0        0     4066 2023-02-20 08:27:40.638408 hello2-1.9.3/hello/video/unwarp.py
+-rw-r--r--   0        0        0      968 2022-08-25 04:09:32.554890 hello2-1.9.3/hello/video/utils.py
+-rw-r--r--   0        0        0      576 2022-11-06 13:41:08.801958 hello2-1.9.3/hello/x3m/__init__.py
+-rw-r--r--   0        0        0       67 2022-09-19 06:15:49.337504 hello2-1.9.3/hello/x3m/__main__.py
+-rw-r--r--   0        0        0     4846 2023-06-07 01:37:27.153419 hello2-1.9.3/hello/x3m/config.py
+-rw-r--r--   0        0        0     5224 2023-06-08 07:56:20.720236 hello2-1.9.3/hello/x3m/nanodet/best_one.py
+-rw-r--r--   0        0        0     3280 2023-06-06 08:46:57.526337 hello2-1.9.3/hello/x3m/preprocess.py
+-rw-r--r--   0        0        0     6928 2022-06-27 01:46:45.026108 hello2-1.9.3/hello/x3m/transforms.py
+-rw-r--r--   0        0        0      808 2022-06-27 01:46:45.026108 hello2-1.9.3/hello_c/CMakeLists.txt
+-rw-r--r--   0        0        0      776 2022-06-27 01:46:45.026108 hello2-1.9.3/hello_c/README.md
+-rw-r--r--   0        0        0     1375 2022-06-27 01:46:45.026108 hello2-1.9.3/hello_c/main.cpp
+-rw-r--r--   0        0        0      262 2022-06-27 01:46:45.026108 hello2-1.9.3/hello_c/trace_model.py
+-rw-r--r--   0        0        0      787 2023-05-15 09:28:06.783743 hello2-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-1.9.3/PKG-INFO
```

### Comparing `hello2-1.9.2/.gitignore` & `hello2-1.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/.readthedocs.yaml` & `hello2-1.9.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/LICENSE` & `hello2-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/docs/Makefile` & `hello2-1.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/docs/make.bat` & `hello2-1.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/docs/source/conf.py` & `hello2-1.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/docs/source/hello.fiftyone.rst` & `hello2-1.9.3/docs/source/hello.fiftyone.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/docs/source/index.rst` & `hello2-1.9.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/README.md` & `hello2-1.9.3/hello/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/__init__.py` & `hello2-1.9.3/hello/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 
 help_doc_str = """\
 usage: hello [--version] [--help]
 
 shell command:
     hello -h
     hello-data -h
```

### Comparing `hello2-1.9.2/hello/data/coco2yolo.py` & `hello2-1.9.3/hello/data/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/__init__.py` & `hello2-1.9.3/hello/fiftyone/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/annotate.py` & `hello2-1.9.3/hello/fiftyone/annotate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/brain.py` & `hello2-1.9.3/hello/fiftyone/brain.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/coco.py` & `hello2-1.9.3/hello/fiftyone/coco.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/coco_utils.py` & `hello2-1.9.3/hello/fiftyone/coco_utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/connected.py` & `hello2-1.9.3/hello/fiftyone/connected.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/core.py` & `hello2-1.9.3/hello/fiftyone/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/dataset.py` & `hello2-1.9.3/hello/fiftyone/dataset.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/dataset_detections.py` & `hello2-1.9.3/hello/fiftyone/dataset_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/dataset_segmentations.py` & `hello2-1.9.3/hello/fiftyone/dataset_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/dataset_yolov5.py` & `hello2-1.9.3/hello/fiftyone/dataset_yolov5.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/dataset_zoo.py` & `hello2-1.9.3/hello/fiftyone/dataset_zoo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/evaluate.py` & `hello2-1.9.3/hello/fiftyone/evaluate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/evaluate_detections.py` & `hello2-1.9.3/hello/fiftyone/evaluate_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/evaluate_segmentations.py` & `hello2-1.9.3/hello/fiftyone/evaluate_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/examples/examples.py` & `hello2-1.9.3/hello/fiftyone/examples/examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/examples/utils.py` & `hello2-1.9.3/hello/fiftyone/examples/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/gen_examples.py` & `hello2-1.9.3/hello/fiftyone/gen_examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/mask_ignore.py` & `hello2-1.9.3/hello/fiftyone/mask_ignore.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/miou.py` & `hello2-1.9.3/hello/fiftyone/miou.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/novabot/big_test.py` & `hello2-1.9.3/hello/fiftyone/novabot/big_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import hello.fiftyone.dataset as hod
 import hello.fiftyone.tarinfo as hot
 import hello.fiftyone.view as hov
 
 print(hello.__version__)
 
 
-def get_images(root, files, out_dir):
+def get_images(root, files, out_dir, exclude_names, include_names):
     sub_dirs = []
 
     if root is not None:
         root = Path(root) if isinstance(root, str) else root
         files = [str(root / f) for f in files]
 
     out_dir = Path(out_dir)
     for i, f in enumerate(files, 1):
-        sub_dir = hot.extract_images(out_dir / f"patch{i:02d}", [f])
+        kwargs = dict(data_path="data", exclude_names=exclude_names, include_names=include_names)
+        sub_dir = hot.extract_images(out_dir / f"patch{i:02d}", [f], **kwargs)
         sub_dirs.append((sub_dir, Path(f).stem))
 
     return sub_dirs
 
 
 def get_dataset(dataset_name, dataset_type, version, classes, mask_targets, sub_dirs):
     hod.delete_datasets([dataset_name], non_persistent=False)
@@ -66,15 +67,21 @@
 
     root = Path("/workspace/data/tarfiles/novabot_front/img_data")
     files = [
         "novabot_front_img_20230516_us_fawndr_ver002.tar",
         "novabot_front_img_20230501_big_test_ver001.tar",
     ]
 
-    sub_dirs = get_images(root, files, f"tmp/{dataset_name}")
+    # {exclude/include}_names: None or json file path or dict or list
+    # for big train dataset, e.g.
+    # exclude_names = hot.get_image_names(tar_file_path)
+    exclude_names = None
+    include_names = None
+
+    sub_dirs = get_images(root, files, f"tmp/{dataset_name}", exclude_names, include_names)
     dataset, counts = get_dataset(dataset_name, dataset_type, version, classes, mask_targets, sub_dirs)
 
     hod.export_image_dataset(f"exports/{dataset_name}", dataset, splits=None)
 
 
 def test_uniqueness():
     dataset_name = "novabot_front_det_20230525_zhengshu_batch02_object9_ver001"
@@ -85,12 +92,18 @@
 
     root = Path("/workspace/data/tarfiles/novabot_front/img_data")
     files = [
         "novabot_front_img_20230525_us_afternoon_ver001.tar",
         "novabot_front_img_20230525_us_evening_ver001.tar",
     ]
 
-    sub_dirs = get_images(root, files, f"tmp/{dataset_name}")
+    # {exclude/include}_names: None or json file path or dict or list
+    # for big train dataset, e.g.
+    # exclude_names = hot.get_image_names(tar_file_path)
+    exclude_names = None
+    include_names = None
+
+    sub_dirs = get_images(root, files, f"tmp/{dataset_name}", exclude_names, include_names)
     dataset, counts = get_dataset(dataset_name, dataset_type, version, classes, mask_targets, sub_dirs)
 
     view, unique_tag = get_uniqueness(dataset, counts, [500] * len(files))
     hod.export_image_dataset(f"exports/{dataset_name}", view, splits=[unique_tag])
```

### Comparing `hello2-1.9.2/hello/fiftyone/novabot/cal_data.py` & `hello2-1.9.3/hello/fiftyone/novabot/cal_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # %%
 import hello
 import hello.fiftyone.dataset as hod
+import hello.fiftyone.tarinfo as hot
 import hello.fiftyone.view as hov
 
 print(hello.__version__)
 
 # %%
 dataset_name = "novabot_front_cal_20230606_charging_station_ver001"
 dataset_type = "unknown"
 version = "001"
 classes = ["ok", "ng"]
 mask_targets = {}
 
 hod.delete_datasets([dataset_name], non_persistent=False)
 dataset = hod.create_dataset(dataset_name, dataset_type, version, classes, mask_targets)
 
-from_dir = "/workspace/users/hejian/tmp/novabot_front_img_20230404_big_test_ver001/train"
+tar_files = [
+    "/workspace/users/hejian/tmp/novabot_front_det_20230404_big_train_object9_ver001.tar",
+]
+from_dir = hot.extract_images(f"tmp/{dataset_name}", tar_files, data_path="data")
 hod.add_images_dir(dataset, f"{from_dir}/data", "cal")
 
 print("count-images:", dataset.count("filepath"))
 
 # %%
-view = hov.uniqueness(dataset, 200, model="clip-vit-base32-torch")
+view = hov.uniqueness(dataset, 100, model="clip-vit-base32-torch")
 
 print("count-images:", view.count("filepath"))
 
 # %%
 hod.export_image_dataset(f"exports/{dataset_name}", view, splits="auto")
```

### Comparing `hello2-1.9.2/hello/fiftyone/novabot/det_annotate.py` & `hello2-1.9.3/hello/fiftyone/novabot/det_annotate.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 hod.delete_datasets([dataset_name], non_persistent=False)
 dataset = hod.create_dataset(dataset_name, dataset_type, version, classes, mask_targets)
 
 # %%
 label_classes = dataset.default_classes
 
 from_dir = "/workspace/users/hejian/todo/novabot_front_det_20230314_zhengshu_batch01_object9_ver004/train"
-hod.add_images_dir(dataset, f"{from_dir}/data", None)
+hod.add_images_dir(dataset, f"{from_dir}/data", "train")
 
 from_dir = "/workspace/users/hejian/todo/novabot_front_det_20230314_zhengshu_batch01_object9_ver004/train"
 hod.add_detection_labels(dataset, "ground_truth", f"{from_dir}/labels.json", label_classes, mode="coco")
 
 ret = hoc.count_values(dataset, "ground_truth.detections.label")
 print("count-images:", dataset.count("filepath"))
 
@@ -56,15 +56,15 @@
 print("count-images:", dataset.count("filepath"))
 
 # %%
 dataset.default_classes = dataset.default_classes[:-1]
 print(f"{dataset.default_classes=}\n{dataset.default_mask_targets=}")
 
 # %%
-hod.delete_duplicate_labels(dataset, "ground_truth", iou_thresh=0.95, method="simple", iscrowd=None, classwise=False)
+hod.delete_duplicate_labels(dataset, "ground_truth", iou_thresh=0.99, method="simple", iscrowd=None, classwise=False)
 print("count-labels:", dataset.count("ground_truth.detections"))
 
 # %% [markdown]
 # ---
 # start
 
 # %%
@@ -81,15 +81,15 @@
 
 # %%
 bbox_area = (
     F("$metadata.width") * F("bounding_box")[2] *
     F("$metadata.height") * F("bounding_box")[3]
 )
 view = dataset.filter_labels(
-    "ground_truth", (1000 <= bbox_area), only_matches=False
+    "ground_truth", (512 <= bbox_area), only_matches=False
 )
 
 print("count-labels:", view.count("ground_truth.detections"))
 
 # %%
 dataset = view.clone()
 dataset.name
@@ -121,31 +121,39 @@
 results = dataset.evaluate_detections(
     "ground_truth",
     gt_field="ground_truth_iter",
     eval_key="eval",
 )
 
 # %%
+dataset.untag_samples("ng")
 view = dataset.match((F("eval_fp") > 0) | (F("eval_fn") > 0))
 print("length:", view.count("filepath"))
 
-view.tag_samples("issue")
 view.untag_samples("train")
+view.tag_samples("issue")
 
 view = view.filter_labels(
     "ground_truth_iter", F("eval") != "tp", only_matches=False
 ).filter_labels(
     "ground_truth", F("eval") != "tp", only_matches=False
 ).match(
     (F("ground_truth_iter.detections").length() > 0) | (F("ground_truth.detections").length() > 0)
 )
 print("count-labels-old:", view.count("ground_truth_iter.detections"))
 print("count-labels-new:", view.count("ground_truth.detections"))
 
-session = fo.launch_app(view, port=20002, address="192.168.0.119", auto=False)  # tag sample for `issue`
+session = fo.launch_app(view, port=20002, address="192.168.0.119", auto=False)  # tag sample for `ng`
+
+# %%
+view.untag_samples("issue")
+view.tag_samples("train")
+
+view.match_tags("ng").untag_samples("train")
+view.match_tags("ng").tag_samples("issue")
 
 # %%
 view = dataset.match_tags("issue")
 
 hoa.to_cvat(
     "novabot_front_det_20230314_iter2", view,
     label_field="ground_truth",
@@ -163,35 +171,37 @@
     cleanup=False,
     url="http://192.168.0.119:8080",
     username="hejian", password="LFIcvat123")
 ret = hoc.count_values(dataset, "ground_truth.detections.label")
 print("count-images:", dataset.count("filepath"))
 
 # %%
+dataset.untag_samples("ok")
 view = dataset.match_tags("issue")
 session = fo.launch_app(view, port=20003, address="192.168.0.119", auto=False)  # tag sample for `ok`
 
 # %%
 dataset.match_tags("ok").untag_samples("issue")
 dataset.match_tags("ok").tag_samples("train")
 ret = hoc.count_values(dataset, "tags")
 
 # %%
+dataset.untag_samples("ng")
 view = dataset.match_tags("train")
-session = fo.launch_app(view, port=20004, address="192.168.0.119", auto=False)  # tag sample for `drop`
+session = fo.launch_app(view, port=20004, address="192.168.0.119", auto=False)  # tag sample for `ng`
 
 # %%
-dataset.match_tags("drop").untag_samples("train")
-dataset.match_tags("drop").tag_samples("issue")
+dataset.match_tags("ng").untag_samples("train")
+dataset.match_tags("ng").tag_samples("issue")
 ret = hoc.count_values(dataset, "tags")
 
 # %% [markdown]
 # end
 #
 # ---
 
 # %%
-hoco.coco_export(f"exports/{dataset_name}", dataset, label_field="ground_truth", splits=["train", "issue"])
+hoco.coco_export(f"exports/{dataset_name}", dataset, label_field="ground_truth", splits=["train", "val", "issue"])
 
 # %%
 hoc.random_split(dataset.match_tags("train"), splits={"val": 0.1, "train": 0.9}, seed=51)
 hoco.coco_export(f"exports/{dataset_name}", dataset, label_field="ground_truth", splits=["train", "val", "issue"])
```

### Comparing `hello2-1.9.2/hello/fiftyone/novabot/det_clear.py` & `hello2-1.9.3/hello/fiftyone/novabot/det_big_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 import hello.fiftyone.coco as hoco
 import hello.fiftyone.core as hoc
 import hello.fiftyone.dataset as hod
 
 print(hello.__version__)
 
 # %%
-dataset_name = "novabot_front_det_20230531_big_train_object9_ver001b"
+dataset_name = "novabot_front_det_20230531_big_train_object9_ver003b"
 dataset_type = "detection"
 version = "object9"
 classes = ["person", "animal", "shoes", "wheel", "other obstacle", "obstacle", "leaf debris", "faeces", "rock", "charging station", "background"]
 mask_targets = {}
 
 hod.delete_datasets([dataset_name], non_persistent=False)
 dataset = hod.create_dataset(dataset_name, dataset_type, version, classes, mask_targets)
 
 # %%
 label_classes = dataset.default_classes
 
-from_dir = "/workspace/users/hejian/tmp/novabot_front_det_20230314_zhengshu_batch01_object9_ver005/ok"
-hod.add_images_dir(dataset, f"{from_dir}/data", None)
+from_dir = "/workspace/users/hejian/tmp/novabot_front_det_20230314_zhengshu_batch01_object9_ver003/train"
+hod.add_images_dir(dataset, f"{from_dir}/data", "train")
 hod.add_detection_labels(dataset, "ground_truth", f"{from_dir}/labels.json", label_classes, mode="coco")
 
-from_dir = "/workspace/users/hejian/tmp/novabot_front_det_20230505_zhengshu_batch02_object9_ver003b/train"
-hod.add_images_dir(dataset, f"{from_dir}/data", None)
+from_dir = "/workspace/users/hejian/tmp/novabot_front_det_20230505_zhengshu_batch02_object9_ver003/train"
+hod.add_images_dir(dataset, f"{from_dir}/data", "val")
 hod.add_detection_labels(dataset, "ground_truth", f"{from_dir}/labels.json", label_classes, mode="coco")
 
 ret = hoc.count_values(dataset, "ground_truth.detections.label")
 print("count-images:", dataset.count("filepath"))
 
 # %%
 dataset = dataset.filter_labels("ground_truth", ~F("label").is_in(["leaf debris"]), only_matches=False)
@@ -58,24 +58,40 @@
 print("count-images:", dataset.count("filepath"))
 
 # %%
 dataset.default_classes = dataset.default_classes[:-1]
 print(f"{dataset.default_classes=}\n{dataset.default_mask_targets=}")
 
 # %%
-hod.delete_duplicate_labels(dataset, "ground_truth", iou_thresh=0.95, method="simple", iscrowd=None, classwise=False)
+hod.delete_duplicate_labels(dataset, "ground_truth", iou_thresh=0.99, method="simple", iscrowd=None, classwise=False)
 print("count-labels:", dataset.count("ground_truth.detections"))
 
 # %% [markdown]
 # ---
 # start
 
 # %%
 label_ids = []
-range_a, range_b = 0, 16 * 16 * 9
+range_a, range_b = 0, 64
+for sample_detections in dataset.values("ground_truth.detections"):
+    for detection in sample_detections:
+        x, y, w, h = detection.bounding_box
+        area = w * 1920 * h * 1080
+        if range_a <= area < range_b:
+            label_ids.append(detection.id)
+print(f"[{range_a}, {range_b}]: {len(label_ids)=}")
+ret = hoc.count_values(dataset, "ground_truth.detections.tags")
+
+# %%
+dataset.select_labels(ids=label_ids).tag_labels("ignore")
+ret = hoc.count_values(dataset, "ground_truth.detections.tags")
+
+# %%
+label_ids = []
+range_a, range_b = 64, 16 * 16 * 9
 for sample_detections in dataset.values("ground_truth.detections"):
     for detection in sample_detections:
         x, y, w, h = detection.bounding_box
         area = w * 1920 * h * 1080
         if range_a <= area < range_b:
             label_ids.append(detection.id)
 print(f"[{range_a}, {range_b}]: {len(label_ids)=}")
@@ -91,46 +107,45 @@
 for sample_detections in dataset.values("ground_truth.detections"):
     for detection in sample_detections:
         x, y, w, h = detection.bounding_box
         area = w * 1920 * h * 1080
         if range_a <= area < range_b:
             label_ids.append(detection.id)
 print(f"[{range_a}, {range_b}]: {len(label_ids)=}")
-ret = hoc.count_values(dataset, "ground_truth.detections.iscrowd")
+ret = hoc.count_values(dataset, "ground_truth.detections.tags")
 
 # %%
-dataset.untag_labels(["issue", "ignore", "todo"])
+dataset.untag_labels("todo")
 dataset.tag_labels("train")
 dataset.select_labels(ids=label_ids).tag_labels("todo")
 dataset.select_labels(tags=["todo"]).untag_labels("train")
 ret = hoc.count_values(dataset, "ground_truth.detections.tags")
 
 # %%
 hob.compute_similarity(dataset, "ground_truth", "gt_sim", "clip-vit-base32-torch")
 
 # %%
 patches = hob.patches_view(dataset, "ground_truth")
 session = fo.launch_app(view=patches, port=20001, address="192.168.0.119", auto=False)  # tag label for `issue/ignore`
 
 # %%
 dataset.untag_samples("issue")
-dataset.tag_samples("train")
 dataset.select_labels(tags="issue", omit_empty=True).tag_samples("issue")
-dataset.match_tags("issue").untag_samples("train")
+dataset.match_tags("issue").untag_samples(["train", "val"])
 ret = hoc.count_values(dataset, "tags")
 
 # %%
 dataset = dataset.exclude_labels(tags="ignore", omit_empty=False)
 ret = hoc.count_values(dataset, "ground_truth.detections.label")
 print("count-images:", dataset.count("filepath"))
 
 # %% [markdown]
 # end
 #
 # ---
 
 # %%
-hoco.coco_export(f"exports/{dataset_name}", dataset, label_field="ground_truth", splits=["train", "issue"])
+hoco.coco_export(f"exports/{dataset_name}", dataset, label_field="ground_truth", splits=["train", "val", "issue"])
 
 # %%
 hoc.random_split(dataset.match_tags("train"), splits={"val": 0.1, "train": 0.9}, seed=51)
 hoco.coco_export(f"exports/{dataset_name}", dataset, label_field="ground_truth", splits=["train", "val", "issue"])
```

### Comparing `hello2-1.9.2/hello/fiftyone/novabot/seg_base.py` & `hello2-1.9.3/hello/fiftyone/novabot/seg_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 import hello
 import hello.fiftyone.core as hoc
 import hello.fiftyone.dataset as hod
 
 print(hello.__version__)
 
 # %%
-dataset_name = "novabot_front_seg_20230404_test_640_suzhou_mall_val_ok_ver001"
+dataset_name = "novabot_front_seg_20230404_test_640_suzhou_mall_ver001"
 dataset_type = "segmentation"
 version = "map9"
 classes = ["unlabeled", "background", "lawn", "road", "terrain", "obstacle", "leaf debris", "faeces", "unknown", "charging station", "ignore"]
 mask_targets = {0: "unlabeled", 1: "background", 2: "lawn", 3: "road", 4: "terrain", 5: "obstacle", 6: "leaf debris", 7: "faeces", 8: "unknown", 9: "charging station", 255: "ignore"}
 
 hod.delete_datasets([dataset_name], non_persistent=False)
 dataset = hod.create_dataset(dataset_name, dataset_type, version, classes, mask_targets)
 
 # %%
 label_mask_targets = dataset.default_mask_targets
 
 from_dir = "/workspace/users/hejian/tmp/Segmentation/train"
-hod.add_images_dir(dataset, f"{from_dir}/data", None)
+hod.add_images_dir(dataset, f"{from_dir}/data", "train")
+
+from_dir = "/workspace/users/hejian/tmp/Segmentation/train"
 hod.add_segmentation_labels(dataset, "ground_truth", f"{from_dir}/labels", label_mask_targets, mode="png")
 
 # %%
 new_classes = None
 
 dataset = hoc.remap_segmentation_dataset(dataset, new_classes, "ground_truth", ignore_index=255, least_one=True)
 print(f"{dataset.default_classes=}\n{dataset.default_mask_targets=}")
```

### Comparing `hello2-1.9.2/hello/fiftyone/novabot/tag_data.py` & `hello2-1.9.3/hello/fiftyone/novabot/tag_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 classes = ["nothing", "anything", "ok", "ng"]
 mask_targets = {}
 
 hod.delete_datasets([dataset_name], non_persistent=False)
 dataset = hod.create_dataset(dataset_name, dataset_type, version, classes, mask_targets)
 
 from_dir = "/workspace/users/hejian/todo/novabot_front_det_20230525_zhengshu_batch02_object9_ver002/nothing"
-hod.add_images_dir(dataset, f"{from_dir}/data", None)
+hod.add_images_dir(dataset, f"{from_dir}/data", "train")
 
 print("count-images:", dataset.count("filepath"))
 
 # %%
 view = dataset
 
 hoa.to_cvat(
```

### Comparing `hello2-1.9.2/hello/fiftyone/patches.py` & `hello2-1.9.3/hello/fiftyone/patches.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/tarinfo.py` & `hello2-1.9.3/hello/fiftyone/tarinfo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/unique.py` & `hello2-1.9.3/hello/fiftyone/unique.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/utils.py` & `hello2-1.9.3/hello/fiftyone/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/video.py` & `hello2-1.9.3/hello/fiftyone/video.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fiftyone/view.py` & `hello2-1.9.3/hello/fiftyone/view.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/fvcore/core.py` & `hello2-1.9.3/hello/fvcore/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/io/image.py` & `hello2-1.9.3/hello/io/image.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/io/utils.py` & `hello2-1.9.3/hello/io/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmdet/__init__.py` & `hello2-1.9.3/hello/mmdet/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmdet/flop.py` & `hello2-1.9.3/hello/mmdet/flop.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmdet/infer.py` & `hello2-1.9.3/hello/mmdet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmdet/log.py` & `hello2-1.9.3/hello/mmdet/log.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmdet/plot.py` & `hello2-1.9.3/hello/mmdet/plot.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmlab/__init__.py` & `hello2-1.9.3/hello/mmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmlab/mmseg.py` & `hello2-1.9.3/hello/mmlab/mmseg.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmseg/__init__.py` & `hello2-1.9.3/hello/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmseg/infer.py` & `hello2-1.9.3/hello/mmseg/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmseg/log.py` & `hello2-1.9.3/hello/mmseg/log.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/mmseg/lr.py` & `hello2-1.9.3/hello/mmseg/lr.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/nanodet/infer.py` & `hello2-1.9.3/hello/nanodet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/onnx/examples/test_sigmoid.py` & `hello2-1.9.3/hello/onnx/examples/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/onnx/export.py` & `hello2-1.9.3/hello/onnx/export.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/onnx/infer.py` & `hello2-1.9.3/hello/onnx/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/transforms/README.md` & `hello2-1.9.3/hello/transforms/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/transforms/transforms.py` & `hello2-1.9.3/hello/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/utils/colors.py` & `hello2-1.9.3/hello/utils/colors.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/utils/compare.py` & `hello2-1.9.3/hello/utils/compare.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/utils/cuda.py` & `hello2-1.9.3/hello/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/utils/plots.py` & `hello2-1.9.3/hello/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/utils/points.py` & `hello2-1.9.3/hello/utils/points.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/__init__.py` & `hello2-1.9.3/hello/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/align.py` & `hello2-1.9.3/hello/video/align.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/clip.py` & `hello2-1.9.3/hello/video/clip.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/fisheye.py` & `hello2-1.9.3/hello/video/fisheye.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/info.py` & `hello2-1.9.3/hello/video/info.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/resize.py` & `hello2-1.9.3/hello/video/resize.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/rtsp.py` & `hello2-1.9.3/hello/video/rtsp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/rtsp_pull.py` & `hello2-1.9.3/hello/video/rtsp_pull.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/split.py` & `hello2-1.9.3/hello/video/split.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/unwarp.py` & `hello2-1.9.3/hello/video/unwarp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/video/utils.py` & `hello2-1.9.3/hello/video/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/x3m/__init__.py` & `hello2-1.9.3/hello/x3m/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/x3m/config.py` & `hello2-1.9.3/hello/x3m/config.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/x3m/nanodet/best_one.py` & `hello2-1.9.3/hello/x3m/nanodet/best_one.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/x3m/preprocess.py` & `hello2-1.9.3/hello/x3m/preprocess.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello/x3m/transforms.py` & `hello2-1.9.3/hello/x3m/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello_c/CMakeLists.txt` & `hello2-1.9.3/hello_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello_c/README.md` & `hello2-1.9.3/hello_c/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/hello_c/main.cpp` & `hello2-1.9.3/hello_c/main.cpp`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/pyproject.toml` & `hello2-1.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hello2-1.9.2/PKG-INFO` & `hello2-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello2
-Version: 1.9.2
+Version: 1.9.3
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scikit-image
```

