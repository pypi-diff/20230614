# Comparing `tmp/backend.ai-client-23.3.5.tar.gz` & `tmp/backend.ai-client-23.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-client-23.3.5.tar", last modified: Tue Jun 13 03:42:14 2023, max compression
+gzip compressed data, was "backend.ai-client-23.3.6.tar", last modified: Wed Jun 14 11:13:23 2023, max compression
```

## Comparing `backend.ai-client-23.3.5.tar` & `backend.ai-client-23.3.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.920270 backend.ai-client-23.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-13 03:42:14.920270 backend.ai-client-23.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.900270 backend.ai-client-23.3.5/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.900270 backend.ai-client-23.3.5/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.904270 backend.ai-client-23.3.5/ai/backend/client/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.908270 backend.ai-client-23.3.5/ai/backend/client/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.912269 backend.ai-client-23.3.5/ai/backend/client/cli/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/admin/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/server_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/cli/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.916269 backend.ai-client-23.3.5/ai/backend/client/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/server_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    49999 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/func/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/load_balancing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.920270 backend.ai-client-23.3.5/ai/backend/client/output/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/output/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/output/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/output/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/output/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/output/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30097 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/request.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/ai/backend/client/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.920270 backend.ai-client-23.3.5/backend.ai_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend.ai_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:14.920270 backend.ai-client-23.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-13 03:42:14.000000 backend.ai-client-23.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.305658 backend.ai-client-23.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-14 11:13:23.305658 backend.ai-client-23.3.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.293658 backend.ai-client-23.3.6/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.293658 backend.ai-client-23.3.6/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.297658 backend.ai-client-23.3.6/ai/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.297658 backend.ai-client-23.3.6/ai/backend/client/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.301658 backend.ai-client-23.3.6/ai/backend/client/cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/admin/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/cli/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.301658 backend.ai-client-23.3.6/ai/backend/client/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49999 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/func/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/load_balancing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.301658 backend.ai-client-23.3.6/ai/backend/client/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/output/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/output/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/output/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30097 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/ai/backend/client/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:13:23.305658 backend.ai-client-23.3.6/backend.ai_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-14 11:13:23.000000 backend.ai-client-23.3.6/backend.ai_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:13:23.305658 backend.ai-client-23.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-06-14 11:13:22.000000 backend.ai-client-23.3.6/setup.py
```

### Comparing `backend.ai-client-23.3.5/PKG-INFO` & `backend.ai-client-23.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-client-23.3.5/ai/backend/client/auth.py` & `backend.ai-client-23.3.6/ai/backend/client/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/__init__.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/acl.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/agent.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/domain.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/etcd.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/group.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/image.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/keypair.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/license.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/license.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/manager.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/resource.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/resource_policy.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/scaling_group.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/session.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/storage.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/user.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/admin/vfolder.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/admin/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/announcement.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/announcement.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/app.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/app.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/config.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/dotfile.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/extensions.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/logs.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/main.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/model.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/pagination.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/params.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/params.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/pretty.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/pretty.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/proxy.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/run.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/run.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/server_log.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/service.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/session.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/session_template.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/ssh.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/ssh.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/cli/vfolder.py` & `backend.ai-client-23.3.6/ai/backend/client/cli/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/compat.py` & `backend.ai-client-23.3.6/ai/backend/client/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/config.py` & `backend.ai-client-23.3.6/ai/backend/client/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/exceptions.py` & `backend.ai-client-23.3.6/ai/backend/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/acl.py` & `backend.ai-client-23.3.6/ai/backend/client/func/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/admin.py` & `backend.ai-client-23.3.6/ai/backend/client/func/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/agent.py` & `backend.ai-client-23.3.6/ai/backend/client/func/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/auth.py` & `backend.ai-client-23.3.6/ai/backend/client/func/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/base.py` & `backend.ai-client-23.3.6/ai/backend/client/func/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/bgtask.py` & `backend.ai-client-23.3.6/ai/backend/client/func/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/domain.py` & `backend.ai-client-23.3.6/ai/backend/client/func/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/dotfile.py` & `backend.ai-client-23.3.6/ai/backend/client/func/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/etcd.py` & `backend.ai-client-23.3.6/ai/backend/client/func/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/group.py` & `backend.ai-client-23.3.6/ai/backend/client/func/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/image.py` & `backend.ai-client-23.3.6/ai/backend/client/func/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/keypair.py` & `backend.ai-client-23.3.6/ai/backend/client/func/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/keypair_resource_policy.py` & `backend.ai-client-23.3.6/ai/backend/client/func/keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/manager.py` & `backend.ai-client-23.3.6/ai/backend/client/func/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/model.py` & `backend.ai-client-23.3.6/ai/backend/client/func/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/resource.py` & `backend.ai-client-23.3.6/ai/backend/client/func/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/scaling_group.py` & `backend.ai-client-23.3.6/ai/backend/client/func/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/server_log.py` & `backend.ai-client-23.3.6/ai/backend/client/func/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/service.py` & `backend.ai-client-23.3.6/ai/backend/client/func/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/session.py` & `backend.ai-client-23.3.6/ai/backend/client/func/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/session_template.py` & `backend.ai-client-23.3.6/ai/backend/client/func/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/storage.py` & `backend.ai-client-23.3.6/ai/backend/client/func/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/system.py` & `backend.ai-client-23.3.6/ai/backend/client/func/system.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/user.py` & `backend.ai-client-23.3.6/ai/backend/client/func/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/func/vfolder.py` & `backend.ai-client-23.3.6/ai/backend/client/func/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/load_balancing.py` & `backend.ai-client-23.3.6/ai/backend/client/load_balancing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/output/__init__.py` & `backend.ai-client-23.3.6/ai/backend/client/output/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/output/console.py` & `backend.ai-client-23.3.6/ai/backend/client/output/console.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/output/fields.py` & `backend.ai-client-23.3.6/ai/backend/client/output/fields.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/output/formatters.py` & `backend.ai-client-23.3.6/ai/backend/client/output/formatters.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/output/json.py` & `backend.ai-client-23.3.6/ai/backend/client/output/json.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/output/types.py` & `backend.ai-client-23.3.6/ai/backend/client/output/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/pagination.py` & `backend.ai-client-23.3.6/ai/backend/client/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/request.py` & `backend.ai-client-23.3.6/ai/backend/client/request.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/session.py` & `backend.ai-client-23.3.6/ai/backend/client/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/utils.py` & `backend.ai-client-23.3.6/ai/backend/client/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/ai/backend/client/versioning.py` & `backend.ai-client-23.3.6/ai/backend/client/versioning.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/backend.ai_client.egg-info/PKG-INFO` & `backend.ai-client-23.3.6/backend.ai_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 23.3.5
+Version: 23.3.6
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-client-23.3.5/backend.ai_client.egg-info/SOURCES.txt` & `backend.ai-client-23.3.6/backend.ai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/backend_shim.py` & `backend.ai-client-23.3.6/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.5/setup.py` & `backend.ai-client-23.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     },
     'install_requires': (
         'aiohttp~=3.8.1',
         'aiotusclient~=0.1.4',
         'appdirs~=1.4.4',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.5
+        """backend.ai-cli==23.03.6
 """,
-        """backend.ai-common==23.03.5
+        """backend.ai-common==23.03.6
 """,
-        """backend.ai-plugin==23.03.5
+        """backend.ai-plugin==23.03.6
 """,
         'click>=7.1.2',
         'faker~=13.12.0',
         'humanize>=3.1.0',
         'inquirer~=2.9.2',
         'janus~=1.0.0',
         'multidict>=6.0',
@@ -282,11 +282,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.5
+    'version': """23.03.6
 """,
     'zip_safe': False,
 })
```

