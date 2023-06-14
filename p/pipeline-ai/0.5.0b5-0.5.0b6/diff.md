# Comparing `tmp/pipeline_ai-0.5.0b5.tar.gz` & `tmp/pipeline_ai-0.5.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-0.5.0b5.tar", max compression
+gzip compressed data, was "pipeline_ai-0.5.0b6.tar", max compression
```

## Comparing `pipeline_ai-0.5.0b5.tar` & `pipeline_ai-0.5.0b6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0    10176 2023-06-13 21:08:36.100200 pipeline_ai-0.5.0b5/LICENSE
--rw-r--r--   0        0        0     6130 2023-06-13 21:08:36.100200 pipeline_ai-0.5.0b5/README.md
--rw-r--r--   0        0        0      434 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/__main__.py
--rw-r--r--   0        0        0       62 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/api/__init__.py
--rw-r--r--   0        0        0       62 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/api/asyncio/__init__.py
--rw-r--r--   0        0        0     8379 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/api/asyncio/cloud.py
--rw-r--r--   0        0        0    29923 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/api/cloud.py
--rw-r--r--   0        0        0      974 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/api/environments.py
--rw-r--r--   0        0        0     3231 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0    11667 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/console/__init__.py
--rw-r--r--   0        0        0     8254 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/console/environments.py
--rw-r--r--   0        0        0     2587 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/console/remote.py
--rw-r--r--   0        0        0     2011 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/console/runs.py
--rw-r--r--   0        0        0     4838 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/console/tags.py
--rw-r--r--   0        0        0     4868 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/docker/__init__.py
--rw-r--r--   0        0        0      276 2023-06-13 21:08:36.104200 pipeline_ai-0.5.0b5/pipeline/exceptions/InvalidSchema.py
--rw-r--r--   0        0        0      283 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/exceptions/MissingActiveToken.py
--rw-r--r--   0        0        0      312 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/exceptions/NonChargeableProfile.py
--rw-r--r--   0        0        0      309 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/exceptions/PipelineNotDeployed.py
--rw-r--r--   0        0        0      546 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     4751 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     2015 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/function.py
--rw-r--r--   0        0        0    10909 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/graph.py
--rw-r--r--   0        0        0      877 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/graph_node.py
--rw-r--r--   0        0        0     1090 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0     1160 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/model.py
--rw-r--r--   0        0        0     3473 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1859 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/variable.py
--rw-r--r--   0        0        0     1712 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/base.py
--rw-r--r--   0        0        0      369 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/compute_requirements.py
--rw-r--r--   0        0        0      558 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/data.py
--rw-r--r--   0        0        0      573 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/deployment.py
--rw-r--r--   0        0        0      516 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/environment.py
--rw-r--r--   0        0        0      714 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/file.py
--rw-r--r--   0        0        0     2426 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/function.py
--rw-r--r--   0        0        0     5236 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/metrics.py
--rw-r--r--   0        0        0      569 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/milestones_register.py
--rw-r--r--   0        0        0     1599 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/model.py
--rw-r--r--   0        0        0      739 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/onboarding.py
--rw-r--r--   0        0        0      943 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/pagination.py
--rw-r--r--   0        0        0     5817 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/pipeline.py
--rw-r--r--   0        0        0     1261 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/pipeline_file.py
--rw-r--r--   0        0        0      537 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/project.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/redis/__init__.py
--rw-r--r--   0        0        0      234 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/redis/command.py
--rw-r--r--   0        0        0      337 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/request.py
--rw-r--r--   0        0        0      261 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/resource.py
--rw-r--r--   0        0        0     3839 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/run.py
--rw-r--r--   0        0        0     1031 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/runnable.py
--rw-r--r--   0        0        0      167 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/tag.py
--rw-r--r--   0        0        0     1668 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/token.py
--rw-r--r--   0        0        0     3827 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/user.py
--rw-r--r--   0        0        0     2493 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/validators.py
--rw-r--r--   0        0        0      320 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/schemas/worker.py
--rw-r--r--   0        0        0     1924 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1127 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/util/logging.py
--rw-r--r--   0        0        0      241 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/__init__.py
--rw-r--r--   0        0        0      286 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/environments.py
--rw-r--r--   0        0        0     2883 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/http.py
--rw-r--r--   0        0        0     4931 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/pipelines.py
--rw-r--r--   0        0        0        0 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/schemas/__init__.py
--rw-r--r--   0        0        0     3779 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/schemas/runs.py
--rw-r--r--   0        0        0     4571 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pipeline/v3/uploading.py
--rw-r--r--   0        0        0     1250 2023-06-13 21:08:36.108200 pipeline_ai-0.5.0b5/pyproject.toml
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b5/PKG-INFO
+-rw-r--r--   0        0        0    10176 2023-06-14 16:35:39.993885 pipeline_ai-0.5.0b6/LICENSE
+-rw-r--r--   0        0        0     6130 2023-06-14 16:35:39.993885 pipeline_ai-0.5.0b6/README.md
+-rw-r--r--   0        0        0      434 2023-06-14 16:35:39.993885 pipeline_ai-0.5.0b6/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2023-06-14 16:35:39.993885 pipeline_ai-0.5.0b6/pipeline/__main__.py
+-rw-r--r--   0        0        0       62 2023-06-14 16:35:39.993885 pipeline_ai-0.5.0b6/pipeline/api/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-14 16:35:39.993885 pipeline_ai-0.5.0b6/pipeline/api/asyncio/__init__.py
+-rw-r--r--   0        0        0     8379 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/api/asyncio/cloud.py
+-rw-r--r--   0        0        0    29923 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/api/cloud.py
+-rw-r--r--   0        0        0      974 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/api/environments.py
+-rw-r--r--   0        0        0     3231 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0    11667 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     8254 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/console/environments.py
+-rw-r--r--   0        0        0     2587 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/console/remote.py
+-rw-r--r--   0        0        0     2011 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/console/runs.py
+-rw-r--r--   0        0        0     4838 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/console/tags.py
+-rw-r--r--   0        0        0     4868 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/docker/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/exceptions/InvalidSchema.py
+-rw-r--r--   0        0        0      283 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/exceptions/MissingActiveToken.py
+-rw-r--r--   0        0        0      312 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/exceptions/NonChargeableProfile.py
+-rw-r--r--   0        0        0      309 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/exceptions/PipelineNotDeployed.py
+-rw-r--r--   0        0        0      546 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     4751 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     2015 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/function.py
+-rw-r--r--   0        0        0    10909 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/graph.py
+-rw-r--r--   0        0        0      877 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/graph_node.py
+-rw-r--r--   0        0        0     1090 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0     1160 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/model.py
+-rw-r--r--   0        0        0     3473 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1913 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/variable.py
+-rw-r--r--   0        0        0     1712 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/base.py
+-rw-r--r--   0        0        0      369 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/compute_requirements.py
+-rw-r--r--   0        0        0      558 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/data.py
+-rw-r--r--   0        0        0      573 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/deployment.py
+-rw-r--r--   0        0        0      516 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/environment.py
+-rw-r--r--   0        0        0      714 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/file.py
+-rw-r--r--   0        0        0     2426 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/function.py
+-rw-r--r--   0        0        0     5236 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/metrics.py
+-rw-r--r--   0        0        0      569 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/milestones_register.py
+-rw-r--r--   0        0        0     1599 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/model.py
+-rw-r--r--   0        0        0      739 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/onboarding.py
+-rw-r--r--   0        0        0      943 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/pagination.py
+-rw-r--r--   0        0        0     5817 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/pipeline.py
+-rw-r--r--   0        0        0     1261 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/pipeline_file.py
+-rw-r--r--   0        0        0      537 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/project.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/redis/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/redis/command.py
+-rw-r--r--   0        0        0      337 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/request.py
+-rw-r--r--   0        0        0      261 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/resource.py
+-rw-r--r--   0        0        0     3839 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/run.py
+-rw-r--r--   0        0        0     1031 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/runnable.py
+-rw-r--r--   0        0        0      167 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/tag.py
+-rw-r--r--   0        0        0     1668 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/token.py
+-rw-r--r--   0        0        0     3827 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/user.py
+-rw-r--r--   0        0        0     2493 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/validators.py
+-rw-r--r--   0        0        0      320 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/schemas/worker.py
+-rw-r--r--   0        0        0     1924 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/util/logging.py
+-rw-r--r--   0        0        0      241 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/__init__.py
+-rw-r--r--   0        0        0      286 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/environments.py
+-rw-r--r--   0        0        0     3107 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/http.py
+-rw-r--r--   0        0        0     5312 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/pipelines.py
+-rw-r--r--   0        0        0        0 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/schemas/__init__.py
+-rw-r--r--   0        0        0     3779 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/schemas/runs.py
+-rw-r--r--   0        0        0     4571 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pipeline/v3/uploading.py
+-rw-r--r--   0        0        0     1250 2023-06-14 16:35:39.997886 pipeline_ai-0.5.0b6/pyproject.toml
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b6/PKG-INFO
```

### Comparing `pipeline_ai-0.5.0b5/LICENSE` & `pipeline_ai-0.5.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/README.md` & `pipeline_ai-0.5.0b6/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/api/asyncio/cloud.py` & `pipeline_ai-0.5.0b6/pipeline/api/asyncio/cloud.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/api/cloud.py` & `pipeline_ai-0.5.0b6/pipeline/api/cloud.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/api/environments.py` & `pipeline_ai-0.5.0b6/pipeline/api/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/configuration/__init__.py` & `pipeline_ai-0.5.0b6/pipeline/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/console/__init__.py` & `pipeline_ai-0.5.0b6/pipeline/console/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/console/environments.py` & `pipeline_ai-0.5.0b6/pipeline/console/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/console/remote.py` & `pipeline_ai-0.5.0b6/pipeline/console/remote.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/console/runs.py` & `pipeline_ai-0.5.0b6/pipeline/console/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/console/tags.py` & `pipeline_ai-0.5.0b6/pipeline/console/tags.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/docker/__init__.py` & `pipeline_ai-0.5.0b6/pipeline/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/__init__.py` & `pipeline_ai-0.5.0b6/pipeline/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/decorators.py` & `pipeline_ai-0.5.0b6/pipeline/objects/decorators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/environment/__init__.py` & `pipeline_ai-0.5.0b6/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/function.py` & `pipeline_ai-0.5.0b6/pipeline/objects/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/graph.py` & `pipeline_ai-0.5.0b6/pipeline/objects/graph.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/graph_node.py` & `pipeline_ai-0.5.0b6/pipeline/objects/graph_node.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-0.5.0b6/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/model.py` & `pipeline_ai-0.5.0b6/pipeline/objects/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/pipeline.py` & `pipeline_ai-0.5.0b6/pipeline/objects/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/variable.py` & `pipeline_ai-0.5.0b6/pipeline/objects/variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Iterable
 
 from pipeline.schemas.pipeline import PipelineVariableGet
 from pipeline.util import generate_id, load_object
 
 
 class Variable:
     local_id: str
@@ -71,7 +71,11 @@
     @classmethod
     def from_schema(cls, schema: PipelineVariableGet):
         return cls(
             path=schema.pipeline_file_variable.path,
             name=schema.name,
             local_id=schema.local_id,
         )
+
+
+class Stream(Variable, Iterable):
+    ...
```

### Comparing `pipeline_ai-0.5.0b5/pipeline/objects/wrappers.py` & `pipeline_ai-0.5.0b6/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/base.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/base.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/data.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/data.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/deployment.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/environment.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/environment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/file.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/function.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/metrics.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/milestones_register.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/milestones_register.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/model.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/onboarding.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/onboarding.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/pagination.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/pipeline.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/pipeline_file.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/pipeline_file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/project.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/project.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/run.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/run.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/runnable.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/runnable.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/token.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/token.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/user.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/user.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/schemas/validators.py` & `pipeline_ai-0.5.0b6/pipeline/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/util/__init__.py` & `pipeline_ai-0.5.0b6/pipeline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/util/logging.py` & `pipeline_ai-0.5.0b6/pipeline/util/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/v3/http.py` & `pipeline_ai-0.5.0b6/pipeline/v3/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,7 +121,19 @@
         response = _client.post(
             endpoint,
             files=files,
             params=params,
         )
 
     return response
+
+
+def stream_post(
+    endpoint: str,
+    json_data: dict = None,
+) -> t.Iterable[httpx.Response]:
+    with _client.stream(
+        "POST",
+        endpoint,
+        json=json_data,
+    ) as response:
+        yield response
```

### Comparing `pipeline_ai-0.5.0b5/pipeline/v3/pipelines.py` & `pipeline_ai-0.5.0b6/pipeline/v3/pipelines.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import cloudpickle as cp
 import httpx
 
 from pipeline.objects import Graph, PipelineFile
 from pipeline.util.logging import _print
 from pipeline.v3 import http
-from pipeline.v3.schemas.runs import Run, RunCreate, RunInput, RunIOType
+from pipeline.v3.schemas.runs import Run, RunCreate, RunInput, RunIOType, RunOutput
 
 
 def upload_pipeline(
     graph: Graph,
     environment_id_or_name: t.Union[str, int],
 ):
     if graph._has_run_startup:
@@ -166,7 +166,23 @@
         inputs = [[graph_id, item] for item in array[start_index:end_index]]
 
         with Pool(pool_size) as p:
             batch_res = p.starmap(run_pipeline, inputs)
             results.extend(batch_res)
 
     return results
+
+
+def stream_pipeline(
+    pipeline_id_or_tag: t.Union[str, int],
+    *data,
+) -> t.Iterable[RunOutput]:
+    run_create_schema = RunCreate(
+        pipeline_id_or_tag=pipeline_id_or_tag,
+        input_data=_data_to_run_input(data),
+        async_run=False,
+    )
+
+    return http.stream_post(
+        "/v3/runs/stream",
+        json_data=run_create_schema.dict(),
+    )
```

### Comparing `pipeline_ai-0.5.0b5/pipeline/v3/schemas/runs.py` & `pipeline_ai-0.5.0b6/pipeline/v3/schemas/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pipeline/v3/uploading.py` & `pipeline_ai-0.5.0b6/pipeline/v3/uploading.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b5/pyproject.toml` & `pipeline_ai-0.5.0b6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "0.5.0b5"
+version = "0.5.0b6"
 
 
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
   "Alex Pearwin <alex@mystic.ai>",
   "Neil Wang <neil@mystic.ai>",
```

### Comparing `pipeline_ai-0.5.0b5/PKG-INFO` & `pipeline_ai-0.5.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 0.5.0b5
+Version: 0.5.0b6
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

