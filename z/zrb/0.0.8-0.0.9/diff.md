# Comparing `tmp/zrb-0.0.8.tar.gz` & `tmp/zrb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb-0.0.8.tar", last modified: Thu Feb  2 08:33:48 2023, max compression
+gzip compressed data, was "zrb-0.0.9.tar", last modified: Fri Feb  3 02:37:15 2023, max compression
```

## Comparing `zrb-0.0.8.tar` & `zrb-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,64 @@
--rw-r--r--   0        0        0       64 2023-02-01 14:04:37.579018 zrb-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2023-01-25 23:16:29.196224 zrb-0.0.8/LICENSE
--rw-r--r--   0        0        0     6223 2023-02-02 00:33:19.375037 zrb-0.0.8/README.md
--rw-r--r--   0        0        0       23 2023-01-26 00:56:17.990155 zrb-0.0.8/playground-template/requirements.txt
--rw-r--r--   0        0        0     1985 2023-02-01 00:54:45.551737 zrb-0.0.8/playground-template/zrb_init.py
--rw-r--r--   0        0        0      885 2023-02-02 08:31:56.853621 zrb-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      456 2023-02-01 14:06:02.425736 zrb-0.0.8/requirements.txt
--rw-r--r--   0        0        0      361 2023-02-02 00:15:49.253344 zrb-0.0.8/src/zrb/__init__.py
--rw-r--r--   0        0        0      308 2023-01-29 07:05:35.143713 zrb-0.0.8/src/zrb/__main__.py
--rw-r--r--   0        0        0        0 2023-01-26 13:13:07.014863 zrb-0.0.8/src/zrb/action/__init__.py
--rw-r--r--   0        0        0      271 2023-01-31 22:50:45.065675 zrb-0.0.8/src/zrb/action/base_action.py
--rw-r--r--   0        0        0     3073 2023-02-01 12:38:32.548047 zrb-0.0.8/src/zrb/action/runner.py
--rw-r--r--   0        0        0        0 2023-01-25 23:08:05.399961 zrb-0.0.8/src/zrb/config.toml
--rw-r--r--   0        0        0        0 2023-01-28 15:51:34.079390 zrb-0.0.8/src/zrb/config/__init__.py
--rw-r--r--   0        0        0      723 2023-02-01 01:07:49.107707 zrb-0.0.8/src/zrb/config/config.py
--rw-r--r--   0        0        0        0 2023-02-01 00:57:08.130185 zrb-0.0.8/src/zrb/default/__init__.py
--rw-r--r--   0        0        0      143 2023-02-01 12:27:30.727064 zrb-0.0.8/src/zrb/default/_register.py
--rw-r--r--   0        0        0        0 2023-02-01 12:23:14.002683 zrb-0.0.8/src/zrb/default/show/__init__.py
--rw-r--r--   0        0        0       71 2023-02-01 12:23:07.211120 zrb-0.0.8/src/zrb/default/show/_group.py
--rw-r--r--   0        0        0      165 2023-02-01 12:25:08.076005 zrb-0.0.8/src/zrb/default/show/_register.py
--rw-r--r--   0        0        0      419 2023-02-01 12:22:39.670923 zrb-0.0.8/src/zrb/default/show/solid_principle.py
--rw-r--r--   0        0        0        0 2023-01-26 17:05:38.257459 zrb-0.0.8/src/zrb/helper/__init__.py
--rw-r--r--   0        0        0        0 2023-01-29 07:18:18.811612 zrb-0.0.8/src/zrb/helper/accessories/__init__.py
--rw-r--r--   0        0        0      605 2023-02-01 13:09:57.333054 zrb-0.0.8/src/zrb/helper/accessories/color.py
--rw-r--r--   0        0        0      289 2023-01-29 07:22:31.556891 zrb-0.0.8/src/zrb/helper/accessories/icon.py
--rw-r--r--   0        0        0      734 2023-01-29 07:23:03.100524 zrb-0.0.8/src/zrb/helper/accessories/name.py
--rw-r--r--   0        0        0        0 2023-01-29 07:04:25.375901 zrb-0.0.8/src/zrb/helper/cli/__init__.py
--rw-r--r--   0        0        0      763 2023-02-01 13:05:10.904709 zrb-0.0.8/src/zrb/helper/cli/create_cli.py
--rw-r--r--   0        0        0        0 2023-02-02 00:07:34.128110 zrb-0.0.8/src/zrb/helper/file/__init__.py
--rw-r--r--   0        0        0     1072 2023-02-02 00:14:53.350008 zrb-0.0.8/src/zrb/helper/file/copy_tree.py
--rw-r--r--   0        0        0        0 2023-01-29 09:51:03.021386 zrb-0.0.8/src/zrb/helper/keyval/__init__.py
--rw-r--r--   0        0        0      292 2023-01-29 12:03:56.752556 zrb-0.0.8/src/zrb/helper/keyval/get_object_from_keyval.py
--rw-r--r--   0        0        0        0 2023-01-30 00:00:14.499191 zrb-0.0.8/src/zrb/helper/list/__init__.py
--rw-r--r--   0        0        0      225 2023-01-30 00:34:10.735498 zrb-0.0.8/src/zrb/helper/list/append_unique.py
--rw-r--r--   0        0        0        0 2023-01-29 07:10:48.042678 zrb-0.0.8/src/zrb/helper/loader/__init__.py
--rw-r--r--   0        0        0      515 2023-01-28 09:35:10.871488 zrb-0.0.8/src/zrb/helper/loader/load_module.py
--rw-r--r--   0        0        0        0 2023-01-30 11:33:05.031065 zrb-0.0.8/src/zrb/helper/string/__init__.py
--rw-r--r--   0        0        0      106 2023-02-02 00:14:42.379983 zrb-0.0.8/src/zrb/helper/string/get_cmd_name.py
--rw-r--r--   0        0        0      222 2023-02-02 00:14:36.549973 zrb-0.0.8/src/zrb/helper/string/parse_replacement.py
--rw-r--r--   0        0        0      112 2023-01-30 12:25:25.659518 zrb-0.0.8/src/zrb/runner.py
--rw-r--r--   0        0        0        0 2023-01-28 08:13:04.531303 zrb-0.0.8/src/zrb/task/__init__.py
--rw-r--r--   0        0        0     8238 2023-02-02 00:14:02.737901 zrb-0.0.8/src/zrb/task/base_model.py
--rw-r--r--   0        0        0     6944 2023-02-01 15:55:45.180982 zrb-0.0.8/src/zrb/task/base_task.py
--rw-r--r--   0        0        0     4451 2023-02-01 15:47:20.176364 zrb-0.0.8/src/zrb/task/cmd_task.py
--rw-r--r--   0        0        0     1535 2023-02-02 00:13:25.496656 zrb-0.0.8/src/zrb/task/code_maker.py
--rw-r--r--   0        0        0     3016 2023-02-01 16:17:30.245187 zrb-0.0.8/src/zrb/task/http_checker.py
--rw-r--r--   0        0        0     2105 2023-02-01 16:17:33.675209 zrb-0.0.8/src/zrb/task/port_checker.py
--rw-r--r--   0        0        0      419 2023-01-31 22:25:28.779442 zrb-0.0.8/src/zrb/task/task.py
--rw-r--r--   0        0        0     1252 2023-02-02 08:33:15.807732 zrb-0.0.8/src/zrb/task_env/env.py
--rw-r--r--   0        0        0        0 2023-01-30 12:22:20.499082 zrb-0.0.8/src/zrb/task_group/__init__.py
--rw-r--r--   0        0        0      976 2023-02-02 00:14:02.737901 zrb-0.0.8/src/zrb/task_group/group.py
--rw-r--r--   0        0        0        0 2023-01-26 13:46:53.388645 zrb-0.0.8/src/zrb/task_input/__init__.py
--rw-r--r--   0        0        0     2635 2023-02-01 00:50:56.349866 zrb-0.0.8/src/zrb/task_input/base_input.py
--rw-r--r--   0        0        0     1593 2023-02-01 00:45:48.330541 zrb-0.0.8/src/zrb/task_input/str_input.py
--rw-r--r--   0        0        0        0 2023-01-26 00:53:09.508720 zrb-0.0.8/tests/.gitignore
--rw-r--r--   0        0        0       10 2023-02-01 15:18:58.069173 zrb-0.0.8/tests/task/sample_cmd/hello.sh
--rw-r--r--   0        0        0     3832 2023-02-02 00:25:50.722135 zrb-0.0.8/tests/task/test_cmd_task.py
--rwxr-xr-x   0        0        0     2729 2023-02-02 00:23:14.924872 zrb-0.0.8/toolkit.sh
--rw-r--r--   0        0        0     6837 1970-01-01 00:00:00.000000 zrb-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-02-03 00:50:39.432627 zrb-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2023-01-25 23:16:29.196224 zrb-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6721 2023-02-03 02:33:59.127475 zrb-0.0.9/README.md
+-rw-r--r--   0        0        0       23 2023-01-26 00:56:17.990155 zrb-0.0.9/playground-template/requirements.txt
+-rw-r--r--   0        0        0     2361 2023-02-03 02:08:04.414417 zrb-0.0.9/playground-template/zrb_init.py
+-rw-r--r--   0        0        0      885 2023-02-03 02:36:44.190380 zrb-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      456 2023-02-01 14:06:02.425736 zrb-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      361 2023-02-02 00:15:49.253344 zrb-0.0.9/src/zrb/__init__.py
+-rw-r--r--   0        0        0      308 2023-01-29 07:05:35.143713 zrb-0.0.9/src/zrb/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-26 13:13:07.014863 zrb-0.0.9/src/zrb/action/__init__.py
+-rw-r--r--   0        0        0      271 2023-01-31 22:50:45.065675 zrb-0.0.9/src/zrb/action/base_action.py
+-rw-r--r--   0        0        0     3188 2023-02-03 01:52:09.242861 zrb-0.0.9/src/zrb/action/runner.py
+-rw-r--r--   0        0        0        0 2023-01-25 23:08:05.399961 zrb-0.0.9/src/zrb/config.toml
+-rw-r--r--   0        0        0        0 2023-01-28 15:51:34.079390 zrb-0.0.9/src/zrb/config/__init__.py
+-rw-r--r--   0        0        0      723 2023-02-01 01:07:49.107707 zrb-0.0.9/src/zrb/config/config.py
+-rw-r--r--   0        0        0        0 2023-02-01 00:57:08.130185 zrb-0.0.9/src/zrb/default/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-01 12:27:30.727064 zrb-0.0.9/src/zrb/default/_register.py
+-rw-r--r--   0        0        0        0 2023-02-01 12:23:14.002683 zrb-0.0.9/src/zrb/default/show/__init__.py
+-rw-r--r--   0        0        0       71 2023-02-01 12:23:07.211120 zrb-0.0.9/src/zrb/default/show/_group.py
+-rw-r--r--   0        0        0      165 2023-02-01 12:25:08.076005 zrb-0.0.9/src/zrb/default/show/_register.py
+-rw-r--r--   0        0        0      419 2023-02-01 12:22:39.670923 zrb-0.0.9/src/zrb/default/show/solid_principle.py
+-rw-r--r--   0        0        0        0 2023-01-26 17:05:38.257459 zrb-0.0.9/src/zrb/helper/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-29 07:18:18.811612 zrb-0.0.9/src/zrb/helper/accessories/__init__.py
+-rw-r--r--   0        0        0      605 2023-02-01 13:09:57.333054 zrb-0.0.9/src/zrb/helper/accessories/color.py
+-rw-r--r--   0        0        0      289 2023-01-29 07:22:31.556891 zrb-0.0.9/src/zrb/helper/accessories/icon.py
+-rw-r--r--   0        0        0      734 2023-01-29 07:23:03.100524 zrb-0.0.9/src/zrb/helper/accessories/name.py
+-rw-r--r--   0        0        0        0 2023-01-29 07:04:25.375901 zrb-0.0.9/src/zrb/helper/cli/__init__.py
+-rw-r--r--   0        0        0      854 2023-02-02 13:26:09.841649 zrb-0.0.9/src/zrb/helper/cli/create_cli.py
+-rw-r--r--   0        0        0        0 2023-02-02 00:07:34.128110 zrb-0.0.9/src/zrb/helper/file/__init__.py
+-rw-r--r--   0        0        0     1072 2023-02-02 00:14:53.350008 zrb-0.0.9/src/zrb/helper/file/copy_tree.py
+-rw-r--r--   0        0        0        0 2023-01-29 09:51:03.021386 zrb-0.0.9/src/zrb/helper/keyval/__init__.py
+-rw-r--r--   0        0        0      292 2023-01-29 12:03:56.752556 zrb-0.0.9/src/zrb/helper/keyval/get_object_from_keyval.py
+-rw-r--r--   0        0        0        0 2023-01-30 00:00:14.499191 zrb-0.0.9/src/zrb/helper/list/__init__.py
+-rw-r--r--   0        0        0      225 2023-01-30 00:34:10.735498 zrb-0.0.9/src/zrb/helper/list/append_unique.py
+-rw-r--r--   0        0        0        0 2023-01-29 07:10:48.042678 zrb-0.0.9/src/zrb/helper/loader/__init__.py
+-rw-r--r--   0        0        0      515 2023-01-28 09:35:10.871488 zrb-0.0.9/src/zrb/helper/loader/load_module.py
+-rw-r--r--   0        0        0        0 2023-01-30 11:33:05.031065 zrb-0.0.9/src/zrb/helper/string/__init__.py
+-rw-r--r--   0        0        0      106 2023-02-02 00:14:42.379983 zrb-0.0.9/src/zrb/helper/string/get_cmd_name.py
+-rw-r--r--   0        0        0      222 2023-02-02 00:14:36.549973 zrb-0.0.9/src/zrb/helper/string/parse_replacement.py
+-rw-r--r--   0        0        0      112 2023-01-30 12:25:25.659518 zrb-0.0.9/src/zrb/runner.py
+-rw-r--r--   0        0        0        0 2023-01-28 08:13:04.531303 zrb-0.0.9/src/zrb/task/__init__.py
+-rw-r--r--   0        0        0     9311 2023-02-03 00:58:03.044328 zrb-0.0.9/src/zrb/task/base_model.py
+-rw-r--r--   0        0        0     8044 2023-02-03 02:31:11.013437 zrb-0.0.9/src/zrb/task/base_task.py
+-rw-r--r--   0        0        0     5817 2023-02-03 01:55:32.572250 zrb-0.0.9/src/zrb/task/cmd_task.py
+-rw-r--r--   0        0        0     1889 2023-02-03 01:55:32.572250 zrb-0.0.9/src/zrb/task/code_maker.py
+-rw-r--r--   0        0        0     3204 2023-02-03 02:31:27.533455 zrb-0.0.9/src/zrb/task/http_checker.py
+-rw-r--r--   0        0        0     2293 2023-02-03 01:55:32.572250 zrb-0.0.9/src/zrb/task/port_checker.py
+-rw-r--r--   0        0        0      178 2023-02-03 01:29:30.760810 zrb-0.0.9/src/zrb/task/task.py
+-rw-r--r--   0        0        0     1256 2023-02-02 13:25:22.958598 zrb-0.0.9/src/zrb/task_env/env.py
+-rw-r--r--   0        0        0        0 2023-01-30 12:22:20.499082 zrb-0.0.9/src/zrb/task_group/__init__.py
+-rw-r--r--   0        0        0      976 2023-02-02 00:14:02.737901 zrb-0.0.9/src/zrb/task_group/group.py
+-rw-r--r--   0        0        0        0 2023-01-26 13:46:53.388645 zrb-0.0.9/src/zrb/task_input/__init__.py
+-rw-r--r--   0        0        0     2635 2023-02-01 00:50:56.349866 zrb-0.0.9/src/zrb/task_input/base_input.py
+-rw-r--r--   0        0        0     1593 2023-02-01 00:45:48.330541 zrb-0.0.9/src/zrb/task_input/str_input.py
+-rw-r--r--   0        0        0        0 2023-01-26 00:53:09.508720 zrb-0.0.9/tests/.gitignore
+-rw-r--r--   0        0        0       72 2023-02-03 00:06:05.061598 zrb-0.0.9/tests/task/cmd_task/templates/hello.sh
+-rw-r--r--   0        0        0       62 2023-02-03 00:05:58.761569 zrb-0.0.9/tests/task/cmd_task/templates/macros.jinja
+-rw-r--r--   0        0        0     3704 2023-02-03 00:41:42.217733 zrb-0.0.9/tests/task/cmd_task/test_cmd_task.py
+-rw-r--r--   0        0        0       21 2023-02-03 00:51:35.527191 zrb-0.0.9/tests/task/code_maker/template/excluded
+-rw-r--r--   0        0        0      111 2023-02-03 00:53:04.081119 zrb-0.0.9/tests/task/code_maker/template/src/app_name.py
+-rw-r--r--   0        0        0       12 2023-02-03 00:53:09.531127 zrb-0.0.9/tests/task/code_maker/template/src/config_app_name.py
+-rw-r--r--   0        0        0     1568 2023-02-03 01:10:58.177183 zrb-0.0.9/tests/task/code_maker/test_code_maker.py
+-rwxr-xr-x   0        0        0     2729 2023-02-02 00:23:14.924872 zrb-0.0.9/toolkit.sh
+-rw-r--r--   0        0        0     7335 1970-01-01 00:00:00.000000 zrb-0.0.9/PKG-INFO
```

### Comparing `zrb-0.0.8/LICENSE` & `zrb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/README.md` & `zrb-0.0.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -28,43 +28,61 @@
 ```bash
 ZRB_SCRIPTS=~/personal/zrb_init.py:~/work/zrb_init.py
 ```
 
 Your Zrb script (e.g: `./zrb_init.py`) should contain your task definitions. For example:
 
 ```python
+from typing import Any
 from zrb import (
-    runner, Env, StrInput, Group, CmdTask, HTTPChecker
+    runner, Env, StrInput, Group, Task, CmdTask, HTTPChecker
 )
 
 '''
-Simple task, read input and show output
+Simple Python task, concatenate words
+'''
+concat = Task(
+    name='concat',
+    inputs=[StrInput(name='separator', description='Separator', default=' ')],
+)
+runner.register(concat)
+
+
+# set concat's runner
+@concat.runner
+def run(*args: str, **kwargs: Any) -> str:
+    separator = kwargs.get('separator', ' ')
+    return separator.join(args)
+
+
+'''
+Simple CLI task, read input and show output
 '''
 hello = CmdTask(
     name='hello',
     inputs=[StrInput(name='name', description='Name', default='world')],
     cmd='echo Hello {{input.name}}'
 )
 runner.register(hello)
 
 make = Group(name='make', description='Make things')
 
 '''
-Simple task, part of 'make' group
+Simple CLI task, part of 'make' group
 '''
 make_coffee = CmdTask(
     name='coffee',
     group=make,
     upstreams=[hello],
     cmd='echo Coffee for you ☕'
 )
 runner.register(make_coffee)
 
 '''
-Simple task, part of 'make' group
+Simple CLI task, part of 'make' group
 '''
 make_beer = CmdTask(
     name='beer',
     group=make,
     upstreams=[hello],
     cmd='echo Cheers 🍺'
 )
@@ -74,30 +92,30 @@
 Sub group of 'make'
 '''
 make_gitignore = Group(
     name='gitignore', description='Make gitignore', parent=make
 )
 
 '''
-Simple task, part of 'make_gitignore' group.
+Simple CLI task, part of 'make_gitignore' group.
 Having multiline cmd
 '''
 make_gitignore_python = CmdTask(
     name='node',
     group=make_gitignore,
     cmd=[
         'echo "node_modules/" >> .gitignore'
         'echo ".npm" >> .gitignore'
         'echo "npm-debug.log" >> .gitignore'
     ]
 )
 runner.register(make_gitignore_python)
 
 '''
-Simple task, part of 'make_gitignore' group.
+Simple CLI task, part of 'make_gitignore' group.
 Having multiline cmd
 '''
 make_gitignore_nodejs = CmdTask(
     name='node',
     group=make_gitignore,
     cmd=[
         'echo "__pycache__/" >> .gitignore'
@@ -107,31 +125,32 @@
 runner.register(make_gitignore_nodejs)
 
 server = Group(
     name='server', description='Server related commands'
 )
 
 '''
-Long running task.
+Long running CLI task.
 Run a server and waiting for the port to be ready.
 '''
 run_server = CmdTask(
     name='run',
     group=server,
     upstreams=[make_coffee, make_beer],
     inputs=[StrInput(name='dir', description='Directory', default='.')],
     envs=[Env(name='PORT', os_name='WEB_PORT', default='3000')],
     cmd='python -m http.server $PORT --directory {{input.dir}}',
     checkers=[HTTPChecker(port='{{env.PORT}}')]
 )
 runner.register(run_server)
-
 ```
 
-Once registered, your task will be accessible from the terminal:
+Once registered, your task will be accessible from the terminal.
+
+For example, you can run a server by performing:
 
 ```bash
 export WEB_PORT=8080
 zrb server run
 ```
 
 The output will be similar to this:
@@ -163,15 +182,16 @@
 
 
 cmd_task = CmdTask(
     name='sample',
     cmd='echo hello'
 )
 main_loop = cmd_task.create_main_loop(env_prefix='')
-main_loop() # This run the task
+result = main_loop() # This run the task
+print(result.output) # Should be "hello"
 ```
 
 
 # Configuration
 
 The following configurations are available:
```

### Comparing `zrb-0.0.8/pyproject.toml` & `zrb-0.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "zrb"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Go Frendi Gunawan", email="gofrendiasgard@gmail.com" },
 ]
 description = "Your faithful companion"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zrb-0.0.8/src/zrb/action/runner.py` & `zrb-0.0.9/src/zrb/action/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 from typing import List, Mapping, Union
 from ..action.base_action import BaseAction
 from ..task.base_task import BaseTask
 from ..task_group.group import Group as TaskGroup
-from click import Group as CliGroup, Command as CliCommand, Option as CliOption
+import click
 
-CliSubcommand = Union[CliGroup, CliCommand]
+CliSubcommand = Union[click.Group, click.Command]
 
 
 class Runner(BaseAction):
     '''
     Runner class.
     Any tasks registered to the runner will be accessible from the terminal
     '''
 
     def __init__(self, env_prefix: str = ''):
         BaseAction.__init__(self)
         self.env_prefix = env_prefix
-        self._registered_groups: Mapping[str, CliGroup] = {}
+        self._registered_groups: Mapping[str, click.Group] = {}
         self._top_levels: List[CliSubcommand] = []
-        self._subcommands: Mapping[str, List[CliGroup]] = {}
+        self._subcommands: Mapping[str, List[click.Group]] = {}
 
-    def serve(self, cli: CliGroup) -> CliGroup:
+    def serve(self, cli: click.Group) -> click.Group:
         for task in self._tasks:
             subcommand = self._create_cli_subcommand(task)
             if subcommand not in self._top_levels:
                 self._top_levels.append(subcommand)
                 cli.add_command(subcommand)
         return cli
 
-    def _create_cli_subcommand(self, task: BaseTask) -> CliGroup:
+    def _create_cli_subcommand(self, task: BaseTask) -> click.Group:
         subcommand: CliSubcommand = self._create_cli_command(task)
         task_group = task.group
         while task_group is not None:
             group = self._register_sub_command(task_group, subcommand)
             if task_group.parent is None:
                 return group
             subcommand = group
             task_group = task_group.parent
         return subcommand
 
     def _register_sub_command(
         self, task_group: TaskGroup, subcommand: CliSubcommand
-    ) -> CliGroup:
+    ) -> click.Group:
         task_group_id = task_group.get_id()
         group = self._get_cli_group(task_group)
         if task_group_id not in self._subcommands:
             self._subcommands[task_group_id] = []
         if subcommand not in self._subcommands[task_group_id]:
             group.add_command(subcommand)
             self._subcommands[task_group_id].append(subcommand)
         return group
 
-    def _get_cli_group(self, task_group: TaskGroup) -> CliGroup:
+    def _get_cli_group(self, task_group: TaskGroup) -> click.Group:
         task_group_id = task_group.get_id()
         if task_group_id in self._registered_groups:
             return self._registered_groups[task_group_id]
         group_cmd_name = task_group.get_cmd_name()
         group_description = task_group.description
-        group = CliGroup(name=group_cmd_name, help=group_description)
+        group = click.Group(name=group_cmd_name, help=group_description)
         self._registered_groups[task_group_id] = group
         return group
 
-    def _create_cli_command(self, task: BaseTask) -> CliCommand:
+    def _create_cli_command(self, task: BaseTask) -> click.Command:
         task_inputs = task.get_all_inputs()
         task_cmd_name = task.get_cmd_name()
         task_description = task.get_description()
         task_main_loop = task.create_main_loop(env_prefix=self.env_prefix)
-        command = CliCommand(
+        command = click.Command(
             callback=task_main_loop, name=task_cmd_name, help=task_description
         )
+        # by default, add an argument named _args
+        command.params.append(click.Argument(['_args'], nargs=-1))
+        # add task inputs
         for task_input in task_inputs:
             param_decl = task_input.get_param_decl()
             options = task_input.get_options()
-            command.params.append(CliOption(param_decl, **options))
+            command.params.append(click.Option(param_decl, **options))
         return command
```

### Comparing `zrb-0.0.8/src/zrb/config/config.py` & `zrb-0.0.9/src/zrb/config/config.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/helper/accessories/color.py` & `zrb-0.0.9/src/zrb/helper/accessories/color.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/helper/accessories/name.py` & `zrb-0.0.9/src/zrb/helper/accessories/name.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/helper/cli/create_cli.py` & `zrb-0.0.9/src/zrb/helper/cli/create_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import click
 import os
 
 
 def create_cli() -> click.Group:
     cli = click.Group(name='zrb', help='Your faithful companion.')
 
+    if 'PYTHONUNBUFFERED' not in os.environ:
+        os.environ['PYTHONUNBUFFERED'] = '1'
+
     # load from ZRB_INIT_SCRIPTS environment
     for init_script in init_scripts:
         load_module(script_path=init_script)
 
     # Load zrb_init.py
     project_script = os.path.join(os.getcwd(), 'zrb_init.py')
     if os.path.isfile(project_script):
```

### Comparing `zrb-0.0.8/src/zrb/helper/file/copy_tree.py` & `zrb-0.0.9/src/zrb/helper/file/copy_tree.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/helper/loader/load_module.py` & `zrb-0.0.9/src/zrb/helper/loader/load_module.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/task/base_model.py` & `zrb-0.0.9/src/zrb/task/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from typing import Any, List, Mapping, Optional, Union
 from typeguard import typechecked
-from jinja2 import Template
 from ..helper.accessories.color import (
     get_random_color, is_valid_color, colored
 )
 from ..helper.accessories.icon import get_random_icon
 from ..helper.keyval.get_object_from_keyval import get_object_from_keyval
 from ..helper.string.get_cmd_name import get_cmd_name
 from ..task_env.env import Env
 from ..task_group.group import Group
 
 import datetime
 import logging
 import os
 import sys
 import time
+import jinja2
+
+
+class AnyExtensionFileSystemLoader(jinja2.FileSystemLoader):
+    def get_source(self, environment, template):
+        for search_dir in self.searchpath:
+            file_path = os.path.join(search_dir, template)
+            if os.path.exists(file_path):
+                with open(file_path, 'r') as file:
+                    contents = file.read()
+                    return contents, file_path, lambda: False
+        raise jinja2.TemplateNotFound(template)
 
 
 @typechecked
 class TimeTracker():
 
     def __init__(self):
         self._start_time: float = 0
@@ -138,15 +149,15 @@
         logging.debug(colored_message)
 
     def log_warn(self, message: Any):
         prefix = self._get_log_prefix()
         colored_message = colored(
             f'{prefix}: {message}', attrs=['dark']
         )
-        logging.warn(colored_message)
+        logging.warning(colored_message)
 
     def log_info(self, message: Any):
         prefix = self._get_log_prefix()
         colored_message = colored(
             f'{prefix}: {message}', attrs=['dark']
         )
         logging.info(colored_message)
@@ -190,56 +201,71 @@
         filled_name = name.rjust(13, ' ')
         return f'{info} • {icon} {filled_name}'
 
     def get_input_map(self) -> Mapping[str, Any]:
         return self._input_map
 
     def get_env_map(self) -> Mapping[str, str]:
-        env_map = os.environ
-        env_map['PYTHONUNBUFFERED'] = '1'
-        env_map.update(self._env_map)
-        return env_map
+        return self._env_map
 
-    def inject_env_map(self, env_map: Mapping[str, str]):
+    def inject_env_map(
+        self, env_map: Mapping[str, str], override: bool = False
+    ):
         for key, val in env_map.items():
-            if key not in self._env_map:
+            if override or key not in self._env_map:
                 self._env_map[key] = val
 
-    def render_str(self, text: str) -> str:
-        template = Template(text)
-        data = {
-            'env': get_object_from_keyval(self._env_map),
-            'input': get_object_from_keyval(self._input_map),
-        }
-        self.log_debug(f'Render template: {text}\nWith data: {data}')
-        rendered_text = template.render(data)
-        self.log_debug(f'Rendered text: {rendered_text}')
-        return rendered_text
-
-    def render_float(self, val: Union[str, float]) -> float:
+    def get_float(self, val: Union[str, float]) -> float:
         if isinstance(val, str):
             return float(self.render_str(val))
         return val
 
-    def render_int(self, val: Union[str, int]) -> int:
+    def get_int(self, val: Union[str, int]) -> int:
         if isinstance(val, str):
             return int(self.render_str(val))
         return val
 
+    def render_str(self, val: str) -> str:
+        template = jinja2.Template(val)
+        data = self._get_default_render_data()
+        self.log_debug(f'Render string template: {val}\nWith data: {data}')
+        rendered_text = template.render(data)
+        self.log_debug(f'Rendered result: {rendered_text}')
+        return rendered_text
+
+    def render_file(self, location: str) -> str:
+        location_dir = os.path.dirname(location)
+        env = jinja2.Environment(
+            loader=AnyExtensionFileSystemLoader([location_dir])
+        )
+        template = env.get_template(location)
+        data = self._get_default_render_data()
+        data['TEMPLATE_DIR'] = location_dir
+        self.log_debug(f'Render template: {location}\nWith data: {data}')
+        rendered_text = template.render(data)
+        self.log_debug(f'Rendered result: {rendered_text}')
+        return rendered_text
+
+    def _get_default_render_data(self) -> Mapping[str, Any]:
+        return {
+            'env': get_object_from_keyval(self._env_map),
+            'input': get_object_from_keyval(self._input_map),
+        }
+
     def set_local_keyval(
         self,
         input_map: Mapping[str, Any],
         env_prefix: str = ''
     ):
         if self._is_keyval_set:
             return True
         self._is_keyval_set = True
         self._input_map = dict(input_map)
         self.log_debug(f'Input map: {self._input_map}')
-        self._env_map = {}
+        self._env_map = os.environ
         for task_env in self.envs:
             env_name = task_env.name
             env_value = task_env.get(env_prefix)
             self._env_map[env_name] = env_value
         self.log_debug(f'Env map: {self._env_map}')
 
     def _get_complete_name(self):
```

### Comparing `zrb-0.0.8/src/zrb/task/base_task.py` & `zrb-0.0.9/src/zrb/task/base_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from typing import Any, List, Mapping, Optional, TypeVar
+from typing import Any, Callable, List, Mapping, Optional, TypeVar
 from typeguard import typechecked
 from .base_model import TaskModel
 from ..task_input.base_input import BaseInput
 from ..task_env.env import Env
 from ..task_group.group import Group
 from ..helper.list.append_unique import append_unique
 
 import asyncio
 import copy
+import inspect
 
 TTask = TypeVar('TTask', bound='BaseTask')
 
 
-def sanitize_interval(interval: float) -> float:
-    if interval <= 0:
-        return 0.1
-    return interval
-
-
 @typechecked
 class BaseTask(TaskModel):
     '''
     Base class for all tasks.
     Every task definition should be extended from this class.
     '''
 
@@ -47,29 +42,46 @@
             envs=envs,
             icon=icon,
             color=color,
             retry=retry
         )
         self.inputs = inputs
         self.description = description
-        self.retry_interval = sanitize_interval(retry_interval)
+        self.retry_interval = self.sanitize_interval(
+            retry_interval, 'retry'
+        )
         self.upstreams = upstreams
         self.checkers = checkers
-        self.checking_interval = sanitize_interval(checking_interval)
+        self.checking_interval = self.sanitize_interval(
+            checking_interval, 'checking'
+        )
         self._is_checked: bool = False
         self._is_executed: bool = False
+        self._runner: Optional[Callable[..., Any]] = None
 
-    async def run(self, **kwargs: Any):
+    def runner(self, runner: Callable[..., Any]):
+        self._runner = runner
+
+    async def run(self, *args: Any, **kwargs: Any) -> Any:
         '''
         Do task execution
         Please override this method.
         '''
         self.log_debug(
-            f'Run with kwargs: {kwargs}'
+            f'Run with args: {args} and kwargs: {kwargs}'
         )
+        if self._runner is not None:
+            result = self._runner(*args, **kwargs)
+            if inspect.isawaitable(result):
+                sync_result = await result
+                self.print_out(sync_result)
+                return sync_result
+            self.print_out(result)
+            return result
+        return True
 
     async def check(self) -> bool:
         '''
         Return true when task is considered completed.
         By default, this will wait the task execution to be completed.
         You can override this method.
         '''
@@ -87,34 +99,42 @@
         return inputs
 
     def get_description(self) -> str:
         if self.description != '':
             return self.description
         return self.name
 
-    def create_main_loop(self, env_prefix: str = ''):
+    def sanitize_interval(self, interval: float, label: str) -> float:
+        if interval < 0:
+            name = self._get_complete_name()
+            self.log_warn(
+                f'Find negative {label} interval for {name}: {interval}'
+            )
+            return 0
+        return interval
+
+    def create_main_loop(self, env_prefix: str = '') -> Callable[..., Any]:
         self_cp = copy.deepcopy(self)
 
-        def main_loop(**kwargs: Any):
+        def main_loop(**kwargs: Any) -> Any:
             '''
             Task main loop.
             '''
-            async def run_and_check_all_async():
+            async def run_and_check_all_async() -> Any:
                 self_cp._set_keyval(input_map=kwargs, env_prefix=env_prefix)
                 processes = [
-                    asyncio.create_task(
-                        self_cp._run_all(**kwargs)
-                    ),
-                    asyncio.create_task(self_cp._loop_check(celebrate=True))
+                    asyncio.create_task(self_cp._loop_check(celebrate=True)),
+                    asyncio.create_task(self_cp._run_all(**kwargs))
                 ]
-                await asyncio.gather(*processes)
+                results = await asyncio.gather(*processes)
+                return results[-1]
             try:
                 return asyncio.run(run_and_check_all_async())
             except Exception:
-                self_cp.log_error('Encounter error')
+                self_cp.log_error('Failed')
                 raise
             finally:
                 self_cp.play_bell()
         return main_loop
 
     async def _loop_check(self, celebrate: bool = False) -> bool:
         while not await self._cached_check():
@@ -147,53 +167,59 @@
             return await self.check()
         check_processes: List[asyncio.Task] = []
         for checker_task in self.checkers:
             check_processes.append(asyncio.create_task(checker_task.run()))
         await asyncio.gather(*check_processes)
         return True
 
-    async def _run_all(self, **kwargs: Any):
+    async def _run_all(self, **kwargs: Any) -> Any:
         processes: List[asyncio.Task] = []
         # Add upstream tasks to processes
         for upstream_task in self.upstreams:
             processes.append(asyncio.create_task(
                 upstream_task._run_all(**kwargs)
             ))
         # Add current task to processes
         processes.append(self._cached_run(**kwargs))
         # Wait everything to complete
-        await asyncio.gather(*processes)
+        results = await asyncio.gather(*processes)
+        return results[-1]
 
-    async def _cached_run(self, **kwargs: Any):
+    async def _cached_run(self, **kwargs: Any) -> Any:
         if self._is_executed:
             self.log_debug('Skip running, because execution flag has been set')
             return
         self._is_executed = True
         self.log_debug('Set execution flag and running')
         self.start_timer()
         # get upstream checker
         upstream_check_processes: List[asyncio.Task] = []
         for upstream_task in self.upstreams:
             upstream_check_processes.append(asyncio.create_task(
                 upstream_task._loop_check()
             ))
         # wait all upstream checkers to complete
         await asyncio.gather(*upstream_check_processes)
+        # initiate args
+        args: List[Any] = [] if '_args' not in kwargs else kwargs['_args']
         # start running task
+        result: Any
         while self.should_attempt():
             try:
-                await self.run(**kwargs)
+                result = await self.run(*args, **kwargs)
                 break
             except Exception:
-                self.log_error('Encounter error')
                 if self.is_last_attempt():
                     raise
+                attempt = self.get_attempt()
+                self.log_error(f'Encounter error on attempt {attempt}')
                 self.increase_attempt()
                 await asyncio.sleep(self.retry_interval)
         self.mark_as_done()
+        return result
 
     def _set_keyval(self, input_map: Mapping[str, Any], env_prefix: str):
         self.set_local_keyval(input_map=input_map, env_prefix=env_prefix)
         for upstream_task in self.upstreams:
             upstream_task._set_keyval(
                 input_map=input_map, env_prefix=env_prefix
             )
```

### Comparing `zrb-0.0.8/src/zrb/task/cmd_task.py` & `zrb-0.0.9/src/zrb/task/cmd_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from ..task_env.env import Env
 from ..task_input.base_input import BaseInput
 from ..task_group.group import Group
 
 import asyncio
 
 
+class CmdResult():
+    def __init__(self, output: str, error: str):
+        self.output = output
+        self.error = error
+
+
 @typechecked
 class CmdTask(BaseTask):
     '''
     Command Task.
     You can use this task to run shell command.
 
     For example:
@@ -32,14 +38,15 @@
     run_server = CmdTask(
         name='run',
         inputs=[StrInput(name='dir', default='.')],
         envs=[Env(name='PORT', os_name='WEB_PORT', default='3000')],
         cmd='python -m http.server $PORT --directory {{input.dir}}',
         checkers=[HTTPChecker(port='{{env.PORT}}')]
     )
+    runner.register(run_server)
     ```
     '''
 
     def __init__(
         self,
         name: str,
         group: Optional[Group] = None,
@@ -51,14 +58,16 @@
         cmd: Union[str, Iterable[str]] = '',
         cmd_path: str = '',
         upstreams: List[BaseTask] = [],
         checkers: List[BaseTask] = [],
         checking_interval: float = 0.1,
         retry: int = 2,
         retry_interval: float = 1,
+        max_output_line: int = 1000,
+        max_error_line: int = 1000
     ):
         BaseTask.__init__(
             self,
             name=name,
             group=group,
             inputs=inputs,
             envs=envs,
@@ -69,76 +78,109 @@
             checkers=checkers,
             checking_interval=checking_interval,
             retry=retry,
             retry_interval=retry_interval
         )
         self.cmd = cmd
         self.cmd_path = cmd_path
+        self.max_output_size = max_output_line
+        self.max_error_size = max_error_line
+        self._output_buffer: List[str] = []
+        self._error_buffer: List[str] = []
+
+    def create_main_loop(
+        self, env_prefix: str = ''
+    ) -> Callable[..., CmdResult]:
+        return super().create_main_loop(env_prefix)
 
-    async def run(self, **kwargs: Any):
-        cmd = self.get_cmd()
+    async def run(self, *args: Any, **kwargs: Any) -> CmdResult:
+        cmd = self._get_cmd_str()
         env = self.get_env_map()
         self.log_debug(f'Run command: {cmd}\nwith env: {env}')
+        self._output_buffer = []
+        self._error_buffer = []
         process = await asyncio.create_subprocess_shell(
             cmd,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
             env=env,
             shell=True
         )
         self.set_task_pid(process.pid)
+        await self._wait_process(process)
+        # get output and error
+        output = '\n'.join(self._output_buffer)
+        error = '\n'.join(self._error_buffer)
+        # get return code
+        return_code = process.returncode
+        if return_code != 0:
+            self.log_debug(f'Exit status: {return_code}')
+            raise Exception(
+                f'Process {self.name} exited ({return_code}): {error}'
+            )
+        return CmdResult(output, error)
+
+    async def _wait_process(self, process: asyncio.subprocess.Process):
         # Create queue
         stdout_queue = asyncio.Queue()
         stderr_queue = asyncio.Queue()
-        # Create reader task
-        stdout_task = asyncio.create_task(self._stream_reader(
+        # Read from streams and put into queue
+        stdout_process = asyncio.create_task(self._queue_stream(
             process.stdout, stdout_queue
         ))
-        stderr_task = asyncio.create_task(self._stream_reader(
+        stderr_process = asyncio.create_task(self._queue_stream(
             process.stderr, stderr_queue
         ))
-        # Create logger task
-        stdout_logger_task = asyncio.create_task(
-            self._stream_logger(self.print_out, stdout_queue)
-        )
-        stderr_logger_task = asyncio.create_task(
-            self._stream_logger(self.print_err, stderr_queue)
-        )
+        # Handle messages in queue
+        stdout_log_process = asyncio.create_task(self._log_from_queue(
+            stdout_queue, self.print_out,
+            self._output_buffer, self.max_output_size
+        ))
+        stderr_log_process = asyncio.create_task(self._log_from_queue(
+            stderr_queue, self.print_err,
+            self._error_buffer, self.max_error_size
+        ))
         # wait process
         await process.wait()
         # wait reader and logger
-        await stdout_task
-        await stderr_task
+        await stdout_process
+        await stderr_process
         await stdout_queue.put(None)
         await stderr_queue.put(None)
-        await stdout_logger_task
-        await stderr_logger_task
-        # get return code
-        return_code = process.returncode
-        if return_code != 0:
-            self.log_debug(f'Exit status: {return_code}')
-            raise Exception(f'Process {self.name} exited ({return_code})')
+        await stdout_log_process
+        await stderr_log_process
 
-    def get_cmd(self) -> str:
+    def _get_cmd_str(self) -> str:
         if self.cmd_path != '':
-            cmd_path = self.render_str(self.cmd_path)
-            with open(cmd_path, 'r') as file:
-                return self.render_str(file.read())
+            return self.render_file(self.cmd_path)
         if isinstance(self.cmd, str):
             return self.render_str(self.cmd)
         return self.render_str('\n'.join(self.cmd))
 
-    async def _stream_reader(self, stream, queue: asyncio.Queue):
+    async def _queue_stream(self, stream, queue: asyncio.Queue):
         while True:
             line = await stream.readline()
             if not line:
                 break
             await queue.put(line)
 
-    async def _stream_logger(
-        self, print_log: Callable[[str], None], queue: asyncio.Queue
+    async def _log_from_queue(
+        self,
+        queue: asyncio.Queue,
+        print_log: Callable[[str], None],
+        buffer: List[str],
+        max_size: int
     ):
         while True:
             line = await queue.get()
             if not line:
                 break
-            print_log(line.decode().rstrip())
+            line_str = line.decode().rstrip()
+            self._add_to_buffer(buffer, max_size, line_str)
+            print_log(line_str)
+
+    def _add_to_buffer(
+        self, buffer: List[str], max_size: int, new_line: str
+    ):
+        if len(buffer) >= max_size:
+            buffer.pop(0)
+        buffer.append(new_line)
```

### Comparing `zrb-0.0.8/src/zrb/task/code_maker.py` & `zrb-0.0.9/src/zrb/task/code_maker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Mapping, Optional
+from typing import Any, Callable, List, Mapping, Optional
 from typeguard import typechecked
 from .base_task import BaseTask
 from ..task_env.env import Env
 from ..task_group.group import Group
 from ..task_input.base_input import BaseInput
 from ..helper.file.copy_tree import copy_tree
 
@@ -38,17 +38,27 @@
             checkers=[],
             checking_interval=0.1,
             retry=0,
             retry_interval=0
         )
         self.template_path = template_path
         self.destination_path = destination_path
-        self.replacements = replacements
         self.excudeds = excludes
+        rendered_replacements: Mapping[str, str] = {
+            old: self.render_str(new)
+            for old, new in replacements.items()
+        }
+        self.replacements = rendered_replacements
 
-    async def run(self, **kwargs: Any):
+    def create_main_loop(
+        self, env_prefix: str = ''
+    ) -> Callable[..., bool]:
+        return super().create_main_loop(env_prefix)
+
+    async def run(self, *args: Any, **kwargs: Any) -> bool:
         copy_tree(
             src=self.template_path,
             dst=self.destination_path,
             replacements=self.replacements,
             excludes=self.excudeds
-        )
+        )
+        return True
```

### Comparing `zrb-0.0.8/src/zrb/task/http_checker.py` & `zrb-0.0.9/src/zrb/task/http_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 from typeguard import typechecked
 from http.client import HTTPConnection, HTTPSConnection
 from .base_task import BaseTask
 from ..task_env.env import Env
 from ..task_group.group import Group
 from ..task_input.base_input import BaseInput
 
@@ -48,22 +48,28 @@
         self.host = host
         self.port = port
         self.timeout = timeout
         self.method = method
         self.url = url
         self.is_https = is_https
 
-    async def run(self, **kwargs: Any):
+    def create_main_loop(
+        self, env_prefix: str = ''
+    ) -> Callable[..., bool]:
+        return super().create_main_loop(env_prefix)
+
+    async def run(self, *args: Any, **kwargs: Any) -> bool:
         method = self.render_str(self.method)
         host = self.render_str(self.host)
-        port = self.render_int(self.port)
+        port = self.get_int(self.port)
         url = self.render_str(self.url)
-        timeout = self.render_int(self.timeout)
+        timeout = self.get_int(self.timeout)
         while not self._check_connection(method, host, port, url, timeout):
             await asyncio.sleep(self.checking_interval)
+        return True
 
     def _check_connection(
         self, method: str, host: str, port: int, url: str, timeout: int
     ) -> bool:
         label = self._get_label(method, host, port, url)
         conn = self._get_connection(host, port, timeout)
         try:
```

### Comparing `zrb-0.0.8/src/zrb/task/port_checker.py` & `zrb-0.0.9/src/zrb/task/port_checker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 from typeguard import typechecked
 from .base_task import BaseTask
 from ..task_env.env import Env
 from ..task_group.group import Group
 from ..task_input.base_input import BaseInput
 
 import socket
@@ -42,20 +42,26 @@
             retry=0,
             retry_interval=0
         )
         self.host = host
         self.port = port
         self.timeout = timeout
 
-    async def run(self, **kwargs: Any):
+    def create_main_loop(
+        self, env_prefix: str = ''
+    ) -> Callable[..., bool]:
+        return super().create_main_loop(env_prefix)
+
+    async def run(self, *args: Any, **kwargs: Any) -> bool:
         host = self.render_str(self.host)
-        port = self.render_int(self.port)
-        timeout = self.render_int(self.timeout)
+        port = self.get_int(self.port)
+        timeout = self.get_int(self.timeout)
         while not self._check_port(host, port, timeout):
             await asyncio.sleep(self.checking_interval)
+        return True
 
     def _check_port(
         self, host: str, port: int, url: str, timeout: int
     ) -> bool:
         label = self._get_label(host, port, url)
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             sock.settimeout(timeout)
```

### Comparing `zrb-0.0.8/src/zrb/task_env/env.py` & `zrb-0.0.9/src/zrb/task_env/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     def get(self, prefix: str = '') -> str:
         '''
         Return environment value.
         You can use prefix to distinguish 'DEV', 'PROD'
 
         Example:
         ```python
-        os.setenv('DEV_SERVER', 'localhost')
-        os.setenv('PROD_SERVER', 'example.com')
+        os.environ['DEV_SERVER'] = 'localhost'
+        os.environ['PROD_SERVER'] = 'example.com'
 
         env = Env(name='HOST', os_name='SERVER', default='0.0.0.0')
 
         print(env.get('DEV'))   # will show 'localhost'
         print(env.get('PROD'))  # will show 'example.com'
         print(env.get('STAG'))  # will show '0.0.0.0'
         ```
```

### Comparing `zrb-0.0.8/src/zrb/task_group/group.py` & `zrb-0.0.9/src/zrb/task_group/group.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/task_input/base_input.py` & `zrb-0.0.9/src/zrb/task_input/base_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/src/zrb/task_input/str_input.py` & `zrb-0.0.9/src/zrb/task_input/str_input.py`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/tests/task/test_cmd_task.py` & `zrb-0.0.9/tests/task/cmd_task/test_cmd_task.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,102 +4,86 @@
 
 
 def test_simple_with_no_error():
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello'
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
-    is_error: bool = False
-    try:
-        main_loop()
-    except Exception:
-        is_error = True
-    assert not is_error
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == 'hello'
 
 
 def test_simple_with_error():
     cmd_task = CmdTask(
         name='simple-error',
         cmd='forbidden command'
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
+    main_loop = cmd_task.create_main_loop()
     is_error: bool = False
     try:
-        main_loop(env_prefix='')
+        main_loop()
     except Exception:
         is_error = True
     assert is_error
 
 
 def test_multiline_cmd():
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd=[
             'echo hello',
             'echo hello again',
         ]
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
-    is_error: bool = False
-    try:
-        main_loop()
-    except Exception:
-        is_error = True
-    assert not is_error
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == '\n'.join(['hello', 'hello again'])
 
 
 def test_cmd_path():
     dir_path = pathlib.Path(__file__).parent.absolute()
     cmd_task = CmdTask(
         name='simple-no-error',
-        cmd_path=os.path.join(dir_path, 'sample_cmd', 'hello.sh')
+        cmd_path=os.path.join(dir_path, 'templates', 'hello.sh')
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
-    is_error: bool = False
-    try:
-        main_loop()
-    except Exception:
-        is_error = True
-    assert not is_error
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == 'Hello, World!'
 
 
 def test_upstream_with_no_error():
     upstream_task = CmdTask(
         name='upstream-no-error',
         cmd='echo upstream'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         upstreams=[upstream_task]
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
-    is_error: bool = False
-    try:
-        main_loop()
-    except Exception:
-        is_error = True
-    assert not is_error
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == 'hello'
 
 
 def test_upstream_with_error():
     upstream_task = CmdTask(
         name='upstream-error',
         cmd='forbidden command'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         upstreams=[upstream_task]
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
+    main_loop = cmd_task.create_main_loop()
     is_error: bool = False
     try:
-        main_loop(env_prefix='')
+        main_loop()
     except Exception:
         is_error = True
     assert is_error
 
 
 def test_diamond_upstream():
     upstream_0 = CmdTask(
@@ -117,52 +101,61 @@
         upstreams=[upstream_0]
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         upstreams=[upstream_1, upstream_2]
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
-    is_error: bool = False
-    try:
-        main_loop()
-    except Exception:
-        is_error = True
-    assert not is_error
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == 'hello'
 
 
 def test_checker_with_no_error():
     checker = CmdTask(
         name='check',
         cmd='echo checked'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         checkers=[checker]
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
-    is_error: bool = False
-    try:
-        main_loop()
-    except Exception:
-        is_error = True
-    assert not is_error
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == 'hello'
 
 
 def test_checker_with_error():
     checker = CmdTask(
         name='check',
         cmd='forbidden command'
     )
     cmd_task = CmdTask(
         name='simple-no-error',
         cmd='echo hello',
         checkers=[checker]
     )
-    main_loop = cmd_task.create_main_loop(env_prefix='')
+    main_loop = cmd_task.create_main_loop()
     is_error: bool = False
     try:
         main_loop()
     except Exception:
         is_error = True
     assert is_error
+
+
+def test_long_output():
+    cmd_task = CmdTask(
+        name='long-output',
+        cmd=[
+            'echo 1',
+            'echo 2',
+            'echo 3',
+            'echo 4',
+            'echo 5',
+        ],
+        max_output_line=3,
+    )
+    main_loop = cmd_task.create_main_loop()
+    result = main_loop()
+    assert result.output == '\n'.join(['3', '4', '5'])
```

### Comparing `zrb-0.0.8/toolkit.sh` & `zrb-0.0.9/toolkit.sh`

 * *Files identical despite different names*

### Comparing `zrb-0.0.8/PKG-INFO` & `zrb-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Your faithful companion
 Author-email: Go Frendi Gunawan <gofrendiasgard@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -45,43 +45,61 @@
 ```bash
 ZRB_SCRIPTS=~/personal/zrb_init.py:~/work/zrb_init.py
 ```
 
 Your Zrb script (e.g: `./zrb_init.py`) should contain your task definitions. For example:
 
 ```python
+from typing import Any
 from zrb import (
-    runner, Env, StrInput, Group, CmdTask, HTTPChecker
+    runner, Env, StrInput, Group, Task, CmdTask, HTTPChecker
 )
 
 '''
-Simple task, read input and show output
+Simple Python task, concatenate words
+'''
+concat = Task(
+    name='concat',
+    inputs=[StrInput(name='separator', description='Separator', default=' ')],
+)
+runner.register(concat)
+
+
+# set concat's runner
+@concat.runner
+def run(*args: str, **kwargs: Any) -> str:
+    separator = kwargs.get('separator', ' ')
+    return separator.join(args)
+
+
+'''
+Simple CLI task, read input and show output
 '''
 hello = CmdTask(
     name='hello',
     inputs=[StrInput(name='name', description='Name', default='world')],
     cmd='echo Hello {{input.name}}'
 )
 runner.register(hello)
 
 make = Group(name='make', description='Make things')
 
 '''
-Simple task, part of 'make' group
+Simple CLI task, part of 'make' group
 '''
 make_coffee = CmdTask(
     name='coffee',
     group=make,
     upstreams=[hello],
     cmd='echo Coffee for you ☕'
 )
 runner.register(make_coffee)
 
 '''
-Simple task, part of 'make' group
+Simple CLI task, part of 'make' group
 '''
 make_beer = CmdTask(
     name='beer',
     group=make,
     upstreams=[hello],
     cmd='echo Cheers 🍺'
 )
@@ -91,30 +109,30 @@
 Sub group of 'make'
 '''
 make_gitignore = Group(
     name='gitignore', description='Make gitignore', parent=make
 )
 
 '''
-Simple task, part of 'make_gitignore' group.
+Simple CLI task, part of 'make_gitignore' group.
 Having multiline cmd
 '''
 make_gitignore_python = CmdTask(
     name='node',
     group=make_gitignore,
     cmd=[
         'echo "node_modules/" >> .gitignore'
         'echo ".npm" >> .gitignore'
         'echo "npm-debug.log" >> .gitignore'
     ]
 )
 runner.register(make_gitignore_python)
 
 '''
-Simple task, part of 'make_gitignore' group.
+Simple CLI task, part of 'make_gitignore' group.
 Having multiline cmd
 '''
 make_gitignore_nodejs = CmdTask(
     name='node',
     group=make_gitignore,
     cmd=[
         'echo "__pycache__/" >> .gitignore'
@@ -124,31 +142,32 @@
 runner.register(make_gitignore_nodejs)
 
 server = Group(
     name='server', description='Server related commands'
 )
 
 '''
-Long running task.
+Long running CLI task.
 Run a server and waiting for the port to be ready.
 '''
 run_server = CmdTask(
     name='run',
     group=server,
     upstreams=[make_coffee, make_beer],
     inputs=[StrInput(name='dir', description='Directory', default='.')],
     envs=[Env(name='PORT', os_name='WEB_PORT', default='3000')],
     cmd='python -m http.server $PORT --directory {{input.dir}}',
     checkers=[HTTPChecker(port='{{env.PORT}}')]
 )
 runner.register(run_server)
-
 ```
 
-Once registered, your task will be accessible from the terminal:
+Once registered, your task will be accessible from the terminal.
+
+For example, you can run a server by performing:
 
 ```bash
 export WEB_PORT=8080
 zrb server run
 ```
 
 The output will be similar to this:
@@ -180,15 +199,16 @@
 
 
 cmd_task = CmdTask(
     name='sample',
     cmd='echo hello'
 )
 main_loop = cmd_task.create_main_loop(env_prefix='')
-main_loop() # This run the task
+result = main_loop() # This run the task
+print(result.output) # Should be "hello"
 ```
 
 
 # Configuration
 
 The following configurations are available:
```

