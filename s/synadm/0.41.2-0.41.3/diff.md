# Comparing `tmp/synadm-0.41.2.tar.gz` & `tmp/synadm-0.41.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synadm-0.41.2.tar", last modified: Thu Apr  6 17:28:00 2023, max compression
+gzip compressed data, was "synadm-0.41.3.tar", last modified: Wed Jun 14 07:10:20 2023, max compression
```

## Comparing `synadm-0.41.2.tar` & `synadm-0.41.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.623012 synadm-0.41.2/
--rw-r--r--   0 jackson    (501) staff       (20)      245 2023-04-06 17:26:21.000000 synadm-0.41.2/.bumpversion.cfg
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.612621 synadm-0.41.2/.github/
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.616376 synadm-0.41.2/.github/workflows/
--rw-r--r--   0 jackson    (501) staff       (20)      435 2023-03-15 12:29:09.000000 synadm-0.41.2/.github/workflows/lint.yaml
--rw-r--r--   0 jackson    (501) staff       (20)     2735 2023-03-28 18:08:19.000000 synadm-0.41.2/.github/workflows/release.yaml
--rw-r--r--   0 jackson    (501) staff       (20)       96 2023-03-28 18:08:19.000000 synadm-0.41.2/.gitignore
--rw-r--r--   0 jackson    (501) staff       (20)    35148 2023-02-24 10:57:22.000000 synadm-0.41.2/LICENSE
--rw-r--r--   0 jackson    (501) staff       (20)      646 2023-02-24 10:57:22.000000 synadm-0.41.2/Makefile
--rw-r--r--   0 jackson    (501) staff       (20)    14558 2023-04-06 17:28:00.622836 synadm-0.41.2/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)    13504 2023-03-28 18:08:19.000000 synadm-0.41.2/README.md
--rwxr-xr-x   0 jackson    (501) staff       (20)      814 2023-02-24 10:57:22.000000 synadm-0.41.2/bump.sh
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.612749 synadm-0.41.2/doc/
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.619104 synadm-0.41.2/doc/source/
--rw-r--r--   0 jackson    (501) staff       (20)     2554 2023-04-06 17:26:21.000000 synadm-0.41.2/doc/source/conf.py
--rw-r--r--   0 jackson    (501) staff       (20)      486 2023-03-25 16:54:14.000000 synadm-0.41.2/doc/source/index.rst
--rw-r--r--   0 jackson    (501) staff       (20)      303 2023-03-15 12:29:09.000000 synadm-0.41.2/doc/source/index_cli_reference.rst
--rw-r--r--   0 jackson    (501) staff       (20)      149 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/index_modules.rst
--rw-r--r--   0 jackson    (501) staff       (20)      110 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.config.rst
--rw-r--r--   0 jackson    (501) staff       (20)       86 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.group.rst
--rw-r--r--   0 jackson    (501) staff       (20)       96 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.history.rst
--rw-r--r--   0 jackson    (501) staff       (20)       92 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.matrix.rst
--rw-r--r--   0 jackson    (501) staff       (20)       86 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.media.rst
--rw-r--r--   0 jackson    (501) staff       (20)       92 2023-03-15 12:29:09.000000 synadm-0.41.2/doc/source/synadm.cli.notice.rst
--rw-r--r--   0 jackson    (501) staff       (20)       92 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.regtok.rst
--rw-r--r--   0 jackson    (501) staff       (20)       81 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.room.rst
--rw-r--r--   0 jackson    (501) staff       (20)       88 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.root.rst
--rw-r--r--   0 jackson    (501) staff       (20)       81 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.cli.user.rst
--rw-r--r--   0 jackson    (501) staff       (20)      948 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.module.cli.rst
--rw-r--r--   0 jackson    (501) staff       (20)      427 2023-02-24 10:57:22.000000 synadm-0.41.2/doc/source/synadm.module.rst
--rwxr-xr-x   0 jackson    (501) staff       (20)      424 2023-04-06 17:26:21.000000 synadm-0.41.2/pypi.sh
--rw-r--r--   0 jackson    (501) staff       (20)       67 2023-02-24 10:57:22.000000 synadm-0.41.2/requirements.txt
--rwxr-xr-x   0 jackson    (501) staff       (20)      536 2023-02-24 10:57:22.000000 synadm-0.41.2/retag.sh
--rw-r--r--   0 jackson    (501) staff       (20)       38 2023-04-06 17:28:00.623052 synadm-0.41.2/setup.cfg
--rwxr-xr-x   0 jackson    (501) staff       (20)     2247 2023-04-06 17:26:21.000000 synadm-0.41.2/setup.py
--rw-r--r--   0 jackson    (501) staff       (20)       60 2023-02-24 10:57:22.000000 synadm-0.41.2/sphinx_requirements.txt
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.619338 synadm-0.41.2/synadm/
--rw-r--r--   0 jackson    (501) staff       (20)        0 2023-02-24 10:57:22.000000 synadm-0.41.2/synadm/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)    53122 2023-04-06 17:26:21.000000 synadm-0.41.2/synadm/api.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.622591 synadm-0.41.2/synadm/cli/
--rw-r--r--   0 jackson    (501) staff       (20)    20407 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/__init__.py
--rw-r--r--   0 jackson    (501) staff       (20)     1458 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/group.py
--rw-r--r--   0 jackson    (501) staff       (20)     4917 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/history.py
--rw-r--r--   0 jackson    (501) staff       (20)     5328 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/matrix.py
--rw-r--r--   0 jackson    (501) staff       (20)    10313 2023-03-25 16:54:14.000000 synadm-0.41.2/synadm/cli/media.py
--rw-r--r--   0 jackson    (501) staff       (20)     5832 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/notice.py
--rw-r--r--   0 jackson    (501) staff       (20)     5438 2023-03-25 16:54:14.000000 synadm-0.41.2/synadm/cli/regtok.py
--rw-r--r--   0 jackson    (501) staff       (20)    12704 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/room.py
--rw-r--r--   0 jackson    (501) staff       (20)    28397 2023-03-28 18:08:19.000000 synadm-0.41.2/synadm/cli/user.py
-drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-04-06 17:28:00.620609 synadm-0.41.2/synadm.egg-info/
--rw-r--r--   0 jackson    (501) staff       (20)    14558 2023-04-06 17:28:00.000000 synadm-0.41.2/synadm.egg-info/PKG-INFO
--rw-r--r--   0 jackson    (501) staff       (20)     1078 2023-04-06 17:28:00.000000 synadm-0.41.2/synadm.egg-info/SOURCES.txt
--rw-r--r--   0 jackson    (501) staff       (20)        1 2023-04-06 17:28:00.000000 synadm-0.41.2/synadm.egg-info/dependency_links.txt
--rw-r--r--   0 jackson    (501) staff       (20)       43 2023-04-06 17:28:00.000000 synadm-0.41.2/synadm.egg-info/entry_points.txt
--rw-r--r--   0 jackson    (501) staff       (20)       77 2023-04-06 17:28:00.000000 synadm-0.41.2/synadm.egg-info/requires.txt
--rw-r--r--   0 jackson    (501) staff       (20)        7 2023-04-06 17:28:00.000000 synadm-0.41.2/synadm.egg-info/top_level.txt
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.032816 synadm-0.41.3/
+-rw-r--r--   0 jackson    (501) staff       (20)      245 2023-06-14 07:06:46.000000 synadm-0.41.3/.bumpversion.cfg
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.023798 synadm-0.41.3/.github/
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.026595 synadm-0.41.3/.github/workflows/
+-rw-r--r--   0 jackson    (501) staff       (20)      435 2023-03-15 12:29:09.000000 synadm-0.41.3/.github/workflows/lint.yaml
+-rw-r--r--   0 jackson    (501) staff       (20)     2735 2023-06-14 06:57:31.000000 synadm-0.41.3/.github/workflows/release.yaml
+-rw-r--r--   0 jackson    (501) staff       (20)       96 2023-06-14 07:01:58.000000 synadm-0.41.3/.gitignore
+-rw-r--r--   0 jackson    (501) staff       (20)    35148 2023-02-24 10:57:22.000000 synadm-0.41.3/LICENSE
+-rw-r--r--   0 jackson    (501) staff       (20)      646 2023-02-24 10:57:22.000000 synadm-0.41.3/Makefile
+-rw-r--r--   0 jackson    (501) staff       (20)    14552 2023-06-14 07:10:20.032632 synadm-0.41.3/PKG-INFO
+-rw-r--r--   0 jackson    (501) staff       (20)    13498 2023-06-14 07:06:35.000000 synadm-0.41.3/README.md
+-rwxr-xr-x   0 jackson    (501) staff       (20)      814 2023-02-24 10:57:22.000000 synadm-0.41.3/bump.sh
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.023919 synadm-0.41.3/doc/
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.029098 synadm-0.41.3/doc/source/
+-rw-r--r--   0 jackson    (501) staff       (20)     2554 2023-06-14 07:06:46.000000 synadm-0.41.3/doc/source/conf.py
+-rw-r--r--   0 jackson    (501) staff       (20)      486 2023-03-25 16:54:14.000000 synadm-0.41.3/doc/source/index.rst
+-rw-r--r--   0 jackson    (501) staff       (20)      303 2023-03-15 12:29:09.000000 synadm-0.41.3/doc/source/index_cli_reference.rst
+-rw-r--r--   0 jackson    (501) staff       (20)      149 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/index_modules.rst
+-rw-r--r--   0 jackson    (501) staff       (20)      110 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.config.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       86 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.group.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       96 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.history.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       92 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.matrix.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       86 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.media.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       92 2023-03-15 12:29:09.000000 synadm-0.41.3/doc/source/synadm.cli.notice.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       92 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.regtok.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       81 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.room.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       88 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.root.rst
+-rw-r--r--   0 jackson    (501) staff       (20)       81 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.cli.user.rst
+-rw-r--r--   0 jackson    (501) staff       (20)      948 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.module.cli.rst
+-rw-r--r--   0 jackson    (501) staff       (20)      427 2023-02-24 10:57:22.000000 synadm-0.41.3/doc/source/synadm.module.rst
+-rwxr-xr-x   0 jackson    (501) staff       (20)      424 2023-06-14 07:06:35.000000 synadm-0.41.3/pypi.sh
+-rw-r--r--   0 jackson    (501) staff       (20)       67 2023-02-24 10:57:22.000000 synadm-0.41.3/requirements.txt
+-rwxr-xr-x   0 jackson    (501) staff       (20)      536 2023-02-24 10:57:22.000000 synadm-0.41.3/retag.sh
+-rw-r--r--   0 jackson    (501) staff       (20)       38 2023-06-14 07:10:20.032858 synadm-0.41.3/setup.cfg
+-rwxr-xr-x   0 jackson    (501) staff       (20)     2247 2023-06-14 07:06:46.000000 synadm-0.41.3/setup.py
+-rw-r--r--   0 jackson    (501) staff       (20)       60 2023-02-24 10:57:22.000000 synadm-0.41.3/sphinx_requirements.txt
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.029323 synadm-0.41.3/synadm/
+-rw-r--r--   0 jackson    (501) staff       (20)        0 2023-02-24 10:57:22.000000 synadm-0.41.3/synadm/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)    53261 2023-06-14 07:06:35.000000 synadm-0.41.3/synadm/api.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.032365 synadm-0.41.3/synadm/cli/
+-rw-r--r--   0 jackson    (501) staff       (20)    20407 2023-06-14 06:57:31.000000 synadm-0.41.3/synadm/cli/__init__.py
+-rw-r--r--   0 jackson    (501) staff       (20)     1458 2023-03-28 18:08:19.000000 synadm-0.41.3/synadm/cli/group.py
+-rw-r--r--   0 jackson    (501) staff       (20)     4917 2023-03-28 18:08:19.000000 synadm-0.41.3/synadm/cli/history.py
+-rw-r--r--   0 jackson    (501) staff       (20)     5328 2023-03-28 18:08:19.000000 synadm-0.41.3/synadm/cli/matrix.py
+-rw-r--r--   0 jackson    (501) staff       (20)    10313 2023-03-25 16:54:14.000000 synadm-0.41.3/synadm/cli/media.py
+-rw-r--r--   0 jackson    (501) staff       (20)     5832 2023-06-14 06:57:31.000000 synadm-0.41.3/synadm/cli/notice.py
+-rw-r--r--   0 jackson    (501) staff       (20)     5438 2023-03-25 16:54:14.000000 synadm-0.41.3/synadm/cli/regtok.py
+-rw-r--r--   0 jackson    (501) staff       (20)    12704 2023-03-28 18:08:19.000000 synadm-0.41.3/synadm/cli/room.py
+-rw-r--r--   0 jackson    (501) staff       (20)    28397 2023-06-14 06:57:31.000000 synadm-0.41.3/synadm/cli/user.py
+drwxr-xr-x   0 jackson    (501) staff       (20)        0 2023-06-14 07:10:20.030507 synadm-0.41.3/synadm.egg-info/
+-rw-r--r--   0 jackson    (501) staff       (20)    14552 2023-06-14 07:10:20.000000 synadm-0.41.3/synadm.egg-info/PKG-INFO
+-rw-r--r--   0 jackson    (501) staff       (20)     1078 2023-06-14 07:10:20.000000 synadm-0.41.3/synadm.egg-info/SOURCES.txt
+-rw-r--r--   0 jackson    (501) staff       (20)        1 2023-06-14 07:10:20.000000 synadm-0.41.3/synadm.egg-info/dependency_links.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       43 2023-06-14 07:10:20.000000 synadm-0.41.3/synadm.egg-info/entry_points.txt
+-rw-r--r--   0 jackson    (501) staff       (20)       77 2023-06-14 07:10:20.000000 synadm-0.41.3/synadm.egg-info/requires.txt
+-rw-r--r--   0 jackson    (501) staff       (20)        7 2023-06-14 07:10:20.000000 synadm-0.41.3/synadm.egg-info/top_level.txt
```

### Comparing `synadm-0.41.2/.github/workflows/release.yaml` & `synadm-0.41.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/LICENSE` & `synadm-0.41.3/LICENSE`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/Makefile` & `synadm-0.41.3/Makefile`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/PKG-INFO` & `synadm-0.41.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synadm
-Version: 0.41.2
+Version: 0.41.3
 Summary: Command line admin tool for Synapse (Matrix reference homeserver)
 Home-page: https://github.com/joj0/synadm
 Author: Johannes Tiefenbacher
 Author-email: jt@peek-a-boo.at
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/joj0/synadm/issues
 Project-URL: Documentation, https://github.com/joj0/synadm
@@ -229,17 +229,17 @@
 
 ```
 cd synadm
 git pull
 pip install .
 ```
 
-*Note: If you installed to a Python venv, first load it as described in [install to virtual environment](#install-to-virtual-environment).*
+*Note: If you installed it to a Python venv, [activate it](CONTRIBUTING.md#3-set-up-a-python3-virtual-environment).*
 
-*Note: If you installed in [development mode](#install-in-development-mode) you can spare the `pip install .` command - just `git pull` and you're done.*
+*Note: If you installed it in [editable mode](CONTRIBUTING.md#4-install-in-editable-mode) (or for development), you can spare the `pip install .` command - just `git pull` and you're done.*
 
 
 
 ## Implementation Status / Commands List
 
 [Follow this link to the official Synapse Admin API docs](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
 
@@ -273,22 +273,21 @@
   * [x] `room delete <room id>`
   * [x] `room make-admin <room id> <user id>`
   * [x] `room state <room id>`
   * [ ] Additional commands and aliases around room management
     * [x] `room search <search-term>` (alias of `room list -n <search-term>`)
     * [x] `room resolve <room alias>`
     * [x] `room power-levels`
-    * [ ] `room count`
-    * [ ] `room top-complexity`
-    * [ ] `room top-members`
     * [x] `room block`
     * [x] `room block-status`
 * [x] [Server Notices](https://matrix-org.github.io/synapse/develop/admin_api/server_notices.html)
 * [x] ~~[Shutdown Room](https://matrix-org.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
 * [ ] [Statistics](https://matrix-org.github.io/synapse/develop/admin_api/statistics.html)
+  * [ ] `synadm media user-stats`
+  * [ ] `synadm room largest`
 * [x] [Users](https://matrix-org.github.io/synapse/develop/admin_api/user_admin_api.html)
   * [x] `user details <user id>`
   * [x] `user modify <user id>` (also used for user creation)
   * [x] `user list`
   * [x] `user deactivate <user id>` (including GDPR erase)
   * [x] `user password <user id>`
   * [x] `user membership <user id>`
@@ -309,15 +308,15 @@
   * [x] `regtok update <registration token>`
   * [x] `regtok delete <registration token>`
 
 
 
 ## Get in Touch
 
-If you need avice on using synadm, have a feature idea or would like to discuss anything else around `synadm`, get in touch via Matrix!
+If you need advice on using synadm, have a feature idea or would like to discuss anything else around `synadm`, get in touch via Matrix!
 
 We are hanging around in the official support room for Synapse, [#synapse:matrix.org](https://matrix.to/#/#synapse:matrix.org). Usually you'll find `synadm` users there that might answer your questions already. If not, mentioning `synadm` will ping us with the help of Element's keyword notify feature and we'll try to get in touch.
 
 The most direct way to reach synadm maintainers as well as seasoned users and Synapse admins is by joining [#synadm:peek-a-boo.at](https://matrix.to/#/#synadm:peek-a-boo.at).
 
 If you are sure you've found a bug that was not already reported, certainly directly opening an [issue on GitHub](https://github.com/JOJ0/synadm/issues) is a valid option too. If unsure, ask in [#synadm:peek-a-boo.at](https://matrix.to/#/#synadm:peek-a-boo.at) first.
```

### Comparing `synadm-0.41.2/README.md` & `synadm-0.41.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -204,17 +204,17 @@
 
 ```
 cd synadm
 git pull
 pip install .
 ```
 
-*Note: If you installed to a Python venv, first load it as described in [install to virtual environment](#install-to-virtual-environment).*
+*Note: If you installed it to a Python venv, [activate it](CONTRIBUTING.md#3-set-up-a-python3-virtual-environment).*
 
-*Note: If you installed in [development mode](#install-in-development-mode) you can spare the `pip install .` command - just `git pull` and you're done.*
+*Note: If you installed it in [editable mode](CONTRIBUTING.md#4-install-in-editable-mode) (or for development), you can spare the `pip install .` command - just `git pull` and you're done.*
 
 
 
 ## Implementation Status / Commands List
 
 [Follow this link to the official Synapse Admin API docs](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
 
@@ -248,22 +248,21 @@
   * [x] `room delete <room id>`
   * [x] `room make-admin <room id> <user id>`
   * [x] `room state <room id>`
   * [ ] Additional commands and aliases around room management
     * [x] `room search <search-term>` (alias of `room list -n <search-term>`)
     * [x] `room resolve <room alias>`
     * [x] `room power-levels`
-    * [ ] `room count`
-    * [ ] `room top-complexity`
-    * [ ] `room top-members`
     * [x] `room block`
     * [x] `room block-status`
 * [x] [Server Notices](https://matrix-org.github.io/synapse/develop/admin_api/server_notices.html)
 * [x] ~~[Shutdown Room](https://matrix-org.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
 * [ ] [Statistics](https://matrix-org.github.io/synapse/develop/admin_api/statistics.html)
+  * [ ] `synadm media user-stats`
+  * [ ] `synadm room largest`
 * [x] [Users](https://matrix-org.github.io/synapse/develop/admin_api/user_admin_api.html)
   * [x] `user details <user id>`
   * [x] `user modify <user id>` (also used for user creation)
   * [x] `user list`
   * [x] `user deactivate <user id>` (including GDPR erase)
   * [x] `user password <user id>`
   * [x] `user membership <user id>`
@@ -284,15 +283,15 @@
   * [x] `regtok update <registration token>`
   * [x] `regtok delete <registration token>`
 
 
 
 ## Get in Touch
 
-If you need avice on using synadm, have a feature idea or would like to discuss anything else around `synadm`, get in touch via Matrix!
+If you need advice on using synadm, have a feature idea or would like to discuss anything else around `synadm`, get in touch via Matrix!
 
 We are hanging around in the official support room for Synapse, [#synapse:matrix.org](https://matrix.to/#/#synapse:matrix.org). Usually you'll find `synadm` users there that might answer your questions already. If not, mentioning `synadm` will ping us with the help of Element's keyword notify feature and we'll try to get in touch.
 
 The most direct way to reach synadm maintainers as well as seasoned users and Synapse admins is by joining [#synadm:peek-a-boo.at](https://matrix.to/#/#synadm:peek-a-boo.at).
 
 If you are sure you've found a bug that was not already reported, certainly directly opening an [issue on GitHub](https://github.com/JOJ0/synadm/issues) is a valid option too. If unsure, ask in [#synadm:peek-a-boo.at](https://matrix.to/#/#synadm:peek-a-boo.at) first.
```

### Comparing `synadm-0.41.2/bump.sh` & `synadm-0.41.3/bump.sh`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/doc/source/conf.py` & `synadm-0.41.3/doc/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 # -- Project information -----------------------------------------------------
 
 project = 'synadm'
 copyright = '2020-2023, Johannes Tiefenbacher'
 author = 'Johannes Tiefenbacher'
 
 # The short X.Y version
-version = '0.41.2'
+version = '0.41.3'
 
 # The full version, including alpha/beta/rc tags
-release = '0.41.2'
+release = '0.41.3'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `synadm-0.41.2/doc/source/synadm.module.cli.rst` & `synadm-0.41.3/doc/source/synadm.module.cli.rst`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/retag.sh` & `synadm-0.41.3/retag.sh`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/setup.py` & `synadm-0.41.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from setuptools import setup, find_packages
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="synadm",
-    version="0.41.2",
+    version="0.41.3",
     author="Johannes Tiefenbacher",
     author_email="jt@peek-a-boo.at",
     description="Command line admin tool for Synapse (Matrix reference homeserver)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joj0/synadm",
     project_urls={
```

### Comparing `synadm-0.41.2/synadm/api.py` & `synadm-0.41.3/synadm/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1144,16 +1144,16 @@
                 timestamp.
 
         Returns:
             string: JSON string containing the admin API's response or None if
                 an exception occured. See Synapse admin API docs for details.
 
         """
-        result = self.query("get", "v1/registration_tokens/{token}",
-                            token=token)
+        result = self.query("get", "v1/registration_tokens/{t}",
+                            t=token)
 
         # Change expiry_time to a human readable format if requested
         if (
             readable_expiry
             and result is not None
             and result.get("expiry_time") is not None
         ):
@@ -1240,30 +1240,33 @@
                 data["expiry_time"] = None
             else:
                 data["expiry_time"] = expiry_ts
         elif expire_at:
             self.log.debug(f"Received --expire-at: {expire_at}")
             data["expiry_time"] = self._timestamp_from_datetime(expire_at)
 
-        return self.query("put", "v1/registration_tokens/{token}", data=data,
-                          token=token)
+        return self.query("put", "v1/registration_tokens/{t}", data=data,
+                          t=token)
 
     def regtok_delete(self, token):
         """ Delete a registration token
 
         Args:
             token (string): The registration token to delete
 
         Returns:
             string: JSON string containing the admin API's response or None if
                 an exception occured. See Synapse admin API docs for details.
 
         """
-        return self.query("delete", "v1/registration_tokens/{token}",
-                          token=token)
+        # t because query also accepts token when we want it for the
+        # request
+        # https://github.com/JOJ0/synadm/issues/110#issuecomment-1590032158
+        return self.query("delete", "v1/registration_tokens/{t}",
+                          t=token)
 
     def user_shadow_ban(self, user_id, unban):
         """ Shadow-ban or unban a user.
 
         Args:
             user_id (string): The user to be banned/unbanned.
             unban (boolean): Unban the specified user.
```

### Comparing `synadm-0.41.2/synadm/cli/__init__.py` & `synadm-0.41.3/synadm/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/group.py` & `synadm-0.41.3/synadm/cli/group.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/history.py` & `synadm-0.41.3/synadm/cli/history.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/matrix.py` & `synadm-0.41.3/synadm/cli/matrix.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/media.py` & `synadm-0.41.3/synadm/cli/media.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/notice.py` & `synadm-0.41.3/synadm/cli/notice.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/regtok.py` & `synadm-0.41.3/synadm/cli/regtok.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/room.py` & `synadm-0.41.3/synadm/cli/room.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm/cli/user.py` & `synadm-0.41.3/synadm/cli/user.py`

 * *Files identical despite different names*

### Comparing `synadm-0.41.2/synadm.egg-info/PKG-INFO` & `synadm-0.41.3/synadm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synadm
-Version: 0.41.2
+Version: 0.41.3
 Summary: Command line admin tool for Synapse (Matrix reference homeserver)
 Home-page: https://github.com/joj0/synadm
 Author: Johannes Tiefenbacher
 Author-email: jt@peek-a-boo.at
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/joj0/synadm/issues
 Project-URL: Documentation, https://github.com/joj0/synadm
@@ -229,17 +229,17 @@
 
 ```
 cd synadm
 git pull
 pip install .
 ```
 
-*Note: If you installed to a Python venv, first load it as described in [install to virtual environment](#install-to-virtual-environment).*
+*Note: If you installed it to a Python venv, [activate it](CONTRIBUTING.md#3-set-up-a-python3-virtual-environment).*
 
-*Note: If you installed in [development mode](#install-in-development-mode) you can spare the `pip install .` command - just `git pull` and you're done.*
+*Note: If you installed it in [editable mode](CONTRIBUTING.md#4-install-in-editable-mode) (or for development), you can spare the `pip install .` command - just `git pull` and you're done.*
 
 
 
 ## Implementation Status / Commands List
 
 [Follow this link to the official Synapse Admin API docs](https://matrix-org.github.io/synapse/develop/usage/administration/admin_api/index.html) - direct links to the specific API documentation pages are provided in the list below.
 
@@ -273,22 +273,21 @@
   * [x] `room delete <room id>`
   * [x] `room make-admin <room id> <user id>`
   * [x] `room state <room id>`
   * [ ] Additional commands and aliases around room management
     * [x] `room search <search-term>` (alias of `room list -n <search-term>`)
     * [x] `room resolve <room alias>`
     * [x] `room power-levels`
-    * [ ] `room count`
-    * [ ] `room top-complexity`
-    * [ ] `room top-members`
     * [x] `room block`
     * [x] `room block-status`
 * [x] [Server Notices](https://matrix-org.github.io/synapse/develop/admin_api/server_notices.html)
 * [x] ~~[Shutdown Room](https://matrix-org.github.io/synapse/develop/admin_api/shutdown_room.html)~~ (DEPRECATED, covered by `room delete`)
 * [ ] [Statistics](https://matrix-org.github.io/synapse/develop/admin_api/statistics.html)
+  * [ ] `synadm media user-stats`
+  * [ ] `synadm room largest`
 * [x] [Users](https://matrix-org.github.io/synapse/develop/admin_api/user_admin_api.html)
   * [x] `user details <user id>`
   * [x] `user modify <user id>` (also used for user creation)
   * [x] `user list`
   * [x] `user deactivate <user id>` (including GDPR erase)
   * [x] `user password <user id>`
   * [x] `user membership <user id>`
@@ -309,15 +308,15 @@
   * [x] `regtok update <registration token>`
   * [x] `regtok delete <registration token>`
 
 
 
 ## Get in Touch
 
-If you need avice on using synadm, have a feature idea or would like to discuss anything else around `synadm`, get in touch via Matrix!
+If you need advice on using synadm, have a feature idea or would like to discuss anything else around `synadm`, get in touch via Matrix!
 
 We are hanging around in the official support room for Synapse, [#synapse:matrix.org](https://matrix.to/#/#synapse:matrix.org). Usually you'll find `synadm` users there that might answer your questions already. If not, mentioning `synadm` will ping us with the help of Element's keyword notify feature and we'll try to get in touch.
 
 The most direct way to reach synadm maintainers as well as seasoned users and Synapse admins is by joining [#synadm:peek-a-boo.at](https://matrix.to/#/#synadm:peek-a-boo.at).
 
 If you are sure you've found a bug that was not already reported, certainly directly opening an [issue on GitHub](https://github.com/JOJ0/synadm/issues) is a valid option too. If unsure, ask in [#synadm:peek-a-boo.at](https://matrix.to/#/#synadm:peek-a-boo.at) first.
```

### Comparing `synadm-0.41.2/synadm.egg-info/SOURCES.txt` & `synadm-0.41.3/synadm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

