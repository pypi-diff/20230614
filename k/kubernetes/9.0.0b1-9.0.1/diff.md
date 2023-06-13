# Comparing `tmp/kubernetes-9.0.0b1.tar.gz` & `tmp/kubernetes-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kubernetes-9.0.0b1.tar", last modified: Wed Feb 13 03:21:20 2019, max compression
+gzip compressed data, was "dist/kubernetes-9.0.1.tar", last modified: Mon Aug 12 19:47:14 2019, max compression
```

## Comparing `kubernetes-9.0.0b1.tar` & `kubernetes-9.0.1.tar`

### file list

```diff
@@ -1,688 +1,688 @@
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/
--rw-r--r--   0 haoweic  (484802) eng       (5000)     1045 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/PKG-INFO
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11354 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/LICENSE
--rw-r--r--   0 haoweic  (484802) eng       (5000)      331 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/requirements.txt
--rw-r--r--   0 haoweic  (484802) eng       (5000)    19917 2019-02-13 03:20:38.000000 kubernetes-9.0.0b1/CHANGELOG.md
--rw-r--r--   0 haoweic  (484802) eng       (5000)      148 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/code-of-conduct.md
--rw-r--r--   0 haoweic  (484802) eng       (5000)      175 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/test-requirements.txt
--rw-r--r--   0 haoweic  (484802) eng       (5000)      132 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/MANIFEST.in
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10114 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/README.md
--rw-r--r--   0 haoweic  (484802) eng       (5000)      523 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/RELEASE.md
--rw-r--r--   0 haoweic  (484802) eng       (5000)     2894 2019-02-13 03:20:38.000000 kubernetes-9.0.0b1/setup.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     1449 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/CONTRIBUTING.md
--rw-r--r--   0 haoweic  (484802) eng       (5000)     1062 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/tox.ini
--rw-r--r--   0 haoweic  (484802) eng       (5000)      130 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/OWNERS
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes.egg-info/
--rw-r--r--   0 haoweic  (484802) eng       (5000)     1045 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 haoweic  (484802) eng       (5000)    34840 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 haoweic  (484802) eng       (5000)      260 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes.egg-info/requires.txt
--rw-r--r--   0 haoweic  (484802) eng       (5000)       11 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes.egg-info/top_level.txt
--rw-r--r--   0 haoweic  (484802) eng       (5000)        1 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 haoweic  (484802) eng       (5000)      159 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/setup.cfg
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes/
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/kubernetes/config/
--rw-r--r--   0 haoweic  (484802) eng       (5000)    21210 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/kube_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     2226 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/dateutil_test.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3538 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/exec_provider.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)      655 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/config_exception.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)      830 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/__init__.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4997 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/exec_provider_test.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     2657 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/dateutil.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3546 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/incluster_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    37516 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/kube_config_test.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4747 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/config/incluster_config_test.py
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/kubernetes/stream/
--rw-r--r--   0 haoweic  (484802) eng       (5000)      638 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/stream/__init__.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9412 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/stream/ws_client.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     1320 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/stream/stream.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     1452 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/stream/ws_client_test.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)      814 2019-02-13 03:20:38.000000 kubernetes-9.0.0b1/kubernetes/__init__.py
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/kubernetes/utils/
--rw-r--r--   0 haoweic  (484802) eng       (5000)      635 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/utils/__init__.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3180 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/utils/create_from_yaml.py
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/kubernetes/watch/
--rw-r--r--   0 haoweic  (484802) eng       (5000)      636 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/watch/__init__.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10181 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/watch/watch_test.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5162 2019-02-13 03:20:25.000000 kubernetes-9.0.0b1/kubernetes/watch/watch.py
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:19.000000 kubernetes-9.0.0b1/kubernetes/client/
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7835 2019-02-13 03:20:38.000000 kubernetes-9.0.0b1/kubernetes/client/configuration.py
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/kubernetes/client/apis/
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4305 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/auditregistration_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4283 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/events_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4297 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/authorization_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4291 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/scheduling_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   482166 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apps_v1beta2_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   115535 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/admissionregistration_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4306 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    95120 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    27022 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/authorization_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4274 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/batch_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4301 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apiregistration_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4284 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/extensions_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   480916 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apps_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4287 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/settings_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4111 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/version_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   112086 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/storage_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7308 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/logs_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    57813 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/auditregistration_v1alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    91264 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/batch_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9647 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/authentication_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   251736 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_v1alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4286 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   127236 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/storage_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    95350 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_v2beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9607 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/authentication_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4297 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apiextensions_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    74892 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/coordination_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4313 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/admissionregistration_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    72863 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apiregistration_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)  1441124 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/core_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    26892 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/authorization_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   148870 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/policy_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4299 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/authentication_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3051 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/__init__.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    59409 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/admissionregistration_v1alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    92309 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/batch_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    58169 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/scheduling_v1alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4272 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apps_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    58447 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/storage_v1alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   160947 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/custom_objects_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    73073 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apiregistration_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   251622 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4295 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/certificates_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    75782 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/networking_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4296 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/core_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4300 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apis_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4295 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/coordination_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   251052 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_v1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    58141 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/scheduling_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   294885 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apps_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)   543396 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/extensions_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    81189 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/certificates_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    75311 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/apiextensions_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4285 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/storage_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    75450 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/settings_v1alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    74836 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/events_v1beta1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    95350 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_v2beta2_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    92355 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/batch_v2alpha1_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4291 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/networking_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4276 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/apis/policy_api.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13463 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/rest.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    43360 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/__init__.py
-drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-02-13 03:21:20.000000 kubernetes-9.0.0b1/kubernetes/client/models/
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4213 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ip_block.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7643 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11757 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_io_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13806 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_storage_class.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7387 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_role_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4506 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_run_as_user_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7443 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7387 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3827 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_aggregation_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6265 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_account_token_projection.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4334 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_update_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6494 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_lease_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6693 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_rolling_update_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5086 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cross_version_object_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6708 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_env_var_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3268 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6476 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_binding_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12939 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_iscsi_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3812 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_event_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6862 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_downward_api_volume_file.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4296 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6922 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7613 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4367 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_job_template_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8875 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/version_info.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7062 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_token_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4688 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_initializer.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8249 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_port.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4794 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_label_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8309 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_os_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3543 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4356 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_job_template_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8038 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7633 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7412 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_flex_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13591 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_class.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7678 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_rules_review_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5547 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_user_info.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    35510 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3623 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_topology_selector_term.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7751 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7311 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_job_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4485 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_weighted_pod_affinity_term.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7413 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_controller_revision.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7033 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6170 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5564 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_glusterfs_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5550 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_selector_requirement.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6478 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3956 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state_waiting.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6670 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6967 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_port.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5310 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3428 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_load_balancer_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3637 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_dns_config_option.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8096 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_owner_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    14181 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9609 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7901 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_webhook_client_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5993 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoint_address.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10645 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_rbd_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3338 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_http_ingress_rule_value.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8597 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6790 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cinder_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7732 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_scale.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6070 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_projection.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3240 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_scale_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7456 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12340 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7892 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7961 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7782 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_affinity.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13917 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_job_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7078 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6939 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_mutating_webhook_configuration.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6119 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_subject.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8139 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_versions.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6398 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6660 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5249 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_nfs_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7110 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6855 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    39757 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6744 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_controller_revision_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4352 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7806 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_rollback.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3381 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_daemon_endpoints.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6405 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_http_get_action.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7787 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7532 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4244 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_topology_selector_label_requirement.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8664 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6604 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_pod_preset_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7892 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12340 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5565 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_group_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3375 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6710 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5593 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3901 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_address.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13018 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6920 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7245 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5476 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_value_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6690 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4397 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_selector_term.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3540 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_validation.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4348 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_update_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7207 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_token_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4612 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_se_linux_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6695 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7561 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7758 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3830 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_exec_action.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4575 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_run_as_group_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7962 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_rollback.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4296 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_flocker_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7436 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_affinity.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6690 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5057 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apiextensions_v1beta1_service_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7178 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5234 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_portworx_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4482 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_port.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6520 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7558 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_scale.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6558 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_peer.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4436 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8198 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4700 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_allowed_host_path.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3135 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3286 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9609 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3254 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_local_object_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3820 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_aggregation_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7110 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10624 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8088 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4125 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_device.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3484 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3780 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_non_resource_attributes.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    30353 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3013 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_preconditions.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5064 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_key_to_path.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4513 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6176 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_role_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12578 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_csi_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6571 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_list_meta.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6728 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_token_review_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7365 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_rules_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    14466 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4118 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_image.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6791 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_access_review_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3409 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8038 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_metric_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11888 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_security_context.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6622 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6764 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7197 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_flex_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4649 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_server_address_by_client_cidr.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7338 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_lease_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    14236 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6375 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5399 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_env_var.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4969 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_rolling_update_daemon_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4796 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_key_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4124 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_resource_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5515 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_status_cause.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3372 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3323 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_session_affinity_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4801 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_handler.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5565 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_taint.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8689 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_column_definition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    16482 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4562 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_run_as_user_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9975 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7404 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4248 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_external_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3778 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_http_header.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4327 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_preferred_scheduling_term.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7395 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6070 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6766 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3958 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7485 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_initializer_configuration.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12963 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7866 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_anti_affinity.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6660 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5593 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_dns_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6948 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4824 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_access_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6512 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role_binding_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6938 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_initializer_configuration_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8415 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_ceph_fs_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7091 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4162 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_resource_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6126 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5471 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_ingress_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6764 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9873 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    17131 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_event.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4789 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6564 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7617 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6302 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7612 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_node_config_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5192 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_git_repo_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7744 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7454 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_access_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4286 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_external_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    27459 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_object_meta.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3526 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6073 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_scale_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7813 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_job_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6324 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_job_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6452 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_lease.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7762 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6764 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4264 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_update_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    22625 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3449 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3987 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_host_port_range.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6460 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4443 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_identifier.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7060 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_validating_webhook_configuration_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4568 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_se_linux_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6476 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8094 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_os_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7370 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6733 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_pod_preset_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5369 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_label_selector_requirement.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3271 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state_running.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    35941 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/__init__.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6722 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3318 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4991 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_field_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4957 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6769 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4059 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apiregistration_v1beta1_service_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7286 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_access_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5918 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_pods_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7757 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6648 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3293 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_rules_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8827 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_resource_attributes.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7662 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6962 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_mount.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3471 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9310 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_priority_class.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7744 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6372 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_azure_file_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6769 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6166 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_role.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3277 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_rollback_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7425 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8291 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_names.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6758 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_account_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    14115 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4717 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoint_port.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6309 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_target.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6350 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_event_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4600 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_non_resource_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4969 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_rolling_update_daemon_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8445 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_policy_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8747 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6610 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3519 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5254 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_egress_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7358 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_rule_with_operations.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4158 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_ip_block.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6702 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7067 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4545 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_non_resource_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3750 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_sysctl.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9611 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8121 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_access_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6552 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8398 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5843 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_pods_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9918 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_account.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11027 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6596 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_rolling_update_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4877 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_service_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13394 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_iscsi_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9039 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6112 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_pod_preset.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7377 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_aws_elastic_block_store_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11682 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_delete_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6654 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7538 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7613 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_local_subject_access_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10969 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_version.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7383 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3219 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_downward_api_projection.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7431 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_access_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6558 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12720 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_system_info.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4293 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_backend.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5118 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_azure_file_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10475 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3971 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_error.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7669 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_toleration.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6790 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4730 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_event_series.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4251 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10869 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_resource.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7591 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6816 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_pod_security_policy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10837 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3973 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_env_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10606 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_config_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7608 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_object_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5386 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_ingress_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4905 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_tls.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6694 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_priority_class_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5341 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_conversion.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4600 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4063 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_attached_volume.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6580 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6759 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_rolling_update_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13970 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_security_context.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3451 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/runtime_raw_extension.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    18454 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_event.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4233 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_watch_event.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    31227 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_pod_security_policy_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6356 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_audit_sink_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5202 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3317 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_allowed_flex_volume.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6212 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_audit_sink.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7528 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_controller_revision.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3835 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_non_resource_attributes.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6710 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7913 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3643 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_capabilities.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7283 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoints.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3785 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_aggregation_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4451 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_fs_group_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8261 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/admissionregistration_v1beta1_webhook_client_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12250 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_webhook.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6644 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role_binding_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3287 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_config_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4155 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_subresources.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4240 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7527 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_object_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10548 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7178 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6448 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4615 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_downward_api_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6560 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4656 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_initializers.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7346 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_gce_persistent_disk_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5124 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_typed_local_object_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7322 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6695 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5747 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_component_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6545 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12130 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6663 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_fc_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5779 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8348 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_policy_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3178 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_initializer.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6634 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_controller_revision_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3170 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_scale_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7807 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4012 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_env_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7758 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_local_subject_access_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7012 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_mutating_webhook_configuration_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6302 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4444 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_token_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10650 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6714 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_resource_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6978 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6298 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7453 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6323 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_subject.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5126 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_event_series.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3484 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scope_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6428 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5088 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_empty_dir_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5612 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scoped_resource_selector_requirement.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    29617 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_json_schema_props.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4499 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_token_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4039 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_policy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6192 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4026 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_error.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4010 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_webhook_throttle_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7528 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_controller_revision.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4375 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_photon_persistent_disk_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6344 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_role_binding_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5292 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4223 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_template_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7858 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range_item.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12282 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6648 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_storage_class_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6595 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4284 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_host_path_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4037 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_error.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7297 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scale.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6454 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_binding_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4366 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_update_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3450 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_readiness_gate.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6454 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6606 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_component_status_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6619 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6615 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cinder_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4733 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_ref.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7348 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4112 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4748 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_ref.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10310 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_rbd_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7209 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6648 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_peer.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6013 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_scale_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4219 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_port.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3414 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_rolling_update_stateful_set_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7802 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4030 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_tcp_socket_action.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    14466 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6558 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8123 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9830 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_group.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6803 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_quobyte_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6451 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7508 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5161 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_cross_version_object_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4519 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_run_as_group_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4226 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6838 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_token_review_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7452 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12170 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_io_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6318 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6280 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3789 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_external_documentation.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9283 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_priority_class.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7607 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_subresource_scale.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6728 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_pod_security_policy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11407 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8148 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_status_details.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4235 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_object_field_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4871 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_env_from_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8728 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7488 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role_binding.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6548 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6672 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_priority_class_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3589 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_client_ip_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6886 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_access_review_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7172 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_glusterfs_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7952 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4751 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_key_selector.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4658 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_role_ref.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6538 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_class_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5567 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoint_subset.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4072 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_load_balancer_ingress.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7978 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5161 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_cross_version_object_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4204 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_pods_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7599 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5854 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_affinity_term.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6420 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6585 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_component_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7442 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_scale.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3258 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_rules_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6344 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7409 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5611 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_projection.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4418 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_update_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6446 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoints_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4188 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_audit_sink_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5355 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_affinity.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4761 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_requirements.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6890 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_pod_security_policy_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4602 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_projected_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11179 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4805 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_http_ingress_path.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6451 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_eviction.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6454 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6674 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_template.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5452 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_user_info.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8747 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8117 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apiextensions_v1beta1_webhook_client_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7803 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_rules_review_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3734 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_host_alias.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6632 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6744 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_controller_revision_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3247 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_node_affinity.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3839 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_service_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3943 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_host_port_range.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5678 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_projection.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7326 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5250 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_lifecycle.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4242 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_pods_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3289 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_allowed_flex_volume.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7895 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6746 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_api_resource_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3198 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_scale_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4295 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_webhook.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6938 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9844 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8598 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7949 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_azure_disk_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6536 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4909 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_access_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7599 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_access_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    12523 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9550 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_object_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7898 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6326 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_node_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4395 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_fs_group_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6649 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_rolling_update_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8021 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_policy_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4324 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_update_strategy.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8282 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4428 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_local_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    31687 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6530 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7562 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3877 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_id_range.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3921 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_id_range.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6286 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    14126 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11269 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5242 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_object_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4801 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7233 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_job.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6611 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_external_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6276 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13991 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6977 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_validating_webhook_configuration.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6496 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_template_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4934 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_rolling_update_daemon_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5132 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6742 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8672 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_attributes.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    10236 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_probe.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6024 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8088 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6494 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_event_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6214 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6516 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6585 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_vsphere_virtual_disk_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6518 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_resource_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8670 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_ceph_fs_persistent_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7510 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_rules_review.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7733 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_condition.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4744 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_allowed_host_path.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7520 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3319 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_rollback_config.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4580 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_supplemental_groups_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8298 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state_terminated.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5177 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/admissionregistration_v1beta1_service_reference.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6163 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_scale_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6308 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6654 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7525 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8391 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4488 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_group_version_for_discovery.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5339 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_egress_rule.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5280 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_object_metric_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    28588 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_container.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7791 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8123 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6601 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_external_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     4636 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6622 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role_binding_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     8264 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_access_review_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6790 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_list.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3129 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_endpoint.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     5231 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_se_linux_options.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     9855 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     3275 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace_status.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     6028 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_resource_metric_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7093 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7158 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_volume_source.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    13178 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    11079 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_spec.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)     7611 2019-02-13 03:20:24.000000 kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler.py
--rw-r--r--   0 haoweic  (484802) eng       (5000)    24582 2019-02-13 03:20:38.000000 kubernetes-9.0.0b1/kubernetes/client/api_client.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     1056 2019-08-12 19:47:14.000000 kubernetes-9.0.1/PKG-INFO
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11354 2019-08-12 19:46:34.000000 kubernetes-9.0.1/LICENSE
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      333 2019-08-12 19:46:34.000000 kubernetes-9.0.1/requirements.txt
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    20417 2019-08-12 19:46:41.000000 kubernetes-9.0.1/CHANGELOG.md
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      148 2019-08-12 19:46:34.000000 kubernetes-9.0.1/code-of-conduct.md
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      175 2019-08-12 19:46:42.000000 kubernetes-9.0.1/test-requirements.txt
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      132 2019-08-12 19:46:34.000000 kubernetes-9.0.1/MANIFEST.in
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10206 2019-08-12 19:46:41.000000 kubernetes-9.0.1/README.md
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      523 2019-08-12 19:46:34.000000 kubernetes-9.0.1/RELEASE.md
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     2905 2019-08-12 19:46:42.000000 kubernetes-9.0.1/setup.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     1449 2019-08-12 19:46:41.000000 kubernetes-9.0.1/CONTRIBUTING.md
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     1062 2019-08-12 19:46:42.000000 kubernetes-9.0.1/tox.ini
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      130 2019-08-12 19:46:41.000000 kubernetes-9.0.1/OWNERS
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes.egg-info/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     1056 2019-08-12 19:47:13.000000 kubernetes-9.0.1/kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    34840 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      262 2019-08-12 19:47:13.000000 kubernetes-9.0.1/kubernetes.egg-info/requires.txt
+-rw-r--r--   0 haoweic  (484802) eng       (5000)       11 2019-08-12 19:47:13.000000 kubernetes-9.0.1/kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 haoweic  (484802) eng       (5000)        1 2019-08-12 19:47:13.000000 kubernetes-9.0.1/kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      159 2019-08-12 19:47:14.000000 kubernetes-9.0.1/setup.cfg
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/config/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    21694 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/config/kube_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     2226 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/config/dateutil_test.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3538 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/config/exec_provider.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      655 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/config/config_exception.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      830 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/config/__init__.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4997 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/config/exec_provider_test.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     2657 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/config/dateutil.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3546 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/config/incluster_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    40705 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/config/kube_config_test.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4747 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/config/incluster_config_test.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/stream/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      638 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/stream/__init__.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9412 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/stream/ws_client.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     1320 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/stream/stream.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     1452 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/stream/ws_client_test.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      812 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/__init__.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/utils/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      635 2019-08-12 19:46:42.000000 kubernetes-9.0.1/kubernetes/utils/__init__.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3180 2019-08-12 19:46:42.000000 kubernetes-9.0.1/kubernetes/utils/create_from_yaml.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/watch/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)      636 2019-08-12 19:46:35.000000 kubernetes-9.0.1/kubernetes/watch/__init__.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10181 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/watch/watch_test.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5162 2019-08-12 19:46:46.000000 kubernetes-9.0.1/kubernetes/watch/watch.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/client/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7833 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/configuration.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/client/apis/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4305 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/auditregistration_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4283 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/events_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4297 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/authorization_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4291 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/scheduling_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   482166 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apps_v1beta2_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   115535 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/admissionregistration_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4306 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    95120 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/autoscaling_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    27022 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/authorization_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4274 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/batch_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4301 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apiregistration_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4284 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/extensions_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   480916 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apps_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4287 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/settings_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4111 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/version_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   112086 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/storage_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7308 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/logs_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    57813 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/auditregistration_v1alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    91264 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/batch_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9647 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/authentication_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   251736 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_v1alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4286 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/autoscaling_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   127236 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/storage_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    95350 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/autoscaling_v2beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9607 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/authentication_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4297 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apiextensions_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    74892 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/coordination_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4313 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/admissionregistration_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    72863 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apiregistration_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)  1441124 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/core_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    26892 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/authorization_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   148870 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/policy_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4299 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/authentication_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3051 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/__init__.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    59409 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/admissionregistration_v1alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    92309 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/batch_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    58169 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/scheduling_v1alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4272 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apps_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    58447 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/storage_v1alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   161727 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/custom_objects_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    73073 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apiregistration_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   251622 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4295 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/certificates_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    75782 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/networking_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4296 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/core_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4300 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apis_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4295 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/coordination_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   251052 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_v1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    58141 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/scheduling_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   294885 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apps_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)   543396 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/extensions_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    81189 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/certificates_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    75311 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/apiextensions_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4285 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/storage_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    75450 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/settings_v1alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    74836 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/events_v1beta1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    95350 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/autoscaling_v2beta2_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    92355 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/batch_v2alpha1_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4291 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/networking_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4276 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/apis/policy_api.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13463 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/rest.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    43360 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/__init__.py
+drwxr-xr-x   0 haoweic  (484802) eng       (5000)        0 2019-08-12 19:47:14.000000 kubernetes-9.0.1/kubernetes/client/models/
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4213 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ip_block.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7643 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11757 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scale_io_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13806 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_storage_class.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7387 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_role_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4506 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_run_as_user_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7443 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7387 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3827 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_aggregation_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6265 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_account_token_projection.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4334 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_update_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6494 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_lease_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6693 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_rolling_update_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5086 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cross_version_object_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6708 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_env_var_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3268 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_service_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6476 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_binding_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12939 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_iscsi_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3812 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_event_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6862 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_downward_api_volume_file.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4296 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6922 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_service.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7613 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4367 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2alpha1_job_template_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8875 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/version_info.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7062 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_token_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4688 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_initializer.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8249 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_port.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4794 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_label_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8309 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_storage_os_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3543 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4356 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_job_template_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8038 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7633 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7412 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_flex_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13591 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_storage_class.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7678 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_subject_rules_review_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5547 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_user_info.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    35510 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3623 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_topology_selector_term.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7751 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7311 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_job_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4485 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_weighted_pod_affinity_term.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7413 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_controller_revision.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7033 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6170 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_service_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5564 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_glusterfs_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5550 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_selector_requirement.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6478 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3956 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_state_waiting.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6670 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6967 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_port.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5310 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3428 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_load_balancer_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3637 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_dns_config_option.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8096 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_owner_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    14181 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9609 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7901 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_webhook_client_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5993 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_endpoint_address.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10645 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_rbd_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3338 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_http_ingress_rule_value.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8597 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6790 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cinder_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7732 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_scale.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6070 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_projection.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3240 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_scale_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7456 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12340 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7892 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7961 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7782 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_affinity.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13917 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_job_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7078 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6939 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_mutating_webhook_configuration.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6119 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_subject.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8139 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_versions.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6398 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6660 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5249 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_nfs_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7110 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6855 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    39813 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6744 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_controller_revision_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4352 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7806 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_rollback.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3381 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_daemon_endpoints.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6405 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_http_get_action.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7787 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7532 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4244 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_topology_selector_label_requirement.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8664 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6604 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_pod_preset_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7892 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12340 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5565 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_group_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3375 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6710 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5593 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3901 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_address.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13018 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6920 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7245 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5476 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_value_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6690 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_namespace_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4397 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_selector_term.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3540 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_validation.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4348 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_update_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7207 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_token_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4612 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_se_linux_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6695 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7561 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7758 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3830 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_exec_action.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4575 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_run_as_group_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7962 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_rollback.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4296 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_flocker_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7436 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_affinity.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6690 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5057 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apiextensions_v1beta1_service_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7178 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5234 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_portworx_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4482 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_port.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6520 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_limit_range.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7558 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_scale.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6558 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_peer.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4436 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8198 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4700 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_allowed_host_path.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3135 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scale_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3286 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_limit_range_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9609 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3254 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_local_object_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3820 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_aggregation_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7110 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10624 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8088 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4125 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_device.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3484 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3780 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_non_resource_attributes.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    30353 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3013 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_preconditions.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5064 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_key_to_path.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4513 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scale_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6176 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_role_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12578 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_csi_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6571 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_list_meta.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6728 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_token_review_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7365 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_rules_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    14466 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4118 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_image.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6791 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_subject_access_review_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3409 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8038 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_metric_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11888 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_security_context.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6622 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6764 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7197 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_flex_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4649 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_server_address_by_client_cidr.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7338 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_lease_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    14236 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6375 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5399 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_env_var.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4969 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_rolling_update_daemon_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4796 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret_key_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4124 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_resource_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5515 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_status_cause.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3372 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3323 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_session_affinity_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4801 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_handler.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5565 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_taint.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8689 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_column_definition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    16482 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4562 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_run_as_user_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9975 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7404 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4248 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_external_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3778 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_http_header.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4327 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_preferred_scheduling_term.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7395 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6070 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6766 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3958 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7485 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_initializer_configuration.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12963 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_service_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7866 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_anti_affinity.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6660 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5593 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_dns_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6948 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4824 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_access_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6512 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role_binding_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6938 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_initializer_configuration_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8415 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_ceph_fs_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7091 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4162 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_resource_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6126 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5471 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_ingress_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6764 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9873 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    17131 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_event.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4789 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_state.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6564 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7617 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6302 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7612 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map_node_config_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5192 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_git_repo_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7744 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7454 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_access_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4286 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_external_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    27459 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_object_meta.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3526 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6073 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_scale_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7813 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_job_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6324 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_job_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6452 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_lease.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7762 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6764 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4264 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_update_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    22625 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3449 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3987 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_host_port_range.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6460 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4443 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_identifier.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7060 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_validating_webhook_configuration_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4568 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_se_linux_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6476 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8094 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_storage_os_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7370 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6733 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_pod_preset_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5369 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_label_selector_requirement.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3271 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_state_running.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    35941 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/__init__.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6722 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3318 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4991 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_field_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4957 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6769 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4059 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apiregistration_v1beta1_service_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7286 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_subject_access_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5918 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_pods_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7757 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6648 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3293 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_rules_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8827 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_resource_attributes.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7662 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6962 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_mount.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3471 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_namespace_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9310 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_priority_class.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7744 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6372 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_azure_file_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6769 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6166 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_role.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3277 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_rollback_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7425 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8291 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_names.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6758 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_account_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    14115 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4717 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_endpoint_port.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6309 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_target.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6350 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_event_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4600 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_non_resource_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4969 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_rolling_update_daemon_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8445 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_policy_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8747 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6610 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3519 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5254 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_egress_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7358 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_rule_with_operations.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4158 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_ip_block.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6702 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_limit_range_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7067 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4545 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_non_resource_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3750 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_sysctl.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9611 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8121 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_subject_access_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6552 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8398 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5843 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_pods_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9918 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_account.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11027 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6596 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_rolling_update_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4877 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_service_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13394 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_iscsi_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9039 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6112 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_pod_preset.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7377 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_aws_elastic_block_store_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11682 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_delete_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6654 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_service_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7538 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7613 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_local_subject_access_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10969 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_version.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7383 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3219 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_downward_api_projection.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7431 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_access_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6558 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12720 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_system_info.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4293 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_backend.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5118 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_azure_file_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10475 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3971 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_error.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7669 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_toleration.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6790 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4730 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_event_series.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4251 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10869 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_resource.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7591 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6816 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_pod_security_policy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10837 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_deployment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3973 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret_env_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10606 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_config_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7608 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_object_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5386 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_ingress_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4905 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_tls.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6694 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_priority_class_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5341 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_conversion.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4600 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4063 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_attached_volume.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6580 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6759 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_rolling_update_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13970 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_security_context.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3451 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/runtime_raw_extension.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    18454 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_event.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4233 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_watch_event.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    31227 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_pod_security_policy_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6356 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_audit_sink_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5202 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3317 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_allowed_flex_volume.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6212 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_audit_sink.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7528 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_controller_revision.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3835 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_non_resource_attributes.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6710 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7913 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3643 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_capabilities.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7283 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_endpoints.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3785 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_aggregation_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4451 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_fs_group_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8261 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/admissionregistration_v1beta1_webhook_client_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12250 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_webhook.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6644 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role_binding_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3287 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_config_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4155 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_subresources.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4240 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7527 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_object_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10548 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7178 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6448 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4615 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_downward_api_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6560 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4656 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_initializers.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7346 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_gce_persistent_disk_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5124 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_typed_local_object_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7322 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6695 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5747 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_component_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6545 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12130 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6663 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_fc_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5779 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8348 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_policy_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3178 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_initializer.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6634 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_controller_revision_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3170 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_scale_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7807 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4012 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map_env_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7758 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_local_subject_access_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7012 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_mutating_webhook_configuration_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6302 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4444 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_token_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10650 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6714 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_resource_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6978 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6298 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7453 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_namespace.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6323 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_subject.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5126 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_event_series.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3484 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scope_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6428 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5088 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_empty_dir_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5612 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scoped_resource_selector_requirement.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    29617 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_json_schema_props.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4499 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_token_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4039 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_policy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6192 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4026 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_error.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4010 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_webhook_throttle_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7528 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_controller_revision.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4375 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_photon_persistent_disk_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6344 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_role_binding_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5292 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4223 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_template_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7858 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_limit_range_item.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12282 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6648 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_storage_class_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6595 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4284 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_host_path_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4037 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_error.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7297 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scale.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6454 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_binding_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4366 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_update_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3450 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_readiness_gate.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6454 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6606 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_component_status_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6619 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6615 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cinder_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4733 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_ref.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7348 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4112 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4748 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_ref.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10310 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_rbd_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7209 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6648 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_peer.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6013 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_scale_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4219 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_port.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3414 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_rolling_update_stateful_set_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7802 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4030 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_tcp_socket_action.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    14466 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6558 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8123 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9830 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_group.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6803 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_quobyte_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6451 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7508 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_deployment_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5161 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_cross_version_object_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4519 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_run_as_group_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4226 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_deployment_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6838 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_token_review_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7452 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12170 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_scale_io_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6318 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_deployment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6280 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3789 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_external_documentation.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9283 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_priority_class.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7607 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_subresource_scale.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6728 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_pod_security_policy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11407 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8148 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_status_details.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4235 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_object_field_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4871 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_env_from_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8728 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7488 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role_binding.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6548 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6672 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_priority_class_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3589 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_client_ip_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6886 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_access_review_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7172 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_glusterfs_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7952 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4751 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map_key_selector.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4658 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_role_ref.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6538 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_storage_class_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5567 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_endpoint_subset.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4072 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_load_balancer_ingress.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7978 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replica_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5161 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_cross_version_object_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4204 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_pods_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7599 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5854 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_affinity_term.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6420 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6585 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_component_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7442 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_scale.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3258 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_rules_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6344 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7409 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5611 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret_projection.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4418 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_update_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6446 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_endpoints_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4188 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_audit_sink_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5355 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_affinity.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4761 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_requirements.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6890 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_pod_security_policy_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4602 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_projected_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11179 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4805 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_http_ingress_path.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6451 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_eviction.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6454 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6674 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_template.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5452 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_user_info.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8747 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8117 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apiextensions_v1beta1_webhook_client_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7803 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_rules_review_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3734 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_host_alias.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6632 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6744 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_controller_revision_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3247 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_volume_node_affinity.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3839 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_service_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3943 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_host_port_range.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5678 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map_projection.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7326 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5250 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_lifecycle.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4242 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_pods_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3289 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_allowed_flex_volume.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7895 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6746 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_api_resource_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3198 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_scale_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4295 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_webhook.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6938 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9844 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8598 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7949 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_azure_disk_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6536 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4909 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_access_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7599 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_access_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    12523 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9550 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_object_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7898 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6326 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_node_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4395 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_fs_group_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6649 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_rolling_update_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8021 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_policy_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4324 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_update_strategy.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8282 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_config_map.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4428 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_local_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    31687 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6530 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7562 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3877 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_id_range.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3921 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_id_range.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6286 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    14126 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11269 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5242 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_object_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4801 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7233 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_job.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6611 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_external_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6276 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_role.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13991 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6977 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_validating_webhook_configuration.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6496 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_template_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4934 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_rolling_update_daemon_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5132 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6742 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8672 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_attributes.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    10236 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_probe.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6024 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8088 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6494 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_event_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6214 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6516 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6585 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_vsphere_virtual_disk_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6518 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_resource_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8670 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_ceph_fs_persistent_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7510 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_rules_review.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7733 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_pod_condition.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4744 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_allowed_host_path.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7520 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3319 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_rollback_config.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4580 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_supplemental_groups_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8298 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container_state_terminated.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5177 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/admissionregistration_v1beta1_service_reference.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6163 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_scale_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6308 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6654 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7525 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8391 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4488 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_group_version_for_discovery.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5339 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_egress_rule.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5280 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta2_object_metric_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    28588 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_container.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7791 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8123 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6601 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_external_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     4636 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6622 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role_binding_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     8264 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_access_review_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6790 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_list.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3129 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_daemon_endpoint.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     5231 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_se_linux_options.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     9855 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     3275 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_namespace_status.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     6028 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v2beta1_resource_metric_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7093 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7158 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_secret_volume_source.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    13178 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    11079 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_deployment_spec.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)     7611 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler.py
+-rw-r--r--   0 haoweic  (484802) eng       (5000)    24580 2019-08-12 19:46:41.000000 kubernetes-9.0.1/kubernetes/client/api_client.py
```

### Comparing `kubernetes-9.0.0b1/PKG-INFO` & `kubernetes-9.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kubernetes
-Version: 9.0.0b1
+Version: 9.0.1
 Summary: Kubernetes python client
 Home-page: https://github.com/kubernetes-client/python
 Author: Kubernetes
 Author-email: 
 License: Apache License Version 2.0
 Description:     Python client for kubernetes http://kubernetes.io/
             
 Keywords: Swagger,OpenAPI,Kubernetes
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `kubernetes-9.0.0b1/LICENSE` & `kubernetes-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/CHANGELOG.md` & `kubernetes-9.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# v9.0.1
+**Security Fix:**
+- Bump urllib3 version to pick up security fix for CVE-2019-11324 [kubernetes-client/python#897](https://github.com/kubernetes-client/python/pull/897)
+
+**Bug Fix:**
+- Fix base64 padding for kube config [kubernetes-client/python-base#79](https://github.com/kubernetes-client/python-base/pull/79)
+
+# v9.0.0
+**Bug Fix:**
+- Add fieldSelector parameter to list/watch methods in custom objects spec [kubernetes-client/gen#106](https://github.com/kubernetes-client/gen/pull/106)
+
 # v9.0.0b1
 **Breaking Change:**
 - Move dependancy adal under extra require [kubernetes-client/python-base#108](https://github.com/kubernetes-client/python-base/pull/108)
 
 **Bug Fix:**
 - Honor the specified resource version in stream request when watch restarts [kubernetes-client/python-base#109](https://github.com/kubernetes-client/python-base/pull/109)
```

### Comparing `kubernetes-9.0.0b1/README.md` & `kubernetes-9.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -117,20 +117,21 @@
 | 3.0 Alpha/Beta | Kubernetes main repo, 1.7 branch     | ✗                             |
 | 3.0            | Kubernetes main repo, 1.7 branch     | ✗                             |
 | 4.0 Alpha/Beta | Kubernetes main repo, 1.8 branch     | ✗                             |
 | 4.0            | Kubernetes main repo, 1.8 branch     | ✗                             |
 | 5.0 Alpha/Beta | Kubernetes main repo, 1.9 branch     | ✗                             |
 | 5.0            | Kubernetes main repo, 1.9 branch     | ✗                             |
 | 6.0 Alpha/Beta | Kubernetes main repo, 1.10 branch    | ✗                             |
-| 6.0            | Kubernetes main repo, 1.10 branch    | ✓                             |
+| 6.0            | Kubernetes main repo, 1.10 branch    | ✗                             |
 | 7.0 Alpha/Beta | Kubernetes main repo, 1.11 branch    | ✗                             |
 | 7.0            | Kubernetes main repo, 1.11 branch    | ✓                             |
 | 8.0 Alpha/Beta | Kubernetes main repo, 1.12 branch    | ✗                             |
 | 8.0            | Kubernetes main repo, 1.12 branch    | ✓                             |
-| 9.0 Alpha/Beta | Kubernetes main repo, 1.13 branch    | ✓                             |
+| 9.0 Alpha/Beta | Kubernetes main repo, 1.13 branch    | ✗                             |
+| 9.0            | Kubernetes main repo, 1.13 branch    | ✓                             |
 
 
 Key:
 
 * `✓` Changes in main Kubernetes repo are manually ([should be automated](https://github.com/kubernetes-client/python/issues/177)) published to client-python when they are available.
 * `✗` No longer maintained; please upgrade.
```

### Comparing `kubernetes-9.0.0b1/RELEASE.md` & `kubernetes-9.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/setup.py` & `kubernetes-9.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup
 
 # Do not edit these constants. They will be updated automatically
 # by scripts/update-client.sh.
-CLIENT_VERSION = "9.0.0b1"
+CLIENT_VERSION = "9.0.1"
 PACKAGE_NAME = "kubernetes"
-DEVELOPMENT_STATUS = "4 - Beta"
+DEVELOPMENT_STATUS = "5 - Production/Stable"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kubernetes-9.0.0b1/CONTRIBUTING.md` & `kubernetes-9.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/tox.ini` & `kubernetes-9.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes.egg-info/PKG-INFO` & `kubernetes-9.0.1/kubernetes.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kubernetes
-Version: 9.0.0b1
+Version: 9.0.1
 Summary: Kubernetes python client
 Home-page: https://github.com/kubernetes-client/python
 Author: Kubernetes
 Author-email: 
 License: Apache License Version 2.0
 Description:     Python client for kubernetes http://kubernetes.io/
             
 Keywords: Swagger,OpenAPI,Kubernetes
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
```

### Comparing `kubernetes-9.0.0b1/kubernetes.egg-info/SOURCES.txt` & `kubernetes-9.0.1/kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/kube_config.py` & `kubernetes-9.0.1/kubernetes/config/kube_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,26 +264,39 @@
         if self._config_persister:
             self._config_persister(self._config.value)
 
     def _load_oid_token(self, provider):
         if 'config' not in provider:
             return
 
-        parts = provider['config']['id-token'].split('.')
+        reserved_characters = frozenset(["=", "+", "/"])
+        token = provider['config']['id-token']
 
+        if any(char in token for char in reserved_characters):
+            # Invalid jwt, as it contains url-unsafe chars
+            return
+
+        parts = token.split('.')
         if len(parts) != 3:  # Not a valid JWT
-            return None
+            return
+
+        padding = (4 - len(parts[1]) % 4) * '='
+        if len(padding) == 3:
+            # According to spec, 3 padding characters cannot occur
+            # in a valid jwt
+            # https://tools.ietf.org/html/rfc7515#appendix-C
+            return
 
         if PY3:
             jwt_attributes = json.loads(
-                base64.b64decode(parts[1]).decode('utf-8')
+                base64.b64decode(parts[1] + padding).decode('utf-8')
             )
         else:
             jwt_attributes = json.loads(
-                base64.b64decode(parts[1] + "==")
+                base64.b64decode(parts[1] + padding)
             )
 
         expire = jwt_attributes.get('exp')
 
         if ((expire is not None) and
             (_is_expired(datetime.datetime.fromtimestamp(expire,
                                                          tz=UTC)))):
```

### Comparing `kubernetes-9.0.0b1/kubernetes/config/dateutil_test.py` & `kubernetes-9.0.1/kubernetes/config/dateutil_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/exec_provider.py` & `kubernetes-9.0.1/kubernetes/config/exec_provider.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/config_exception.py` & `kubernetes-9.0.1/kubernetes/config/config_exception.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/__init__.py` & `kubernetes-9.0.1/kubernetes/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/exec_provider_test.py` & `kubernetes-9.0.1/kubernetes/config/exec_provider_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/dateutil.py` & `kubernetes-9.0.1/kubernetes/config/dateutil.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/incluster_config.py` & `kubernetes-9.0.1/kubernetes/config/incluster_config.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/config/kube_config_test.py` & `kubernetes-9.0.1/kubernetes/config/kube_config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 NON_EXISTING_FILE = "zz_non_existing_file_472398324"
 
 
 def _base64(string):
     return base64.standard_b64encode(string.encode()).decode()
 
 
+def _urlsafe_unpadded_b64encode(string):
+    return base64.urlsafe_b64encode(string.encode()).decode().rstrip('=')
+
+
 def _format_expiry_datetime(dt):
     return dt.strftime(EXPIRY_DATETIME_FORMAT)
 
 
 def _get_expiry(loader, active_context):
     expired_gcp_conf = (item for item in loader._config.value.get("users")
                         if item.get("name") == active_context)
@@ -92,20 +96,41 @@
 TEST_CLIENT_KEY_BASE64 = _base64(TEST_CLIENT_KEY)
 TEST_CLIENT_CERT = "client-cert"
 TEST_CLIENT_CERT_BASE64 = _base64(TEST_CLIENT_CERT)
 
 
 TEST_OIDC_TOKEN = "test-oidc-token"
 TEST_OIDC_INFO = "{\"name\": \"test\"}"
-TEST_OIDC_BASE = _base64(TEST_OIDC_TOKEN) + "." + _base64(TEST_OIDC_INFO)
-TEST_OIDC_LOGIN = TEST_OIDC_BASE + "." + TEST_CLIENT_CERT_BASE64
+TEST_OIDC_BASE = ".".join([
+    _urlsafe_unpadded_b64encode(TEST_OIDC_TOKEN),
+    _urlsafe_unpadded_b64encode(TEST_OIDC_INFO)
+])
+TEST_OIDC_LOGIN = ".".join([
+    TEST_OIDC_BASE,
+    _urlsafe_unpadded_b64encode(TEST_CLIENT_CERT_BASE64)
+])
 TEST_OIDC_TOKEN = "Bearer %s" % TEST_OIDC_LOGIN
 TEST_OIDC_EXP = "{\"name\": \"test\",\"exp\": 536457600}"
-TEST_OIDC_EXP_BASE = _base64(TEST_OIDC_TOKEN) + "." + _base64(TEST_OIDC_EXP)
-TEST_OIDC_EXPIRED_LOGIN = TEST_OIDC_EXP_BASE + "." + TEST_CLIENT_CERT_BASE64
+TEST_OIDC_EXP_BASE = _urlsafe_unpadded_b64encode(
+    TEST_OIDC_TOKEN) + "." + _urlsafe_unpadded_b64encode(TEST_OIDC_EXP)
+TEST_OIDC_EXPIRED_LOGIN = ".".join([
+    TEST_OIDC_EXP_BASE,
+    _urlsafe_unpadded_b64encode(TEST_CLIENT_CERT)
+])
+TEST_OIDC_CONTAINS_RESERVED_CHARACTERS = ".".join([
+    _urlsafe_unpadded_b64encode(TEST_OIDC_TOKEN),
+    _urlsafe_unpadded_b64encode(TEST_OIDC_INFO).replace("a", "+"),
+    _urlsafe_unpadded_b64encode(TEST_CLIENT_CERT)
+])
+TEST_OIDC_INVALID_PADDING_LENGTH = ".".join([
+    _urlsafe_unpadded_b64encode(TEST_OIDC_TOKEN),
+    "aaaaa",
+    _urlsafe_unpadded_b64encode(TEST_CLIENT_CERT)
+])
+
 TEST_OIDC_CA = _base64(TEST_CERTIFICATE_AUTH)
 
 
 class BaseTestCase(unittest.TestCase):
 
     def setUp(self):
         self._temp_files = []
@@ -405,14 +430,30 @@
                 "name": "expired_oidc_nocert",
                 "context": {
                     "cluster": "default",
                     "user": "expired_oidc_nocert"
                 }
             },
             {
+                "name": "oidc_contains_reserved_character",
+                "context": {
+                    "cluster": "default",
+                    "user": "oidc_contains_reserved_character"
+
+                }
+            },
+            {
+                "name": "oidc_invalid_padding_length",
+                "context": {
+                    "cluster": "default",
+                    "user": "oidc_invalid_padding_length"
+
+                }
+            },
+            {
                 "name": "user_pass",
                 "context": {
                     "cluster": "default",
                     "user": "user_pass"
                 }
             },
             {
@@ -591,14 +632,46 @@
                             "refresh-token":
                                 "lucWJjEhlxZW01cXI3YmVlcYnpxNGhzk"
                         }
                     }
                 }
             },
             {
+                "name": "oidc_contains_reserved_character",
+                "user": {
+                    "auth-provider": {
+                        "name": "oidc",
+                        "config": {
+                            "client-id": "tectonic-kubectl",
+                            "client-secret": "FAKE_SECRET",
+                            "id-token": TEST_OIDC_CONTAINS_RESERVED_CHARACTERS,
+                            "idp-issuer-url": "https://example.org/identity",
+                            "refresh-token":
+                                "lucWJjEhlxZW01cXI3YmVlcYnpxNGhzk"
+                        }
+                    }
+                }
+            },
+            {
+                "name": "oidc_invalid_padding_length",
+                "user": {
+                    "auth-provider": {
+                        "name": "oidc",
+                        "config": {
+                            "client-id": "tectonic-kubectl",
+                            "client-secret": "FAKE_SECRET",
+                            "id-token": TEST_OIDC_INVALID_PADDING_LENGTH,
+                            "idp-issuer-url": "https://example.org/identity",
+                            "refresh-token":
+                                "lucWJjEhlxZW01cXI3YmVlcYnpxNGhzk"
+                        }
+                    }
+                }
+            },
+            {
                 "name": "user_pass",
                 "user": {
                     "username": TEST_USERNAME,  # should be ignored
                     "password": TEST_PASSWORD,  # should be ignored
                 }
             },
             {
@@ -788,14 +861,34 @@
         loader = KubeConfigLoader(
             config_dict=self.TEST_KUBE_CONFIG,
             active_context="expired_oidc_nocert",
         )
         self.assertTrue(loader._load_auth_provider_token())
         self.assertEqual("Bearer abc123", loader.token)
 
+    def test_oidc_fails_if_contains_reserved_chars(self):
+        loader = KubeConfigLoader(
+            config_dict=self.TEST_KUBE_CONFIG,
+            active_context="oidc_contains_reserved_character",
+        )
+        self.assertEqual(
+            loader._load_oid_token("oidc_contains_reserved_character"),
+            None,
+        )
+
+    def test_oidc_fails_if_invalid_padding_length(self):
+        loader = KubeConfigLoader(
+            config_dict=self.TEST_KUBE_CONFIG,
+            active_context="oidc_invalid_padding_length",
+        )
+        self.assertEqual(
+            loader._load_oid_token("oidc_invalid_padding_length"),
+            None,
+        )
+
     def test_user_pass(self):
         expected = FakeConfig(host=TEST_HOST, token=TEST_BASIC_TOKEN)
         actual = FakeConfig()
         KubeConfigLoader(
             config_dict=self.TEST_KUBE_CONFIG,
             active_context="user_pass").load_and_set(actual)
         self.assertEqual(expected, actual)
```

### Comparing `kubernetes-9.0.0b1/kubernetes/config/incluster_config_test.py` & `kubernetes-9.0.1/kubernetes/config/incluster_config_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/stream/__init__.py` & `kubernetes-9.0.1/kubernetes/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/stream/ws_client.py` & `kubernetes-9.0.1/kubernetes/stream/ws_client.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/stream/stream.py` & `kubernetes-9.0.1/kubernetes/stream/stream.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/stream/ws_client_test.py` & `kubernetes-9.0.1/kubernetes/stream/ws_client_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/__init__.py` & `kubernetes-9.0.1/kubernetes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __project__ = 'kubernetes'
 # The version is auto-updated. Please do not edit.
-__version__ = "9.0.0b1"
+__version__ = "9.0.1"
 
 import kubernetes.client
 import kubernetes.config
 import kubernetes.watch
 import kubernetes.stream
 import kubernetes.utils
```

### Comparing `kubernetes-9.0.0b1/kubernetes/utils/__init__.py` & `kubernetes-9.0.1/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/utils/create_from_yaml.py` & `kubernetes-9.0.1/kubernetes/utils/create_from_yaml.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/watch/__init__.py` & `kubernetes-9.0.1/kubernetes/watch/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/watch/watch_test.py` & `kubernetes-9.0.1/kubernetes/watch/watch_test.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/watch/watch.py` & `kubernetes-9.0.1/kubernetes/watch/watch.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/client/configuration.py` & `kubernetes-9.0.1/kubernetes/client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -235,10 +235,10 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: v1.13.4\n"\
-               "SDK Package Version: 9.0.0b1".\
+               "Version of the API: v1.13.9\n"\
+               "SDK Package Version: 9.0.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/auditregistration_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/auditregistration_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/events_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/events_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/authorization_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/authorization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/scheduling_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/scheduling_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apps_v1beta2_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apps_v1beta2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/admissionregistration_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/admissionregistration_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/autoscaling_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/authorization_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/authorization_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/batch_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/batch_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apiregistration_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apiregistration_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/extensions_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apiextensions_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -19,15 +19,15 @@
 
 # python 2 and python 3 compatibility library
 from six import iteritems
 
 from ..api_client import ApiClient
 
 
-class ExtensionsApi(object):
+class ApiextensionsApi(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
@@ -104,15 +104,15 @@
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.\
             select_header_content_type(['application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf'])
 
         # Authentication setting
         auth_settings = ['BearerToken']
 
-        return self.api_client.call_api('/apis/extensions/', 'GET',
+        return self.api_client.call_api('/apis/apiextensions.k8s.io/', 'GET',
                                         path_params,
                                         query_params,
                                         header_params,
                                         body=body_params,
                                         post_params=form_params,
                                         files=local_var_files,
                                         response_type='V1APIGroup',
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apps_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apps_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/settings_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/settings_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/version_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/version_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/storage_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/storage_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/logs_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/logs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/auditregistration_v1alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/auditregistration_v1alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/batch_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/batch_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/authentication_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/authentication_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_v1alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_v1alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/autoscaling_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/storage_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/storage_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_v2beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/autoscaling_v2beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/authentication_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/authentication_v1_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apiextensions_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/certificates_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -19,15 +19,15 @@
 
 # python 2 and python 3 compatibility library
 from six import iteritems
 
 from ..api_client import ApiClient
 
 
-class ApiextensionsApi(object):
+class CertificatesApi(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
@@ -104,15 +104,15 @@
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.\
             select_header_content_type(['application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf'])
 
         # Authentication setting
         auth_settings = ['BearerToken']
 
-        return self.api_client.call_api('/apis/apiextensions.k8s.io/', 'GET',
+        return self.api_client.call_api('/apis/certificates.k8s.io/', 'GET',
                                         path_params,
                                         query_params,
                                         header_params,
                                         body=body_params,
                                         post_params=form_params,
                                         files=local_var_files,
                                         response_type='V1APIGroup',
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/coordination_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/coordination_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/admissionregistration_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/admissionregistration_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apiregistration_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apiregistration_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/core_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/core_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/authorization_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/authorization_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/policy_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/policy_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/authentication_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/authentication_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/__init__.py` & `kubernetes-9.0.1/kubernetes/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/admissionregistration_v1alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/admissionregistration_v1alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/batch_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/batch_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/scheduling_v1alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/scheduling_v1alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apps_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apps_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/storage_v1alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/storage_v1alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/custom_objects_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/custom_objects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -1287,14 +1287,15 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str group: The custom resource's group name (required)
         :param str version: The custom resource's version (required)
         :param str plural: The custom resource's plural name. For TPRs this would be lowercase plural kind. (required)
         :param str pretty: If 'true', then the output is pretty printed.
+        :param str field_selector: A selector to restrict the list of returned objects by their fields. Defaults to everything.
         :param str label_selector: A selector to restrict the list of returned objects by their labels. Defaults to everything.
         :param str resource_version: When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it's 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv.
         :param int timeout_seconds: Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity.
         :param bool watch: Watch for changes to the described resources and return them as a stream of add, update, and remove notifications.
         :return: object
                  If the method is called asynchronously,
                  returns the request thread.
@@ -1315,24 +1316,25 @@
         >>> result = thread.get()
 
         :param async_req bool
         :param str group: The custom resource's group name (required)
         :param str version: The custom resource's version (required)
         :param str plural: The custom resource's plural name. For TPRs this would be lowercase plural kind. (required)
         :param str pretty: If 'true', then the output is pretty printed.
+        :param str field_selector: A selector to restrict the list of returned objects by their fields. Defaults to everything.
         :param str label_selector: A selector to restrict the list of returned objects by their labels. Defaults to everything.
         :param str resource_version: When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it's 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv.
         :param int timeout_seconds: Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity.
         :param bool watch: Watch for changes to the described resources and return them as a stream of add, update, and remove notifications.
         :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['group', 'version', 'plural', 'pretty', 'label_selector', 'resource_version', 'timeout_seconds', 'watch']
+        all_params = ['group', 'version', 'plural', 'pretty', 'field_selector', 'label_selector', 'resource_version', 'timeout_seconds', 'watch']
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -1363,14 +1365,16 @@
             path_params['version'] = params['version']
         if 'plural' in params:
             path_params['plural'] = params['plural']
 
         query_params = []
         if 'pretty' in params:
             query_params.append(('pretty', params['pretty']))
+        if 'field_selector' in params:
+            query_params.append(('fieldSelector', params['field_selector']))
         if 'label_selector' in params:
             query_params.append(('labelSelector', params['label_selector']))
         if 'resource_version' in params:
             query_params.append(('resourceVersion', params['resource_version']))
         if 'timeout_seconds' in params:
             query_params.append(('timeoutSeconds', params['timeout_seconds']))
         if 'watch' in params:
@@ -1418,14 +1422,15 @@
 
         :param async_req bool
         :param str group: The custom resource's group name (required)
         :param str version: The custom resource's version (required)
         :param str namespace: The custom resource's namespace (required)
         :param str plural: The custom resource's plural name. For TPRs this would be lowercase plural kind. (required)
         :param str pretty: If 'true', then the output is pretty printed.
+        :param str field_selector: A selector to restrict the list of returned objects by their fields. Defaults to everything.
         :param str label_selector: A selector to restrict the list of returned objects by their labels. Defaults to everything.
         :param str resource_version: When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it's 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv.
         :param int timeout_seconds: Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity.
         :param bool watch: Watch for changes to the described resources and return them as a stream of add, update, and remove notifications.
         :return: object
                  If the method is called asynchronously,
                  returns the request thread.
@@ -1447,24 +1452,25 @@
 
         :param async_req bool
         :param str group: The custom resource's group name (required)
         :param str version: The custom resource's version (required)
         :param str namespace: The custom resource's namespace (required)
         :param str plural: The custom resource's plural name. For TPRs this would be lowercase plural kind. (required)
         :param str pretty: If 'true', then the output is pretty printed.
+        :param str field_selector: A selector to restrict the list of returned objects by their fields. Defaults to everything.
         :param str label_selector: A selector to restrict the list of returned objects by their labels. Defaults to everything.
         :param str resource_version: When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. When specified for list: - if unset, then the result is returned from remote storage based on quorum-read flag; - if it's 0, then we simply return what we currently have in cache, no guarantee; - if set to non zero, then the result is at least as fresh as given rv.
         :param int timeout_seconds: Timeout for the list/watch call. This limits the duration of the call, regardless of any activity or inactivity.
         :param bool watch: Watch for changes to the described resources and return them as a stream of add, update, and remove notifications.
         :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['group', 'version', 'namespace', 'plural', 'pretty', 'label_selector', 'resource_version', 'timeout_seconds', 'watch']
+        all_params = ['group', 'version', 'namespace', 'plural', 'pretty', 'field_selector', 'label_selector', 'resource_version', 'timeout_seconds', 'watch']
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -1500,14 +1506,16 @@
             path_params['namespace'] = params['namespace']
         if 'plural' in params:
             path_params['plural'] = params['plural']
 
         query_params = []
         if 'pretty' in params:
             query_params.append(('pretty', params['pretty']))
+        if 'field_selector' in params:
+            query_params.append(('fieldSelector', params['field_selector']))
         if 'label_selector' in params:
             query_params.append(('labelSelector', params['label_selector']))
         if 'resource_version' in params:
             query_params.append(('resourceVersion', params['resource_version']))
         if 'timeout_seconds' in params:
             query_params.append(('timeoutSeconds', params['timeout_seconds']))
         if 'watch' in params:
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apiregistration_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apiregistration_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/certificates_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/policy_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -19,15 +19,15 @@
 
 # python 2 and python 3 compatibility library
 from six import iteritems
 
 from ..api_client import ApiClient
 
 
-class CertificatesApi(object):
+class PolicyApi(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
@@ -104,15 +104,15 @@
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.\
             select_header_content_type(['application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf'])
 
         # Authentication setting
         auth_settings = ['BearerToken']
 
-        return self.api_client.call_api('/apis/certificates.k8s.io/', 'GET',
+        return self.api_client.call_api('/apis/policy/', 'GET',
                                         path_params,
                                         query_params,
                                         header_params,
                                         body=body_params,
                                         post_params=form_params,
                                         files=local_var_files,
                                         response_type='V1APIGroup',
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/networking_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/networking_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/core_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/core_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apis_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apis_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/coordination_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/coordination_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/rbac_authorization_v1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/rbac_authorization_v1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/scheduling_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/scheduling_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apps_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apps_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/extensions_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/extensions_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/certificates_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/certificates_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/apiextensions_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/apiextensions_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/storage_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/storage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/settings_v1alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/settings_v1alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/events_v1beta1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/events_v1beta1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/autoscaling_v2beta2_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/autoscaling_v2beta2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/batch_v2alpha1_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/batch_v2alpha1_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/networking_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/extensions_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -19,15 +19,15 @@
 
 # python 2 and python 3 compatibility library
 from six import iteritems
 
 from ..api_client import ApiClient
 
 
-class NetworkingApi(object):
+class ExtensionsApi(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
@@ -104,15 +104,15 @@
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.\
             select_header_content_type(['application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf'])
 
         # Authentication setting
         auth_settings = ['BearerToken']
 
-        return self.api_client.call_api('/apis/networking.k8s.io/', 'GET',
+        return self.api_client.call_api('/apis/extensions/', 'GET',
                                         path_params,
                                         query_params,
                                         header_params,
                                         body=body_params,
                                         post_params=form_params,
                                         files=local_var_files,
                                         response_type='V1APIGroup',
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/apis/policy_api.py` & `kubernetes-9.0.1/kubernetes/client/apis/networking_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -19,15 +19,15 @@
 
 # python 2 and python 3 compatibility library
 from six import iteritems
 
 from ..api_client import ApiClient
 
 
-class PolicyApi(object):
+class NetworkingApi(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
@@ -104,15 +104,15 @@
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.\
             select_header_content_type(['application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf'])
 
         # Authentication setting
         auth_settings = ['BearerToken']
 
-        return self.api_client.call_api('/apis/policy/', 'GET',
+        return self.api_client.call_api('/apis/networking.k8s.io/', 'GET',
                                         path_params,
                                         query_params,
                                         header_params,
                                         body=body_params,
                                         post_params=form_params,
                                         files=local_var_files,
                                         response_type='V1APIGroup',
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/rest.py` & `kubernetes-9.0.1/kubernetes/client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/__init__.py` & `kubernetes-9.0.1/kubernetes/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ip_block.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ip_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_io_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scale_io_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_storage_class.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_storage_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_role_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_role_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_run_as_user_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_run_as_user_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_aggregation_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_aggregation_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_account_token_projection.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_account_token_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_update_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_update_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_lease_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_lease_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_rolling_update_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_rolling_update_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cross_version_object_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cross_version_object_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_env_var_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_env_var_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_service_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_binding_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_binding_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_iscsi_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_iscsi_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_event_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_event_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_downward_api_volume_file.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_downward_api_volume_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_job_template_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v2alpha1_job_template_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/version_info.py` & `kubernetes-9.0.1/kubernetes/client/models/version_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_token_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_token_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_initializer.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_initializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_port.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_label_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_label_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_os_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_storage_os_persistent_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_job_template_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_job_template_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_flex_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_flex_persistent_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_class.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_storage_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_rules_review_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_subject_rules_review_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_user_info.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_user_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_topology_selector_term.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_topology_selector_term.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_job_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_job_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_weighted_pod_affinity_term.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_weighted_pod_affinity_term.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_controller_revision.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_controller_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_service_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_glusterfs_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_glusterfs_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_selector_requirement.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_selector_requirement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state_waiting.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_state_waiting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_port.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_load_balancer_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_load_balancer_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_dns_config_option.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_dns_config_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_owner_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_owner_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_webhook_client_config.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_webhook_client_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoint_address.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_endpoint_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_rbd_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_rbd_persistent_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_http_ingress_rule_value.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_http_ingress_rule_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cinder_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cinder_persistent_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_scale.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_projection.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_scale_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_scale_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_affinity.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_affinity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_job_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_mutating_webhook_configuration.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_mutating_webhook_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_subject.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_versions.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_nfs_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_nfs_volume_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
@@ -333,26 +333,26 @@
 
         self._dns_policy = dns_policy
 
     @property
     def enable_service_links(self):
         """
         Gets the enable_service_links of this V1PodSpec.
-        EnableServiceLinks indicates whether information about services should be injected into pod's environment variables, matching the syntax of Docker links.
+        EnableServiceLinks indicates whether information about services should be injected into pod's environment variables, matching the syntax of Docker links. Optional: Defaults to true.
 
         :return: The enable_service_links of this V1PodSpec.
         :rtype: bool
         """
         return self._enable_service_links
 
     @enable_service_links.setter
     def enable_service_links(self, enable_service_links):
         """
         Sets the enable_service_links of this V1PodSpec.
-        EnableServiceLinks indicates whether information about services should be injected into pod's environment variables, matching the syntax of Docker links.
+        EnableServiceLinks indicates whether information about services should be injected into pod's environment variables, matching the syntax of Docker links. Optional: Defaults to true.
 
         :param enable_service_links: The enable_service_links of this V1PodSpec.
         :type: bool
         """
 
         self._enable_service_links = enable_service_links
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_controller_revision_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_controller_revision_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_rollback.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_rollback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_daemon_endpoints.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_daemon_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_http_get_action.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_http_get_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_topology_selector_label_requirement.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_topology_selector_label_requirement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_pod_preset_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_pod_preset_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_group_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_group_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_address.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_value_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_value_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_namespace_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_selector_term.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_selector_term.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_validation.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_update_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_update_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_token_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_token_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_se_linux_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_se_linux_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_exec_action.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_exec_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_run_as_group_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_run_as_group_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_rollback.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_rollback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_flocker_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_flocker_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_affinity.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_affinity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apiextensions_v1beta1_service_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/apiextensions_v1beta1_service_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_portworx_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_portworx_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_port.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_limit_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_scale.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_peer.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_peer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_allowed_host_path.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_allowed_host_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scale_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_limit_range_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_local_object_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_local_object_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_aggregation_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_aggregation_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_device.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_non_resource_attributes.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_non_resource_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_preconditions.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_preconditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_key_to_path.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_key_to_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scale_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_role_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_csi_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_csi_persistent_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_list_meta.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_list_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_token_review_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_token_review_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_rules_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_rules_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_image.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_access_review_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_subject_access_review_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_rolling_update_stateful_set_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_rolling_update_stateful_set_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_metric_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_metric_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_security_context.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_security_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_flex_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_flex_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_server_address_by_client_cidr.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_server_address_by_client_cidr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_lease_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_lease_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_env_var.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_env_var.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_rolling_update_daemon_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_rolling_update_daemon_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_key_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret_key_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_resource_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_resource_metric_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_status_cause.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_status_cause.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_session_affinity_config.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_session_affinity_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_handler.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_taint.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_taint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_column_definition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_column_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_run_as_user_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_run_as_user_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_external_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_external_metric_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_http_header.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_http_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_preferred_scheduling_term.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_preferred_scheduling_term.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_initializer_configuration.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_initializer_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_service_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_anti_affinity.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_anti_affinity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_dns_config.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_dns_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_access_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_access_review_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role_binding_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role_binding_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_initializer_configuration_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_initializer_configuration_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_ceph_fs_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_ceph_fs_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_resource_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_resource_metric_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_ingress_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_ingress_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_event.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_node_config_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map_node_config_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_git_repo_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_git_repo_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_access_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_access_review.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_external_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_external_metric_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_object_meta.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_object_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_scale_status.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_scale_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_job_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_job_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_lease.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_lease.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_update_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_update_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_rolling_update_stateful_set_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_rolling_update_stateful_set_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_host_port_range.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_host_port_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_identifier.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_validating_webhook_configuration_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_validating_webhook_configuration_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_se_linux_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_se_linux_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_os_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_storage_os_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_pod_preset_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_pod_preset_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_label_selector_requirement.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_label_selector_requirement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state_running.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_state_running.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/__init__.py` & `kubernetes-9.0.1/kubernetes/client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_field_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_field_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apiregistration_v1beta1_service_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/apiregistration_v1beta1_service_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_access_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_subject_access_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_pods_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_pods_metric_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_rules_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_rules_review_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_resource_attributes.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_resource_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_mount.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_namespace_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_priority_class.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_priority_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_azure_file_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_azure_file_persistent_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_role.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_rollback_config.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_rollback_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_names.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_account_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_account_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoint_port.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_endpoint_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_metric_target.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_metric_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_event_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_event_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_non_resource_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_non_resource_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_rolling_update_daemon_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_rolling_update_daemon_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_policy_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_policy_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_egress_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_egress_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_rule_with_operations.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_rule_with_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_ip_block.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_ip_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_limit_range_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_non_resource_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_non_resource_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_sysctl.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_sysctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_subject_access_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_subject_access_review_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_pods_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_pods_metric_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_account.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_rolling_update_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_rolling_update_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_service_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_service_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_iscsi_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_iscsi_persistent_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_pod_preset.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_pod_preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_aws_elastic_block_store_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_aws_elastic_block_store_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_delete_options.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_delete_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_service_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_service_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_local_subject_access_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_local_subject_access_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_definition_version.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_definition_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_downward_api_projection.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_downward_api_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_access_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_access_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_system_info.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_backend.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_azure_file_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_azure_file_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_error.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_toleration.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_toleration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_event_series.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_event_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_resource.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2alpha1_cron_job.py` & `kubernetes-9.0.1/kubernetes/client/models/v2alpha1_cron_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_pod_security_policy.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_pod_security_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_deployment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_env_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret_env_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_config_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_config_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_object_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_object_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_ingress_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_ingress_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_tls.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_tls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_priority_class_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_priority_class_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_conversion.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_attached_volume.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_attached_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_rolling_update_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_rolling_update_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_security_context.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_security_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/runtime_raw_extension.py` & `kubernetes-9.0.1/kubernetes/client/models/runtime_raw_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_event.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_watch_event.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_watch_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_pod_security_policy_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_pod_security_policy_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_audit_sink_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_audit_sink_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_allowed_flex_volume.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_allowed_flex_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_audit_sink.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_audit_sink.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_controller_revision.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_controller_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_non_resource_attributes.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_non_resource_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_capabilities.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_capabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoints.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_aggregation_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_aggregation_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_fs_group_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_fs_group_strategy_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/admissionregistration_v1beta1_webhook_client_config.py` & `kubernetes-9.0.1/kubernetes/client/models/admissionregistration_v1beta1_webhook_client_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_webhook.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_cluster_role_binding_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_cluster_role_binding_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_config_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_config_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_subresources.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_subresources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_object_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_object_metric_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_downward_api_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_downward_api_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_initializers.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_gce_persistent_disk_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_gce_persistent_disk_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_typed_local_object_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_typed_local_object_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_pod_disruption_budget.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_pod_disruption_budget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_component_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_component_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_fc_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_fc_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_policy_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_policy_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_initializer.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_initializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_controller_revision_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_controller_revision_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_scale_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_scale_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_env_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map_env_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_local_subject_access_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_local_subject_access_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_mutating_webhook_configuration_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_mutating_webhook_configuration_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_token_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_token_review_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_resource_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_resource_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_list.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_subject.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_event_series.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_event_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scope_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scope_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_empty_dir_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_empty_dir_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scoped_resource_selector_requirement.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scoped_resource_selector_requirement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_json_schema_props.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_json_schema_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_token_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_token_review_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_policy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_error.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_webhook_throttle_config.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_webhook_throttle_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_controller_revision.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_controller_revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_photon_persistent_disk_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_photon_persistent_disk_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_role_binding_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_role_binding_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_template_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_template_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_limit_range_item.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_limit_range_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_storage_class_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_storage_class_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_host_path_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_host_path_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_error.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scale.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_binding_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_binding_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_update_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_update_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_readiness_gate.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_readiness_gate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_component_status_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_component_status_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cinder_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cinder_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_ref.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_ref.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_rbd_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_rbd_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_peer.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_peer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_scale_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_scale_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_port.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_port.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_rolling_update_stateful_set_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_rolling_update_stateful_set_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_tcp_socket_action.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_tcp_socket_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_replica_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_replica_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_group.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_quobyte_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_quobyte_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_deployment_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_cross_version_object_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_cross_version_object_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_run_as_group_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_run_as_group_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_deployment_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_token_review_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_token_review_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_scale_io_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_scale_io_persistent_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_deployment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_external_documentation.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_external_documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_priority_class.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_priority_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_custom_resource_subresource_scale.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_custom_resource_subresource_scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_pod_security_policy.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_pod_security_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_deployment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_deployment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_status_details.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_status_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_object_field_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_object_field_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_env_from_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_env_from_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_daemon_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_daemon_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role_binding.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_priority_class_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_priority_class_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_client_ip_config.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_client_ip_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_access_review_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_access_review_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_glusterfs_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_glusterfs_persistent_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_horizontal_pod_autoscaler_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_key_selector.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map_key_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_role_ref.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_role_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_storage_class_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_storage_class_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoint_subset.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_endpoint_subset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_load_balancer_ingress.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_load_balancer_ingress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replica_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_cross_version_object_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_cross_version_object_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_pods_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_pods_metric_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_affinity_term.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_affinity_term.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_component_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_component_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_scale.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_self_subject_rules_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_self_subject_rules_review_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_cluster_role_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_cluster_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_projection.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_stateful_set_update_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_stateful_set_update_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_endpoints_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_endpoints_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_audit_sink_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_audit_sink_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_affinity.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_affinity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_requirements.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_pod_security_policy_list.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_pod_security_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_projected_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_projected_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_status.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_http_ingress_path.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_http_ingress_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_eviction.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_eviction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_template.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_user_info.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_user_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apiextensions_v1beta1_webhook_client_config.py` & `kubernetes-9.0.1/kubernetes/client/models/apiextensions_v1beta1_webhook_client_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_rules_review_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_rules_review_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_host_alias.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_host_alias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_attachment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_attachment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_controller_revision_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_controller_revision_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_volume_node_affinity.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_volume_node_affinity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_service_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_service_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_host_port_range.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_host_port_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map_projection.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map_projection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_lifecycle.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_lifecycle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_pods_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_pods_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_allowed_flex_volume.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_allowed_flex_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_api_resource_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_api_resource_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_scale_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_scale_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_webhook.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_webhook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_claim_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_claim_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_network_policy_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_network_policy_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_azure_disk_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_azure_disk_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_access_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_access_review_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_access_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_access_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_object_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_object_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_node_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_node_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_fs_group_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_fs_group_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_rolling_update_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_rolling_update_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_policy_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_policy_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_update_strategy.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_update_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_config_map.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_config_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_local_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_local_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_pod_security_policy_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cron_job.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cron_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_id_range.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_id_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_id_range.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_id_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_stateful_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_stateful_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_object_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_object_metric_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_job.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_external_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_external_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_role.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_stateful_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_stateful_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_validating_webhook_configuration.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_validating_webhook_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_template_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_template_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_rolling_update_daemon_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_rolling_update_daemon_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_persistent_volume_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_persistent_volume_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_volume_attachment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_volume_attachment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_attributes.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_probe.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_probe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_certificate_signing_request_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_certificate_signing_request_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_event_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_event_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/apps_v1beta1_deployment_list.py` & `kubernetes-9.0.1/kubernetes/client/models/apps_v1beta1_deployment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_vsphere_virtual_disk_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_vsphere_virtual_disk_volume_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_resource_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_resource_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_ceph_fs_persistent_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_ceph_fs_persistent_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_self_subject_rules_review.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_self_subject_rules_review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_pod_condition.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_pod_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_allowed_host_path.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_allowed_host_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_ingress.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_ingress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_rollback_config.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_rollback_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/policy_v1beta1_supplemental_groups_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/policy_v1beta1_supplemental_groups_strategy_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container_state_terminated.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container_state_terminated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/admissionregistration_v1beta1_service_reference.py` & `kubernetes-9.0.1/kubernetes/client/models/admissionregistration_v1beta1_service_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_scale_status.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_scale_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_role_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replica_set_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replica_set_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_resource_quota.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_resource_quota.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_replication_controller.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_replication_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_group_version_for_discovery.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_group_version_for_discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_network_policy_egress_rule.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_network_policy_egress_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta2_object_metric_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta2_object_metric_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_container.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1alpha1_volume_attachment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1alpha1_volume_attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_replica_set.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_replica_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_external_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_external_metric_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py` & `kubernetes-9.0.1/kubernetes/client/models/extensions_v1beta1_supplemental_groups_strategy_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_cluster_role_binding_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_cluster_role_binding_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_subject_access_review_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_subject_access_review_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_list.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_horizontal_pod_autoscaler_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_daemon_endpoint.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_daemon_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_se_linux_options.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_se_linux_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_daemon_set_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_daemon_set_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_namespace_status.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_namespace_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v2beta1_resource_metric_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v2beta1_resource_metric_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta2_deployment.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta2_deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_secret_volume_source.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_secret_volume_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1beta1_api_service_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1beta1_api_service_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_deployment_spec.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_deployment_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/models/v1_horizontal_pod_autoscaler.py` & `kubernetes-9.0.1/kubernetes/client/models/v1_horizontal_pod_autoscaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `kubernetes-9.0.0b1/kubernetes/client/api_client.py` & `kubernetes-9.0.1/kubernetes/client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Kubernetes
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: v1.13.4
+    OpenAPI spec version: v1.13.9
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import os
@@ -69,15 +69,15 @@
 
         self.rest_client = RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/9.0.0b1/python'
+        self.user_agent = 'Swagger-Codegen/9.0.1/python'
     
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
             self._pool = None
```

