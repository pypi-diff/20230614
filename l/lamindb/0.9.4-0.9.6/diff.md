# Comparing `tmp/lamindb-0.9.4.tar.gz` & `tmp/lamindb-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb-0.9.4.tar", last modified: Tue Oct 18 14:01:58 2022, max compression
+gzip compressed data, was "lamindb-0.9.6.tar", last modified: Thu Oct 20 11:04:49 2022, max compression
```

## Comparing `lamindb-0.9.4.tar` & `lamindb-0.9.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     2852 2022-10-08 00:17:16.975733 lamindb-0.9.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-08-29 16:57:35.537184 lamindb-0.9.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-08-29 16:57:35.537275 lamindb-0.9.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     2441 2022-10-13 08:37:13.715193 lamindb-0.9.4/.gitignore
--rw-r--r--   0        0        0     1758 2022-10-12 21:47:11.291104 lamindb-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-08-29 16:57:35.537597 lamindb-0.9.4/LICENSE
--rw-r--r--   0        0        0      344 2022-08-29 16:57:35.537676 lamindb-0.9.4/README.md
--rw-r--r--   0        0        0       49 2022-08-29 16:57:35.537791 lamindb-0.9.4/docs/api.md
--rw-r--r--   0        0        0    37752 2022-10-18 14:00:44.463216 lamindb-0.9.4/docs/changelog.md
--rw-r--r--   0        0        0     2823 2022-10-13 08:37:13.715803 lamindb-0.9.4/docs/faq/flow.ipynb
--rw-r--r--   0        0        0      107 2022-10-13 08:37:13.715953 lamindb-0.9.4/docs/faq/index.md
--rw-r--r--   0        0        0     6226 2022-10-18 13:16:58.684244 lamindb-0.9.4/docs/faq/ingest-bfx.ipynb
--rw-r--r--   0        0        0     2693 2022-10-13 08:37:13.716358 lamindb-0.9.4/docs/faq/ingest-same-file-twice.ipynb
--rw-r--r--   0        0        0        0 2022-10-08 00:17:16.976352 lamindb-0.9.4/docs/faq/mydata_postgres/lG43w46tdNczbjKdotJsI.fastq.gz
--rw-r--r--   0        0        0     2677 2022-10-18 13:34:43.491463 lamindb-0.9.4/docs/faq/postgres.ipynb
--rw-r--r--   0        0        0     9855 2022-10-12 15:40:20.248107 lamindb-0.9.4/docs/faq/select.ipynb
--rw-r--r--   0        0        0     1155 2022-10-10 19:58:03.161510 lamindb-0.9.4/docs/faq/setup.ipynb
--rw-r--r--   0        0        0     6632 2022-10-10 19:58:03.161696 lamindb-0.9.4/docs/faq/storage.ipynb
--rw-r--r--   0        0        0     5734 2022-10-13 10:58:19.007246 lamindb-0.9.4/docs/guide/A1-get-started.ipynb
--rw-r--r--   0        0        0     3112 2022-10-12 23:36:08.977428 lamindb-0.9.4/docs/guide/A2-schema.ipynb
--rw-r--r--   0        0        0     9780 2022-10-14 12:19:32.786009 lamindb-0.9.4/docs/guide/A3-ingest.ipynb
--rw-r--r--   0        0        0     3330 2022-10-12 22:08:14.322492 lamindb-0.9.4/docs/guide/A4-link.ipynb
--rw-r--r--   0        0        0     8504 2022-10-18 13:58:30.075524 lamindb-0.9.4/docs/guide/A5-select-load.ipynb
--rw-r--r--   0        0        0     4541 2022-10-12 15:40:20.248737 lamindb-0.9.4/docs/guide/A6-insert-update-delete.ipynb
--rw-r--r--   0        0        0     3767 2022-10-12 15:40:20.248900 lamindb-0.9.4/docs/guide/A7-pipeline.ipynb
--rw-r--r--   0        0        0     2291 2022-10-13 08:37:13.717244 lamindb-0.9.4/docs/guide/A8-introspect.ipynb
--rw-r--r--   0        0        0     4234 2022-10-12 22:08:14.323137 lamindb-0.9.4/docs/guide/B1-setup.ipynb
--rw-r--r--   0        0        0     7579 2022-10-12 15:40:20.249188 lamindb-0.9.4/docs/guide/B2-design-experiment.ipynb
--rw-r--r--   0        0        0     1984 2022-10-12 15:40:20.249321 lamindb-0.9.4/docs/guide/B3-perform-experiment.ipynb
--rw-r--r--   0        0        0     5282 2022-10-13 08:37:13.717486 lamindb-0.9.4/docs/guide/B4-analyze-assay.ipynb
--rw-r--r--   0        0        0     2584 2022-10-10 19:58:03.162777 lamindb-0.9.4/docs/guide/B5-bfx.ipynb
--rw-r--r--   0        0        0     8042 2022-10-12 15:40:20.249645 lamindb-0.9.4/docs/guide/B6-compbio.ipynb
--rw-r--r--   0        0        0     2995 2022-10-18 13:58:30.075966 lamindb-0.9.4/docs/guide/B7-dataflow.ipynb
--rw-r--r--   0        0        0      143 2022-10-12 15:40:20.250251 lamindb-0.9.4/docs/guide/basic.md
--rw-r--r--   0        0        0       49 2022-10-05 19:20:37.087895 lamindb-0.9.4/docs/guide/index.md
--rw-r--r--   0        0        0      144 2022-10-05 19:20:37.088024 lamindb-0.9.4/docs/guide/rd.md
--rw-r--r--   0        0        0     1249 2022-10-12 22:08:14.323647 lamindb-0.9.4/docs/index.md
--rw-r--r--   0        0        0      122 2022-08-29 16:57:35.541759 lamindb-0.9.4/lamin-project.yaml
--rw-r--r--   0        0        0      863 2022-10-18 13:59:58.185020 lamindb-0.9.4/lamindb/__init__.py
--rw-r--r--   0        0        0     1395 2022-10-13 08:37:13.718089 lamindb-0.9.4/lamindb/_check_versions.py
--rw-r--r--   0        0        0       48 2022-08-29 16:57:35.542013 lamindb-0.9.4/lamindb/_logger.py
--rw-r--r--   0        0        0      274 2022-10-13 08:37:13.718986 lamindb-0.9.4/lamindb/_nb.py
--rw-r--r--   0        0        0      465 2022-09-12 14:19:16.651523 lamindb-0.9.4/lamindb/datasets/__init__.py
--rw-r--r--   0        0        0     3046 2022-10-10 21:33:35.403383 lamindb-0.9.4/lamindb/datasets/_core.py
--rw-r--r--   0        0        0      921 2022-10-12 22:08:14.323932 lamindb-0.9.4/lamindb/db/__init__.py
--rw-r--r--   0        0        0     2576 2022-10-13 11:02:45.936971 lamindb-0.9.4/lamindb/db/_delete.py
--rw-r--r--   0        0        0     7559 2022-10-18 13:16:58.685006 lamindb-0.9.4/lamindb/db/_ingest.py
--rw-r--r--   0        0        0     2668 2022-10-12 15:40:20.251678 lamindb-0.9.4/lamindb/db/_load.py
--rw-r--r--   0        0        0     1622 2022-10-13 08:37:13.719618 lamindb-0.9.4/lamindb/db/_view.py
--rw-r--r--   0        0        0      273 2022-10-12 15:40:20.251822 lamindb-0.9.4/lamindb/dev/__init__.py
--rw-r--r--   0        0        0      599 2022-10-12 15:40:20.251936 lamindb-0.9.4/lamindb/dev/_core.py
--rw-r--r--   0        0        0      240 2022-08-29 16:57:35.543137 lamindb-0.9.4/lamindb/dev/_docs.py
--rw-r--r--   0        0        0      399 2022-10-13 08:37:13.719980 lamindb-0.9.4/lamindb/dev/db/__init__.py
--rw-r--r--   0        0        0     2045 2022-10-18 13:58:30.076397 lamindb-0.9.4/lamindb/dev/db/_core.py
--rw-r--r--   0        0        0     9719 2022-10-12 15:40:20.252712 lamindb-0.9.4/lamindb/dev/db/_insert.py
--rw-r--r--   0        0        0     6512 2022-10-12 15:40:20.252806 lamindb-0.9.4/lamindb/dev/db/_link.py
--rw-r--r--   0        0        0    10644 2022-10-18 13:58:30.076684 lamindb-0.9.4/lamindb/dev/db/_select.py
--rw-r--r--   0        0        0     1767 2022-10-12 15:40:20.253038 lamindb-0.9.4/lamindb/dev/db/_select_result.py
--rw-r--r--   0        0        0     9131 2022-10-18 13:58:30.077071 lamindb-0.9.4/lamindb/dev/db/_staged.py
--rw-r--r--   0        0        0      313 2022-10-12 15:40:20.253182 lamindb-0.9.4/lamindb/dev/db/_track_usage.py
--rw-r--r--   0        0        0     1268 2022-10-12 15:40:20.253249 lamindb-0.9.4/lamindb/dev/db/_update.py
--rw-r--r--   0        0        0       75 2022-09-22 22:22:44.442741 lamindb-0.9.4/lamindb/dev/db/exception.py
--rw-r--r--   0        0        0      367 2022-10-12 15:40:20.253814 lamindb-0.9.4/lamindb/dev/file/__init__.py
--rw-r--r--   0        0        0     2692 2022-10-18 13:16:58.686640 lamindb-0.9.4/lamindb/dev/file/_file.py
--rw-r--r--   0        0        0      496 2022-10-12 15:40:20.254145 lamindb-0.9.4/lamindb/dev/file/_h5ad.py
--rw-r--r--   0        0        0      200 2022-08-29 16:57:35.543784 lamindb-0.9.4/lamindb/dev/file/_images.py
--rw-r--r--   0        0        0      562 2022-10-12 15:40:20.254237 lamindb-0.9.4/lamindb/dev/file/_zarr.py
--rw-r--r--   0        0        0      184 2022-09-22 09:46:57.710548 lamindb-0.9.4/lamindb/dev/object/__init__.py
--rw-r--r--   0        0        0     1164 2022-08-29 16:57:35.543975 lamindb-0.9.4/lamindb/dev/object/_anndata.py
--rw-r--r--   0        0        0      855 2022-10-12 15:40:20.255086 lamindb-0.9.4/lamindb/dev/object/_core.py
--rw-r--r--   0        0        0     1047 2022-10-12 22:08:14.324617 lamindb-0.9.4/lamindb/schema/__init__.py
--rw-r--r--   0        0        0     2198 2022-10-12 22:08:14.324884 lamindb-0.9.4/lamindb/schema/_core.py
--rw-r--r--   0        0        0     1188 2022-09-29 13:35:03.941060 lamindb-0.9.4/lamindb/schema/_table.py
--rw-r--r--   0        0        0     1206 2022-10-13 11:28:06.524494 lamindb-0.9.4/noxfile.py
--rw-r--r--   0        0        0     1277 2022-10-18 13:16:58.687022 lamindb-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     1973 2022-08-29 16:57:35.544603 lamindb-0.9.4/tests/test_conversion.py
--rw-r--r--   0        0        0     1465 2022-10-12 15:40:20.255705 lamindb-0.9.4/tests/test_db.py
--rw-r--r--   0        0        0     1029 2022-10-13 08:37:13.721441 lamindb-0.9.4/tests/test_file.py
--rw-r--r--   0        0        0      380 2022-10-03 16:09:31.739862 lamindb-0.9.4/tests/test_notebooks.py
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 lamindb-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     2852 2022-10-08 00:17:16.975733 lamindb-0.9.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-08-29 16:57:35.537184 lamindb-0.9.6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-08-29 16:57:35.537275 lamindb-0.9.6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     2441 2022-10-13 08:37:13.715193 lamindb-0.9.6/.gitignore
+-rw-r--r--   0        0        0     1758 2022-10-12 21:47:11.291104 lamindb-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-08-29 16:57:35.537597 lamindb-0.9.6/LICENSE
+-rw-r--r--   0        0        0      344 2022-08-29 16:57:35.537676 lamindb-0.9.6/README.md
+-rw-r--r--   0        0        0       49 2022-08-29 16:57:35.537791 lamindb-0.9.6/docs/api.md
+-rw-r--r--   0        0        0    38375 2022-10-20 11:03:10.696824 lamindb-0.9.6/docs/changelog.md
+-rw-r--r--   0        0        0     2823 2022-10-13 08:37:13.715803 lamindb-0.9.6/docs/faq/flow.ipynb
+-rw-r--r--   0        0        0      107 2022-10-13 08:37:13.715953 lamindb-0.9.6/docs/faq/index.md
+-rw-r--r--   0        0        0     6226 2022-10-18 13:16:58.684244 lamindb-0.9.6/docs/faq/ingest-bfx.ipynb
+-rw-r--r--   0        0        0     2693 2022-10-13 08:37:13.716358 lamindb-0.9.6/docs/faq/ingest-same-file-twice.ipynb
+-rw-r--r--   0        0        0        0 2022-10-08 00:17:16.976352 lamindb-0.9.6/docs/faq/mydata_postgres/lG43w46tdNczbjKdotJsI.fastq.gz
+-rw-r--r--   0        0        0     2674 2022-10-20 11:02:50.684137 lamindb-0.9.6/docs/faq/postgres.ipynb
+-rw-r--r--   0        0        0    20086 2022-10-18 17:01:46.253653 lamindb-0.9.6/docs/faq/select.ipynb
+-rw-r--r--   0        0        0     1155 2022-10-10 19:58:03.161510 lamindb-0.9.6/docs/faq/setup.ipynb
+-rw-r--r--   0        0        0     6632 2022-10-10 19:58:03.161696 lamindb-0.9.6/docs/faq/storage.ipynb
+-rw-r--r--   0        0        0     5734 2022-10-18 16:04:36.663068 lamindb-0.9.6/docs/guide/A1-get-started.ipynb
+-rw-r--r--   0        0        0     3112 2022-10-18 16:04:36.664035 lamindb-0.9.6/docs/guide/A2-schema.ipynb
+-rw-r--r--   0        0        0     9780 2022-10-14 12:19:32.786009 lamindb-0.9.6/docs/guide/A3-ingest.ipynb
+-rw-r--r--   0        0        0     3330 2022-10-12 22:08:14.322492 lamindb-0.9.6/docs/guide/A4-link.ipynb
+-rw-r--r--   0        0        0     8504 2022-10-18 13:58:30.075524 lamindb-0.9.6/docs/guide/A5-select-load.ipynb
+-rw-r--r--   0        0        0     4541 2022-10-12 15:40:20.248737 lamindb-0.9.6/docs/guide/A6-insert-update-delete.ipynb
+-rw-r--r--   0        0        0     3767 2022-10-12 15:40:20.248900 lamindb-0.9.6/docs/guide/A7-pipeline.ipynb
+-rw-r--r--   0        0        0     2291 2022-10-13 08:37:13.717244 lamindb-0.9.6/docs/guide/A8-introspect.ipynb
+-rw-r--r--   0        0        0     4128 2022-10-19 20:33:05.020748 lamindb-0.9.6/docs/guide/B1-setup.ipynb
+-rw-r--r--   0        0        0     7535 2022-10-19 20:33:05.021104 lamindb-0.9.6/docs/guide/B2-design-experiment.ipynb
+-rw-r--r--   0        0        0     2230 2022-10-18 17:01:46.254742 lamindb-0.9.6/docs/guide/B3-perform-experiment.ipynb
+-rw-r--r--   0        0        0     5316 2022-10-19 20:33:05.021426 lamindb-0.9.6/docs/guide/B4-analyze-assay.ipynb
+-rw-r--r--   0        0        0     2584 2022-10-18 16:13:35.590724 lamindb-0.9.6/docs/guide/B5-bfx.ipynb
+-rw-r--r--   0        0        0     8216 2022-10-18 17:01:46.255131 lamindb-0.9.6/docs/guide/B6-compbio.ipynb
+-rw-r--r--   0        0        0     2989 2022-10-18 17:01:46.255328 lamindb-0.9.6/docs/guide/B7-dataflow.ipynb
+-rw-r--r--   0        0        0      143 2022-10-12 15:40:20.250251 lamindb-0.9.6/docs/guide/basic.md
+-rw-r--r--   0        0        0       49 2022-10-05 19:20:37.087895 lamindb-0.9.6/docs/guide/index.md
+-rw-r--r--   0        0        0      144 2022-10-05 19:20:37.088024 lamindb-0.9.6/docs/guide/rd.md
+-rw-r--r--   0        0        0     1249 2022-10-12 22:08:14.323647 lamindb-0.9.6/docs/index.md
+-rw-r--r--   0        0        0      122 2022-08-29 16:57:35.541759 lamindb-0.9.6/lamin-project.yaml
+-rw-r--r--   0        0        0      863 2022-10-20 11:03:27.115125 lamindb-0.9.6/lamindb/__init__.py
+-rw-r--r--   0        0        0     1395 2022-10-20 11:02:50.684573 lamindb-0.9.6/lamindb/_check_versions.py
+-rw-r--r--   0        0        0       48 2022-08-29 16:57:35.542013 lamindb-0.9.6/lamindb/_logger.py
+-rw-r--r--   0        0        0      274 2022-10-13 08:37:13.718986 lamindb-0.9.6/lamindb/_nb.py
+-rw-r--r--   0        0        0      465 2022-09-12 14:19:16.651523 lamindb-0.9.6/lamindb/datasets/__init__.py
+-rw-r--r--   0        0        0     3046 2022-10-10 21:33:35.403383 lamindb-0.9.6/lamindb/datasets/_core.py
+-rw-r--r--   0        0        0      921 2022-10-12 22:08:14.323932 lamindb-0.9.6/lamindb/db/__init__.py
+-rw-r--r--   0        0        0     2576 2022-10-13 11:02:45.936971 lamindb-0.9.6/lamindb/db/_delete.py
+-rw-r--r--   0        0        0     7559 2022-10-18 13:16:58.685006 lamindb-0.9.6/lamindb/db/_ingest.py
+-rw-r--r--   0        0        0     2668 2022-10-12 15:40:20.251678 lamindb-0.9.6/lamindb/db/_load.py
+-rw-r--r--   0        0        0     1622 2022-10-13 08:37:13.719618 lamindb-0.9.6/lamindb/db/_view.py
+-rw-r--r--   0        0        0      273 2022-10-12 15:40:20.251822 lamindb-0.9.6/lamindb/dev/__init__.py
+-rw-r--r--   0        0        0      599 2022-10-12 15:40:20.251936 lamindb-0.9.6/lamindb/dev/_core.py
+-rw-r--r--   0        0        0      240 2022-08-29 16:57:35.543137 lamindb-0.9.6/lamindb/dev/_docs.py
+-rw-r--r--   0        0        0      399 2022-10-13 08:37:13.719980 lamindb-0.9.6/lamindb/dev/db/__init__.py
+-rw-r--r--   0        0        0     2045 2022-10-18 13:58:30.076397 lamindb-0.9.6/lamindb/dev/db/_core.py
+-rw-r--r--   0        0        0     9719 2022-10-12 15:40:20.252712 lamindb-0.9.6/lamindb/dev/db/_insert.py
+-rw-r--r--   0        0        0     6512 2022-10-12 15:40:20.252806 lamindb-0.9.6/lamindb/dev/db/_link.py
+-rw-r--r--   0        0        0    10644 2022-10-18 13:58:30.076684 lamindb-0.9.6/lamindb/dev/db/_select.py
+-rw-r--r--   0        0        0     1767 2022-10-12 15:40:20.253038 lamindb-0.9.6/lamindb/dev/db/_select_result.py
+-rw-r--r--   0        0        0     9131 2022-10-18 13:58:30.077071 lamindb-0.9.6/lamindb/dev/db/_staged.py
+-rw-r--r--   0        0        0      313 2022-10-12 15:40:20.253182 lamindb-0.9.6/lamindb/dev/db/_track_usage.py
+-rw-r--r--   0        0        0     1268 2022-10-12 15:40:20.253249 lamindb-0.9.6/lamindb/dev/db/_update.py
+-rw-r--r--   0        0        0       75 2022-09-22 22:22:44.442741 lamindb-0.9.6/lamindb/dev/db/exception.py
+-rw-r--r--   0        0        0      367 2022-10-12 15:40:20.253814 lamindb-0.9.6/lamindb/dev/file/__init__.py
+-rw-r--r--   0        0        0     2692 2022-10-18 13:16:58.686640 lamindb-0.9.6/lamindb/dev/file/_file.py
+-rw-r--r--   0        0        0      496 2022-10-12 15:40:20.254145 lamindb-0.9.6/lamindb/dev/file/_h5ad.py
+-rw-r--r--   0        0        0      200 2022-08-29 16:57:35.543784 lamindb-0.9.6/lamindb/dev/file/_images.py
+-rw-r--r--   0        0        0      562 2022-10-12 15:40:20.254237 lamindb-0.9.6/lamindb/dev/file/_zarr.py
+-rw-r--r--   0        0        0      184 2022-09-22 09:46:57.710548 lamindb-0.9.6/lamindb/dev/object/__init__.py
+-rw-r--r--   0        0        0     1164 2022-08-29 16:57:35.543975 lamindb-0.9.6/lamindb/dev/object/_anndata.py
+-rw-r--r--   0        0        0      855 2022-10-12 15:40:20.255086 lamindb-0.9.6/lamindb/dev/object/_core.py
+-rw-r--r--   0        0        0     1047 2022-10-12 22:08:14.324617 lamindb-0.9.6/lamindb/schema/__init__.py
+-rw-r--r--   0        0        0     2198 2022-10-12 22:08:14.324884 lamindb-0.9.6/lamindb/schema/_core.py
+-rw-r--r--   0        0        0     1188 2022-09-29 13:35:03.941060 lamindb-0.9.6/lamindb/schema/_table.py
+-rw-r--r--   0        0        0     1206 2022-10-13 11:28:06.524494 lamindb-0.9.6/noxfile.py
+-rw-r--r--   0        0        0     1277 2022-10-20 11:02:50.684918 lamindb-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1973 2022-08-29 16:57:35.544603 lamindb-0.9.6/tests/test_conversion.py
+-rw-r--r--   0        0        0     1465 2022-10-12 15:40:20.255705 lamindb-0.9.6/tests/test_db.py
+-rw-r--r--   0        0        0     1029 2022-10-13 08:37:13.721441 lamindb-0.9.6/tests/test_file.py
+-rw-r--r--   0        0        0      380 2022-10-03 16:09:31.739862 lamindb-0.9.6/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 lamindb-0.9.6/PKG-INFO
```

### Comparing `lamindb-0.9.4/.github/workflows/build.yml` & `lamindb-0.9.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/.github/workflows/latest-changes.yml` & `lamindb-0.9.6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/.gitignore` & `lamindb-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/.pre-commit-config.yaml` & `lamindb-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/LICENSE` & `lamindb-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/changelog.md` & `lamindb-0.9.6/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade wetlab schema | [297](https://github.com/laminlabs/lamindb/pull/297) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-20 | 0.9.6
+⬆️ Added `dset` and `project` tables to core | [296](https://github.com/laminlabs/lamindb/pull/296) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-19 | 0.9.5
+🩹 Fixed rds nbs | [295](https://github.com/laminlabs/lamindb/pull/295) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-18 |
+📝 Add prisma examples and implementation ideas | [294](https://github.com/laminlabs/lamindb/pull/294) | [fredericenard](https://github.com/fredericenard) | 2022-10-18 |
 ♻️ Refactor linked select | [286](https://github.com/laminlabs/lamindb/pull/286) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-18 | 0.9.4
 ✏️ Fix typo in link table entry fetching | [292](https://github.com/laminlabs/lamindb/pull/292) | [bpenteado](https://github.com/bpenteado) | 2022-10-17 |
 🐛 Fixed link via link tables | [291](https://github.com/laminlabs/lamindb/pull/291) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-15 | 0.9.3
 ✨ Add an option to use `fsspec` for upload | [288](https://github.com/laminlabs/lamindb/pull/288) | [Koncopd](https://github.com/Koncopd) | 2022-10-15 |
 ✨ Load returns filepath if no in-memory format is found | [287](https://github.com/laminlabs/lamindb/pull/287) | [sunnyosun](https://github.com/sunnyosun) | 2022-10-13 | 0.9.2
 🎨 Clean up dtransform_in | [commit](https://github.com/laminlabs/lamindb/commit/429abf1c12b2e518e6d65329e4c4067e96d28fec) | [falexwolf](https://github.com/falexwolf) | 2022-10-13 | 0.9.1
 🎨 Continue overhaul | [285](https://github.com/laminlabs/lamindb/pull/285) | [falexwolf](https://github.com/falexwolf) | 2022-10-13 | 0.9.0
```

### Comparing `lamindb-0.9.4/docs/faq/flow.ipynb` & `lamindb-0.9.6/docs/faq/flow.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/faq/ingest-bfx.ipynb` & `lamindb-0.9.6/docs/faq/ingest-bfx.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/faq/ingest-same-file-twice.ipynb` & `lamindb-0.9.6/docs/faq/ingest-same-file-twice.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/faq/postgres.ipynb` & `lamindb-0.9.6/docs/faq/postgres.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923735119047619%*

 * *Differences: {"'metadata'": "{'kernelspec': {'display_name': 'Python 3.10.6 64-bit'}, 'language_info': "*

 * *               "{'version': '3.10.6'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e'}}}"}*

```diff
@@ -91,43 +91,43 @@
             "source": [
                 "ingest.commit()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.12 ('base1')",
+            "display_name": "Python 3.10.6 64-bit",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.10.6"
         },
         "nbproject": {
             "id": "DMAcnk6XsuFy",
             "parent": null,
             "pypackage": {
                 "lamindb": "0.6.0",
                 "scanpy": "1.8.2",
                 "scikit-learn": "1.1.2"
             },
             "time_init": "2022-10-07T20:45:37.197030+00:00",
             "version": "2"
         },
         "vscode": {
             "interpreter": {
-                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
+                "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lamindb-0.9.4/docs/faq/select.ipynb` & `lamindb-0.9.6/docs/guide/A5-select-load.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9364380411255412%*

 * *Differences: {"'cells'": "{0: {'id': '1a515a1b-34ac-4c0b-ae6c-0f360bd3ac9b', 'source': ['# Load and select "*

 * *            "data: `db.load & db.select`']}, 1: {'id': 'fe98f316-2175-4c16-8bb5-726f61fdf85c', "*

 * *            "'source': {delete: [4, 3, 2, 1]}}, 4: {'id': 'e1dc8fd8', 'source': ['dobject = "*

 * *            'ln.db.select.dobject(name="iris").first()\\n\', \'\\n\', \'df = '*

 * *            "ln.db.load(dobject)']}, 5: {'id': 'f5356880', 'source': ['df.head()']}, 6: {'id': "*

 * *            "'3ef9f658', 'source': ['If no in-mem […]*

```diff
@@ -1,445 +1,416 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "434a0140-b55c-42a2-ad41-f97e4ef65a28",
+            "id": "1a515a1b-34ac-4c0b-ae6c-0f360bd3ac9b",
             "metadata": {},
             "source": [
-                "# How does LaminDB's `select` relate to SQLModel's `select`?"
+                "# Load and select data: `db.load & db.select`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cff57921-7332-493a-a627-7b9b587f4cf8",
+            "id": "fe98f316-2175-4c16-8bb5-726f61fdf85c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb as ln\n",
-                "import sqlmodel as sqm\n",
-                "import lnschema_core as core\n",
-                "from datetime import datetime\n",
-                "import pandas as pd\n",
                 "\n",
                 "ln.nb.header()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f9565708-d03d-43e8-be80-6ee057eb9626",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "engine = ln.settings.instance.db_engine()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "4d16a536-5bf0-43c3-8e62-125ff478c5f3",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "def to_df(select_list):\n",
-                "    return pd.DataFrame(\n",
-                "        [row.dict() for row in select_list], columns=select_list[0].__fields__\n",
-                "    )"
-            ]
-        },
-        {
             "cell_type": "markdown",
-            "id": "b837c04c-bba2-4005-ac68-6ef4cf7c6e7f",
+            "id": "19a6382c",
             "metadata": {},
             "source": [
-                "## Selecting a whole table"
+                "## Load"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ae68bb41-f3c7-4aed-8416-6d5f59c8c540",
+            "id": "50c90781",
             "metadata": {},
             "source": [
-                "### (A) SQLModel"
+                "Load data objects into memory via {class}`~lamindb.db.load`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3c8be7c7-679c-48f3-9db5-83d2ae8d9ecc",
+            "id": "e1dc8fd8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with sqm.Session(engine) as session:\n",
-                "    df = to_df(session.exec(sqm.select(core.dobject)).all())"
+                "dobject = ln.db.select.dobject(name=\"iris\").first()\n",
+                "\n",
+                "df = ln.db.load(dobject)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a1acf368-5a41-41b5-922c-5d6e46575d9a",
+            "id": "f5356880",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df"
+                "df.head()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0ba2c38b-7e5e-4f11-8a4e-0ed68d8c6a74",
+            "id": "3ef9f658",
             "metadata": {},
             "source": [
-                "### (B) LaminDB"
+                "If no in-memory format can be found, returns the filepath:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2cb8cab9-1ca6-46fe-907d-de0aac9cf185",
+            "id": "332ea6e5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df = ln.db.select.dobject().df()"
+                "dobject = ln.db.select.dobject(name=\"paradisi05_laminopathic_nuclei\").one()\n",
+                "\n",
+                "ln.db.load(dobject)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "aaf48393",
+            "metadata": {},
+            "source": [
+                "To trace data back to its source, you can use the linked `dtransform` that generated the data. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "df8acf8f-3f18-40fa-8b8a-cd39a59c6e16",
+            "id": "ef8373c6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df"
+                "dobject.dtransform_id"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6a4350e3-74dc-4585-bba2-1be085bc8e48",
+            "id": "bbda4807",
             "metadata": {},
             "source": [
-                "## Subsetting a selection with `where`: equality"
+                "## Select"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6e8a3eba-5989-4228-ae6a-da55389d5c0a",
-            "metadata": {
-                "tags": []
-            },
+            "id": "233821ee",
+            "metadata": {},
             "source": [
-                "### (A) SQLModel"
+                "For simple frequent queries, LaminDB has a high-level select API {class}`~lamindb.db.select` based on [SQLModel](https://sqlmodel.tiangolo.com).\n",
+                "\n",
+                "For complicated queries, you can use any SQL select. See below."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "2fef54c7-506f-4810-8823-351ec804dcb0",
+            "cell_type": "markdown",
+            "id": "25816b0f",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "with sqm.Session(engine) as session:\n",
-                "    df = to_df(\n",
-                "        session.exec(\n",
-                "            sqm.select(core.dobject).where(core.dobject.suffix == \".feather\")\n",
-                "        ).all()\n",
-                "    )"
+                "### Simple table queries"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "bf0adf82-46db-4f44-8308-8c9eaa2f1705",
+            "cell_type": "markdown",
+            "id": "649fe5de",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "df"
+                "You can select any entity table in the database by its fields, for instance:"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ef8a7794-da68-4f8d-b656-b6b0c7320954",
+            "id": "ccee9eee",
             "metadata": {},
             "source": [
-                "### (B) LaminDB"
+                "The high-level select API by default returns a list of results:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5095c450-222b-4fe4-918d-4f09a2dacdb9",
+            "id": "6c4a09c7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject(suffix=\".feather\").df()"
+                "ln.db.select.dobject(suffix=\".feather\").all()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "450cf126-3baf-464a-b9c1-d9ecdeec8d06",
+            "id": "431a45ac",
             "metadata": {},
             "source": [
-                "## Queries involving linked tables"
+                "You can call `.df()` to return a `DataFrame` instead."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "feeabc0b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.db.select.dobject(suffix=\".feather\").df()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "866e6063-cd16-4dfb-ba14-2d940755857e",
+            "id": "79dd60af",
             "metadata": {},
             "source": [
-                "### (A) SQLModel"
+                "If no constraints are passed, the select returns all rows in the table."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b64919b2-e875-4b67-a2e7-5b21cdccb240",
+            "id": "a03a9291",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.user().df()"
+                "ln.db.select.dobject().df()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9f61985f-5a5a-42ab-8a1e-57db92406fae",
+            "cell_type": "markdown",
+            "id": "b6bf7cd4",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "user_id = \"DzTjkKse\""
+                "### Select data objects by linked entities"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "fe548aef-2eee-4624-808f-7fd67b45de30",
+            "id": "4dbfbd08",
             "metadata": {},
             "source": [
-                "Select version without joins, but using the `in_` operator."
+                "You can select data objects by fields that are not present in the `dobject` table via linked entities.\n",
+                "\n",
+                "You can do this through providing a `where` dictionary."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "646fe3d5-2878-4be5-b7a0-f8b43fd7faea",
+            "id": "314db444",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with sqm.Session(engine) as session:\n",
-                "    # all notebooks authored by the user\n",
-                "    jupynbs = session.exec(\n",
-                "        sqm.select(core.jupynb).where(core.jupynb.created_by == user_id)\n",
-                "    ).all()\n",
-                "    jupynb_ids = [jupynb.id for jupynb in jupynbs]\n",
-                "    # all dtransforms linked to these notebooks\n",
-                "    dtransforms = session.exec(\n",
-                "        sqm.select(core.dtransform).where(core.dtransform.jupynb_id.in_(jupynb_ids))\n",
-                "    ).all()\n",
-                "    dtransform_ids = [dtransform.id for dtransform in dtransforms]\n",
-                "    # all dobjects linked to these dtransforms\n",
-                "    df = to_df(\n",
-                "        session.exec(\n",
-                "            sqm.select(core.dobject).where(\n",
-                "                core.dobject.dtransform_id.in_(dtransform_ids)\n",
-                "            )\n",
-                "        ).all()\n",
-                "    )"
+                "ln.db.select.dobject(where=dict(jupynb=dict(name=\"Ingest data: `db.Ingest`\"))).df()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f2fe1334-b697-4f8b-9fab-2bd3403270f4",
+            "id": "0f5d7ac9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df"
+                "ln.db.select.dobject(suffix=\".h5ad\", where=dict(gene=dict(symbol=\"Actg1\"))).df()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a9d539ec-0c12-46e9-b938-f08c2f52a68f",
+            "id": "2733453e",
             "metadata": {},
             "source": [
-                "### LaminDB"
+                "`where` can filter conditions from multiple entities."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "40ec7add-d71b-4d15-bf7f-3434c57d81be",
+            "id": "dff3bb85",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# ln.db.select.dobject(where=dict(user=dict(id=\"DzTjkKse\")))"
+                "from bioreadout import lookup\n",
+                "\n",
+                "ln.db.select.dobject(\n",
+                "    where=dict(\n",
+                "        gene=dict(ncbi_gene_id=66722),\n",
+                "        readout=dict(efo_id=lookup.readout.single_cell_RNA_sequencing),\n",
+                "    )\n",
+                ").df()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "7b36b044-ae74-467a-b686-3dc34390fcb5",
+            "id": "7df355c9",
             "metadata": {},
             "source": [
-                "## Subsetting a selection with `where`: general comparisons"
+                "query dobject by user"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "adb3b232-dfb3-413a-ad2f-020e7470358b",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "6181d6a6",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### (A) SQLModel"
+                "ln.db.select.dobject(where=dict(user=dict(name=\"Test User1\"))).df()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "dc62ac95-34cf-449d-baca-f8f0c3866c5d",
+            "id": "c5581f50",
             "metadata": {},
             "source": [
-                "Subsetting the previous select to the most recent additions."
+                "### SQL queries"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e8c787c0-1f66-4d17-be49-dbd889056c3d",
+            "cell_type": "markdown",
+            "id": "0e463f89",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "time = datetime(2022, 10, 11, 23, 0, 0)"
+                "You can construct arbitrary SQL queries via [SQLModel](https://sqlmodel.tiangolo.com)."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "8b2813c4-2f8e-4291-8ff8-129a5d606221",
+            "cell_type": "markdown",
+            "id": "4e5e039b",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "with sqm.Session(engine) as session:\n",
-                "    df = to_df(\n",
-                "        session.exec(\n",
-                "            sqm.select(core.dobject).where(\n",
-                "                core.dobject.suffix == \".feather\", core.dobject.created_at > time\n",
-                "            )\n",
-                "        ).all()\n",
-                "    )"
+                "For instance, let's select for a data source via the linked `dtransform`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f6395d63-d0d1-4c79-bb74-4aa78394048c",
+            "id": "25deec4b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df"
+                "with ln.db.session() as session:\n",
+                "    dtransform = session.get(ln.schema.core.dtransform, dobject.dtransform_id)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a1fac3b1-126e-4cb2-9bf6-4395f8b13901",
+            "id": "c0236234",
             "metadata": {},
             "source": [
-                "### (B) LaminDB"
+                "Inspecting the result we see that the dobject originates from a Jupyter Notebook."
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "82bf743b-bd9b-4919-b527-a8ffceb62530",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "39f75d53",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "We can't do this right now."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "1003ad5d-e8aa-4ad2-8f3f-6ce1b7672097",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "## Subsetting a selection with `where`: combine expressions using `or`"
+                "dtransform"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "cb3d2363-495c-46e9-b931-1b0874d1e0e6",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0bfbcade",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "SQLModel only."
+                "with ln.db.session() as session:\n",
+                "    jupynb = session.get(\n",
+                "        ln.schema.core.jupynb,\n",
+                "        (dtransform.jupynb_id, dtransform.jupynb_v),  # it's version \"1\" see jupynb_v\n",
+                "    )"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "168343fe-6011-4a29-9dc4-2915f00ec1b2",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "5f889852",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Subsetting a selection with `where`: limit select results"
+                "jupynb"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "59f0d0d5-e623-474a-a82e-c0ec9171d33d",
+            "id": "b7c16562",
             "metadata": {},
             "source": [
-                "SQLModel only."
+                "Now we found the person who last edited the notebook!"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "4835c466-9aa5-47a1-af67-0767965ce1a9",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c55ca2cd",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Limiting and offsetting select results"
+                "with ln.db.session() as session:\n",
+                "    user = session.get(ln.schema.core.user, jupynb.created_by)"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "053a4928-8d45-49f1-a1b1-aba59fe1587f",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "1c199ae7",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "This is important for selecting tables with very high numbers of rows."
+                "user"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "9194b6d6-6ec7-4eb2-ba1b-284bf0b60bc8",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7edd5a1f",
             "metadata": {},
-            "source": [
-                "SQLModel only."
-            ]
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.12 ('base1')",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.13"
         },
         "nbproject": {
-            "id": "Lu39q1AU48Ik",
+            "id": "hmWrrFMGO5Dg",
             "parent": null,
             "pypackage": null,
-            "time_init": "2022-10-12T10:15:17.608530+00:00",
+            "time_init": "2022-07-31T16:34:36.395954+00:00",
             "version": "draft"
         },
         "vscode": {
             "interpreter": {
-                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
+                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lamindb-0.9.4/docs/faq/setup.ipynb` & `lamindb-0.9.6/docs/faq/setup.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/faq/storage.ipynb` & `lamindb-0.9.6/docs/faq/storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A1-get-started.ipynb` & `lamindb-0.9.6/docs/guide/A1-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A2-schema.ipynb` & `lamindb-0.9.6/docs/guide/A2-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A3-ingest.ipynb` & `lamindb-0.9.6/docs/guide/A3-ingest.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A4-link.ipynb` & `lamindb-0.9.6/docs/guide/A4-link.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A5-select-load.ipynb` & `lamindb-0.9.6/docs/guide/B6-compbio.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9377967116724739%*

 * *Differences: {"'cells'": "{0: {'id': '8b86aba3', 'source': ['# Compbio analysis']}, 1: {'id': 'a69a8f5f', "*

 * *            "'source': {insert: [(1, 'import scanpy as sc\\n')]}}, 3: {'id': 'be15396a', 'source': "*

 * *            "['## Link experimental metadata to the datasets']}, 4: {'id': 'dade1621', 'source': "*

 * *            "['Select for datasets ingested from a bioinformatics run:']}, 5: {'id': '6c501dad', "*

 * *            "'source': ['# bfx_runs = ln.db.select.pipeline_run().all()\\n', '# bfx_runs']}, 6: "*

 * *            "{'id':  […]*

```diff
@@ -1,392 +1,351 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "1a515a1b-34ac-4c0b-ae6c-0f360bd3ac9b",
+            "id": "8b86aba3",
             "metadata": {},
             "source": [
-                "# Load and select data: `db.load & db.select`"
+                "# Compbio analysis"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "fe98f316-2175-4c16-8bb5-726f61fdf85c",
+            "id": "a69a8f5f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb as ln\n",
+                "import scanpy as sc\n",
                 "\n",
                 "ln.nb.header()"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "19a6382c",
-            "metadata": {},
-            "source": [
-                "## Load"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "50c90781",
-            "metadata": {},
-            "source": [
-                "Load data objects into memory via {class}`~lamindb.db.load`:"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e1dc8fd8",
+            "id": "a79fb38e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dobject = ln.db.select.dobject(name=\"iris\").first()\n",
-                "\n",
-                "df = ln.db.load(dobject)"
+                "!lndb login testuser2"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f5356880",
+            "cell_type": "markdown",
+            "id": "be15396a",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "df.head()"
+                "## Link experimental metadata to the datasets"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3ef9f658",
+            "id": "dade1621",
             "metadata": {},
             "source": [
-                "If no in-memory format can be found, returns the filepath:"
+                "Select for datasets ingested from a bioinformatics run:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "332ea6e5",
+            "id": "6c501dad",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dobject = ln.db.select.dobject(name=\"paradisi05_laminopathic_nuclei\").one()\n",
-                "\n",
-                "ln.db.load(dobject)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "aaf48393",
-            "metadata": {},
-            "source": [
-                "To trace data back to its source, you can use the linked `dtransform` that generated the data. "
+                "# bfx_runs = ln.db.select.pipeline_run().all()\n",
+                "# bfx_runs"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ef8373c6",
+            "id": "ea67d809",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dobject.dtransform_id"
+                "# dtransform_id = ln.db.select.dtransform(pipeline_run_id=bfx_runs[0].id).first().id\n",
+                "# dobjects = ln.db.select.dobject(dtransform_id=dtransform_id).all()\n",
+                "# len(dobjects)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "bbda4807",
+            "id": "07c02ad1",
             "metadata": {},
             "source": [
-                "## Select"
+                "Now let's link biometa to the bfx run output datasets:"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "233821ee",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "606fef05",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "For simple frequent queries, LaminDB has a high-level select API {class}`~lamindb.db.select` based on [SQLModel](https://sqlmodel.tiangolo.com).\n",
+                "# biometa = ln.db.select.biometa(\n",
+                "#     readout_id=ln.db.select.readout(name=\"single-cell RNA sequencing\").one().id\n",
+                "# ).one()\n",
                 "\n",
-                "For complicated queries, you can use any SQL select. See below."
+                "# for dobject in dobjects:\n",
+                "#     ln.db.link.biometa(dobject_id=dobject.id, biometa_id=biometa.id)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "25816b0f",
+            "id": "89060817",
             "metadata": {},
             "source": [
-                "### Simple table queries"
+                "Let's also link the screen results to its biometa."
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "649fe5de",
-            "metadata": {},
-            "source": [
-                "You can select any entity table in the database by its fields, for instance:"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "ccee9eee",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4abd4386",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "The high-level select API by default returns a list of results:"
+                "# dobject = ln.db.select.dobject(name=\"schmidt22-crispra-gws-IFNG\").one()\n",
+                "# dobject"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6c4a09c7",
+            "id": "64a96cc3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject(suffix=\".feather\").all()"
+                "# biometa = ln.db.select.biometa(\n",
+                "#     readout_id=ln.db.select.readout(name=\"interferon gamma\").one().id\n",
+                "# ).one()\n",
+                "\n",
+                "# ln.db.link.biometa(dobject_id=dobject.id, biometa_id=biometa.id)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "431a45ac",
+            "id": "01afc466",
             "metadata": {},
             "source": [
-                "You can call `.df()` to return a `DataFrame` instead."
+                "Fill out additional biometa fields for dobjects ingested with feature models."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "feeabc0b",
+            "id": "6e9f78da",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject(suffix=\".feather\").df()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "79dd60af",
-            "metadata": {},
-            "source": [
-                "If no constraints are passed, the select returns all rows in the table."
+                "ln.db.select.jupynb(name=\"Track and analyze experimental data\").all()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "a03a9291",
+            "id": "82c5881e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject().df()"
+                "jupynb_id = ln.db.select.jupynb(name=\"Track and analyze experimental data\").all()[-1].id\n",
+                "dtransform_id = ln.db.select.dtransform(jupynb_id=jupynb_id).all()[-1].id"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "b6bf7cd4",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "ae32492b",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### Select data objects by linked entities"
+                "jupynb_id, dtransform_id"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "4dbfbd08",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "dda07ff7",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You can select data objects by fields that are not present in the `dobject` table via linked entities.\n",
-                "\n",
-                "You can do this through providing a `where` dictionary."
+                "dobjects = ln.db.select.dobject(dtransform_id=dtransform_id).all()\n",
+                "dobjects"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "314db444",
+            "id": "e837f0ab",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject(where=dict(jupynb=dict(name=\"Ingest data: `db.Ingest`\"))).df()"
+                "# biometa1 = ln.db.select.biometa(\n",
+                "#     readout_id=ln.db.select.readout(name=\"interferon gamma\").one().id\n",
+                "# ).one()\n",
+                "\n",
+                "# for dobject in dobjects:\n",
+                "#     doject_biometa = ln.db.select.dobject_biometa(dobject_id=dobject.id).one()\n",
+                "#     biometa = ln.db.select.biometa(id=doject_biometa.biometa_id).one()\n",
+                "#     insert_dict = {}\n",
+                "#     for key in biometa.dict().keys():\n",
+                "#         if key in [\"id\", \"featureset_id\"]:\n",
+                "#             continue\n",
+                "#         if biometa1.__getattribute__(key) is not None:\n",
+                "#             insert_dict[key] = biometa1.__getattribute__(key)\n",
+                "\n",
+                "#     ln.db.update.biometa(key=biometa.id, **insert_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0f5d7ac9",
+            "id": "4ef146a4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject(suffix=\".h5ad\", where=dict(gene=dict(symbol=\"Actg1\"))).df()"
+                "# ln.db.select.biometa(id=doject_biometa.biometa_id).all()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "2733453e",
+            "id": "8f74a7d1",
             "metadata": {},
             "source": [
-                "`where` can filter conditions from multiple entities."
+                "## Load in the raw data generated from the BFX pipeline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dff3bb85",
+            "id": "751ec81a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from bioreadout import lookup\n",
-                "\n",
-                "ln.db.select.dobject(\n",
-                "    where=dict(\n",
-                "        gene=dict(ncbi_gene_id=66722),\n",
-                "        readout=dict(efo_id=lookup.readout.single_cell_RNA_sequencing),\n",
-                "    )\n",
-                ").df()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "7df355c9",
-            "metadata": {},
-            "source": [
-                "query dobject by user"
+                "# h5ad = ln.db.select.dobject(suffix=\".h5ad\").first()\n",
+                "# h5ad"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6181d6a6",
+            "id": "559d74c1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.dobject(where=dict(user=dict(name=\"Test User1\"))).df()"
+                "hits = ln.db.select.dobject(name=\"schmidt22_crispra_gws_IFNG_hits\").one()\n",
+                "hits"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "c5581f50",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "199d7009",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "### SQL queries"
+                "# adata = ln.db.load(h5ad)"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "0e463f89",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "36b9886e",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "You can construct arbitrary SQL queries via [SQLModel](https://sqlmodel.tiangolo.com)."
+                "screen_hits = ln.db.load(hits)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "4e5e039b",
+            "id": "9bdf36b8",
             "metadata": {},
             "source": [
-                "For instance, let's select for a data source via the linked `dtransform`:"
+                "## Perform single cell analysis, integrating the CRISPR screen data"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "25deec4b",
+            "id": "481a6ef7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with ln.db.session() as session:\n",
-                "    dtransform = session.get(ln.schema.core.dtransform, dobject.dtransform_id)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "c0236234",
-            "metadata": {},
-            "source": [
-                "Inspecting the result we see that the dobject originates from a Jupyter Notebook."
+                "# sc.tl.score_genes(\n",
+                "#     adata, adata.var_names.intersection(screen_hits[\"id\"].values).tolist()\n",
+                "# )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "39f75d53",
+            "id": "30392a7e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "dtransform"
+                "# sc.pl.umap(adata, color=\"cluster_name\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "0bfbcade",
+            "id": "972a5071",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with ln.db.session() as session:\n",
-                "    jupynb = session.get(\n",
-                "        ln.schema.core.jupynb,\n",
-                "        (dtransform.jupynb_id, dtransform.jupynb_v),  # it's version \"1\" see jupynb_v\n",
-                "    )"
+                "# sc.pl.umap(adata, color=\"score\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5f889852",
+            "id": "4072962b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "jupynb"
+                "# sc.pl.matrixplot(adata, groupby=\"cluster_name\", var_names=[\"score\"])"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "b7c16562",
+            "id": "4aa0cc70",
             "metadata": {},
             "source": [
-                "Now we found the person who last edited the notebook!"
+                "## Ingest the processed dataset into LaminDB"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "c55ca2cd",
+            "id": "b5a97c12",
             "metadata": {},
             "outputs": [],
             "source": [
-                "with ln.db.session() as session:\n",
-                "    user = session.get(ln.schema.core.user, jupynb.created_by)"
+                "# ln.db.ingest.add(adata, name=\"schmidt22_perturbseq_analyzed\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1c199ae7",
+            "id": "bd34c28b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "user"
+                "# ln.db.ingest.commit()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "7edd5a1f",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3.9.13 ('py39')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -395,19 +354,22 @@
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.13"
         },
         "nbproject": {
-            "id": "hmWrrFMGO5Dg",
+            "id": "lEVRZ3cfzpu6",
             "parent": null,
-            "pypackage": null,
-            "time_init": "2022-07-31T16:34:36.395954+00:00",
-            "version": "draft"
+            "pypackage": {
+                "lamindb": "0.3.3",
+                "scanpy": "1.8.2"
+            },
+            "time_init": "2022-08-30T22:20:03.913240+00:00",
+            "version": "4"
         },
         "vscode": {
             "interpreter": {
                 "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
     },
```

### Comparing `lamindb-0.9.4/docs/guide/A6-insert-update-delete.ipynb` & `lamindb-0.9.6/docs/guide/A6-insert-update-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A7-pipeline.ipynb` & `lamindb-0.9.6/docs/guide/A7-pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/A8-introspect.ipynb` & `lamindb-0.9.6/docs/guide/A8-introspect.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/B1-setup.ipynb` & `lamindb-0.9.6/docs/guide/B1-setup.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9919549851190477%*

 * *Differences: {"'cells'": "{12: {'source': {delete: [1]}}, 13: {'source': {delete: [1]}}, 14: {'source': "*

 * *            '{delete: [1]}}}',*

 * * "'metadata'": '{\'kernelspec\': {\'display_name\': "Python 3.9.13 (\'py39\')"}, '*

 * *               "'language_info': {'version': '3.9.13'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754'}}}"}*

```diff
@@ -121,41 +121,38 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "01dab8b0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.db.insert.project(\n",
-                "    external_id=\"P001\",\n",
                 "    name=\"Optimizing gRNA transfection in primary human T cells\",\n",
                 ");"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a1d911ac",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.db.insert.project(\n",
-                "    external_id=\"P002\",\n",
                 "    name=\"T cell enrichment from human PBMCs\",\n",
                 ");"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "881f05ec",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.db.insert.project(\n",
-                "    external_id=\"P003\",\n",
                 "    name=(\n",
                 "        \"CRISPR activation screens to decode stimulation responses in\"\n",
                 "        \" primary human T cells\"\n",
                 "    ),\n",
                 ");"
             ]
         },
@@ -166,39 +163,39 @@
             "source": [
                 "The 3rd project here is based on [Schmidt _et al._, Science (2022)](https://www.science.org/doi/10.1126/science.abj4008)."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3.9.12 ('base1')",
+            "display_name": "Python 3.9.13 ('py39')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.13"
         },
         "nbproject": {
             "id": "1qgezw298UrW",
             "parent": null,
             "pypackage": null,
             "time_init": "2022-08-30T22:17:51.266023+00:00",
             "version": "draft"
         },
         "vscode": {
             "interpreter": {
-                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
+                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lamindb-0.9.4/docs/guide/B2-design-experiment.ipynb` & `lamindb-0.9.6/docs/guide/B2-design-experiment.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.983313235077348%*

 * *Differences: {"'cells'": '{6: {\'source\': [\'exp_type1 = ln.db.insert.experiment_type(efo_id="EFO:0030033", '*

 * *            'name="gRNA-seq")\\n\', \'exp_type1\']}, 7: {\'source\': [\'exp_type2 = '*

 * *            'ln.db.insert.experiment_type(efo_id="EFO:0008860", name="Perturb-Seq")\\n\', '*

 * *            "'exp_type2']}, 9: {'source': {insert: [(7, ')\\n'), (8, 'experiment1')], delete: [8, "*

 * *            "6]}}, 10: {'source': {insert: [(7, ')\\n'), (8, 'experiment2')], delete: [8, 6]}}, "*

 * *            '13: {\'source\': [\'speci […]*

```diff
@@ -44,57 +44,40 @@
             "metadata": {},
             "source": [
                 "## Register experiment level metadata"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c97c60a0",
-            "metadata": {},
-            "source": [
-                "Let's select for our project of interest:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "d1329b60",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "project = ln.db.select.project(external_id=\"P003\").one()\n",
-                "project"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "1c8b0836",
             "metadata": {},
             "source": [
                 "Next, we register two experiment types:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fb93306f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "exp_type1 = ln.db.insert.experiment_type(efo_id=\"EFO:0030033\", name=\"gRNA-seq\")"
+                "exp_type1 = ln.db.insert.experiment_type(efo_id=\"EFO:0030033\", name=\"gRNA-seq\")\n",
+                "exp_type1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3fb33754",
             "metadata": {},
             "outputs": [],
             "source": [
-                "exp_type2 = ln.db.insert.experiment_type(efo_id=\"EFO:0008860\", name=\"Perturb-Seq\")"
+                "exp_type2 = ln.db.insert.experiment_type(efo_id=\"EFO:0008860\", name=\"Perturb-Seq\")\n",
+                "exp_type2"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "90650cee",
             "metadata": {},
             "source": [
@@ -110,17 +93,17 @@
             "source": [
                 "experiment1 = ln.db.insert.experiment(\n",
                 "    external_id=\"EXP001\",\n",
                 "    name=(\n",
                 "        \"Genome-wide CRISPRi screen for functional regulators of cytokine production in\"\n",
                 "        \" response to stimulation\"\n",
                 "    ),\n",
-                "    project_id=project.id,\n",
                 "    experiment_type_id=exp_type1.id,\n",
-                ")"
+                ")\n",
+                "experiment1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f364dd1d",
             "metadata": {},
@@ -128,17 +111,17 @@
             "source": [
                 "experiment2 = ln.db.insert.experiment(\n",
                 "    external_id=\"EXP002\",\n",
                 "    name=(\n",
                 "        \"CRISPRa Perturb-seq for characterizing molecular phenotypes of cytokine\"\n",
                 "        \" regulators\"\n",
                 "    ),\n",
-                "    project_id=project.id,\n",
                 "    experiment_type_id=exp_type2.id,\n",
-                ")"
+                ")\n",
+                "experiment2"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2760be19",
             "metadata": {},
             "source": [
@@ -158,37 +141,40 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "245b1f1c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "species = ln.db.insert.species(common_name=\"human\")"
+                "species = ln.db.insert.species(common_name=\"human\")\n",
+                "species"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0f3e3c27",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cell_type = ln.db.insert.cell_type(ontology_id=\"CL:0000084\", name=\"T cell\")"
+                "cell_type = ln.db.insert.cell_type(ontology_id=\"CL:0000084\", name=\"T cell\")\n",
+                "cell_type"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ba10bd72",
             "metadata": {},
             "outputs": [],
             "source": [
                 "tissue = ln.db.insert.tissue(\n",
                 "    ontology_id=\"CL:2000001\", name=\"peripheral blood mononuclear cell\"\n",
-                ")"
+                ")\n",
+                "tissue"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8a27dd22",
             "metadata": {},
@@ -197,15 +183,16 @@
                 "biosample = ln.db.insert.biosample(\n",
                 "    external_id=\"S1\",\n",
                 "    name=\"primary human T cell\",\n",
                 "    batch=\"1\",\n",
                 "    species_id=species.id,\n",
                 "    cell_type_id=cell_type.id,\n",
                 "    tissue_id=tissue.id,\n",
-                ")"
+                ")\n",
+                "biosample"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d5be95da",
             "metadata": {},
             "source": [
@@ -223,25 +210,27 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "75535150",
             "metadata": {},
             "outputs": [],
             "source": [
-                "readout1 = ln.db.insert.readout(efo_id=\"EFO:0003024\")"
+                "readout1 = ln.db.insert.readout(efo_id=\"EFO:0003024\")\n",
+                "readout1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "84c0b062",
             "metadata": {},
             "outputs": [],
             "source": [
-                "readout2 = ln.db.insert.readout(efo_id=\"EFO:0008913\")"
+                "readout2 = ln.db.insert.readout(efo_id=\"EFO:0008913\")\n",
+                "readout2"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "47e1d597",
             "metadata": {},
             "source": [
@@ -259,27 +248,29 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9ec2eadf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "featureset1 = ln.db.insert.featureset(feature_entity=\"gene\", name=\"CRISPRa-geneset-1\")"
+                "featureset1 = ln.db.insert.featureset(feature_entity=\"gene\", name=\"CRISPRa-geneset-1\")\n",
+                "featureset1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1472a739",
             "metadata": {},
             "outputs": [],
             "source": [
                 "featureset2 = ln.db.insert.featureset(\n",
                 "    feature_entity=\"gene\", name=\"Perturbseq-geneset-1\"\n",
-                ")"
+                ")\n",
+                "featureset2"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9eefd6e0",
             "metadata": {},
             "source": [
@@ -291,36 +282,46 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c0415107",
             "metadata": {},
             "outputs": [],
             "source": [
-                "biometa1_id = ln.db.insert.biometa(\n",
+                "biometa1 = ln.db.insert.biometa(\n",
                 "    experiment_id=experiment1.id,\n",
                 "    biosample_id=biosample.id,\n",
                 "    readout_id=readout1.id,\n",
                 "    featureset_id=featureset1.id,\n",
-                ")"
+                ")\n",
+                "biometa1"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "692c16e2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "biometa2_id = ln.db.insert.biometa(\n",
+                "biometa2 = ln.db.insert.biometa(\n",
                 "    experiment_id=experiment2.id,\n",
                 "    biosample_id=biosample.id,\n",
                 "    readout_id=readout2.id,\n",
                 "    featureset_id=featureset2.id,\n",
-                ")"
+                ")\n",
+                "biometa2"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0349d57d",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -331,15 +332,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.13"
         },
         "nbproject": {
             "id": "W4oWHHbY0oG6",
             "parent": null,
             "pypackage": null,
             "time_init": "2022-08-30T22:19:33.279387+00:00",
             "version": "draft"
```

### Comparing `lamindb-0.9.4/docs/guide/B3-perform-experiment.ipynb` & `lamindb-0.9.6/docs/guide/B3-perform-experiment.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9697498139880952%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(2, 'ingest.commit(i_confirm_i_saved=True)')], delete: "*

 * *            "[2]}}, insert: [(7, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('id', '4af1a86c'), ('metadata', OrderedDict()), ('outputs', []), ('source', [])]))]}",*

 * * "'metadata'": '{\'kernelspec\': {\'display_name\': "Python 3.9.13 (\'py39\')"}, '*

 * *               "'language_info': {'version': '3.9.13'}, 'nbproject': {'pypackage': {'lamindb': "*

 * *               "'0.6.0'}, 'user_handle […]*

```diff
@@ -62,47 +62,58 @@
             "execution_count": null,
             "id": "868a219c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ingest = ln.db.Ingest()\n",
                 "ingest.add(filepath)\n",
-                "ingest.commit()"
+                "ingest.commit(i_confirm_i_saved=True)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "4af1a86c",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3.9.13 ('py39')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.13"
         },
         "nbproject": {
             "id": "ddbsqoSJPFSJ",
             "parent": null,
             "pypackage": {
-                "lamindb": "0.3.3"
+                "lamindb": "0.6.0"
             },
             "time_init": "2022-08-30T22:20:56.505044+00:00",
+            "user_handle": "testuser1",
+            "user_id": "DzTjkKse",
+            "user_name": "Test User1",
             "version": "5"
         },
         "vscode": {
             "interpreter": {
-                "hash": "2775e555cdc2d728c54aa22130c79afb1fa4da64f22f2fc6dcc2aa346c4e0672"
+                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lamindb-0.9.4/docs/guide/B4-analyze-assay.ipynb` & `lamindb-0.9.6/docs/guide/B4-analyze-assay.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9797192433359213%*

 * *Differences: {"'cells'": '{5: {\'source\': ["Let\'s check which experiments the `testuser1` has registered:"]}, '*

 * *            '6: {\'source\': [\'ln.db.select.experiment(external_id="EXP001").df()\']}, 18: '*

 * *            "{'source': {insert: [(3, ').link_features(feature_model, "*

 * *            'featureset_name="CRISPRa-geneset-1");\')], delete: [3]}}, 19: {\'source\': {insert: '*

 * *            "[(3, ').link_features(feature_model, "*

 * *            'featureset_name="schmidt22_crispra_gws_IFNG_hits");\')], delete: [3]}}, 20: '*

 * *    […]*

```diff
@@ -49,35 +49,25 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e18de864",
             "metadata": {},
             "source": [
-                "Let's check which experiments the `testuser1` has registered for project P001:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "b1e0b60d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.db.select.project(external_id=\"P001\").df()"
+                "Let's check which experiments the `testuser1` has registered:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d18db94c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.db.select.experiment(project_id=1).df()"
+                "ln.db.select.experiment(external_id=\"EXP001\").df()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e156c30e",
             "metadata": {},
@@ -188,39 +178,47 @@
             "id": "002696c8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ingest.add(\n",
                 "    df,\n",
                 "    name=\"schmidt22_crispra_gws_IFNG_analyzed\",\n",
-                ").link_features(feature_model, featureset_name=\"CRISPRa-geneset-1\")"
+                ").link_features(feature_model, featureset_name=\"CRISPRa-geneset-1\");"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "47edadbf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ingest.add(\n",
                 "    hits_df,\n",
                 "    name=\"schmidt22_crispra_gws_IFNG_hits\",\n",
-                ").link_features(feature_model, featureset_name=\"schmidt22_crispra_gws_IFNG_hits\")"
+                ").link_features(feature_model, featureset_name=\"schmidt22_crispra_gws_IFNG_hits\");"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c44c407e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ingest.commit()"
+                "ingest.commit(i_confirm_i_saved=True)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "0406d857",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -231,25 +229,28 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.13"
         },
         "nbproject": {
             "id": "PtTXoc0RbOIq",
             "parent": null,
             "pypackage": {
-                "bionty": "0.0.6+17.g0499eed",
-                "lamindb": "0.3.3",
-                "pandas": "1.4.3"
+                "bionty": "0.3.2",
+                "lamindb": "0.6.0",
+                "pandas": "1.5.0"
             },
             "time_init": "2022-08-30T22:14:41.728518+00:00",
+            "user_handle": "testuser1",
+            "user_id": "DzTjkKse",
+            "user_name": "Test User1",
             "version": "6"
         },
         "vscode": {
             "interpreter": {
                 "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
```

### Comparing `lamindb-0.9.4/docs/guide/B5-bfx.ipynb` & `lamindb-0.9.6/docs/guide/B5-bfx.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/docs/guide/B7-dataflow.ipynb` & `lamindb-0.9.6/docs/guide/B7-dataflow.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9906374007936508%*

 * *Differences: {"'cells'": "{5: {'source': "*

 * *            "['ln.db.select.dobject(where=dict(gene=dict(ncbi_gene_id=9535))).all()']}, 6: "*

 * *            '{\'source\': [\'ln.db.select.dobject(where=dict(gene=dict(symbol="IFNG"))).all()\']}}',*

 * * "'metadata'": '{\'kernelspec\': {\'display_name\': "Python 3.9.13 (\'py39\')"}, '*

 * *               "'language_info': {'version': '3.9.13'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754'}}}"}*

```diff
@@ -53,25 +53,25 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bae693d0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# ln.db.select.dobject(where={\"gene\": {\"ncbi_gene_id\": 9535}}).all()"
+                "ln.db.select.dobject(where=dict(gene=dict(ncbi_gene_id=9535))).all()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e5df9770",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# ln.db.select.dobject(where={\"gene\": {\"symbol\": \"IFNG\"}}).all()"
+                "ln.db.select.dobject(where=dict(gene=dict(symbol=\"IFNG\"))).all()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c6d07db2",
             "metadata": {},
             "source": [
@@ -113,39 +113,39 @@
             "source": [
                 "You can also select any sample level biological entities"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3.9.13 ('py39')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.9.13"
         },
         "nbproject": {
             "id": "ZbOkNEck4fZR",
             "parent": null,
             "pypackage": null,
             "time_init": "2022-08-30T22:20:30.996102+00:00",
             "version": "draft"
         },
         "vscode": {
             "interpreter": {
-                "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
+                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lamindb-0.9.4/docs/index.md` & `lamindb-0.9.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/__init__.py` & `lamindb-0.9.6/lamindb/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
    settings
    datasets
    nb
    dev
 
 """
 
-__version__ = "0.9.4"
+__version__ = "0.9.6"
 
 import warnings
 
 from lndb_setup import settings  # noqa
 from lndb_setup._migrate import check_migrate as _check_migrate
 
 from . import _check_versions  # executes checks during import
```

### Comparing `lamindb-0.9.4/lamindb/_check_versions.py` & `lamindb-0.9.6/lamindb/_check_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from lndb_setup import __version__ as lndb_setup_v
 from lnschema_bionty import __version__ as lnschema_bionty_v
 from lnschema_core import __version__ as lnschema_core_v
 from lnschema_wetlab import __version__ as lnschema_wetlab_v
 from nbproject import __version__ as nbproject_v
 from packaging import version
 
-if version.parse(lnschema_core_v) != version.parse("0.13.0"):
-    raise RuntimeError("lamindb needs lnschema_core==0.13.0")
+if version.parse(lnschema_core_v) != version.parse("0.14.0"):
+    raise RuntimeError("lamindb needs lnschema_core==0.14.0")
 
-if version.parse(lnschema_wetlab_v) != version.parse("0.5.0"):
-    raise RuntimeError("lamindb needs lnschema_wetlab==0.5.0")
+if version.parse(lnschema_wetlab_v) != version.parse("0.7.2"):
+    raise RuntimeError("lamindb needs lnschema_wetlab==0.7.2")
 
 if version.parse(lnschema_bionty_v) != version.parse("0.4.3"):
     raise RuntimeError("lamindb needs lnschema_bionty==0.4.3")
 
-if version.parse(lndb_setup_v) != version.parse("0.12.1"):
-    raise RuntimeError("lamindb needs lndb_setup==0.12.1")
+if version.parse(lndb_setup_v) != version.parse("0.12.2"):
+    raise RuntimeError("lamindb needs lndb_setup==0.12.2")
 
 if version.parse(lndb_hub_v) != version.parse("0.5.6"):
     raise RuntimeError("lamindb needs lndb_hub==0.5.6")
 
 if version.parse(nbproject_v) < version.parse("0.7.0"):
     raise RuntimeError("lamindb needs nbproject>=0.7.0")
 
-if version.parse(lnbfx_v) < version.parse("0.4.2"):
-    raise RuntimeError("lamindb needs lnbfx>=0.4.2")
+if version.parse(lnbfx_v) < version.parse("0.4.4"):
+    raise RuntimeError("lamindb needs lnbfx>=0.4.4")
 
 if version.parse(bioreadout_v) < version.parse("0.2.1"):
     raise RuntimeError("lamindb needs bioreadout>=0.2.1")
```

### Comparing `lamindb-0.9.4/lamindb/datasets/_core.py` & `lamindb-0.9.6/lamindb/datasets/_core.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/db/__init__.py` & `lamindb-0.9.6/lamindb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/db/_delete.py` & `lamindb-0.9.6/lamindb/db/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/db/_ingest.py` & `lamindb-0.9.6/lamindb/db/_ingest.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/db/_load.py` & `lamindb-0.9.6/lamindb/db/_load.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/db/_view.py` & `lamindb-0.9.6/lamindb/db/_view.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/_core.py` & `lamindb-0.9.6/lamindb/dev/_core.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_core.py` & `lamindb-0.9.6/lamindb/dev/db/_core.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_insert.py` & `lamindb-0.9.6/lamindb/dev/db/_insert.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_link.py` & `lamindb-0.9.6/lamindb/dev/db/_link.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_select.py` & `lamindb-0.9.6/lamindb/dev/db/_select.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_select_result.py` & `lamindb-0.9.6/lamindb/dev/db/_select_result.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_staged.py` & `lamindb-0.9.6/lamindb/dev/db/_staged.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/db/_update.py` & `lamindb-0.9.6/lamindb/dev/db/_update.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/file/_file.py` & `lamindb-0.9.6/lamindb/dev/file/_file.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/file/_zarr.py` & `lamindb-0.9.6/lamindb/dev/file/_zarr.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/object/_anndata.py` & `lamindb-0.9.6/lamindb/dev/object/_anndata.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/dev/object/_core.py` & `lamindb-0.9.6/lamindb/dev/object/_core.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/schema/__init__.py` & `lamindb-0.9.6/lamindb/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/schema/_core.py` & `lamindb-0.9.6/lamindb/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/lamindb/schema/_table.py` & `lamindb-0.9.6/lamindb/schema/_table.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/noxfile.py` & `lamindb-0.9.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/pyproject.toml` & `lamindb-0.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [project]
 name = "lamindb"
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # Lamin pinned packages
-    "lnschema_core==0.13.0",
-    "lnschema_wetlab==0.5.0",
+    "lnschema_core==0.14.0",
+    "lnschema_wetlab==0.7.2",
     "lnschema_bionty==0.4.3",
-    "lndb_setup==0.12.1",
-    "lnbfx==0.4.2",
+    "lndb_setup==0.12.2",
+    "lnbfx==0.4.4",
     "lndb_hub==0.5.6",
     "bioreadout==0.2.1",
     "bionty>=0.3.1",
     "nbproject>=0.7.0",
     "readfcs",
     "lamin_logger",
     # External packages
```

### Comparing `lamindb-0.9.4/tests/test_conversion.py` & `lamindb-0.9.6/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/tests/test_db.py` & `lamindb-0.9.6/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/tests/test_file.py` & `lamindb-0.9.6/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `lamindb-0.9.4/PKG-INFO` & `lamindb-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lamindb
-Version: 0.9.4
+Version: 0.9.6
 Summary: LaminDB: Manage data & analyses.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnschema_core==0.13.0
-Requires-Dist: lnschema_wetlab==0.5.0
+Requires-Dist: lnschema_core==0.14.0
+Requires-Dist: lnschema_wetlab==0.7.2
 Requires-Dist: lnschema_bionty==0.4.3
-Requires-Dist: lndb_setup==0.12.1
-Requires-Dist: lnbfx==0.4.2
+Requires-Dist: lndb_setup==0.12.2
+Requires-Dist: lnbfx==0.4.4
 Requires-Dist: lndb_hub==0.5.6
 Requires-Dist: bioreadout==0.2.1
 Requires-Dist: bionty>=0.3.1
 Requires-Dist: nbproject>=0.7.0
 Requires-Dist: readfcs
 Requires-Dist: lamin_logger
 Requires-Dist: anndata
```

