# Comparing `tmp/vss-cli-2023.6.0.tar.gz` & `tmp/vss-cli-2023.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2023.6.0.tar", last modified: Wed Jun 14 19:12:13 2023, max compression
+gzip compressed data, was "vss-cli-2023.6.0.dev0.tar", last modified: Wed Jun 14 16:01:10 2023, max compression
```

## Comparing `vss-cli-2023.6.0.tar` & `vss-cli-2023.6.0.dev0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.015714 vss-cli-2023.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12454 2023-06-14 19:12:13.015714 vss-cli-2023.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-14 19:12:13.015714 vss-cli-2023.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:12.999714 vss-cli-2023.6.0/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18320 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7453 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    62673 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    13882 2023-06-14 19:02:56.000000 vss-cli-2023.6.0/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.003714 vss-cli-2023.6.0/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-06-14 19:02:56.000000 vss-cli-2023.6.0/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4065 2023-06-14 19:02:56.000000 vss-cli-2023.6.0/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2946 2023-06-14 19:02:56.000000 vss-cli-2023.6.0/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3993 2023-06-14 19:02:56.000000 vss-cli-2023.6.0/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25272 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.007714 vss-cli-2023.6.0/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 19:12:08.000000 vss-cli-2023.6.0/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.011714 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2838 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9402 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   139900 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.015714 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.015714 vss-cli-2023.6.0/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-14 16:00:18.000000 vss-cli-2023.6.0/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 19:12:13.003714 vss-cli-2023.6.0/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12454 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2388 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 19:12:12.000000 vss-cli-2023.6.0/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.590262 vss-cli-2023.6.0.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-06-14 16:01:10.590262 vss-cli-2023.6.0.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11153 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-06-14 16:01:10.590262 vss-cli-2023.6.0.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.578262 vss-cli-2023.6.0.dev0/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18320 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7453 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    62673 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    13887 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.582262 vss-cli-2023.6.0.dev0/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4070 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25272 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.586262 vss-cli-2023.6.0.dev0/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-14 16:01:06.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.586262 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9105 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2838 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9402 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   139900 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.590262 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.590262 vss-cli-2023.6.0.dev0/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-06-14 16:00:18.000000 vss-cli-2023.6.0.dev0/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 16:01:10.578262 vss-cli-2023.6.0.dev0/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12464 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 16:01:10.000000 vss-cli-2023.6.0.dev0/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2023.6.0/LICENSE` & `vss-cli-2023.6.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/PKG-INFO` & `vss-cli-2023.6.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2023.6.0
+Version: 2023.6.0.dev0
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.0-dev0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
```

### Comparing `vss-cli-2023.6.0/README.md` & `vss-cli-2023.6.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/setup.cfg` & `vss-cli-2023.6.0.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/setup.py` & `vss-cli-2023.6.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/autocompletion.py` & `vss-cli-2023.6.0.dev0/vss_cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/cli.py` & `vss-cli-2023.6.0.dev0/vss_cli/cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/config.py` & `vss-cli-2023.6.0.dev0/vss_cli/config.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/const.py` & `vss-cli-2023.6.0.dev0/vss_cli/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
 
 import pkg_resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2023.6.0"
+__version__ = "2023.6.0-dev0"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
 _LEGACY_CONFIG = ("~", ".vss-cli", "config.json")
```

### Comparing `vss-cli-2023.6.0/vss_cli/data/clib.yaml` & `vss-cli-2023.6.0.dev0/vss_cli/data/clib.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2023.6.0             #
+#     VSS-CLI Spec from CLib 2023.6.0-dev0             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
```

### Comparing `vss-cli-2023.6.0/vss_cli/data/clone.yaml` & `vss-cli-2023.6.0.dev0/vss_cli/data/clone.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2023.6.0             #
+#     VSS-CLI Spec from Clone 2023.6.0-dev0             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
```

### Comparing `vss-cli-2023.6.0/vss_cli/data/config.yaml` & `vss-cli-2023.6.0.dev0/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/data/image.yaml` & `vss-cli-2023.6.0.dev0/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/data/shell.yaml` & `vss-cli-2023.6.0.dev0/vss_cli/data/shell.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM v2023.6.0             #
+#     VSS-CLI Spec shell VM v2023.6.0-dev0             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
```

### Comparing `vss-cli-2023.6.0/vss_cli/data/template.yaml` & `vss-cli-2023.6.0.dev0/vss_cli/data/template.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template v2023.6.0         #
+#     VSS-CLI Spec from Template v2023.6.0-dev0         #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:
```

### Comparing `vss-cli-2023.6.0/vss_cli/data_types.py` & `vss-cli-2023.6.0.dev0/vss_cli/data_types.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/hcio.py` & `vss-cli-2023.6.0.dev0/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/helper.py` & `vss-cli-2023.6.0.dev0/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/account.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/completion.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/domain.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/helper.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/vm.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/configure.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/key.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/message.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/misc.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/ovf.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/plugins.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/raw.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/raw.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/service.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/shell.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/status.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/stor.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/token.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/plugins/upgrade.py` & `vss-cli-2023.6.0.dev0/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/rel_opts.py` & `vss-cli-2023.6.0.dev0/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/sstatus.py` & `vss-cli-2023.6.0.dev0/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/utils/emoji.py` & `vss-cli-2023.6.0.dev0/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/utils/threading.py` & `vss-cli-2023.6.0.dev0/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/validators.py` & `vss-cli-2023.6.0.dev0/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/vss.py` & `vss-cli-2023.6.0.dev0/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli/yaml.py` & `vss-cli-2023.6.0.dev0/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli.egg-info/PKG-INFO` & `vss-cli-2023.6.0.dev0/vss_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2023.6.0
+Version: 2023.6.0.dev0
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.6.0-dev0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
```

### Comparing `vss-cli-2023.6.0/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2023.6.0.dev0/vss_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.6.0/vss_cli.egg-info/requires.txt` & `vss-cli-2023.6.0.dev0/vss_cli.egg-info/requires.txt`

 * *Files identical despite different names*

