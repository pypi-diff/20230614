# Comparing `tmp/coiled-0.7.5.dev3.tar.gz` & `tmp/coiled-0.7.5.dev5.tar.gz`

## Comparing `coiled-0.7.5.dev3.tar` & `coiled-0.7.5.dev5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/analytics.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/coiled.yaml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/context.py
--rw-r--r--   0        0        0   102119 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/exceptions.py
--rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/magic.py
--rw-r--r--   0        0        0    13390 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/software.py
--rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/types.py
--rw-r--r--   0        0        0    52368 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/websockets.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    89772 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    58518 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/core.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/login.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/cluster/metrics.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    44216 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/pyproject.toml
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.7.5.dev3/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/analytics.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/context.py
+-rw-r--r--   0        0        0   102119 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/exceptions.py
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/magic.py
+-rw-r--r--   0        0        0    13390 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/software.py
+-rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/types.py
+-rw-r--r--   0        0        0    52368 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/websockets.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    89772 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    58518 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/core.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/login.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/cluster/metrics.py
+-rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    44216 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/pyproject.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 coiled-0.7.5.dev5/PKG-INFO
```

### Comparing `coiled-0.7.5.dev3/coiled/__init__.py` & `coiled-0.7.5.dev5/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/analytics.py` & `coiled-0.7.5.dev5/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cluster.py` & `coiled-0.7.5.dev5/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/coiled.yaml` & `coiled-0.7.5.dev5/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/context.py` & `coiled-0.7.5.dev5/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/core.py` & `coiled-0.7.5.dev5/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/exceptions.py` & `coiled-0.7.5.dev5/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/magic.py` & `coiled-0.7.5.dev5/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/scan.py` & `coiled-0.7.5.dev5/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/software.py` & `coiled-0.7.5.dev5/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/types.py` & `coiled-0.7.5.dev5/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/utils.py` & `coiled-0.7.5.dev5/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/websockets.py` & `coiled-0.7.5.dev5/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/__init__.py` & `coiled-0.7.5.dev5/coiled/_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/cluster.py` & `coiled-0.7.5.dev5/coiled/_beta/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/core.py` & `coiled-0.7.5.dev5/coiled/_beta/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/cwi_log_link.py` & `coiled-0.7.5.dev5/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/states.py` & `coiled-0.7.5.dev5/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/widgets/__init__.py` & `coiled-0.7.5.dev5/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/widgets/rich.py` & `coiled-0.7.5.dev5/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/_beta/widgets/util.py` & `coiled-0.7.5.dev5/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/config.py` & `coiled-0.7.5.dev5/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/core.py` & `coiled-0.7.5.dev5/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/curl.py` & `coiled-0.7.5.dev5/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/env.py` & `coiled-0.7.5.dev5/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/login.py` & `coiled-0.7.5.dev5/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/package_sync.py` & `coiled-0.7.5.dev5/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/utils.py` & `coiled-0.7.5.dev5/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/cluster/__init__.py` & `coiled-0.7.5.dev5/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/cluster/better_logs.py` & `coiled-0.7.5.dev5/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/cluster/logs.py` & `coiled-0.7.5.dev5/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/cluster/metrics.py` & `coiled-0.7.5.dev5/coiled/cli/cluster/metrics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/cluster/ssh.py` & `coiled-0.7.5.dev5/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/cluster/utils.py` & `coiled-0.7.5.dev5/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/notebook/__init__.py` & `coiled-0.7.5.dev5/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/notebook/notebook.py` & `coiled-0.7.5.dev5/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/setup/__init__.py` & `coiled-0.7.5.dev5/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/setup/amp.py` & `coiled-0.7.5.dev5/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/setup/aws.py` & `coiled-0.7.5.dev5/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/setup/entry.py` & `coiled-0.7.5.dev5/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/setup/gcp.py` & `coiled-0.7.5.dev5/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/cli/setup/prometheus.py` & `coiled-0.7.5.dev5/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/coiled/v2/__init__.py` & `coiled-0.7.5.dev5/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/LICENSE` & `coiled-0.7.5.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/README.md` & `coiled-0.7.5.dev5/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/pyproject.toml` & `coiled-0.7.5.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.7.5.dev3/PKG-INFO` & `coiled-0.7.5.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.7.5.dev3
+Version: 0.7.5.dev5
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.7.5.dev3 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.7.5.dev5 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
 Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
```

