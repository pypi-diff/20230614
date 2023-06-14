# Comparing `tmp/ktrain-0.9.3.tar.gz` & `tmp/ktrain-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ktrain-0.9.3.tar", last modified: Tue Feb 11 20:30:45 2020, max compression
+gzip compressed data, was "dist/ktrain-0.9.4.tar", last modified: Thu Feb 13 21:39:11 2020, max compression
```

## Comparing `ktrain-0.9.3.tar` & `ktrain-0.9.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:45.000000 ktrain-0.9.3/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:44.000000 ktrain-0.9.3/ktrain/
--rwxrwx---   0 root         (0) vboxsf     (999)    61309 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/core.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3507 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/data.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:44.000000 ktrain-0.9.3/ktrain/graph/
--rwxrwx---   0 root         (0) vboxsf     (999)     9765 2019-12-11 21:58:35.000000 ktrain-0.9.3/ktrain/graph/data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2767 2019-10-16 17:25:36.000000 ktrain-0.9.3/ktrain/graph/learner.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2488 2020-01-14 19:30:25.000000 ktrain-0.9.3/ktrain/graph/models.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2489 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/graph/node_generator.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1590 2019-10-16 17:25:36.000000 ktrain-0.9.3/ktrain/graph/predictor.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5930 2020-02-07 20:08:16.000000 ktrain-0.9.3/ktrain/graph/preprocessor.py
--rwxrwx---   0 root         (0) vboxsf     (999)      194 2019-10-16 17:25:36.000000 ktrain-0.9.3/ktrain/graph/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6598 2020-01-14 19:30:25.000000 ktrain-0.9.3/ktrain/imports.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:44.000000 ktrain-0.9.3/ktrain/lroptimize/
--rwxrwx---   0 root         (0) vboxsf     (999)     6021 2020-01-27 19:10:29.000000 ktrain-0.9.3/ktrain/lroptimize/lrfinder.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3837 2019-08-13 01:50:24.000000 ktrain-0.9.3/ktrain/lroptimize/sgdr.py
--rwxrwx---   0 root         (0) vboxsf     (999)    11085 2019-12-30 21:47:15.000000 ktrain-0.9.3/ktrain/lroptimize/triangular.py
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2019-03-15 01:36:03.000000 ktrain-0.9.3/ktrain/lroptimize/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)      748 2020-01-14 19:30:25.000000 ktrain-0.9.3/ktrain/predictor.py
--rwxrwx---   0 root         (0) vboxsf     (999)      355 2019-08-13 01:49:06.000000 ktrain-0.9.3/ktrain/preprocessor.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:44.000000 ktrain-0.9.3/ktrain/text/
--rwxrwx---   0 root         (0) vboxsf     (999)    17494 2020-01-30 16:51:03.000000 ktrain-0.9.3/ktrain/text/data.py
--rwxrwx---   0 root         (0) vboxsf     (999)    28196 2019-12-04 17:25:39.000000 ktrain-0.9.3/ktrain/text/eda.py
--rwxrwx---   0 root         (0) vboxsf     (999)     8049 2020-01-30 16:51:03.000000 ktrain-0.9.3/ktrain/text/learner.py
--rwxrwx---   0 root         (0) vboxsf     (999)    20671 2020-01-30 16:51:03.000000 ktrain-0.9.3/ktrain/text/models.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:44.000000 ktrain-0.9.3/ktrain/text/ner/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:45.000000 ktrain-0.9.3/ktrain/text/ner/anago/
--rwxrwx---   0 root         (0) vboxsf     (999)     1163 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/callbacks.py
--rwxrwx---   0 root         (0) vboxsf     (999)    31267 2020-01-08 16:17:22.000000 ktrain-0.9.3/ktrain/text/ner/anago/layers.py
--rwxrwx---   0 root         (0) vboxsf     (999)    27158 2019-09-30 21:20:23.000000 ktrain-0.9.3/ktrain/text/ner/anago/layers_standalone.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4821 2020-01-08 16:17:19.000000 ktrain-0.9.3/ktrain/text/ner/anago/models.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5579 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/preprocessing.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3682 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/tagger.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2145 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/trainer.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7354 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/utils.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5234 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/wrapper.py
--rwxrwx---   0 root         (0) vboxsf     (999)       86 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/anago/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6979 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5474 2019-09-30 21:30:10.000000 ktrain-0.9.3/ktrain/text/ner/learner.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3748 2020-01-14 19:30:25.000000 ktrain-0.9.3/ktrain/text/ner/models.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1380 2019-09-23 18:15:25.000000 ktrain-0.9.3/ktrain/text/ner/predictor.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4850 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/text/ner/preprocessor.py
--rwxrwx---   0 root         (0) vboxsf     (999)      156 2019-09-30 21:20:23.000000 ktrain-0.9.3/ktrain/text/ner/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5886 2020-02-04 19:17:46.000000 ktrain-0.9.3/ktrain/text/predictor.py
--rwxrwx---   0 root         (0) vboxsf     (999)    36197 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/text/preprocessor.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5939 2019-12-04 17:25:39.000000 ktrain-0.9.3/ktrain/text/textutils.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1476 2020-01-30 16:51:03.000000 ktrain-0.9.3/ktrain/text/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)    13671 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/utils.py
--rwxrwx---   0 root         (0) vboxsf     (999)       48 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/version.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:45.000000 ktrain-0.9.3/ktrain/vision/
--rwxrwx---   0 root         (0) vboxsf     (999)    24891 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/vision/data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3453 2019-09-30 21:30:10.000000 ktrain-0.9.3/ktrain/vision/learner.py
--rwxrwx---   0 root         (0) vboxsf     (999)    14321 2019-09-30 21:20:23.000000 ktrain-0.9.3/ktrain/vision/models.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6594 2020-01-14 19:30:25.000000 ktrain-0.9.3/ktrain/vision/predictor.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3343 2019-08-13 01:52:15.000000 ktrain-0.9.3/ktrain/vision/preprocessor.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6313 2020-02-11 20:29:55.000000 ktrain-0.9.3/ktrain/vision/wrn.py
--rwxrwx---   0 root         (0) vboxsf     (999)      320 2019-08-13 01:52:15.000000 ktrain-0.9.3/ktrain/vision/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4685 2020-01-20 04:16:09.000000 ktrain-0.9.3/ktrain/__init__.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-11 20:30:44.000000 ktrain-0.9.3/ktrain.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2020-02-11 20:30:43.000000 ktrain-0.9.3/ktrain.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)    17764 2020-02-11 20:30:43.000000 ktrain-0.9.3/ktrain.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      203 2020-02-11 20:30:43.000000 ktrain-0.9.3/ktrain.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)     1489 2020-02-11 20:30:43.000000 ktrain-0.9.3/ktrain.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        7 2020-02-11 20:30:43.000000 ktrain-0.9.3/ktrain.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (999)    17764 2020-02-11 20:30:45.000000 ktrain-0.9.3/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)    15256 2020-02-02 03:10:58.000000 ktrain-0.9.3/README.md
--rwxrwx---   0 root         (0) vboxsf     (999)       79 2020-02-11 20:30:45.000000 ktrain-0.9.3/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1873 2020-01-22 21:09:18.000000 ktrain-0.9.3/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/
+-rwxrwx---   0 root         (0) vboxsf     (999)    61309 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/core.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3507 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/data.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/graph/
+-rwxrwx---   0 root         (0) vboxsf     (999)     9765 2019-12-11 21:58:35.000000 ktrain-0.9.4/ktrain/graph/data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2767 2019-10-16 17:25:36.000000 ktrain-0.9.4/ktrain/graph/learner.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2488 2020-01-14 19:30:25.000000 ktrain-0.9.4/ktrain/graph/models.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2489 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/graph/node_generator.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1590 2019-10-16 17:25:36.000000 ktrain-0.9.4/ktrain/graph/predictor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5930 2020-02-07 20:08:16.000000 ktrain-0.9.4/ktrain/graph/preprocessor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      194 2019-10-16 17:25:36.000000 ktrain-0.9.4/ktrain/graph/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6598 2020-01-14 19:30:25.000000 ktrain-0.9.4/ktrain/imports.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/lroptimize/
+-rwxrwx---   0 root         (0) vboxsf     (999)     6021 2020-01-27 19:10:29.000000 ktrain-0.9.4/ktrain/lroptimize/lrfinder.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3837 2019-08-13 01:50:24.000000 ktrain-0.9.4/ktrain/lroptimize/sgdr.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    11085 2019-12-30 21:47:15.000000 ktrain-0.9.4/ktrain/lroptimize/triangular.py
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2019-03-15 01:36:03.000000 ktrain-0.9.4/ktrain/lroptimize/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      748 2020-01-14 19:30:25.000000 ktrain-0.9.4/ktrain/predictor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      355 2019-08-13 01:49:06.000000 ktrain-0.9.4/ktrain/preprocessor.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/text/
+-rwxrwx---   0 root         (0) vboxsf     (999)    17494 2020-01-30 16:51:03.000000 ktrain-0.9.4/ktrain/text/data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    28196 2019-12-04 17:25:39.000000 ktrain-0.9.4/ktrain/text/eda.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     8049 2020-01-30 16:51:03.000000 ktrain-0.9.4/ktrain/text/learner.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    20671 2020-01-30 16:51:03.000000 ktrain-0.9.4/ktrain/text/models.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/text/ner/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/text/ner/anago/
+-rwxrwx---   0 root         (0) vboxsf     (999)     1163 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/callbacks.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    31267 2020-01-08 16:17:22.000000 ktrain-0.9.4/ktrain/text/ner/anago/layers.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    27158 2019-09-30 21:20:23.000000 ktrain-0.9.4/ktrain/text/ner/anago/layers_standalone.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4821 2020-01-08 16:17:19.000000 ktrain-0.9.4/ktrain/text/ner/anago/models.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5579 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/preprocessing.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3682 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/tagger.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2145 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/trainer.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7354 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/utils.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5234 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/wrapper.py
+-rwxrwx---   0 root         (0) vboxsf     (999)       86 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/anago/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6979 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5474 2019-09-30 21:30:10.000000 ktrain-0.9.4/ktrain/text/ner/learner.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3748 2020-01-14 19:30:25.000000 ktrain-0.9.4/ktrain/text/ner/models.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1380 2019-09-23 18:15:25.000000 ktrain-0.9.4/ktrain/text/ner/predictor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4850 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/text/ner/preprocessor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      156 2019-09-30 21:20:23.000000 ktrain-0.9.4/ktrain/text/ner/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5886 2020-02-04 19:17:46.000000 ktrain-0.9.4/ktrain/text/predictor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    36197 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/text/preprocessor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5939 2019-12-04 17:25:39.000000 ktrain-0.9.4/ktrain/text/textutils.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1476 2020-01-30 16:51:03.000000 ktrain-0.9.4/ktrain/text/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    13671 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/utils.py
+-rwxrwx---   0 root         (0) vboxsf     (999)       48 2020-02-13 21:38:57.000000 ktrain-0.9.4/ktrain/version.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain/vision/
+-rwxrwx---   0 root         (0) vboxsf     (999)    24891 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/vision/data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3453 2019-09-30 21:30:10.000000 ktrain-0.9.4/ktrain/vision/learner.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    14321 2019-09-30 21:20:23.000000 ktrain-0.9.4/ktrain/vision/models.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6594 2020-01-14 19:30:25.000000 ktrain-0.9.4/ktrain/vision/predictor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3343 2019-08-13 01:52:15.000000 ktrain-0.9.4/ktrain/vision/preprocessor.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6313 2020-02-11 20:29:55.000000 ktrain-0.9.4/ktrain/vision/wrn.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      320 2019-08-13 01:52:15.000000 ktrain-0.9.4/ktrain/vision/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4685 2020-01-20 04:16:09.000000 ktrain-0.9.4/ktrain/__init__.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2020-02-13 21:39:11.000000 ktrain-0.9.4/ktrain.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2020-02-13 21:39:10.000000 ktrain-0.9.4/ktrain.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)    17764 2020-02-13 21:39:10.000000 ktrain-0.9.4/ktrain.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      206 2020-02-13 21:39:10.000000 ktrain-0.9.4/ktrain.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)     1489 2020-02-13 21:39:10.000000 ktrain-0.9.4/ktrain.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        7 2020-02-13 21:39:10.000000 ktrain-0.9.4/ktrain.egg-info/top_level.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)    17764 2020-02-13 21:39:11.000000 ktrain-0.9.4/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)    15256 2020-02-02 03:10:58.000000 ktrain-0.9.4/README.md
+-rwxrwx---   0 root         (0) vboxsf     (999)       79 2020-02-13 21:39:12.000000 ktrain-0.9.4/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1876 2020-02-13 21:38:57.000000 ktrain-0.9.4/setup.py
```

### Comparing `ktrain-0.9.3/ktrain/core.py` & `ktrain-0.9.4/ktrain/core.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/data.py` & `ktrain-0.9.4/ktrain/data.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/graph/data.py` & `ktrain-0.9.4/ktrain/graph/data.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/graph/learner.py` & `ktrain-0.9.4/ktrain/graph/learner.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/graph/models.py` & `ktrain-0.9.4/ktrain/graph/models.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/graph/node_generator.py` & `ktrain-0.9.4/ktrain/graph/node_generator.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/graph/predictor.py` & `ktrain-0.9.4/ktrain/graph/predictor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/graph/preprocessor.py` & `ktrain-0.9.4/ktrain/graph/preprocessor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/imports.py` & `ktrain-0.9.4/ktrain/imports.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/lroptimize/lrfinder.py` & `ktrain-0.9.4/ktrain/lroptimize/lrfinder.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/lroptimize/sgdr.py` & `ktrain-0.9.4/ktrain/lroptimize/sgdr.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/lroptimize/triangular.py` & `ktrain-0.9.4/ktrain/lroptimize/triangular.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/predictor.py` & `ktrain-0.9.4/ktrain/predictor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/data.py` & `ktrain-0.9.4/ktrain/text/data.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/eda.py` & `ktrain-0.9.4/ktrain/text/eda.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/learner.py` & `ktrain-0.9.4/ktrain/text/learner.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/models.py` & `ktrain-0.9.4/ktrain/text/models.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/callbacks.py` & `ktrain-0.9.4/ktrain/text/ner/anago/callbacks.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/layers.py` & `ktrain-0.9.4/ktrain/text/ner/anago/layers.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/layers_standalone.py` & `ktrain-0.9.4/ktrain/text/ner/anago/layers_standalone.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/models.py` & `ktrain-0.9.4/ktrain/text/ner/anago/models.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/preprocessing.py` & `ktrain-0.9.4/ktrain/text/ner/anago/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/tagger.py` & `ktrain-0.9.4/ktrain/text/ner/anago/tagger.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/trainer.py` & `ktrain-0.9.4/ktrain/text/ner/anago/trainer.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/utils.py` & `ktrain-0.9.4/ktrain/text/ner/anago/utils.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/anago/wrapper.py` & `ktrain-0.9.4/ktrain/text/ner/anago/wrapper.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/data.py` & `ktrain-0.9.4/ktrain/text/ner/data.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/learner.py` & `ktrain-0.9.4/ktrain/text/ner/learner.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/models.py` & `ktrain-0.9.4/ktrain/text/ner/models.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/predictor.py` & `ktrain-0.9.4/ktrain/text/ner/predictor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/ner/preprocessor.py` & `ktrain-0.9.4/ktrain/text/ner/preprocessor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/predictor.py` & `ktrain-0.9.4/ktrain/text/predictor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/preprocessor.py` & `ktrain-0.9.4/ktrain/text/preprocessor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/textutils.py` & `ktrain-0.9.4/ktrain/text/textutils.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/text/__init__.py` & `ktrain-0.9.4/ktrain/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/utils.py` & `ktrain-0.9.4/ktrain/utils.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/vision/data.py` & `ktrain-0.9.4/ktrain/vision/data.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/vision/learner.py` & `ktrain-0.9.4/ktrain/vision/learner.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/vision/models.py` & `ktrain-0.9.4/ktrain/vision/models.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/vision/predictor.py` & `ktrain-0.9.4/ktrain/vision/predictor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/vision/preprocessor.py` & `ktrain-0.9.4/ktrain/vision/preprocessor.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/vision/wrn.py` & `ktrain-0.9.4/ktrain/vision/wrn.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain/__init__.py` & `ktrain-0.9.4/ktrain/__init__.py`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/ktrain.egg-info/PKG-INFO` & `ktrain-0.9.4/ktrain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktrain
-Version: 0.9.3
+Version: 0.9.4
 Summary: ktrain is a lightweight wrapper for TensorFlow Keras to help train neural networks
 Home-page: https://github.com/amaiya/ktrain
 Author: Arun S. Maiya
 Author-email: arun@maiya.net
 License: MIT
 Description: 
         # ktrain
```

### Comparing `ktrain-0.9.3/ktrain.egg-info/SOURCES.txt` & `ktrain-0.9.4/ktrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/PKG-INFO` & `ktrain-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktrain
-Version: 0.9.3
+Version: 0.9.4
 Summary: ktrain is a lightweight wrapper for TensorFlow Keras to help train neural networks
 Home-page: https://github.com/amaiya/ktrain
 Author: Arun S. Maiya
 Author-email: arun@maiya.net
 License: MIT
 Description: 
         # ktrain
```

### Comparing `ktrain-0.9.3/README.md` & `ktrain-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ktrain-0.9.3/setup.py` & `ktrain-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   author = 'Arun S. Maiya',
   author_email = 'arun@maiya.net',
   url = 'https://github.com/amaiya/ktrain',
   keywords = ['tensorflow', 'keras', 'deep learning', 'machine learning'],
   install_requires=[
           'scikit-learn == 0.21.3',
           'matplotlib >= 3.0.0',
-          'pandas < 1.0',
+          'pandas >= 1.0.1',
           'fastprogress >= 0.1.21',
           'keras_bert',
           'requests',
           'joblib',
           'langdetect',
           'jieba',
           'cchardet',
```

