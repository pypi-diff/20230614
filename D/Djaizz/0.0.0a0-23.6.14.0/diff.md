# Comparing `tmp/Djaizz-0.0.0a0.tar.gz` & `tmp/Djaizz-23.6.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Djaizz-0.0.0a0.tar", last modified: Wed Mar  1 07:06:05 2023, max compression
+gzip compressed data, was "Djaizz-23.6.14.0.tar", last modified: Wed Jun 14 21:54:48 2023, max compression
```

## Comparing `Djaizz-0.0.0a0.tar` & `Djaizz-23.6.14.0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.892354 Djaizz-0.0.0a0/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:49:59.000000 Djaizz-0.0.0a0/LICENSE
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5699 2023-03-01 07:06:05.891390 Djaizz-0.0.0a0/PKG-INFO
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      187 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/README.md
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.834139 Djaizz-0.0.0a0/metadata/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2584 2023-03-01 06:43:11.000000 Djaizz-0.0.0a0/metadata/classifiers
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       52 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/metadata/description
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       65 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/metadata/entry-points
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.835695 Djaizz-0.0.0a0/metadata/requirements/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6383 2023-03-01 06:40:05.000000 Djaizz-0.0.0a0/metadata/requirements/base.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/metadata/requirements/build.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       41 2023-02-28 19:58:24.000000 Djaizz-0.0.0a0/metadata/requirements/dev.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      199 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/metadata/requirements/doc.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      189 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/metadata/requirements/lint.txt
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)       15 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/metadata/requirements/publish.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/metadata/requirements/test.txt
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)      159 2023-03-01 05:20:06.000000 Djaizz-0.0.0a0/metadata/requirements/viz.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        9 2023-03-01 07:05:50.000000 Djaizz-0.0.0a0/metadata/version
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2722 2023-03-01 03:33:37.000000 Djaizz-0.0.0a0/pyproject.toml
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-03-01 07:06:05.892435 Djaizz-0.0.0a0/setup.cfg
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.827186 Djaizz-0.0.0a0/src/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.836886 Djaizz-0.0.0a0/src/Djaizz.egg-info/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5699 2023-03-01 07:06:05.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/PKG-INFO
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5814 2023-03-01 07:06:05.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/SOURCES.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 07:06:05.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/dependency_links.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       50 2023-03-01 07:06:05.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/entry_points.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3486 2023-03-01 07:06:05.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/requires.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-03-01 07:06:05.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/top_level.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 01:27:25.000000 Djaizz-0.0.0a0/src/Djaizz.egg-info/zip-safe
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.838179 Djaizz-0.0.0a0/src/djaizz/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      300 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.838873 Djaizz-0.0.0a0/src/djaizz/client/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      270 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/client/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.842449 Djaizz-0.0.0a0/src/djaizz/data/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      873 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/data/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.843026 Djaizz-0.0.0a0/src/djaizz/data/api/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      816 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/data/api/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.843380 Djaizz-0.0.0a0/src/djaizz/data/api/gql/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/data/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.843550 Djaizz-0.0.0a0/src/djaizz/data/api/json/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/data/api/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.843686 Djaizz-0.0.0a0/src/djaizz/data/api/rest/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/data/api/rest/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2703 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/data/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.846026 Djaizz-0.0.0a0/src/djaizz/data/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6026 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1730 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1537 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/data/migrations/0003_Django4.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/data/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.853975 Djaizz-0.0.0a0/src/djaizz/data/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1005 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/audio.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8019 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/data/models/base.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/csv.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/hdf.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/image.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2596 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/data/models/json.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      528 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/live_api.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      585 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/numpy.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/orc.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      595 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/pandas.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      550 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/parquet.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.857917 Djaizz-0.0.0a0/src/djaizz/data/models/public/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/gov.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/hugging_face.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/intl_dev.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       31 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/kaggle.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/tf.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       30 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/torch.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       51 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/public/weather.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      538 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/text.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/tfrecord.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/models/video.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      294 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/data/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.859418 Djaizz-0.0.0a0/src/djaizz/model/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2559 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.859850 Djaizz-0.0.0a0/src/djaizz/model/api/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1821 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/api/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.860211 Djaizz-0.0.0a0/src/djaizz/model/api/gql/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/model/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.860392 Djaizz-0.0.0a0/src/djaizz/model/api/json/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/model/api/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.860534 Djaizz-0.0.0a0/src/djaizz/model/api/rest/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/model/api/rest/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3259 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.863050 Djaizz-0.0.0a0/src/djaizz/model/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3211 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/0001_AIModel.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2941 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    18732 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1226 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/0004_CloudAIService.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1237 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/0005_GoogleTranslate.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8705 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/0006_Django4.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/model/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.863565 Djaizz-0.0.0a0/src/djaizz/model/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1867 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    22849 2023-03-01 05:20:06.000000 Djaizz-0.0.0a0/src/djaizz/model/models/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.864996 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      340 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.865638 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/amazon/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/amazon/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1021 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.866425 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/google/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      286 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/google/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8515 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/google/translation.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.866742 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/hugging_face/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       58 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/hugging_face/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.866984 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.867229 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/meta/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       72 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/meta/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.867515 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/microsoft/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/microsoft/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.867883 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       59 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.868616 Djaizz-0.0.0a0/src/djaizz/model/models/ml/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1769 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1903 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.876350 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1905 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9281 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/audio_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1205 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/base.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9015 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9838 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/mask_filling.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9808 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/object_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10454 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/question_answering.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8687 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9357 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9626 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8708 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10322 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text_generation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9563 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text_summarization.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8802 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/token_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10212 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/translation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10360 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.877059 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      386 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2127 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.877396 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/pre_trained/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      322 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/pre_trained/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.878162 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/pre_trained/vision/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      343 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/pre_trained/vision/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    12295 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1446 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/skl.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.878683 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      265 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      814 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.878925 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       46 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.879485 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/audio/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/audio/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       74 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/audio/text_to_speech.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.882062 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       71 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/instance_segmentation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       69 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/keypoint_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       67 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/object_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       70 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/semantic_segmentation.py
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/pre_trained/vision/video_classification.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.883380 Djaizz-0.0.0a0/src/djaizz/model/scripts/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      401 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/scripts/setup_google_cloud_ai_svcs.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    19753 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8394 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/scripts/setup_pretrained_keras_models.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      705 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/model/urls.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5321 2023-03-01 05:20:06.000000 Djaizz-0.0.0a0/src/djaizz/model/views.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      838 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.885943 Djaizz-0.0.0a0/src/djaizz/util/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1018 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.887737 Djaizz-0.0.0a0/src/djaizz/util/cli/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      734 2023-03-01 06:27:43.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.888933 Djaizz-0.0.0a0/src/djaizz/util/cli/_server_files/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/_server_files/asgi.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      426 2023-02-28 00:21:53.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/_server_files/manage.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      553 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/_server_files/wsgi.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-03-01 07:06:05.890915 Djaizz-0.0.0a0/src/djaizz/util/cli/aws_eb/
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)     8629 2023-02-28 22:45:23.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/aws_eb/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1261 2023-03-01 06:40:05.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/deps.py
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)     4374 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/cli/run_cmd.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1310 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/git.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1321 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/pip.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1740 2023-02-28 04:56:41.000000 Djaizz-0.0.0a0/src/djaizz/util/views.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.393320 Djaizz-23.6.14.0/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:49:59.000000 Djaizz-23.6.14.0/LICENSE
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-14 21:54:48.393090 Djaizz-23.6.14.0/PKG-INFO
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      187 2023-02-28 01:51:17.000000 Djaizz-23.6.14.0/README.md
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.302869 Djaizz-23.6.14.0/metadata/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2584 2023-03-09 04:40:50.000000 Djaizz-23.6.14.0/metadata/classifiers
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       52 2023-02-28 04:56:41.000000 Djaizz-23.6.14.0/metadata/description
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       65 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/metadata/entry-points
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.304092 Djaizz-23.6.14.0/metadata/requirements/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     6282 2023-06-14 21:25:21.000000 Djaizz-23.6.14.0/metadata/requirements/base.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-02-28 04:56:41.000000 Djaizz-23.6.14.0/metadata/requirements/build.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       40 2023-06-14 20:47:00.000000 Djaizz-23.6.14.0/metadata/requirements/dev.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      215 2023-06-14 21:42:52.000000 Djaizz-23.6.14.0/metadata/requirements/doc.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      225 2023-06-14 19:57:11.000000 Djaizz-23.6.14.0/metadata/requirements/lint.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       15 2023-02-28 04:56:41.000000 Djaizz-23.6.14.0/metadata/requirements/publish.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-06-13 01:17:31.000000 Djaizz-23.6.14.0/metadata/requirements/test.txt
+-rwxr-xr-x   0 thevinhluong102   (501) staff       (20)      150 2023-06-13 01:17:55.000000 Djaizz-23.6.14.0/metadata/requirements/viz.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-14 20:00:31.000000 Djaizz-23.6.14.0/metadata/version
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3129 2023-06-14 20:38:47.000000 Djaizz-23.6.14.0/pyproject.toml
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-14 21:54:48.393384 Djaizz-23.6.14.0/setup.cfg
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.298295 Djaizz-23.6.14.0/src/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.305152 Djaizz-23.6.14.0/src/Djaizz.egg-info/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/PKG-INFO
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5814 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/SOURCES.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/dependency_links.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       50 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/entry_points.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3893 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/requires.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-14 21:54:48.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/top_level.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 01:27:25.000000 Djaizz-23.6.14.0/src/Djaizz.egg-info/zip-safe
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.306645 Djaizz-23.6.14.0/src/djaizz/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      300 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.307220 Djaizz-23.6.14.0/src/djaizz/client/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      270 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/client/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.309140 Djaizz-23.6.14.0/src/djaizz/data/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      873 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.309786 Djaizz-23.6.14.0/src/djaizz/data/api/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      816 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/api/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.310254 Djaizz-23.6.14.0/src/djaizz/data/api/gql/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.310426 Djaizz-23.6.14.0/src/djaizz/data/api/json/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/api/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.310595 Djaizz-23.6.14.0/src/djaizz/data/api/rest/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/api/rest/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2703 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.312795 Djaizz-23.6.14.0/src/djaizz/data/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     6026 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1730 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1537 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/0003_Django4.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.329470 Djaizz-23.6.14.0/src/djaizz/data/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1005 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/audio.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8019 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/models/base.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/csv.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/hdf.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/image.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2596 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/data/models/json.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      528 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/live_api.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      585 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/numpy.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/orc.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      595 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/pandas.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      550 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/parquet.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.334832 Djaizz-23.6.14.0/src/djaizz/data/models/public/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/gov.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/hugging_face.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/intl_dev.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       31 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/kaggle.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/tf.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       30 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/torch.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       51 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/public/weather.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      538 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/text.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/tfrecord.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/models/video.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      294 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/data/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.337023 Djaizz-23.6.14.0/src/djaizz/model/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2559 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.341411 Djaizz-23.6.14.0/src/djaizz/model/api/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1821 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/api/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.342006 Djaizz-23.6.14.0/src/djaizz/model/api/gql/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.342148 Djaizz-23.6.14.0/src/djaizz/model/api/json/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/api/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.342283 Djaizz-23.6.14.0/src/djaizz/model/api/rest/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/api/rest/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3259 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.349570 Djaizz-23.6.14.0/src/djaizz/model/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3211 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0001_AIModel.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2941 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    18732 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1226 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0004_CloudAIService.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1237 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0005_GoogleTranslate.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8705 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/0006_Django4.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.358789 Djaizz-23.6.14.0/src/djaizz/model/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1867 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    22789 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.360350 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      340 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.361069 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/amazon/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/amazon/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1021 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.362278 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      286 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8461 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.362545 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       58 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.363135 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.363567 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/meta/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       72 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/meta/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.365053 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/microsoft/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/microsoft/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.365594 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       59 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.366755 Djaizz-23.6.14.0/src/djaizz/model/models/ml/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1769 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1849 2023-06-06 18:00:24.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.374283 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1905 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9221 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1205 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/base.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8955 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9778 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9748 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/object_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10400 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/question_answering.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8633 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9303 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9572 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8648 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10268 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_generation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9509 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8748 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/token_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10158 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/translation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10300 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.375283 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      386 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2127 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.375759 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      322 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.376787 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      343 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    12235 2023-06-06 18:00:24.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1446 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/skl.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.377568 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      265 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      814 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.378052 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       46 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.379318 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/audio/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/audio/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       74 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/audio/text_to_speech.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.384334 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       71 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/instance_segmentation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       69 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/keypoint_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       67 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/object_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       70 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/semantic_segmentation.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/pre_trained/vision/video_classification.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.386250 Djaizz-23.6.14.0/src/djaizz/model/scripts/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      401 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_google_cloud_ai_svcs.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    19753 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8394 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      705 2023-02-28 22:45:23.000000 Djaizz-23.6.14.0/src/djaizz/model/urls.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5267 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/model/views.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      838 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.388759 Djaizz-23.6.14.0/src/djaizz/util/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1018 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.390666 Djaizz-23.6.14.0/src/djaizz/util/cli/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      735 2023-05-26 21:52:35.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.392113 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/asgi.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      426 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/manage.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      553 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/wsgi.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 21:54:48.392645 Djaizz-23.6.14.0/src/djaizz/util/cli/aws_eb/
+-rwxr-xr-x   0 thevinhluong102   (501) staff       (20)    11074 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/aws_eb/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1022 2023-06-14 19:36:12.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/deps.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     4374 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/cli/run_cmd.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1310 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/git.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1261 2023-06-06 18:00:20.000000 Djaizz-23.6.14.0/src/djaizz/util/pip.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1740 2023-02-28 00:21:53.000000 Djaizz-23.6.14.0/src/djaizz/util/views.py
```

### Comparing `Djaizz-0.0.0a0/LICENSE` & `Djaizz-23.6.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/PKG-INFO` & `Djaizz-23.6.14.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaizz
-Version: 0.0.0a0
+Version: 23.6.14.0
 Summary: Artificial Intelligence (AI) in Django Applications
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
         
@@ -92,15 +92,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: lint
 Provides-Extra: publish
 Provides-Extra: test
```

### Comparing `Djaizz-0.0.0a0/metadata/classifiers` & `Djaizz-23.6.14.0/metadata/classifiers`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/metadata/requirements/base.txt` & `Djaizz-23.6.14.0/metadata/requirements/base.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,147 +1,161 @@
 # DATA MANAGEMENT & PROCESSING
 # ============================
 
-Dask >= 2023.2.1
-Distributed >= 2023.2.1
-MetaFlow >= 2.8.0
-NumBa >= 0.56.4; python_version < '3.11'
+Dask >= 2023.6.0
+Distributed >= 2023.6.0
+Kedro >= 0.18.10; python_version < '3.11'
+MetaFlow >= 2.9.4
+NumBa >= 0.57.0
 NumPy >= 1.23
   # let higher dependencies figure
-Pandas >= 1.5.3
-Pandarallel >= 1.6.4
-PyArrow >= 11.0.0
-PySpark >= 3.3.2
-Ray >= 1.13.0; python_version < '3.11'
+Pandas >= 1.5
+  # let higher dependencies figure
+Pandarallel >= 1.6.5
+PyArrow >= 12.0.1
+PySpark >= 3.4.0
+Ray >= 2.5.0; python_version < '3.11'
 SciPy >= 1.10.1
 
-Pillow >= 9.4.0
+Pillow >= 9.5.0
 # Pillow-SIMD >= 9.0.0
   # complex to install
-SciKit-Image >= 0.19.3
+PyCOCOTools >= 2.0.6
+SciKit-Image >= 0.21.0
 
-Kedro >= 0.18.5; python_version < '3.11'
+XDF >= 23.6.14
 
 
 # MACHINE LEARNING / DEEP LEARNING & RELATED
 # ==========================================
 
 Imbalanced-Learn >= 0.10.1
-StatsModels >= 0.13.5
+StatsModels >= 0.14.0
 
 # SciKit-Learn & related
 # Auto-SKLearn >= 0.15.0
   # depends on SciKit-Learn < 0.25
-SciKit-Learn >= 1.2.1
+SciKit-Learn >= 1.2.2
 
 # TensorFlow & related
-TensorFlow >= 2.12.0rc0
-TensorFlow-DataSets >= 4.8.3
-TensorFlow-Hub >= 0.12.0
+TensorFlow >= 2.12.0; sys_platform != 'darwin'
+TensorFlow-MacOS >= 2.12.0; sys_platform == 'darwin'
+TensorFlow-Metal >= 1.0.1; sys_platform == 'darwin'
+TensorFlow-DataSets >= 4.9.2
+TensorFlow-Hub >= 0.13.0
 
 # Torch & related
-Torch >= 1.13.1; python_version < '3.11'
-Torch-Model-Archiver >= 0.7.1
-TorchServe >= 0.7.1
-
-TorchAudio >= 0.13.1; python_version < '3.11'
-TorchText >= 0.14.1; python_version < '3.11'
-TorchVision >= 0.14.1; python_version < '3.11'
+Torch >= 2.0.1
+Torch-Model-Archiver >= 0.8.1
+TorchServe >= 0.8.1
+
+TorchAudio >= 2.0.2
+TorchText >= 0.15.2
+TorchVision >= 0.15.2
 
 # Computer Vision
 OpenCV-Python >= 4.7.0
 
 # Hugging Face & related
-DataSets >= 2.10.0
-HuggingFace-Hub >= 0.12.1
-Transformers >= 4.26.1
+DataSets >= 2.13.0
+HuggingFace-Hub >= 0.15.1
+Transformers >= 4.30.2
 
-SentencePiece >= 0.1.97
-TIMM >= 0.6.12; python_version < '3.11'
+SentencePiece >= 0.1.99
+TIMM >= 0.9.2
 # Torch-Scatter >= 2.1.0
   # Table Question Answering - requires Torch first
 
+# Fast AI
+FastAI >= 2.7.12
+
 # Topological Data Analysis (TDA) & related
-Giotto-TDA >= 0.6.0; python_version < '3.11'
-GUDHI >= 3.7.1
+Giotto-TDA >= 0.6.0; python_version < '3.11'  # TODO
+GUDHI >= 3.8.0
 
 # Cloud AI/ML Services
-# Google-Cloud-Translate >= 3.10.1
+# Google-Cloud-Translate >= 3.11.1
   # conflicting/slow-resolving dependencies
 GoogleTrans >= 4.0.0rc1
 
 # Hyper-Parameter Tuning & related
-Bayesian-Optimization >= 1.4.2
-ConfigSpace >= 0.6.1
+Bayesian-Optimization >= 1.4.3
+ConfigSpace >= 0.7.1
 Hpbandster >= 0.7.4
 Tabulate >= 0.9.0
 
 # ML Model Explainability & related
-# CausalNex >= 0.11.0; python_version < '3.11'
+CausalNex >= 0.12.0; python_version < '3.11'
   # depends on outdated SciPy, SciKit-Learn
 LIME >= 0.2.0.1
-SHAP >= 0.41.0; python_version < '3.11'
+SHAP >= 0.41.0
 
 # ML Model Management
-# MLFLow >= 2.1.1
-  # conflicting/slow-resolving dependencies
+# MLFLow >= 2.3.2
+  # depends on outdated PyArrow < 12
 
 
 # NON-ML MODELING
 # ===============
 
 # Fuzzy Logic
 SciKit-Fuzzy >= 0.4.2
 
 
+# LARGE FOUNDATIONAL MODELS & related
+# ===================================
+
+AutoGPT >= 0.0.1.dev0
+LangChain >= 0.0.200
+OpenAI >= 0.27.8
+PandasAI >= 0.5.2
+
+
 # FILE SYSTEMS
 # ============
-FSSpec >= 2023.1.0
-# S3FS >= 2023.1.0
-  # conflicting/slow-resolving dependencies
+FSSpec >= 2023.6.0
 
 
 # MODEL REPOSITORY & RELATED
 # ==========================
 CloudPickle >= 2.2.1
 JobLib >= 1.2.0
 
 
 # DJANGO & RELATED APPLICATION DEVELOPMENT
 # ========================================
 
 # Django Core
-Django >= 4.1.7
+Django >= 4.2.2
 
 # Django Polymorphic Models
 Django-Polymorphic >= 3.1.0
 
 # Django Admin-related
 Django-Admin-HStore-Widget >= 1.2.1
 Django-Admin-Relation-Links >= 0.2.5
-# Django-ForestAdmin >= 1.4.5; python_version < '3.11'
-  # depends on outdated Python < 3.11
-Django-Grappelli >= 3.0.4
+Django-ForestAdmin >= 1.5.0; python_version < '3.11'  # TODO
+Django-Grappelli >= 3.0.6
 Django-Jazzmin >= 2.6.0
 
 # Django-AutoComplete-Light & related
-Django-Autocomplete-Light >= 3.9.4
+Django-Autocomplete-Light >= 3.9.7
 Django-Generic-M2M >= 0.3.1
 Django-GM2M >= 1.1.1
 Django-QuerySetSequence >= 0.16
 Django-Tagging >= 0.5.0
-Django-Taggit >= 3.1.0
+Django-Taggit >= 4.0.0
 
 # GraphQL
-Ariadne >= 0.18.1
+Ariadne >= 0.19.1
 Django-GraphQL-Extensions >= 0.1.0
 Django-RESTQL >= 0.15.3
-GQL >= 3.4.0
-Graphene >= 3.2.1
-Graphene-Django >= 3.0.0
+GQL >= 3.4.1
+Graphene >= 3.2.2
+Graphene-Django >= 3.1.1
 # Graphene-Django-Extras >= 0.5.2
   # conflicting/slow-resolving dependencies
 Graphene-Django-Optimizer >= 0.9.1
 # Graphene-Django-Subscriptions >= 0.0.9
   # conflicting/slow-resolving dependencies
 # Graphene-Django-Tools >= 0.21.0
   # conflicting/slow-resolving dependencies
@@ -149,146 +163,150 @@
   # conflicting/slow-resolving dependencies
 # Graphene-SQLAlchemy >= 2.3.0
   # conflicting/slow-resolving dependencies
 GraphQLClient >= 0.2.4
 GraphQL-Core >= 3.2.3
 GraphQL-Relay >= 3.2.0
 Py-GQL >= 0.6.1
-SGQLC >= 16.1
-Strawberry-GraphQL >= 0.159.0
+SGQLC >= 16.2
+Strawberry-GraphQL >= 0.185.1
 
 # Django REST Framework & other API-related
 DjangoRESTFramework >= 3.14.0
 DRFPasswordless >= 1.5.8
-DRF-Writable-Nested >= 0.6.4
+DRF-Writable-Nested >= 0.7.0
 CoreAPI >= 2.3.3
   # closely related to Django REST Framework
 CoreAPI-CLI >= 1.0.9
-Markdown >= 3.4.1
+Markdown >= 3.4.3
   # Markdown support for the browsable API
 
-DjangoRESTFramework-JSONAPI >= 6.0.0
+# DjangoRESTFramework-JSONAPI >= 6.0.0
+  # depends on outdated Django < 4.2
 DRF-Nested-Routers >= 0.93.4
-Django-PolyModels >= 1.7.0
-Django-Typed-Models >= 0.12.0
+Django-PolyModels >= 1.8.0
+Django-Typed-Models >= 0.13.0
 
 HAL-Codec >= 1.0.2
 JSONHyperSchema-Codec >= 1.0.3
 OpenAPI-Codec >= 1.3.2
 
 JSONSchema >= 4.17.3
-Pydantic >= 1.10.5
+Pydantic >= 1.10.9
 
-HTTPie >= 3.2.1
+HTTPie >= 3.2.2
 
 # Django Filtering
-Django-Filter >= 22.1
+Django-Filter >= 23.2
 DjangoRESTFramework-Filters >= 1.0.0.dev2
 
 # Django Object-Level Permissions
 Django-Guardian >= 2.4.0
 Rules >= 3.3
 
 # Django Debugging & Query Profiling
-Django-Debug-Toolbar >= 3.8.1
+Django-Debug-Toolbar >= 4.1.0
 Django-Query-Profiler >= 0.9
 Django-Silk >= 5.0.3
-Kolo >= 2.4.2
+Kolo >= 2.9.4
 
 # Django Extensions & Utilities
 Django-Annoying >= 0.10.6
 Django-Choices >= 1.7.2
 Django-Compressor >= 4.3.1
-Django-Configurations >= 2.4
+Django-Configurations >= 2.4.1
 Django-Crispy-Forms >= 2.0
-Django-Environ >= 0.9.0
-Django-Extensions >= 3.2.1
+Django-Environ >= 0.10.0
+Django-Extensions >= 3.2.3
 Django-JSON-Widget >= 1.1.1
-Django-LocalFlavor >= 3.1
+Django-LocalFlavor >= 4.0
 Django-Nested-InLines >= 0.1
 Django-Storages >= 1.13.2
 
-Django-Query-Graph >= 0.0.0.dev1
-Dj-Util >= 0.0.0.dev1
+Django-Query-Graph >= 23.6.14
+Dju >= 23.6.14
 
 # Django CORS Headers
-Django-CORS-Headers >= 3.10
-  # let higher dependencies figure
+Django-CORS-Headers >= 4.1.0
 
 # Application UIs
-Django-HTMX >= 1.14.0
+Django-HTMX >= 1.15.0
 
-Django-Plotly-Dash >= 1.7
-  # DPD >=2 depends on outdated Django < 4
-  # github.com/GibbsConsulting/django-plotly-dash/issues/403
-Dash-Bootstrap-Components >= 0.13
-  # compatible with Django-Plotly-Dash < 2
+Django-Plotly-Dash >= 2.2.1
+Dash-Bootstrap-Components >= 1.4.1
 DPD-Static-Support >= 0.0.5
-Django-Bootstrap4 >= 22.3
+Django-Bootstrap4 >= 23.1
 WhiteNoise >= 6.4.0
 
-Flask >= 2.1, < 2.2
-  # github.com/localstack/localstack/issues/6587
-Werkzeug >= 2.0, < 2.1
-  # github.com/plotly/dash/issues/1992
-
-Gradio >= 3.19.1
+Gradio >= 3.34.0
+Gradio-Tools >= 0.0.9
 
-Streamlit >= 1.19.0
-Watchdog >= 2.3.0
+Streamlit >= 1.23.1
+Watchdog >= 3.0.0
 
 # Database Adapters/Backends/Connectors/Drivers
 MariaDB-DynCol >= 3.6.1
 Django-MySQL >= 4.9.0
 MySQLClient >= 2.1.1
-MySQL-Connector-Python >= 8.0.32
-PsycoPG2-binary >= 2.9.5
+MySQL-Connector-Python >= 8.0.33
+PsycoPG >= 3.1.9
+PsycoPG2-binary >= 2.9.6
 
 # ASGI Web Servers & related
-ASGIRef >= 3.6.0
-Channels >= 2.4
-  # let higher dependencies figure
-Daphne >= 2.5
-  # let higher dependencies figure
+ASGIRef >= 3.7.2
+Channels >= 4.0.0
+Daphne >= 4.0.0
 GUnicorn >= 20.1.0
 H11 >= 0.9
   # let higher dependencies figure
 Hypercorn >= 0.14.3
-Quart >= 0.17
-  # let higher dependencies figure
-Starlette >= 0.25.0
-Uvicorn >= 0.20.0
+Quart >= 0.18.4
+Starlette >= 0.28.0
+Uvicorn >= 0.22.0
 
 
 # COMMAND-LINE INTERFACE (CLI)
 # ============================
 CLICK >= 8.1.3
 Colored >= 1.4.4
 
 
 # JUPYTER
 # =======
 Jupyter >= 1.0.0
 
 
+# CLOUD
+# =====
+
+# Amazon Web Services (AWS)
+S3FS >= 2023.6.0
+
+# Microsoft Azure
+ADLFS >= 2023.4.0
+
+# Google Cloud Platform (GCP)
+GCSFS >= 2023.6.0
+GDriveFS >= 0.14.13
+
+# Dropbox
+DropboxDriveFS >= 1.3.1
+
+
+# REACT JAVASCRIPT
+# ================
+ReactPy >= 1.0.0
+ReactPy-Django >= 3.1.0
+ReactPy-Jupyter >= 0.9.5
+
+
 # MISC / OTHER
 # ============
 GitPython >= 3.1.31
-Ruamel.YAML >= 0.17.21
-PSUtil >= 5.9.4
+Loguru >= 0.7.0
+PSUtil >= 5.9.5
 Python-DateUtil >= 2.8.2
 Python-DotEnv >= 1.0.0
-PyTZ >= 2022.7.1
-Requests >= 2.28.2
-Tqdm >= 4.64.1
-
-
-# CLOUD
-# =====
-
-# AWS deps: to install separately as they are notoriously hard to install alongside others
-# --------
-# AWSCLI ~= 1.21
-# Boto3 ~= 1.19
-
-# AWSEBCLI ~= 3.2
-# AWSWrangler >= 0.0.8
+PyTZ >= 2023.3
+Requests >= 2.31.0
+Ruamel.YAML >= 0.17.31
+Tqdm >= 4.65.0
```

### Comparing `Djaizz-0.0.0a0/src/Djaizz.egg-info/PKG-INFO` & `Djaizz-23.6.14.0/src/Djaizz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaizz
-Version: 0.0.0a0
+Version: 23.6.14.0
 Summary: Artificial Intelligence (AI) in Django Applications
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
         
@@ -92,15 +92,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Widget Sets
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: build
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: lint
 Provides-Extra: publish
 Provides-Extra: test
```

### Comparing `Djaizz-0.0.0a0/src/Djaizz.egg-info/SOURCES.txt` & `Djaizz-23.6.14.0/src/Djaizz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/Djaizz.egg-info/requires.txt` & `Djaizz-23.6.14.0/src/Djaizz.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,212 @@
-Dask>=2023.2.1
-Distributed>=2023.2.1
-MetaFlow>=2.8.0
+Dask>=2023.6.0
+Distributed>=2023.6.0
+MetaFlow>=2.9.4
+NumBa>=0.57.0
 NumPy>=1.23
-Pandas>=1.5.3
-Pandarallel>=1.6.4
-PyArrow>=11.0.0
-PySpark>=3.3.2
+Pandas>=1.5
+Pandarallel>=1.6.5
+PyArrow>=12.0.1
+PySpark>=3.4.0
 SciPy>=1.10.1
-Pillow>=9.4.0
-SciKit-Image>=0.19.3
+Pillow>=9.5.0
+PyCOCOTools>=2.0.6
+SciKit-Image>=0.21.0
+XDF>=23.6.14
 Imbalanced-Learn>=0.10.1
-StatsModels>=0.13.5
-SciKit-Learn>=1.2.1
-TensorFlow>=2.12.0rc0
-TensorFlow-DataSets>=4.8.3
-TensorFlow-Hub>=0.12.0
-Torch-Model-Archiver>=0.7.1
-TorchServe>=0.7.1
+StatsModels>=0.14.0
+SciKit-Learn>=1.2.2
+TensorFlow-DataSets>=4.9.2
+TensorFlow-Hub>=0.13.0
+Torch>=2.0.1
+Torch-Model-Archiver>=0.8.1
+TorchServe>=0.8.1
+TorchAudio>=2.0.2
+TorchText>=0.15.2
+TorchVision>=0.15.2
 OpenCV-Python>=4.7.0
-DataSets>=2.10.0
-HuggingFace-Hub>=0.12.1
-Transformers>=4.26.1
-SentencePiece>=0.1.97
-GUDHI>=3.7.1
+DataSets>=2.13.0
+HuggingFace-Hub>=0.15.1
+Transformers>=4.30.2
+SentencePiece>=0.1.99
+TIMM>=0.9.2
+FastAI>=2.7.12
+GUDHI>=3.8.0
 GoogleTrans>=4.0.0rc1
-Bayesian-Optimization>=1.4.2
-ConfigSpace>=0.6.1
+Bayesian-Optimization>=1.4.3
+ConfigSpace>=0.7.1
 Hpbandster>=0.7.4
 Tabulate>=0.9.0
 LIME>=0.2.0.1
+SHAP>=0.41.0
 SciKit-Fuzzy>=0.4.2
-FSSpec>=2023.1.0
+AutoGPT>=0.0.1.dev0
+LangChain>=0.0.200
+OpenAI>=0.27.8
+PandasAI>=0.5.2
+FSSpec>=2023.6.0
 CloudPickle>=2.2.1
 JobLib>=1.2.0
-Django>=4.1.7
+Django>=4.2.2
 Django-Polymorphic>=3.1.0
 Django-Admin-HStore-Widget>=1.2.1
 Django-Admin-Relation-Links>=0.2.5
-Django-Grappelli>=3.0.4
+Django-Grappelli>=3.0.6
 Django-Jazzmin>=2.6.0
-Django-Autocomplete-Light>=3.9.4
+Django-Autocomplete-Light>=3.9.7
 Django-Generic-M2M>=0.3.1
 Django-GM2M>=1.1.1
 Django-QuerySetSequence>=0.16
 Django-Tagging>=0.5.0
-Django-Taggit>=3.1.0
-Ariadne>=0.18.1
+Django-Taggit>=4.0.0
+Ariadne>=0.19.1
 Django-GraphQL-Extensions>=0.1.0
 Django-RESTQL>=0.15.3
-GQL>=3.4.0
-Graphene>=3.2.1
-Graphene-Django>=3.0.0
+GQL>=3.4.1
+Graphene>=3.2.2
+Graphene-Django>=3.1.1
 Graphene-Django-Optimizer>=0.9.1
 GraphQLClient>=0.2.4
 GraphQL-Core>=3.2.3
 GraphQL-Relay>=3.2.0
 Py-GQL>=0.6.1
-SGQLC>=16.1
-Strawberry-GraphQL>=0.159.0
+SGQLC>=16.2
+Strawberry-GraphQL>=0.185.1
 DjangoRESTFramework>=3.14.0
 DRFPasswordless>=1.5.8
-DRF-Writable-Nested>=0.6.4
+DRF-Writable-Nested>=0.7.0
 CoreAPI>=2.3.3
 CoreAPI-CLI>=1.0.9
-Markdown>=3.4.1
-DjangoRESTFramework-JSONAPI>=6.0.0
+Markdown>=3.4.3
 DRF-Nested-Routers>=0.93.4
-Django-PolyModels>=1.7.0
-Django-Typed-Models>=0.12.0
+Django-PolyModels>=1.8.0
+Django-Typed-Models>=0.13.0
 HAL-Codec>=1.0.2
 JSONHyperSchema-Codec>=1.0.3
 OpenAPI-Codec>=1.3.2
 JSONSchema>=4.17.3
-Pydantic>=1.10.5
-HTTPie>=3.2.1
-Django-Filter>=22.1
+Pydantic>=1.10.9
+HTTPie>=3.2.2
+Django-Filter>=23.2
 DjangoRESTFramework-Filters>=1.0.0.dev2
 Django-Guardian>=2.4.0
 Rules>=3.3
-Django-Debug-Toolbar>=3.8.1
+Django-Debug-Toolbar>=4.1.0
 Django-Query-Profiler>=0.9
 Django-Silk>=5.0.3
-Kolo>=2.4.2
+Kolo>=2.9.4
 Django-Annoying>=0.10.6
 Django-Choices>=1.7.2
 Django-Compressor>=4.3.1
-Django-Configurations>=2.4
+Django-Configurations>=2.4.1
 Django-Crispy-Forms>=2.0
-Django-Environ>=0.9.0
-Django-Extensions>=3.2.1
+Django-Environ>=0.10.0
+Django-Extensions>=3.2.3
 Django-JSON-Widget>=1.1.1
-Django-LocalFlavor>=3.1
+Django-LocalFlavor>=4.0
 Django-Nested-InLines>=0.1
 Django-Storages>=1.13.2
-Django-Query-Graph>=0.0.0.dev1
-Dj-Util>=0.0.0.dev1
-Django-CORS-Headers>=3.10
-Django-HTMX>=1.14.0
-Django-Plotly-Dash>=1.7
-Dash-Bootstrap-Components>=0.13
+Django-Query-Graph>=23.6.14
+Dju>=23.6.14
+Django-CORS-Headers>=4.1.0
+Django-HTMX>=1.15.0
+Django-Plotly-Dash>=2.2.1
+Dash-Bootstrap-Components>=1.4.1
 DPD-Static-Support>=0.0.5
-Django-Bootstrap4>=22.3
+Django-Bootstrap4>=23.1
 WhiteNoise>=6.4.0
-Flask<2.2,>=2.1
-Werkzeug<2.1,>=2.0
-Gradio>=3.19.1
-Streamlit>=1.19.0
-Watchdog>=2.3.0
+Gradio>=3.34.0
+Gradio-Tools>=0.0.9
+Streamlit>=1.23.1
+Watchdog>=3.0.0
 MariaDB-DynCol>=3.6.1
 Django-MySQL>=4.9.0
 MySQLClient>=2.1.1
-MySQL-Connector-Python>=8.0.32
-PsycoPG2-binary>=2.9.5
-ASGIRef>=3.6.0
-Channels>=2.4
-Daphne>=2.5
+MySQL-Connector-Python>=8.0.33
+PsycoPG>=3.1.9
+PsycoPG2-binary>=2.9.6
+ASGIRef>=3.7.2
+Channels>=4.0.0
+Daphne>=4.0.0
 GUnicorn>=20.1.0
 H11>=0.9
 Hypercorn>=0.14.3
-Quart>=0.17
-Starlette>=0.25.0
-Uvicorn>=0.20.0
+Quart>=0.18.4
+Starlette>=0.28.0
+Uvicorn>=0.22.0
 CLICK>=8.1.3
 Colored>=1.4.4
 Jupyter>=1.0.0
+S3FS>=2023.6.0
+ADLFS>=2023.4.0
+GCSFS>=2023.6.0
+GDriveFS>=0.14.13
+DropboxDriveFS>=1.3.1
+ReactPy>=1.0.0
+ReactPy-Django>=3.1.0
+ReactPy-Jupyter>=0.9.5
 GitPython>=3.1.31
-Ruamel.YAML>=0.17.21
-PSUtil>=5.9.4
+Loguru>=0.7.0
+PSUtil>=5.9.5
 Python-DateUtil>=2.8.2
 Python-DotEnv>=1.0.0
-PyTZ>=2022.7.1
-Requests>=2.28.2
-Tqdm>=4.64.1
+PyTZ>=2023.3
+Requests>=2.31.0
+Ruamel.YAML>=0.17.31
+Tqdm>=4.65.0
 
 [:python_version < "3.11"]
-NumBa>=0.56.4
-Ray>=1.13.0
-Kedro>=0.18.5
-Torch>=1.13.1
-TorchAudio>=0.13.1
-TorchText>=0.14.1
-TorchVision>=0.14.1
-TIMM>=0.6.12
+Kedro>=0.18.10
+Ray>=2.5.0
 Giotto-TDA>=0.6.0
-SHAP>=0.41.0
+CausalNex>=0.12.0
+Django-ForestAdmin>=1.5.0
+
+[:sys_platform != "darwin"]
+TensorFlow>=2.12.0
+
+[:sys_platform == "darwin"]
+TensorFlow-MacOS>=2.12.0
+TensorFlow-Metal>=1.0.1
 
 [build]
 Build>=0.10.0
 
 [dev]
-Commitizen>=2.42.1
-Pre-Commit>=3.1.1
+Commitizen>=3.3.0
+Pre-Commit>=3.3.3
 
 [doc]
-Sphinx>=6.1.3
+Sphinx>=7.0.1
 Sphinx-AutoBuild>=2021.3.14
 SphinxContrib-JSMath>=1.0.1
 CommonMark>=0.9.1
 ReCommonMark>=0.7.1
 
 [lint]
-Bandit>=1.7.4
+Bandit>=1.7.5
 Flake8>=6.0.0
-MyPy>=1.0.0
+MyPy>=1.3.0
 PyCodeStyle>=2.10.0
 PyDocStyle>=6.3.0
 PyLama>=8.4.1
-PyLint>=2.16.1
+PyLint>=2.17.4
+ReactPy-Flake8>=0.7.0
 
 [publish]
 Twine>=4.0.2
 
 [test]
 Nose>=1.3.7
-Nose2>=0.12.0
-PyTest>=7.2.1
-PyTest-Cov>=4.0.0
+Nose2>=0.13.0
+PyTest>=7.3.2
+PyTest-Cov>=4.1.0
 UnitTest2>=1.1.0
 
 [viz]
-Altair>=4.2.2
-Bokeh>=3.0.3
-Dash>=1.20
+Altair>=5.0.1
+Bokeh>=3.1.1
+Dash>=2.9
 Dash-DAQ>=0.5.0
-PlotLy>=5.13.0
-PlotNine>=0.10.1
+PlotLy>=5.15.0
+PlotNine>=0.12.1
 Seaborn>=0.12.2
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/admin.py` & `Djaizz-23.6.14.0/src/djaizz/data/admin.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/api/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/apps.py` & `Djaizz-23.6.14.0/src/djaizz/data/apps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py` & `Djaizz-23.6.14.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py` & `Djaizz-23.6.14.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/migrations/0003_Django4.py` & `Djaizz-23.6.14.0/src/djaizz/data/migrations/0003_Django4.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/audio.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/audio.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/base.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/csv.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/csv.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/hdf.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/hdf.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/image.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/image.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/json.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/json.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/live_api.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/live_api.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/numpy.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/numpy.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/orc.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/orc.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/pandas.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/pandas.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/parquet.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/parquet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/text.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/text.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/tfrecord.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/tfrecord.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/data/models/video.py` & `Djaizz-23.6.14.0/src/djaizz/data/models/video.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/admin.py` & `Djaizz-23.6.14.0/src/djaizz/model/admin.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/api/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/apps.py` & `Djaizz-23.6.14.0/src/djaizz/model/apps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/migrations/0001_AIModel.py` & `Djaizz-23.6.14.0/src/djaizz/model/migrations/0001_AIModel.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py` & `Djaizz-23.6.14.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py` & `Djaizz-23.6.14.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/migrations/0004_CloudAIService.py` & `Djaizz-23.6.14.0/src/djaizz/model/migrations/0004_CloudAIService.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/migrations/0005_GoogleTranslate.py` & `Djaizz-23.6.14.0/src/djaizz/model/migrations/0005_GoogleTranslate.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/migrations/0006_Django4.py` & `Djaizz-23.6.14.0/src/djaizz/model/migrations/0006_Django4.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/base.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Djaizz base AIModel class."""
 
 
 from abc import abstractmethod
 from json.decoder import JSONDecoder
 from sys import version_info
 from typing import Any, Optional
-from typing import Dict, List   # Py3.9+: use generic types
 
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db.models.fields import CharField
 from django.db.models.fields.json import JSONField
 from django.utils.functional import classproperty
 
 from polymorphic.base import PolymorphicModelBase
@@ -100,49 +99,49 @@
         # pylint: disable=no-self-argument
         """Generate AIModel class's subclasses."""
         for subclass in cls.__subclasses__():
             yield subclass
             yield from subclass._subclasses
 
     @classproperty
-    def subclasses(cls) -> List[PolymorphicModelBase]:   # noqa: N805
+    def subclasses(cls) -> list[PolymorphicModelBase]:   # noqa: N805
         # pylint: disable=no-self-argument
         """List of AIModel class's subclasses."""
         return list(cls._subclasses)
 
     @classproperty
-    def subclass_names(cls) -> List[str]:   # noqa: N805
+    def subclass_names(cls) -> list[str]:   # noqa: N805
         # pylint: disable=no-self-argument
         """List of AIModel class's subclasses' names."""
         return [s.__name__
                 for s in cls._subclasses   # pylint: disable=not-an-iterable
                 ]
 
     @classproperty
-    def subclasses_by_name(cls) -> Dict[str, PolymorphicModelBase]:   # noqa: E501,N805
+    def subclasses_by_name(cls) -> dict[str, PolymorphicModelBase]:   # noqa: E501,N805
         # pylint: disable=no-self-argument
         """Return AIModel class's subclass-by-name dictionary.
 
         Dictionary mapping from AIModel class's subclasses' names
         to such subclasses.
         """
         return {s.__name__: s
                 for s in cls._subclasses   # pylint: disable=not-an-iterable
                 }
 
     @classproperty
-    def subclass_full_qual_names(cls) -> List[str]:   # noqa: N805
+    def subclass_full_qual_names(cls) -> list[str]:   # noqa: N805
         # pylint: disable=no-self-argument
         """List of AIModel class's subclasses' fully-qualified names."""
         return [full_qual_name(s)
                 for s in cls._subclasses   # pylint: disable=not-an-iterable
                 ]
 
     @classproperty
-    def subclasses_by_full_qual_name(cls) -> Dict[str, PolymorphicModelBase]:   # noqa: E501,N805
+    def subclasses_by_full_qual_name(cls) -> dict[str, PolymorphicModelBase]:   # noqa: E501,N805
         # pylint: disable=no-self-argument
         """Return AIModel class's subclass-by-fully-qualified name dict.
 
         Dictionary mapping from AIModel class's subclasses'
         fully-qualified names to such subclasses.
         """
         return {full_qual_name(s): s
@@ -389,36 +388,36 @@
         # pylint: disable=no-self-argument
         """Return the AIModel class's Gradio Interface."""
         return Interface(
             fn=cls.predict,
             # (Callable) - the function to wrap an interface around.
 
             inputs=[],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='AI Model Output'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -502,15 +501,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/base.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/cloud_ai_svc/google/translation.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Djaizz Google Cloud AI Translation Service model classes."""
 
 
 from sys import version_info
 from typing import Union
-from typing import List   # Py3.9+: use generic types
 
 from django.utils.functional import classproperty
 
 from googletrans.client import Translator
 from googletrans.constants import LANGUAGES
 
 from gradio.interface import Interface
@@ -52,15 +51,15 @@
     def load(self) -> None:
         """Load Google Translate Client."""
         if not self.client:
             self.client = Translator()
 
     def predict(self,
                 text_or_texts: Union[str, Sequence[str]],
-                src: str = 'auto', dest: str = 'en') -> Union[str, List[str]]:
+                src: str = 'auto', dest: str = 'en') -> Union[str, list[str]]:
         # pylint: disable=arguments-differ
         """Translate."""
         self.load()
 
         return (self.client.translate(text=text_or_texts,
                                       dest=dest, src=src).text
                 if isinstance(text_or_texts, str)
@@ -87,36 +86,36 @@
                                   default='auto',
                                   label='Source Language'),
 
                     DropdownInput(choices=languages,
                                   type='value',
                                   default='english',
                                   label='Destination Language')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=TextboxOutput(type='str', label='Translated Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -199,15 +198,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/base.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Machine Learning Model base classes."""
 
 
 from sys import version_info
-from typing import Dict   # Py3.9+: use generic types
 from typing import Any
 
 from django.db.models.fields import CharField
 
 from djaizz.util import import_obj
 
 from ..base import _AIModelWithArtifactFilesABC
@@ -52,14 +51,14 @@
 
     @property
     def loader(self) -> callable:
         """Loader method to load the Model's native object."""
         return import_obj(self.loader_module_and_qualname)
 
     @property
-    def init_params(self) -> Dict[str, Any]:
+    def init_params(self) -> dict[str, Any]:
         """Extract initialization parameters from in-database params JSON."""
         return ({} if self.params is None else self.params).get('__init__', {})
 
     def load(self) -> None:
         if not self.native_obj:
             self.native_obj = self.loader(**self.init_params)
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/audio_classification.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Audio Classifier Model class."""
 
 
 from sys import version_info
-from typing import Dict, List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Audio as AudioInput,
                            Slider as SliderInput)
@@ -25,15 +24,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceAudioClassifier',)
 
 
 AudioClassificationInputType = Union[numpy.ndarray, str]
-AudioClassificationOutputType = Dict[str, float]
+AudioClassificationOutputType = dict[str, float]
 
 
 class PreTrainedHuggingFaceAudioClassifier(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Audio Classifier Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -52,21 +51,21 @@
 
     def predict(self,
                 audio_or_audios:
                     Union[AudioClassificationInputType,
                           Sequence[AudioClassificationInputType]],
                 n_labels: int = 5) \
             -> Union[AudioClassificationOutputType,
-                     List[AudioClassificationOutputType]]:
+                     list[AudioClassificationOutputType]]:
         # pylint: disable=arguments-differ
         """Classify Audio(s)."""
         single_audio: bool = isinstance(audio_or_audios, (numpy.ndarray, str))
 
         if not (single_audio or isinstance(audio_or_audios, list)):
-            audio_or_audios: List[AudioClassificationInputType] = \
+            audio_or_audios: list[AudioClassificationInputType] = \
                 list(audio_or_audios)
 
         self.load()
 
         output = self.native_obj(inputs=audio_or_audios, top_k=n_labels)
 
         return ({i['label']: i['score'] for i in output}
@@ -77,15 +76,15 @@
     @classproperty
     def gradio_ui(cls) -> Interface:   # noqa: N805
         # pylint: disable=no-self-argument
         """Gradio Interface."""
         def _predict(self,
                      sampling_rate_and_double_channel_audio_array:
                      tuple[int, numpy.ndarray],
-                     n_labels: int = 5) -> Dict[str, float]:
+                     n_labels: int = 5) -> dict[str, float]:
             _sampling_rate, double_channel_audio_array = \
                 sampling_rate_and_double_channel_audio_array
 
             return cls.predict(
                 self,
                 audio_or_audios=(double_channel_audio_array[:, 0]
                                  .astype(numpy.float32)),
@@ -98,38 +97,38 @@
             inputs=[AudioInput(source='upload',
                                type='numpy',
                                label='Audio to Classify',
                                optional=False),
 
                     SliderInput(minimum=3, maximum=10, step=1, default=5,
                                 label='No. of Labels to Return')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=LabelOutput(num_top_classes=10,
                                 type='auto',
                                 label='Audio Classification'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -210,15 +209,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/base.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/image_classification.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/image_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Image Classifier Model class."""
 
 
 from sys import version_info
-from typing import Dict, List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Image as ImageInput,
                            Slider as SliderInput)
@@ -25,15 +24,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceImageClassifier',)
 
 
 ImageClassificationInputType = Union[str, Image]
-ImageClassificationOutputType = Dict[str, float]
+ImageClassificationOutputType = dict[str, float]
 
 
 class PreTrainedHuggingFaceImageClassifier(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Image Classifier Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -51,21 +50,21 @@
         default_related_name: str = 'pretrained_hugging_face_image_classifiers'
 
     def predict(self,
                 image_or_images: Union[ImageClassificationInputType,
                                        Sequence[ImageClassificationInputType]],
                 n_labels: int = 5) \
             -> Union[ImageClassificationOutputType,
-                     List[ImageClassificationOutputType]]:
+                     list[ImageClassificationOutputType]]:
         # pylint: disable=arguments-differ
         """Classify Image(s)."""
         single_img: bool = isinstance(image_or_images, (str, Image))
 
         if not (single_img or isinstance(image_or_images, list)):
-            image_or_images: List[ImageClassificationInputType] = \
+            image_or_images: list[ImageClassificationInputType] = \
                 list(image_or_images)
 
         self.load()
 
         output = self.native_obj(images=image_or_images, top_k=n_labels)
 
         return ({i['label']: i['score'] for i in output}
@@ -88,38 +87,38 @@
                                tool='editor',
                                type='pil',
                                label='Upload an Image to Classify',
                                optional=False),
 
                     SliderInput(minimum=3, maximum=10, step=1, default=5,
                                 label='No. of Labels to Return')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=LabelOutput(num_top_classes=10,
                                 type='auto',
                                 label='Likely ImageNet Classes'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -202,15 +201,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/mask_filling.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Mask Filler Model class."""
 
 
 from sys import version_info
-from typing import Dict, List   # Py3.9+: use generic types
 from typing import Optional, Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Textbox as TextboxInput,
                            Dataframe as DataframeInput,
@@ -24,15 +23,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceMaskFiller',)
 
 
 MaskFillingInputType = str
-MaskFillingOutputType = Dict[str, float]
+MaskFillingOutputType = dict[str, float]
 
 
 class PreTrainedHuggingFaceMaskFiller(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Mask Filler Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -48,23 +47,23 @@
             ValueError(f'*** "{db_table}" DB TABLE NAME TOO LONG ***')
 
         default_related_name: str = 'pretrained_hugging_face_mask_fillers'
 
     def predict(self,
                 text_or_texts: Union[MaskFillingInputType,
                                      Sequence[MaskFillingInputType]],
-                targets: Optional[List[str]] = None,
+                targets: Optional[list[str]] = None,
                 n_labels: int = 5) \
-            -> Union[MaskFillingOutputType, List[MaskFillingOutputType]]:
+            -> Union[MaskFillingOutputType, list[MaskFillingOutputType]]:
         # pylint: disable=arguments-differ
         """Classify Image(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[MaskFillingInputType] = list(text_or_texts)
+            text_or_texts: list[MaskFillingInputType] = list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(text_or_texts,
                                  targets=targets,
                                  top_k=n_labels)
 
@@ -75,18 +74,18 @@
 
     @classproperty
     def gradio_ui(cls) -> Interface:   # noqa: N805
         # pylint: disable=no-self-argument
         """Gradio Interface."""
         def _predict(self,
                      text: str,
-                     targets: Optional[List[str]] = None,
-                     n_labels: int = 5) -> Dict[str, float]:
+                     targets: Optional[list[str]] = None,
+                     n_labels: int = 5) -> dict[str, float]:
             if targets:
-                targets: List[str] = [s for s in targets if s]
+                targets: list[str] = [s for s in targets if s]
 
             return cls.predict(self,
                                text_or_texts=text,
                                targets=targets if targets else None,
                                n_labels=n_labels)
 
         return Interface(
@@ -107,38 +106,38 @@
                                    col_width=100,
                                    default=None,
                                    type='array',
                                    label='Targets'),
 
                     SliderInput(minimum=3, maximum=10, step=1, default=5,
                                 label='No. of Labels to Return')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=LabelOutput(num_top_classes=10,
                                 type='auto',
                                 label='Generated Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -221,15 +220,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/object_detection.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/object_detection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Object Detector Model class."""
 
 
 from sys import version_info
-from typing import Dict, List   # Py3.9+: use generic types
 from typing import Any, Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Image as ImageInput,
                            Slider as SliderInput)
@@ -26,15 +25,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceObjectDetector',)
 
 
 ObjectDetectionInputType = Union[str, Image]
-ObjectDetectionOutputType = List[dict]
+ObjectDetectionOutputType = list[dict]
 
 
 class PreTrainedHuggingFaceObjectDetector(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Object Detector Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -56,34 +55,34 @@
                                        Sequence[ObjectDetectionInputType]],
                 threshold: float = 0.9) \
             -> Union[ObjectDetectionOutputType,
                      Sequence[ObjectDetectionOutputType]]:
         # pylint: disable=arguments-differ
         """Detect Objects from Image(s)."""
         if not isinstance(image_or_images, (str, Image, list)):
-            image_or_images: List[ObjectDetectionInputType] = \
+            image_or_images: list[ObjectDetectionInputType] = \
                 list(image_or_images)
 
         self.load()
 
         return self.native_obj(inputs=image_or_images,   # images=?
                                threshold=threshold)
 
     @classproperty
     def gradio_ui(cls) -> Interface:   # noqa: N805
         # pylint: disable=no-self-argument
         """Gradio Interface."""
         BoundingBoxType = tuple[str, int, int, int, int]   # noqa: N806
 
         def _predict(self, img: Image, threshold: float = 0.9) \
-                -> tuple[Image, List[BoundingBoxType]]:
-            detected_objs: List[Dict[str, Any]] = \
+                -> tuple[Image, list[BoundingBoxType]]:
+            detected_objs: list[dict[str, Any]] = \
                 cls.predict(self, image_or_images=img, threshold=threshold)
 
-            bounding_boxes: List[BoundingBoxType] = []
+            bounding_boxes: list[BoundingBoxType] = []
             for i in detected_objs:
                 box_coords = i['box']
                 bounding_boxes.append((i['label'],
                                        box_coords['xmin'],   # left-x
                                        box_coords['ymin'],   # top-y
                                        box_coords['xmax'],   # right-x
                                        box_coords['ymax']    # bottom-y
@@ -102,40 +101,40 @@
                                tool='editor',
                                type='pil',
                                label=('Upload an Image to Detect Objects'),
                                optional=False),
 
                     SliderInput(minimum=.5, maximum=.9, step=.1, default=.9,
                                 label='Confidence Threshold')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=[ImageOutput(type='pil',
                                  # labeled_segments=True,   # TODO: fix
                                  label='Detected Objects'),
 
                      JSONOutput(label='Detected Objects')],
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -218,15 +217,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/question_answering.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/question_answering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Question Answerer Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Textbox as TextboxInput,
                            Number as NumberInput,
@@ -57,22 +56,22 @@
                                Sequence[QuestionAnswerInputType]],
                 top_k: int = 1,
                 doc_stride: int = 128,
                 max_answer_len: int = 15,
                 max_seq_len: int = 384,
                 max_question_len: int = 64,
                 handle_impossible_answer: bool = False) \
-            -> Union[QuestionAnswerOutputType, List[QuestionAnswerOutputType]]:
+            -> Union[QuestionAnswerOutputType, list[QuestionAnswerOutputType]]:
         # pylint: disable=arguments-differ,too-many-arguments
         """Answer Question(s) based on Text(s)."""
         if not isinstance(question, (str, list)):
-            question: List[QuestionAnswerInputType] = list(question)
+            question: list[QuestionAnswerInputType] = list(question)
 
         if not isinstance(context, (str, list)):
-            context: List[QuestionAnswerInputType] = list(context)
+            context: list[QuestionAnswerInputType] = list(context)
 
         self.load()
 
         return self.native_obj(
             question=question, context=context, top_k=top_k,
             doc_stride=doc_stride,
             max_answer_len=max_answer_len,
@@ -121,36 +120,36 @@
                     NumberInput(default=384, label='Max Sequence Length'),
 
                     NumberInput(default=64, label='Max Question Length'),
 
                     CheckboxInput(default=False,
                                   label='Handle Impossible Answer?')],
 
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Likely Answer(s)'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -234,15 +233,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Djaizz Pre-Trained Hugging Face Speech Recognizer Model class."""
 
 
 from sys import version_info
 from tempfile import NamedTemporaryFile
 from typing import Union
-from typing import List   # Py3.9+: use generic types
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import Audio as AudioInput
 from gradio.outputs import Textbox as TextboxOutput
 
@@ -52,22 +51,22 @@
         default_related_name = 'pretrained_hugging_face_speech_recognizers'
 
     def predict(self,
                 speech_or_speeches:
                     Union[SpeechRecognitionInputType,
                           Sequence[SpeechRecognitionInputType]]) \
             -> Union[SpeechRecognitionOutputType,
-                     List[SpeechRecognitionOutputType]]:
+                     list[SpeechRecognitionOutputType]]:
         # pylint: disable=arguments-differ
         """Recognize Speech(es)."""
         single_speech: bool = isinstance(speech_or_speeches, (numpy.ndarray,
                                                               str))
 
         if not (single_speech or isinstance(speech_or_speeches, list)):
-            speech_or_speeches: List[SpeechRecognitionInputType] = \
+            speech_or_speeches: list[SpeechRecognitionInputType] = \
                 list(speech_or_speeches)
 
         self.load()
 
         output = self.native_obj(inputs=speech_or_speeches)
 
         return (output['text']
@@ -85,36 +84,36 @@
             fn=_predict,
             # (Callable) - the function to wrap an interface around.
 
             inputs=AudioInput(source='microphone',
                               type='file',
                               label='Recorded Speech to Transcribe',
                               optional=False),
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=TextboxOutput(type='str', label='Transcribed Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -197,15 +196,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Table Question Answerer Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Dataframe as DataframeInput,
                            Textbox as TextboxInput,
@@ -57,15 +56,15 @@
     def predict(self,
                 table: TableQuestionAnswerInputType,
                 queries: Union[str, Sequence[str]],
                 sequential: bool = False,
                 padding: Union[bool, str] = False,
                 truncation: Union[bool, str] = False) \
             -> Union[TableQuestionAnswerOutputType,
-                     List[TableQuestionAnswerOutputType]]:
+                     list[TableQuestionAnswerOutputType]]:
         # pylint: disable=arguments-differ,too-many-arguments
         """Answer Question(s) on a Tabular Data Set."""
         self.load()
 
         return self.native_obj(table=table, query=queries,
                                sequential=sequential,
                                padding=padding, truncation=truncation)
@@ -96,36 +95,36 @@
                                  label='Query'),
 
                     CheckboxInput(default=False, label='Sequential?'),
 
                     CheckboxInput(default=False, label='Padding?'),
 
                     CheckboxInput(default=False, label='Truncation?')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Likely Answer(s)'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -209,15 +208,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Text-to-Text Generator Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Textbox as TextboxInput,
                            Checkbox as CheckboxInput)
@@ -23,15 +22,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceText2TextGenerator',)
 
 
 Text2TextGenerationInputType = str
-Text2TextGenerationOutputType = Union[str, List[int]]
+Text2TextGenerationOutputType = Union[str, list[int]]
 
 
 class PreTrainedHuggingFaceText2TextGenerator(
         PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Text-to-Text Generator Model class."""
 
@@ -54,21 +53,21 @@
                 text_or_texts: Union[Text2TextGenerationInputType,
                                      Sequence[Text2TextGenerationInputType]],
                 return_tensors: bool = False,
                 return_text: bool = True,
                 clean_up_tokenization_spaces: bool = True,
                 **generate_kwargs) \
             -> Union[Text2TextGenerationOutputType,
-                     List[Text2TextGenerationOutputType]]:
+                     list[Text2TextGenerationOutputType]]:
         # pylint: disable=arguments-differ
         """Generate Text-to-Text."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[Text2TextGenerationInputType] = \
+            text_or_texts: list[Text2TextGenerationInputType] = \
                 list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(
             text_or_texts,
             return_tensors=return_tensors,
@@ -106,36 +105,36 @@
                                  numeric=False,
                                  type='str',
                                  label='Text to Generate from'),
 
                     CheckboxInput(default=False, label='Return Tensors?'),
 
                     CheckboxInput(default=True, label='Return Text?')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Generated Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -219,15 +218,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text_classification.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Text Classifier Model class."""
 
 
 from sys import version_info
-from typing import Dict, List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import Textbox as TextboxInput
 from gradio.outputs import Label as LabelOutput
@@ -22,15 +21,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceTextClassifier',)
 
 
 TextClassificationInputType = str
-TextClassificationOutputType = Dict[str, float]
+TextClassificationOutputType = dict[str, float]
 
 
 class PreTrainedHuggingFaceTextClassifier(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Text Classifier Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -53,15 +52,15 @@
             -> Union[TextClassificationOutputType,
                      Sequence[TextClassificationOutputType]]:
         # pylint: disable=arguments-differ
         """Classify Text(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[TextClassificationInputType] = \
+            text_or_texts: list[TextClassificationInputType] = \
                 list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(text_or_texts,
                                  return_all_scores=True,
                                  function_to_apply=None)
@@ -81,38 +80,38 @@
 
             inputs=TextboxInput(lines=10,
                                 placeholder='Text to Classify',
                                 default='',
                                 numeric=False,
                                 type='str',
                                 label='Text to Classify'),
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=LabelOutput(num_top_classes=10,
                                 type='auto',
                                 label='Likely Text Classes'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -195,15 +194,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text_generation.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Text Generator Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Optional, Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Textbox as TextboxInput,
                            Checkbox as CheckboxInput)
@@ -23,15 +22,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceTextGenerator',)
 
 
 TextGenerationInputType = str
-TextGenerationOutputType = Union[str, List[int]]
+TextGenerationOutputType = Union[str, list[int]]
 
 
 class PreTrainedHuggingFaceTextGenerator(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Text Generator Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -53,21 +52,21 @@
                                      Sequence[TextGenerationInputType]],
                 return_tensors: bool = False,
                 return_text: bool = True,
                 return_full_text: bool = True,
                 clean_up_tokenization_spaces: bool = True,
                 prefix: Optional[str] = None,
                 **generate_kwargs) \
-            -> Union[TextGenerationOutputType, List[TextGenerationOutputType]]:
+            -> Union[TextGenerationOutputType, list[TextGenerationOutputType]]:
         # pylint: disable=arguments-differ,too-many-arguments
         """Generate Text(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[TextGenerationInputType] = list(text_or_texts)
+            text_or_texts: list[TextGenerationInputType] = list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(
             text_inputs=text_or_texts,
             return_tensors=return_tensors,
             return_text=return_text,
@@ -121,36 +120,36 @@
 
                     TextboxInput(lines=1,
                                  placeholder='Generated Text Prefix',
                                  default='',
                                  numeric=False,
                                  type='str',
                                  label='Generated Text Prefix')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Generated Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -234,15 +233,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/text_summarization.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Text Summarizer Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Textbox as TextboxInput,
                            Checkbox as CheckboxInput)
@@ -23,15 +22,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceTextSummarizer',)
 
 
 TextSummarizationInputType = str
-TextSummarizationOutputType = Union[str, List[int]]
+TextSummarizationOutputType = Union[str, list[int]]
 
 
 class PreTrainedHuggingFaceTextSummarizer(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Text Summarizer Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -52,21 +51,21 @@
                 text_or_texts: Union[TextSummarizationInputType,
                                      Sequence[TextSummarizationInputType]],
                 return_text: bool = True,
                 return_tensors: bool = False,
                 clean_up_tokenization_spaces: bool = True,
                 **generate_kwargs) \
             -> Union[TextSummarizationOutputType,
-                     List[TextSummarizationOutputType]]:
+                     list[TextSummarizationOutputType]]:
         # pylint: disable=arguments-differ
         """Summarize Text(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[TextSummarizationInputType] = \
+            text_or_texts: list[TextSummarizationInputType] = \
                 list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(
             inputs=text_or_texts,   # documents=?
             return_text=return_text,
@@ -105,36 +104,36 @@
                                  label='Text to Summarize'),
 
                     CheckboxInput(default=True, label='Return Text?'),
 
                     CheckboxInput(default=False, label='Return Tensors?'),
 
                     CheckboxInput(default=True, label='Clean Up Spaces?')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Summary Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -217,15 +216,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/token_classification.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/token_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Token Classifier Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import Textbox as TextboxInput
 from gradio.outputs import JSON as JSONOutput   # noqa: N811
@@ -22,15 +21,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceTokenClassifier',)
 
 
 TokenClassificationInputType = str
-TokenClassificationOutputType = List[dict]
+TokenClassificationOutputType = list[dict]
 
 
 class PreTrainedHuggingFaceTokenClassifier(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Token Classifier Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -53,15 +52,15 @@
             -> Union[TokenClassificationOutputType,
                      Sequence[TokenClassificationOutputType]]:
         # pylint: disable=arguments-differ
         """Classify Tokens in Text(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[TokenClassificationInputType] = \
+            text_or_texts: list[TokenClassificationInputType] = \
                 list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(inputs=text_or_texts)
 
         return ([{k: (float(v) if k == 'score' else v) for k, v in d.items()}
@@ -83,36 +82,36 @@
             inputs=TextboxInput(lines=10,
                                 placeholder=('Text from which '
                                              'to Recognize Tokens'),
                                 default='',
                                 numeric=False,
                                 type='str',
                                 label=('Text from which to Recognize Tokens')),
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Recognized Tokens'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -196,15 +195,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/translation.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/translation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Translator Model class."""
 
 
 from sys import version_info
-from typing import List   # Py3.9+: use generic types
 from typing import Optional, Union
 
 from django.utils.functional import classproperty
 
 from googletrans.constants import LANGUAGES
 
 from gradio.interface import Interface
@@ -26,15 +25,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceTranslator',)
 
 
 TranslationInputType = str
-TranslationOutputType = Union[str, List[int]]
+TranslationOutputType = Union[str, list[int]]
 
 
 class PreTrainedHuggingFaceTranslator(PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Translator Model class."""
 
     class Meta(PreTrainedHuggingFaceTransformer.Meta):
@@ -56,21 +55,21 @@
                                      Sequence[TranslationInputType]],
                 return_tensors: bool = False,
                 return_text: bool = True,
                 clean_up_tokenization_spaces: bool = True,
                 src_lang: Optional[str] = None,
                 tgt_lang: Optional[str] = None,
                 **generate_kwargs) \
-            -> Union[TranslationOutputType, List[TranslationOutputType]]:
+            -> Union[TranslationOutputType, list[TranslationOutputType]]:
         # pylint: disable=arguments-differ,too-many-arguments
         """Translate Text(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[TranslationInputType] = list(text_or_texts)
+            text_or_texts: list[TranslationInputType] = list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(
             inputs=text_or_texts,   # documents=?
             return_tensors=return_tensors,
             return_text=return_text,
@@ -122,36 +121,36 @@
                                   default='en',
                                   label='Source Language'),
 
                     DropDownInput(choices=languages,
                                   type='value',
                                   default='fr',
                                   label='Target Language')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=JSONOutput(label='Translated Text'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -234,15 +233,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Djaizz Pre-Trained Hugging Face Zero-Shot Classifier Model class."""
 
 
 from sys import version_info
-from typing import Dict, List   # Py3.9+: use generic types
 from typing import Union
 
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import (Textbox as TextboxInput,
                            Dataframe as DataframeInput,
@@ -24,15 +23,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedHuggingFaceZeroShotClassifier',)
 
 
 ZeroShotClassificationInputType = str
-ZeroShotClassificationOutputType = Dict[str, float]
+ZeroShotClassificationOutputType = dict[str, float]
 
 
 class PreTrainedHuggingFaceZeroShotClassifier(
         PreTrainedHuggingFaceTransformer):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Hugging Face Zero-Shot Classifier Model class."""
 
@@ -51,25 +50,25 @@
 
         default_related_name = 'pretrained_hugging_face_zero_shot_classifiers'
 
     def predict(self,
                 text_or_texts:
                     Union[ZeroShotClassificationInputType,
                           Sequence[ZeroShotClassificationInputType]],
-                candidate_labels: List[str],
+                candidate_labels: list[str],
                 hypothesis_template: str = 'This example is {}.',
                 multi_label: bool = False) \
             -> Union[ZeroShotClassificationOutputType,
-                     List[ZeroShotClassificationOutputType]]:
+                     list[ZeroShotClassificationOutputType]]:
         # pylint: disable=arguments-differ
         """Zero-Shot Classification of Text(s)."""
         single_text: bool = isinstance(text_or_texts, str)
 
         if not (single_text or isinstance(text_or_texts, list)):
-            text_or_texts: List[ZeroShotClassificationInputType] = \
+            text_or_texts: list[ZeroShotClassificationInputType] = \
                 list(text_or_texts)
 
         self.load()
 
         output = self.native_obj(sequences=text_or_texts,
                                  candidate_labels=candidate_labels,
                                  hypothesis_template=hypothesis_template,
@@ -113,38 +112,38 @@
                                  placeholder='Hypothesis Format',
                                  default='This example is {}.',
                                  numeric=False,
                                  type='str',
                                  label='Hypothesis Format'),
 
                     CheckboxInput(default=False, label='Multi-Label?')],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=LabelOutput(num_top_classes=10,
                                 type='auto',
                                 label='Label Probabilities'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -228,15 +227,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/base.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Djaizz Pre-Trained Keras Image Classification Model class."""
 
 
 from io import BytesIO
 from sys import version_info
 from typing import Union
-from typing import Dict, List   # Py3.9+: use generic types
 
 from django.db.models.fields import CharField
 from django.utils.functional import classproperty
 
 from gradio.interface import Interface
 from gradio.inputs import Image as ImageInput, Slider as SliderInput
 from gradio.outputs import Label as LabelOutput
@@ -29,15 +28,15 @@
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('PreTrainedKerasImageNetClassifier',)
 
 
 ImageClassificationInputType = Union[str, BytesIO, Image.Image, numpy.ndarray]
-ImageClassificationOutputType = Dict[str, float]
+ImageClassificationOutputType = dict[str, float]
 
 
 class PreTrainedKerasImageNetClassifier(_PreTrainedMLModelABC):
     # pylint: disable=abstract-method,too-many-ancestors
     """Djaizz Pre-Trained Keras Image Classification Model class."""
 
     preprocessor_module_and_qualname: CharField = \
@@ -113,22 +112,22 @@
         return import_obj(self.preprocessor_module_and_qualname)
 
     def predict(self,
                 image_or_images: Union[ImageClassificationInputType,
                                        Sequence[ImageClassificationInputType]],
                 n_labels: int = 5) \
             -> Union[ImageClassificationOutputType,
-                     List[ImageClassificationOutputType]]:
+                     list[ImageClassificationOutputType]]:
         # pylint: disable=arguments-differ
         """Classify Image(s)."""
         single_img: bool = isinstance(image_or_images, (str, BytesIO,
                                                         Image.Image,
                                                         numpy.ndarray))
 
-        imgs: List[ImageClassificationInputType] = ([image_or_images]
+        imgs: list[ImageClassificationInputType] = ([image_or_images]
                                                     if single_img
                                                     else image_or_images)
 
         # construct 4D array of images' data fitted into standardized size
         fitted_img_batch_arr: numpy.ndarray = \
             numpy.vstack([self._image_to_4d_array(image=img) for img in imgs])
 
@@ -139,15 +138,15 @@
         # load native model object & predict
         self.load()
 
         pred_prob_arr: numpy.ndarray = \
             self.native_obj.predict(x=preprocessed_fitted_img_batch_arr)
 
         # decode predictions & return JSON-serializable dict
-        decoded_preds: List[Dict[str, float]] = [{tup[1]: float(tup[2])
+        decoded_preds: list[dict[str, float]] = [{tup[1]: float(tup[2])
                                                   for tup in decoded_pred}
                                                  for decoded_pred in
                                                  decode_predictions(
                                                      preds=pred_prob_arr,
                                                      top=n_labels)]
 
         return decoded_preds[0] if single_img else decoded_preds
@@ -167,38 +166,38 @@
                                tool='editor',
                                type='pil',
                                label='Upload an Image to Classify',
                                optional=False),
 
                     SliderInput(minimum=3, maximum=10, step=1, default=5,
                                 label=('No. of ImageNet Labels to Return'))],
-            # (Union[str, List[Union[str, InputComponent]]]) -
+            # (Union[str, list[Union[str, InputComponent]]]) -
             # a single Gradio input component,
             # or list of Gradio input components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of input components should match
             # the number of parameters in fn.
 
             outputs=LabelOutput(num_top_classes=10,
                                 type='auto',
                                 label='Likely ImageNet Labels'),
-            # (Union[str, List[Union[str, OutputComponent]]]) -
+            # (Union[str, list[Union[str, OutputComponent]]]) -
             # a single Gradio output component,
             # or list of Gradio output components.
             # Components can either be passed as instantiated objects,
             # or referred to by their string shortcuts.
             # The number of output components should match
             # the number of values returned by fn.
 
             verbose=True,
             # (bool) - whether to print detailed information during launch.
 
             examples=None,
-            # (Union[List[List[Any]], str]) - sample inputs for the function;
+            # (Union[list[list[Any]], str]) - sample inputs for the function;
             # if provided, appears below the UI components and can be used
             # to populate the interface.
             # Should be nested list, in which the outer list consists of
             # samples and each inner list consists of an input
             # corresponding to each input component.
             # A string path to a directory of examples can also be provided.
             # If there are multiple input components and a directory
@@ -281,15 +280,15 @@
             # to take a screenshot of the interface.
 
             allow_flagging=False,
             # (bool) - if False, users will not see a button
             # to flag an input and output.
 
             flagging_options=None,
-            # (List[str]) - if not None, provides options a user must select
+            # (list[str]) - if not None, provides options a user must select
             # when flagging.
 
             encrypt=False,
             # (bool) - If True, flagged data will be encrypted
             # by key provided by creator at launch
 
             show_tips=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/skl.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/skl.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/models/ml/torch/base.py` & `Djaizz-23.6.14.0/src/djaizz/model/models/ml/torch/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py` & `Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/scripts/setup_pretrained_keras_models.py` & `Djaizz-23.6.14.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/urls.py` & `Djaizz-23.6.14.0/src/djaizz/model/urls.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/model/views.py` & `Djaizz-23.6.14.0/src/djaizz/model/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Djaizz Model Views."""
 
 
 from inspect import isclass
 from typing import Literal, Union
-from typing import List   # Py3.9+: use generic types
 
 from django.http.request import HttpRequest
 from django.http.response import Http404, HttpResponse, HttpResponseRedirect
 from django.shortcuts import redirect, render
 
 from django_plotly_dash.dash_wrapper import DjangoDash
 from django_plotly_dash.models import DashApp, StatelessApp
@@ -40,15 +39,15 @@
                 name_or_uuid=model_class_or_instance_name_or_uuid)
 
         except AIModel.DoesNotExist as ai_model_does_not_exist:
             raise Http404('*** MODEL INSTANCE ' +
                           model_class_or_instance_name_or_uuid +
                           ' NOT FOUND ***') from ai_model_does_not_exist
 
-        model_names_or_uuids: List[str] = model.names_or_uuids
+        model_names_or_uuids: list[str] = model.names_or_uuids
 
     if ui_type == 'dash':
         if not isinstance(dash_ui := model.dash_ui, DjangoDash):
             raise Http404(f'*** {model} DOES NOT HAVE A DASH UI ***')
 
         # if `model` is an AIModel instance, then render the view for its class
         if isinstance(model, AIModel):
@@ -106,15 +105,15 @@
                 # from your computer for the interface.
 
                 debug=False,
                 # (bool) - if True, and the interface was launched
                 # from Google Colab, prints the errors in the cell output.
 
                 auth=None,
-                # (Callable, Union[Tuple[str, str], List[Tuple[str, str]]]) -
+                # (Callable, Union[tuple[str, str], list[tuple[str, str]]]) -
                 # If provided, username and password
                 # (or list of username-password tuples)
                 # required to access interface.
                 # Can also provide function that takes username and password
                 # and returns True if valid login.
 
                 auth_message=None,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/urls.py` & `Djaizz-23.6.14.0/src/djaizz/urls.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/util/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/cli/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/util/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .aws_eb import djaizz_aws_eb
 from .deps import capped_deps
 
 
 @click.group(name='djaizz',
              cls=click.Group,
              commands={'aws-eb': djaizz_aws_eb,
-                       'capped-deps': capped_deps
+                       'capped-deps': capped_deps,
                        },
              invoke_without_command=False,
              no_args_is_help=True,
              subcommand_metavar='DJAI_SUB_COMMAND',
              chain=False,
              help='Djaizz CLI >>>',
              epilog='^^^ Djaizz CLI',
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/cli/_server_files/asgi.py` & `Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/asgi.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/cli/_server_files/wsgi.py` & `Djaizz-23.6.14.0/src/djaizz/util/cli/_server_files/wsgi.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/cli/aws_eb/__init__.py` & `Djaizz-23.6.14.0/src/djaizz/util/cli/aws_eb/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,74 @@
 """Djaizz AWS Elastic Beanstalk CLI."""
 
 
 from contextlib import AbstractContextManager
 import os
 from pathlib import Path
-import shutil
+from pprint import pprint
+from shutil import copyfile, copytree, ignore_patterns
 from typing import Optional
-from typing import List   # Py3.9+: use built-in
 
 import click
+from ruamel import yaml
 
 from ..run_cmd import run_cmd
 
 
 _DJAI_AWS_EB_CLI_UTIL_DIR_PATH: Path = Path(__file__).parent
 
 
+_EC2_INSTANCE_TYPES_FILE_NAME: str = 'EC2-Instance-Types.yml'
+
+with open(file=_DJAI_AWS_EB_CLI_UTIL_DIR_PATH / _EC2_INSTANCE_TYPES_FILE_NAME,
+          mode='rt',
+          buffering=-1,
+          encoding='utf-8',
+          errors='raise',
+          newline=None,
+          closefd=True,
+          opener=None) as f:
+    _EC2_INSTANCE_TYPES: dict = yaml.safe_load(stream=f, version=None)
+
+
 _EB_EXTENSIONS_DIR_NAME: str = '.ebextensions'
 _PLATFORM_DIR_NAME: str = '.platform'
+_INSTALL_CUDA_SCRIPT_NAME: str = '.Install-CUDA'
 
 
 class ConfigFilesHandling(AbstractContextManager):
     """Handle config/extension files, e.g., `.ebextensions`/`.platform`."""
 
-    def __init__(self, config_dir_name: str, /):
+    def __init__(self, config_dir_name: str, /, *, gpu: Optional[bool] = False):  # noqa: E501
         """Initialize context manager."""
         self.config_dir_name: str = config_dir_name
-        self.config_dir_path: Path = _DJAI_AWS_EB_CLI_UTIL_DIR_PATH / config_dir_name   # noqa: E501
+        self.config_dir_path: Path = _DJAI_AWS_EB_CLI_UTIL_DIR_PATH / config_dir_name  # noqa: E501
+        self.gpu: bool = gpu
 
     def __enter__(self):
         """Add config/extension files."""
-        shutil.copytree(src=self.config_dir_path,
-                        dst=self.config_dir_name,
-                        symlinks=False,
-                        ignore=None,
-                        ignore_dangling_symlinks=False,
-                        dirs_exist_ok=True)
+        copytree(
+            src=self.config_dir_path,
+            dst=self.config_dir_name,
+            symlinks=False,
+            ignore=(None
+                    if self.gpu
+                    else ignore_patterns(_INSTALL_CUDA_SCRIPT_NAME)),
+            ignore_dangling_symlinks=False,
+            dirs_exist_ok=True)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Remove config/extension files."""
-        paths: List[Path] = list(self.config_dir_path.rglob(pattern='*'))
+        paths: list[Path] = list(self.config_dir_path.rglob(pattern='*'))
 
         for path in paths:
-            if path.is_file():
-                os.remove(path=path.relative_to(_DJAI_AWS_EB_CLI_UTIL_DIR_PATH))   # noqa: E501
+            if path.is_file() and (True
+                                   if self.gpu
+                                   else (path.name != _INSTALL_CUDA_SCRIPT_NAME)):  # noqa: E501
+                os.remove(path=path.relative_to(_DJAI_AWS_EB_CLI_UTIL_DIR_PATH))  # noqa: E501
 
         # remove empty directories
         for path in (paths + [self.config_dir_path]):
             if path.is_dir() and \
                     (not any((dir_path :=
                               path.relative_to(_DJAI_AWS_EB_CLI_UTIL_DIR_PATH))
                              .iterdir())):
@@ -68,39 +89,39 @@
                       mode='rt',
                       buffering=-1,
                       encoding='utf-8',
                       errors='strict',
                       newline=None,
                       closefd=True,
                       opener=None) as eb_ignore_file:
-                self.eb_ignore_content: List[str] = eb_ignore_file.readlines()
+                self.eb_ignore_content: list[str] = eb_ignore_file.readlines()
 
     def __enter__(self):
         """Add `.ebignore` file, if applicable."""
         if self.eb_ignore_exists:
             with (open(self.EB_IGNORE_FILE_NAME,
                        mode='at',
                        buffering=-1,
                        encoding='utf-8',
                        errors='strict',
                        newline=None,
                        closefd=True,
                        opener=None) as dst,
-                  open(_DJAI_AWS_EB_CLI_UTIL_DIR_PATH / self.EB_IGNORE_FILE_NAME,   # noqa: E501
+                  open(_DJAI_AWS_EB_CLI_UTIL_DIR_PATH / self.EB_IGNORE_FILE_NAME,  # noqa: E501
                        mode='rt',
                        buffering=-1,
                        encoding='utf-8',
                        errors='strict',
                        newline=None,
                        closefd=True,
                        opener=None) as src):
                 dst.writelines(src.readlines())
 
         else:
-            shutil.copyfile(
+            copyfile(
                 src=_DJAI_AWS_EB_CLI_UTIL_DIR_PATH / self.EB_IGNORE_FILE_NAME,
                 dst=self.EB_IGNORE_FILE_NAME)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         """Remove `.ebignore` file, if applicable."""
         if self.eb_ignore_exists:
             with open(self.EB_IGNORE_FILE_NAME,
@@ -174,23 +195,46 @@
               required=False,
               callback=None,
               nargs=None,
               metavar='ASGI',
               expose_value=True,
               is_eager=False,
               envvar=None)
+@click.option('--gpu',
+              cls=click.Option,
+              show_default=True,
+              prompt=False,
+              confirmation_prompt=False,
+              hide_input=False,
+              is_flag=True,
+              flag_value=True,
+              multiple=False,
+              count=False,
+              allow_from_autoenv=False,
+              type=bool,
+              help='Whether to use GPU',
+              show_choices=True,
+              default=False,
+              required=False,
+              callback=None,
+              nargs=None,
+              metavar='GPU',
+              expose_value=True,
+              is_eager=False,
+              envvar=None)
 def deploy(aws_eb_env_name: Optional[str] = None,
-           asgi: Optional[str] = None):
+           asgi: Optional[str] = None,
+           gpu: Optional[bool] = False):
     """Deploy Djaizz onto AWS Elastic Beanstalk."""
     profile = input('AWS CLI Profile (if not default) = ')
     if not profile.strip():
         profile = 'default'
 
     with (ConfigFilesHandling(_EB_EXTENSIONS_DIR_NAME),
-          ConfigFilesHandling(_PLATFORM_DIR_NAME),
+          ConfigFilesHandling(_PLATFORM_DIR_NAME, gpu=gpu),
           EBIgnoreHandling()):
         if aws_eb_env_name:
             run_cmd(command=f'eb deploy --profile {profile} {aws_eb_env_name}',
                     asgi=asgi)
 
         else:
             region = input('AWS Region = ')
@@ -198,27 +242,50 @@
             subnets = input('AWS Subnets = ')
             assert region and vpc and subnets
 
             # AWS EC2 Instance Type: by default, pick a
             # Compute-optimized instance type
             # with good Networking performance and sufficient Memory
             # (note: Graviton (g) instances not compatible with Djaizz deps)
-            instance_type = input('AWS EC2 Instance Type '
-                                  '(default: c6i.xlarge; min: c6i.large) = ')
-            if not instance_type.strip():
-                instance_type = 'c6i.xlarge'
+            if gpu:
+                pprint(object=_EC2_INSTANCE_TYPES['gpu'],
+                       stream=None,
+                       indent=2,
+                       width=80,
+                       depth=None,
+                       compact=True,
+                       sort_dicts=False,
+                       underscore_numbers=False)
+                instance_type = input('AWS EC2 Instance Type '
+                                      '(default: g4dn.xlarge; min: g4dn.xlarge) = ')  # noqa: E501
+                if not instance_type.strip():
+                    instance_type = 'g4dn.xlarge'
+
+            else:
+                pprint(object=_EC2_INSTANCE_TYPES['cpu'],
+                       stream=None,
+                       indent=2,
+                       width=80,
+                       depth=None,
+                       compact=True,
+                       sort_dicts=False,
+                       underscore_numbers=False)
+                instance_type = input('AWS EC2 Instance Type '
+                                      '(default: c6i.xlarge; min: c6i.large) = ')  # noqa: E501
+                if not instance_type.strip():
+                    instance_type = 'c6i.xlarge'
 
             run_cmd(command=(f'eb create --profile {profile}'
                              f' --region {region}'
                              f' --vpc.id {vpc} --vpc.publicip'
                              f' --vpc.dbsubnets {subnets}'
                              f' --vpc.ec2subnets {subnets}'
                              f' --vpc.elbsubnets {subnets} --vpc.elbpublic'
                              f' --instance_type {instance_type}'
-                             f' --timeout 20'),
+                             f' --timeout 30'),
                     asgi=asgi)
 
 
 @click.group(name='aws-eb',
              cls=click.Group,
              commands={'init': init, 'deploy': deploy},
              invoke_without_command=False,
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/cli/deps.py` & `Djaizz-23.6.14.0/src/djaizz/util/cli/deps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """Djaizz Dependencies."""
 
 
+from collections.abc import Sequence
 from importlib.metadata import version
 from pprint import pprint
-from typing import Sequence  # Py3.9+: use built-ins/collections.abc
 
 import click
 
 
-CAPPED_DEPS: Sequence[str] = ('Channels',
-                              'Daphne',
-                              'Dash-Bootstrap-Components',
-                              'Django-CORS-Headers',
-                              'Django-Plotly-Dash',
+CAPPED_DEPS: Sequence[str] = ('Dash',
                               'H11',
                               'NumPy',
-                              'Quart')
+                              'Pandas')
 
 
 @click.command(name='capped-deps',
                cls=click.Command,
                context_settings=None,
                help=('Djaizz Capped Dependencies CLI >>>'),
                epilog=('^^^ Djaizz Capped Dependencies CLI'),
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/cli/run_cmd.py` & `Djaizz-23.6.14.0/src/djaizz/util/cli/run_cmd.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/git.py` & `Djaizz-23.6.14.0/src/djaizz/util/git.py`

 * *Files identical despite different names*

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/pip.py` & `Djaizz-23.6.14.0/src/djaizz/util/pip.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """Djaizz PIP-related Utilities."""
 
 
 from sys import version_info
 from typing import Optional
-from typing import Dict, List   # Py3.9+: use generic types
 
 from pip._internal.operations.freeze import (   # pylint: disable=import-error
     freeze)
 
 if version_info >= (3, 9):
     from collections.abc import Sequence
 else:
     from typing import Sequence   # pylint: disable=ungrouped-imports
 
 
 __all__: Sequence[str] = ('get_python_dependencies',)
 
 
-def get_python_dependencies() -> Dict[str, Optional[str]]:
+def get_python_dependencies() -> dict[str, Optional[str]]:
     """Get Python Dependencies."""
-    deps_and_vers_dict: Dict[str, Optional[str]] = {}
+    deps_and_vers_dict: dict[str, Optional[str]] = {}
 
     for dep_and_ver_str in freeze(requirement=None,
                                   local_only=False,
                                   user_only=False,
                                   paths=None,
                                   isolated=False,
                                   exclude_editable=False,
                                   skip=()):
-        dep_and_ver_tuple: List[str] = dep_and_ver_str.split('==')
+        dep_and_ver_tuple: list[str] = dep_and_ver_str.split('==')
 
         if len(dep_and_ver_tuple) == 2:
             deps_and_vers_dict[dep_and_ver_tuple[0]] = dep_and_ver_tuple[1]
 
         else:
             assert len(dep_and_ver_tuple) == 1, f'*** {dep_and_ver_tuple} ***'
             deps_and_vers_dict[dep_and_ver_tuple[0]] = None
```

### Comparing `Djaizz-0.0.0a0/src/djaizz/util/views.py` & `Djaizz-23.6.14.0/src/djaizz/util/views.py`

 * *Files identical despite different names*

