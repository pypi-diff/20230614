# Comparing `tmp/unstructured-0.7.4.tar.gz` & `tmp/unstructured-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.7.4.tar", last modified: Mon Jun 12 18:57:23 2023, max compression
+gzip compressed data, was "unstructured-0.7.5.tar", last modified: Wed Jun 14 06:10:10 2023, max compression
```

## Comparing `unstructured-0.7.4.tar` & `unstructured-0.7.5.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.223657 unstructured-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-12 18:57:12.000000 unstructured-0.7.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-12 18:57:12.000000 unstructured-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-12 18:57:23.223657 unstructured-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-06-12 18:57:12.000000 unstructured-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.199657 unstructured-0.7.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/huggingface.in
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-azure.in
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-discord.in
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-github.in
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-gitlab.in
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-google-drive.in
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-reddit.in
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-s3.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-slack.in
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/ingest-wikipedia.in
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 18:57:12.000000 unstructured-0.7.4/requirements/local-inference.in
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-12 18:57:23.223657 unstructured-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-12 18:57:12.000000 unstructured-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.199657 unstructured-0.7.4/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-12 18:57:12.000000 unstructured-0.7.4/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.207657 unstructured-0.7.4/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.207657 unstructured-0.7.4/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.207657 unstructured-0.7.4/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.211657 unstructured-0.7.4/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.211657 unstructured-0.7.4/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.211657 unstructured-0.7.4/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.215657 unstructured-0.7.4/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.219657 unstructured-0.7.4/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.223657 unstructured-0.7.4/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/staging/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-12 18:57:12.000000 unstructured-0.7.4/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 18:57:23.203657 unstructured-0.7.4/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-12 18:57:23.000000 unstructured-0.7.4/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 18:57:22.000000 unstructured-0.7.4/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.747967 unstructured-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-14 06:09:58.000000 unstructured-0.7.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-14 06:09:58.000000 unstructured-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-14 06:10:10.747967 unstructured-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14627 2023-06-14 06:09:58.000000 unstructured-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.723967 unstructured-0.7.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/huggingface.in
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-azure.in
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-discord.in
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-github.in
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-gitlab.in
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-google-drive.in
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-reddit.in
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-s3.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-slack.in
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/ingest-wikipedia.in
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 06:09:58.000000 unstructured-0.7.5/requirements/local-inference.in
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-14 06:10:10.751967 unstructured-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-14 06:09:58.000000 unstructured-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.723967 unstructured-0.7.5/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-14 06:09:58.000000 unstructured-0.7.5/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.731967 unstructured-0.7.5/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.731967 unstructured-0.7.5/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.731967 unstructured-0.7.5/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.735967 unstructured-0.7.5/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.735967 unstructured-0.7.5/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24579 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.735967 unstructured-0.7.5/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.743967 unstructured-0.7.5/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.747967 unstructured-0.7.5/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.747967 unstructured-0.7.5/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/staging/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-14 06:09:58.000000 unstructured-0.7.5/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 06:10:10.727967 unstructured-0.7.5/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-14 06:10:10.000000 unstructured-0.7.5/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.7.4/LICENSE.md` & `unstructured-0.7.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/PKG-INFO` & `unstructured-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.4
+Version: 0.7.5
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -104,14 +104,15 @@
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
+        | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.4 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.5 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -67,17 +67,18 @@
 Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include
-Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
-| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
+Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
+Include Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes |
+None | | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.4/README.md` & `unstructured-0.7.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
 | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
 | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
 | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
 | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
 | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
+| ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
 | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
 | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
 | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
 | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
```

#### html2text {}

```diff
@@ -63,17 +63,18 @@
 Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include
-Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
-| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
+Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
+Include Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes |
+None | | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.4/setup.py` & `unstructured-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.7.5/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.7.5/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/test_unstructured/test_utils.py` & `unstructured-0.7.5/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/cleaners/core.py` & `unstructured-0.7.5/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/cleaners/extract.py` & `unstructured-0.7.5/unstructured/cleaners/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 import re
-from typing import List
+from typing import List, Optional
 
 from unstructured.nlp.patterns import (
     EMAIL_ADDRESS_PATTERN,
     EMAIL_DATETIMETZ_PATTERN,
     IP_ADDRESS_NAME_PATTERN,
     IP_ADDRESS_PATTERN_RE,
     MAPI_ID_PATTERN,
@@ -71,17 +71,20 @@
 
 def extract_mapi_id(text: str) -> List[str]:
     mapi_ids = re.findall(MAPI_ID_PATTERN, text)
     mapi_ids = [mid.replace(";", "") for mid in mapi_ids]
     return mapi_ids
 
 
-def extract_datetimetz(text: str) -> datetime.datetime:
-    date_string = re.findall(EMAIL_DATETIMETZ_PATTERN, text)
-    return datetime.datetime.strptime(date_string[0], "%a, %d %b %Y %H:%M:%S %z")
+def extract_datetimetz(text: str) -> Optional[datetime.datetime]:
+    date_extractions = re.findall(EMAIL_DATETIMETZ_PATTERN, text)
+    if len(date_extractions) > 0:
+        return datetime.datetime.strptime(date_extractions[0], "%a, %d %b %Y %H:%M:%S %z")
+    else:
+        return None
 
 
 def extract_us_phone_number(text: str):
     """Extracts a US phone number from a section of text that includes a phone number. If there
     is no phone number present, the result will be an empty string.
 
     Example
```

### Comparing `unstructured-0.7.4/unstructured/cleaners/translate.py` & `unstructured-0.7.5/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/documents/base.py` & `unstructured-0.7.5/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/documents/elements.py` & `unstructured-0.7.5/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/documents/email_elements.py` & `unstructured-0.7.5/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/documents/html.py` & `unstructured-0.7.5/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/documents/xml.py` & `unstructured-0.7.5/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/file_utils/encoding.py` & `unstructured-0.7.5/unstructured/file_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/file_utils/exploration.py` & `unstructured-0.7.5/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/file_utils/file_conversion.py` & `unstructured-0.7.5/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/file_utils/filetype.py` & `unstructured-0.7.5/unstructured/file_utils/filetype.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import os
 import re
 import zipfile
 from enum import Enum
 from functools import wraps
 from typing import IO, Callable, List, Optional
 
-import filetype as ft
-
 from unstructured.documents.elements import Element, PageBreak
 from unstructured.file_utils.encoding import detect_file_encoding
 from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import (
     _add_element_metadata,
     _remove_element_metadata,
     exactly_one,
@@ -78,14 +76,15 @@
     CSV = 44
 
     # Markup Types
     HTML = 50
     XML = 51
     MD = 52
     EPUB = 53
+    RST = 54
 
     # Compressed Types
     ZIP = 60
 
     # Open Office Types
     ODT = 70
 
@@ -105,14 +104,15 @@
     "application/csv": FileType.CSV,
     "application/x-csv": FileType.CSV,
     "text/comma-separated-values": FileType.CSV,
     "text/x-comma-separated-values": FileType.CSV,
     "text/csv": FileType.CSV,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
+    "text/x-rst": FileType.RST,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
     "application/json": FileType.JSON,
     "application/rtf": FileType.RTF,
     "text/rtf": FileType.RTF,
     "text/html": FileType.HTML,
     "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet": FileType.XLSX,
@@ -148,14 +148,15 @@
     ".text": FileType.TXT,
     ".log": FileType.TXT,
     ".eml": FileType.EML,
     ".xml": FileType.XML,
     ".htm": FileType.HTML,
     ".html": FileType.HTML,
     ".md": FileType.MD,
+    ".rst": FileType.RST,
     ".xlsx": FileType.XLSX,
     ".pptx": FileType.PPTX,
     ".png": FileType.PNG,
     ".doc": FileType.DOC,
     ".zip": FileType.ZIP,
     ".xls": FileType.XLS,
     ".ppt": FileType.PPT,
@@ -217,26 +218,30 @@
         extension = extension.lower()
         if os.path.isfile(_filename) and LIBMAGIC_AVAILABLE:
             mime_type = magic.from_file(
                 _resolve_symlink(filename or file_filename),
                 mime=True,
             )  # type: ignore
         elif os.path.isfile(_filename):
+            import filetype as ft
+
             mime_type = ft.guess_mime(filename)
         if mime_type is None:
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
 
     elif file is not None:
         extension = None
         # NOTE(robinson) - the python-magic docs recommend reading at least the first 2048 bytes
         # Increased to 4096 because otherwise .xlsx files get detected as a zip file
         # ref: https://github.com/ahupp/python-magic#usage
         if LIBMAGIC_AVAILABLE:
             mime_type = magic.from_buffer(file.read(4096), mime=True)
         else:
+            import filetype as ft
+
             mime_type = ft.guess_mime(file.read(4096))
         if mime_type is None:
             logger.warning(
                 "libmagic is unavailable but assists in filetype detection on file-like objects."
                 "Please consider installing libmagic for better results.",
             )
             return EXT_TO_FILETYPE.get(extension, FileType.UNK)
@@ -263,14 +268,16 @@
             return FileType.XML
 
     elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
         if extension and extension == ".eml":
             return FileType.EML
         elif extension and extension == ".md":
             return FileType.MD
+        elif extension and extension == ".rst":
+            return FileType.RST
         elif extension and extension == ".rtf":
             return FileType.RTF
         elif extension and extension == ".html":
             return FileType.HTML
 
         if _is_text_file_a_json(file=file, filename=filename, encoding=encoding):
             return FileType.JSON
```

### Comparing `unstructured-0.7.4/unstructured/file_utils/metadata.py` & `unstructured-0.7.5/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/azure.py` & `unstructured-0.7.5/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/biomed.py` & `unstructured-0.7.5/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/discord.py` & `unstructured-0.7.5/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/fsspec.py` & `unstructured-0.7.5/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/git.py` & `unstructured-0.7.5/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/github.py` & `unstructured-0.7.5/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/gitlab.py` & `unstructured-0.7.5/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/google_drive.py` & `unstructured-0.7.5/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/local.py` & `unstructured-0.7.5/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/reddit.py` & `unstructured-0.7.5/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/s3.py` & `unstructured-0.7.5/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/slack.py` & `unstructured-0.7.5/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.7.5/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.7.5/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/ingest/interfaces.py` & `unstructured-0.7.5/unstructured/ingest/interfaces.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     download_only: bool = False
     fields_include: str = "element_id,text,type,metadata"
     flatten_metadata: bool = False
     metadata_exclude: Optional[str] = None
     metadata_include: Optional[str] = None
     partition_by_api: bool = False
     partition_endpoint: str = "https://api.unstructured.io/general/v0/general"
+    api_key: str = ""
     preserve_downloads: bool = False
     re_download: bool = False
 
 
 class BaseConnectorConfig(ABC):
     """Abstract definition on which to define connector-specific attributes."""
 
@@ -175,17 +176,21 @@
 
         else:
             endpoint = self.standard_config.partition_endpoint
 
             logger.debug(f"Using remote partition ({endpoint})")
 
             with open(self.filename, "rb") as f:
+                headers_dict = {}
+                if len(self.standard_config.api_key) > 0:
+                    headers_dict["UNSTRUCTURED-API-KEY"] = self.standard_config.api_key
                 response = requests.post(
                     f"{endpoint}",
                     files={"files": (str(self.filename), f)},
+                    headers=headers_dict,
                     # TODO: add m_data_source_metadata to unstructured-api pipeline_api and then
                     # pass the stringified json here
                 )
 
             if response.status_code != 200:
                 raise RuntimeError(f"Caught {response.status_code} from API: {response.text}")
```

### Comparing `unstructured-0.7.4/unstructured/ingest/main.py` & `unstructured-0.7.5/unstructured/ingest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,19 @@
 @click.option(
     "--partition-strategy",
     default="auto",
     help="The method that will be used to process the documents. "
     "Default: auto. Other strategies include `fast` and `hi_res`.",
 )
 @click.option(
+    "--api-key",
+    default="",
+    help="API Key for partition endpoint.",
+)
+@click.option(
     "--local-input-path",
     default=None,
     help="Path to the location in the local file system that will be processed.",
 )
 @click.option(
     "--local-recursive",
     is_flag=True,
@@ -439,14 +444,15 @@
     metadata_exclude,
     fields_include,
     flatten_metadata,
     max_docs,
     partition_by_api,
     partition_endpoint,
     partition_strategy,
+    api_key,
     local_input_path,
     local_recursive,
     local_file_glob,
     download_only,
 ):
     default_values = collections.Counter([option.default for option in ctx.command.params])
     passed_values = collections.Counter(ctx.params.values())
@@ -541,14 +547,15 @@
         flatten_metadata=flatten_metadata,
         metadata_exclude=metadata_exclude,
         metadata_include=metadata_include,
         partition_by_api=partition_by_api,
         partition_endpoint=partition_endpoint,
         preserve_downloads=preserve_downloads,
         re_download=re_download,
+        api_key=api_key,
     )
     if remote_url:
         protocol = urlparse(remote_url).scheme
         if protocol in ("s3", "s3a"):
             from unstructured.ingest.connector.s3 import S3Connector, SimpleS3Config
 
             doc_connector = S3Connector(  # type: ignore
```

### Comparing `unstructured-0.7.4/unstructured/nlp/english-words.txt` & `unstructured-0.7.5/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/nlp/english_words.py` & `unstructured-0.7.5/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/nlp/patterns.py` & `unstructured-0.7.5/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/nlp/tokenize.py` & `unstructured-0.7.5/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/__init__.py` & `unstructured-0.7.5/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/api.py` & `unstructured-0.7.5/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/auto.py` & `unstructured-0.7.5/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from unstructured.partition.json import partition_json
 from unstructured.partition.md import partition_md
 from unstructured.partition.msg import partition_msg
 from unstructured.partition.odt import partition_odt
 from unstructured.partition.pdf import partition_pdf
 from unstructured.partition.ppt import partition_ppt
 from unstructured.partition.pptx import partition_pptx
+from unstructured.partition.rst import partition_rst
 from unstructured.partition.rtf import partition_rtf
 from unstructured.partition.text import partition_text
 from unstructured.partition.xlsx import partition_xlsx
 from unstructured.partition.xml import partition_xml
 
 
 def partition(
@@ -144,14 +145,20 @@
         )
     elif filetype == FileType.EPUB:
         elements = partition_epub(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
         )
+    elif filetype == FileType.RST:
+        elements = partition_rst(
+            filename=filename,
+            file=file,
+            include_page_breaks=include_page_breaks,
+        )
     elif filetype == FileType.MD:
         elements = partition_md(
             filename=filename,
             file=file,
             include_page_breaks=include_page_breaks,
         )
     elif filetype == FileType.PDF:
```

### Comparing `unstructured-0.7.4/unstructured/partition/common.py` & `unstructured-0.7.5/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/csv.py` & `unstructured-0.7.5/unstructured/partition/csv.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/doc.py` & `unstructured-0.7.5/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/docx.py` & `unstructured-0.7.5/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/email.py` & `unstructured-0.7.5/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/epub.py` & `unstructured-0.7.5/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/html.py` & `unstructured-0.7.5/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/image.py` & `unstructured-0.7.5/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/json.py` & `unstructured-0.7.5/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/md.py` & `unstructured-0.7.5/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/msg.py` & `unstructured-0.7.5/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/odt.py` & `unstructured-0.7.5/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/pdf.py` & `unstructured-0.7.5/unstructured/partition/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,15 @@
     elements: List[Element] = []
 
     for i, page in enumerate(extract_pages(fp)):  # type: ignore
         metadata = ElementMetadata(filename=filename, page_number=i + 1)
         height = page.height
 
         text_segments = []
+        page_elements = []
         for obj in page:
             x1, y2, x2, y1 = obj.bbox
             y1 = height - y1
             y2 = height - y2
 
             # NOTE(robinson) - "Figure" is an example of an object type that does
             # not have a get_text method
@@ -282,15 +283,24 @@
             _text = re.sub(PARAGRAPH_PATTERN, " ", _text)
             _text = clean_extra_whitespace(_text)
             if _text.strip():
                 text_segments.append(_text)
                 element = element_from_text(_text)
                 element.coordinates = ((x1, y1), (x1, y2), (x2, y2), (x2, y1))
                 element.metadata = metadata
-                elements.append(element)
+                page_elements.append(element)
+
+        sorted_page_elements = sorted(
+            page_elements,
+            key=lambda el: (
+                el.coordinates[0][1] if el.coordinates else float("inf"),
+                el.coordinates[0][0] if el.coordinates else float("inf"),
+            ),
+        )
+        elements += sorted_page_elements
 
         if include_page_breaks:
             elements.append(PageBreak())
 
     return elements
```

### Comparing `unstructured-0.7.4/unstructured/partition/ppt.py` & `unstructured-0.7.5/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/pptx.py` & `unstructured-0.7.5/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/rtf.py` & `unstructured-0.7.5/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/strategies.py` & `unstructured-0.7.5/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/text.py` & `unstructured-0.7.5/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/text_type.py` & `unstructured-0.7.5/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/xlsx.py` & `unstructured-0.7.5/unstructured/partition/xlsx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/partition/xml.py` & `unstructured-0.7.5/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/argilla.py` & `unstructured-0.7.5/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/base.py` & `unstructured-0.7.5/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/baseplate.py` & `unstructured-0.7.5/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/datasaur.py` & `unstructured-0.7.5/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/huggingface.py` & `unstructured-0.7.5/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/label_box.py` & `unstructured-0.7.5/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/label_studio.py` & `unstructured-0.7.5/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/prodigy.py` & `unstructured-0.7.5/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/staging/weaviate.py` & `unstructured-0.7.5/unstructured/staging/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured/utils.py` & `unstructured-0.7.5/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.7.4/unstructured.egg-info/PKG-INFO` & `unstructured-0.7.5/unstructured.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.7.4
+Version: 0.7.5
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -104,14 +104,15 @@
         | Images (`.png`/`.jpg`) | `partition_image` | `"auto"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks |
         | Open Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None |
         | PDFs (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy |
         | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph Grouper |
         | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page Breaks |
         | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page Breaks |
+        | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include Page Breaks |
         | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include Page Breaks |
         | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
         | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None |
         | XML Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.7.4 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.7.5 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -67,17 +67,18 @@
 Markdown (`.md`) | `partitin_md` | N/A | Yes | Include Page Breaks | | Open
 Office Documents (`.odt`) | `partition_odt` | N/A | Yes | None | | PDFs
 (`.pdf`) | `partition_pdf` | `"auto"`, `"fast"`, `"hi_res"`, `"ocr_only"` | Yes
 | Encoding; Include Page Breaks; Infer Table Structure; OCR Languages, Strategy
 | | Plain Text (`.txt`) | `partition_text` | N/A | No | Encoding, Paragraph
 Grouper | | Power Points (`.ppt`) | `partition_ppt` | N/A | Yes | Include Page
 Breaks | | Power Points (`.pptx`) | `partition_pptx` | N/A | Yes | Include Page
-Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes | Include
-Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes | None |
-| Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
+Breaks | | ReStructured Text (`.rst`) | `partition_rst` | N/A | Yes | Include
+Page Breaks | | Rich Text Files (`.rtf`) | `partition_rtf` | N/A | Yes |
+Include Page Breaks | | Word Documents (`.doc`) | `partition_doc` | N/A | Yes |
+None | | Word Documents (`.docx`) | `partition_docx` | N/A | Yes | None | | XML
 Documents (`.xml`) | `partition_xml` | N/A | No | Encoding; XML Keep Tags | ##
 :dizzy: Instructions for using the docker image The following instructions are
 intended to help you get up and running using Docker to interact with
 `unstructured`. See [here](https://docs.docker.com/get-docker/) if you don't
 already have docker installed on your machine. NOTE: we build multi-platform
 images to support both x86_64 and Apple silicon hardware. `docker pull` should
 download the corresponding image for your architecture, but you can specify
```

### Comparing `unstructured-0.7.4/unstructured.egg-info/SOURCES.txt` & `unstructured-0.7.5/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 unstructured/partition/json.py
 unstructured/partition/md.py
 unstructured/partition/msg.py
 unstructured/partition/odt.py
 unstructured/partition/pdf.py
 unstructured/partition/ppt.py
 unstructured/partition/pptx.py
+unstructured/partition/rst.py
 unstructured/partition/rtf.py
 unstructured/partition/strategies.py
 unstructured/partition/text.py
 unstructured/partition/text_type.py
 unstructured/partition/xlsx.py
 unstructured/partition/xml.py
 unstructured/staging/__init__.py
```

