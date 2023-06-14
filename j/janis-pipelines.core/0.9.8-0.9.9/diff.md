# Comparing `tmp/janis-pipelines.core-0.9.8.tar.gz` & `tmp/janis-pipelines.core-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/janis-pipelines.core-0.9.8.tar", last modified: Wed Mar 18 01:58:27 2020, max compression
+gzip compressed data, was "dist/janis-pipelines.core-0.9.9.tar", last modified: Fri Mar 20 04:45:36 2020, max compression
```

## Comparing `janis-pipelines.core-0.9.8.tar` & `janis-pipelines.core-0.9.9.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2048 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/translationdeps/
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translationdeps/supportedtranslations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translationdeps/exportpath.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translationdeps/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/code/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4021 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/code/codetool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/code/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6013 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/code/pythontool.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/types/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9250 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/types/data_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      108 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/types/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18281 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/types/common_data_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6182 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/types/selectors.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/hints/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/hints/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/workflow/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26013 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/workflow/workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/workflow/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/translations/
--rw-rw-r--   0 travis    (2000) travis    (2000)    65025 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translations/wdl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32869 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translations/cwl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14640 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translations/translationbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3510 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/translations/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/registry/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2080 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/registry/entrypoints.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3046 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/registry/registry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6850 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/registry/shed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/registry/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/graph/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7584 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/graph/steptaginput.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/graph/node.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/graph/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/__meta__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5131 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/janisconstants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/validators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3749 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/docparser_info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      572 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/yaml_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      229 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/bracketmatching.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2703 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/metadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/levenshteindistance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      750 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1881 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1387 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/scatter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3145 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/utils/generics_util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_core/tool/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5800 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/tool/tool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/tool/documentation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21591 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/tool/commandtool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5545 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/tool/cwl_tool_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/tool/batchrun.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/tool/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2101 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/janis_core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2048 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      103 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-03-18 01:58:27.000000 janis-pipelines.core-0.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2673 2020-03-18 01:58:03.000000 janis-pipelines.core-0.9.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2048 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/translationdeps/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translationdeps/supportedtranslations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1578 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translationdeps/exportpath.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translationdeps/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/code/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4021 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/code/codetool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/code/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6013 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/code/pythontool.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9250 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/types/data_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      108 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/types/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18281 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/types/common_data_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6182 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/types/selectors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/hints/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1272 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/hints/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/workflow/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26013 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/workflow/workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/workflow/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/translations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63941 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translations/wdl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32869 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translations/cwl.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14640 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translations/translationbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3510 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/translations/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/graph/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7584 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/graph/steptaginput.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/graph/node.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/graph/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/__meta__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5131 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/logger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/janisconstants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1237 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/validators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3749 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/docparser_info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      572 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/yaml_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      229 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/resources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/secondary.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1661 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/bracketmatching.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2703 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/metadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/levenshteindistance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      750 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/generators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1881 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1064 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1387 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/scatter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3145 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/utils/generics_util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/tool/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5800 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/tool/tool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/tool/documentation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21591 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/tool/commandtool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5545 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/tool/cwl_tool_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/tool/batchrun.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/tool/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2181 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_core/toolbox/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2080 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/toolbox/entrypoints.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6848 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/toolbox/toolbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3046 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/toolbox/register.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/janis_core/toolbox/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2048 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1786 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      103 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-03-20 04:45:36.000000 janis-pipelines.core-0.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2673 2020-03-20 04:45:13.000000 janis-pipelines.core-0.9.9/setup.py
```

### Comparing `janis-pipelines.core-0.9.8/PKG-INFO` & `janis-pipelines.core-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.core
-Version: 0.9.8
+Version: 0.9.9
 Summary: Contains classes and helpers to build a workflow, and provide options to convert to CWL / WDL
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis
 Author: Michael Franklin, Evan Thomas, Mohammad Bhuyan
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description:
```

### Comparing `janis-pipelines.core-0.9.8/janis_core/translationdeps/exportpath.py` & `janis-pipelines.core-0.9.9/janis_core/translationdeps/exportpath.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/code/codetool.py` & `janis-pipelines.core-0.9.9/janis_core/code/codetool.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/code/pythontool.py` & `janis-pipelines.core-0.9.9/janis_core/code/pythontool.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/types/data_types.py` & `janis-pipelines.core-0.9.9/janis_core/types/data_types.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/types/common_data_types.py` & `janis-pipelines.core-0.9.9/janis_core/types/common_data_types.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/types/selectors.py` & `janis-pipelines.core-0.9.9/janis_core/types/selectors.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/hints/__init__.py` & `janis-pipelines.core-0.9.9/janis_core/hints/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/workflow/workflow.py` & `janis-pipelines.core-0.9.9/janis_core/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/translations/wdl.py` & `janis-pipelines.core-0.9.9/janis_core/translations/wdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 - other translate methods
 - selector helpers (InputSelector, WildcardSelector, CpuSelector, MemorySelector)
 - helper methods
 """
 
 import json
 from inspect import isclass
-from typing import List, Dict, Optional, Any, Set, Tuple
+from typing import List, Dict, Any, Set, Tuple
 
 import wdlgen as wdl
-from janis_core.utils.metadata import ToolMetadata, Metadata
 
 from janis_core.code.codetool import CodeTool
 from janis_core.graph.steptaginput import Edge, StepTagInput
 from janis_core.tool.commandtool import CommandTool, ToolInput, ToolArgument, ToolOutput
-from janis_core.tool.tool import Tool, TOutput, TInput
+from janis_core.tool.tool import Tool, TOutput
 from janis_core.translations.translationbase import TranslatorBase
 from janis_core.types import (
     InputSelector,
     WildcardSelector,
     CpuSelector,
     StringFormatter,
     String,
@@ -45,14 +44,18 @@
     File,
 )
 from janis_core.utils import first_value, recursive_2param_wrap, find_duplicates
 from janis_core.utils.generators import generate_new_id_from
 from janis_core.utils.logger import Logger
 from janis_core.utils.scatter import ScatterDescription, ScatterMethods
 from janis_core.utils.validators import Validators
+from janis_core.utils.secondary import (
+    split_secondary_file_carats,
+    apply_secondary_file_format_to_filename,
+)
 
 # from janis_core.workflow.step import StepNode
 
 
 ## PRIMARY TRANSLATION METHODS
 
 SED_REMOVE_EXTENSION = "| sed 's/\\.[^.]*$//'"
@@ -1546,51 +1549,14 @@
 
 
 def get_secondary_tag_from_original_tag(original, secondary):
     secondary_without_punctuation = secondary.replace(".", "").replace("^", "")
     return original + "_" + secondary_without_punctuation
 
 
-def split_secondary_file_carats(secondary_annotation: str):
-    fixed_sec = secondary_annotation.lstrip("^")
-    leading = len(secondary_annotation) - len(fixed_sec)
-    return secondary_annotation[leading:], leading
-
-
-def apply_secondary_file_format_to_filename(
-    filepath: Optional[str], secondary_file: str
-):
-    """
-    This is actually clever, you can probably trust this to do what you want.
-    :param filepath: Filename to base
-    :param secondary_file: CWL secondary format (Remove 1 extension for each leading ^.
-    """
-    if not filepath:
-        return None
-
-    fixed_sec = secondary_file.lstrip("^")
-    leading = len(secondary_file) - len(fixed_sec)
-    if leading <= 0:
-        return filepath + fixed_sec
-
-    basepath = ""
-    filename = filepath
-    if "/" in filename:
-        idx = len(filepath) - filepath[::-1].index("/")
-        basepath = filepath[:idx]
-        filename = filepath[idx:]
-
-    split = filename.split(".")
-
-    newfname = filename + fixed_sec
-    if len(split) > 1:
-        newfname = ".".join(split[: -min(leading, len(split) - 1)]) + fixed_sec
-    return basepath + newfname
-
-
 def prepare_env_var_setters(
     reqs: Dict[str, Any], inputsdict, **debugkwargs
 ) -> List[wdl.Task.Command]:
     if not reqs:
         return []
 
     statements = []
```

### Comparing `janis-pipelines.core-0.9.8/janis_core/translations/cwl.py` & `janis-pipelines.core-0.9.9/janis_core/translations/cwl.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/translations/translationbase.py` & `janis-pipelines.core-0.9.9/janis_core/translations/translationbase.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/translations/__init__.py` & `janis-pipelines.core-0.9.9/janis_core/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/registry/entrypoints.py` & `janis-pipelines.core-0.9.9/janis_core/toolbox/entrypoints.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/registry/registry.py` & `janis-pipelines.core-0.9.9/janis_core/toolbox/register.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/registry/shed.py` & `janis-pipelines.core-0.9.9/janis_core/toolbox/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from inspect import isfunction, ismodule, isabstract, isclass
 
 from janis_core.tool.commandtool import Tool, ToolTypes, CommandTool, CommandToolBuilder
 from janis_core.code.pythontool import CodeTool, PythonTool
 from janis_core.workflow.workflow import Workflow, WorkflowBuilder
 from janis_core.types.data_types import DataType
 from janis_core.utils.logger import Logger, LogLevel
-import janis_core.registry.entrypoints as EP
-from janis_core.registry.registry import TaggedRegistry, Registry
+import janis_core.toolbox.entrypoints as EP
+from janis_core.toolbox.register import TaggedRegistry, Registry
 
 
 class JanisShed:
 
     MAX_RECURSION_DEPTH = 4
 
     _byclassname = Registry()
```

### Comparing `janis-pipelines.core-0.9.8/janis_core/graph/steptaginput.py` & `janis-pipelines.core-0.9.9/janis_core/graph/steptaginput.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/graph/node.py` & `janis-pipelines.core-0.9.9/janis_core/graph/node.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/logger.py` & `janis-pipelines.core-0.9.9/janis_core/utils/logger.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/validators.py` & `janis-pipelines.core-0.9.9/janis_core/utils/validators.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/docparser_info.py` & `janis-pipelines.core-0.9.9/janis_core/utils/docparser_info.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/yaml_utils.py` & `janis-pipelines.core-0.9.9/janis_core/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/bracketmatching.py` & `janis-pipelines.core-0.9.9/janis_core/utils/bracketmatching.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/metadata.py` & `janis-pipelines.core-0.9.9/janis_core/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/generators.py` & `janis-pipelines.core-0.9.9/janis_core/utils/generators.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/__init__.py` & `janis-pipelines.core-0.9.9/janis_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/errors.py` & `janis-pipelines.core-0.9.9/janis_core/utils/errors.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/scatter.py` & `janis-pipelines.core-0.9.9/janis_core/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/utils/generics_util.py` & `janis-pipelines.core-0.9.9/janis_core/utils/generics_util.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/tool/tool.py` & `janis-pipelines.core-0.9.9/janis_core/tool/tool.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/tool/documentation.py` & `janis-pipelines.core-0.9.9/janis_core/tool/documentation.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/tool/commandtool.py` & `janis-pipelines.core-0.9.9/janis_core/tool/commandtool.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/tool/cwl_tool_parser.py` & `janis-pipelines.core-0.9.9/janis_core/tool/cwl_tool_parser.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/tool/batchrun.py` & `janis-pipelines.core-0.9.9/janis_core/tool/batchrun.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_core/__init__.py` & `janis-pipelines.core-0.9.9/janis_core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 _Proudly made on Planet Earth._
 
 """
 
 # PEP396:  https://www.python.org/dev/peps/pep-0396/
 from janis_core.__meta__ import __version__
-from janis_core.registry.shed import JanisShed
-import janis_core.registry.entrypoints as entrypoints
+from janis_core.toolbox.toolbox import JanisShed
+import janis_core.toolbox.entrypoints as entrypoints
 
 # Tools
 from janis_core.tool.tool import Tool, ToolTypes, TOutput, TInput
 from janis_core.workflow.workflow import Workflow, WorkflowBuilder
 from janis_core.tool.commandtool import (
     CommandTool,
     CommandToolBuilder,
@@ -67,7 +67,8 @@
 from janis_core.tool.documentation import *
 from janis_core.utils.logger import Logger, LogLevel
 from janis_core.translations import SupportedTranslations
 from janis_core.utils.scatter import ScatterDescription, ScatterMethods
 from janis_core.hints import CaptureType, Engine, HINTS, Hint, HintEnum, HintArray
 from janis_core.utils import get_value_for_hints_and_ordered_resource_tuple
 from janis_core.utils.metadata import Metadata, WorkflowMetadata, ToolMetadata
+from janis_core.utils.secondary import apply_secondary_file_format_to_filename
```

### Comparing `janis-pipelines.core-0.9.8/README.md` & `janis-pipelines.core-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/PKG-INFO` & `janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.core
-Version: 0.9.8
+Version: 0.9.9
 Summary: Contains classes and helpers to build a workflow, and provide options to convert to CWL / WDL
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis
 Author: Michael Franklin, Evan Thomas, Mohammad Bhuyan
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description:
```

### Comparing `janis-pipelines.core-0.9.8/janis_pipelines.core.egg-info/SOURCES.txt` & `janis-pipelines.core-0.9.9/janis_pipelines.core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 janis_core/code/__init__.py
 janis_core/code/codetool.py
 janis_core/code/pythontool.py
 janis_core/graph/__init__.py
 janis_core/graph/node.py
 janis_core/graph/steptaginput.py
 janis_core/hints/__init__.py
-janis_core/registry/__init__.py
-janis_core/registry/entrypoints.py
-janis_core/registry/registry.py
-janis_core/registry/shed.py
 janis_core/tool/__init__.py
 janis_core/tool/batchrun.py
 janis_core/tool/commandtool.py
 janis_core/tool/cwl_tool_parser.py
 janis_core/tool/documentation.py
 janis_core/tool/tool.py
+janis_core/toolbox/__init__.py
+janis_core/toolbox/entrypoints.py
+janis_core/toolbox/register.py
+janis_core/toolbox/toolbox.py
 janis_core/translationdeps/__init__.py
 janis_core/translationdeps/exportpath.py
 janis_core/translationdeps/supportedtranslations.py
 janis_core/translations/__init__.py
 janis_core/translations/cwl.py
 janis_core/translations/translationbase.py
 janis_core/translations/wdl.py
@@ -39,14 +39,15 @@
 janis_core/utils/generics_util.py
 janis_core/utils/janisconstants.py
 janis_core/utils/levenshteindistance.py
 janis_core/utils/logger.py
 janis_core/utils/metadata.py
 janis_core/utils/resources.py
 janis_core/utils/scatter.py
+janis_core/utils/secondary.py
 janis_core/utils/validators.py
 janis_core/utils/yaml_utils.py
 janis_core/workflow/__init__.py
 janis_core/workflow/workflow.py
 janis_pipelines.core.egg-info/PKG-INFO
 janis_pipelines.core.egg-info/SOURCES.txt
 janis_pipelines.core.egg-info/dependency_links.txt
```

### Comparing `janis-pipelines.core-0.9.8/setup.py` & `janis-pipelines.core-0.9.9/setup.py`

 * *Files identical despite different names*

