# Comparing `tmp/janis-pipelines.runner-0.9.8.tar.gz` & `tmp/janis-pipelines.runner-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/janis-pipelines.runner-0.9.8.tar", last modified: Wed Feb 26 01:44:43 2020, max compression
+gzip compressed data, was "dist/janis-pipelines.runner-0.9.9.tar", last modified: Mon Mar 16 07:00:48 2020, max compression
```

## Comparing `janis-pipelines.runner-0.9.8.tar` & `janis-pipelines.runner-0.9.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11522 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11522 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      170 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      107 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     9120 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/containers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/containers/docker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5086 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/containers/singularity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/containers/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/containers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4236 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/examples/scratch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/examples/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1596 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/local.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4819 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4597 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/slurm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4015 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/templates/pbs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1285 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/keyvaluedbproviderbase.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/enums/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1440 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/enums/taskstatus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/enums/taskinfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      859 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/enums/workflowmetadatakeys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/enums/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/enums/taskprogress.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/models/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4883 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/models/workflowjob.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8936 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/models/filescheme.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2975 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/models/workflow.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/models/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3429 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/models/outputs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/dbproviderbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/jobeventdbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      782 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/versionsdbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2273 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/janisdbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/outputdbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2400 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/progressdbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6392 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/jobdbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2312 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/workflowmetadataprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1506 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/rundbprovider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/data/providers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/toil/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/toil/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/toil/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/engine.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      273 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/enginetypes.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/
--rw-rw-r--   0 travis    (2000) travis    (2000)    27709 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/cromwellconfiguration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10466 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/cromwellmetadata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/data_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21208 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      847 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cwltool/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7862 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cwltool/cwltoolconfiguation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14051 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cwltool/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/engines/cwltool/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21915 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/cli.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/environments/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/environments/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2234 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/environments/environment.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/validation/
--rw-rw-r--   0 travis    (2000) travis    (2000)      919 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/validation/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/__meta__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3159 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/inputshelper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/fileutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3749 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/docparser_info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/batchrun.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8766 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/getuser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6119 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/pathhelper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1007 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/dateutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2793 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/processlogger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5204 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15754 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      534 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/envvariables.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15392 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2026 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/notificationmanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8174 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/configmanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6954 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/workflowdbmanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      369 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39761 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/workflowmanager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3779 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/management/mysql.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/modifiers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2612 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/modifiers/inputqualifier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3310 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/modifiers/validatormodifier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1011 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/modifiers/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/modifiers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5771 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/modifiers/batchmodifier.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/janis_assistant/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1588 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/tests/test_fileschemes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2772 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/tests/test_templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      494 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/tests/test_configuration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/janis_assistant/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-02-26 01:44:43.000000 janis-pipelines.runner-0.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-02-26 01:44:00.000000 janis-pipelines.runner-0.9.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11522 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11522 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3616 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      170 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      107 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9120 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/containers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/containers/docker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5086 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/containers/singularity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/containers/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/containers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4236 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/examples/scratch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/examples/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1596 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4820 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/local.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4840 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4330 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/slurm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3136 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4204 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/templates/pbs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1285 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/keyvaluedbproviderbase.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/enums/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1440 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/enums/taskstatus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      456 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/enums/taskinfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      859 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/enums/workflowmetadatakeys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/enums/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/enums/taskprogress.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/models/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4883 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/models/workflowjob.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8936 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/models/filescheme.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2975 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/models/workflow.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/models/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3429 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/models/outputs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/dbproviderbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2393 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/jobeventdbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      782 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/versionsdbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2273 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/janisdbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3150 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/outputdbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2400 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/progressdbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6392 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/jobdbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2312 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/workflowmetadataprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1506 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/rundbprovider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/data/providers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/toil/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/toil/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/toil/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2003 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/engine.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      273 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/enginetypes.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28111 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/cromwellconfiguration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10466 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/cromwellmetadata.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      806 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/data_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20956 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      121 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      847 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cwltool/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7862 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cwltool/cwltoolconfiguation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14313 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cwltool/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/engines/cwltool/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23304 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/cli.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/environments/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/environments/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2234 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/environments/environment.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/validation/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      919 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/validation/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      223 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/__meta__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3159 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/inputshelper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      684 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/fileutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3749 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/docparser_info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/batchrun.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8766 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/getuser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6119 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/pathhelper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1007 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/dateutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2793 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/processlogger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5204 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16119 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      534 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1924 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/envvariables.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15845 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/configuration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2026 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/notificationmanager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8174 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/configmanager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6954 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/workflowdbmanager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      369 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39761 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/workflowmanager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3779 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/management/mysql.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/modifiers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2612 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/modifiers/inputqualifier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3310 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/modifiers/validatormodifier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1011 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/modifiers/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/modifiers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6592 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/modifiers/batchmodifier.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/janis_assistant/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1588 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/tests/test_fileschemes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2772 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/tests/test_templates.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      494 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/tests/test_configuration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7951 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/janis_assistant/tests/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-03-16 07:00:48.000000 janis-pipelines.runner-0.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-03-16 07:00:07.000000 janis-pipelines.runner-0.9.9/setup.py
```

### Comparing `janis-pipelines.runner-0.9.8/PKG-INFO` & `janis-pipelines.runner-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.runner
-Version: 0.9.8
+Version: 0.9.9
 Summary: Easier way to run workflows, configurable across environments
 Home-page: UNKNOWN
 Author: Michael Franklin
 Author-email: michael.franklin@petermac.org
 License: MIT
 Description: # Welcome to Janis-Assistant
```

### Comparing `janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/PKG-INFO` & `janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.runner
-Version: 0.9.8
+Version: 0.9.9
 Summary: Easier way to run workflows, configurable across environments
 Home-page: UNKNOWN
 Author: Michael Franklin
 Author-email: michael.franklin@petermac.org
 License: MIT
 Description: # Welcome to Janis-Assistant
```

### Comparing `janis-pipelines.runner-0.9.8/janis_pipelines.runner.egg-info/SOURCES.txt` & `janis-pipelines.runner-0.9.9/janis_pipelines.runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/README.md` & `janis-pipelines.runner-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/containers/docker.py` & `janis-pipelines.runner-0.9.9/janis_assistant/containers/docker.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/containers/singularity.py` & `janis-pipelines.runner-0.9.9/janis_assistant/containers/singularity.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/containers/base.py` & `janis-pipelines.runner-0.9.9/janis_assistant/containers/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/examples/scratch.py` & `janis-pipelines.runner-0.9.9/janis_assistant/examples/scratch.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/templates/templates.py` & `janis-pipelines.runner-0.9.9/janis_assistant/templates/templates.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/templates/base.py` & `janis-pipelines.runner-0.9.9/janis_assistant/templates/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.max_cores = max_cores
         self.max_ram = max_ram
 
         self.can_run_in_foreground = can_run_in_foreground
         self.run_in_background = run_in_background
 
     @abstractmethod
-    def engine_config(self, engine: EngineType):
+    def engine_config(self, engine: EngineType, janis_configuration):
         pass
 
     def submit_detatched_resume(
         self,
         wid: str,
         command: List[str],
         scriptdir: str,
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/templates/slurm.py` & `janis-pipelines.runner-0.9.9/janis_assistant/templates/pbs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,48 @@
-from typing import Union, List
+from typing import List, Union
 
 from janis_assistant.engines.cromwell.cromwellconfiguration import CromwellConfiguration
 from janis_assistant.engines.enginetypes import EngineType
 from janis_assistant.templates.base import SingularityEnvironmentTemplate
 
 
-class SlurmSingularityTemplate(SingularityEnvironmentTemplate):
+class PbsSingularityTemplate(SingularityEnvironmentTemplate):
 
     ignore_init_keys = [
+        "can_run_in_foreground",
+        "run_in_background",
         "build_instructions",
         "singularity_load_instructions",
-        "limit_resources",
         "max_cores",
         "max_ram",
-        "can_run_in_foreground",
-        "run_in_background",
     ]
 
     def __init__(
         self,
         container_dir: str,
         execution_dir: str = None,
         queues: Union[str, List[str]] = None,
         mail_program=None,
         send_job_emails=True,
-        catch_slurm_errors=False,
+        catch_pbs_errors=True,
         build_instructions=f"singularity pull $image docker://${{docker}}",
         singularity_load_instructions=None,
-        limit_resources=False,
         max_cores=None,
         max_ram=None,
         can_run_in_foreground=True,
         run_in_background=False,
     ):
         """
         :param execution_dir: A location where the execution should take place
         :param container_dir: Location where to save and execute containers from
-        :param queues: A single or list of queues that work should be submitted to
+        :param queues: A queue that work should be submitted to
         :param mail_program: Mail program to pipe email to, eg: 'sendmail -t'
-        :param catch_slurm_errors: Catch Slurm errors (like OOM or walltime)
         :param send_job_emails: (requires JanisConfiguration.notifications.email to be set) Send emails for mail types END
         :param build_instructions: Instructions for building singularity, it's recommended to not touch this setting.
         :param singularity_load_instructions: Ensure singularity with this command executed in shell
-        :param limit_resources: Limit resources with singularity using cgroups (REQUIRES ROOT)
         :param max_cores: Maximum number of cores a task can request
         :param max_ram: Maximum amount of ram (GB) that a task can request
         """
 
         super().__init__(
             mail_program=mail_program,
             container_dir=container_dir,
@@ -54,60 +50,55 @@
             load_instructions=singularity_load_instructions,
             max_cores=max_cores,
             max_ram=max_ram,
             can_run_in_foreground=can_run_in_foreground,
             run_in_background=run_in_background,
         )
         self.execution_dir = execution_dir
-        self.queues = queues or []
-        self.send_slurm_emails = send_job_emails
-        self.catch_slurm_errors = catch_slurm_errors
-        self.limitResources = limit_resources
-
-    def cromwell(self):
-        from janis_assistant.management.configuration import JanisConfiguration
-
-        slurm_email = None
-        if self.send_slurm_emails:
-            slurm_email = JanisConfiguration.manager().notifications.email
+        self.queues = queues
+        self.send_job_emails = send_job_emails
+        self.catch_pbs_errors = catch_pbs_errors
+
+    def cromwell(self, janis_configuration):
+
+        job_email = None
+        if self.send_job_emails:
+            job_email = janis_configuration.notifications.email
 
         config = CromwellConfiguration(
             system=CromwellConfiguration.System(
                 job_shell="/bin/sh"  # file_hash_cache=True
             ),
             backend=CromwellConfiguration.Backend(
-                default="slurm-singularity",
+                default="pbs-singularity",
                 providers={
-                    "slurm-singularity": CromwellConfiguration.Backend.Provider.slurm_singularity(
+                    "pbs-singularity": CromwellConfiguration.Backend.Provider.torque_singularity(
                         singularityloadinstructions=self.singularity_load_instructions,
                         singularitycontainerdir=self.singularity_container_dir,
                         buildinstructions=self.singularity_build_instructions,
-                        jobemail=slurm_email,
-                        jobqueues=self.queues,
-                        afternotokaycatch=self.catch_slurm_errors,
-                        limit_resources=self.limitResources,
+                        jobemail=job_email,
+                        queues=self.queues,
+                        afternotokaycatch=self.catch_pbs_errors,
+                        call_caching_method=janis_configuration.cromwell.call_caching_method,
                     )
                 },
             ),
         )
 
         beconfig: CromwellConfiguration.Backend.Provider.Config = config.backend.providers[
             config.backend.default
         ].config
         if self.execution_dir:
             beconfig.root = self.execution_dir
-        beconfig.filesystems = {
-            "local": {
-                "localization": ["hard-link", "cached-copy", "soft-link", "copy"]
-            },
-            # "caching": {"hashing-strategy": "path+modtime"},
-        }
+
+        if janis_configuration.call_caching_enabled:
+            config.call_caching = CromwellConfiguration.CallCaching(enabled=True)
 
         return config
 
-    def engine_config(self, engine: EngineType):
+    def engine_config(self, engine: EngineType, janis_configuration):
         if engine == EngineType.cromwell:
-            return self.cromwell()
+            return self.cromwell(janis_configuration=janis_configuration)
 
         raise NotImplementedError(
             f"The {self.__class__.__name__} template does not have a configuration for {engine.value}"
         )
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/templates/__init__.py` & `janis-pipelines.runner-0.9.9/janis_assistant/templates/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,15 +80,17 @@
 
     provided_params = set(options.keys())
     missing_params = required_params - provided_params
     extra_params = provided_params - recognised_params
 
     if len(missing_params) > 0:
         raise Exception(
-            f"Couldn't construct the template '{template.__name__}', missing the params: {', '.join(missing_params)}"
+            f"There was an error initialising the template '{template.__name__}', as the template "
+            f"is missing the following keys: {', '.join(missing_params)}"
         )
     if len(extra_params) > 0:
         raise Exception(
-            f"Couldn't construct the template '{template.__name__}', unrecognised params: {', '.join(extra_params)}"
+            f"There was an error initialising the template '{template.__name__}', there were unrecognised parameters "
+            f"{', '.join(extra_params)} (the template might have been updated and some of your keys are now invalid)"
         )
 
     return True
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/templates/pbs.py` & `janis-pipelines.runner-0.9.9/janis_assistant/templates/slurm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-from typing import List, Union
+from typing import Union, List
 
 from janis_assistant.engines.cromwell.cromwellconfiguration import CromwellConfiguration
 from janis_assistant.engines.enginetypes import EngineType
 from janis_assistant.templates.base import SingularityEnvironmentTemplate
 
 
-class PbsSingularityTemplate(SingularityEnvironmentTemplate):
+class SlurmSingularityTemplate(SingularityEnvironmentTemplate):
 
     ignore_init_keys = [
-        "can_run_in_foreground",
-        "run_in_background",
         "build_instructions",
         "singularity_load_instructions",
+        "limit_resources",
         "max_cores",
         "max_ram",
+        "can_run_in_foreground",
+        "run_in_background",
     ]
 
     def __init__(
         self,
         container_dir: str,
         execution_dir: str = None,
         queues: Union[str, List[str]] = None,
         mail_program=None,
         send_job_emails=True,
-        catch_pbs_errors=True,
+        catch_slurm_errors=False,
         build_instructions=f"singularity pull $image docker://${{docker}}",
         singularity_load_instructions=None,
         max_cores=None,
         max_ram=None,
         can_run_in_foreground=True,
         run_in_background=False,
     ):
         """
         :param execution_dir: A location where the execution should take place
         :param container_dir: Location where to save and execute containers from
-        :param queues: A queue that work should be submitted to
+        :param queues: A single or list of queues that work should be submitted to
         :param mail_program: Mail program to pipe email to, eg: 'sendmail -t'
+        :param catch_slurm_errors: Catch Slurm errors (like OOM or walltime)
         :param send_job_emails: (requires JanisConfiguration.notifications.email to be set) Send emails for mail types END
         :param build_instructions: Instructions for building singularity, it's recommended to not touch this setting.
         :param singularity_load_instructions: Ensure singularity with this command executed in shell
         :param max_cores: Maximum number of cores a task can request
         :param max_ram: Maximum amount of ram (GB) that a task can request
         """
 
@@ -50,53 +52,55 @@
             load_instructions=singularity_load_instructions,
             max_cores=max_cores,
             max_ram=max_ram,
             can_run_in_foreground=can_run_in_foreground,
             run_in_background=run_in_background,
         )
         self.execution_dir = execution_dir
-        self.queues = queues
+        self.queues = queues or []
         self.send_job_emails = send_job_emails
-        self.catch_pbs_errors = catch_pbs_errors
+        self.catch_slurm_errors = catch_slurm_errors
+
+    def cromwell(self, janis_configuration):
 
-    def cromwell(self):
+        job_email = None
+        if self.send_job_emails:
+            job_email = janis_configuration.notifications.email
 
         config = CromwellConfiguration(
             system=CromwellConfiguration.System(
                 job_shell="/bin/sh"  # file_hash_cache=True
             ),
             backend=CromwellConfiguration.Backend(
-                default="pbs-singularity",
+                default="slurm-singularity",
                 providers={
-                    "pbs-singularity": CromwellConfiguration.Backend.Provider.torque_singularity(
+                    "slurm-singularity": CromwellConfiguration.Backend.Provider.slurm_singularity(
                         singularityloadinstructions=self.singularity_load_instructions,
                         singularitycontainerdir=self.singularity_container_dir,
                         buildinstructions=self.singularity_build_instructions,
-                        send_job_updates=self.send_job_emails,
-                        queues=self.queues,
-                        afternotokaycatch=self.catch_pbs_errors,
+                        jobemail=job_email,
+                        jobqueues=self.queues,
+                        afternotokaycatch=self.catch_slurm_errors,
+                        call_caching_method=janis_configuration.cromwell.call_caching_method,
                     )
                 },
             ),
         )
 
         beconfig: CromwellConfiguration.Backend.Provider.Config = config.backend.providers[
             config.backend.default
         ].config
         if self.execution_dir:
             beconfig.root = self.execution_dir
-        beconfig.filesystems = {
-            "local": {
-                "localization": ["hard-link", "cached-copy", "soft-link", "copy"]
-            },
-            # "caching": {"hashing-strategy": "path+modtime"},
-        }
+
+        if janis_configuration.call_caching_enabled:
+            config.call_caching = CromwellConfiguration.CallCaching(enabled=True)
 
         return config
 
-    def engine_config(self, engine: EngineType):
+    def engine_config(self, engine: EngineType, janis_configuration):
         if engine == EngineType.cromwell:
-            return self.cromwell()
+            return self.cromwell(janis_configuration)
 
         raise NotImplementedError(
             f"The {self.__class__.__name__} template does not have a configuration for {engine.value}"
         )
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/keyvaluedbproviderbase.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/keyvaluedbproviderbase.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/enums/taskstatus.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/enums/taskstatus.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/enums/workflowmetadatakeys.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/enums/workflowmetadatakeys.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/models/workflowjob.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/models/workflowjob.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/models/filescheme.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/models/filescheme.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/models/workflow.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/models/workflow.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/models/outputs.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/models/outputs.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/jobeventdbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/jobeventdbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/versionsdbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/versionsdbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/janisdbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/janisdbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/outputdbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/outputdbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/progressdbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/progressdbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/jobdbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/jobdbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/workflowmetadataprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/workflowmetadataprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/data/providers/rundbprovider.py` & `janis-pipelines.runner-0.9.9/janis_assistant/data/providers/rundbprovider.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/toil/main.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/toil/main.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/engine.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/engine.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/cromwellconfiguration.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/cromwellconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from enum import Enum
 from typing import Tuple, Any, Dict, Union, List
 
 from janis_core.utils.logger import Logger
 
 
 class Serializable:
     parse_types = {}
@@ -85,14 +86,26 @@
             self.instance_name = instance_name
 
         key_map = {
             "binding_timeout": "binding-timeout",
             "instance_name": "instance.name",
         }
 
+    class CromwellFilesystem(Enum):
+        """
+        Filesystems must be one of these: https://cromwell.readthedocs.io/en/stable/filesystems/Filesystems/
+        """
+
+        local = "local"  # Shared file system
+        s3 = "s3"  # Simple Storage Service
+        gcs = "gcs"
+        oss = "oss"
+        http = "http"
+        ftp = "ftp"
+
     class Akka(Serializable):
         pass
 
     class System(Serializable):
         class Io(Serializable):
             def __init__(
                 self, per=None, number_of_attempts=None, number_of_requests=None
@@ -206,17 +219,35 @@
 
                         key_map = {
                             "duplication_strategy": "duplication-strategy",
                             "hashing_strategy": "hashing-strategy",
                             "check_sibling_md5": "check-sibling-md5",
                         }
 
-                    def __init__(self, caching: Caching = None):
+                    def __init__(self, enabled: bool = True, caching: Caching = None):
+                        self.enabled = enabled
                         self.caching = caching
 
+                    @staticmethod
+                    def default_filesystem(cache_method: str = None):
+
+                        return {
+                            "local": CromwellConfiguration.Backend.Provider.Config.Filesystem(
+                                caching=CromwellConfiguration.Backend.Provider.Config.Filesystem.Caching(
+                                    duplication_strategy=[
+                                        "hard-link",
+                                        "cached-copy",
+                                        "copy",
+                                        "soft-link",
+                                    ],
+                                    hashing_strategy=(cache_method or "path+modtime"),
+                                )
+                            )
+                        }
+
                 def __init__(
                     self,
                     submit=None,
                     submit_docker=None,
                     runtime_attributes=None,
                     kill=None,
                     kill_docker=None,
@@ -229,20 +260,16 @@
                     root=None,
                     **kwargs,
                 ):
                     self.root = root
                     self.default_runtime_attributes = default_runtime_attributes
 
                     self.concurrent_job_limit = concurrent_job_limit
+                    self.filesystems = filesystems
 
-                    self.filesystems = filesystems or {
-                        "local": self.Filesystem(
-                            self.Filesystem.Caching(hashing_strategy="File")
-                        )
-                    }
                     self.runtime_attributes = (runtime_attributes or "").replace(
                         "\n", "\\n"
                     )
 
                     self.submit = submit
                     self.submit_docker = submit_docker
                     self.kill = kill
@@ -272,15 +299,16 @@
             ):
                 self.actor_factory = actor_factory
                 self.config = config
 
             key_map = {"actor_factory": "actor-factory"}
 
             @classmethod
-            def slurm(cls):
+            def slurm(cls, call_caching_method: str = None):
+
                 return cls(
                     actor_factory="cromwell.backend.impl.sfs.config.ConfigBackendLifecycleActorFactory",
                     config=cls.Config(
                         runtime_attributes="""\
 Int runtime_minutes = 1440
 Int? cpu = 1
 Int memory_mb = 3500
@@ -296,55 +324,45 @@
         ${"-p " + queue} \\
         ${"-n " + cpu} \\
         --mem=${memory_mb} \\
         --wrap "/usr/bin/env ${job_shell} ${script}" """,
                         kill="scancel ${job_id}",
                         check_alive="scontrol show job ${job_id}",
                         job_id_regex="Submitted batch job (\\d+).*",
+                        filesystems=cls.Config.Filesystem.default_filesystem(
+                            call_caching_method
+                        ),
                     ),
                 )
 
             @classmethod
             def slurm_singularity(
                 cls,
                 singularityloadinstructions,
                 singularitycontainerdir,
                 buildinstructions,
                 jobemail,
                 jobqueues,
                 afternotokaycatch: bool = True,
-                limit_resources: bool = False,
+                call_caching_method: str = None,
             ):
-                slurm = cls.slurm()
+                slurm = cls.slurm(call_caching_method=call_caching_method)
 
                 afternotokaycommand = ""
                 if afternotokaycatch:
                     afternotokaycommand = " && NTOKDEP=$(sbatch --parsable --kill-on-invalid-dep=yes --dependency=afternotokay:$JOBID --wrap 'echo 1 >> ${cwd}/execution/rc')"
 
                 partitions = (
                     ",".join(jobqueues) if isinstance(jobqueues, list) else jobqueues
                 )
                 partition_string = ("-p " + partitions) if partitions else ""
                 emailextra = (
                     f"--mail-user {jobemail} --mail-type END" if jobemail else ""
                 )
 
-                cgroups_creation = (
-                    """# Generate singularity cgroups command
-                cgroupsfile="${cwd}/execution/singularity-cgroup.toml"
-                printf "[memory]\\n  limit = $((${memory_mb} * 1048576))" > $cgroupsfile\
-                """
-                    if limit_resources
-                    else ""
-                )
-
-                cgroups_binding = (
-                    " --apply-cgroups $cgroupsfile" if limit_resources else ""
-                )
-
                 slurm.config.runtime_attributes = """\
 Int runtime_minutes = 1440
 String kvruntime_value = ""
 Int? cpu = 1
 Int memory_mb = 3500
 String? docker
 """
@@ -352,16 +370,14 @@
                 slurm.config.submit_docker = f"""\
             {singularityloadinstructions}
 
             docker_subbed=$(sed -e 's/[^A-Za-z0-9._-]/_/g' <<< ${{docker}})
             image={singularitycontainerdir}/$docker_subbed.sif
             lock_path={singularitycontainerdir}/$docker_subbed.lock
 
-            {cgroups_creation}
-
             if [ ! -f "$image" ]; then
               {buildinstructions}
             fi
 
             # Submit the script to SLURM
             jobname={CromwellConfiguration.JOBNAME_TRANSFORM}
             JOBID=$(sbatch \\
@@ -371,70 +387,60 @@
                 --cpus-per-task ${{if defined(cpu) then cpu else 1}} \\
                 {partition_string} \\
                 -D ${{cwd}} \\
                 -o ${{cwd}}/execution/stdout \\
                 -e ${{cwd}}/execution/stderr \\
                 -t ${{runtime_minutes}} \\
                 {emailextra} \\
-                --wrap "singularity exec --bind ${{cwd}}:${{docker_cwd}}{cgroups_binding} $image ${{job_shell}} ${{docker_script}}") \\
+                --wrap "singularity exec --bind ${{cwd}}:${{docker_cwd}} $image ${{job_shell}} ${{docker_script}}") \\
                 {afternotokaycommand} \\
                 && echo Submitted batch job $JOBID
             """
                 return slurm
 
             @classmethod
             def singularity(
                 cls,
                 singularityloadinstructions,
                 singularitycontainerdir,
                 buildinstructions,
-                limit_resources: bool = False,
-                executionDirectory: str = None,
+                execution_directory: str = None,
+                call_caching_method: str = None,
             ):
 
                 config = cls(
                     actor_factory="cromwell.backend.impl.sfs.config.ConfigBackendLifecycleActorFactory",
                     config=cls.Config(
-                        runtime_attributes="""\
-String? docker""".strip(),
+                        runtime_attributes="""String? docker""".strip(),
                         run_in_background=True,
-                        root=executionDirectory,
+                        root=execution_directory,
+                        filesystems=CromwellConfiguration.Backend.Provider.Config.Filesystem.default_filesystem(
+                            call_caching_method
+                        ),
                     ),
                 )
 
-                cgroups_creation = (
-                    """# Generate singularity cgroups command
-                cgroupsfile="${{cwd}}/execution/singularity-cgroup.toml"
-                printf "[memory]\\n  limit = $((${{memory_mb}} * 1048576))" > $cgroupsfile\
-                """
-                    if limit_resources
-                    else ""
-                )
-                cgroups_binding = (
-                    " --apply-cgroups $cgroupsfile" if limit_resources else ""
-                )
-
                 config.config.submit_docker = f"""
                     {singularityloadinstructions}
 
                     docker_subbed=$(sed -e 's/[^A-Za-z0-9._-]/_/g' <<< ${{docker}})
                     image={singularitycontainerdir}/$docker_subbed.sif
                     lock_path={singularitycontainerdir}/$docker_subbed.lock
 
                     {buildinstructions}
 
-                    {cgroups_creation}
-
-                    singularity exec --bind ${{cwd}}:${{docker_cwd}}{cgroups_binding} $image ${{job_shell}} ${{docker_script}}
+                    singularity exec --bind ${{cwd}}:${{docker_cwd}} $image ${{job_shell}} ${{docker_script}}
                     """
                 return config
 
             # noinspection PyPep8
             @classmethod
-            def torque(cls, queues: Union[str, List[str]]):
+            def torque(
+                cls, queues: Union[str, List[str]], call_caching_method: str = None
+            ):
                 """
                 Source: https://gatkforums.broadinstitute.org/wdl/discussion/12992/failed-to-evaluate-job-outputs-error
                 """
 
                 qparam = ""
                 if queues:
                     qparam = "-q " + (
@@ -453,54 +459,48 @@
     chmod +x ${{script}}
     echo "${{job_shell}} ${{script}}" | qsub -V -d ${{cwd}} -N ${{job_name}} -o ${{out}} -e ${{err}} {qparam} -l nodes=1:ppn=${{cpu}}" \
         -l walltime=${{walltime}} -l mem=${{memory_mb}}
             """,
                         job_id_regex="^(\\d+).*",
                         kill="qdel ${job_id}",
                         check_alive="qstat ${job_id}",
+                        filesystems=CromwellConfiguration.Backend.Provider.Config.Filesystem.default_filesystem(
+                            call_caching_method
+                        ),
                     ),
                 )
 
             @classmethod
             def torque_singularity(
                 cls,
                 queues: Union[str, List[str]],
                 singularityloadinstructions,
                 singularitycontainerdir,
                 buildinstructions,
-                send_job_updates,
+                jobemail: str = None,
                 afternotokaycatch=False,
+                call_caching_method: str = None,
             ):
                 """
                 Source: https://gatkforums.broadinstitute.org/wdl/discussion/12992/failed-to-evaluate-job-outputs-error
                 """
 
-                from janis_assistant.management.configuration import JanisConfiguration
-
-                torq = cls.torque(queues)
+                torq = cls.torque(queues, call_caching_method=call_caching_method)
 
                 afternotokaycommand = ""
                 if afternotokaycatch:
                     afternotokaycommand = " && NTOKDEP=$(echo 'echo 1 >> ${cwd}/execution/rc' | qsub -W depend=afternotok:$JOBID -l nodes=1:ppn=1,mem=1GB,walltime=00:01:00)"
 
                 qparam = ""
                 if queues:
                     qparam = "-q " + (
                         ",".join(queues) if isinstance(queues, list) else queues
                     )
 
-                emailparams = ""
-                email = JanisConfiguration.manager().notifications.email
-                if send_job_updates:
-                    if not email:
-                        Logger.info(
-                            "Skipping send_job_updates for Torque as no email was found in the configuration"
-                        )
-                    else:
-                        emailparams = f"-m ea -M {email}"
+                emailparams = f"-m ea -M {jobemail}" if jobemail else ""
 
                 loadinstructions = (
                     (singularityloadinstructions + " &&")
                     if singularityloadinstructions
                     else ""
                 )
 
@@ -580,15 +580,16 @@
 
         @staticmethod
         def with_new_local_exec_dir(execution_directory: str):
             return CromwellConfiguration.Backend(
                 providers={
                     "Local": CromwellConfiguration.Backend.Provider(
                         config=CromwellConfiguration.Backend.Provider.Config(
-                            root=execution_directory
+                            root=execution_directory,
+                            filesystems=CromwellConfiguration.Backend.Provider.Config.Filesystem.default_filesystem(),
                         )
                     )
                 }
             )
 
     class Engine(Serializable):
         def __init__(self, s3: Union[bool, str] = None, gcs: Union[bool, str] = None):
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/cromwellmetadata.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/cromwellmetadata.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/data_types.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/data_types.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/cromwell/main.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/cromwell/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,29 +552,23 @@
             shutil.copyfile(config_path, self.config_path)
 
         elif jc.cromwell.configpath:
             shutil.copyfile(jc.cromwell.configpath, self.config_path)
 
         else:
             self.config: CromwellConfiguration = jc.template.template.engine_config(
-                EngineType.cromwell
+                EngineType.cromwell, jc
             ) or CromwellConfiguration()
             if not self.config.system:
                 self.config.system = CromwellConfiguration.System()
             self.config.system.cromwell_id = identifier
             self.config.system.cromwell_id_random_suffix = False
             self.config.system.job_shell = "/bin/sh"
 
         if self.config:
-            # if self.config.call_caching:
-            #     self.config.call_caching.enabled = True
-            # else:
-            #     self.config.call_caching = CromwellConfiguration.CallCaching(
-            #         enabled=True
-            #     )
 
             if self.config.backend:
                 if len(self.config.backend.providers) == 1:
                     cnf: CromwellConfiguration.Backend.Provider = first_value(
                         self.config.backend.providers
                     )
                     if not cnf.config.root:
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/__init__.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/cwltool/cwltoolconfiguation.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/cwltool/cwltoolconfiguation.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/engines/cwltool/main.py` & `janis-pipelines.runner-0.9.9/janis_assistant/engines/cwltool/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
         jc = JanisConfiguration.manager()
 
         if config:
             self.config = config
         else:
             self.config = (
-                jc.template.template.engine_config(EngineType.cwltool)
+                jc.template.template.engine_config(EngineType.cwltool, jc)
                 or CWLToolConfiguration()
             )
 
     def test_connection(self):
         return bool(self.process_id)
 
     def start_engine(self):
@@ -355,32 +355,40 @@
             # outputs=meta.get("outputs") or [],
             jobs=list(self.taskmeta.get("jobs", {}).values()),
             error=self.taskmeta.get("error"),
             # executiondir=None,
         )
 
     def start_from_paths(self, wid, source_path: str, input_path: str, deps_path: str):
+
+        from janis_assistant.management.configuration import JanisConfiguration
+
+        jc = JanisConfiguration.manager()
+
         self.taskmeta = {
             "start": DateUtil.now(),
             "status": TaskStatus.PROCESSING,
             "jobs": {},
         }
-        config = self.config
+        config: CWLToolConfiguration = self.config
 
         if Logger.CONSOLE_LEVEL == LogLevel.VERBOSE:
             config.debug = True
 
         config.disable_color = True
 
         # more options
         if not config.tmpdir_prefix:
             config.outdir = self.execution_dir + "/"
             config.tmpdir_prefix = self.execution_dir + "/"
             config.leave_tmpdir = True
 
+        if jc.call_caching_enabled:
+            config.cachedir = os.path.join(self.execution_dir, "cached/")
+
         cmd = config.build_command_line(source_path, input_path)
 
         Logger.debug("Running command: '" + " ".join(cmd) + "'")
 
         process = subprocess.Popen(
             cmd, stdout=subprocess.PIPE, preexec_fn=os.setsid, stderr=subprocess.PIPE
         )
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/cli.py` & `janis-pipelines.runner-0.9.9/janis_assistant/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import argparse
 import json
 
 import ruamel.yaml
 import tabulate
+from janis_core import InputQualityType
 
 from janis_core.translationdeps.supportedtranslations import SupportedTranslations
 
 from janis_assistant.__meta__ import DOCS_URL
 from janis_assistant.templates.templates import get_template_names
 from janis_assistant.engines.enginetypes import EngineType
 from janis_assistant.management.configuration import JanisConfiguration
@@ -240,26 +241,47 @@
         help="Force re-download of workflow if remote",
         action="store_true",
     )
 
 
 def add_inputs_args(parser):
     parser.add_argument("workflow", help="workflow to generate inputs for")
+    parser.add_argument("-c", "--config", help="Path to config file")
+
     parser.add_argument("-o", "--output", help="file to output to, else stdout")
     parser.add_argument(
         "-a",
         "--all",
         action="store_true",
         help="Include inputs that have default values",
     )
-    parser.add_argument("-r", "--recipes", help="Recipes from template", nargs="+")
+
+    parser.add_argument(
+        "--user",
+        action="store_true",
+        help="Only include user inputs (ignore inputs with a qualityType of static or configuration). "
+        "Note, this is only available for pilelines that have inputs that are annotated with input qualities.",
+    )
+    parser.add_argument(
+        "--static",
+        action="store_true",
+        help="Include all inputs with a quality type of static or configuration. "
+        "Note, this is only available for pilelines that have inputs that are annotated with input qualities.",
+    )
+
+    parser.add_argument(
+        "-r",
+        "--recipes",
+        help="If you have values available from these recipes, they will be ignored from the output",
+        nargs="+",
+    )
     parser.add_argument(
         "--resources",
         action="store_true",
-        help="Add resource overrides into inputs file",
+        help="Add resource overrides into inputs file (eg: runtime_cpu / runtime_memory)",
     )
     parser.add_argument(
         "--json", action="store_true", help="Output to JSON instead of yaml"
     )
     parser.add_argument("-i", "--inputs", help="additional inputs to pull values from")
     parser.add_argument(
         "-n",
@@ -294,14 +316,16 @@
     parser.add_argument(
         "-o",
         "--output-dir",
         help="This directory to copy outputs to. By default intermediate results are "
         "within a janis/execution subfolder (unless overriden by a template)",
     )
 
+    parser.add_argument("-F", "--foreground", action="store_true", default=False)
+
     parser.add_argument(
         "-B",
         "--background",
         action="store_true",
         default=False,
         help="Run the workflow engine in the background (or submit to a cluster if your template supports it)",
     )
@@ -645,14 +669,15 @@
 
     mysql = args.mysql
     keep_intermediate_files = args.keep_intermediate_files is True
 
     if args.development:
         mysql = True
         keep_intermediate_files = True
+        JanisConfiguration.manager().cromwell.call_caching_enabled = True
 
     wid = fromjanis(
         args.workflow,
         name=args.name,
         validation_reqs=validation_reqs,
         batchrun_reqs=batchrun_reqs,
         engine=args.engine,
@@ -666,14 +691,15 @@
         watch=args.progress,
         max_cores=args.max_cores,
         max_mem=args.max_memory,
         force=args.no_cache,
         recipes=args.recipe,
         keep_intermediate_files=keep_intermediate_files,
         run_in_background=(args.background is True),
+        run_in_foreground=(args.foreground is True),
         mysql=mysql,
         only_registry=args.registry,
         no_store=args.no_store,
     )
 
     Logger.info("Exiting")
     raise SystemExit
@@ -686,21 +712,34 @@
         force=args.no_cache,
         registry_only=args.registry,
         trace=args.trace,
     )
 
 
 def do_inputs(args):
+
+    if args.config or args.recipes:
+        JanisConfiguration.initial_configuration(args.config)
+
+    quality_type = None
+
+    if args.user:
+        quality_type = [InputQualityType.user]
+    elif args.static:
+        quality_type = [InputQualityType.static, InputQualityType.configuration]
+
     outd = generate_inputs(
         args.workflow,
         all=args.all,
         name=args.name,
         force=args.no_cache,
         additional_inputs=args.inputs,
         with_resources=args.resources,
+        quality_type=quality_type,
+        recipes=args.recipes,
     )
 
     if args.json:
         outs = json.dumps(outd, sort_keys=True, indent=4, separators=(",", ": "))
     else:
         outs = ruamel.yaml.dump(outd, default_flow_style=False)
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/environments/environment.py` & `janis-pipelines.runner-0.9.9/janis_assistant/environments/environment.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/validation/__init__.py` & `janis-pipelines.runner-0.9.9/janis_assistant/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/inputshelper.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/inputshelper.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/fileutil.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/fileutil.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/docparser_info.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/docparser_info.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/getuser.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/getuser.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/pathhelper.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/pathhelper.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/dateutil.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/dateutil.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/processlogger.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/processlogger.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/utils/__init__.py` & `janis-pipelines.runner-0.9.9/janis_assistant/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/main.py` & `janis-pipelines.runner-0.9.9/janis_assistant/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 """
 import sys, os
 from inspect import isclass
 
 import janis_core as j
 from typing import Optional, Dict, Union, Type, List
 
+from janis_core import InputQualityType
+
 from janis_assistant.templates import TemplateInput
 
 from janis_assistant.management.workflowmanager import WorkflowManager
 
 from janis_assistant.data.models.filescheme import (
     FileScheme,
     LocalFileScheme,
@@ -166,28 +168,38 @@
 def generate_inputs(
     tool: Union[str, j.CommandTool, j.Workflow],
     all=False,
     name=None,
     force=False,
     additional_inputs=None,
     with_resources=False,
+    quality_type=List[InputQualityType],
+    recipes=List[str],
 ):
     toolref = resolve_tool(tool, name, from_toolshed=True, force=force)
     inputsdict = None
     if additional_inputs:
         inputsfile = get_file_from_searchname(additional_inputs, ".")
         inputsdict = parse_dict(inputsfile)
 
+    values_to_ignore = set()
+    if recipes:
+        jc = JanisConfiguration.manager()
+        for k in jc.recipes.get_recipe_for_keys(recipes):
+            values_to_ignore.add(k)
+
     if not toolref:
         raise Exception("Couldn't find workflow with name: " + str(tool))
 
     return toolref.generate_inputs_override(
         additional_inputs=inputsdict,
         with_resource_overrides=with_resources,
         include_defaults=all,
+        values_to_ignore=values_to_ignore,
+        quality_type=quality_type,
     )
 
 
 import argparse
 
 
 class InitArgParser(argparse.ArgumentParser):
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/__init__.py` & `janis-pipelines.runner-0.9.9/janis_assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/envvariables.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/envvariables.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/configuration.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         Engine = "engine"
         Environment = "environment"
         Cromwell = "cromwell"
         Template = "template"
         Recipes = "recipes"
         Notifications = "notifications"
         RunInBackground = "run_in_background"
+        CallCachingEnabled = "call_caching_enabled"
 
     _managed = None  # type: JanisConfiguration
 
     _configpath = None
 
     @staticmethod
     def manager():
@@ -114,14 +115,15 @@
 
     class JanisConfigurationCromwell(NoAttributeErrors):
         class Keys(HashableEnum):
             JarPath = "jar"
             ConfigPath = "config_path"
             Url = "url"
             Memory = "memory_mb"
+            CallCachingMethod = "call_caching_method"
 
         def __init__(self, d: dict, default: dict):
             d = d if d else {}
 
             self.jarpath = JanisConfiguration.get_value_for_key(
                 d, self.Keys.JarPath, default
             )
@@ -130,14 +132,18 @@
             )
 
             self.url = JanisConfiguration.get_value_for_key(d, self.Keys.Url, default)
             self.memory = JanisConfiguration.get_value_for_key(
                 d, self.Keys.Memory, default
             )
 
+            self.call_caching_method = JanisConfiguration.get_value_for_key(
+                d, self.Keys.CallCachingMethod, default
+            )
+
     class JanisConfigurationRecipes(NoAttributeErrors):
         class Keys(HashableEnum):
             Recipes = "recipes"
             Paths = "paths"
             Directories = "directories"
 
         def __init__(self, d: dict, default: dict):
@@ -314,14 +320,17 @@
         self.outputdir = self.get_value_for_key(
             d, JanisConfiguration.Keys.OutputDir, default
         )
 
         self.executiondir = self.get_value_for_key(
             d, JanisConfiguration.Keys.ExecutionDir, default
         )
+        self.call_caching_enabled = JanisConfiguration.get_value_for_key(
+            d, self.Keys.CallCachingEnabled, default
+        )
 
         self.engine = self.get_value_for_key(d, JanisConfiguration.Keys.Engine, default)
         self.cromwell = JanisConfiguration.JanisConfigurationCromwell(
             d.get(JanisConfiguration.Keys.Cromwell),
             default.get(JanisConfiguration.Keys.Cromwell),
         )
 
@@ -406,14 +415,15 @@
             JanisConfiguration.Keys.Template: {
                 JanisConfiguration.JanisConfigurationTemplate.Keys.Id: "local"
             },
             JanisConfiguration.Keys.Notifications: {
                 JanisConfiguration.JanisConfigurationNotifications.Keys.Email: None
             },
             JanisConfiguration.Keys.RunInBackground: None,
+            JanisConfiguration.Keys.CallCachingEnabled: None,
         }
         return stringify_dict_keys_or_return_value(deflt)
 
     @staticmethod
     def default():
         """
         The defaults listed are provided to the user on init, they should be
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/notificationmanager.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/notificationmanager.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/configmanager.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/configmanager.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/workflowdbmanager.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/workflowdbmanager.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/workflowmanager.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/workflowmanager.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/management/mysql.py` & `janis-pipelines.runner-0.9.9/janis_assistant/management/mysql.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/modifiers/inputqualifier.py` & `janis-pipelines.runner-0.9.9/janis_assistant/modifiers/inputqualifier.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/modifiers/validatormodifier.py` & `janis-pipelines.runner-0.9.9/janis_assistant/modifiers/validatormodifier.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/modifiers/base.py` & `janis-pipelines.runner-0.9.9/janis_assistant/modifiers/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/modifiers/batchmodifier.py` & `janis-pipelines.runner-0.9.9/janis_assistant/modifiers/batchmodifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Dict, List
 
 from janis_core import Tool, WorkflowBuilder, Workflow, Array
-from janis_core.utils import find_duplicates
+from janis_core.utils import find_duplicates, validators
+from janis_core.utils.validators import Validators
 
 from janis_assistant.modifiers.base import PipelineModifierBase
 from janis_assistant.utils.batchrun import BatchRunRequirements
 
 
 class BatchPipelineModifier(PipelineModifierBase):
 
@@ -47,23 +48,35 @@
             if i.id() in fields:
                 continue
 
             innode_base[i.id()] = w.input(
                 i.id(), i.intype, default=i.default, doc=i.doc
             )
 
-        groupby_values = inputs[self.batch.groupby]
+        raw_groupby_values = inputs[self.batch.groupby]
 
-        duplicate_keys = find_duplicates(groupby_values)
+        duplicate_keys = find_duplicates(raw_groupby_values)
         if len(duplicate_keys) > 0:
             raise Exception(
                 f"There are duplicate group_by ({self.batch.groupby}) keys in the input: "
                 + ", ".join(duplicate_keys)
             )
 
+        groupby_values = [
+            Validators.transform_identifier_to_be_valid(ident)
+            for ident in raw_groupby_values
+        ]
+        duplicate_keys = find_duplicates(groupby_values)
+        if len(duplicate_keys) > 0:
+            raise Exception(
+                f"Janis transformed values in the group_by field ({self.batch.groupby}) to be a valid identifiers, "
+                f"after this transformation, there were duplicates keys: "
+                + ", ".join(duplicate_keys)
+            )
+
         w.input(self.GROUPBY_FIELDNAME, Array(str), value=groupby_values)
 
         steps_created = []
 
         stepid_from_gb = lambda gb: f"{gbvalue}_{tool.id()}"
 
         for gbvalue in groupby_values:
@@ -75,40 +88,45 @@
 
             steps_created.append(
                 w.step(stepid_from_gb(gbvalue), tool(**innode_base, **extra_ins))
             )
 
         for out in tool.tool_outputs():
             output_folders = []
-            output_name = None
+            output_name = out.id()
             if isinstance(tool, Workflow):
                 on = tool.output_nodes[out.id()]
                 output_folders = on.output_folder or []
-                output_name = on.output_name
+                if on.output_name:
+                    output_name = on.output_name
 
-            for gbvalue in groupby_values:
+            for gbvalue, raw_gbvalue in zip(groupby_values, raw_groupby_values):
 
                 w.output(
                     f"{gbvalue}_{out.id()}",
                     source=w[stepid_from_gb(gbvalue)][out.id()],
                     output_name=output_name,
-                    output_folder=[gbvalue],
+                    output_folder=[raw_gbvalue],
                 )
 
         return w
 
     def inputs_modifier(self, wf: Tool, inputs: Dict, hints: Dict[str, str]) -> Dict:
 
         if self.batch.groupby not in inputs:
             raise Exception(
                 "the group_by field '{self.batch.groupby}' was not found in the inputs"
             )
 
         # batch_inputs is seen as the source of truth for the length operations
-        groupby_values = inputs[self.batch.groupby]
+        raw_groupby_values = inputs[self.batch.groupby]
+        groupby_values = [
+            Validators.transform_identifier_to_be_valid(ident)
+            for ident in raw_groupby_values
+        ]
         if not isinstance(groupby_values, list):
             raise ValueError(
                 f"The value of the groupBy field '{self.batch.groupby}' was not a 'list', got '{type(groupby_values)}'"
             )
 
         # Split up the inputs dict to be keyed by the groupBy field
```

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/tests/test_fileschemes.py` & `janis-pipelines.runner-0.9.9/janis_assistant/tests/test_fileschemes.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/tests/test_templates.py` & `janis-pipelines.runner-0.9.9/janis_assistant/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/janis_assistant/tests/test_utils.py` & `janis-pipelines.runner-0.9.9/janis_assistant/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.runner-0.9.8/setup.py` & `janis-pipelines.runner-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     license="MIT",
     keywords=["janis", "workflows", "assistant"],
     entry_points={
         "console_scripts": ["janis=janis_assistant.cli:process_args"],
         "janis.extension": ["assistant=janis_assistant"],
     },
     install_requires=[
-        "janis-pipelines.core>=0.9.0",
+        "janis-pipelines.core>=0.9.7",
         "janis-pipelines.templates>=0.9.0",
         "requests",
         "path.py",
         "python-dateutil",
         "progressbar2",
         "sqlitedict",
         "tabulate",
```

