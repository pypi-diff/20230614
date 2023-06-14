# Comparing `tmp/troubleshooter-1.0.8.tar.gz` & `tmp/troubleshooter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/troubleshooter-1.0.8.tar", last modified: Sat May 27 01:52:00 2023, max compression
+gzip compressed data, was "dist/troubleshooter-1.0.9.tar", last modified: Sat May 27 09:12:24 2023, max compression
```

## Comparing `troubleshooter-1.0.8.tar` & `troubleshooter-1.0.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:01.000000 troubleshooter-1.0.8/
--rwxrwxrwx   0 root         (0) root         (0)    11357 2023-04-19 06:32:30.000000 troubleshooter-1.0.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      472 2023-05-27 01:52:01.000000 troubleshooter-1.0.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2224 2023-05-16 11:01:20.000000 troubleshooter-1.0.8/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-27 01:52:01.000000 troubleshooter-1.0.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4001 2023-05-27 01:49:35.000000 troubleshooter-1.0.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/
--rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/proposer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/proposer/1_9/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/1_9/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3537 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/1_9/test_compile.py
--rwxrwxrwx   0 root         (0) root         (0)      482 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/1_9/test_ops.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/tests/proposer/master/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7485 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_ascend_vm.py
--rwxrwxrwx   0 root         (0) root         (0)    14663 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_compile.py
--rwxrwxrwx   0 root         (0) root         (0)     9667 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     3163 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_me_front.py
--rwxrwxrwx   0 root         (0) root         (0)     4310 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_ops.py
--rwxrwxrwx   0 root         (0) root         (0)     2572 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/proposer/master/test_st_output.py
--rwxrwxrwx   0 root         (0) root         (0)     1395 2023-04-19 06:32:34.000000 troubleshooter-1.0.8/tests/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/
--rwxrwxrwx   0 root         (0) root         (0)     1432 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/common/
--rwxrwxrwx   0 root         (0) root         (0)      893 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/common/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13403 2023-05-26 01:41:35.000000 troubleshooter-1.0.8/troubleshooter/common/format_msg.py
--rwxrwxrwx   0 root         (0) root         (0)     2071 2023-05-20 07:28:58.000000 troubleshooter-1.0.8/troubleshooter/common/framework_detection.py
--rwxrwxrwx   0 root         (0) root         (0)     1515 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/common/ms_callback.py
--rwxrwxrwx   0 root         (0) root         (0)     3789 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/common/ms_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     6105 2023-05-26 09:04:19.000000 troubleshooter-1.0.8/troubleshooter/common/util.py
--rwxrwxrwx   0 root         (0) root         (0)     3259 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/log.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/migrator/
--rwxrwxrwx   0 root         (0) root         (0)     1314 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6523 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/diff_handler.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/
--rwxrwxrwx   0 root         (0) root         (0)      686 2023-05-20 07:28:58.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      805 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_adapter.py
--rwxrwxrwx   0 root         (0) root         (0)     1461 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    12331 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/net_diff_finder.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/
--rwxrwxrwx   0 root         (0) root         (0)     1207 2023-05-24 09:27:50.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3022 2023-05-26 00:34:42.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/base_saver.py
--rwxrwxrwx   0 root         (0) root         (0)     1786 2023-05-26 00:34:42.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/mindspore_saver.py
--rwxrwxrwx   0 root         (0) root         (0)     1646 2023-05-26 00:34:42.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/torch_saver.py
--rwxrwxrwx   0 root         (0) root         (0)     2706 2023-05-24 09:27:50.000000 troubleshooter-1.0.8/troubleshooter/migrator/save/unified_saver.py
--rwxrwxrwx   0 root         (0) root         (0)    12874 2023-05-27 01:47:49.000000 troubleshooter-1.0.8/troubleshooter/migrator/weight_migrator.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/proposer/
--rwxrwxrwx   0 root         (0) root         (0)      797 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/
--rwxrwxrwx   0 root         (0) root         (0)     1838 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3242 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/base_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1533 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1548 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1479 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1438 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1243 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/default_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1682 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/front_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1476 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     1570 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_scene_proposer.py
--rwxrwxrwx   0 root         (0) root         (0)     2565 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/allproposers/vm_proposer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/
--rwxrwxrwx   0 root         (0) root         (0)      673 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1751 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/common_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    36588 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    16642 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     6744 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/front_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    28388 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/operators_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)    19787 2023-05-20 07:26:22.000000 troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/vm_exp_lib.py
--rwxrwxrwx   0 root         (0) root         (0)     3429 2023-05-20 07:27:16.000000 troubleshooter-1.0.8/troubleshooter/proposer/proposal_action.py
--rwxrwxrwx   0 root         (0) root         (0)     2237 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/proposer/proposer_factory.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/toolbox/
--rwxrwxrwx   0 root         (0) root         (0)      776 2023-05-25 01:37:45.000000 troubleshooter-1.0.8/troubleshooter/toolbox/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/
--rwxrwxrwx   0 root         (0) root         (0)      686 2023-05-20 07:28:58.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4161 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/alexnet.py
--rwxrwxrwx   0 root         (0) root         (0)     1762 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/cell.py
--rwxrwxrwx   0 root         (0) root         (0)     1128 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/demo.py
--rwxrwxrwx   0 root         (0) root         (0)    12883 2023-05-20 07:21:24.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     2557 2023-05-24 09:27:50.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/initialize.py
--rwxrwxrwx   0 root         (0) root         (0)     8212 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     1950 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_functional.py
--rwxrwxrwx   0 root         (0) root         (0)     2131 2023-05-20 07:21:24.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_nn.py
--rwxrwxrwx   0 root         (0) root         (0)     1890 2023-05-18 12:36:19.000000 troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_tensor.py
--rwxrwxrwx   0 root         (0) root         (0)     2803 2023-05-26 10:02:37.000000 troubleshooter-1.0.8/troubleshooter/toolbox/widget_pocket.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter/tracker/
--rwxrwxrwx   0 root         (0) root         (0)      774 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/tracker/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6685 2023-05-20 07:26:21.000000 troubleshooter-1.0.8/troubleshooter/tracker/tracker.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 01:52:00.000000 troubleshooter-1.0.8/troubleshooter.egg-info/
--r-xr-xr-x   0 root         (0) root         (0)      472 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/PKG-INFO
--r-xr-xr-x   0 root         (0) root         (0)     3174 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/SOURCES.txt
--r-xr-xr-x   0 root         (0) root         (0)        1 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/dependency_links.txt
--r-xr-xr-x   0 root         (0) root         (0)       36 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/requires.txt
--r-xr-xr-x   0 root         (0) root         (0)       21 2023-05-27 01:51:59.000000 troubleshooter-1.0.8/troubleshooter.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/
+-rwxrwxrwx   0 root         (0) root         (0)    11357 2023-04-19 06:32:30.000000 troubleshooter-1.0.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      472 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2224 2023-05-16 11:01:20.000000 troubleshooter-1.0.9/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4001 2023-05-27 09:08:21.000000 troubleshooter-1.0.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      668 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/tests/proposer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/tests/proposer/1_9/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/1_9/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3537 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/1_9/test_compile.py
+-rwxrwxrwx   0 root         (0) root         (0)      482 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/1_9/test_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/tests/proposer/master/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7485 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/test_ascend_vm.py
+-rwxrwxrwx   0 root         (0) root         (0)    14663 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/test_compile.py
+-rwxrwxrwx   0 root         (0) root         (0)     9667 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/test_dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     3163 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/test_me_front.py
+-rwxrwxrwx   0 root         (0) root         (0)     4310 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/test_ops.py
+-rwxrwxrwx   0 root         (0) root         (0)     2572 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/proposer/master/test_st_output.py
+-rwxrwxrwx   0 root         (0) root         (0)     1395 2023-04-19 06:32:34.000000 troubleshooter-1.0.9/tests/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter/
+-rwxrwxrwx   0 root         (0) root         (0)     1473 2023-05-27 07:34:23.000000 troubleshooter-1.0.9/troubleshooter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter/common/
+-rwxrwxrwx   0 root         (0) root         (0)      893 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/common/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    13403 2023-05-26 01:41:35.000000 troubleshooter-1.0.9/troubleshooter/common/format_msg.py
+-rwxrwxrwx   0 root         (0) root         (0)     2071 2023-05-20 07:28:58.000000 troubleshooter-1.0.9/troubleshooter/common/framework_detection.py
+-rwxrwxrwx   0 root         (0) root         (0)     1515 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/common/ms_callback.py
+-rwxrwxrwx   0 root         (0) root         (0)     3789 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/common/ms_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     6228 2023-05-27 07:06:10.000000 troubleshooter-1.0.9/troubleshooter/common/util.py
+-rwxrwxrwx   0 root         (0) root         (0)     3259 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/log.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter/migrator/
+-rwxrwxrwx   0 root         (0) root         (0)     1314 2023-05-27 01:47:49.000000 troubleshooter-1.0.9/troubleshooter/migrator/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6649 2023-05-27 07:57:20.000000 troubleshooter-1.0.9/troubleshooter/migrator/diff_handler.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/
+-rwxrwxrwx   0 root         (0) root         (0)      686 2023-05-20 07:28:58.000000 troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      805 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/weight_adapter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1461 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    12331 2023-05-27 01:47:49.000000 troubleshooter-1.0.9/troubleshooter/migrator/net_diff_finder.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter/migrator/save/
+-rwxrwxrwx   0 root         (0) root         (0)     1207 2023-05-24 09:27:50.000000 troubleshooter-1.0.9/troubleshooter/migrator/save/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3022 2023-05-26 00:34:42.000000 troubleshooter-1.0.9/troubleshooter/migrator/save/base_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)     1786 2023-05-26 00:34:42.000000 troubleshooter-1.0.9/troubleshooter/migrator/save/mindspore_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)     1646 2023-05-26 00:34:42.000000 troubleshooter-1.0.9/troubleshooter/migrator/save/torch_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)     2706 2023-05-24 09:27:50.000000 troubleshooter-1.0.9/troubleshooter/migrator/save/unified_saver.py
+-rwxrwxrwx   0 root         (0) root         (0)    12967 2023-05-27 08:18:15.000000 troubleshooter-1.0.9/troubleshooter/migrator/weight_migrator.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter/proposer/
+-rwxrwxrwx   0 root         (0) root         (0)      797 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/
+-rwxrwxrwx   0 root         (0) root         (0)     1838 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3242 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/base_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1533 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/compiler_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1548 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/compiler_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1479 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/dataset_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1438 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/dataset_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/default_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1682 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/front_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1476 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/operators_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1570 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/operators_scene_proposer.py
+-rwxrwxrwx   0 root         (0) root         (0)     2565 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/allproposers/vm_proposer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/
+-rwxrwxrwx   0 root         (0) root         (0)      673 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1751 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/common_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    36588 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    16642 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     6744 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/front_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    28388 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/operators_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)    19787 2023-05-20 07:26:22.000000 troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/vm_exp_lib.py
+-rwxrwxrwx   0 root         (0) root         (0)     3429 2023-05-20 07:27:16.000000 troubleshooter-1.0.9/troubleshooter/proposer/proposal_action.py
+-rwxrwxrwx   0 root         (0) root         (0)     2237 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/proposer/proposer_factory.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/troubleshooter/toolbox/
+-rwxrwxrwx   0 root         (0) root         (0)      767 2023-05-27 07:37:54.000000 troubleshooter-1.0.9/troubleshooter/toolbox/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/
+-rwxrwxrwx   0 root         (0) root         (0)      686 2023-05-20 07:28:58.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4161 2023-05-18 12:36:19.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/alexnet.py
+-rwxrwxrwx   0 root         (0) root         (0)     1762 2023-05-18 12:36:19.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/cell.py
+-rwxrwxrwx   0 root         (0) root         (0)     1128 2023-05-18 12:36:19.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/demo.py
+-rwxrwxrwx   0 root         (0) root         (0)    12883 2023-05-20 07:21:24.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2557 2023-05-24 09:27:50.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/initialize.py
+-rwxrwxrwx   0 root         (0) root         (0)     8212 2023-05-18 12:36:19.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1950 2023-05-18 12:36:19.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/wrap_functional.py
+-rwxrwxrwx   0 root         (0) root         (0)     2131 2023-05-20 07:21:24.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/wrap_nn.py
+-rwxrwxrwx   0 root         (0) root         (0)     1890 2023-05-18 12:36:19.000000 troubleshooter-1.0.9/troubleshooter/toolbox/dump/wrap_tensor.py
+-rwxrwxrwx   0 root         (0) root         (0)     2929 2023-05-27 07:27:32.000000 troubleshooter-1.0.9/troubleshooter/toolbox/widget_pocket.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:24.000000 troubleshooter-1.0.9/troubleshooter/tracker/
+-rwxrwxrwx   0 root         (0) root         (0)      774 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/tracker/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6685 2023-05-20 07:26:21.000000 troubleshooter-1.0.9/troubleshooter/tracker/tracker.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-05-27 09:12:22.000000 troubleshooter-1.0.9/troubleshooter/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter.egg-info/
+-r-xr-xr-x   0 root         (0) root         (0)      472 2023-05-27 09:12:22.000000 troubleshooter-1.0.9/troubleshooter.egg-info/PKG-INFO
+-r-xr-xr-x   0 root         (0) root         (0)     3174 2023-05-27 09:12:23.000000 troubleshooter-1.0.9/troubleshooter.egg-info/SOURCES.txt
+-r-xr-xr-x   0 root         (0) root         (0)        1 2023-05-27 09:12:22.000000 troubleshooter-1.0.9/troubleshooter.egg-info/dependency_links.txt
+-r-xr-xr-x   0 root         (0) root         (0)       36 2023-05-27 09:12:22.000000 troubleshooter-1.0.9/troubleshooter.egg-info/requires.txt
+-r-xr-xr-x   0 root         (0) root         (0)       21 2023-05-27 09:12:22.000000 troubleshooter-1.0.9/troubleshooter.egg-info/top_level.txt
```

### Comparing `troubleshooter-1.0.8/LICENSE` & `troubleshooter-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/README.md` & `troubleshooter-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/setup.py` & `troubleshooter-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import shutil
 import subprocess
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command.egg_info import egg_info
 from setuptools.command.build_py import build_py
 
-version = '1.0.8'
+version = '1.0.9'
 cur_dir = os.path.dirname(os.path.realpath(__file__))
 pkg_dir = os.path.join(cur_dir, 'build')
 
 
 def clean():
     """clean"""
     def readonly_handler(func, path, execinfo):
```

### Comparing `troubleshooter-1.0.8/tests/__init__.py` & `troubleshooter-1.0.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/1_9/test_compile.py` & `troubleshooter-1.0.9/tests/proposer/1_9/test_compile.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/master/test_ascend_vm.py` & `troubleshooter-1.0.9/tests/proposer/master/test_ascend_vm.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/master/test_compile.py` & `troubleshooter-1.0.9/tests/proposer/master/test_compile.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/master/test_dataset.py` & `troubleshooter-1.0.9/tests/proposer/master/test_dataset.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/master/test_me_front.py` & `troubleshooter-1.0.9/tests/proposer/master/test_me_front.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/master/test_ops.py` & `troubleshooter-1.0.9/tests/proposer/master/test_ops.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/proposer/master/test_st_output.py` & `troubleshooter-1.0.9/tests/proposer/master/test_st_output.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/tests/util.py` & `troubleshooter-1.0.9/tests/util.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/__init__.py` & `troubleshooter-1.0.9/troubleshooter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,7 +24,8 @@
 """
 from __future__ import absolute_import
 from troubleshooter.common import FRAMEWORK_TYPE
 from troubleshooter import common, migrator, proposer, tracker
 from troubleshooter.migrator import save
 from troubleshooter.proposer import ProposalAction as proposal
 from troubleshooter.tracker import Tracker as tracking
+from troubleshooter.toolbox import widget
```

### Comparing `troubleshooter-1.0.8/troubleshooter/common/__init__.py` & `troubleshooter-1.0.9/troubleshooter/common/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/common/format_msg.py` & `troubleshooter-1.0.9/troubleshooter/common/format_msg.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/common/framework_detection.py` & `troubleshooter-1.0.9/troubleshooter/common/framework_detection.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/common/ms_callback.py` & `troubleshooter-1.0.9/troubleshooter/common/ms_callback.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/common/ms_utils.py` & `troubleshooter-1.0.9/troubleshooter/common/ms_utils.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/common/util.py` & `troubleshooter-1.0.9/troubleshooter/common/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,16 +100,17 @@
     normal_dir = validate_and_normalize_path(dir)
     walk_generator = os.walk(normal_dir)
     for root_path, dirs, files in walk_generator:
         if len(files) < 1:
             continue
         for file in files:
             file_name, suffix_name = os.path.splitext(file)
-            if suffix_name == suffix:
+            if suffix_name == suffix and root_path == normal_dir:
                 file_list.append(file)
+    file_list = sorted(file_list, key=lambda x: os.path.getctime(os.path.join(normal_dir, x)))
     return file_list
 
 
 def make_directory(path: str):
     """Make directory."""
     if path is None or not isinstance(path, str) or path.strip() == "":
         raise TypeError("Input path '{}' is invalid type".format(path))
```

### Comparing `troubleshooter-1.0.8/troubleshooter/log.py` & `troubleshooter-1.0.9/troubleshooter/log.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/__init__.py` & `troubleshooter-1.0.9/troubleshooter/migrator/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/diff_handler.py` & `troubleshooter-1.0.9/troubleshooter/migrator/diff_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from troubleshooter import log as logger
 
 __all__ = [
     "get_filename_map_list",
     "compare_npy_dir",
     "get_list_filename_map_list",
     "compare_list_npy_dir",
+    "compare_grads_dir",
     "cal_algorithm",
     "cal_cosine_sim"
 ]
 
 def get_filename_map_list(orig_dir, target_dir):
     name_map_list = []
     orig_name_list = find_file(orig_dir)
@@ -76,17 +77,19 @@
 
     for name_map in name_map_list:
         orig_name = name_map[0]
         target_name = name_map[1]
 
         if orig_name is None or target_name is None:
             result = False
+            rel_ratio = 0
+            cosine_sim = 0
             diff_detail = ()
             result_list.append(
-                (orig_name, target_name, result, diff_detail))
+                (orig_name, target_name, result, rel_ratio, cosine_sim,diff_detail))
             continue
 
         orig_file = os.path.join(normal_orig_dir, orig_name)
         target_file = os.path.join(normal_target_dir, target_name)
 
         if not os.path.isfile(orig_file) or not os.path.isfile(target_file):
             continue
@@ -121,18 +124,18 @@
 
 
 def compare_list_npy_dir(orig_dir, target_dir, *, name_map_list=None, **kwargs):
     none_and_isdir_check(orig_dir, 'orig_dir')
     none_and_isdir_check(target_dir, 'target_dir')
     if name_map_list is None:
         name_map_list = get_list_filename_map_list(orig_dir, target_dir)
-    compare_npy_dir(name_map_list=name_map_list, **kwargs)
+    compare_npy_dir(orig_dir, target_dir, name_map_list=name_map_list, **kwargs)
 
 
-compare_grads = compare_list_npy_dir
+compare_grads_dir = compare_list_npy_dir
 
 
 def cal_algorithm(orig_value, target_value, rtol, atol, equal_nan):
     if orig_value.shape == target_value.shape:
         result = np.allclose(orig_value, target_value, rtol=rtol, atol=atol, equal_nan=equal_nan)
         if not result:
             value_diff = np.abs(orig_value - target_value)
```

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/__init__.py` & `troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_adapter.py` & `troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/weight_adapter.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py` & `troubleshooter-1.0.9/troubleshooter/migrator/mapping_relation/weight_mapping_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/net_diff_finder.py` & `troubleshooter-1.0.9/troubleshooter/migrator/net_diff_finder.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/save/__init__.py` & `troubleshooter-1.0.9/troubleshooter/migrator/save/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/save/base_saver.py` & `troubleshooter-1.0.9/troubleshooter/migrator/save/base_saver.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/save/mindspore_saver.py` & `troubleshooter-1.0.9/troubleshooter/migrator/save/mindspore_saver.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/save/torch_saver.py` & `troubleshooter-1.0.9/troubleshooter/migrator/save/torch_saver.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/save/unified_saver.py` & `troubleshooter-1.0.9/troubleshooter/migrator/save/unified_saver.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/migrator/weight_migrator.py` & `troubleshooter-1.0.9/troubleshooter/migrator/weight_migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,18 +277,20 @@
 def compare_pth_and_ckpt(weight_map_path=None, pt_file_path=None, ms_file_path=None, **kwargs):
     temp_save_path = validate_and_normalize_path(kwargs.get('temp_save_path', './'))
     timestamp = time.time()
     formatted_time = time.strftime('%Y%m%d-%H%M%S', time.localtime(timestamp))
     temp_name = formatted_time + "_ts_temp_file.ckpt"
     tmp_ckpt_file = os.path.join(temp_save_path, temp_name)
     print_level = kwargs.get('print_level', 1)
+    print_conv_info = kwargs.get('print_conv_info', False)
+
 
     none_and_isfile_check(weight_map_path, 'weight_map_path')
     none_and_isfile_check(pt_file_path, 'pt_file_path')
     none_and_isfile_check(ms_file_path, 'ms_file_path')
 
     convert_weight(weight_map_path=weight_map_path, pt_file_path=pt_file_path, ms_file_save_path=tmp_ckpt_file,
-                                  print_level=print_level)
+                                  print_conv_info=print_conv_info)
     compare_ms_ckpt(orig_file_path=tmp_ckpt_file, target_file_path=ms_file_path,
-                    compare_value=True, weight_map_path=weight_map_path)
+                    compare_value=True, weight_map_path=weight_map_path, print_level=print_level)
     clear_tmp_file(tmp_ckpt_file)
```

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/__init__.py` & `troubleshooter-1.0.9/troubleshooter/proposer/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/__init__.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/base_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/base_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/compiler_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/compiler_scene_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/compiler_scene_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/dataset_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/dataset_scene_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/dataset_scene_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/default_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/default_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/front_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/front_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/operators_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/operators_scene_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/operators_scene_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/allproposers/vm_proposer.py` & `troubleshooter-1.0.9/troubleshooter/proposer/allproposers/vm_proposer.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/__init__.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/__init__.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/common_exp_lib.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/common_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/compiler_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/dataset_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/front_exp_lib.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/front_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/operators_exp_lib.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/operators_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/knowledge_base/vm_exp_lib.py` & `troubleshooter-1.0.9/troubleshooter/proposer/knowledge_base/vm_exp_lib.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/proposal_action.py` & `troubleshooter-1.0.9/troubleshooter/proposer/proposal_action.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/proposer/proposer_factory.py` & `troubleshooter-1.0.9/troubleshooter/proposer/proposer_factory.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/__init__.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,12 +8,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ============================================================================
-__all__ = [
-    'widget'
-]
-
-from troubleshooter.toolbox import widget_pocket as widget
```

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/__init__.py` & `troubleshooter-1.0.9/troubleshooter/tracker/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# Copyright 2022-2023 Huawei Technologies Co., Ltd
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+"""Proposer for profiler."""
+from troubleshooter.tracker.tracker import Tracker
+__all__ = ["Tracker"]
```

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/alexnet.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/alexnet.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/cell.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/cell.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/demo.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/demo.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/hooks.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/hooks.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/initialize.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/initialize.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/utils.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/utils.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_functional.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/wrap_functional.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_nn.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/wrap_nn.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/dump/wrap_tensor.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/dump/wrap_tensor.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter/toolbox/widget_pocket.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/widget_pocket.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 # limitations under the License.
 # ============================================================================
 import random
 import os
 import numpy as np
 from troubleshooter.common.util import validate_and_normalize_path
 
+__all__ = [
+    "fix_random",
+    "get_pt_grads",
+    "load_ms_weight2net",
+    "object_load",
+    "object_dump",
+]
+
 FW_PT=True
 FW_MS=True
 
 
 try:
     import torch
 except ModuleNotFoundError as e:
@@ -57,16 +65,16 @@
         if FW_MS:
             mindspore.set_seed(seed)
 
 
 def get_pt_grads(model):
     grads_dict = {}
     i=0
-    for name ,params in model.named_parmeters():
-        name = name + '-' + str(i)
+    for name ,params in model.named_parameters():
+        name = name + '_' + str(i)
         grads_dict.update({name:params.grad})
         i += 1
     return grads_dict
 
 
 def load_ms_weight2net(model,file):
     file = validate_and_normalize_path(file)
```

### Comparing `troubleshooter-1.0.8/troubleshooter/tracker/__init__.py` & `troubleshooter-1.0.9/troubleshooter/toolbox/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# Copyright 2022-2023 Huawei Technologies Co., Ltd
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ============================================================================
-"""Proposer for profiler."""
-from troubleshooter.tracker.tracker import Tracker
-__all__ = ["Tracker"]
+# Copyright 2022-2023 Huawei Technologies Co., Ltd
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ============================================================================
+from troubleshooter.toolbox import widget_pocket as widget
+__all__ = ["widget",]
```

### Comparing `troubleshooter-1.0.8/troubleshooter/tracker/tracker.py` & `troubleshooter-1.0.9/troubleshooter/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `troubleshooter-1.0.8/troubleshooter.egg-info/SOURCES.txt` & `troubleshooter-1.0.9/troubleshooter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

