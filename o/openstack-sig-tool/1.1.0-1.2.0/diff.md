# Comparing `tmp/openstack-sig-tool-1.1.0.tar.gz` & `tmp/openstack-sig-tool-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-sig-tool-1.1.0.tar", last modified: Tue Feb 28 07:44:10 2023, max compression
+gzip compressed data, was "openstack-sig-tool-1.2.0.tar", last modified: Wed Jun 14 08:49:58 2023, max compression
```

## Comparing `openstack-sig-tool-1.1.0.tar` & `openstack-sig-tool-1.2.0.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.071909 openstack-sig-tool-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     1194 2023-02-28 07:44:09.000000 openstack-sig-tool-1.1.0/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    66060 2023-02-28 07:44:09.000000 openstack-sig-tool-1.1.0/ChangeLog
--rw-r--r--   0 root         (0) root         (0)    11357 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9538 2023-02-28 07:44:10.071909 openstack-sig-tool-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8749 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.065909 openstack-sig-tool-1.1.0/etc/
--rw-r--r--   0 root         (0) root         (0)   103616 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/constants.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.066909 openstack-sig-tool-1.1.0/etc/inventory/
--rw-r--r--   0 root         (0) root         (0)     3595 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/inventory/oos_inventory.j2
--rwxr-xr-x   0 root         (0) root         (0)     4403 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/inventory/oos_inventory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.066909 openstack-sig-tool-1.1.0/etc/key_pair/
--r--------   0 root         (0) root         (0)     2590 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/key_pair/id_rsa
--rw-r--r--   0 root         (0) root         (0)      557 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/key_pair/id_rsa.pub
--rw-r--r--   0 root         (0) root         (0)     1048 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/oos.conf
--rw-r--r--   0 root         (0) root         (0)   296205 2023-02-28 07:40:34.000000 openstack-sig-tool-1.1.0/etc/openeuler_repo.yaml
--rw-r--r--   0 root         (0) root         (0)    14242 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/openeuler_sig_repo.yaml
--rw-r--r--   0 root         (0) root         (0)    68813 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/openstack_release.yaml
--rw-r--r--   0 root         (0) root         (0)     2900 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/package.spec.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/etc/playbooks/
--rw-r--r--   0 root         (0) root         (0)     3248 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/aodh.yaml
--rw-r--r--   0 root         (0) root         (0)     1632 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/ceilometer.yaml
--rw-r--r--   0 root         (0) root         (0)     4102 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/cinder.yaml
--rw-r--r--   0 root         (0) root         (0)     2993 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/cleanup.yaml
--rw-r--r--   0 root         (0) root         (0)     2784 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/cyborg.yaml
--rw-r--r--   0 root         (0) root         (0)     1425 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/entry.yaml
--rw-r--r--   0 root         (0) root         (0)     1832 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/glance.yaml
--rw-r--r--   0 root         (0) root         (0)     2412 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/gnocchi.yaml
--rw-r--r--   0 root         (0) root         (0)     3474 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/heat.yaml
--rw-r--r--   0 root         (0) root         (0)     1684 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/horizon.yaml
--rw-r--r--   0 root         (0) root         (0)     7322 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/init.yaml
--rw-r--r--   0 root         (0) root         (0)     2780 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/keystone.yaml
--rw-r--r--   0 root         (0) root         (0)      388 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/kolla.yaml
--rw-r--r--   0 root         (0) root         (0)     1585 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/mariadb.yaml
--rw-r--r--   0 root         (0) root         (0)      483 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/memcached.yaml
--rw-r--r--   0 root         (0) root         (0)     6688 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/neutron.yaml
--rw-r--r--   0 root         (0) root         (0)     8757 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/nova.yaml
--rw-r--r--   0 root         (0) root         (0)     1590 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/placement.yaml
--rw-r--r--   0 root         (0) root         (0)     2329 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/pre.yaml
--rw-r--r--   0 root         (0) root         (0)      450 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/rabbitmq.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/rally.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.063909 openstack-sig-tool-1.1.0/etc/playbooks/roles/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.063909 openstack-sig-tool-1.1.0/etc/playbooks/roles/create_identity_service/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/etc/playbooks/roles/create_identity_service/tasks/
--rw-r--r--   0 root         (0) root         (0)      452 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/roles/create_identity_service/tasks/main.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.063909 openstack-sig-tool-1.1.0/etc/playbooks/roles/create_identity_user/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/etc/playbooks/roles/create_identity_user/tasks/
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/roles/create_identity_user/tasks/main.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.063909 openstack-sig-tool-1.1.0/etc/playbooks/roles/init_database/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/etc/playbooks/roles/init_database/tasks/
--rw-r--r--   0 root         (0) root         (0)      906 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/roles/init_database/tasks/main.yaml
--rw-r--r--   0 root         (0) root         (0)     9240 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/swift.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/tempest.yaml
--rw-r--r--   0 root         (0) root         (0)     1197 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/test.yaml
--rw-r--r--   0 root         (0) root         (0)     3567 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/etc/playbooks/trove.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/example/
--rw-r--r--   0 root         (0) root         (0)      283 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/example/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/oos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      468 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.068909 openstack-sig-tool-1.1.0/oos/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.069908 openstack-sig-tool-1.1.0/oos/commands/dependence/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/dependence/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7812 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/dependence/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.069908 openstack-sig-tool-1.1.0/oos/commands/environment/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/environment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6913 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/environment/cli.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/environment/constants.py
--rw-r--r--   0 root         (0) root         (0)    12568 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/environment/provider.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/environment/sqlite_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.069908 openstack-sig-tool-1.1.0/oos/commands/repo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/repo/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15987 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/repo/cli.py
--rw-r--r--   0 root         (0) root         (0)     7822 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/repo/repo_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.070909 openstack-sig-tool-1.1.0/oos/commands/spec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/spec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/spec/cli.py
--rw-r--r--   0 root         (0) root         (0)    12795 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/commands/spec/spec_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.070909 openstack-sig-tool-1.1.0/oos/common/
--rw-r--r--   0 root         (0) root         (0)     3808 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/common/click_custom.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/common/gitee.py
--rw-r--r--   0 root         (0) root         (0)      642 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/common/pypi.py
--rw-r--r--   0 root         (0) root         (0)      628 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/oos/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 07:44:10.071909 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9538 2023-02-28 07:44:10.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2045 2023-02-28 07:44:10.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 07:44:10.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 07:44:10.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 07:42:12.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-02-28 07:44:09.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)      175 2023-02-28 07:44:10.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-28 07:44:10.000000 openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      967 2023-02-28 07:44:10.071909 openstack-sig-tool-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      682 2023-02-28 07:39:53.000000 openstack-sig-tool-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.845790 openstack-sig-tool-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    70808 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9560 2023-06-14 08:49:58.845790 openstack-sig-tool-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8749 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.766790 openstack-sig-tool-1.2.0/etc/
+-rw-r--r--   0 root         (0) root         (0)     6151 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/etc/constants.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.766790 openstack-sig-tool-1.2.0/etc/inventory/
+-rw-r--r--   0 root         (0) root         (0)     3637 2023-05-05 01:54:24.000000 openstack-sig-tool-1.2.0/etc/inventory/oos_inventory.j2
+-rwxr-xr-x   0 root         (0) root         (0)     4465 2023-05-05 01:54:24.000000 openstack-sig-tool-1.2.0/etc/inventory/oos_inventory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.767790 openstack-sig-tool-1.2.0/etc/key_pair/
+-r--------   0 root         (0) root         (0)     2590 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/key_pair/id_rsa
+-rw-r--r--   0 root         (0) root         (0)      557 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/key_pair/id_rsa.pub
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/oos.conf
+-rw-r--r--   0 root         (0) root         (0)   314180 2023-06-14 03:51:20.000000 openstack-sig-tool-1.2.0/etc/openeuler_repo.yaml
+-rw-r--r--   0 root         (0) root         (0)    16402 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/etc/openeuler_sig_repo.yaml
+-rw-r--r--   0 root         (0) root         (0)    68814 2023-06-14 03:51:20.000000 openstack-sig-tool-1.2.0/etc/openstack_release.yaml
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/etc/package.spec.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.802790 openstack-sig-tool-1.2.0/etc/playbooks/
+-rw-r--r--   0 root         (0) root         (0)     3248 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/aodh.yaml
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/ceilometer.yaml
+-rw-r--r--   0 root         (0) root         (0)     4102 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/cinder.yaml
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/cleanup.yaml
+-rw-r--r--   0 root         (0) root         (0)     2784 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/cyborg.yaml
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/entry.yaml
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/glance.yaml
+-rw-r--r--   0 root         (0) root         (0)     2412 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/gnocchi.yaml
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/heat.yaml
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/horizon.yaml
+-rw-r--r--   0 root         (0) root         (0)     7322 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/init.yaml
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/keystone.yaml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/kolla.yaml
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/mariadb.yaml
+-rw-r--r--   0 root         (0) root         (0)      483 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/memcached.yaml
+-rw-r--r--   0 root         (0) root         (0)     6688 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/neutron.yaml
+-rw-r--r--   0 root         (0) root         (0)     8757 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/nova.yaml
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/placement.yaml
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-05-05 09:16:44.000000 openstack-sig-tool-1.2.0/etc/playbooks/pre.yaml
+-rw-r--r--   0 root         (0) root         (0)      450 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/rabbitmq.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/rally.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.741790 openstack-sig-tool-1.2.0/etc/playbooks/roles/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.741790 openstack-sig-tool-1.2.0/etc/playbooks/roles/create_identity_service/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.802790 openstack-sig-tool-1.2.0/etc/playbooks/roles/create_identity_service/tasks/
+-rw-r--r--   0 root         (0) root         (0)      452 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/roles/create_identity_service/tasks/main.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.741790 openstack-sig-tool-1.2.0/etc/playbooks/roles/create_identity_user/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.805790 openstack-sig-tool-1.2.0/etc/playbooks/roles/create_identity_user/tasks/
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/roles/create_identity_user/tasks/main.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.741790 openstack-sig-tool-1.2.0/etc/playbooks/roles/init_database/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.806790 openstack-sig-tool-1.2.0/etc/playbooks/roles/init_database/tasks/
+-rw-r--r--   0 root         (0) root         (0)      906 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/roles/init_database/tasks/main.yaml
+-rw-r--r--   0 root         (0) root         (0)     9240 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/swift.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/tempest.yaml
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/test.yaml
+-rw-r--r--   0 root         (0) root         (0)     3567 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/etc/playbooks/trove.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.806790 openstack-sig-tool-1.2.0/example/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/example/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.823790 openstack-sig-tool-1.2.0/oos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/oos/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.824790 openstack-sig-tool-1.2.0/oos/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.824790 openstack-sig-tool-1.2.0/oos/commands/dependence/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/dependence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7689 2023-05-05 01:54:24.000000 openstack-sig-tool-1.2.0/oos/commands/dependence/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.828790 openstack-sig-tool-1.2.0/oos/commands/environment/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/environment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2023-05-05 01:54:24.000000 openstack-sig-tool-1.2.0/oos/commands/environment/cli.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/environment/constants.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/environment/provider.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/environment/sqlite_ops.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.829790 openstack-sig-tool-1.2.0/oos/commands/repo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/repo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15972 2023-05-05 01:54:24.000000 openstack-sig-tool-1.2.0/oos/commands/repo/cli.py
+-rw-r--r--   0 root         (0) root         (0)     7822 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/repo/repo_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.829790 openstack-sig-tool-1.2.0/oos/commands/spec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/commands/spec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/oos/commands/spec/cli.py
+-rw-r--r--   0 root         (0) root         (0)    12843 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/oos/commands/spec/spec_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.831790 openstack-sig-tool-1.2.0/oos/common/
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/common/click_custom.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/oos/common/gitee.py
+-rw-r--r--   0 root         (0) root         (0)      642 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/oos/common/pypi.py
+-rw-r--r--   0 root         (0) root         (0)      617 2023-05-05 01:54:24.000000 openstack-sig-tool-1.2.0/oos/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.845790 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9560 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 07:42:12.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-14 08:49:58.000000 openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      967 2023-06-14 08:49:58.846790 openstack-sig-tool-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      682 2023-02-28 07:39:53.000000 openstack-sig-tool-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 08:49:58.845790 openstack-sig-tool-1.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-14 03:51:09.000000 openstack-sig-tool-1.2.0/test/test_cli.py
```

### Comparing `openstack-sig-tool-1.1.0/AUTHORS` & `openstack-sig-tool-1.2.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Andy Lee <li_kunshan@163.com>
 AnneY <evangeline-lun@foxmail.com>
 FFrog <ljw1101.vip@gmail.com>
 Fan Zhang <zh.f@outlook.com>
 Han Guangyu <hanguangyu@uniontech.com>
 Jiachen Fan <fjc837005411@outlook.com>
 KevinZhu <zhukeqian1@huawei.com>
+Mozambick <m202271745@hust.edu.cn>
 Song.Gao <gaos50@chinaunicom.cn>
 Yinuo Deng <i@dyn.im>
 ZH.F <zh.f@outlook.com>
 bzhaoop <270162781@qq.com>
 guolei <guolei_yewu@cmss.chinamobile.com>
 honeymoon_217 <jiahui@isrc.iscas.ac.cn>
 huangtianhua <huangtianhua@huawei.com>
@@ -24,12 +25,13 @@
 wangkuntian <wangkuntian@uniontech.com>
 wangxiyuan <wangxiyuan1007@gmail.com>
 xiyuanwang <wangxiyuan1007@gmail.com>
 yanhuiling <jamieyanyan@126.com>
 zhangy1317 <zhangy1317@chinaunicom.cn>
 zhaojf <zhaojf_xt@teamsun.com.cn>
 zhuyong931114 <1316783560@qq.com>
+zwlpp <u202014366@hust.edu.cn>
 刘洋葱 <liuyc@heikite.com>
 哦哈哟 <wangxiyuan1007@gmail.com>
 王玺源 <wangxiyuan1007@gmail.com>
 胡秀杰 <huxiujie1@huawei.com>
 韩光宇 <hanguangyu@uniontech.com>
```

### Comparing `openstack-sig-tool-1.1.0/ChangeLog` & `openstack-sig-tool-1.2.0/ChangeLog`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,150 @@
 CHANGES
 =======
 
+1.2.0
+-----
+
+* !717 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !716 Daily update - openEuler repo
+* !715 Daily update - opentack release
+* Daily update - openEuler repo
+* Daily update - opentack release
+* !714 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !713 Daily update - opentack release
+* Daily update - opentack release
+* !712 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !711 Update unit test Merge pull request !711 from 王玺源/master
+* Update unit test
+* !710 Update unit test
+* Update unit test
+* !708 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !707 Add unittest for oos
+* Add unittest
+* !705 【轻量级 PR】：specify openstackclient version for 22.03 LTS SP1
+* specify openstackclient version for 22.03 LTS SP1
+* !703 Daily update - openEuler repo
+* !702 Daily update - opentack release
+* Daily update - openEuler repo
+* Daily update - opentack release
+* Update oos requirement
+* add docs/spec/openstack-sig-tool-requirement.md
+* !701 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !700 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !698 Daily update - opentack release
+* Daily update - opentack release
+* !697 Add OOS SPEC FILE
+* OOS SPEC
+* !696 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !695 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !694 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !693 Daily update - opentack release
+* Daily update - opentack release
+* !691 Add pyproject support for oos spec create
+* Add pyproject support for oos spec create
+* !692 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !689 Daily update - opentack release
+* !690 Daily update - openEuler repo
+* Daily update - openEuler repo
+* Daily update - opentack release
+* !688 Add oos pypi mapping
+* Add oos pypi mapping
+* !687 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !686 Fix some issue
+* Fix spec update issue
+* !685 Daily update - opentack release
+* Daily update - opentack release
+* !683 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !682 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !681 Fix repo mirror and mapping problem
+* Fix repo mirror and mapping problem
+* !680 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !679 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !678 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !677 Daily update - opentack release
+* Daily update - opentack release
+* !674 Remove unused imports and local variables
+* remove unused imports and local variables
+* !676 【轻量级 PR】：修复了api请求函数中的一些问题
+* fix bugs
+* !675 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !673 Daily update - openEuler repo
+* !672 Daily update - opentack release
+* Daily update - openEuler repo
+* Daily update - opentack release
+* !671 Daily update - openEuler repo
+* !670 Daily update - opentack release
+* Daily update - openEuler repo
+* Daily update - opentack release
+* !669 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !668 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !667 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !666 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !665 oos nit update
+* OOS nit fix
+* !664 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !662 Fix 22.03 lts sp1 doc
+* Fix 22.03 lts sp1 doc
+* !661 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !660 Add more openstack project
+* Add more openstack project
+* !659 Daily update - opentack release
+* Daily update - opentack release
+* !658 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !657 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !656 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !655 Daily update - openEuler repo
+* !654 【轻量级 PR】：update openstack ci script
+* Daily update - openEuler repo
+* update openstack ci script
+* !653 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !652 Daily update - openEuler repo
+* !651 Daily update - opentack release
+* Daily update - openEuler repo
+* Daily update - opentack release
+* !650 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !649 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !648 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !646 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !645 Daily update - openEuler repo
+* Daily update - openEuler repo
+* !644 Daily update - openEuler repo
+* Daily update - openEuler repo
+
 1.1.0
 -----
 
 * !643 Daily update - openEuler repo
 * Daily update - openEuler repo
 * !641 Daily update - openEuler repo
 * Daily update - openEuler repo
```

### Comparing `openstack-sig-tool-1.1.0/LICENSE` & `openstack-sig-tool-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/PKG-INFO` & `openstack-sig-tool-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-sig-tool
-Version: 1.1.0
+Version: 1.2.0
 Summary: The command line tool for openEuler OpenStack SIG
 Home-page: https://gitee.com/openeuler/openstack/
 Author: openEuler OpenStack SIG
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: AUTHORS
 
 # OpenStack SIG 开发工具
 
 oos(openEuler OpenStack SIG)是OpenStack SIG提供的命令行工具。该工具为OpenStack SIG开发提供了若干功能。包括
 
 1. 自动生成、更新RPM Spec
 2. 自动分析OpenStack软件包依赖
```

### Comparing `openstack-sig-tool-1.1.0/README.md` & `openstack-sig-tool-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/inventory/oos_inventory.j2` & `openstack-sig-tool-1.2.0/etc/inventory/oos_inventory.j2`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     {% for device in swift_storage_devices %}
                 "{{ device }}"{% if not loop.last %},{% endif %}
     {% endfor %}
             ],
             "openstack_release": "{{ openstack_release }}",
             "oos_env_type": "{{ oos_env_type }}",
             "keypair_dir": "{{ keypair_dir }}",
+            "provider": "{{ provider }}",
             "cinder_api_workers": "{{ cinder_api_workers }}",
             "glance_api_workers": "{{ glance_api_workers }}",
             "neutron_api_workers": "{{ neutron_api_workers }}",
             "nova_api_workers": "{{ nova_api_workers }}",
             "nova_metadata_api_workers": "{{ nova_metadata_api_workers }}",
             "nova_conductor_workers": "{{ nova_conductor_workers }}",
             "nova_scheduler_workers": "{{ nova_scheduler_workers }}"
```

### Comparing `openstack-sig-tool-1.1.0/etc/inventory/oos_inventory.py` & `openstack-sig-tool-1.2.0/etc/inventory/oos_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
                      'nova_conductor_workers': config.get('environment', 'nova_conductor_workers'),
                      'nova_scheduler_workers': config.get('environment', 'nova_scheduler_workers'),
                      'neutron_api_workers': config.get('environment', 'neutron_api_workers'),
                      'horizon_allowed_host': config.get('environment', 'horizon_allowed_host'),
                      'kolla_openeuler_plugin': config.get('environment', 'kolla_openeuler_plugin'),
                      'oos_env_type': os.environ.get('OOS_ENV_TYPE'),
                      'openstack_release': os.environ.get('OpenStack_Release'),
-                     'keypair_dir': os.environ.get('keypair_dir')
+                     'keypair_dir': os.environ.get('keypair_dir'),
+                     'provider': os.environ.get('provider'),
                     }
     output = template.render(template_vars)
     return output
 
 
 def init_config():
     search_paths = ['/etc/oos/',
```

### Comparing `openstack-sig-tool-1.1.0/etc/key_pair/id_rsa` & `openstack-sig-tool-1.2.0/etc/key_pair/id_rsa`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/key_pair/id_rsa.pub` & `openstack-sig-tool-1.2.0/etc/key_pair/id_rsa.pub`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/oos.conf` & `openstack-sig-tool-1.2.0/etc/oos.conf`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/openeuler_repo.yaml` & `openstack-sig-tool-1.2.0/etc/openeuler_repo.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -5,52 +5,57 @@
   A-Tune-BPF-Collection: A-Tune
   A-Tune-Collector: A-Tune
   A-Tune-UI: A-Tune
   A-guard: sig-Gatekeeper
   Agith: sig-ebpf
   AppAPIChecker: sig-OSRefTools
   AvxToNeon: sig-AccLib
+  BIDK: sig-HPC
   BiSheng-Adoptium: Compiler
   BiShengCLanguage: Compiler
   CPM4OSSP-PROXY: sig-ops
   CPM4OSSP-SERVER: sig-ops
   CPM4OSSP-UI: sig-ops
   CPython: Compiler
   CTinspector: sig-ebpf
   Cpds: sig-CloudNative
   CreateImage: sig-Gatekeeper
   DyscheOS-kernel: sig-recycle
   DyscheOS-meta: sig-recycle
   DyscheOS-utils: sig-recycle
+  EulerMonitor: sig-ops
   EulerRobot: sig-QA
   G11N: G11N
   GNFC: sig-high-performance-network
   GearOS: sig-industrial-control
   Intel-Arch-doc: sig-Intel-Arch
   Intel-gcc: sig-Intel-Arch
   Intel-glibc: sig-Intel-Arch
+  Jailhouse-gui: sig-industrial-control
   Java-Packages: sig-Java
   KPL-gmssl: sig-WayCa
   KPL-zlib: sig-WayCa
   Kmesh: sig-ebpf
   KubeHawk: sig-CloudNative
   KubeHawkeyes: sig-CloudNative
   KubeOS: sig-CloudNative
   NestOS: sig-CloudNative
   OSAPIChecker: sig-OSRefTools
   OSCompatibility: sig-OSRefTools
   OSPerformance: sig-OSRefTools
+  OSPerformanceTools: sig-OSRefTools
   PRIP: Networking
   PilotGo: sig-ops
   PilotGo-plugins: sig-ops
   PilotGo-web: sig-ops
   Preempt_RT: sig-industrial-control
   QA: sig-QA
   QARobot: sig-QA
   RISC-V: sig-RISC-V
+  Replay-N: sig-high-performance-network
   TC: TC
   TCP_option_address: Kernel
   UniProton: sig-embedded
   WasmEngine: sig-CloudNative
   WayCa: sig-WayCa
   X-diagnosis: sig-ops
   aarch32-rootfs-builder: sig-Yocto
@@ -78,14 +83,16 @@
   bishengjdk-11: Compiler
   bishengjdk-17: Compiler
   bishengjdk-8: Compiler
   bishengjdk-build: Compiler
   bishengjdk-riscv: Compiler
   blesschess: sig-minzuchess
   blog: sig-recycle
+  c2rust: dev-utils
+  cache-proxy: Infrastructure
   capsule: Virt
   ceph_dev: sig-SDS
   certificate-center: sig-OpenDesign
   ci-bot: sig-Gatekeeper
   clibcni: iSulad
   cloudnative: sig-CloudNative
   community: TC
@@ -107,33 +114,39 @@
   cve-manager: Infrastructure
   dcs: sig-power-efficient
   dde: sig-DDE
   deepin-rpm-installer: sig-DDE
   deepin-upgrade-tool: sig-DDE
   digest-list-tools: sig-security-facility
   dim_tools: sig-security-facility
+  distributed-codelabs: sig-distributed-middleware
   docs: doc
   docs-accompany-reading: sig-OpenDesign
+  donau-pam-adopt: sig-HPC
   donau-slurm-wrappers: sig-HPC
   dpdk: sig-high-performance-network
   dpu-core: sig-DPU
   dpu-utilities: sig-DPU
   dsoftbus_standard: sig-embedded
   duoyibu-ai: sig-minzuchess
   eagle: sig-power-efficient
   easy-checker: sig-EasyLife
   eggo: sig-CloudNative
   elfin-parser: sig-HPC
   embedded: sig-embedded
+  embedded-ci: sig-Yocto
   embedded-ipc: sig-embedded
+  env_check: sig-Compatibility-Infra
   etmem: Storage
   eulerfs: Kernel
   eulerfs-test: Kernel
+  eulerlauncher: Infrastructure
   evs: sig-high-performance-network
   extfuse: Storage
+  ft_engine: sig-FangTian
   gala-anteater: sig-ops
   gala-docs: sig-ops
   gala-gopher: sig-ebpf
   gala-ragdoll: sig-ops
   gala-spider: sig-ops
   gazelle: sig-high-performance-network
   gazelle-cni: sig-recycle
@@ -141,26 +154,29 @@
   gcc-anti-sca: Compiler
   gcc-for-openEuler: Compiler
   geo-coding: dev-utils
   git-basics: sig-OSCourse
   gitbook-theme-hugo: Infrastructure
   globalization: G11N
   go-gitee: Infrastructure
+  gostone: sig-openstack
   ha-api: sig-Ha
   ha-web: sig-Ha
   hands-on: sig-OSCourse
   hikptool: sig-WayCa
   hmir: sig-ops
   hostha: sig-openstack
   hpc: sig-HPC
+  hpcpilot: sig-HPC
   hpcrunner: sig-HPC
   hsak: Storage
   hw-buaa-lab: sig-OSCourse
   iSulad: iSulad
   iSulad-img: sig-recycle
+  ifm_nettle: sig-AccLib
   imageTailor: sig-OS-Builder
   infrastructure: Infrastructure
   install-scripts: sig-OS-Builder
   integration-test: sig-QA
   intel-kernel: sig-Intel-Arch
   intel-qemu: sig-Intel-Arch
   isula-build: iSulad
@@ -173,14 +189,15 @@
   kbox: sig-ops
   kbuild-standalone: Kernel
   kconfigDetector: Kernel
   kernel: Kernel
   kernel-ascend: Kernel
   kernel-cloudnative: Kernel
   kernel-docs: Kernel
+  kiran-authentication-devices: sig-KIRAN-DESKTOP
   kiran-authentication-service: sig-KIRAN-DESKTOP
   kiran-biometrics: sig-KIRAN-DESKTOP
   kiran-calculator: sig-KIRAN-DESKTOP
   kiran-calendar: sig-KIRAN-DESKTOP
   kiran-cc-daemon: sig-KIRAN-DESKTOP
   kiran-control-panel: sig-KIRAN-DESKTOP
   kiran-desktop: sig-KIRAN-DESKTOP
@@ -191,14 +208,15 @@
   kiran-menu: sig-KIRAN-DESKTOP
   kiran-panel: sig-KIRAN-DESKTOP
   kiran-qdbusxml2cpp: sig-KIRAN-DESKTOP
   kiran-qt5-integration: sig-KIRAN-DESKTOP
   kiran-screensaver: sig-KIRAN-DESKTOP
   kiran-session-guard: sig-KIRAN-DESKTOP
   kiran-session-manager: sig-KIRAN-DESKTOP
+  kiran-shell: sig-KIRAN-DESKTOP
   kiran-tests: sig-KIRAN-DESKTOP
   kiran-wallpapers: sig-KIRAN-DESKTOP
   kiran-widgets-qt5: sig-KIRAN-DESKTOP
   kml_adapter: sig-AccLib
   ksc-defender: sig-security-facility
   kunpeng-competition: sig-OSCourse
   kunpengsecl: sig-security-facility
@@ -218,40 +236,42 @@
   libvirt: Virt
   libwd: sig-AccLib
   libxml2-rust: Base-service
   linux-operation: sig-OSCourse
   llvm-project: Compiler
   lxcfs-tools: iSulad
   lzu-icc-nsg: sig-OSCourse
+  m1600-driver: sig-Compatibility-Infra
   marketing: Marketing
   mate-desktop: sig-mate-desktop
   mcs: sig-embedded
   memory-scan: Storage
   memwatch: dev-utils
   micro-certification: sig-OSCourse
   migration-assistant: sig-Migration
+  migration-tools: sig-Migration
   mugen: sig-QA
-  n5p-core: sig-n5p
   nankai_university_2021: sig-recycle
   native-turbo: A-Tune
   native-turbo-kernel: A-Tune
   nestos-assembler: sig-CloudNative
   nestos-config: sig-CloudNative
   nestos-installer: sig-CloudNative
+  nestos-kubernetes-deployer: sig-K8sDistro
   nestos-website: sig-CloudNative
   nodejsporter: dev-utils
   nvme-snsd: Storage
   nvwa: sig-ops
   oe-performance: sig-Compatibility-Infra
   oebuild: sig-Yocto
   oec-application: sig-Compatibility-Infra
+  oec-cloud: sig-Compatibility-Infra
   oec-hardware: sig-Compatibility-Infra
   oecp: sig-Compatibility-Infra
   oemaker: sig-OS-Builder
-  omnivirt: Infrastructure
   oncn-bwm: sig-high-performance-network
   open-source-summer: sig-OSCourse
   openEuler-Advisor: sig-EasyLife
   openEuler-bootstrap: dev-utils
   openEuler-lsb: sig-release-management
   openEuler-menus: sig-KDE
   openEuler-pkginfo: dev-utils
@@ -290,56 +310,62 @@
   peking_university_2021: sig-recycle
   perlporter: dev-utils
   pin-gcc-client: Compiler
   pin-server: Compiler
   pkgporter: dev-utils
   pkgship: sig-EasyLife
   plymouth-theme-kiran: sig-KIRAN-DESKTOP
+  portal-application-license-monitor: sig-HPC
   portal-mulit-cluster-script: sig-HPC
   powerapi: sig-power-efficient
   prefetch_tuning: A-Tune
   ptcr: sig-CloudNative
   pyisula: sig-openstack
   pyporter: dev-utils
   python-multi_key_dict: sig-python-modules
   qax-gm-certificates: sig-security-facility
   qemu: Virt
   qla2xxx: sig-Compatibility-Infra
+  qt6: sig-QT
   quick-issue: sig-OpenDesign
   radiaTest: sig-QA
   raspberrypi: sig-RaspberryPi
   raspberrypi-build: sig-RaspberryPi
   raspberrypi-kernel: sig-RaspberryPi
   re2-rust: Base-service
   release-management: sig-release-management
   release-tools: sig-EasyLife
   reproducible-builds: sig-reproducible-builds
   rockchip: sig-RaspberryPi
   rockchip-kernel: sig-RaspberryPi
   ros: sig-ROS
+  ros-porting-tools: sig-ROS
   rubik: sig-CloudNative
   rubyporter: dev-utils
   rust_shyper: Virt
+  sds_doc: sig-SDS
   secGear: sig-confidential-computing
   secpaver: sig-security-facility
   security-committee: security-committee
   security-facility: sig-security-facility
   security-tool: sig-security-facility
   service_capability: sig-Talent-and-Service
   service_trainning: sig-Talent-and-Service
   sig-Edge: sig-Edge
   sig-OSCourse: sig-OSCourse
-  sig-OpenBoard: sig-OpenBoard
+  sig-OpenBoard: sig-recycle
+  signatrust: Infrastructure
   skylark: Virt
   sonic-linux-kernel: sig-ONL
   stortrace: Storage
   stratovirt: Virt
   summer2022: sig-OSCourse
   sw-committee: sig-sw-arch
   sync-bot: sig-EasyLife
+  sysboost: A-Tune
   syscare: sig-ops
   syscontainer-tools: iSulad
   sysmaster: dev-utils
   sysmonitor: sig-ops
   taishan-oslab: sig-OSCourse
   talent-assessment: sig-OpenDesign
   tarsier: sig-high-performance-network
@@ -352,14 +378,16 @@
   trucker: dev-utils
   uadk: sig-AccLib
   uadk_engine: sig-AccLib
   ubackup: sig-Migration
   ukui: sig-UKUI
   umdk: sig-high-performance-network
   user-committee: user-committee
+  utshell: sig-memsafety
+  utsudo: sig-memsafety
   vectorBlas: bigdata
   vmtop: Virt
   wayca-scheduler: sig-WayCa
   wayca-scheduler-bench: sig-WayCa
   website: Infrastructure
   website-v2: sig-recycle
   wine-app: sig-compat-winapp
@@ -382,30 +410,35 @@
   A-Ops: sig-ops
   A-Tune: A-Tune
   A-Tune-BPF-Collection: A-Tune
   A-Tune-Collector: A-Tune
   A-Tune-UI: A-Tune
   BareBonesBrowserLaunch: sig-Java
   Bear: Compiler
+  BehaviorTree.CPP: sig-ROS
   CUnit: Base-service
+  Catch2: sig-ROS
   CharLS: Desktop
   ComputeLibrary: ai
   Control-FREEC: sig-bio
   CreateImage: sig-Gatekeeper
   Cython: Programming-language
   DCache: Storage
   DevIL: Application
   Done: Private
+  DynamixelSDK: sig-ROS
+  EulerMonitor: sig-ops
   FAudio: sig-compat-winapp
   Fast-CDR: sig-ROS
   Fast-DDS: sig-ROS
   Flask-RESTful: Private
+  FluentRviz: sig-ROS
+  FogROS2: sig-ROS
   GAPP: dev-utils
   GATK: sig-bio
-  GATK3: sig-bio
   GConf2: Desktop
   GeoIP: Networking
   GeoIP-GeoLite-data: Networking
   GraphicsMagick: Application
   HdrHistogram: Application
   HikariCP: sig-Java
   ImageMagick: Others
@@ -438,14 +471,15 @@
   OpenCSD: dev-utils
   OpenEXR: Runtime
   OpenIPMI: Networking
   PEGTL: dev-utils
   PackageKit: Desktop
   PackageKit-Qt: Desktop
   Picard: sig-bio
+  PlotJuggler: sig-ROS
   PyDrive: sig-UKUI
   PyPAM: Others
   PyQt4: sig-python-modules
   PyYAML: sig-python-modules
   R-AUC: sig-RISC-V
   R-AsioHeaders: sig-RISC-V
   R-BH-devel: sig-RISC-V
@@ -475,15 +509,14 @@
   R-brio: sig-RISC-V
   R-cachem: sig-RISC-V
   R-callr: sig-RISC-V
   R-car: sig-RISC-V
   R-cli: sig-RISC-V
   R-coda: sig-RISC-V
   R-commonmark: sig-RISC-V
-  R-core: sig-bio
   R-cpp11: sig-RISC-V
   R-crayon: sig-RISC-V
   R-curl: sig-RISC-V
   R-desc: sig-RISC-V
   R-dichromat: sig-RISC-V
   R-diffobj: sig-RISC-V
   R-digest: sig-RISC-V
@@ -554,24 +587,29 @@
   R-whisker: sig-RISC-V
   R-withr: sig-RISC-V
   R-xfun: sig-RISC-V
   R-xml2: sig-RISC-V
   R-xtable: sig-RISC-V
   R-yaml: sig-RISC-V
   R-zoo: sig-RISC-V
+  RSL: sig-ROS
   SDL: Programming-language
   SDL2: Others
   SDL_sound: dev-utils
+  SMACC2: sig-ROS
   ShellCheck: sig-CloudNative
   SuperLU: dev-utils
   SuperLUMT: ai
   TCP_option_address: Kernel
   TRF: sig-HPC
   TeXamator: Base-service
   Thunar: xfce
+  Universal_Robots_Client_Library: sig-ROS
+  Universal_Robots_ROS2_Description: sig-ROS
+  Universal_Robots_ROS2_Driver: sig-ROS
   WALinuxAgent: sig-CloudNative
   WLLVM: Compiler
   WasmEngine: sig-CloudNative
   X-diagnosis: sig-ops
   Xaw3d: Desktop
   Xenomai4: sig-industrial-control
   XmlSchema: Application
@@ -582,55 +620,65 @@
   abduco: Application
   abi-compliance-checker: sig-EasyLife
   abi-dumper: sig-EasyLife
   abrt: Application
   abrt-java-connector: Application
   abrt-server-info-page: Application
   abseil-cpp: Base-service
+  acado_vendor: sig-ROS
   accel-config: sig-Intel-Arch
   accerciser: sig-KIRAN-DESKTOP
   accounts-qml-module: sig-KDE
   accountsservice: Desktop
   accumulo: bigdata
+  ackermann_msgs: sig-ROS
   acl: Base-service
   acme-tiny: Application
   acpica-tools: Base-service
   acpid: Computing
   actionlib: sig-ROS
   activemq: Application
+  adaptive_component: sig-ROS
   adb-enhanced: dev-utils
   adcli: Base-service
   adobe-mappings-cmap: Desktop
   adobe-mappings-pdf: Desktop
   adwaita-icon-theme: Desktop
   adwaita-qt: Desktop
   aesh: sig-Java
   aespipe: sig-security-facility
   afflib: Others
   afterburn: sig-CloudNative
   aha: Application
   aide: Base-service
   airline: Base-service
+  aisleriot: sig-desktop-apps
   alertmanager: sig-CloudNative
   allegro: Private
   alluxio: bigdata
   alpine: Application
   alsa-firmware: Computing
   alsa-lib: Computing
   alsa-plugins: Runtime
   alsa-tools: Computing
   alsa-utils: Application
   amanda: Application
   amavis: Application
   ambari: bigdata
+  ament_acceleration: sig-ROS
+  ament_black: sig-ROS
   ament_cmake: sig-ROS
+  ament_cmake_catch2: sig-ROS
   ament_cmake_ros: sig-ROS
+  ament_download: sig-ROS
   ament_index: sig-ROS
   ament_lint: sig-ROS
+  ament_nodl: sig-ROS
   ament_package: sig-ROS
+  ament_vitis: sig-ROS
   amtk: Application
   anaconda: sig-OS-Builder
   anaconda-user-help: sig-OS-Builder
   android-json-org-java: sig-Java
   angles: sig-ROS
   annobin: Others
   annotation-indexer: sig-Java
@@ -702,27 +750,32 @@
   apache-rat: Application
   apache-resource-bundles: sig-Java
   apache-rpm-macros: Application
   apache-sshd: dev-utils
   apache2-mod_xforward: Others
   apacheds: sig-Java
   apacheds-ldap-api: sig-Java
+  apex_containers: sig-ROS
+  apex_test_tools: sig-ROS
   api-guarder: sig-EasyLife
   apiguardian: sig-Java
   apisix: sig-OpenResty
   apisix-dashboard: sig-OpenResty
   apisix-deps: sig-OpenResty
   apiviz: dev-utils
   apparmor: sig-security-facility
   appstream: dev-utils
   appstream-data: sig-recycle
   apptainer: sig-HPC
   appweb: Networking
   apr: Base-service
   apr-util: Base-service
+  apriltag: sig-ROS
+  apriltag_msgs: sig-ROS
+  apriltag_ros: sig-ROS
   aqute-bnd: sig-Java
   arangodb: sig-ops
   argbash: Application
   argon2: Base-service
   args4j: sig-Java
   argus: Application
   argyllcms: System-tool
@@ -743,25 +796,27 @@
   arp-scan: Networking
   arpack: sig-epol
   arpack-ng: Computing
   arptables: Networking
   arpwatch: Networking
   arquillian-core: sig-Java
   artemis: sig-Java
+  aruco_ros: sig-ROS
   asciidoc: Base-service
   asdcplib: sig-epol
   asio: dev-utils
   aspectjweaver: sig-Java
   aspell: Application
   aspell-en: Application
   assertj-core: Programming-language
   assimp: Others
   astream: Kernel
   astyle: sig-KDE
   asymptote: dev-utils
+  async_web_server_cpp: sig-ROS
   at: Base-service
   at-spi2-atk: Desktop
   at-spi2-core: Desktop
   atf: Base-service
   atinject: sig-Java
   atk: Desktop
   atkmm: GNOME
@@ -785,63 +840,70 @@
   autoconf-archive: Programming-language
   autoconf213: Programming-language
   autofdo: Compiler
   autofs: System-tool
   autogen: Base-service
   automake: Base-service
   automoc: dev-utils
+  automotive_autonomy_msgs: sig-ROS
   autossh: Application
   autotrace: Private
   autotune: Others
+  autoware_auto_msgs: sig-ROS
   avahi: Desktop
   avalon-framework: sig-Java
   avalon-logkit: sig-Java
   avocado: sig-QA
   avor: bigdata
   avro: Application
   avro-python3: sig-openstack
+  avt_vimba_camera: sig-ROS
+  aws-robomaker-small-warehouse-world: sig-ROS
   aws-sdk-java: sig-Java
   awscli: sig-CloudNative
   axel: sig-epol
   axiom: Base-service
   azote: Desktop
   b43-openfwwf: Networking
   b43-tools: System-tool
   babel: Base-service
   babeld: Networking
   babeltrace: Base-service
   babeltrace2: Base-service
   babl: Others
   backintime: Desktop
   backupninja: Application
+  backward_ros: sig-ROS
   bacula: System-tool
+  bag2_to_image: sig-ROS
   bam: dev-utils
   bamf: sig-UKUI
   bamtools: sig-bio
   banner: Application
   baobab: GNOME
   barcode: Application
   barman: DB
   barrier: Application
   base64coder: dev-utils
   basesystem: Base-service
   bash: Base-service
   bash-argsparse: dev-utils
   bash-completion: Base-service
+  bat: dev-utils
   batik: sig-Java
   bazel: ai
   bc: Base-service
   bcache-tools: Storage
   bcc: sig-ebpf
   bcel: dev-utils
   bcftools: sig-bio
   bcm283x-firmware: Private
   bcrypt: dev-utils
   bea-stax: dev-utils
-  beakerlib: Others
+  beakerlib: Base-service
   bean-validation-api: sig-Java
   beanstalkd: Computing
   bedops: sig-bio
   bedtools: sig-bio
   beust-jcommander: dev-utils
   bgenix: sig-bio
   biber: sig-perl-modules
@@ -858,20 +920,22 @@
   blaze: bigdata
   blis: sig-epol
   blivet-gui: sig-OS-Builder
   blktrace: Storage
   blueman: sig-UKUI
   bluez: Base-service
   blur-effect: Desktop
+  bno055: sig-ROS
   bogofilter: sig-UKUI
   boilerpipe: Application
   bolt: System-tool
   bond_core: sig-ROS
   boom-boot: Others
   boost: Computing
+  boost_geometry_util: sig-ROS
   booth: sig-Ha
   bootstrap: sig-nodejs
   bootupd: sig-K8sDistro
   botan2: sig-KDE
   bouncycastle: dev-utils
   bowtie2: sig-bio
   box86: sig-compat-winapp
@@ -906,14 +970,15 @@
   bytelist: sig-Java
   byteman: sig-Java
   byzanz: Desktop
   bzip2: Base-service
   c-STAR: sig-bio
   c-ares: Networking
   c-blosc: dev-utils
+  c2rust: dev-utils
   c3p0: sig-Java
   ca-certificates: Base-service
   cachefilesd: Storage
   cadvisor: sig-CloudNative
   caffe: sig-recycle
   caffeine: dev-utils
   cairo: Desktop
@@ -932,17 +997,19 @@
   canfestival-xenomai: sig-industrial-control
   canopennode: sig-industrial-control
   capstone: Base-service
   capsule: Virt
   caribou: sig-cinnamon
   cartographer: sig-ROS
   cartographer_ros: sig-ROS
+  cascade_lifecycle: sig-ROS
   cassandra-java-driver: sig-Java
   castor: Base-service
   castor-maven-plugin: sig-Java
+  castxml: Desktop
   catatonit: sig-CloudNative
   catch1: dev-utils
   catdoc: sig-KDE
   catfish: xfce
   catkin: sig-ROS
   cbi-plugins: Base-service
   ccache: Compiler
@@ -965,14 +1032,15 @@
   cgit: sig-epol
   cglib: dev-utils
   check: Programming-language
   checkpolicy: sig-security-facility
   checkstyle: Application
   cheese: Desktop
   chkconfig: Base-service
+  chmlib: sig-desktop-apps
   chromaprint: dev-utils
   chromium: Application
   chrony: Networking
   chrpath: Base-service
   ci_check: Private
   ci_project: Private
   cifs-utils: Storage
@@ -1048,23 +1116,27 @@
   coin-or-dylp: sig-epol
   coin-or-osi: sig-epol
   coin-or-sample: sig-epol
   coin-or-vol: sig-epol
   collectd: oVirt
   colm: dev-utils
   color-filesystem: Desktop
+  color_names-release: sig-ROS
   colord: Desktop
   colord-gtk: System-tool
   colordiff: dev-utils
   common_interfaces: sig-ROS
   common_msgs: sig-ROS
   common_tutorials: sig-ROS
+  commonlibrary_c_utils: sig-distributed-middleware
+  communication_ipc: sig-distributed-middleware
   compat-libgfortran: Private
   compat-lua: sig-epol
   compat-openssl11: sig-security-facility
+  compat-rest: Desktop
   compface: Application
   compiler-rt: Compiler
   compiler-rt-15: Compiler
   compress-lzf: Application
   comps-extras: Desktop
   concurrent-trees: dev-utils
   conmon: Others
@@ -1074,14 +1146,15 @@
   console_bridge: sig-ROS
   console_bridge_vendor: sig-ROS
   container-exception-logger: Others
   container-selinux: sig-CloudNative
   containerd: sig-CloudNative
   containernetworking-plugins: sig-CloudNative
   containers-common: sig-CloudNative
+  control_box_rst: sig-ROS
   control_msgs: sig-ROS
   control_toolbox: sig-ROS
   convmv: Application
   cookcc: Base-service
   cookxml: sig-recycle
   copy-jdk-configs: Packaging
   coredns: sig-CloudNative
@@ -1090,23 +1163,26 @@
   corosync: sig-Ha
   corosync-qdevice: sig-Ha
   courier-unicode: dev-utils
   cowsay: sig-recycle
   cpio: Base-service
   cpp-hocon: Base-service
   cpp-httplib: dev-utils
+  cpp_polyfills: sig-ROS
   cppcheck: Programming-language
   cpptasks: sig-Java
   cppunit: Programming-language
+  cppzmq: sig-ROS
   cpuid: dev-utils
   cracklib: sig-security-facility
   crash: Base-service
   crash-gcore-command: Programming-language
   crash-trace-command: Programming-language
   crda: sig-recycle
+  create3_sim-release: sig-ROS
   createrepo_c: Base-service
   cri-o: sig-CloudNative
   cri-tools: sig-CloudNative
   criu: sig-ops
   cronie: Base-service
   crontabs: Base-service
   crudini: sig-openstack
@@ -1116,25 +1192,27 @@
   crypto-policies: sig-security-facility
   cryptopp: sig-security-facility
   cryptsetup: Storage
   cscope: Programming-language
   csmith: dev-utils
   ct-ng: sig-embedded
   ctags: Base-service
+  cudnn_cmake_module: sig-ROS
   cufflinks: sig-bio
   culmus-fonts: Application
   cups: Desktop
   cups-filters: System-tool
   cups-pk-helper: Desktop
   curator: dev-utils
   curl: Networking
   curl-rust: Networking
   curvesapi: dev-utils
   custodia: System-tool
   custom_build_tool: Application
+  customization_config_policy: sig-distributed-middleware
   cvs: Programming-language
   cvsps: Private
   cxf: Base-service
   cxf-build-utils: sig-Java
   cxf-xjc-utils: sig-Java
   cyclonedds: sig-ROS
   cyrus-imapd: Application
@@ -1147,22 +1225,25 @@
   daos: sig-SDS
   dash: Application
   datafu: bigdata
   datanucleus-api-jdo: sig-Java
   datanucleus-core: sig-Java
   datanucleus-maven-parent: sig-Java
   datanucleus-rdbms: sig-Java
+  dataspeed_can: sig-ROS
+  datovka: sig-desktop-apps
   dav1d: Desktop
   dblatex: Application
   dbus: Base-service
   dbus-broker: Base-service
   dbus-cpp: dev-utils
   dbus-glib: Base-service
   dbus-python: Base-service
   dbusmenu-qt: dev-utils
+  dbw_ros: sig-ROS
   dbxtool: Base-service
   dcmtk: sig-epol
   dconf: Desktop
   dconf-editor: Desktop
   dcraw: Application
   dcs: sig-power-efficient
   ddcutil: sig-UKUI
@@ -1226,14 +1307,18 @@
   deepin-wallpapers: sig-DDE
   deja-dup: sig-UKUI
   dejagnu: Programming-language
   dejavu-fonts: System-tool
   delta: bigdata
   deltarpm: Base-service
   delve: dev-utils
+  demos: sig-ROS
+  depthai-core: sig-ROS
+  depthai-ros: sig-ROS
+  depthimage_to_laserscan: sig-ROS
   derby: DB
   desktop-file-utils: Desktop
   devhelp: GNOME
   dhcp: Networking
   diagnostics: sig-ROS
   dialog: Base-service
   dibbler: sig-openstack
@@ -1244,22 +1329,30 @@
   digest-list-tools: sig-security-facility
   dim_tools: sig-security-facility
   ding-libs: Base-service
   discount: Application
   diskimage-builder: sig-openstack
   disomaster: Desktop
   disruptor: Base-service
+  distributed-build: sig-distributed-middleware
+  distributed-build_lite: sig-distributed-middleware
+  distributeddatamgr_data_object: sig-distributed-middleware
+  distributeddatamgr_datamgr_service: sig-distributed-middleware
+  distributeddatamgr_kv_store: sig-distributed-middleware
+  distributeddatamgr_relational_store: sig-distributed-middleware
+  distributedhardware_device_manager: sig-distributed-middleware
   djvulibre: Others
   dkms: Others
   dleyna-connector-dbus: dev-utils
   dleyna-core: dev-utils
   dleyna-renderer: GNOME
   dleyna-server: Application
   dlib: ai
   dlm: Application
+  dmenu: Desktop
   dmidecode: Computing
   dmraid: Storage
   dnf: sig-OS-Builder
   dnf-plugin-ovl: sig-OS-Builder
   dnf-plugins-core: sig-OS-Builder
   dnsjava: sig-Java
   dnsmasq: Networking
@@ -1272,16 +1365,18 @@
   docbook5-schemas: Application
   docbook5-style-xsl: Application
   docker: sig-CloudNative
   docker-anaconda-addon: sig-recycle
   docker-client-java: sig-CloudNative
   docker-compose: sig-CloudNative
   dogtail: Others
+  dolly: sig-ROS
   dolphin: sig-KDE
   dom4j: sig-Java
+  domain_bridge: sig-ROS
   doracms: sig-epol
   dos2unix: Base-service
   dosfstools: Storage
   dotconf: Programming-language
   double-conversion: Computing
   dovecot: Application
   doxygen: Application
@@ -1291,14 +1386,15 @@
   dracut: Base-service
   drbd: sig-Ha
   dropwatch: Networking
   drpm: Base-service
   druid: bigdata
   dsoftbus: sig-embedded
   dtc: Base-service
+  dtkcommon: sig-DDE
   dtkcore: sig-DDE
   dtkcore2: sig-DDE
   dtkgui: sig-DDE
   dtkwidget: sig-DDE
   dtkwidget2: sig-DDE
   dtkwm: sig-DDE
   duktape: Base-service
@@ -1306,22 +1402,25 @@
   dump: Storage
   duplicity: sig-UKUI
   dust: Application
   dvdplusrw-tools: Others
   dwarves: sig-high-performance-network
   dwz: Base-service
   dynamic_reconfigure: sig-ROS
+  dynamixel-workbench: sig-ROS
+  dynamixel-workbench-msgs: sig-ROS
   dyninst: Computing
   e2fsprogs: Storage
   eagle: sig-power-efficient
   easy-checker: sig-EasyLife
   easymock: sig-Java
   ebook-tools: sig-KDE
   ebtables: Networking
   ecj: dev-utils
+  ecl_tools: sig-ROS
   eclipse: sig-Java
   eclipse-cdt: sig-Java
   eclipse-ecf: sig-Java
   eclipse-egit: sig-Java
   eclipse-emf: sig-Java
   eclipse-gef: sig-Java
   eclipse-jgit: sig-Java
@@ -1353,14 +1452,16 @@
   eglexternalplatform: Programming-language
   ehcache-core: sig-Java
   ehcache-parent: sig-Java
   ehcache-sizeof-agent: sig-Java
   eigen: ai
   eigen3: sig-epol
   eigen3_cmake_module: sig-ROS
+  eigen_stl_containers: sig-ROS
+  eigenpy: sig-ROS
   elfutils: Base-service
   eli5: ai
   elinks: Application
   elixir: Application
   emacs: Desktop
   emacs-auctex: Others
   embedded-kernel: sig-embedded
@@ -1372,14 +1473,15 @@
   engrampa: sig-UKUI
   enscript: Application
   ensmallen: ai
   entr: System-tool
   environment-modules: Base-service
   eog: GNOME
   eom: sig-mate-desktop
+  ephemeral-port-reserve: sig-python-modules
   epiphany: Desktop
   epstool: bigdata
   epydoc: Base-service
   erlang: Programming-language
   erlang-eflame: Programming-language
   erlang-erlsyslog: Programming-language
   erlang-erlydtl: Programming-language
@@ -1402,14 +1504,16 @@
   ethercat-igh: sig-industrial-control
   ethtool: Networking
   etmem: Storage
   eunomia-bpf: sig-ebpf
   evince: GNOME
   evo-inflector: sig-Java
   evolution-data-server: Desktop
+  example_interfaces: sig-ROS
+  examples: sig-ROS
   exec-maven-plugin: sig-Java
   execstack: sig-Ha
   executive_smach: sig-ROS
   exempi: Base-service
   exfat-utils: Application
   exfatprogs: Application
   exim: Application
@@ -1445,16 +1549,19 @@
   fcgi: dev-utils
   fcitx: Desktop
   fcitx-cloudpinyin: Desktop
   fcitx-configtool: Desktop
   fcitx-libpinyin: Desktop
   fcitx-qt5: Desktop
   fcitx-sunpinyin: Desktop
+  fcl: sig-ROS
   fcoe-utils: System-tool
   fdupes: Application
+  feathernotes: sig-desktop-apps
+  featherpad: sig-desktop-apps
   feedbackd: GNOME
   felix-bundlerepository: sig-Java
   felix-framework: sig-Java
   felix-gogo-command: sig-Java
   felix-gogo-parent: sig-Java
   felix-gogo-runtime: Application
   felix-gogo-shell: Application
@@ -1480,40 +1587,47 @@
   ffmpegthumbnailer: Desktop
   fftw: Runtime
   fftw2: Application
   figlet: dev-utils
   file: Storage
   file-roller: GNOME
   filebench: Storage
+  filemanagement_dfs_service: sig-distributed-middleware
   filesystem: Storage
   filter: sig-ROS
+  filters: sig-ROS
+  find-object: sig-ROS
   findbugs: sig-Java
   findbugs-bcel: sig-Java
   findutils: Base-service
   fio: Application
   fipscheck: Base-service
   firebird: DB
   firefox: Application
   firesim: sig-RISC-V
   firewalld: Networking
   fish: Desktop
+  fisher: ecopkg
   flac: Computing
   flamegraph: sig-ops
   flang: Compiler
+  flann: sig-ROS
   flatbuffers: dev-utils
   flatpak: Programming-language
   flatpak-builder: GNOME
   flex: Base-service
   flexiblas: sig-epol
   flink: bigdata
   flite: Others
   fltk: Desktop
   fluid-soundfont: Private
   fluidsynth: Application
   flume: bigdata
+  fmi_adapter: sig-ROS
+  fmilibrary_vendor: sig-ROS
   fmpp: Application
   fmt: dev-utils
   folks: GNOME
   folks-telepathy: Private
   fontawesome-fonts: System-tool
   fontconfig: Desktop
   fontforge: Application
@@ -1526,14 +1640,17 @@
   fop: sig-Java
   forbidden-apis: Application
   foreman: sig-ops
   foreman-installer: sig-ops
   foreman-proxy: sig-ops
   foreman-selinux: sig-ops
   forge-parent: Application
+  formiko: sig-desktop-apps
+  foros: sig-ROS
+  four_wheel_steering_msgs: sig-ROS
   fpaste: Base-service
   fping: dev-utils
   fprintd: System-tool
   freeglut: Runtime
   freeimage: dev-utils
   freeipa: oVirt
   freeipmi: System-tool
@@ -1569,31 +1686,36 @@
   gala-anteater: sig-ops
   gala-gopher: sig-ebpf
   gala-spider: sig-ops
   galera: Others
   game-music-emu: dev-utils
   gamemode: Desktop
   gamin: sig-recycle
+  gammaray: sig-desktop-apps
   ganglia: Base-service
   garcon: xfce
   gavl: Others
   gawk: Base-service
   gazebo: sig-ROS
+  gazebo_ros2_control: sig-ROS
   gazebo_ros_pkgs: sig-ROS
   gazelle: sig-high-performance-network
   gazelle-cni: sig-recycle
   gc: Base-service
+  gc_spl: sig-ROS
   gcab: GNOME
   gcc: Compiler
   gcc-12: Compiler
+  gcc-7: Compiler
   gcc-cross: Compiler
   gcc-for-openEuler: Compiler
   gcc_secure: Others
   gcolor2: sig-mate-desktop
   gcr: Desktop
+  gcr4: GNOME
   gd: Desktop
   gdal: Application
   gdb: Computing
   gdbm: Storage
   gdbus-codegen-glibmm: sig-KIRAN-DESKTOP
   gdcm: sig-epol
   gdisk: Storage
@@ -1606,24 +1728,28 @@
   gecode: sig-epol
   gedit: GNOME
   gedit-control-your-tabs: GNOME
   gegl04: Others
   gemini-blueprint: Base-service
   gencpp: sig-ROS
   genders: Application
+  gendesk: sig-desktop-apps
+  generate_parameter_library: sig-ROS
   geneus: sig-ROS
   genlisp: sig-ROS
   genmsg: sig-ROS
   gennodejs: sig-ROS
   genpy: sig-ROS
   genwqe-tools: Application
   geoclue2: Desktop
   geocode-glib: Desktop
+  geographic_info: sig-ROS
   geolatte-geom: DB
   geolite2: sig-recycle
+  geometric_shapes: sig-ROS
   geometry: sig-ROS
   geometry2: sig-ROS
   geometry_tutorials: sig-ROS
   geos: dev-utils
   geronimo-annotation: sig-Java
   geronimo-commonj: sig-Java
   geronimo-ejb: dev-utils
@@ -1648,14 +1774,15 @@
   ghostscript: Base-service
   gi-docgen: GNOME
   giflib: Desktop
   gigolo: xfce
   gimp: Others
   gio-qt: Desktop
   giraph: bigdata
+  girara: sig-desktop-apps
   git: Base-service
   git-cola: dev-utils
   git-lfs: dev-utils
   git-review: dev-utils
   git-secret: dev-utils
   git-tools: dev-utils
   gjs: Desktop
@@ -1775,28 +1902,30 @@
   gnome-vfs2: GNOME
   gnome-video-effects: GNOME
   gnome-weather: GNOME
   gnu-efi: Programming-language
   gnu-free-fonts: Desktop
   gnu-getopt: sig-Java
   gnulib: Base-service
+  gnumeric: sig-desktop-apps
   gnupg: Application
   gnupg2: sig-security-facility
   gnuplot: Application
   gnustep-base: sig-epol
   gnustep-make: sig-epol
   gnutls: sig-security-facility
   go-bindata: sig-high-performance-network
   go-compilers: sig-recycle
   go-ovirt-engine-sdk4: oVirt
   go-rpm-macros: sig-K8sDistro
   go-srpm-macros: sig-K8sDistro
   goaccess: Application
   gobject-introspection: Base-service
   goebpf: sig-ebpf
+  goffice: sig-desktop-apps
   golang: sig-golang
   golang-github-coreos-go-iptables: sig-recycle
   golang-github-cpuguy83-go-md2man: sig-recycle
   golang-github-d2g-dhcp4: sig-recycle
   golang-github-fsnotify-fsnotify: sig-recycle
   golang-github-go-tomb-tomb: sig-recycle
   golang-github-golang-sys: sig-recycle
@@ -1810,62 +1939,71 @@
   golang-googlecode-goprotobuf: sig-recycle
   golang-googlecode-net: sig-recycle
   golang-googlecode-text: sig-recycle
   golang-googlecode-tools: sig-recycle
   golang-gopkg-yaml: sig-recycle
   gom: GNOME
   google-api-core: sig-openstack
-  google-api-python-client: sig-python-modules
+  google-api-python-client: sig-openstack
   google-auth-httplib2: sig-openstack
   google-croscore-fonts: Desktop
   google-crosextra-carlito-fonts: Application
   google-droid-fonts: Desktop
   google-gson: dev-utils
   google-guice: sig-Java
   google-http-java-client: sig-Java
   google-noto-cjk-fonts: Desktop
   google-noto-emoji-fonts: Desktop
   google-noto-fonts: Desktop
   google-oauth-java-client: sig-Java
   google-roboto-slab-fonts: Application
+  google_benchmark: sig-ROS
   google_benchmark_vendor: sig-ROS
   googleapis-common-protos: sig-openstack
   googletest: sig-ROS
   goversioninfo: sig-K8sDistro
   gpac: sig-epol
   gpars: sig-Java
   gparted: sig-mate-desktop
   gpdb: DB
   gperf: Programming-language
   gperftools: Computing
   gpgme: Base-service
   gphoto2: Base-service
   gpm: Desktop
+  gps_umd: sig-ROS
   gpsd: sig-KDE
   gradle: sig-Java
   grafana: Application
+  granite: sig-desktop-apps
   grantlee: sig-UKUI
   grantlee-qt5: sig-UKUI
+  graph_msgs: sig-ROS
   graphene: GNOME
   graphite2: Desktop
   graphviz: Desktop
+  grasping_msgs: sig-ROS
+  grbl_msgs: sig-ROS
+  grbl_ros: sig-ROS
   greatsql: DB
   grep: Base-service
+  grid_map: sig-ROS
   grilo: Desktop
   grilo-plugins: GNOME
   grizzly: dev-utils
   grizzly-npn: sig-Java
   groff: Base-service
   gromacs: Application
   groovy: sig-Java
   groovy18: sig-Java
   grpc: Networking
   grub2: sig-OS-Builder
   grubby: Base-service
   gsbase: sig-Java
+  gscam: sig-ROS
   gsettings-desktop-schemas: Desktop
   gsettings-qt: sig-UKUI
   gshhg-gmt-nc4: Application
   gsl: Runtime
   gsm: Desktop
   gsoap: Application
   gsound: GNOME
@@ -1890,28 +2028,30 @@
   gtk-vnc: GNOME
   gtk2: Desktop
   gtk2-engines: sig-mate-desktop
   gtk3: Desktop
   gtk4: Others
   gtkmm24: dev-utils
   gtkmm30: Others
+  gtksourceview2: sig-desktop-apps
   gtksourceview3: Others
   gtksourceview4: sig-mate-desktop
   gtksourceview5: GNOME
   gtkspell: sig-recycle
   gtkspell3: dev-utils
   gtkspellmm30: dev-utils
   gts: sig-ROS
   guacamole: Networking
   guava: dev-utils
   guava20: sig-Java
   gubbi-fonts: Desktop
   gucharmap: sig-mate-desktop
   guile: Desktop
   gumbo-parser: sig-UKUI
+  gummi: sig-desktop-apps
   gupnp: Programming-language
   gupnp-av: Base-service
   gupnp-dlna: GNOME
   gupnp-igd: Programming-language
   gutenprint: System-tool
   gv: Desktop
   gvfs: Desktop
@@ -1921,27 +2061,29 @@
   gz-common: sig-ROS
   gz-fuel-tools: sig-ROS
   gz-math: sig-ROS
   gz-msgs: sig-ROS
   gz-tools: sig-ROS
   gz-transport: sig-ROS
   gz-utils: sig-ROS
+  gz_ros2_control: sig-ROS
   gzip: Base-service
   h2: DB
   ha-api: sig-Ha
   ha-web: sig-Ha
   hadoop: bigdata
   hadoop-3.1: bigdata
   hamcrest: dev-utils
   haproxy: System-tool
   haproxy_exporter: sig-CloudNative
   harbor: sig-CloudNative
   hardinfo: dev-utils
   hardlink: sig-recycle
   harfbuzz: Desktop
+  hash_library_vendor: sig-ROS
   haveged: Base-service
   hawtbuf: sig-Java
   hawtdispatch: dev-utils
   hawtjni: sig-Java
   hawtjni-runtime: Private
   hazelcast: Application
   hbase: bigdata
@@ -1950,14 +2092,15 @@
   hdf5: Runtime
   hdparm: Storage
   hello: dev-utils
   help2man: Programming-language
   hesiod: sig-recycle
   hessian: sig-Java
   hexedit: Base-service
+  hey5_description: sig-ROS
   hfsplus-tools: Others
   hibernate: sig-Java
   hibernate-commons-annotations: sig-Java
   hibernate-jpa: sig-Java
   hibernate-jpa-2.0-api: sig-Java
   hibernate-jpa-2.1-api: sig-Java
   hibernate-search: sig-Java
@@ -1966,17 +2109,22 @@
   hibernate4: sig-Java
   hicolor-icon-theme: Desktop
   highlight: oVirt
   hikptool: sig-WayCa
   hiredis: Base-service
   hive: bigdata
   hivex: System-tool
+  hiviewdfx_hilog: sig-distributed-middleware
+  hiviewdfx_hisysevent: sig-distributed-middleware
+  hls_lfcd_lds_driver: sig-ROS
+  hmdfs: sig-distributed-middleware
   hostname: Networking
   hping: dev-utils
   hplip: System-tool
+  hpp-fcl: sig-ROS
   hppc: Base-service
   hsak: Storage
   hspell: Application
   hsqldb: sig-Java
   hsqldb1: Application
   htmlcxx: Desktop
   htop: dev-utils
@@ -2179,62 +2327,69 @@
   ibus-table-array30: Desktop
   ibus-table-chinese: Desktop
   ibus-theme-tools: Desktop
   ibus-typing-booster: Desktop
   icc-profiles-openicc: Application
   iceberg: bigdata
   icedtea-web: Compiler
+  iceoryx: sig-ROS
   icfg: Networking
   icon-naming-utils: Desktop
   icoutils: Others
   icu: Base-service
   icu4j: sig-Java
   id3lib: sig-epol
   idlj-maven-plugin: sig-Java
   idm-console-framework: Application
+  ifm3d-release: sig-ROS
   iftop: dev-utils
   igh-ethercat-xenomai: sig-industrial-control
   ignite: bigdata
   ignition: sig-K8sDistro
+  ignition_cmake2_vendor: sig-ROS
+  ignition_math6_vendor: sig-ROS
   iio-sensor-proxy: Application
   ilmbase: Programming-language
   im-chooser: sig-mate-desktop
   ima-evm-utils: Base-service
   imageTailor: sig-OS-Builder
   image_common: sig-ROS
   image_pipeline: sig-ROS
   image_transport: sig-ROS
   image_transport_plugins: sig-ROS
   imake: Desktop
   imgbased: oVirt
   imlib2: sig-UKUI
   impala: bigdata
   imsettings: Desktop
+  imu_tools: sig-ROS
   imwheel: sig-UKUI
   incubator-mxnet: ai
   indent: Application
   indicator-china-weather: sig-UKUI
   infiniband-diags: sig-recycle
   infinispan: sig-Java
   influxdb_exporter: sig-CloudNative
   inih: dev-utils
   iniparser: dev-utils
   initial-setup: System-tool
   initscripts: Networking
   inotify-tools: Application
+  input-pad: sig-desktop-apps
   inst-source-utils: sig-perl-modules
   install-scripts: sig-OS-Builder
   intel-cmt-cat: Programming-language
   intel-device-plugins-for-kubernetes: sig-confidential-computing
   intel-sgx-ssl: sig-confidential-computing
   interactive_markers: sig-ROS
   internal-issue: Private
   intltool: Programming-language
   invokebinder: sig-Java
   inxi: sig-cinnamon
+  iodine: Networking
   ioping: Application
   ioprocess: oVirt
   iotop: Storage
   iowatcher: sig-recycle
   iozone: dev-utils
   ipcalc: Networking
   iperf2: Application
@@ -2248,14 +2403,15 @@
   iptraf-ng: Networking
   iptstate: Networking
   iputils: Networking
   ipvsadm: Networking
   ipwatchd: dev-utils
   ipxe: sig-OS-Builder
   ipython: Private
+  iqtree: sig-bio
   irclib: sig-Java
   ironjacamar: sig-Java
   irqbalance: Computing
   irrXML: Private
   irrlicht: Others
   irssi: Application
   isa-l: dev-utils
@@ -2477,14 +2633,16 @@
   joda-time: sig-Java
   johnzon: sig-Java
   joint_state_publisher: sig-ROS
   jomolhari-fonts: Desktop
   joni: dev-utils
   jopt-simple: dev-utils
   jose: Base-service
+  joy_tester: sig-ROS
+  joystick_drivers: sig-ROS
   jpegoptim: Application
   jq: Base-service
   jruby: sig-ruby
   js-excanvas: dev-utils
   js-jquery: sig-nodejs
   js-jquery1: sig-recycle
   js-jquery2: sig-recycle
@@ -2529,14 +2687,15 @@
   k3s-containerd: sig-K8sDistro
   k3s-plugins: sig-K8sDistro
   k3s-selinux: sig-K8sDistro
   kabi-dw: Kernel
   kaccounts-integration: sig-KDE
   kacst-fonts: Desktop
   kactivitymanagerd: sig-KDE
+  kaddressbook: sig-KDE
   kae_driver: sig-AccLib
   kafka: bigdata
   kafka-python: sig-openstack
   kata-containers: sig-CloudNative
   kata-micro-kernel: sig-recycle
   kata_integration: sig-CloudNative
   kate: sig-KDE
@@ -2550,48 +2709,58 @@
   kconfigDetector: Kernel
   kcron: sig-KDE
   kde-cli-tools: sig-KDE
   kde-connect: sig-KDE
   kde-filesystem: System-tool
   kde-settings: Desktop
   kdecoration: sig-KDE
+  kdegraphics-mobipocket: sig-KDE
+  kdepim-runtime: sig-KDE
   kdevelop: sig-KDE
   kdevelop-pg-qt: sig-KDE
   kdevelopkdevelop-pg-qt: sig-KDE
+  kdiagram: sig-KDE
   kdl_parser: sig-ROS
   kdnssd: sig-KDE
   kdsoap: sig-KDE
   kdump-anaconda-addon: Base-service
+  kea: Networking
   keditbookmarks: sig-KDE
   keepalived: Networking
   kernel: Kernel
   kexec-tools: Base-service
   keybinder: xfce
   keybinder3: Desktop
+  keyboard_handler: sig-ROS
   keycloak-httpd-client-install: sig-security-facility
   keyrings-filesystem: Others
   keyutils: sig-security-facility
   kf5: sig-KDE
+  kf5-akonadi-calendar: sig-KDE
   kf5-akonadi-contacts: sig-KDE
   kf5-akonadi-mime: sig-KDE
   kf5-akonadi-notes: sig-KDE
   kf5-akonadi-search: sig-KDE
   kf5-akonadi-server: sig-KDE
   kf5-attica: sig-KDE
   kf5-baloo: sig-KDE
   kf5-bluez-qt: sig-KDE
+  kf5-calendarsupport: sig-KDE
+  kf5-eventviews: sig-KDE
   kf5-frameworkintegration: sig-KDE
   kf5-grantleetheme: sig-KDE
+  kf5-incidenceeditor: sig-KDE
   kf5-kactivities: sig-KDE
   kf5-kactivities-stats: sig-KDE
   kf5-kapidox: sig-KDE
   kf5-karchive: sig-KDE
   kf5-kauth: sig-KDE
   kf5-kbookmarks: sig-KDE
   kf5-kcalendarcore: sig-KDE
+  kf5-kcalendarutils: sig-KDE
   kf5-kcmutils: sig-KDE
   kf5-kcodecs: sig-KDE
   kf5-kcompletion: sig-KDE
   kf5-kconfig: sig-KDE
   kf5-kconfigwidgets: sig-KDE
   kf5-kcontacts: sig-KDE
   kf5-kcoreaddons: sig-KDE
@@ -2644,24 +2813,27 @@
   kf5-kquickcharts: sig-KDE
   kf5-kross: sig-KDE
   kf5-krunner: sig-KDE
   kf5-kservice: sig-KDE
   kf5-ksmtp: sig-KDE
   kf5-ktexteditor: sig-KDE
   kf5-ktextwidgets: sig-KDE
+  kf5-ktnef: sig-KDE
   kf5-kunitconversion: sig-KDE
   kf5-kwallet: sig-KDE
   kf5-kwayland: sig-KDE
   kf5-kwidgetsaddons: sig-KDE
   kf5-kwindowsystem: sig-KDE
   kf5-kxmlgui: sig-KDE
   kf5-kxmlrpcclient: sig-KDE
   kf5-libgravatar: sig-KDE
   kf5-libkdepim: sig-KDE
+  kf5-libkexiv2: sig-KDE
   kf5-libkleo: sig-KDE
+  kf5-libksieve: sig-KDE
   kf5-mailcommon: sig-KDE
   kf5-mailimporter: sig-KDE
   kf5-messagelib: sig-KDE
   kf5-modemmanager-qt: sig-KDE
   kf5-networkmanager-qt: sig-KDE
   kf5-pimcommon: sig-KDE
   kf5-plasma: sig-KDE
@@ -2672,15 +2844,17 @@
   kf5-syndication: sig-KDE
   kf5-syntax-highlighting: sig-KDE
   kf5-threadweaver: sig-KDE
   khelpcenter: sig-KDE
   khmeros-fonts: System-tool
   khotkeys: sig-KDE
   kim-api: Application
+  kinematics_interface: sig-ROS
   kio-extras: sig-KDE
+  kiran-authentication-devices: sig-KIRAN-DESKTOP
   kiran-authentication-service: sig-KIRAN-DESKTOP
   kiran-avatar-editor: sig-KIRAN-DESKTOP
   kiran-biometrics: sig-KIRAN-DESKTOP
   kiran-calculator: sig-KIRAN-DESKTOP
   kiran-calendar: sig-KIRAN-DESKTOP
   kiran-cc-daemon: sig-KIRAN-DESKTOP
   kiran-control-panel: sig-KIRAN-DESKTOP
@@ -2702,39 +2876,45 @@
   kiran-panel: sig-KIRAN-DESKTOP
   kiran-qdbusxml2cpp: sig-KIRAN-DESKTOP
   kiran-qt5-integration: sig-KIRAN-DESKTOP
   kiran-screensaver: sig-KIRAN-DESKTOP
   kiran-screensaver-dialog: sig-KIRAN-DESKTOP
   kiran-session-guard: sig-KIRAN-DESKTOP
   kiran-session-manager: sig-KIRAN-DESKTOP
+  kiran-shell: sig-KIRAN-DESKTOP
   kiran-tests: sig-KIRAN-DESKTOP
   kiran-themes: sig-KIRAN-DESKTOP
   kiran-wallpapers: sig-KIRAN-DESKTOP
   kiran-widgets-qt5: sig-KIRAN-DESKTOP
   kite-sdk: bigdata
   kiwi: Base-service
   kiwi-dlimage: Private
   kiwi-template-openEuler: Private
+  kmail: sig-KDE
   kmenuedit: sig-KDE
   kmod: Computing
   kmod-drbd90: sig-Ha
   kmod-kvdo: Runtime
   kmodtool: dev-utils
   knox: bigdata
+  kobuki_ros_interfaces: sig-ROS
+  kobuki_velocity_smoother: sig-ROS
   kohsuke-pom: Application
   konsole5: sig-KDE
   kontact: sig-KDE
+  korganizer: sig-KDE
   kpatch: Base-service
   krb5: Base-service
   kronosnet: Networking
   kryo: sig-Java
   ksc-defender: sig-security-facility
   kscreenlocker: sig-KDE
   ksh: Base-service
   ksystemstats: sig-KDE
+  kuasar: sig-CloudNative
   kubeedge: sig-Edge
   kubekey: sig-K8sDistro
   kubernetes: sig-CloudNative
   kubevirt: sig-CloudNative
   kudu: bigdata
   kunpengsecl: sig-security-facility
   kurdit-unikurd-web-fonts: Desktop
@@ -2763,42 +2943,50 @@
   kylin-weather: sig-UKUI
   kyotocabinet: Others
   kyua: Base-service
   labltk: Programming-language
   ladspa: dev-utils
   lame: Others
   lammps: sig-HPC
+  lanelet2: sig-ROS
   langpacks: sig-recycle
   langtable: Base-service
   language-detector: sig-Java
   lapack: Programming-language
+  lasem: sig-desktop-apps
   laser_assembler: sig-ROS
   laser_filters: sig-ROS
   laser_geometry: sig-ROS
   laser_pipeline: sig-ROS
+  laser_proc: sig-ROS
   lasso: Base-service
   lastpass-cli: Application
   latex2html: Others
   latexmk: sig-perl-modules
   lato-fonts: Desktop
   latrace: sig-recycle
   launch: sig-ROS
+  launch_pal: sig-ROS
+  launch_param_builder: sig-ROS
   launch_ros: sig-ROS
   layer-shell-qt: sig-KDE
   lcdf-typetools: Application
   lcms2: Desktop
   lcov: Base-service
   lcr: iSulad
   ldapjdk: dev-utils
   ldaptive: sig-Java
   ldns: Networking
   ldtp: sig-KIRAN-DESKTOP
   leatherman: Base-service
   ledmon: Application
   lensfun: dev-utils
+  leo_common-ros2: sig-ROS
+  leo_desktop-ros2: sig-ROS
+  leo_robot-ros2: sig-ROS
   leptonica: Base-service
   less: Base-service
   lettuce: sig-Java
   leveldb: System-tool
   leveldb-java: sig-Java
   leveldbjni: sig-Java
   lftp: Networking
@@ -2851,14 +3039,15 @@
   libart_lgpl: Desktop
   libass: Application
   libassuan: Networking
   libasyncns: Desktop
   libatasmart: Desktop
   libatomic_ops: Computing
   libavc1394: Runtime
+  libb2: sig-UKUI
   libblockdev: Storage
   libbluray: Desktop
   libbonobo: Desktop
   libbonoboui: Desktop
   libboundscheck: Base-service
   libbpf: sig-ebpf
   libbs2b: Application
@@ -2869,37 +3058,40 @@
   libcaca: sig-epol
   libcacard: Desktop
   libcanberra: Desktop
   libcap: sig-security-facility
   libcap-ng: Base-service
   libcareplus: Virt
   libcbor: Base-service
+  libccd: sig-ROS
   libcddb: sig-epol
   libcdio: Desktop
   libcdio-paranoia: Desktop
   libcec: sig-epol
   libcgroup: sig-CloudNative
   libchamplain: GNOME
   libchewing: sig-KDE
   libclc: Base-service
   libcloudproviders: GNOME
+  libcoap: sig-distributed-middleware
   libcomps: Base-service
   libconfig: Base-service
   libconfuse: Base-service
   libcroco: sig-recycle
   libcrystalhd: sig-UKUI
   libcue: Desktop
   libcutl: sig-KIRAN-DESKTOP
   libcxx: Compiler
   libcxx-15: Compiler
   libcxxabi: Compiler
   libcxxabi-15: Compiler
   libcyaml: Base-service
   libdaemon: Base-service
   libdap: sig-recycle
+  libdatovka: sig-desktop-apps
   libdatrie: Base-service
   libdazzle: Desktop
   libdb: Base-service
   libdbi: Base-service
   libdbusextended-qt5: Desktop
   libdbusmenu: Programming-language
   libdc1394: sig-epol
@@ -2942,14 +3134,15 @@
   libffado: sig-compat-winapp
   libffi: Base-service
   libfm: xfce
   libfontenc: Desktop
   libfprint: sig-UKUI
   libfreenect: sig-epol
   libftdi: sig-embedded
+  libg2o-release: sig-ROS
   libgadu: Application
   libgcrypt: Networking
   libgdata: Desktop
   libgdiplus: Base-service
   libgdither: Others
   libgdl: GNOME
   libgee: Desktop
@@ -2966,14 +3159,15 @@
   libgnomecanvas: GNOME
   libgnomecanvasmm26: xfce
   libgnomekbd: GNOME
   libgnomeui: Others
   libgovirt: Others
   libgpg-error: Base-service
   libgphoto2: System-tool
+  libgringotts: sig-desktop-apps
   libgsasl: Application
   libgsf: Base-service
   libgssglue: dev-utils
   libgta: dev-utils
   libgtop2: Desktop
   libgudev: Desktop
   libguess: Desktop
@@ -2985,14 +3179,15 @@
   libhandy: dev-utils
   libhangul: System-tool
   libharu: sig-epol
   libhbaapi: Base-service
   libhbalinux: Others
   libhdfs: bigdata
   libhugetlbfs: Computing
+  libhv: Base-service
   libibmad: sig-recycle
   libical: Base-service
   libid3tag: Others
   libidn: Base-service
   libidn2: Base-service
   libiec61883: Runtime
   libieee1284: Runtime
@@ -3016,14 +3211,15 @@
   libkcapi: Base-service
   libkeepalive: dev-utils
   libkefir: sig-recycle
   libkgapi: sig-KDE
   libkkc: Application
   libkkc-data: Private
   libkml: sig-recycle
+  libkolabxml: sig-KDE
   libkomparediff2: sig-KDE
   libksba: Base-service
   libkscreen-qt5: sig-UKUI
   libksysguard: sig-KDE
   libkylin-chkname: sig-UKUI
   libkysdk-applications: sig-UKUI
   libkysdk-base: sig-UKUI
@@ -3065,14 +3261,15 @@
   libmpeg2: Application
   libmpris-qt5: Desktop
   libmspack: Base-service
   libmtp: Application
   libmusicbrainz5: Application
   libmypaint: Others
   libmysofa: sig-epol
+  libnabo: sig-ROS
   libnatpmp: sig-epol
   libndp: Networking
   libnet: Networking
   libnetconf2: sig-industrial-control
   libnetfilter_conntrack: Networking
   libnetfilter_cthelper: Base-service
   libnetfilter_cttimeout: Base-service
@@ -3089,15 +3286,15 @@
   libntlm: Application
   libnvme: System-tool
   liboauth: Base-service
   libofa: sig-recycle
   libogg: Computing
   liboggz: sig-recycle
   liboil: sig-recycle
-  libomp: Private
+  libomp: sig-ROS
   libomxil-bellagio: Base-service
   libopenmpt: sig-epol
   libopenraw: Others
   libosinfo: Base-service
   libotf: System-tool
   libpanel: GNOME
   libpaper: Base-service
@@ -3106,14 +3303,15 @@
   libpeas: GNOME
   libpfm: Programming-language
   libpinyin: Others
   libpipeline: Base-service
   libplist: Base-service
   libpng: Base-service
   libpng12: sig-recycle
+  libpointmatcher: sig-ROS
   libportal: GNOME
   libpq: DB
   libproxy: Networking
   libpsl: Base-service
   libpwquality: sig-security-facility
   libqalculate: sig-KDE
   libqb: Computing
@@ -3121,14 +3319,15 @@
   libqtxdg: sig-UKUI
   libquvi: Base-service
   libquvi-scripts: Base-service
   librabbitmq: Runtime
   libraqm: Desktop
   libraw1394: System-tool
   librdkafka: Programming-language
+  librealsense: sig-ROS
   librelp: Programming-language
   librepo: Base-service
   libreport: Base-service
   libreswan: System-tool
   librevenge: dev-utils
   librpcsecgss: dev-utils
   librsvg2: Desktop
@@ -3203,14 +3402,15 @@
   liburing: Storage
   libusb: Storage
   libusbmuxd: Storage
   libusbx: Storage
   libuser: Base-service
   libutempter: Base-service
   libuv: Programming-language
+  libuvc: sig-ROS
   libva: Runtime
   libvarlink: sig-CloudNative
   libvdpau: Runtime
   libverto: Base-service
   libvirt: Virt
   libvirt-dbus: Virt
   libvirt-glib: Virt
@@ -3254,14 +3454,15 @@
   libyang: sig-high-performance-network
   libyang1: sig-industrial-control
   libytnef: sig-UKUI
   libyubikey: dev-utils
   libzapojit: Others
   libzen: Desktop
   libzip: Programming-language
+  libzmq: sig-ROS
   lightcouch: sig-Java
   lightdm: Desktop
   lightdm-gtk: Desktop
   lightdm-gtk-greeter: sig-recycle
   lightdm-kiran-greeter: sig-KIRAN-DESKTOP
   lightgbm: ai
   lighttpd: Networking
@@ -3293,14 +3494,15 @@
   llvm-libunwind: Compiler
   llvm-libunwind-15: Compiler
   llvm-mlir: Compiler
   lm_sensors: Computing
   lmbench: dev-utils
   lmdb: Base-service
   lmfit: Application
+  locator_ros_bridge: sig-ROS
   loci: sig-openstack
   lockdev: Computing
   lodash: sig-nodejs
   log4cplus: dev-utils
   log4cpp: dev-utils
   log4j: sig-Java
   log4j-jboss-logmanager: sig-Java
@@ -3320,20 +3522,22 @@
   lohit-odia-fonts: Application
   lohit-tamil-fonts: Application
   lohit-telugu-fonts: Application
   lorax: sig-OS-Builder
   low-memory-monitor: Desktop
   lpg: Application
   lrzsz: Application
+  lsc_ros2_driver: sig-ROS
   lshw: Base-service
   lshw-B.02.18: sig-recycle
   lsof: Base-service
   lsscsi: Storage
   lsyncd: Application
   ltrace: Programming-language
+  lttng-tools: sig-ROS
   lttng-ust: Computing
   lua: Base-service
   lua-expat: Base-service
   lua-filesystem: Programming-language
   lua-json: Base-service
   lua-lpeg: Base-service
   lua-lunit: Programming-language
@@ -3344,16 +3548,16 @@
   luarocks: sig-OpenResty
   lucene: sig-Java
   lucene3: sig-Java
   lucene4: sig-Java
   lucenepp: Desktop
   luksmeta: Storage
   lunar-date: sig-KIRAN-DESKTOP
+  lusb: sig-ROS
   lustre: sig-SDS
-  lustre-e2fsprogs: sig-SDS
   lutok: Base-service
   lv2: sig-epol
   lvm2: Storage
   lwip: sig-high-performance-network
   lxappearance: xfce
   lxc: iSulad
   lxcfs: iSulad
@@ -3368,27 +3572,31 @@
   lxpanel: xfce
   lxqt-build-tools: sig-UKUI
   lxsession: Desktop
   lxshortcut: xfce
   lxtask: xfce
   lxterminal: xfce
   lynx: Application
+  lyx: sig-desktop-apps
   lz4: Base-service
   lz4-java: sig-Java
   lzip: bigdata
   lzma: sig-recycle
   lzma-java: sig-Java
   lzo: Base-service
   lzop: Base-service
+  m1600-driver: sig-Compatibility-Infra
   m17n-db: System-tool
   m17n-lib: System-tool
   m2crypto: Runtime
   m4: Base-service
   mac-robber: Others
   madan-fonts: Desktop
+  mafft: sig-bio
+  magic_enum: sig-ROS
   mahout: bigdata
   mailcap: Base-service
   maildrop: Application
   mailman: Application
   mailx: Desktop
   mainline.list: Private
   make: Base-service
@@ -3400,20 +3608,23 @@
   maliit-keyboard: sig-KDE
   mallard-rng: Programming-language
   man-db: Base-service
   man-pages: Base-service
   man2html: sig-epol
   mandoc: sig-epol
   mapserver: Application
+  mapviz: sig-ROS
   marco: sig-mate-desktop
   mariadb: DB
   mariadb-connector-c: Base-service
   mariadb-connector-odbc: DB
   marisa: Others
   marked: sig-UKUI
+  marti_common: sig-ROS
+  marti_messages: sig-ROS
   masscan: sig-epol
   mate-applets: sig-mate-desktop
   mate-backgrounds: sig-mate-desktop
   mate-calc: sig-mate-desktop
   mate-common: sig-mate-desktop
   mate-control-center: sig-mate-desktop
   mate-desktop: sig-mate-desktop
@@ -3497,14 +3708,16 @@
   maven-surefire: sig-Java
   maven-verifier: sig-Java
   maven-verifier-plugin: Base-service
   maven-wagon: sig-Java
   maven-war-plugin: sig-Java
   maven2: sig-Java
   mavibot: sig-Java
+  mavlink-gbp-release: sig-ROS
+  mavros: sig-ROS
   mc: Application
   mcelog: Base-service
   mchange-commons: sig-Java
   mcpp: Base-service
   mcstrans: sig-security-facility
   mdadm: Storage
   mdb: dev-utils
@@ -3520,14 +3733,15 @@
   memcached: Application
   memcached_exporter: sig-CloudNative
   memkind: Computing
   memleax: dev-utils
   memoryfilesystem: sig-Java
   memtester: dev-utils
   memwatch: dev-utils
+  menge_vendor: sig-ROS
   menu-cache: xfce
   mercurial: Base-service
   mesa: Desktop
   mesa-demos: Runtime
   mesa-libGLU: Desktop
   mesa-libGLw: sig-recycle
   meson: Programming-language
@@ -3535,22 +3749,28 @@
   message_generation: sig-ROS
   message_runtime: sig-ROS
   metacity: Desktop
   metadata-extractor2: Application
   metainf-services: sig-Java
   metis: Application
   metrics: sig-Java
+  metslib: sig-ROS
+  mhash: sig-desktop-apps
   mhvtl: dev-utils
+  micro_ros_diagnostics: sig-ROS
+  micro_ros_msgs: sig-ROS
   microcode_ctl: System-tool
+  microstrain_inertial: sig-ROS
   migration-assistant: sig-Migration
   mikmod: Application
   mimepull: sig-Java
   mimetic: Desktop
   mimick_vendor: sig-ROS
   mina-ftpserver: Application
+  minder: sig-desktop-apps
   mindspore: ai
   mingw-binutils: sig-compat-winapp
   mingw-crt: sig-compat-winapp
   mingw-filesystem: sig-compat-winapp
   mingw-gcc: sig-compat-winapp
   mingw-headers: sig-compat-winapp
   mingw-spice-vdagent: oVirt
@@ -3572,26 +3792,28 @@
   mm-common: GNOME
   mobile-broadband-provider-info: Networking
   moby: sig-CloudNative
   mocha: dev-utils
   mock: dev-utils
   mock-core-configs: dev-utils
   mockito: Programming-language
+  mod: sig-ROS
   mod_auth_gssapi: System-tool
   mod_auth_openidc: sig-security-facility
   mod_authnz_pam: sig-security-facility
   mod_fcgid: System-tool
   mod_http2: Networking
   mod_intercept_form_submit: Application
   mod_lookup_identity: Application
   mod_perl: sig-perl-modules
   mod_security: System-tool
   mod_security_crs: Base-service
   mod_wsgi: Application
   modello: Base-service
+  modeltest-ng: sig-bio
   mojarra: sig-Java
   mojo-parent: sig-Java
   mokutil: sig-security-facility
   mold: sig-RISC-V
   mom: oVirt
   mongo-c-driver: Others
   mongo-java-driver: sig-Java
@@ -3602,26 +3824,34 @@
   moosefs: sig-K8sDistro
   morfologik-stemming: Base-service
   morphia: dev-utils
   mosquitto: Application
   motif: Runtime
   mousepad: xfce
   mousetweaks: Application
+  moveit2: sig-ROS
+  moveit_msgs: sig-ROS
+  moveit_resources: sig-ROS
+  moveit_visual_tools: sig-ROS
   mozilla-filesystem: Desktop
   mozjs102: GNOME
   mozjs52: sig-recycle
   mozjs60: sig-recycle
   mozjs68: sig-recycle
   mozjs78: Desktop
   mp: sig-epol
   mpfr: Computing
   mpg123: sig-UKUI
   mpi4py: sig-epol
   mpich: Programming-language
   mpv: Desktop
+  mrbayes: sig-bio
+  mrpt: sig-ROS
+  mrpt_msgs: sig-ROS
+  mrt_cmake_modules: sig-ROS
   mrtg: Application
   msgpack-c: sig-epol
   mstflint: System-tool
   msv: Application
   mt-st: Others
   mtd-utils: sig-embedded
   mtdev: Base-service
@@ -3642,14 +3872,15 @@
   musescore: sig-desktop-apps
   musl: Computing
   mustache-java: sig-Java
   mutt: Application
   mutter: GNOME
   mvapich2: Programming-language
   mvel: Base-service
+  mvsim: sig-ROS
   mx4j: sig-Java
   mxml: Application
   mxparser: sig-Java
   mybatis: sig-Java
   mybatis-generator: sig-Java
   mybatis-parent: sig-Java
   mypaint-brushes: Others
@@ -3662,22 +3893,26 @@
   mythes: Application
   nafees-web-naskh-fonts: Desktop
   nagios: System-tool
   nagios-plugins: Networking
   nailgun: Base-service
   nano: Application
   nanomsg: DB
+  nao_button_sim: sig-ROS
+  nao_interfaces: sig-ROS
+  nao_lola: sig-ROS
   narayana: sig-Java
   nasm: Programming-language
   native-platform: sig-Java
   native-turbo: A-Tune
   nautilus: GNOME
   nautilus-sendto: Private
   nauty: sig-epol
   navigation: sig-ROS
+  navigation2: sig-ROS
   navigation_msgs: sig-ROS
   navilu-fonts: Desktop
   nbdkit: Others
   ncbi-blast: sig-bio
   nccl: ai
   ncdu: dev-utils
   ncompress: Base-service
@@ -3686,16 +3921,18 @@
   ndisc6: Networking
   neXtaw: dev-utils
   neethi: Networking
   nekohtml: Application
   nemo: sig-cinnamon
   nemo-extensions: sig-cinnamon
   neo4j: DB
+  neo_simulation2: sig-ROS
   neofetch: dev-utils
   neon: Programming-language
+  nerian_stereo_ros2: sig-ROS
   nestos-installer: sig-CloudNative
   net-snmp: Networking
   net-tools: Networking
   netavark: sig-CloudNative
   netcdf: dev-utils
   netcdf-cxx: sig-epol
   netcf: Networking
@@ -3725,15 +3962,19 @@
   nghttp2: Networking
   nginx: Packaging
   nilfs-utils: Others
   nim: Programming-language
   ninja-build: Programming-language
   nispor: oVirt
   nload: dev-utils
+  nlohmann_json: sig-ROS
+  nlohmann_json_schema_validator_vendor: sig-ROS
   nmap: Networking
+  nmea_hardware_interface: sig-ROS
+  nmea_msgs: sig-ROS
   nmon: dev-utils
   nmstate: oVirt
   nng: dev-utils
   node-gyp: sig-nodejs
   node_exporter: sig-CloudNative
   nodejs: sig-nodejs
   nodejs-abbrev: sig-nodejs
@@ -4095,45 +4336,53 @@
   nodejs-xtend: sig-nodejs
   nodejs-yamlish: sig-nodejs
   nodejs-yargs: sig-nodejs
   nodejs-yarn: oVirt
   nodejsporter: dev-utils
   nodelet_core: sig-ROS
   nodeunit: sig-nodejs
+  nodl: sig-ROS
+  nodl_to_policy: sig-ROS
   noggit: sig-Java
   notebook: bigdata
   notepadqq: Desktop
   notification-daemon: Networking
+  notification_common_event_service: sig-distributed-middleware
+  notification_eventhandler: sig-distributed-middleware
   nototools: Programming-language
+  novatel_gps_driver: sig-ROS
   novnc: sig-openstack
   npth: Computing
   nrpe: System-tool
   nsis-simple-service-plugin: oVirt
   nspr: Computing
   nss: sig-security-facility
   nss-altfiles: Application
   nss-mdns: Application
   nss-pam-ldapd: Base-service
   nss-pem: sig-security-facility
   nss_nis: Base-service
   nss_wrapper: Application
   ntfs-3g: Application
   ntp: Networking
+  ntpd_driver: sig-ROS
   ntpstat: Networking
+  ntrip_client: sig-ROS
   numactl: Computing
   numad: Computing
   numpy: Programming-language
   nv-codec-headers: Desktop
   nvidia-gpu-kernel-modules: sig-Compatibility-Infra
   nvme-cli: System-tool
   nvme-snsd: Storage
   nvmetcli: System-tool
   nvml: Programming-language
   nvwa: sig-ops
   oath-toolkit: sig-security-facility
+  object_recognition_msgs: sig-ROS
   objectweb-asm: Application
   objectweb-asm3: Application
   objectweb-pom: sig-Java
   objenesis: sig-Java
   obs-build: Others
   obs-bundled-gems: Others
   obs-env: Programming-language
@@ -4160,26 +4409,34 @@
   ocaml-ocamlbuild: Programming-language
   ocaml-ounit: Application
   ocaml-xml-light: dev-utils
   ocf: Storage
   oci-systemd-hook: sig-recycle
   ocl-icd: Base-service
   octave: ai
+  octomap: sig-ROS
+  octomap_mapping: sig-ROS
+  octomap_msgs: sig-ROS
+  octomap_ros: sig-ROS
+  octomap_rviz_plugins: sig-ROS
   oddjob: Base-service
   oec-application: sig-Compatibility-Infra
+  oec-cloud: sig-Compatibility-Infra
   oec-hardware: sig-Compatibility-Infra
   oemaker: sig-OS-Builder
+  oepkgs-release: sig-Compatibility-Infra
   ogdi: dev-utils
   ogre: sig-ROS
   ohc: sig-Java
   okhttp: ai
   okteta: sig-KDE
   okular: sig-KDE
   oldstandard-sfd-fonts: Application
   ompi: ai
+  ompl: sig-ROS
   onboard: Others
   oncn-bwm: sig-high-performance-network
   oneDAL: ai
   oneDNN: ai
   ongres-scram: dev-utils
   ongres-stringprep: sig-Java
   oniguruma: Base-service
@@ -4214,14 +4471,16 @@
   opencl-filesystem: ai
   opencl-headers: ai
   openconnect: Application
   opencore-amr: Desktop
   opencryptoki: dev-utils
   opencv: ai
   opendmarc: Base-service
+  openeuler-ros: sig-ROS
+  openfortivpn: Networking
   opengauss-dcf: DB
   opengauss-server: DB
   openhpi: System-tool
   openjade: Application
   openjdk-1.8.0: Compiler
   openjdk-11: Compiler
   openjdk-17: Compiler
@@ -4230,14 +4489,15 @@
   openjfx8: Compiler
   openjpa: sig-Java
   openjpeg: sig-recycle
   openjpeg2: Desktop
   openldap: Networking
   openmotif: Private
   openmpi: Application
+  openni: sig-ROS
   opennlp: Application
   opennn: ai
   openoffice-lv: Application
   openoffice.org-dict-cs_CZ: Application
   openpgm: dev-utils
   openpmix: ai
   openresty: sig-OpenResty
@@ -4257,20 +4517,25 @@
   opensm: Application
   opensp: Application
   openssh: Networking
   openssl: sig-security-facility
   openssl-pkcs11: sig-security-facility
   openssl_tpm2_engine: sig-security-facility
   openstack-aodh: sig-openstack
+  openstack-barbican: sig-openstack
   openstack-ceilometer: sig-openstack
   openstack-cinder: sig-openstack
+  openstack-cloudkitty: sig-openstack
   openstack-cyborg: sig-openstack
+  openstack-designate: sig-openstack
+  openstack-designate-ui: sig-openstack
   openstack-glance: sig-openstack
   openstack-heat: sig-openstack
   openstack-heat-agents: sig-openstack
+  openstack-heat-ui: sig-openstack
   openstack-helm: sig-openstack
   openstack-helm-images: sig-openstack
   openstack-helm-infra: sig-openstack
   openstack-horizon: sig-openstack
   openstack-ironic: sig-openstack
   openstack-ironic-inspector: sig-openstack
   openstack-ironic-python-agent: sig-openstack
@@ -4279,26 +4544,40 @@
   openstack-java-sdk: oVirt
   openstack-keystone: sig-openstack
   openstack-kolla: sig-openstack
   openstack-kolla-ansible: sig-openstack
   openstack-kolla-ansible-plugin: sig-openstack
   openstack-kolla-plugin: sig-openstack
   openstack-macros: sig-openstack
+  openstack-magnum-ui: sig-openstack
+  openstack-manila: sig-openstack
+  openstack-masakari: sig-openstack
+  openstack-mistral: sig-openstack
+  openstack-mistral-ui: sig-openstack
   openstack-neutron: sig-openstack
+  openstack-neutron-dynamic-routing: sig-openstack
+  openstack-neutron-vpnaas: sig-openstack
   openstack-nova: sig-openstack
+  openstack-octavia: sig-openstack
+  openstack-octavia-ui: sig-openstack
   openstack-panko: sig-openstack
   openstack-placement: sig-openstack
   openstack-plugin: sig-openstack
   openstack-rally: sig-openstack
   openstack-rally-plugins: sig-openstack
   openstack-releases: sig-openstack
+  openstack-sahara-ui: sig-openstack
+  openstack-senlin: sig-openstack
   openstack-swift: sig-openstack
   openstack-tempest: sig-openstack
   openstack-trove: sig-openstack
+  openstack-vitrage-ui: sig-openstack
+  openstack-zaqar: sig-openstack
   opentest4j: Application
+  openttd: sig-desktop-apps
   openvpn: Application
   openvswitch: Networking
   openvswitch-kmod: sig-recycle
   openwebbeans: sig-Java
   openwsman: System-tool
   optimized-routines: Compiler
   options: dev-utils
@@ -4306,30 +4585,34 @@
   opus: Computing
   opusfile: Others
   orage: sig-recycle
   orc: Base-service
   orca: Desktop
   origin: sig-K8sDistro
   orocos_kdl: sig-ROS
+  orocos_kdl_vendor: sig-ROS
   orocos_kinematics_dynamics: sig-ROS
   os-maven-plugin: sig-Java
   os-net-config: sig-openstack
   os-prober: Base-service
   osc: Others
   oscap-anaconda-addon: sig-security-facility
   osgi-annotation: sig-Java
   osgi-compendium: sig-Java
   osgi-core: sig-Java
   osinfo-db: Base-service
   osinfo-db-tools: Base-service
+  osmo: sig-desktop-apps
+  osqp_vendor: sig-ROS
   osrf_pycommon: sig-ROS
   osrf_testing_tools_cpp: sig-ROS
   ostree: Base-service
   ostree_assembly: sig-Ostree-Assembly
   otopi: oVirt
+  ouxt_common: sig-ROS
   overpass-fonts: System-tool
   ovirt-ansible-cluster-upgrade: oVirt
   ovirt-ansible-collection: oVirt
   ovirt-ansible-disaster-recovery: oVirt
   ovirt-ansible-engine-setup: oVirt
   ovirt-ansible-hosted-engine-setup: oVirt
   ovirt-ansible-image-template: oVirt
@@ -4389,14 +4672,18 @@
   p7zip: dev-utils
   pacemaker: sig-Ha
   pacemaker-mgmt: sig-Ha
   pakchois: Packaging
   paktype-naqsh-fonts: Desktop
   paktype-naskh-basic-fonts: Desktop
   paktype-tehreer-fonts: Desktop
+  pal_gazebo_plugins: sig-ROS
+  pal_gazebo_worlds: sig-ROS
+  pal_gripper: sig-ROS
+  pal_statistics: sig-ROS
   pam: sig-security-facility
   pam_krb5: Application
   pam_wrapper: sig-security-facility
   pango: Desktop
   pangomm: Programming-language
   pangox-compat: sig-mate-desktop
   papi: Programming-language
@@ -4419,34 +4706,38 @@
   patchelf: sig-embedded
   patchutils: Application
   pavucontrol: Application
   pax: Application
   pbzip2: Application
   pcaudiolib: Others
   pciutils: Storage
+  pcl: sig-ROS
   pcl_conversion: sig-ROS
   pcl_msgs: sig-ROS
   pcmanfm: xfce
   pcp: Application
   pcre: Base-service
   pcre2: Base-service
   pcs: sig-Ha
   pcsc-lite: Storage
   pdf-renderer: sig-Java
   pdfbox: sig-Java
   pdfpc: Application
+  pdfsam: sig-desktop-apps
   pdoc: sig-python-modules
   pdsh: Application
   pegdown: sig-Java
   peony: sig-UKUI
   peony-extensions: sig-UKUI
+  perception_open3d: sig-ROS
   perception_pcl: sig-ROS
   percona-server: DB
   percona-toolkit: DB
   percona-xtrabackup: DB
+  performance_test: sig-ROS
   performance_test_fixture: sig-ROS
   perftest: sig-high-performance-network
   perl: Base-service
   perl-Acme-Damn: sig-perl-modules
   perl-Algorithm-C3: sig-perl-modules
   perl-Algorithm-Combinatorics: sig-perl-modules
   perl-Algorithm-Dependency: sig-perl-modules
@@ -5985,14 +6276,15 @@
   perl-XML-Tiny: sig-perl-modules
   perl-XML-TokeParser: sig-perl-modules
   perl-XML-TreePP: sig-perl-modules
   perl-XML-Twig: sig-perl-modules
   perl-XML-Writer: sig-perl-modules
   perl-XML-XPath: Programming-language
   perl-XML-XPathEngine: sig-perl-modules
+  perl-XS-Parse-Keyword: sig-perl-modules
   perl-XString: sig-RISC-V
   perl-XXX: sig-perl-modules
   perl-YAML: Programming-language
   perl-YAML-LibYAML: sig-perl-modules
   perl-YAML-PP: sig-perl-modules
   perl-YAML-Syck: sig-perl-modules
   perl-YAML-Tiny: Programming-language
@@ -6047,34 +6339,37 @@
   perl-version: sig-perl-modules
   perlporter: dev-utils
   pesign: Application
   pesign-obs-integration: sig-security-facility
   pgadmin4-server: DB
   pgpool2: DB
   phantomjs: bigdata
+  phidgets_drivers: sig-ROS
   phodav: GNOME
   phoenix: DB
   phonon: Others
   phonon-backend-gstreamer: Private
   phonon-qt4: sig-KDE
   php: Base-service
   php-pear: sig-epol
   php-pecl-zip: sig-epol
   physfs: dev-utils
+  pick_ik: sig-ROS
   picketbox: sig-Java
   picketbox-commons: sig-Java
   picketbox-xacml: sig-Java
   pidgin: Application
   pig: DB
   pigpio: sig-RaspberryPi
   pigz: Base-service
   pin-gcc-client: Compiler
   pin-server: Compiler
   pinentry: Desktop
   pinfo: System-tool
+  pinocchio: sig-ROS
   pipewire: Desktop
   pistache: sig-high-performance-network
   pixman: Desktop
   pkcs11-helper: Runtime
   pkgconf: Base-service
   pkgconfig: Private
   pkgdiff: sig-EasyLife
@@ -6127,42 +6422,51 @@
   plexus-io: sig-Java
   plexus-languages: sig-Java
   plexus-pom: sig-Java
   plexus-resources: sig-Java
   plexus-sec-dispatcher: sig-Java
   plexus-utils: sig-Java
   plexus-velocity: sig-Java
+  plotjuggler-ros-plugins: sig-ROS
+  plotjuggler_msgs: sig-ROS
   plotutils: Application
   pluginlib: sig-ROS
   pluma: sig-UKUI
   plymouth: Desktop
   plymouth-theme-kiran: sig-KIRAN-DESKTOP
+  pmb2_navigation: sig-ROS
+  pmb2_robot: sig-ROS
+  pmb2_simulation: sig-ROS
   pmix: Base-service
   pngcrush: Application
   pngquant: Application
   pnm2ppa: Application
   po4a: Application
   poco: sig-ROS
   podman: sig-CloudNative
+  point_cloud_msg_wrapper: sig-ROS
+  pointcloud_to_laserscan: sig-ROS
   policycoreutils: sig-security-facility
   polkit: Base-service
   polkit-gnome: Base-service
   polkit-kde: sig-KDE
   polkit-pkla-compat: Base-service
   polkit-qt-1: sig-UKUI
   poly2tri: Others
   polycube: sig-high-performance-network
   polyglot: sig-Java
+  popf: sig-ROS
   poppler: Desktop
   poppler-data: Desktop
   popt: Base-service
   portals-pom: dev-utils
   portaudio: dev-utils
   portlet-2.0-api: dev-utils
   portreserve: System-tool
+  pose_cov_ops: sig-ROS
   postfix: Networking
   postgresql: DB
   postgresql-13: DB
   postgresql-jdbc: sig-Java
   postgresql-odbc: DB
   potrace: Application
   powerapi: sig-power-efficient
@@ -6193,14 +6497,15 @@
   protostream: sig-Java
   proxool: sig-Java
   proxychains-ng: Application
   proxytoys: sig-Java
   prrte: ai
   ps_mem: Computing
   psacct: Application
+  psiconv: sig-desktop-apps
   psm: dev-utils
   psmisc: Computing
   pstoedit: Application
   psutils: Application
   ptcr: sig-CloudNative
   ptpython: sig-python-modules
   publicsuffix-list: Base-service
@@ -6212,32 +6517,41 @@
   pushgateway: sig-CloudNative
   pv: Base-service
   pwgen: sig-recycle
   py3c: sig-python-modules
   pyArango: sig-ops
   pyOpenSSL: sig-security-facility
   pyScss: sig-python-modules
+  py_trees: sig-ROS
+  py_trees_js: sig-ROS
+  py_trees_ros: sig-ROS
+  py_trees_ros_interfaces: sig-ROS
   pyang: sig-high-performance-network
   pyang-swagger: sig-high-performance-network
   pyatspi: Desktop
   pybind11: sig-python-modules
+  pybind11_json_vendor: sig-ROS
+  pybind11_vendor: sig-ROS
   pycairo: Desktop
   pycharm-community: sig-UKUI
   pyelftools: Programming-language
   pyflakes: Programming-language
   pygobject2: sig-recycle
   pygobject3: Base-service
   pygtk2: sig-recycle
   pykickstart: Base-service
   pyliblzma: Base-service
   pylint: Application
+  pympress: sig-desktop-apps
   pyorbit: sig-recycle
   pyparsing: Base-service
   pyparted: Base-service
   pyporter: dev-utils
+  pyproject-api: sig-python-modules
+  pyproject-hooks: sig-python-modules
   pyproject-rpm-macros: sig-python-modules
   pyserial: Base-service
   pytest: Programming-language
   python-3parclient: sig-openstack
   python-APScheduler: sig-python-modules
   python-ATpy: sig-python-modules
   python-AWSIoTPythonSDK: sig-python-modules
@@ -6328,28 +6642,34 @@
   python-XStatic-Angular-FileUpload: sig-openstack
   python-XStatic-Angular-Gettext: sig-openstack
   python-XStatic-Angular-Schema-Form: sig-openstack
   python-XStatic-Angular-lrdragndrop: sig-openstack
   python-XStatic-Bootstrap-Datepicker: sig-openstack
   python-XStatic-Bootstrap-SCSS: sig-openstack
   python-XStatic-D3: sig-openstack
+  python-XStatic-Dagre: sig-openstack
+  python-XStatic-Dagre-D3: sig-openstack
   python-XStatic-Font-Awesome: sig-openstack
+  python-XStatic-Graphlib: sig-openstack
   python-XStatic-Hogan: sig-openstack
   python-XStatic-JQuery-Migrate: sig-openstack
   python-XStatic-JQuery.TableSorter: sig-openstack
   python-XStatic-JQuery.quicksearch: sig-openstack
   python-XStatic-JSEncrypt: sig-openstack
   python-XStatic-Jasmine: sig-openstack
+  python-XStatic-Moment-Timezone: sig-openstack
   python-XStatic-Patternfly-Bootstrap-Treeview: sig-python-modules
   python-XStatic-Rickshaw: sig-openstack
   python-XStatic-Spin: sig-openstack
   python-XStatic-bootswatch: sig-openstack
   python-XStatic-jQuery: sig-openstack
   python-XStatic-jquery-ui: sig-openstack
+  python-XStatic-lodash: sig-openstack
   python-XStatic-mdi: sig-openstack
+  python-XStatic-moment: sig-openstack
   python-XStatic-objectpath: sig-openstack
   python-XStatic-roboto-fontface: sig-openstack
   python-XStatic-smart-table: sig-openstack
   python-XStatic-term.js: sig-openstack
   python-XStatic-tv4: sig-openstack
   python-XlsxWriter: sig-python-modules
   python-Yapsy: sig-python-modules
@@ -6383,15 +6703,15 @@
   python-aiounittest: sig-python-modules
   python-aiowinreg: sig-python-modules
   python-aiozeroconf: sig-python-modules
   python-airspeed: sig-python-modules
   python-alembic: sig-python-modules
   python-alsa: sig-python-modules
   python-altgraph: sig-python-modules
-  python-amqp: sig-python-modules
+  python-amqp: sig-openstack
   python-animatplot: sig-python-modules
   python-aniso8601: sig-python-modules
   python-ansi2html: sig-python-modules
   python-ansible-inventory-grapher: sig-python-modules
   python-ansible-review: sig-python-modules
   python-ansible-runner: oVirt
   python-ansicolor: sig-python-modules
@@ -6406,14 +6726,15 @@
   python-apipkg: sig-python-modules
   python-appdirs: sig-python-modules
   python-apptools: sig-python-modules
   python-apypie: sig-python-modules
   python-argcomplete: sig-python-modules
   python-argh: sig-python-modules
   python-argon2-cffi: sig-python-modules
+  python-argon2-cffi-bindings: sig-python-modules
   python-argparse: sig-openstack
   python-argparse-manpage: sig-python-modules
   python-args: sig-python-modules
   python-arpy: sig-python-modules
   python-arrow: sig-openstack
   python-asciitree: sig-python-modules
   python-asgiref: sig-python-modules
@@ -6426,14 +6747,15 @@
   python-astroML: sig-python-modules
   python-astroid: sig-python-modules
   python-astroplan: sig-python-modules
   python-astropy: sig-python-modules
   python-astropy-healpix: sig-python-modules
   python-astropy-helpers: sig-python-modules
   python-astroquery: sig-python-modules
+  python-asttokens: ai
   python-astunparse: sig-python-modules
   python-async-generator: sig-openstack
   python-async-timeout: sig-python-modules
   python-async_generator: sig-python-modules
   python-asyncssh: sig-python-modules
   python-asynctest: sig-python-modules
   python-asysocks: sig-python-modules
@@ -6441,26 +6763,28 @@
   python-atpublic: sig-python-modules
   python-attrs: Programming-language
   python-audioread: sig-python-modules
   python-augeas: Programming-language
   python-auth.credential: sig-python-modules
   python-authheaders: sig-python-modules
   python-authres: sig-python-modules
+  python-autobahn: sig-openstack
+  python-autocommand: sig-python-modules
   python-automaton: sig-openstack
   python-autopage: sig-openstack
   python-autopep8: sig-python-modules
   python-aws-sam-translator: sig-openstack
   python-aws-xray-sdk: sig-openstack
   python-awscrt: sig-openstack
   python-azure-core: sig-openstack
   python-babelfish: sig-python-modules
   python-backcall: sig-python-modules
   python-backlash: sig-python-modules
   python-backoff: sig-python-modules
-  python-backports: Base-service
+  python-backports: sig-recycle
   python-backports-functools_lru_cache: Private
   python-backports-shutil_get_terminal_size: Private
   python-backports-ssl_match_hostname: Networking
   python-backports-unittest_mock: sig-python-modules
   python-backports_abc: Programming-language
   python-baluhn: sig-python-modules
   python-bandit: sig-python-modules
@@ -6480,14 +6804,15 @@
   python-binary-memcached: sig-openstack
   python-binaryornot: sig-python-modules
   python-binstruct: sig-python-modules
   python-bintrees: sig-python-modules
   python-bitcoinlib: sig-python-modules
   python-bitmath: sig-python-modules
   python-bitstring: sig-python-modules
+  python-black: sig-python-modules
   python-blazarclient: sig-openstack
   python-blaze: sig-python-modules
   python-bleach: sig-python-modules
   python-blessed: sig-python-modules
   python-blessings: sig-python-modules
   python-blindspin: sig-python-modules
   python-blinker: Programming-language
@@ -6506,14 +6831,15 @@
   python-branca: sig-python-modules
   python-breathe: sig-python-modules
   python-brotlipy: sig-openstack
   python-bson: sig-python-modules
   python-btrfs: sig-python-modules
   python-bucky: sig-python-modules
   python-bugzilla: sig-python-modules
+  python-build: sig-python-modules
   python-bunch: sig-openstack
   python-bytesize: sig-python-modules
   python-bz2file: sig-python-modules
   python-cached_property: sig-python-modules
   python-cachelib: sig-python-modules
   python-cachetools: sig-python-modules
   python-cachez: sig-python-modules
@@ -6523,32 +6849,36 @@
   python-capacity: sig-openstack
   python-capturer: sig-python-modules
   python-caribou: sig-python-modules
   python-case: sig-python-modules
   python-cassandra-driver: sig-openstack
   python-castellan: sig-openstack
   python-catkin-sphinx: sig-python-modules
+  python-catkin_pkg: sig-ROS
+  python-catkin_sphinx: sig-ROS
   python-cccolutils: sig-python-modules
   python-ccdproc: sig-python-modules
   python-cchardet: sig-python-modules
+  python-ceilometerclient: sig-openstack
   python-ceilometermiddleware: sig-openstack
   python-celery: sig-python-modules
   python-certbot: sig-python-modules
-  python-certifi: sig-python-modules
+  python-certifi: sig-openstack
   python-cffi: Base-service
   python-cfgv: sig-python-modules
   python-cfn-lint: sig-openstack
   python-chardet: Base-service
   python-charset-normalizer: Base-service
   python-check-manifest: sig-python-modules
   python-cheetah: Base-service
   python-cheroot: sig-python-modules
   python-cherrypy: sig-python-modules
   python-cinder-tempest-plugin: sig-openstack
   python-cinderclient: sig-openstack
+  python-cinderlib: sig-openstack
   python-citeproc-py: sig-python-modules
   python-cjdns: sig-python-modules
   python-click: Programming-language
   python-click-completion: sig-python-modules
   python-click-didyoumean: sig-python-modules
   python-click-help-colors: sig-python-modules
   python-click-log: sig-python-modules
@@ -6558,24 +6888,26 @@
   python-click-threading: sig-python-modules
   python-clickclick: sig-python-modules
   python-cliff: sig-openstack
   python-cliff-tablib: sig-python-modules
   python-cligj: sig-python-modules
   python-clint: sig-python-modules
   python-cloud_sptheme: sig-python-modules
+  python-cloudkittyclient: sig-openstack
   python-cloudpickle: sig-python-modules
   python-cltk: sig-python-modules
   python-clufter: sig-python-modules
   python-cmarkgfm: sig-python-modules
   python-cmd2: sig-python-modules
   python-cmdln: sig-python-modules
   python-cmigemo: sig-python-modules
   python-cocotb: sig-python-modules
   python-codecov: sig-python-modules
   python-colcon-bazel: sig-python-modules
+  python-colcon_core: sig-ROS
   python-colorama: sig-python-modules
   python-colorclass: sig-python-modules
   python-coloredlogs: sig-python-modules
   python-colorful: sig-python-modules
   python-colorlog: sig-python-modules
   python-colorspacious: sig-python-modules
   python-colour: sig-python-modules
@@ -6594,14 +6926,15 @@
   python-congressclient: sig-openstack
   python-connexion: sig-python-modules
   python-constantly: sig-python-modules
   python-construct: Programming-language
   python-consul: sig-openstack
   python-contextlib2: sig-python-modules
   python-contextvars: sig-python-modules
+  python-contourpy: sig-python-modules
   python-convertdate: sig-python-modules
   python-copr: sig-python-modules
   python-copr-common: sig-python-modules
   python-copr-messaging: sig-python-modules
   python-cotyledon: sig-openstack
   python-cov-core: sig-python-modules
   python-covdefaults: sig-openstack
@@ -6610,16 +6943,16 @@
   python-cpio: Base-service
   python-cppy: sig-python-modules
   python-cram: sig-python-modules
   python-crank: sig-python-modules
   python-crashtest: sig-python-modules
   python-crayons: sig-python-modules
   python-crcelk: sig-python-modules
-  python-croniter: sig-python-modules
-  python-crypto: Base-service
+  python-croniter: sig-openstack
+  python-crypto: sig-recycle
   python-cryptography: Base-service
   python-cryptography-vectors: Programming-language
   python-cson: sig-python-modules
   python-css-parser: sig-python-modules
   python-cssmin: sig-python-modules
   python-cssselect: sig-python-modules
   python-cssselect2: sig-python-modules
@@ -6657,19 +6990,21 @@
   python-decorator: Base-service
   python-deepmerge: sig-python-modules
   python-defusedxml: sig-python-modules
   python-demjson: sig-python-modules
   python-deprecated: sig-python-modules
   python-deprecation: sig-python-modules
   python-designateclient: sig-openstack
+  python-devpi-process: sig-python-modules
   python-dfs-sdk: sig-openstack
   python-dib-utils: sig-openstack
   python-dict.sorted: sig-python-modules
   python-dict2xml: sig-python-modules
   python-dictdumper: sig-python-modules
+  python-diff-cover: sig-python-modules
   python-diff-match-patch: sig-python-modules
   python-dill: sig-python-modules
   python-dingz: sig-python-modules
   python-dirq: sig-python-modules
   python-discover: sig-openstack
   python-diskcache: sig-python-modules
   python-distlib: sig-python-modules
@@ -6731,38 +7066,42 @@
   python-docker-pycreds: sig-python-modules
   python-docker-squash: sig-python-modules
   python-dockerfile-parse: sig-python-modules
   python-dockerpty: sig-python-modules
   python-docopt: Base-service
   python-docutils: Programming-language
   python-docx: sig-python-modules
-  python-dogpile.cache: sig-python-modules
+  python-dogpile.cache: sig-openstack
   python-doit: sig-python-modules
   python-dominate: sig-python-modules
   python-dotenv: sig-python-modules
   python-dpath: sig-python-modules
   python-dpkt: sig-python-modules
   python-dracclient: sig-openstack
   python-drat: sig-python-modules
+  python-drgn: sig-python-modules
   python-duecredit: sig-python-modules
   python-dulwich: sig-python-modules
   python-easy-server: sig-openstack
   python-easy-vault: sig-openstack
   python-easyargs: sig-python-modules
   python-easygui: sig-python-modules
   python-ecdsa: sig-python-modules
+  python-edgegrid: sig-openstack
+  python-editables: sig-python-modules
   python-editdistance: sig-python-modules
   python-editor: sig-python-modules
   python-elasticsearch2: sig-openstack
   python-elasticsearch7: sig-EasyLife
   python-elementpath: sig-openstack
   python-eli5: sig-python-modules
   python-email_reply_parser: sig-python-modules
   python-emcee: sig-python-modules
   python-emoji: sig-python-modules
+  python-empy: sig-ROS
   python-enchant: Programming-language
   python-enmerkar: sig-python-modules
   python-entrypoints: Programming-language
   python-enum34: Base-service
   python-envisage: sig-python-modules
   python-enzyme: sig-python-modules
   python-epdb: sig-python-modules
@@ -6771,26 +7110,27 @@
   python-estimator: A-Tune
   python-et_xmlfile: sig-python-modules
   python-etcd3: sig-openstack
   python-etcd3gw: sig-openstack
   python-ethtool: Desktop
   python-evdev: sig-python-modules
   python-eventlet: sig-python-modules
+  python-exceptiongroup: sig-python-modules
   python-execnet: sig-python-modules
   python-exif: sig-python-modules
   python-extras: Programming-language
   python-ez_setup: sig-python-modules
   python-f5-icontrol-rest: sig-python-modules
   python-fabulous: sig-python-modules
-  python-falcon: sig-python-modules
+  python-falcon: sig-openstack
   python-fastavro: sig-python-modules
   python-fastecdsa: sig-python-modules
   python-fasteners: sig-python-modules
   python-fastimport: sig-python-modules
-  python-fastjsonschema: bigdata
+  python-fastjsonschema: sig-python-modules
   python-fastnumbers: sig-python-modules
   python-fastpurge: sig-python-modules
   python-faust: Programming-language
   python-fauxquests: sig-python-modules
   python-fdb: sig-python-modules
   python-feedgenerator: sig-python-modules
   python-feedparser: sig-python-modules
@@ -6901,22 +7241,24 @@
   python-graphviz: sig-python-modules
   python-greenlet: Programming-language
   python-gremlinpython: sig-openstack
   python-grpcio-gcp: sig-openstack
   python-grpcio-status: sig-openstack
   python-gssapi: Base-service
   python-guizero: sig-python-modules
-  python-gunicorn: sig-python-modules
+  python-gunicorn: sig-openstack
   python-gwebsockets: sig-python-modules
   python-h11: sig-python-modules
   python-h2: sig-python-modules
   python-h5io: sig-python-modules
   python-h5py: A-Tune
   python-hacking: sig-openstack
   python-hamcrest: sig-python-modules
+  python-hatch-vcs: sig-python-modules
+  python-hatchling: sig-python-modules
   python-hdfs: sig-python-modules
   python-heat-cfntools: sig-openstack
   python-heatclient: sig-openstack
   python-heketi: sig-python-modules
   python-hgapi: sig-python-modules
   python-hidapi: sig-openstack
   python-hkdf: sig-python-modules
@@ -6934,26 +7276,28 @@
   python-httpbin: Private
   python-httpie: sig-python-modules
   python-httplib2: Runtime
   python-httpretty: Programming-language
   python-httpsig_cffi: sig-python-modules
   python-httptools: sig-python-modules
   python-httpx: sig-python-modules
+  python-hug: sig-python-modules
   python-humanfriendly: sig-python-modules
   python-humanize: sig-python-modules
   python-humblewx: sig-python-modules
   python-hupper: sig-python-modules
   python-husl: sig-python-modules
   python-hvac: sig-python-modules
   python-hwdata: sig-python-modules
   python-hyperframe: sig-python-modules
-  python-hyperlink: sig-python-modules
+  python-hyperlink: sig-openstack
   python-hyperopt: A-Tune
   python-hypothesis: Programming-language
   python-hypothesis-fspaths: sig-python-modules
+  python-hypothesmith: sig-python-modules
   python-ibm-db-sa: sig-openstack
   python-ibmcclient: sig-openstack
   python-icalendar: sig-python-modules
   python-icdiff: sig-python-modules
   python-identify: sig-python-modules
   python-idna: Networking
   python-idstools: sig-python-modules
@@ -6967,15 +7311,17 @@
   python-importlib-resources: sig-python-modules
   python-importmagic: sig-python-modules
   python-incremental: sig-python-modules
   python-inema: sig-python-modules
   python-infi.dtypes.iqn: sig-openstack
   python-infi.dtypes.wwn: sig-openstack
   python-infinisdk: sig-openstack
+  python-inflect: sig-python-modules
   python-inflection: sig-python-modules
+  python-influxdb: sig-openstack
   python-iniconfig: sig-python-modules
   python-iniparse: Base-service
   python-injector: sig-python-modules
   python-inotify: Base-service
   python-interfile: sig-python-modules
   python-intervals: sig-openstack
   python-intervaltree: sig-python-modules
@@ -6998,14 +7344,15 @@
   python-isodate: sig-python-modules
   python-isort: sig-python-modules
   python-isula: sig-openstack
   python-itsdangerous: Programming-language
   python-jaeger-client: sig-openstack
   python-jaraco-classes: sig-python-modules
   python-jaraco-collections: sig-python-modules
+  python-jaraco-context: sig-python-modules
   python-jaraco-functools: sig-python-modules
   python-jaraco-text: sig-python-modules
   python-jaraco.envs: sig-openstack
   python-jaraco.packaging: sig-openstack
   python-jaraco.path: sig-openstack
   python-jaraco.tidelift: sig-openstack
   python-javalang: sig-python-modules
@@ -7044,15 +7391,15 @@
   python-kaitaistruct: sig-python-modules
   python-kaptan: sig-python-modules
   python-karborclient: sig-openstack
   python-kazoo: sig-openstack
   python-kdcproxy: sig-python-modules
   python-keras-rl2: A-Tune
   python-kerberos: sig-python-modules
-  python-keyczar: sig-python-modules
+  python-keyczar: sig-recycle
   python-keyring: Programming-language
   python-keystone-tempest-plugin: sig-openstack
   python-keystoneauth1: sig-openstack
   python-keystoneclient: sig-openstack
   python-keystonemiddleware: sig-openstack
   python-kickstart: sig-python-modules
   python-kitchen: sig-python-modules
@@ -7073,25 +7420,26 @@
   python-lazr.delegates: sig-python-modules
   python-lazr.restfulclient: sig-python-modules
   python-lazr.smtptest: sig-python-modules
   python-lazr.uri: sig-python-modules
   python-lazy-object-proxy: sig-python-modules
   python-lazyarray: sig-python-modules
   python-ldap: sig-python-modules
-  python-ldap3: sig-python-modules
+  python-ldap3: sig-openstack
   python-ldappool: sig-openstack
   python-leather: sig-python-modules
   python-lefthandclient: sig-openstack
   python-lesscpy: sig-python-modules
   python-lexicon: sig-python-modules
   python-lhsmdu: Base-service
   python-libNeuroML: sig-python-modules
   python-libarchive-c: sig-python-modules
   python-libcloud: sig-python-modules
   python-libconf: sig-ops
+  python-libcst: sig-python-modules
   python-libevdev: sig-python-modules
   python-liblinear: sig-python-modules
   python-libmount: sig-python-modules
   python-libnacl: sig-python-modules
   python-libnl: sig-python-modules
   python-librosa: sig-python-modules
   python-libsass: sig-python-modules
@@ -7131,15 +7479,17 @@
   python-manilaclient: sig-openstack
   python-manuel: sig-python-modules
   python-maps: sig-python-modules
   python-markdown: Programming-language
   python-markdown2: sig-python-modules
   python-markupsafe: Base-service
   python-marshmallow: sig-python-modules
+  python-masakariclient: sig-openstack
   python-matplotlib: sig-python-modules
+  python-maturin: sig-python-modules
   python-mccabe: sig-python-modules
   python-mdx_gh_links: sig-python-modules
   python-meh: Base-service
   python-memcached: sig-python-modules
   python-memory-profiler: sig-openstack
   python-metaextract: sig-python-modules
   python-metar: sig-python-modules
@@ -7149,25 +7499,30 @@
   python-migen: sig-python-modules
   python-migrate: sig-python-modules
   python-mimeparse: Programming-language
   python-mimerender: sig-python-modules
   python-minibelt: sig-python-modules
   python-minidb: sig-python-modules
   python-minidump: sig-python-modules
+  python-mistral-lib: sig-openstack
   python-mistralclient: sig-openstack
   python-mistune: sig-python-modules
   python-mitba: sig-openstack
   python-mitmproxy: sig-python-modules
+  python-mitmproxy-wireguard: sig-python-modules
+  python-mkdocs: sig-python-modules
+  python-mkdocs-material: sig-python-modules
   python-mne: sig-python-modules
   python-mne-bids: sig-python-modules
   python-mnemonic: sig-python-modules
   python-mock: Programming-language
   python-mode: Programming-language
   python-modernize: sig-python-modules
   python-moksha.common: sig-python-modules
+  python-monasca-statsd: sig-openstack
   python-monascaclient: sig-openstack
   python-mongoengine: sig-python-modules
   python-monotonic: sig-python-modules
   python-more-itertools: Programming-language
   python-moto: sig-openstack
   python-mox: Base-service
   python-mox3: sig-openstack
@@ -7188,30 +7543,32 @@
   python-musicbrainzngs: sig-python-modules
   python-mutagen: sig-python-modules
   python-mwclient: sig-python-modules
   python-mygpoclient: sig-python-modules
   python-mypy: sig-python-modules
   python-mypy-extensions: sig-openstack
   python-mysqlclient: sig-python-modules
-  python-myst-parser: bigdata
+  python-myst-parser: sig-python-modules
+  python-natsort: sig-openstack
   python-nb2plots: sig-python-modules
-  python-nbconvert: bigdata
-  python-nbformat: bigdata
-  python-nbsphinx: bigdata
-  python-nbval: bigdata
+  python-nbconvert: sig-python-modules
+  python-nbformat: sig-python-modules
+  python-nbsphinx: sig-python-modules
+  python-nbval: sig-python-modules
   python-nbxmpp: sig-mate-desktop
   python-ndjson-testrunner: sig-python-modules
   python-neomodel: sig-python-modules
   python-neotime: sig-python-modules
   python-neovim: sig-python-modules
   python-netaddr: Programming-language
   python-netdata: sig-python-modules
   python-netifaces: A-Tune
   python-netmiko: sig-openstack
   python-networking-ovn: sig-openstack
+  python-networking-sfc: sig-openstack
   python-networkx: A-Tune
   python-neutron-lib: sig-openstack
   python-neutron-tempest-plugin: sig-openstack
   python-neutronclient: sig-openstack
   python-ngram: sig-python-modules
   python-nine: sig-python-modules
   python-nltk: sig-python-modules
@@ -7243,14 +7600,15 @@
   python-ntplib: Desktop
   python-nudatus: sig-python-modules
   python-num2words: sig-python-modules
   python-numexpr: Private
   python-numpoly: sig-python-modules
   python-oauth2client: sig-python-modules
   python-oauthlib: Base-service
+  python-octavia-lib: sig-openstack
   python-octaviaclient: sig-openstack
   python-odML: sig-python-modules
   python-odfpy: sig-python-modules
   python-odo: sig-python-modules
   python-offtrac: sig-python-modules
   python-ofxparse: sig-python-modules
   python-okaara: sig-python-modules
@@ -7311,14 +7669,15 @@
   python-oslo.versionedobjects: sig-openstack
   python-oslo.vmware: sig-openstack
   python-oslotest: sig-openstack
   python-osprofiler: sig-openstack
   python-outcome: sig-python-modules
   python-outdated: sig-python-modules
   python-ovirt-engine-sdk4: oVirt
+  python-ovn-octavia-provider: sig-openstack
   python-ovsdbapp: sig-openstack
   python-packaging: Programming-language
   python-packit: sig-python-modules
   python-pacpy: sig-python-modules
   python-pact: sig-openstack
   python-paho-mqtt: sig-python-modules
   python-pallets-sphinx-themes: sig-python-modules
@@ -7349,14 +7708,16 @@
   python-pbkdf2: sig-python-modules
   python-pbr: Programming-language
   python-pdc-client: sig-python-modules
   python-pdfkit: sig-python-modules
   python-pdfminer: sig-python-modules
   python-pdfrw: sig-python-modules
   python-pdir2: sig-python-modules
+  python-pdm-pep517: sig-python-modules
+  python-pdocs: sig-python-modules
   python-pecan: sig-python-modules
   python-peewee: sig-python-modules
   python-pendulum: sig-python-modules
   python-pep257: sig-openstack
   python-pep517: sig-python-modules
   python-pep8: sig-openstack
   python-pep8-naming: sig-python-modules
@@ -7375,35 +7736,39 @@
   python-pika: sig-openstack
   python-pika-pool: sig-python-modules
   python-pillow: sig-python-modules
   python-pint: sig-python-modules
   python-pip: Base-service
   python-pip-api: sig-openstack
   python-pip-run: sig-openstack
+  python-pip-shims: sig-python-modules
   python-pipdeptree: sig-python-modules
   python-pipreqs: sig-openstack
   python-pkgconfig: A-Tune
   python-pkginfo: sig-python-modules
   python-pkgwat.api: sig-python-modules
   python-plaintable: sig-python-modules
   python-platformdirs: Application
   python-player: sig-python-modules
+  python-plette: sig-python-modules
   python-plink: sig-python-modules
   python-pluggy: Programming-language
   python-pluginbase: sig-python-modules
   python-pluginlib: sig-python-modules
   python-plugnplay: sig-python-modules
   python-plum-py: sig-cinnamon
   python-plumbum: sig-python-modules
   python-ply: Base-service
   python-pocketlint: Base-service
   python-podcastparser: sig-python-modules
+  python-poetry-core: sig-python-modules
   python-polib: Base-service
   python-portalocker: sig-python-modules
   python-portend: sig-python-modules
+  python-portray: sig-python-modules
   python-posix_ipc: sig-python-modules
   python-power: sig-python-modules
   python-poyo: sig-python-modules
   python-praw: sig-python-modules
   python-pre-commit: sig-openstack
   python-precis_i18n: sig-mate-desktop
   python-pretend: Programming-language
@@ -7451,15 +7816,15 @@
   python-pybeam: sig-python-modules
   python-pybtex: sig-python-modules
   python-pybtex-docutils: sig-python-modules
   python-pycadf: sig-openstack
   python-pycares: sig-python-modules
   python-pycdlib: sig-OS-Builder
   python-pyclipper: sig-python-modules
-  python-pycodestyle: sig-python-modules
+  python-pycodestyle: sig-openstack
   python-pycollada: sig-python-modules
   python-pycountry: sig-openstack
   python-pycparser: Base-service
   python-pycryptodome: sig-python-modules
   python-pycryptodomex: sig-python-modules
   python-pycscope: sig-python-modules
   python-pycurl: Base-service
@@ -7484,21 +7849,23 @@
   python-pyghmi: sig-openstack
   python-pyglet: Private
   python-pygments: Programming-language
   python-pygments-style-solarized: sig-python-modules
   python-pyhcl: sig-python-modules
   python-pyi2cflash: sig-python-modules
   python-pyinstaller: sig-python-modules
+  python-pyinstaller-hooks-contrib: sig-python-modules
   python-pykalman: sig-python-modules
   python-pykeepass: sig-python-modules
   python-pylama: sig-openstack
   python-pylast: sig-python-modules
   python-pylev: sig-python-modules
   python-pylons-sphinx-themes: sig-python-modules
   python-pymatreader: sig-python-modules
+  python-pymdown-extensions: sig-python-modules
   python-pymemcache: sig-python-modules
   python-pymoc: sig-python-modules
   python-pymod2pkg: sig-python-modules
   python-pymongo: Programming-language
   python-pymongocrypt: sig-openstack
   python-pynacl: sig-python-modules
   python-pynetdicom: sig-python-modules
@@ -7513,17 +7880,17 @@
   python-pypng: sig-python-modules
   python-pypowervm: sig-openstack
   python-pyprocdev: sig-python-modules
   python-pyquery: sig-python-modules
   python-pyrad: sig-python-modules
   python-pyramid_fas_openid: sig-python-modules
   python-pyreadline: sig-python-modules
-  python-pyroute2: sig-python-modules
+  python-pyroute2: sig-openstack
   python-pyrpm: sig-python-modules
-  python-pyrsistent: sig-python-modules
+  python-pyrsistent: sig-openstack
   python-pyrtlsdr: sig-python-modules
   python-pysaml2: sig-python-modules
   python-pysb: sig-python-modules
   python-pyscard: sig-python-modules
   python-pysendfile: sig-python-modules
   python-pyserial: sig-python-modules
   python-pyshark: sig-python-modules
@@ -7539,14 +7906,15 @@
   python-pystache: sig-python-modules
   python-pystalk: sig-python-modules
   python-pystoi: sig-python-modules
   python-pystray: sig-python-modules
   python-pytest-arraydiff: sig-python-modules
   python-pytest-asyncio: sig-python-modules
   python-pytest-beakerlib: sig-python-modules
+  python-pytest-benchmark: sig-python-modules
   python-pytest-black: sig-openstack
   python-pytest-cache: sig-python-modules
   python-pytest-catchlog: sig-python-modules
   python-pytest-checkdocs: sig-openstack
   python-pytest-cov: Base-service
   python-pytest-datafiles: sig-python-modules
   python-pytest-django: sig-openstack
@@ -7594,14 +7962,15 @@
   python-pytest-xdist: sig-python-modules
   python-pytest-xprocess: sig-python-modules
   python-pythonwebhdfs: A-Tune
   python-pytimeparse: sig-python-modules
   python-pytoml: Programming-language
   python-pytools: sig-python-modules
   python-pytrailer: sig-python-modules
+  python-pytz-deprecation-shim: sig-python-modules
   python-pytzdata: sig-python-modules
   python-pyu2f: sig-openstack
   python-pyudev: Base-service
   python-pyusb: sig-python-modules
   python-pyvit: sig-python-modules
   python-pyvmomi: sig-python-modules
   python-pyvo: sig-python-modules
@@ -7622,14 +7991,15 @@
   python-rangehttpserver: sig-python-modules
   python-rarfile: sig-python-modules
   python-ratelimitingfilter: sig-python-modules
   python-rawkit: sig-python-modules
   python-rbd-iscsi-client: sig-openstack
   python-rcssmin: sig-python-modules
   python-rdflib: sig-python-modules
+  python-re-assert: sig-python-modules
   python-readme-renderer: sig-python-modules
   python-rebulk: sig-python-modules
   python-recommonmark: Base-service
   python-redis: Base-service
   python-regex: sig-python-modules
   python-remoto: sig-python-modules
   python-renderspec: sig-python-modules
@@ -7646,15 +8016,15 @@
   python-requests-ftp: Networking
   python-requests-gssapi: sig-python-modules
   python-requests-kerberos: sig-python-modules
   python-requests-mock: sig-openstack
   python-requests-ntlm: sig-python-modules
   python-requests-oauthlib: sig-python-modules
   python-requests-toolbelt: sig-python-modules
-  python-requests-unixsocket: bigdata
+  python-requests-unixsocket: sig-python-modules
   python-requestsexceptions: sig-openstack
   python-requirementslib: sig-openstack
   python-responses: sig-openstack
   python-restfly: sig-python-modules
   python-restructuredtext-lint: sig-openstack
   python-restsh: sig-python-modules
   python-retask: sig-python-modules
@@ -7667,28 +8037,30 @@
   python-rjsmin: sig-python-modules
   python-rmtest: sig-python-modules
   python-rnc2rng: sig-python-modules
   python-robotframework: sig-ROS
   python-rocket: sig-python-modules
   python-roman: sig-python-modules
   python-rope: sig-python-modules
+  python-rosdistro: sig-ROS
   python-rosinstall: sig-python-modules
+  python-rospkg: sig-ROS
   python-routes: sig-python-modules
   python-rpdb: sig-python-modules
   python-rpkg: sig-python-modules
   python-rply: sig-python-modules
   python-rpm-generators: Base-service
   python-rpmfluff: Private
   python-rsa: sig-python-modules
   python-rsd-lib: sig-openstack
   python-rsdclient: sig-openstack
   python-rst.linker: sig-openstack
   python-rst2txt: Programming-language
   python-rstcheck: sig-python-modules
-  python-rtslib: sig-python-modules
+  python-rtslib: sig-openstack
   python-rtslib-fb: sig-openstack
   python-ruamel-yaml: sig-python-modules
   python-ruamel-yaml-clib: sig-python-modules
   python-ruffus: sig-python-modules
   python-rustcfg: sig-python-modules
   python-rxjson: sig-python-modules
   python-ryu: sig-openstack
@@ -7729,14 +8101,15 @@
   python-setuptools_hg: sig-python-modules
   python-setuptools_scm: Programming-language
   python-sh: sig-python-modules
   python-shamir-mnemonic: sig-python-modules
   python-shodan: sig-python-modules
   python-shortuuid: sig-python-modules
   python-should_dsl: sig-python-modules
+  python-shtab: sig-python-modules
   python-sieve: sig-python-modules
   python-simplebayes: sig-python-modules
   python-simpleeval: sig-python-modules
   python-simplegeneric: sig-python-modules
   python-simplejson: sig-python-modules
   python-simpleline: Base-service
   python-simplepam: sig-python-modules
@@ -7769,15 +8142,15 @@
   python-speedtest-cli: sig-python-modules
   python-speg: sig-python-modules
   python-sphinx: Programming-language
   python-sphinx-argparse: sig-python-modules
   python-sphinx-autodoc-typehints: sig-openstack
   python-sphinx-bootstrap-theme: sig-python-modules
   python-sphinx-epytext: sig-python-modules
-  python-sphinx-feature-classification: sig-python-modules
+  python-sphinx-feature-classification: sig-openstack
   python-sphinx-gallery: sig-python-modules
   python-sphinx-intl: sig-python-modules
   python-sphinx-issues: sig-python-modules
   python-sphinx-notfound-page: sig-python-modules
   python-sphinx-testing: sig-openstack
   python-sphinx-theme-alabaster: Programming-language
   python-sphinx_lv2_theme: sig-epol
@@ -7786,15 +8159,15 @@
   python-sphinxcontrib-apidoc: sig-python-modules
   python-sphinxcontrib-applehelp: sig-python-modules
   python-sphinxcontrib-autoprogram: sig-openstack
   python-sphinxcontrib-bibtex: sig-python-modules
   python-sphinxcontrib-blockdiag: sig-python-modules
   python-sphinxcontrib-devhelp: sig-python-modules
   python-sphinxcontrib-fulltoc: sig-python-modules
-  python-sphinxcontrib-github-alt: bigdata
+  python-sphinxcontrib-github-alt: sig-python-modules
   python-sphinxcontrib-htmlhelp: sig-python-modules
   python-sphinxcontrib-httpdomain: sig-python-modules
   python-sphinxcontrib-issuetracker: sig-python-modules
   python-sphinxcontrib-jsmath: sig-python-modules
   python-sphinxcontrib-log-cabinet: Programming-language
   python-sphinxcontrib-pecanwsme: sig-python-modules
   python-sphinxcontrib-programoutput: sig-openstack
@@ -7862,15 +8235,15 @@
   python-tempest-lib: sig-openstack
   python-tempita: Base-service
   python-tempora: sig-python-modules
   python-tenacity: sig-python-modules
   python-tensorboard: A-Tune
   python-tensorboard-plugin-wit: A-Tune
   python-termcolor: sig-python-modules
-  python-terminado: bigdata
+  python-terminado: sig-python-modules
   python-terminaltables: sig-python-modules
   python-test-server: sig-python-modules
   python-testfixtures: sig-openstack
   python-testpath: sig-python-modules
   python-testrepository: sig-python-modules
   python-testresources: sig-python-modules
   python-testscenarios: Programming-language
@@ -7880,27 +8253,30 @@
   python-textfsm: sig-openstack
   python-textparser: sig-python-modules
   python-texttable: sig-python-modules
   python-tftpy: sig-python-modules
   python-tgext.crud: sig-python-modules
   python-threadloop: sig-openstack
   python-threadpoolctl: sig-python-modules
+  python-time-machine: sig-python-modules
   python-timeout-decorator: sig-python-modules
   python-timeunit: sig-python-modules
   python-tinycss2: sig-cinnamon
   python-tinydb: sig-python-modules
   python-tinyrpc: sig-python-modules
   python-toml: sig-python-modules
   python-tomli: sig-python-modules
   python-tomli-w: sig-python-modules
+  python-tomlkit: sig-python-modules
   python-toolz: sig-python-modules
   python-tooz: sig-openstack
   python-tornado: Programming-language
   python-towncrier: sig-openstack
   python-tox: sig-python-modules
+  python-tox-current-env: sig-python-modules
   python-tqdm: sig-python-modules
   python-traceback2: Programming-language
   python-traitlets: sig-python-modules
   python-traitsui: sig-python-modules
   python-transaction: sig-openstack
   python-translationstring: sig-python-modules
   python-treelib: sig-ops
@@ -7915,21 +8291,24 @@
   python-tw2.jqplugins.ui: sig-python-modules
   python-tw2.jquery: sig-python-modules
   python-twilio: sig-python-modules
   python-twine: sig-python-modules
   python-twisted: sig-python-modules
   python-txWS: sig-python-modules
   python-txZMQ: sig-python-modules
+  python-txaio: sig-openstack
   python-typed-ast: sig-openstack
+  python-typeguard: sig-ROS
   python-types-cryptography: sig-openstack
   python-types-enum34: sig-openstack
   python-types-ipaddress: sig-openstack
   python-types-paramiko: sig-openstack
   python-typing: sig-python-modules
   python-typing-extensions: sig-openstack
+  python-typing-inspect: sig-python-modules
   python-typogrify: sig-python-modules
   python-tzlocal: sig-python-modules
   python-u-msgpack-python: Base-service
   python-uamqp: sig-openstack
   python-ucam-webauth: sig-python-modules
   python-uhashring: sig-openstack
   python-ujson: sig-openstack
@@ -7959,14 +8338,15 @@
   python-vintage: sig-openstack
   python-virtualenv: Programming-language
   python-virtualenv-api: sig-python-modules
   python-virtualenv-clone: sig-python-modules
   python-virtualenvwrapper: sig-python-modules
   python-visidata: sig-python-modules
   python-visitor: sig-python-modules
+  python-vistir: sig-python-modules
   python-visvis: sig-python-modules
   python-vitrageclient: sig-openstack
   python-vobject: sig-python-modules
   python-volkszaehler: sig-python-modules
   python-voluptuous: sig-python-modules
   python-vpoller: sig-python-modules
   python-vulture: sig-python-modules
@@ -8023,14 +8403,19 @@
   python-xlwt: sig-python-modules
   python-xml2rfc: sig-python-modules
   python-xmlrunner: sig-python-modules
   python-xmlschema: sig-openstack
   python-xmltodict: sig-python-modules
   python-xmod: sig-python-modules
   python-xpath-expressions: sig-python-modules
+  python-xstatic-angular-uuid: sig-openstack
+  python-xstatic-angular-vis: sig-openstack
+  python-xstatic-filesaver: sig-openstack
+  python-xstatic-js-yaml: sig-openstack
+  python-xstatic-json2yaml: sig-openstack
   python-xtermcolor: sig-python-modules
   python-xunitparser: sig-python-modules
   python-xvfbwrapper: sig-python-modules
   python-xxhash: sig-python-modules
   python-yagot: sig-openstack
   python-yamllint: sig-openstack
   python-yamlloader: sig-openstack
@@ -8097,14 +8482,15 @@
   qhull: Others
   qjson: sig-UKUI
   qla2xxx: sig-Compatibility-Infra
   qpdf: Programming-language
   qperf: Application
   qpid-proton: Base-service
   qpid-proton-java: sig-Java
+  qpoases_vendor: sig-ROS
   qqc2-desktop-style: sig-KDE
   qrencode: Desktop
   qrupdate: bigdata
   qscintilla: bigdata
   qstardict: sig-desktop-apps
   qt: Runtime
   qt-assistant-adp: Others
@@ -8125,14 +8511,15 @@
   qt5-qtenginio: Others
   qt5-qtfeedback: sig-KDE
   qt5-qtgamepad: Programming-language
   qt5-qtgraphicaleffects: Programming-language
   qt5-qtimageformats: Programming-language
   qt5-qtlocation: Programming-language
   qt5-qtmultimedia: Programming-language
+  qt5-qtnetworkauth: sig-QT
   qt5-qtquickcontrols: Programming-language
   qt5-qtquickcontrols2: Programming-language
   qt5-qtremoteobjects: Programming-language
   qt5-qtscript: Programming-language
   qt5-qtscxml: Programming-language
   qt5-qtsensors: Programming-language
   qt5-qtserialbus: Programming-language
@@ -8149,61 +8536,121 @@
   qt5-qtwebsockets: Programming-language
   qt5-qtwebview: Programming-language
   qt5-qtx11extras: Programming-language
   qt5-qtxmlpatterns: Programming-language
   qt5-ukui-platformtheme: sig-UKUI
   qt5dxcb-plugin: sig-DDE
   qt5integration: sig-DDE
+  qt6: sig-QT
+  qt6-qt3d: sig-QT
+  qt6-qt5compat: sig-QT
+  qt6-qtbase: sig-QT
+  qt6-qtcharts: sig-QT
+  qt6-qtcoap: sig-QT
+  qt6-qtconnectivity: sig-QT
+  qt6-qtdatavis3d: sig-QT
+  qt6-qtdeclarative: sig-QT
+  qt6-qtdoc: sig-QT
+  qt6-qthttpserver: sig-QT
+  qt6-qtimageformats: sig-QT
+  qt6-qtlanguageserver: sig-QT
+  qt6-qtlocation: sig-QT
+  qt6-qtlottie: sig-QT
+  qt6-qtmqtt: sig-QT
+  qt6-qtmultimedia: sig-QT
+  qt6-qtnetworkauth: sig-QT
+  qt6-qtopcua: sig-QT
+  qt6-qtpositioning: sig-QT
+  qt6-qtquick3d: sig-QT
+  qt6-qtquick3dphysics: sig-QT
+  qt6-qtquickcontrols2: sig-QT
+  qt6-qtquicktimeline: sig-QT
+  qt6-qtremoteobjects: sig-QT
+  qt6-qtscxml: sig-QT
+  qt6-qtsensors: sig-QT
+  qt6-qtserialbus: sig-QT
+  qt6-qtserialport: sig-QT
+  qt6-qtshadertools: sig-QT
+  qt6-qtspeech: sig-QT
+  qt6-qtsvg: sig-QT
+  qt6-qttools: sig-QT
+  qt6-qttranslations: sig-QT
+  qt6-qtvirtualkeyboard: sig-QT
+  qt6-qtwayland: sig-QT
+  qt6-qtwebchannel: sig-QT
+  qt6-qtwebengine: sig-QT
+  qt6-qtwebsockets: sig-QT
+  qt6-qtwebview: sig-QT
+  qt_gui_core: sig-ROS
   qtav: sig-UKUI
   qtchooser: sig-UKUI
   qtkeychain-qt5: sig-KDE
   qtwebkit: sig-recycle
   quartz: sig-Java
+  quaternion_operation: sig-ROS
   quay: sig-K8sDistro
   quazip-qt5: sig-UKUI
   querydsl3: sig-Java
   quilt: Application
   quota: Storage
   qwt: sig-ROS
   qwt_dependency: sig-ROS
+  r2r_spl: sig-ROS
   rabbitmq-java-client: sig-Java
   rabbitmq-server: Application
   racon: sig-bio
+  radar_msgs-release: sig-ROS
   radvd: Networking
   ragel: dev-utils
   rain: bigdata
+  random_numbers: sig-ROS
   randomizedtesting: Base-service
+  range-v3: sig-ROS
   ranger: dev-utils
   rapidjson: Base-service
   raptor2: Others
   rarian: Base-service
   rasdaemon: Base-service
   raspberrypi-bluetooth: sig-RaspberryPi
   raspberrypi-build: sig-RaspberryPi
   raspberrypi-eeprom: sig-RaspberryPi
   raspberrypi-firmware: sig-RaspberryPi
   raspberrypi-kernel: sig-RaspberryPi
   raspberrypi-userland: sig-RaspberryPi
   raspi-config: sig-RaspberryPi
+  raspimouse2: sig-ROS
+  raspimouse_description: sig-ROS
   rasqal: Application
+  raxml-ng: sig-bio
+  rc_common_msgs_ros2: sig-ROS
+  rc_dynamics_api: sig-ROS
+  rc_genicam_api: sig-ROS
+  rc_genicam_driver_ros2: sig-ROS
+  rc_reason_clients_ros2: sig-ROS
+  rcdiscover: sig-ROS
   rcl: sig-ROS
   rcl_interfaces: sig-ROS
   rcl_logging: sig-ROS
+  rclc: sig-ROS
   rclcpp: sig-ROS
+  rclpy: sig-ROS
   rcpputils: sig-ROS
   rcs: Others
+  rcss3d_agent: sig-ROS
+  rcutils: sig-ROS
   rcutilsl: sig-ROS
   rdate: Application
   rdiff-backup: Application
   rdma-core: sig-high-performance-network
   re2: Others
   re2-rust: Base-service
   re2c: sig-mate-desktop
   readline: Base-service
   realmd: Base-service
+  realsense-ros: sig-ROS
   realtime_support: sig-ROS
   realtime_tools: sig-ROS
   rear: Others
   recode: Base-service
   redhat-menus: sig-recycle
   redis: Others
   redis-protocol: Application
@@ -8231,62 +8678,101 @@
   rhnlib: Programming-language
   rhq-plugin-annotations: sig-Java
   rhythmbox: Application
   riemann-c-client: oVirt
   rinetd: Application
   risc-v-kernel: sig-RISC-V
   ristretto: xfce
+  rmf_api_msgs: sig-ROS
+  rmf_battery: sig-ROS
+  rmf_building_map_msgs: sig-ROS
+  rmf_cmake_uncrustify: sig-ROS
+  rmf_internal_msgs: sig-ROS
+  rmf_ros2: sig-ROS
+  rmf_simulation: sig-ROS
+  rmf_task: sig-ROS
+  rmf_traffic: sig-ROS
+  rmf_traffic_editor: sig-ROS
+  rmf_utils: sig-ROS
+  rmf_visualization: sig-ROS
+  rmf_visualization_msgs: sig-ROS
   rmic-maven-plugin: Base-service
   rmw: sig-ROS
   rmw_connext: sig-ROS
+  rmw_connextdds: sig-ROS
   rmw_cyclonedds: sig-ROS
   rmw_dds_common: sig-ROS
   rmw_fastrtps: sig-ROS
+  rmw_gurumdds: sig-ROS
   rmw_implementation: sig-ROS
   rng-tools: Base-service
   rngom: Application
   robodoc: Application
+  robot_calibration: sig-ROS
+  robot_controllers: sig-ROS
   robot_state_publisher: sig-ROS
+  robot_upstart: sig-ROS
+  robotraconteur: sig-ROS
   robust-http-client: sig-Java
   rocksdb: System-tool
   rome: sig-Java
   rootfiles: Base-service
   rootsh: Others
   ros: sig-ROS
+  ros-foxglove-bridge: sig-ROS
+  ros-octomap: sig-ROS
   ros1_bridge: sig-ROS
+  ros2_angles: sig-ROS
   ros2_base: sig-ROS
   ros2_cartographer: sig-ROS
   ros2_cartographer_ros: sig-ROS
   ros2_class_loader: sig-ROS
   ros2_control: sig-ROS
   ros2_control_msgs: sig-ROS
+  ros2_control_toolbox: sig-ROS
   ros2_controllers: sig-ROS
   ros2_demos: sig-ROS
   ros2_depthimage_to_laserscan: sig-ROS
+  ros2_diagnosticsn: sig-ROS
+  ros2_dynamixel_sdk: sig-ROS
   ros2_eigen_stl_containers: sig-ROS
   ros2_example_interfaces: sig-ROS
   ros2_examples: sig-ROS
   ros2_geometric_shapes: sig-ROS
   ros2_geometry2: sig-ROS
   ros2_graph_msgs: sig-ROS
+  ros2_hls_lfcd_lds_driver: sig-ROS
   ros2_image_common: sig-ROS
   ros2_image_pipeline: sig-ROS
   ros2_image_transport_plugins: sig-ROS
   ros2_image_transport_tutorials: sig-ROS
   ros2_interactive_markers: sig-ROS
   ros2_kdl_parser: sig-ROS
   ros2_laser_geometry: sig-ROS
+  ros2_laser_proc: sig-ROS
+  ros2_moveit2: sig-ROS
+  ros2_moveit2_tutorials: sig-ROS
   ros2_moveit_msgs: sig-ROS
+  ros2_moveit_resources: sig-ROS
+  ros2_moveit_visual_tools: sig-ROS
   ros2_navigation2: sig-ROS
   ros2_navigation_msgs: sig-ROS
+  ros2_object_recognition_msgs: sig-ROS
+  ros2_octomap: sig-ROS
+  ros2_octomap_msgs: sig-ROS
   ros2_orocos_kinematics_dynamics: sig-ROS
+  ros2_ouster_drivers: sig-ROS
+  ros2_pcl_msgs: sig-ROS
+  ros2_perception_pcl: sig-ROS
+  ros2_planning_system: sig-ROS
   ros2_pluginlib: sig-ROS
   ros2_python_qt_binding: sig-ROS
   ros2_qt_gui_core: sig-ROS
   ros2_random_numbers: sig-ROS
+  ros2_realtime_tools: sig-ROS
   ros2_resource_retriever: sig-ROS
   ros2_robot_state_publisher: sig-ROS
   ros2_ros_environment: sig-ROS
   ros2_ros_tutorials: sig-ROS
   ros2_rqt: sig-ROS
   ros2_rqt_action: sig-ROS
   ros2_rqt_console: sig-ROS
@@ -8298,48 +8784,75 @@
   ros2_rqt_reconfigure: sig-ROS
   ros2_rqt_service_caller: sig-ROS
   ros2_rqt_shell: sig-ROS
   ros2_rqt_srv: sig-ROS
   ros2_rqt_top: sig-ROS
   ros2_rqt_topic: sig-ROS
   ros2_rviz: sig-ROS
+  ros2_rviz_visual_tools: sig-ROS
+  ros2_socketcan: sig-ROS
   ros2_srdfdom: sig-ROS
+  ros2_system_modes: sig-ROS
   ros2_system_tests: sig-ROS
   ros2_tracing: sig-ROS
+  ros2_transport_drivers: sig-ROS
+  ros2_turtlebot3: sig-ROS
+  ros2_turtlebot3_msgs: sig-ROS
+  ros2_udp_msgs: sig-ROS
   ros2_urdf: sig-ROS
+  ros2_urg_c: sig-ROS
+  ros2_urg_node: sig-ROS
+  ros2_urg_node_msgs: sig-ROS
+  ros2_use_cam: sig-ROS
+  ros2_v4l2_camera: sig-ROS
   ros2_vision_opencv: sig-ROS
   ros2_warehouse_ros: sig-ROS
+  ros2_warehouse_ros_sqlite: sig-ROS
+  ros2_wireless: sig-ROS
+  ros2_xacro: sig-ROS
+  ros2acceleration: sig-ROS
   ros2cli: sig-ROS
   ros2cli_common_extensions: sig-ROS
+  ros2launch_security: sig-ROS
+  ros_aruco_opencv: sig-ROS
+  ros_canopen: sig-ROS
   ros_comm: sig-ROS
   ros_comm_msgs: sig-ROS
   ros_control: sig-ROS
   ros_controllers: sig-ROS
   ros_environment: sig-ROS
+  ros_gz: sig-ROS
+  ros_image_to_qimage: sig-ROS
+  ros_system_fingerprint: sig-ROS
   ros_testing: sig-ROS
   ros_tutorials: sig-ROS
+  ros_workspace: sig-ROS
   rosbag2: sig-ROS
   rosbag_migration_rule: sig-ROS
+  rosbridge_suite: sig-ROS
   rosconsole: sig-ROS
   rosconsole_bridge: sig-ROS
   roscpp_core: sig-ROS
   rosidl: sig-ROS
   rosidl_dds: sig-ROS
   rosidl_defaults: sig-ROS
   rosidl_python: sig-ROS
   rosidl_runtime_py: sig-ROS
   rosidl_typesupport: sig-ROS
   rosidl_typesupport_connext: sig-ROS
   rosidl_typesupport_fastrtps: sig-ROS
   roslint: sig-ROS
   roslisp: sig-ROS
   rospack: sig-ROS
+  rospy_message_converter: sig-ROS
+  rot_conv_lib: sig-ROS
   rpcbind: Networking
   rpcsvc-proto: Application
   rpg_svo: sig-ROS
+  rplidar_ros: sig-ROS
   rpm: Base-service
   rpm-mpi-hooks: Private
   rpm-ostree: sig-K8sDistro
   rpm-ostree-toolbox: sig-Ostree-Assembly
   rpmdevtools: Packaging
   rpmlint: Programming-language
   rpmrebuild: Base-service
@@ -8347,14 +8860,15 @@
   rqt: sig-ROS
   rqt_action: sig-ROS
   rqt_bag: sig-ROS
   rqt_common_plugins: sig-ROS
   rqt_console: sig-ROS
   rqt_dep: sig-ROS
   rqt_graph: sig-ROS
+  rqt_image_overlay: sig-ROS
   rqt_image_view: sig-ROS
   rqt_launch: sig-ROS
   rqt_logger_level: sig-ROS
   rqt_moveit: sig-ROS
   rqt_msg: sig-ROS
   rqt_nav_view: sig-ROS
   rqt_plot: sig-ROS
@@ -8377,15 +8891,20 @@
   rqt_web: sig-ROS
   rrdtool: Application
   rsh: Private
   rstudio: sig-bio
   rsync: Base-service
   rsyslog: Base-service
   rt-tests: sig-industrial-control
+  rt_manipulators_cpp: sig-ROS
+  rt_usb_9axisimu_driver: sig-ROS
+  rtabmap: sig-ROS
+  rtabmap_ros: sig-ROS
   rtcheck: sig-industrial-control
+  rtcm_msgs: sig-ROS
   rteval: sig-industrial-control
   rtkit: Desktop
   rtorrent: Application
   rubberband: Desktop
   rubik: sig-CloudNative
   ruby: sig-ruby
   ruby-augeas: sig-ruby
@@ -8432,14 +8951,15 @@
   rubygem-bootsnap: sig-ruby
   rubygem-bootstrap-sass: sig-ops
   rubygem-bson: sig-ruby
   rubygem-builder: sig-ruby
   rubygem-bundler: sig-ruby
   rubygem-bundler_ext: sig-ops
   rubygem-byebug: sig-ruby
+  rubygem-capng_c: sig-ruby
   rubygem-capybara: sig-ruby
   rubygem-childprocess: sig-ruby
   rubygem-chronic: sig-ruby
   rubygem-clamp: sig-ruby
   rubygem-coderay: sig-ruby
   rubygem-coffee-rails: sig-ops
   rubygem-coffee-script: sig-ruby
@@ -8702,21 +9222,26 @@
   rubygem-wikicloth: sig-ruby
   rubygem-will_paginate: sig-ruby
   rubygem-xpath: sig-ruby
   rubygem-yajl-ruby: sig-ruby
   rubygem-yard: sig-ruby
   rubygem-zeitwerk: sig-Ha
   rubyporter: dev-utils
+  ruckig: sig-ROS
   runc: sig-CloudNative
   rust: sig-Rust
+  rust-bindgen: sig-Rust
   rust-cbindgen: sig-Rust
   rust-packaging: sig-Rust
   rust-srpm-macros: sig-epol
   rustup: sig-Rust
   rviz: sig-ROS
+  rviz_2d_overlay_plugins: sig-ROS
+  rviz_satellite: sig-ROS
+  rviz_visual_tools: sig-ROS
   rxjava: sig-Java
   rxtx: sig-Java
   rygel: GNOME
   s-tui: dev-utils
   s3fs-fuse: Storage
   saab-fonts: Desktop
   sac: sig-Java
@@ -8741,36 +9266,43 @@
   sblim-sfcc: System-tool
   sbt: sig-Java
   scala: sig-Java
   scalapack: sig-epol
   scannotation: sig-Java
   scap-security-guide: sig-security-facility
   scap-workbench: sig-security-facility
+  schemas: sig-ROS
   schroedinger: sig-epol
   scim: sig-KDE
   scipy: Computing
   scl-utils: Application
   scotch: sig-epol
   screen: Base-service
   scrub: Application
   scsi-target-utils: Others
   sddm: sig-KDE
   sddm-kcm: sig-KDE
   sdformat: sig-ROS
+  sdformat_urdf: sig-ROS
   sdparm: Storage
   seabios: Others
   seahorse: Desktop
   seastar: sig-high-performance-network
   secGear: sig-confidential-computing
   secpaver: sig-security-facility
   security-tool: sig-security-facility
+  security_dataclassification: sig-distributed-middleware
+  security_device_auth: sig-distributed-middleware
+  security_device_security_level: sig-distributed-middleware
+  security_huks: sig-distributed-middleware
   sed: Base-service
   selinux-policy: sig-security-facility
   sendmail: Desktop
   sentencepiece: ai
+  septentrio_gnss_driver: sig-ROS
   seqtk: sig-bio
   sequence-library: sig-Java
   serd: sig-epol
   serp: sig-Java
   setools: Base-service
   setroubleshoot: sig-security-facility
   setroubleshoot-plugins: Base-service
@@ -8793,79 +9325,95 @@
   shim: Base-service
   shim-unsigned-aarch64: sig-recycle
   shotwell: sig-UKUI
   shrinkwrap: sig-Java
   shrinkwrap-descriptors: sig-Java
   shrinkwrap-resolver: sig-Java
   si-units: Base-service
+  sick_safetyscanners2: sig-ROS
+  sick_safetyscanners2_interfaces: sig-ROS
+  sick_safetyscanners_base: sig-ROS
   siege: sig-epol
   sigar: sig-Java
+  sigil: sig-desktop-apps
   signon: sig-KDE
   signon-plugin-oauth2: sig-KDE
   signpost-core: sig-Java
   sil-abyssinica-fonts: System-tool
   sil-nuosu-fonts: Desktop
   sil-padauk-fonts: Desktop
   sil-scheherazade-fonts: System-tool
   simde: dev-utils
   simple: sig-Java
   simple-scan: GNOME
+  simple-term-menu: sig-ROS
   simple-xml: sig-Java
+  simple_actions: sig-ROS
+  simple_launch: sig-ROS
   sip: Others
   sisu: sig-Java
   sisu-mojos: sig-Java
   skkdic: Application
   skopeo: sig-CloudNative
   skylark: Virt
   slam_gmapping: sig-ROS
   slam_gmapping_ros2: sig-ROS
+  slam_toolbox: sig-ROS
   slang: Base-service
   slapi-nis: Application
   sleuthkit: Others
   slf4j: sig-Java
   slf4j-jboss-logmanager: sig-Java
+  slider_publisher: sig-ROS
   slirp4netns: sig-CloudNative
   slurm: dev-utils
   smartdenovo: sig-bio
   smartmontools: Storage
   smc-fonts: System-tool
   smp_utils: Storage
   snakeyaml: Base-service
   snapd-glib: Application
   snappy: Base-service
   snappy-java: Base-service
   sni-qt: Private
   snmp4j: oVirt
   snowball-java: sig-Java
+  snowbot_operating_system: sig-ROS
   socat: Application
+  soccer_interfaces: sig-ROS
+  soccer_object_msgs: sig-ROS
+  soccer_visualization: sig-ROS
   socket_wrapper: Programming-language
   soem: sig-industrial-control
   soes: sig-industrial-control
   sofia-sip: GNOME
   softhsm: sig-security-facility
+  sol_vendor: sig-ROS
   solr: Application
   sombok: Base-service
   sonatype-oss-parent: sig-Java
   sonatype-plugins-parent: sig-Java
   sonic-buildimage: sig-ONL
   sonic-linux-kernel: sig-ONL
+  sophus: sig-ROS
   sord: sig-epol
   sos: Base-service
   sos-collector: Private
   sound-theme-freedesktop: Desktop
   soundtouch: Application
   source-highlight: Desktop
   sox: Others
   soxr: Desktop
   spamassassin: Application
   spark: bigdata
   sparsehash: sig-epol
   spatial4j: sig-Java
   spawn-fcgi: Networking
   spdk: Storage
+  spdlog: sig-ROS
   spdlog_vendor: sig-ROS
   spec-version-maven-plugin: Application
   speech-dispatcher: System-tool
   speex: Base-service
   speexdsp: Base-service
   sphinx: Others
   spice: Desktop
@@ -8892,14 +9440,15 @@
   sqlite: DB
   sqlite-jdbc: dev-utils
   sqljet: sig-Java
   squashfs-tools: Storage
   squashfuse: sig-HPC
   squid: Networking
   sratom: sig-epol
+  srdfdom: sig-ROS
   sros2: sig-ROS
   srt: Desktop
   sscg: Base-service
   ssh-key-dir: sig-CloudNative
   sshj: sig-Java
   sshpass: Application
   sslext: sig-Java
@@ -8926,14 +9475,15 @@
   stream-lib: sig-Java
   stress-ng: dev-utils
   stringtemplate: dev-utils
   stringtemplate4: Base-service
   stringtie: sig-bio
   strongswan: sig-security-facility
   struts: sig-Java
+  stubborn_buddies: sig-ROS
   stunnel: Application
   subscription-manager: sig-recycle
   subunit: Programming-language
   subversion: Base-service
   sudo: Base-service
   suitesparse: Others
   sundials: ai
@@ -8943,18 +9493,20 @@
   svnkit: sig-Java
   swagger-codegen: sig-recycle
   swagger-core: sig-Java
   swagger-spec-validator: sig-python-modules
   swagger-ui-bundle: sig-python-modules
   swig: Programming-language
   switcheroo-control: Desktop
+  swri_console: sig-ROS
   swt-chart: sig-Java
   swtpm: sig-security-facility
   symlinks: Base-service
   sysbench: dev-utils
+  sysboost: A-Tune
   syscare: sig-ops
   sysconftool: sig-epol
   syscontainer-tools: iSulad
   sysdig: A-Tune
   sysfsutils: Storage
   sysget: dev-utils
   syslinux: sig-OS-Builder
@@ -8966,28 +9518,31 @@
   sysstat: Base-service
   system-config-firewall: Private
   system-config-language: sig-UKUI
   system-config-printer: System-tool
   system-config-users: sig-mate-desktop
   system-config-users-docs: sig-mate-desktop
   system-storage-manager: Storage
+  system_modes: sig-ROS
+  systemabilitymgr_safwk: sig-distributed-middleware
   systemd: Base-service
   systemd-bootchart: dev-utils
   systemtap: Computing
   t-digest: Application
   t1utils: Application
   taglib: Desktop
   taglist-enable: Private
   tagsoup: sig-Java
   takari-archiver: sig-Java
   takari-incrementalbuild: sig-Java
   takari-lifecycle: sig-Java
   takari-plugin-testing: sig-Java
   takari-pom: sig-Java
   tang: System-tool
+  tango_icon_theme: sig-ROS
   tango_icons_vendor: sig-ROS
   tar: Base-service
   targetcli: Application
   tarsier: sig-high-performance-network
   tascalate-asmx: sig-Java
   tascalate-javaflow: sig-Java
   tbb: Programming-language
@@ -8997,22 +9552,26 @@
   tclx: Base-service
   tcmu-runner: Storage
   tcp_wrappers: Networking
   tcpdump: Networking
   tcsh: Base-service
   teckit: dev-utils
   telegraf: bigdata
+  teleop_tools: sig-ROS
+  teleop_twist_joy: sig-ROS
+  teleop_twist_keyboard: sig-ROS
   telepathy-filesystem: Desktop
   telepathy-glib: Desktop
   telepathy-logger: Desktop
   teleport: Networking
   telnet: Networking
   template-glib: GNOME
   tengine: Application
   tensorflow: ai
+  tensorrt_cmake_module: sig-ROS
   tepl: GNOME
   terminator: GNOME
   tesseract: Application
   tesseract-tessdata: Application
   test-interface: sig-Java
   test_interface_files: sig-ROS
   testng: Application
@@ -9045,15 +9604,17 @@
   texlive-split-t: Application
   texlive-split-u: Application
   texlive-split-v: Application
   texlive-split-w: Application
   texlive-split-x: Application
   texlive-split-y: Application
   texlive-split-z: Application
+  texworks: sig-desktop-apps
   tez: DB
+  tf_transformations: sig-ROS
   tftp: Networking
   thai-scalable-fonts: Desktop
   the_silver_searcher: dev-utils
   thin-provisioning-tools: Storage
   thonny: Desktop
   thredds: sig-Java
   three-eight-nine-ds-base: Application
@@ -9061,14 +9622,18 @@
   thunar-archive-plugin: xfce
   thunar-media-tags-plugin: xfce
   thunar-vcs-plugin: xfce
   thunar-volman: xfce
   thunarx-python: xfce
   thunderbird: sig-desktop-apps
   thx: Private
+  tiago_moveit_config: sig-ROS
+  tiago_navigation: sig-ROS
+  tiago_robot: sig-ROS
+  tiago_simulation: sig-ROS
   tibetan-machine-uni-fonts: Desktop
   tidb: DB
   tidy: Others
   tig: dev-utils
   tigervnc: Desktop
   tika: sig-Java
   tilda: sig-desktop-apps
@@ -9076,14 +9641,15 @@
   time: Base-service
   time-api: sig-Java
   time-shutdown: sig-UKUI
   timedatex: Base-service
   tint2: sig-cinnamon
   tinycdb: Runtime
   tinyproxy: Networking
+  tinytoml: Compiler
   tinyxml: sig-compat-winapp
   tinyxml2: Programming-language
   tinyxml2_vendor: sig-ROS
   tinyxml_vendor: sig-ROS
   tipcutils: Networking
   tito: dev-utils
   tix: Programming-language
@@ -9097,66 +9663,86 @@
   tog-pegasus: System-tool
   tokyocabinet: Base-service
   tomcat: Application
   tomcat-taglibs-parent: sig-Java
   tomcat-taglibs-standard: Application
   tomcatjss: Base-service
   toolbox: sig-CloudNative
+  topic_tools: sig-ROS
   torque: Application
   totem: Base-service
   totem-pl-parser: Base-service
   tpm-quote-tools: Application
   tpm-tools: Application
   tpm2-abrmd: sig-security-facility
   tpm2-abrmd-selinux: sig-recycle
+  tpm2-openssl: sig-security-facility
   tpm2-tools: sig-security-facility
   tpm2-tss: sig-security-facility
+  tpm2-tss-engine: sig-security-facility
   trace-cmd: Programming-language
   traceroute: Networking
+  tracetools_acceleration: sig-ROS
+  tracetools_analysis: sig-ROS
   tracker: Base-service
   tracker-miners: Base-service
   tracker3: GNOME
   tracker3-miners: GNOME
   trafficserver: Networking
   transfig: Application
   transmission: Desktop
+  transport_drivers: sig-ROS
   tre: Application
   tree: Storage
   treelayout: sig-Java
   trilead-putty-extension: sig-Java
   trilead-ssh2: sig-Java
+  trimal: sig-bio
   trimmomatic: sig-bio
   trinity: sig-QA
   trousers: Base-service
   tslib: sig-compat-winapp
   tss2: sig-security-facility
   ttembed: Application
   ttfautohint: Application
   ttmkfdir: Application
   tumbler: xfce
   tuna: Others
   tuned: Computing
+  turbojpeg_compressed_image_transport: sig-ROS
+  turtlebot3: sig-ROS
+  turtlebot3_msgs: sig-ROS
+  turtlebot3_simulations: sig-ROS
+  turtlebot4: sig-ROS
+  turtlebot4_desktop: sig-ROS
+  turtlebot4_robot: sig-ROS
   tuscany-sdo-java: Base-service
+  tvm_vendor: sig-ROS
+  twist_mux: sig-ROS
+  twist_stamper: sig-ROS
   twolame: Others
   txt2man: sig-epol
   txw2: sig-Java
   tycho: sig-Java
   tycho-extras: sig-Java
   typesafe-config: sig-Java
   tzdata: Computing
   u2f-hidraw-policy: Others
   uadk_engine: sig-AccLib
   ubackup: sig-Migration
+  ublox: sig-ROS
+  ublox_dgnss: sig-ROS
   uboot-tools: sig-OS-Builder
   ubu-keyring: Private
   ubuntukylin-default-settings: sig-UKUI
   uchardet: Others
   ucs-miscfixed-fonts: Others
   udisks2: Storage
   udisks2-qt5: Desktop
+  udp_msgs: sig-ROS
   uget: sig-desktop-apps
   uglify-js: sig-nodejs
   uglify-js1: sig-nodejs
   uhttpmock: GNOME
   uid_wrapper: Application
   uima-addons: sig-Java
   uima-parent-pom: sig-Java
@@ -9215,24 +9801,31 @@
   uom-lib: Base-service
   uom-parent: Base-service
   uom-se: dev-utils
   uom-systems: Base-service
   update-desktop-files: Desktop
   uperf: Application
   upower: Computing
+  ur_msgs: sig-ROS
   urdf: sig-ROS
+  urdf_parser_py: sig-ROS
   urdf_sim_tutorial: sig-ROS
+  urdf_test: sig-ROS
   urdf_tutorial: sig-ROS
   urdfdom: sig-ROS
   urdfdom_headers: sig-ROS
   urdfdom_py: sig-ROS
+  urg_c: sig-ROS
+  urg_node: sig-ROS
+  urg_node_msgs: sig-ROS
   uriparser: dev-utils
   urjtag: sig-embedded
   urlview: Others
   urw-base35-fonts: Desktop
+  usb_cam: sig-ROS
   usb_modeswitch: System-tool
   usb_modeswitch-data: Application
   usbguard: Application
   usbmuxd: Runtime
   usbredir: Storage
   usbutils: Storage
   usermode: Base-service
@@ -9250,67 +9843,81 @@
   vagrant-hostmanager: Virt
   vagrant-libvirt: Virt
   vagrant-lxc: Virt
   vala: GNOME
   valgrind: Programming-language
   vamp-plugin-sdk: Desktop
   vapoursynth: sig-epol
+  variants: sig-ROS
   varnish: System-tool
   vboot-utils: Base-service
   vcftools: sig-bio
   vconfig: Networking
   vdo: Runtime
   vdsm: oVirt
   vdsm-jsonrpc-java: oVirt
   velocity: sig-Java
   velocity-tools: sig-Java
+  velodyne: sig-ROS
+  velodyne_simulator: sig-ROS
   vhostmd: oVirt
   vid.stab: Desktop
   viewnior: Desktop
   vim: Base-service
   vim-airline: Application
   vim-ansible: Application
   vinagre: Application
   vino: Desktop
   virglrenderer: Virt
   virt-manager: oVirt
   virt-top: Private
   virt-viewer: oVirt
   virt-what: sig-CloudNative
+  vision_msgs: sig-ROS
+  vision_msgs_layers: sig-ROS
   vision_opencv: sig-ROS
+  visp: sig-ROS
   visualization_tutorials: sig-ROS
+  vitis_common: sig-ROS
   vkd3d: sig-compat-winapp
   vlc: sig-epol
   vmaf: sig-epol
   vmtop: Virt
   vnpy: sig-desktop-apps
   vo-amrwbenc: Desktop
   volume_key: Base-service
   vorbis-java: sig-Java
   vorbis-tools: Application
   voroplusplus: Application
+  vpnc: Networking
   vpnc-script: Application
+  vrpn: sig-ROS
   vsftpd: Networking
   vte: Application
   vte291: GNOME
   vtk: sig-epol
   vulkan-headers: Base-service
   vulkan-loader: Base-service
   waf: Programming-language
+  wall_follower_ros2: sig-ROS
+  warehouse_ros: sig-ROS
+  warehouse_ros_sqlite: sig-ROS
   watchdog: System-tool
   wavpack: Application
   wayland: Desktop
   wayland-protocols: Application
   wdiff: Application
   web-assets: Application
   webbench: dev-utils
   webkit2gtk3: Desktop
   webkit2gtk4: Desktop
   webkit2gtk5: Desktop
   webkit_dependency: sig-ROS
+  webots_ros2: sig-ROS
+  webp-pixbuf-loader: GNOME
   webrtc-audio-processing: Desktop
   weechat: Application
   weld-api: sig-Java
   weld-core: sig-Java
   weld-parent: sig-Java
   weston: Application
   wget: Networking
@@ -9364,14 +9971,15 @@
   xcb-util: Desktop
   xcb-util-cursor: Programming-language
   xcb-util-image: Programming-language
   xcb-util-keysyms: Programming-language
   xcb-util-renderutil: Programming-language
   xcb-util-wm: Programming-language
   xcb-util-xrm: Desktop
+  xchm: sig-desktop-apps
   xclip: Application
   xdelta: Programming-language
   xdg-dbus-proxy: Application
   xdg-desktop-portal: Desktop
   xdg-desktop-portal-gnome: GNOME
   xdg-desktop-portal-gtk: Application
   xdg-user-dirs: Desktop
@@ -9516,46 +10124,53 @@
   yakuake: sig-KDE
   yaml-cpp: Base-service
   yaml-cpp03: Base-service
   yaml_cpp_vendor: sig-ROS
   yapet: System-tool
   yasm: Base-service
   ycsb: bigdata
+  ydlidar-sdk: sig-ROS
   yecht: sig-Java
   yelp: Desktop
   yelp-tools: GNOME
   yelp-xsl: Desktop
   ykpers: dev-utils
   yocto-opkg-utils: sig-Yocto
   yocto-poky: sig-Yocto
   yocto-pseudo: sig-Yocto
+  yokadi: sig-desktop-apps
   yolov5: sig-ROS
   you-get: Application
   youker-assistant: sig-UKUI
   yp-tools: Desktop
   ypbind: Desktop
   ypserv: Desktop
   yum-metadata-parser: sig-recycle
   zabbix: Base-service
+  zathura: sig-desktop-apps
   zbar: Application
+  zbar_ros: sig-ROS
   zchunk: sig-CloudNative
   zd1211-firmware: Networking
+  zegrapher: sig-desktop-apps
   zenity: Desktop
+  zenoh-plugin-dds: sig-ROS
   zephyr: sig-Zephyr
   zeppelin: bigdata
   zerofree: Others
   zeromq: dev-utils
   zfs: sig-SDS
   zimg: Desktop
   zinc: sig-Java
   zincati: sig-CloudNative
   zip: Base-service
   zipkin: sig-epol
   zlib: Base-service
   zlog: sig-KIRAN-DESKTOP
+  zmqpp_vendor: sig-ROS
   znerd-oss-parent: sig-Java
   zookeeper: bigdata
   zopfli: Base-service
   zram-generator: sig-CloudNative
   zsh: Base-service
   zssh: Desktop
   zstd: Base-service
```

### Comparing `openstack-sig-tool-1.1.0/etc/openeuler_sig_repo.yaml` & `openstack-sig-tool-1.2.0/etc/openeuler_sig_repo.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 openeuler:
+  gostone: sig-openstack
   hostha: sig-openstack
   opensd: sig-openstack
   openstack: sig-openstack
   openstack-kolla-ansible-plugin: sig-openstack
   openstack-kolla-plugin: sig-openstack
   openstack-plugin: sig-openstack
   openstack-releases: sig-openstack
@@ -11,30 +12,36 @@
   ansible-lint: sig-openstack
   avro-python3: sig-openstack
   crudini: sig-openstack
   dibbler: sig-openstack
   diskimage-builder: sig-openstack
   gnocchi: sig-openstack
   google-api-core: sig-openstack
+  google-api-python-client: sig-openstack
   google-auth-httplib2: sig-openstack
   googleapis-common-protos: sig-openstack
   kafka-python: sig-openstack
   liberasurecode: sig-openstack
   loci: sig-openstack
   networking-baremetal: sig-openstack
   networking-generic-switch: sig-openstack
   novnc: sig-openstack
   opensd: sig-openstack
   openstack-aodh: sig-openstack
+  openstack-barbican: sig-openstack
   openstack-ceilometer: sig-openstack
   openstack-cinder: sig-openstack
+  openstack-cloudkitty: sig-openstack
   openstack-cyborg: sig-openstack
+  openstack-designate: sig-openstack
+  openstack-designate-ui: sig-openstack
   openstack-glance: sig-openstack
   openstack-heat: sig-openstack
   openstack-heat-agents: sig-openstack
+  openstack-heat-ui: sig-openstack
   openstack-helm: sig-openstack
   openstack-helm-images: sig-openstack
   openstack-helm-infra: sig-openstack
   openstack-horizon: sig-openstack
   openstack-ironic: sig-openstack
   openstack-ironic-inspector: sig-openstack
   openstack-ironic-python-agent: sig-openstack
@@ -42,62 +49,83 @@
   openstack-ironic-staging-drivers: sig-openstack
   openstack-keystone: sig-openstack
   openstack-kolla: sig-openstack
   openstack-kolla-ansible: sig-openstack
   openstack-kolla-ansible-plugin: sig-openstack
   openstack-kolla-plugin: sig-openstack
   openstack-macros: sig-openstack
+  openstack-magnum-ui: sig-openstack
+  openstack-manila: sig-openstack
+  openstack-masakari: sig-openstack
+  openstack-mistral: sig-openstack
+  openstack-mistral-ui: sig-openstack
   openstack-neutron: sig-openstack
+  openstack-neutron-dynamic-routing: sig-openstack
+  openstack-neutron-vpnaas: sig-openstack
   openstack-nova: sig-openstack
+  openstack-octavia: sig-openstack
+  openstack-octavia-ui: sig-openstack
   openstack-panko: sig-openstack
   openstack-placement: sig-openstack
   openstack-plugin: sig-openstack
   openstack-rally: sig-openstack
   openstack-rally-plugins: sig-openstack
   openstack-releases: sig-openstack
+  openstack-sahara-ui: sig-openstack
+  openstack-senlin: sig-openstack
   openstack-swift: sig-openstack
   openstack-tempest: sig-openstack
   openstack-trove: sig-openstack
+  openstack-vitrage-ui: sig-openstack
+  openstack-zaqar: sig-openstack
   os-net-config: sig-openstack
   ovn: sig-openstack
   python-3parclient: sig-openstack
   python-PyMI: sig-openstack
   python-URLObject: sig-openstack
   python-XStatic-Angular: sig-openstack
   python-XStatic-Angular-Bootstrap: sig-openstack
   python-XStatic-Angular-FileUpload: sig-openstack
   python-XStatic-Angular-Gettext: sig-openstack
   python-XStatic-Angular-Schema-Form: sig-openstack
   python-XStatic-Angular-lrdragndrop: sig-openstack
   python-XStatic-Bootstrap-Datepicker: sig-openstack
   python-XStatic-Bootstrap-SCSS: sig-openstack
   python-XStatic-D3: sig-openstack
+  python-XStatic-Dagre: sig-openstack
+  python-XStatic-Dagre-D3: sig-openstack
   python-XStatic-Font-Awesome: sig-openstack
+  python-XStatic-Graphlib: sig-openstack
   python-XStatic-Hogan: sig-openstack
   python-XStatic-JQuery-Migrate: sig-openstack
   python-XStatic-JQuery.TableSorter: sig-openstack
   python-XStatic-JQuery.quicksearch: sig-openstack
   python-XStatic-JSEncrypt: sig-openstack
   python-XStatic-Jasmine: sig-openstack
+  python-XStatic-Moment-Timezone: sig-openstack
   python-XStatic-Rickshaw: sig-openstack
   python-XStatic-Spin: sig-openstack
   python-XStatic-bootswatch: sig-openstack
   python-XStatic-jQuery: sig-openstack
   python-XStatic-jquery-ui: sig-openstack
+  python-XStatic-lodash: sig-openstack
   python-XStatic-mdi: sig-openstack
+  python-XStatic-moment: sig-openstack
   python-XStatic-objectpath: sig-openstack
   python-XStatic-roboto-fontface: sig-openstack
   python-XStatic-smart-table: sig-openstack
   python-XStatic-term.js: sig-openstack
   python-XStatic-tv4: sig-openstack
+  python-amqp: sig-openstack
   python-aodhclient: sig-openstack
   python-api-object-schema: sig-openstack
   python-argparse: sig-openstack
   python-arrow: sig-openstack
   python-async-generator: sig-openstack
+  python-autobahn: sig-openstack
   python-automaton: sig-openstack
   python-autopage: sig-openstack
   python-aws-sam-translator: sig-openstack
   python-aws-xray-sdk: sig-openstack
   python-awscrt: sig-openstack
   python-azure-core: sig-openstack
   python-barbicanclient: sig-openstack
@@ -106,43 +134,51 @@
   python-blazarclient: sig-openstack
   python-brotlipy: sig-openstack
   python-bunch: sig-openstack
   python-cairosvg: sig-openstack
   python-capacity: sig-openstack
   python-cassandra-driver: sig-openstack
   python-castellan: sig-openstack
+  python-ceilometerclient: sig-openstack
   python-ceilometermiddleware: sig-openstack
+  python-certifi: sig-openstack
   python-cfn-lint: sig-openstack
   python-cinder-tempest-plugin: sig-openstack
   python-cinderclient: sig-openstack
+  python-cinderlib: sig-openstack
   python-cliff: sig-openstack
+  python-cloudkittyclient: sig-openstack
   python-confetti: sig-openstack
   python-confget: sig-openstack
   python-confluent-kafka: sig-openstack
   python-congressclient: sig-openstack
   python-consul: sig-openstack
   python-cotyledon: sig-openstack
   python-covdefaults: sig-openstack
   python-coverage-enable-subprocess: sig-openstack
+  python-croniter: sig-openstack
   python-cursive: sig-openstack
   python-cyborgclient: sig-openstack
   python-debtcollector: sig-openstack
   python-designateclient: sig-openstack
   python-dfs-sdk: sig-openstack
   python-dib-utils: sig-openstack
   python-discover: sig-openstack
   python-django-configurations: sig-openstack
   python-doc8: sig-openstack
+  python-dogpile.cache: sig-openstack
   python-dracclient: sig-openstack
   python-easy-server: sig-openstack
   python-easy-vault: sig-openstack
+  python-edgegrid: sig-openstack
   python-elasticsearch2: sig-openstack
   python-elementpath: sig-openstack
   python-etcd3: sig-openstack
   python-etcd3gw: sig-openstack
+  python-falcon: sig-openstack
   python-flake8-docstrings: sig-openstack
   python-flake8-logging-format: sig-openstack
   python-flux: sig-openstack
   python-furo: sig-openstack
   python-futurist: sig-openstack
   python-fuzzywuzzy: sig-openstack
   python-glance-store: sig-openstack
@@ -150,23 +186,26 @@
   python-glanceclient: sig-openstack
   python-gnocchiclient: sig-openstack
   python-gossip: sig-openstack
   python-graphql-core: sig-openstack
   python-gremlinpython: sig-openstack
   python-grpcio-gcp: sig-openstack
   python-grpcio-status: sig-openstack
+  python-gunicorn: sig-openstack
   python-hacking: sig-openstack
   python-heat-cfntools: sig-openstack
   python-heatclient: sig-openstack
   python-hidapi: sig-openstack
+  python-hyperlink: sig-openstack
   python-ibm-db-sa: sig-openstack
   python-ibmcclient: sig-openstack
   python-infi.dtypes.iqn: sig-openstack
   python-infi.dtypes.wwn: sig-openstack
   python-infinisdk: sig-openstack
+  python-influxdb: sig-openstack
   python-intervals: sig-openstack
   python-ironic-inspector-client: sig-openstack
   python-ironic-lib: sig-openstack
   python-ironic-prometheus-exporter: sig-openstack
   python-ironic-tempest-plugin: sig-openstack
   python-ironic-ui: sig-openstack
   python-ironicclient: sig-openstack
@@ -182,43 +221,50 @@
   python-karborclient: sig-openstack
   python-kazoo: sig-openstack
   python-keystone-tempest-plugin: sig-openstack
   python-keystoneauth1: sig-openstack
   python-keystoneclient: sig-openstack
   python-keystonemiddleware: sig-openstack
   python-krest: sig-openstack
+  python-ldap3: sig-openstack
   python-ldappool: sig-openstack
   python-lefthandclient: sig-openstack
   python-lz4: sig-openstack
   python-magnumclient: sig-openstack
   python-manilaclient: sig-openstack
+  python-masakariclient: sig-openstack
   python-memory-profiler: sig-openstack
   python-microversion-parse: sig-openstack
+  python-mistral-lib: sig-openstack
   python-mistralclient: sig-openstack
   python-mitba: sig-openstack
+  python-monasca-statsd: sig-openstack
   python-monascaclient: sig-openstack
   python-moto: sig-openstack
   python-mox3: sig-openstack
   python-msrest: sig-openstack
   python-multiprocessing: sig-openstack
   python-murano-pkg-check: sig-openstack
   python-muranoclient: sig-openstack
   python-mypy-extensions: sig-openstack
+  python-natsort: sig-openstack
   python-netmiko: sig-openstack
   python-networking-ovn: sig-openstack
+  python-networking-sfc: sig-openstack
   python-neutron-lib: sig-openstack
   python-neutron-tempest-plugin: sig-openstack
   python-neutronclient: sig-openstack
   python-nocasedict: sig-openstack
   python-nocaselist: sig-openstack
   python-nodeenv: sig-openstack
   python-nosehtmloutput: sig-openstack
   python-nosexcover: sig-openstack
   python-novaclient: sig-openstack
   python-ntc-templates: sig-openstack
+  python-octavia-lib: sig-openstack
   python-octaviaclient: sig-openstack
   python-openstack-doc-tools: sig-openstack
   python-openstack.nose_plugin: sig-openstack
   python-openstackclient: sig-openstack
   python-openstackdocstheme: sig-openstack
   python-openstacksdk: sig-openstack
   python-opentracing: sig-openstack
@@ -259,14 +305,15 @@
   python-oslo.sphinx: sig-openstack
   python-oslo.upgradecheck: sig-openstack
   python-oslo.utils: sig-openstack
   python-oslo.versionedobjects: sig-openstack
   python-oslo.vmware: sig-openstack
   python-oslotest: sig-openstack
   python-osprofiler: sig-openstack
+  python-ovn-octavia-provider: sig-openstack
   python-ovsdbapp: sig-openstack
   python-pact: sig-openstack
   python-pathlib: sig-openstack
   python-pep257: sig-openstack
   python-pep8: sig-openstack
   python-pifpaf: sig-openstack
   python-pika: sig-openstack
@@ -276,24 +323,27 @@
   python-pre-commit: sig-openstack
   python-proboscis: sig-openstack
   python-proliantutils: sig-openstack
   python-psycopg2-binary: sig-openstack
   python-psycopg2cffi: sig-openstack
   python-purestorage: sig-openstack
   python-pycadf: sig-openstack
+  python-pycodestyle: sig-openstack
   python-pycountry: sig-openstack
   python-pydata-sphinx-theme: sig-openstack
   python-pydotplus: sig-openstack
   python-pyeclib: sig-openstack
   python-pyforge: sig-openstack
   python-pyghmi: sig-openstack
   python-pylama: sig-openstack
   python-pymongocrypt: sig-openstack
   python-pyodbc: sig-openstack
   python-pypowervm: sig-openstack
+  python-pyroute2: sig-openstack
+  python-pyrsistent: sig-openstack
   python-pyspnego: sig-openstack
   python-pytest-black: sig-openstack
   python-pytest-checkdocs: sig-openstack
   python-pytest-django: sig-openstack
   python-pytest-easy-server: sig-openstack
   python-pytest-enabler: sig-openstack
   python-pytest-env: sig-openstack
@@ -312,26 +362,28 @@
   python-requestsexceptions: sig-openstack
   python-requirementslib: sig-openstack
   python-responses: sig-openstack
   python-restructuredtext-lint: sig-openstack
   python-rsd-lib: sig-openstack
   python-rsdclient: sig-openstack
   python-rst.linker: sig-openstack
+  python-rtslib: sig-openstack
   python-rtslib-fb: sig-openstack
   python-ryu: sig-openstack
   python-saharaclient: sig-openstack
   python-scciclient: sig-openstack
   python-scripttest: sig-openstack
   python-searchlightclient: sig-openstack
   python-selenium: sig-openstack
   python-senlinclient: sig-openstack
   python-sentinels: sig-openstack
   python-setuptools-rust: sig-openstack
   python-soupsieve: sig-openstack
   python-sphinx-autodoc-typehints: sig-openstack
+  python-sphinx-feature-classification: sig-openstack
   python-sphinx-testing: sig-openstack
   python-sphinxcontrib-autoprogram: sig-openstack
   python-sphinxcontrib-programoutput: sig-openstack
   python-sqlalchemy-migrate: sig-openstack
   python-sshpubkeys: sig-openstack
   python-stestr: sig-openstack
   python-stevedore: sig-openstack
@@ -356,14 +408,15 @@
   python-tooz: sig-openstack
   python-towncrier: sig-openstack
   python-transaction: sig-openstack
   python-trio: sig-openstack
   python-trove-dashboard: sig-openstack
   python-trove-tempest-plugin: sig-openstack
   python-troveclient: sig-openstack
+  python-txaio: sig-openstack
   python-typed-ast: sig-openstack
   python-types-cryptography: sig-openstack
   python-types-enum34: sig-openstack
   python-types-ipaddress: sig-openstack
   python-types-paramiko: sig-openstack
   python-typing-extensions: sig-openstack
   python-uamqp: sig-openstack
@@ -378,14 +431,19 @@
   python-websockify: sig-openstack
   python-whereto: sig-openstack
   python-wmi: sig-openstack
   python-wsme: sig-openstack
   python-xattr: sig-openstack
   python-xclarityclient: sig-openstack
   python-xmlschema: sig-openstack
+  python-xstatic-angular-uuid: sig-openstack
+  python-xstatic-angular-vis: sig-openstack
+  python-xstatic-filesaver: sig-openstack
+  python-xstatic-js-yaml: sig-openstack
+  python-xstatic-json2yaml: sig-openstack
   python-yagot: sig-openstack
   python-yamllint: sig-openstack
   python-yamlloader: sig-openstack
   python-zVMCloudConnector: sig-openstack
   python-zake: sig-openstack
   python-zaqarclient: sig-openstack
   python-zunclient: sig-openstack
```

### Comparing `openstack-sig-tool-1.1.0/etc/openstack_release.yaml` & `openstack-sig-tool-1.2.0/etc/openstack_release.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -2007,28 +2007,28 @@
   zun-tempest-plugin: 4.3.0
   zun-ui: 7.0.0
 xena:
   adjutant-ui: 3.0.0
   ansible-role-atos-hsm: 2.0.0
   ansible-role-lunasa-hsm: 2.0.0
   ansible-role-thales-hsm: 2.0.0
-  aodh: 13.0.0
+  aodh: 13.1.0
   aodhclient: 2.3.1
   automaton: 2.4.0
   barbican: 13.0.2
   barbican_tempest_plugin: 1.5.0
   bifrost: 11.2.2
   blazar: 8.0.1
   blazar-dashboard: 6.0.0
   blazar-nova: 2.3.0
   blazar_tempest_plugin: 0.7.0
   castellan: 3.9.1
   ceilometer: 17.0.2
   ceilometermiddleware: 2.3.0
-  cinder: 19.2.0
+  cinder: 19.3.0
   cinder-tempest-plugin: 1.5.0
   cinderlib: 4.1.0
   cliff: 3.9.0
   cloudkitty: 15.0.1
   cloudkitty-dashboard: 13.0.0
   cloudkitty_tempest_plugin: 2.4.1
   compute-hyperv: 13.0.0
@@ -2043,43 +2043,43 @@
   freezer-dr: 11.0.0
   freezer-web-ui: 11.0.0
   freezer_tempest_plugin: 1.3.1
   glance: 23.1.0
   glance-tempest-plugin: 0.2.0
   glance_store: 2.7.1
   heat-agents: 3.0.0
-  heat-dashboard: 6.0.0
+  heat-dashboard: 6.0.1
   heat-tempest-plugin: 1.4.0
   heat-translator: 2.4.1
-  horizon: 20.1.3
-  ironic: 18.2.2
+  horizon: 20.1.4
+  ironic: 18.3.0
   ironic-inspector: 10.8.1
   ironic-lib: 5.0.1
   ironic-prometheus-exporter: 3.0.0
   ironic-python-agent: 8.2.3
   ironic-python-agent-builder: 3.0.0
   ironic-tempest-plugin: 2.3.1
   ironic-ui: 5.0.0
-  kayobe: 11.7.0
+  kayobe: 11.8.0
   kayobe-config: 11.7.0
   kayobe-config-dev: 11.5.0
   keystone: 20.0.1
   keystone_tempest_plugin: 0.8.0
   keystoneauth1: 4.4.0
   keystonemiddleware: 9.3.0
-  kolla: 13.9.0
-  kolla-ansible: 13.8.0
+  kolla: 13.10.0
+  kolla-ansible: 13.9.0
   kuryr-kubernetes: 5.0.0
   kuryr-lib: 2.4.0
   kuryr-libnetwork: 8.0.0
   kuryr-tempest-plugin: 0.11.0
-  magnum: 13.1.0
+  magnum: 13.1.1
   magnum-ui: 9.0.0
   magnum_tempest_plugin: 1.5.0
-  manila: 13.1.0
+  manila: 13.2.0
   manila-tempest-plugin: 1.6.0
   manila-ui: 6.0.0
   masakari: 12.0.3
   masakari-dashboard: 5.0.0
   masakari-monitors: 12.1.0
   metalsmith: 1.5.3
   mistral: 13.0.0
@@ -2103,27 +2103,27 @@
   networking-bagpipe: 15.0.0
   networking-baremetal: 5.0.0
   networking-bgpvpn: 15.0.0
   networking-generic-switch: 6.0.0
   networking-hyperv: 11.0.0
   networking-odl: 19.0.0
   networking-sfc: 13.0.0
-  neutron: 19.5.0
+  neutron: 19.7.0
   neutron-dynamic-routing: 19.1.1
-  neutron-lib: 2.15.3
+  neutron-lib: 2.15.4
   neutron-tempest-plugin: 1.7.0
   neutron-vpnaas: 19.0.1
   neutron-vpnaas-dashboard: 5.0.0
-  nova: 24.2.0
+  nova: 24.2.1
   octavia: 9.1.0
   octavia-dashboard: 8.0.1
   octavia-lib: 2.4.1
   octavia-tempest-plugin: 1.8.1
   openstack-cyborg: 7.0.1
-  openstack-heat: 17.0.1
+  openstack-heat: 17.0.2
   openstack-placement: 6.0.0
   openstacksdk: 0.59.0
   os-brick: 5.0.3
   os-ken: 2.1.1
   os-win: 5.5.0
   os_vif: 2.6.1
   osc-lib: 2.4.2
@@ -2141,54 +2141,54 @@
   oslo.serialization: 4.2.0
   oslo.service: 2.6.2
   oslo.upgradecheck: 1.4.0
   oslo.utils: 4.10.2
   oslo.versionedobjects: 2.5.0
   oslo.vmware: 3.9.3
   oswin-tempest-plugin: 1.3.0
-  ovn-octavia-provider: 1.2.0
+  ovn-octavia-provider: 1.3.1
   ovsdbapp: 1.12.3
   patrole: 0.13.0
   puppet-aodh: 19.4.0
-  puppet-barbican: 19.4.0
-  puppet-ceilometer: 19.4.0
-  puppet-cinder: 19.4.0
+  puppet-barbican: 19.4.1
+  puppet-ceilometer: 19.5.0
+  puppet-cinder: 19.5.0
   puppet-cloudkitty: 8.4.0
-  puppet-designate: 19.4.0
+  puppet-designate: 19.5.0
   puppet-ec2api: 19.4.0
   puppet-freezer: 19.1.0
-  puppet-glance: 19.4.0
-  puppet-gnocchi: 19.4.0
-  puppet-heat: 19.4.0
-  puppet-horizon: 19.4.0
-  puppet-ironic: 19.4.0
-  puppet-keystone: 19.4.0
+  puppet-glance: 19.5.0
+  puppet-gnocchi: 19.5.0
+  puppet-heat: 19.5.0
+  puppet-horizon: 19.5.0
+  puppet-ironic: 19.5.0
+  puppet-keystone: 19.5.0
   puppet-magnum: 19.4.0
-  puppet-manila: 19.4.0
-  puppet-mistral: 19.4.0
+  puppet-manila: 19.5.0
+  puppet-mistral: 19.4.1
   puppet-monasca: 8.1.0
   puppet-murano: 19.4.0
-  puppet-neutron: 19.4.0
-  puppet-nova: 19.4.0
-  puppet-octavia: 19.4.0
-  puppet-openstack_extras: 19.4.0
-  puppet-openstacklib: 19.4.0
-  puppet-oslo: 19.4.0
-  puppet-ovn: 19.4.0
-  puppet-placement: 6.4.0
+  puppet-neutron: 19.5.0
+  puppet-nova: 19.5.0
+  puppet-octavia: 19.5.0
+  puppet-openstack_extras: 19.4.1
+  puppet-openstacklib: 19.5.0
+  puppet-oslo: 19.5.0
+  puppet-ovn: 19.5.0
+  puppet-placement: 6.4.1
   puppet-qdr: 8.4.0
   puppet-rally: 7.4.0
   puppet-sahara: 19.4.0
   puppet-senlin: 6.4.0
-  puppet-swift: 19.4.0
+  puppet-swift: 19.5.0
   puppet-tacker: 19.4.0
-  puppet-tempest: 19.5.0
+  puppet-tempest: 19.5.1
   puppet-trove: 19.4.0
-  puppet-vitrage: 9.4.0
-  puppet-vswitch: 15.4.0
+  puppet-vitrage: 9.4.1
+  puppet-vswitch: 15.4.1
   puppet-watcher: 19.4.0
   puppet-zaqar: 19.4.0
   python-adjutant: 3.0.1
   python-adjutantclient: 0.9.0
   python-barbicanclient: 5.2.0
   python-blazarclient: 3.3.2
   python-brick-cinderclient-ext: 1.4.0
@@ -2199,15 +2199,15 @@
   python-freezerclient: 4.3.0
   python-glanceclient: 3.5.0
   python-heatclient: 2.4.0
   python-ironic-inspector-client: 4.6.0
   python-ironicclient: 4.8.2
   python-keystoneclient: 4.3.0
   python-magnumclient: 3.5.0
-  python-manilaclient: 3.0.2
+  python-manilaclient: 3.0.3
   python-masakariclient: 7.1.0
   python-mistralclient: 4.3.0
   python-monascaclient: 2.4.0
   python-muranoclient: 2.3.0
   python-neutronclient: 7.6.0
   python-novaclient: 17.6.0
   python-octaviaclient: 2.4.0
@@ -2276,38 +2276,38 @@
   barbican_tempest_plugin: 1.6.0
   bifrost: 14.0.0
   blazar: 9.0.0
   blazar-dashboard: 7.0.0
   blazar-nova: 2.5.0
   blazar_tempest_plugin: 0.8.0
   castellan: 3.10.2
-  ceilometer: 18.0.0
+  ceilometer: 18.1.0
   ceilometermiddleware: 2.4.1
-  cinder: 20.1.0
+  cinder: 20.3.0
   cinder-tempest-plugin: 1.6.0
   cinderlib: 4.2.0
   cliff: 3.10.1
   cloudkitty: 16.0.0
   cloudkitty-dashboard: 14.0.1
   cloudkitty_tempest_plugin: 2.5.0
   compute-hyperv: 14.0.0
   cyborg-tempest-plugin: 1.4.0
-  designate: 14.0.1
+  designate: 14.0.2
   designate-dashboard: 14.0.0
   designate-tempest-plugin: 0.13.0
   ec2-api: 14.0.1
   ec2api-tempest-plugin: 1.4.0
   freezer: 12.0.0
   freezer-api: 12.0.0
   freezer-dr: 12.0.0
   freezer-web-ui: 12.0.0
   freezer_tempest_plugin: 1.4.0
   glance: 24.2.0
   glance-tempest-plugin: 0.3.0
-  glance_store: 3.0.0
+  glance_store: 3.0.1
   heat-agents: 4.0.0
   heat-dashboard: 7.0.0
   heat-tempest-plugin: 1.5.0
   heat-translator: 2.5.0
   horizon: 22.1.0
   ironic: 20.1.1
   ironic-inspector: 10.11.0
@@ -2329,15 +2329,15 @@
   kuryr-kubernetes: 6.0.0
   kuryr-lib: 2.5.0
   kuryr-libnetwork: 9.0.0
   kuryr-tempest-plugin: 0.12.0
   magnum: 14.1.0
   magnum-ui: 10.0.0
   magnum_tempest_plugin: 1.6.0
-  manila: 14.0.1
+  manila: 14.1.0
   manila-tempest-plugin: 1.7.0
   manila-ui: 7.0.0
   masakari: 13.0.3
   masakari-dashboard: 6.0.0
   masakari-monitors: 13.1.0
   metalsmith: 1.6.3
   mistral: 14.0.0
@@ -2361,30 +2361,30 @@
   networking-bagpipe: 16.0.0
   networking-baremetal: 5.1.1
   networking-bgpvpn: 16.0.0
   networking-generic-switch: 6.1.0
   networking-hyperv: 12.0.0
   networking-odl: 20.0.0
   networking-sfc: 14.0.0
-  neutron: 20.2.0
-  neutron-dynamic-routing: 20.0.0
-  neutron-lib: 2.20.0
+  neutron: 20.3.1
+  neutron-dynamic-routing: 20.0.1
+  neutron-lib: 2.20.2
   neutron-tempest-plugin: 1.9.0
   neutron-vpnaas: 20.0.1
   neutron-vpnaas-dashboard: 6.0.0
-  nova: 25.1.0
+  nova: 25.2.0
   octavia: 10.0.0
   octavia-dashboard: 9.0.0
   octavia-lib: 2.5.0
   octavia-tempest-plugin: 1.9.0
   openstack-cyborg: 8.0.0
-  openstack-heat: 18.0.0
+  openstack-heat: 18.0.1
   openstack-placement: 7.0.0
   openstacksdk: 0.62.0
-  os-brick: 5.2.2
+  os-brick: 5.2.3
   os-ken: 2.3.1
   os-win: 5.6.0
   os_vif: 2.7.1
   osc-lib: 2.5.0
   osc-placement: 3.2.0
   oslo.cache: 2.10.1
   oslo.config: 8.8.0
@@ -2399,16 +2399,16 @@
   oslo.serialization: 4.3.0
   oslo.service: 2.8.0
   oslo.upgradecheck: 1.5.0
   oslo.utils: 4.12.3
   oslo.versionedobjects: 2.6.0
   oslo.vmware: 3.10.0
   oswin-tempest-plugin: 1.4.0
-  ovn-octavia-provider: 2.0.0
-  ovsdbapp: 1.15.2
+  ovn-octavia-provider: 2.1.1
+  ovsdbapp: 1.15.3
   patrole: 0.14.0
   puppet-aodh: 20.3.0
   puppet-barbican: 20.3.0
   puppet-ceilometer: 20.3.0
   puppet-cinder: 20.3.0
   puppet-cloudkitty: 9.3.0
   puppet-designate: 20.3.0
@@ -2454,15 +2454,15 @@
   python-freezerclient: 4.4.0
   python-glanceclient: 3.6.0
   python-heatclient: 2.5.1
   python-ironic-inspector-client: 4.7.1
   python-ironicclient: 4.11.0
   python-keystoneclient: 4.4.0
   python-magnumclient: 3.6.0
-  python-manilaclient: 3.3.1
+  python-manilaclient: 3.3.2
   python-masakariclient: 7.2.0
   python-mistralclient: 4.4.0
   python-monascaclient: 2.5.0
   python-muranoclient: 2.4.1
   python-neutronclient: 7.8.0
   python-novaclient: 17.7.0
   python-octaviaclient: 2.5.0
@@ -2532,17 +2532,17 @@
   barbican_tempest_plugin: 1.7.0
   bifrost: 15.0.0
   blazar: 10.0.0
   blazar-dashboard: 8.0.0
   blazar-nova: 2.6.1
   blazar_tempest_plugin: 0.9.0
   castellan: 4.0.0
-  ceilometer: 19.0.0
+  ceilometer: 19.1.0
   ceilometermiddleware: 3.0.0
-  cinder: 21.1.0
+  cinder: 21.3.0
   cinder-tempest-plugin: 1.7.2
   cinderlib: 5.0.0
   cliff: 4.0.0
   cloudkitty: 17.0.0
   cloudkitty-dashboard: 15.0.0
   cloudkitty_tempest_plugin: 2.6.0
   compute-hyperv: 15.0.0
@@ -2555,15 +2555,15 @@
   freezer: 13.0.0
   freezer-api: 13.0.0
   freezer-dr: 13.0.0
   freezer-web-ui: 13.0.0
   freezer_tempest_plugin: 2.0.0
   glance: 25.1.0
   glance-tempest-plugin: 0.5.0
-  glance_store: 4.1.0
+  glance_store: 4.1.1
   heat-agents: 5.0.0
   heat-dashboard: 8.0.0
   heat-tempest-plugin: 1.6.0
   heat-translator: 2.6.0
   horizon: 23.0.0
   ironic: 21.1.0
   ironic-inspector: 11.1.0
@@ -2585,15 +2585,15 @@
   kuryr-kubernetes: 7.0.0
   kuryr-lib: 2.6.0
   kuryr-libnetwork: 10.0.0
   kuryr-tempest-plugin: 0.13.0
   magnum: 15.0.1
   magnum-ui: 11.0.0
   magnum_tempest_plugin: 1.7.0
-  manila: 15.1.0
+  manila: 15.2.0
   manila-tempest-plugin: 1.10.0
   manila-ui: 8.0.0
   masakari: 14.0.2
   masakari-dashboard: 7.0.0
   masakari-monitors: 14.0.0
   metalsmith: 1.8.0
   mistral: 15.0.0
@@ -2617,57 +2617,57 @@
   networking-bagpipe: 17.0.0
   networking-baremetal: 6.0.0
   networking-bgpvpn: 17.0.0
   networking-generic-switch: 7.0.0
   networking-hyperv: 13.0.0
   networking-odl: 21.0.0
   networking-sfc: 15.0.0
-  neutron: 21.0.0
-  neutron-dynamic-routing: 21.0.0
+  neutron: 21.1.1
+  neutron-dynamic-routing: 21.0.1
   neutron-fwaas: 17.0.0
   neutron-fwaas-dashboard: 4.0.0
-  neutron-lib: 3.1.0
+  neutron-lib: 3.1.2
   neutron-tempest-plugin: 2.0.0
   neutron-vpnaas: 21.0.0
   neutron-vpnaas-dashboard: 7.0.0
-  nova: 26.1.0
+  nova: 26.2.0
   octavia: 11.0.0
   octavia-dashboard: 10.0.0
   octavia-lib: 3.1.0
   octavia-tempest-plugin: 2.0.0
   openstack-cyborg: 9.0.0
-  openstack-heat: 19.0.0
+  openstack-heat: 19.0.1
   openstack-placement: 8.0.0
   openstack-venus: 1.0.0
   openstacksdk: 0.101.0
-  os-brick: 6.1.0
+  os-brick: 6.1.1
   os-ken: 2.5.0
   os-win: 5.7.1
   os_vif: 3.0.0
   osc-lib: 2.6.2
   osc-placement: 4.0.0
   oslo.cache: 3.2.0
   oslo.config: 9.0.0
   oslo.context: 5.0.0
-  oslo.db: 12.1.0
+  oslo.db: 12.1.1
   oslo.limit: 2.0.1
   oslo.messaging: 14.0.0
-  oslo.metrics: 0.5.0
+  oslo.metrics: 0.5.1
   oslo.middleware: 5.0.0
   oslo.policy: 4.0.0
   oslo.privsep: 3.0.1
   oslo.serialization: 5.0.0
   oslo.service: 3.0.0
   oslo.upgradecheck: 2.0.0
-  oslo.utils: 6.0.1
+  oslo.utils: 6.0.2
   oslo.versionedobjects: 3.0.1
   oslo.vmware: 4.0.1
   oswin-tempest-plugin: 2.0.0
-  ovn-octavia-provider: 3.0.0
-  ovsdbapp: 2.1.0
+  ovn-octavia-provider: 3.1.1
+  ovsdbapp: 2.1.1
   patrole: 0.15.0
   puppet-aodh: 21.0.0
   puppet-barbican: 21.0.0
   puppet-ceilometer: 21.0.0
   puppet-cinder: 21.0.0
   puppet-cloudkitty: 10.0.0
   puppet-designate: 21.0.0
@@ -2702,26 +2702,26 @@
   puppet-watcher: 21.0.0
   puppet-zaqar: 21.0.0
   python-adjutant: 5.0.0
   python-adjutantclient: 0.11.0
   python-barbicanclient: 5.4.0
   python-blazarclient: 3.5.0
   python-brick-cinderclient-ext: 2.0.0
-  python-cinderclient: 9.1.0
+  python-cinderclient: 9.1.1
   python-cloudkittyclient: 4.6.0
   python-cyborgclient: 2.0.0
   python-designateclient: 5.0.0
   python-freezerclient: 5.0.0
   python-glanceclient: 4.1.0
   python-heatclient: 3.1.0
   python-ironic-inspector-client: 4.8.0
   python-ironicclient: 5.0.1
   python-keystoneclient: 5.0.1
   python-magnumclient: 4.0.0
-  python-manilaclient: 4.1.1
+  python-manilaclient: 4.1.2
   python-masakariclient: 8.0.0
   python-mistralclient: 4.5.0
   python-monascaclient: 2.6.0
   python-muranoclient: 2.5.0
   python-neutronclient: 8.1.0
   python-novaclient: 18.1.0
   python-octaviaclient: 3.1.0
```

### Comparing `openstack-sig-tool-1.1.0/etc/package.spec.j2` & `openstack-sig-tool-1.2.0/etc/package.spec.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 %global _empty_manifest_terminate_build 0
+%global common_description \
+{{ description }}
+
 Name:           {{ spec_name }}
 Version:        {{ version }}
 Release:        1
 Summary:        {{ pkg_summary }}
 License:        {{ pkg_license }}
 URL:            {{ pkg_home }}
 Source0:        {{ source_url }}
 {% if not build_arch %}
 BuildArch:      noarch
 {% endif %}
 %description
-{{ description }}
+%{common_description}
 
 %package -n {{ pkg_name }}
 Summary:        {{ pkg_summary }}
 Provides:       {{ provides }}
 {% if base_build_requires %}
 # Base build requires
 {% for br in base_build_requires %}
@@ -46,30 +49,38 @@
 {% if test_requires %}
 # Tests running requires
 {% for tr in test_requires %}
 Requires:       {{ tr }}
 {% endfor %}
 {% endif %}
 %description -n {{ pkg_name }}
-{{ description }}
+%{common_description}
 
 %package help
 Summary:        {{ pkg_summary }}
 Provides:       {{ pkg_name }}-doc
 %description help
-{{ description }}
+%{common_description}
 
 %prep
 %autosetup -n {{ source_file_dir }}
 
 %build
+{% if is_pyproject %}
+%pyproject_build
+{% else %}
 %py3_build
+{% endif %}
 
 %install
+{% if is_pyproject %}
+%pyproject_install
+{% else %}
 %py3_install
+{% endif %}
 
 install -d -m755 %{buildroot}/%{_pkgdocdir}
 if [ -d doc ]; then cp -arf doc %{buildroot}/%{_pkgdocdir}; fi
 if [ -d docs ]; then cp -arf docs %{buildroot}/%{_pkgdocdir}; fi
 if [ -d example ]; then cp -arf example %{buildroot}/%{_pkgdocdir}; fi
 if [ -d examples ]; then cp -arf examples %{buildroot}/%{_pkgdocdir}; fi
 pushd %{buildroot}
@@ -91,16 +102,20 @@
 fi
 popd
 mv %{buildroot}/filelist.lst .
 mv %{buildroot}/doclist.lst .
 
 {% if add_check %}
 %check
+{% if is_pyproject %}
+pytest
+{% else %}
 %{__python3} setup.py test
 {% endif %}
+{% endif %}
 
 %files -n {{ pkg_name }} -f filelist.lst
 {% if not build_arch %}
 %dir %{python3_sitelib}/*
 {% else %}
 %dir %{python3_sitearch}/*
 {% endif %}
@@ -112,13 +127,12 @@
 * {{ today }} OpenStack_SIG <openstack@openeuler.org> - {{ version }}-1
 {% if old_changelog %}
 - {{ up_down_grade }} package {{ pkg_name }} to version {{ version }}
 {% else %}
 - Init package {{ pkg_name }} of version {{ version }}
 {% endif %}
 
-
 {% if old_changelog %}
 {% for cl in old_changelog %}
 {{ cl }}
 {% endfor %}
 {% endif %}
```

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/aodh.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/aodh.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/ceilometer.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/ceilometer.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/cinder.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/cinder.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/cleanup.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/cleanup.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/cyborg.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/cyborg.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/entry.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/entry.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/glance.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/glance.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/gnocchi.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/gnocchi.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/heat.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/heat.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/horizon.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/horizon.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/init.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/init.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/keystone.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/keystone.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/mariadb.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/mariadb.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/neutron.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/neutron.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/nova.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/nova.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/placement.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/placement.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/pre.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/pre.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 - name: Config OpenStack yum repo
   hosts: all
   become: true
   tasks:
+    - name: Update yum mirror - huaweicloud
+      shell: |
+        sed -i "s/repo.openeuler.org/repo.huaweicloud.com\/openeuler/g" /etc/yum.repos.d/openEuler.repo
+      when: "'{{ provider }}' == 'huaweicloud'"
+
     - name: Install openstack-releases package
       yum:
         name:
         - openstack-release-{{ openstack_release }}
       ignore_errors: yes
 
-    # huaweicloud mirror is broken. Enable this task once it works.
-    # - name: Update yum mirror
-    #   shell: |
-    #     sed -i "s/repo.openeuler.org/repo.huaweicloud.com/g" /etc/yum.repos.d/openEuler.repo
-    #     sed -i "s/repo.openeuler.org/repo.huaweicloud.com/g" /etc/yum.repos.d/openstack-{{ openstack_release }}.repo
-    #   ignore_errors: yes
+    - name: Update yum mirror - huaweicloud
+      shell: |
+        sed -i "s/repo.openeuler.org/repo.huaweicloud.com\/openeuler/g" /etc/yum.repos.d/openstack-{{ openstack_release }}.repo
+      ignore_errors: yes
+      when: "'{{ provider }}' == 'huaweicloud'"
 
 - name: Config mutual trust for root
   hosts: all
   become: true
   tasks:
     - name: Copy file for hosts
       copy:
```

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/roles/init_database/tasks/main.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/roles/init_database/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/swift.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/swift.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/test.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/test.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/etc/playbooks/trove.yaml` & `openstack-sig-tool-1.2.0/etc/playbooks/trove.yaml`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/commands/dependence/cli.py` & `openstack-sig-tool-1.2.0/oos/commands/dependence/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,15 @@
         with open(self.output, "w") as csv_file:
             writer=csv.writer(csv_file)
             writer.writerow(["Project Name", "openEuler Repo", "SIG", "Repo version",
                 "Required (Min) Version", "lt Version", "ne Version", "Upper Version", "Status",
                 "Requires", "Depth"])
             for file_name in file_list:
                 with open(self.location + '/' + file_name, 'r', encoding='utf8') as fp:
-                    if file_name == 'unknown':
-                        project_list = [{'name': project} for project in fp.read().splitlines()]
-                    else:
+                    if file_name != 'unknown':
                         project_list = [json.load(fp)]
                 for project_dict in project_list:
                     project_name = project_dict['name']
                     version_dict = project_dict.get('version_dict')
                     project_version = version_dict['version'] if version_dict else ''
                     project_eq_version = version_dict['eq_version'] if version_dict else ''
                     project_lt_version = version_dict['lt_version'] if version_dict else ''
```

### Comparing `openstack-sig-tool-1.1.0/oos/commands/environment/cli.py` & `openstack-sig-tool-1.2.0/oos/commands/environment/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,17 +103,20 @@
               help='OpenStack release to install, like train, wallaby...')
 @click.argument('target')
 def setup(release, target):
     oe = sqlite_ops.get_target_column(target, 'openEuler_release')[0][0]
     if release.lower() not in constants.OE_OS_RELEASE[oe]:
         print("%s does not support openstack %s" % (oe, release))
         return
+    provider_name = sqlite_ops.get_target_column(target, 'provider')[0][0]
 
     os.environ.setdefault('OpenStack_Release', release.lower())
     os.environ.setdefault('keypair_dir', KEY_DIR)
+    os.environ.setdefault('provider', provider_name)
+
     _run_action(target, 'entry')
     sql = 'UPDATE resource SET openstack_release=? WHERE name=?'
     sqlite_ops.exe_sql(sql, (release.lower(), target))
 
 
 @group.command(name='init',
                help='Initialize the base OpenStack resource for the Cluster')
```

### Comparing `openstack-sig-tool-1.1.0/oos/commands/environment/constants.py` & `openstack-sig-tool-1.2.0/oos/commands/environment/constants.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/commands/environment/provider.py` & `openstack-sig-tool-1.2.0/oos/commands/environment/provider.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/commands/environment/sqlite_ops.py` & `openstack-sig-tool-1.2.0/oos/commands/environment/sqlite_ops.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/commands/repo/cli.py` & `openstack-sig-tool-1.2.0/oos/commands/repo/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 
 import os
-import shutil
 import subprocess
 
 import click
 import pandas
 import yaml
 
 from oos.commands.repo.repo_class import PkgGitRepo
```

### Comparing `openstack-sig-tool-1.1.0/oos/commands/repo/repo_class.py` & `openstack-sig-tool-1.2.0/oos/commands/repo/repo_class.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/commands/spec/cli.py` & `openstack-sig-tool-1.2.0/oos/commands/spec/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 import click
 
 from oos.commands.spec.spec_class import RPMSpec
 from oos.commands.spec.spec_class import RPMSpecBuild
 
 
 def _get_old_spec_info(name):
-    spec_f = os.path.join(f'python-{name}.spec')
-    try:
-        with open(spec_f) as f_spec:
-            lines = f_spec.readlines()
-    except FileNotFoundError:
-        raise click.ClickException(f"Can not find the spec file {spec_f}")
+    names = [os.path.join(f'{name}.spec'), os.path.join(f'python-{name}.spec')]
+    for spec_name in names:
+        try:
+            with open(spec_name) as f_spec:
+                lines = f_spec.readlines()
+                break
+        except FileNotFoundError:
+            continue
+    else:
+        raise click.ClickException(f"Can not find the spec file.")
 
     noarch = False
     check = False
 
     for l_num, line in enumerate(lines):
         if 'BuildArch:' in line and 'noarch' in line:
             noarch = True
@@ -37,17 +41,18 @@
 
 
 @group.command(name='create', help='Create RPM spec for common python library')
 @click.option("-n", "--name", required=True, help="Name of package to build")
 @click.option("-v", "--version", default='latest', help="Package version, deault is the newest version")
 @click.option("-a", "--arch", is_flag=True, help="Build module with arch, noarch by default.")
 @click.option("-nc", "--no-check", is_flag=True, help="Do not add %check step in spec")
+@click.option("-pp", "--pyproject", is_flag=True, help="Generate the spec for pyproject project")
 @click.option("-o", "--output", help="Specify output file of generated Spec")
-def create(name, version, arch, no_check, output):
-    spec = RPMSpec(name, version, arch, not no_check)
+def create(name, version, arch, no_check, pyproject, output):
+    spec = RPMSpec(name, version, arch, not no_check, pyproject=pyproject)
     spec.generate_spec(output)
 
 
 @group.command(name='update', help='Update(upgrade or downgrade) RPM spec for the python library')
 @click.option("-n", "--name", required=True, help="Name of package to build")
 @click.option("-v", "--version", default='latest', help="Package version, deault is the newest version")
 @click.option("-o", "--output", help="Specify output file of generated Spec")
```

### Comparing `openstack-sig-tool-1.1.0/oos/commands/spec/spec_class.py` & `openstack-sig-tool-1.2.0/oos/commands/spec/spec_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 from oos.common import CONSTANTS
 from oos.common import SPEC_TEMPLATE_DIR
 from oos.common import pypi
 
 
 class RPMSpec(object):
     def __init__(self, pypi_name, version='latest', arch=None, add_check=True,
-                 old_changelog=None, old_version=None):
+                 old_changelog=None, old_version=None, pyproject=None):
         self.pypi_name = pypi_name
         # use 'latest' as version if version is NaN
         self.version = 'latest' if version != version else version
         self.arch = arch
         self.old_changelog = old_changelog
         self.old_version = old_version
         self.spec_path = ''
         self.source_path = ''
         self.add_check = add_check
+        self.is_pyproject = pyproject
 
         self._pypi_json = None
         self._spec_name = ""
         self._pkg_name = ""
         self._pkg_summary = ""
         self._pkg_home = ""
         self._source_url = ""
@@ -150,20 +151,18 @@
             if url_info["packagetype"] == "sdist":
                 self._source_file = url_info["filename"]
                 self._source_url = url_info["url"]
         if self._source_file:
             self._source_file_dir = self._source_file.partition(
                 '-' + self.version_num)[0] + '-%{version}'
 
-    def _get_description(self, shorten=True):
-        if self.pypi_name in CONSTANTS['pkg_description']:
-            return CONSTANTS['pkg_description'][self.pypi_name]
+    def _get_description(self):
+        # if self.pypi_name in CONSTANTS['pkg_description']:
+        #     return CONSTANTS['pkg_description'][self.pypi_name]
         org_description = self.pypi_json["info"]["description"]
-        if not shorten:
-            return org_description
         cut_dot = org_description.find('.', 80 * 8)
         cut_br = org_description.find('\n', 80 * 8)
         if cut_dot > -1:
             shorted = org_description[:cut_dot + 1]
         elif cut_br > -1:
             shorted = org_description[:cut_br]
         else:
@@ -177,15 +176,15 @@
                           # very short lines, typically titles
                           re.sub('((\r?\n)|^).{0,8}((\r?\n)|$)', '',
                                  # PyPI's version and downloads tags
                                  re.sub(
                                      '((\r*.. image::|:target:) https?|'
                                      '(:align:|:alt:))[^\n]*\n', '',
                                      shorted)))))
-        return '\n'.join(textwrap.wrap(spec_description, 80))
+        return ' \\\n'.join(textwrap.wrap(spec_description, 80))
 
     def _parse_requires(self):
         self._base_build_requires = []
         self._dev_requires = []
         self._test_requires = []
         self._base_build_requires = ['python3-devel', 'python3-setuptools',
                                      'python3-pbr', 'python3-pip',
@@ -248,14 +247,15 @@
                          'provides': self._get_provide_name(),
                          'base_build_requires': self._base_build_requires,
                          'dev_requires': self._dev_requires,
                          'test_requires': test_requires,
                          'description': self._get_description(),
                          'today': datetime.date.today().strftime("%a %b %d %Y"),
                          'add_check': self.add_check,
+                         'is_pyproject': self.is_pyproject,
                          "source_file_dir": self._source_file_dir,
                          "old_changelog": self.old_changelog,
                          "up_down_grade": up_down_grade,
                          }
         output = template.render(template_vars)
         with open(spec_path, 'w') as f:
             f.write(output)
```

### Comparing `openstack-sig-tool-1.1.0/oos/common/__init__.py` & `openstack-sig-tool-1.2.0/oos/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/common/click_custom.py` & `openstack-sig-tool-1.2.0/oos/common/click_custom.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/common/gitee.py` & `openstack-sig-tool-1.2.0/oos/common/gitee.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 
+from packaging import version as p_version
 import requests
 
 
 def get_gitee_project_tree(owner, project, branch, access_token=None):
     """Get project content tree from gitee"""
     headers = {
         'Content-Type': 'application/json;charset=UTF-8',
@@ -30,14 +31,18 @@
                 sub_str = file['path'].rsplit('.', 1)[0]
             if '-' in sub_str:
                 version = sub_str.rsplit('-', 1)[1].strip('v')
             elif '_' in sub_str:
                 version = sub_str.rsplit('_', 1)[1].strip('v')
             else:
                 version = sub_str.strip('v')
+            try:
+                p_version.parse(version)
+            except p_version.InvalidVersion:
+                continue
             break
 
     return version
 
 
 def has_branch(owner, project, branch, access_token=None):
     """Check if the repo has specified branch"""
@@ -53,13 +58,13 @@
         return False
     else:
         return True
 
 
 def get_user_info(token):
     user_info_url = 'https://gitee.com/api/v5/user?access_token=%s' % token
-    user_info = requests.request('GET', user_info_url).json()
+    user_info = requests.get(user_info_url).json()
     gitee_user = user_info['login']
     if not user_info.get('email'):
         return gitee_user, None
     gitee_email = user_info['email'] if '@' in user_info['email'] else None
     return gitee_user, gitee_email
```

### Comparing `openstack-sig-tool-1.1.0/oos/common/pypi.py` & `openstack-sig-tool-1.2.0/oos/common/pypi.py`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/oos/common/utils.py` & `openstack-sig-tool-1.2.0/oos/common/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import os
-
 from oos.common import CONSTANTS
 from oos.common import OPENEULER_REPO
 
 
 def get_openeuler_repo_name_and_sig(pypi_name):
     openeuler_name = CONSTANTS['pypi2reponame'].get(pypi_name, pypi_name)
-    if OPENEULER_REPO.get(openeuler_name):
-        return openeuler_name, OPENEULER_REPO[openeuler_name]
-    elif OPENEULER_REPO.get('python-' + openeuler_name):
+    if OPENEULER_REPO.get('python-' + openeuler_name):
         return 'python-'+openeuler_name, OPENEULER_REPO['python-'+openeuler_name]
+    elif OPENEULER_REPO.get(openeuler_name):
+        return openeuler_name, OPENEULER_REPO[openeuler_name]
     elif OPENEULER_REPO.get('openstack-'+openeuler_name):
         return 'openstack-'+openeuler_name, OPENEULER_REPO['openstack-'+openeuler_name]
     else:
         return '', ''
```

### Comparing `openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/PKG-INFO` & `openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-sig-tool
-Version: 1.1.0
+Version: 1.2.0
 Summary: The command line tool for openEuler OpenStack SIG
 Home-page: https://gitee.com/openeuler/openstack/
 Author: openEuler OpenStack SIG
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: AUTHORS
 
 # OpenStack SIG 开发工具
 
 oos(openEuler OpenStack SIG)是OpenStack SIG提供的命令行工具。该工具为OpenStack SIG开发提供了若干功能。包括
 
 1. 自动生成、更新RPM Spec
 2. 自动分析OpenStack软件包依赖
```

### Comparing `openstack-sig-tool-1.1.0/openstack_sig_tool.egg-info/SOURCES.txt` & `openstack-sig-tool-1.2.0/openstack_sig_tool.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,9 @@
 openstack_sig_tool.egg-info/PKG-INFO
 openstack_sig_tool.egg-info/SOURCES.txt
 openstack_sig_tool.egg-info/dependency_links.txt
 openstack_sig_tool.egg-info/entry_points.txt
 openstack_sig_tool.egg-info/not-zip-safe
 openstack_sig_tool.egg-info/pbr.json
 openstack_sig_tool.egg-info/requires.txt
-openstack_sig_tool.egg-info/top_level.txt
+openstack_sig_tool.egg-info/top_level.txt
+test/test_cli.py
```

### Comparing `openstack-sig-tool-1.1.0/setup.cfg` & `openstack-sig-tool-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstack-sig-tool-1.1.0/setup.py` & `openstack-sig-tool-1.2.0/setup.py`

 * *Files identical despite different names*

