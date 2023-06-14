# Comparing `tmp/upkeep-1.4.1.tar.gz` & `tmp/upkeep-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upkeep-1.4.1.tar", max compression
+gzip compressed data, was "upkeep-1.4.2.tar", max compression
```

## Comparing `upkeep-1.4.1.tar` & `upkeep-1.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2023-04-02 17:48:07.514387 upkeep-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     2693 2023-04-02 17:48:07.514387 upkeep-1.4.1/README.md
--rw-r--r--   0        0        0      977 2023-04-02 17:48:07.514387 upkeep-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/__init__.py
--rw-r--r--   0        0        0      366 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/commands/__init__.py
--rw-r--r--   0        0        0     1149 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/commands/ecleans.py
--rw-r--r--   0        0        0     4045 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/commands/emerges.py
--rw-r--r--   0        0        0     1426 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/commands/esync.py
--rw-r--r--   0        0        0     1925 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/commands/kernel.py
--rw-r--r--   0        0        0     1129 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/constants.py
--rw-r--r--   0        0        0      739 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/decorators.py
--rw-r--r--   0        0        0      112 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/exceptions.py
--rw-r--r--   0        0        0     2669 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/utils/__init__.py
--rw-r--r--   0        0        0    12096 2023-04-02 17:48:07.514387 upkeep-1.4.1/upkeep/utils/kernel.py
--rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 upkeep-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2020-04-20 14:44:56.283989 upkeep-1.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     2693 2020-04-26 05:07:53.597673 upkeep-1.4.2/README.md
+-rw-r--r--   0        0        0     1015 2023-06-14 07:03:18.113388 upkeep-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-01-29 20:50:07.006926 upkeep-1.4.2/upkeep/__init__.py
+-rw-r--r--   0        0        0      366 2023-04-02 04:42:25.896450 upkeep-1.4.2/upkeep/commands/__init__.py
+-rw-r--r--   0        0        0     1122 2023-06-14 07:01:15.030916 upkeep-1.4.2/upkeep/commands/ecleans.py
+-rw-r--r--   0        0        0     4125 2023-06-14 06:59:05.450859 upkeep-1.4.2/upkeep/commands/emerges.py
+-rw-r--r--   0        0        0     1455 2023-06-14 07:01:15.058916 upkeep-1.4.2/upkeep/commands/esync.py
+-rw-r--r--   0        0        0     1884 2023-06-14 07:01:15.052916 upkeep-1.4.2/upkeep/commands/kernel.py
+-rw-r--r--   0        0        0     1129 2023-02-06 06:02:44.131698 upkeep-1.4.2/upkeep/constants.py
+-rw-r--r--   0        0        0      736 2023-06-14 07:01:14.804919 upkeep-1.4.2/upkeep/decorators.py
+-rw-r--r--   0        0        0      111 2023-06-14 07:01:14.812919 upkeep-1.4.2/upkeep/exceptions.py
+-rw-r--r--   0        0        0     2668 2023-06-14 07:01:14.826919 upkeep-1.4.2/upkeep/utils/__init__.py
+-rw-r--r--   0        0        0    12057 2023-04-02 17:50:33.105009 upkeep-1.4.2/upkeep/utils/kernel.py
+-rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 upkeep-1.4.2/PKG-INFO
```

### Comparing `upkeep-1.4.1/LICENSE.txt` & `upkeep-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `upkeep-1.4.1/README.md` & `upkeep-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `upkeep-1.4.1/pyproject.toml` & `upkeep-1.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "upkeep"
-version = "1.4.1"
+version = "1.4.2"
 description = "Portage update helper commands."
 authors = ["Andrew Udvare <audvare@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+packages = [{include = "upkeep"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10,<4"
 click = "^8.1.3"
-loguru = "^0.6.0"
+loguru = ">=0.6,<0.8"
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
-mypy-extensions = "^0.4.3"
+mypy = ">=0.991,<1.4"
 pylint = "^2.15.10"
 pylint-quotes = "^0.2.3"
 rope = "^1.7.0"
 isort = "^5.12.0"
 toml = "^0.10.2"
 
 [tool.poetry.group.testing.dependencies]
-levenshtein = "^0.20.9"
+levenshtein = ">=0.20.9,<0.22.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^6.1.3"
+sphinx = ">=6.1.3,<8.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ecleans = "upkeep.commands:ecleans_command"
```

### Comparing `upkeep-1.4.1/upkeep/commands/ecleans.py` & `upkeep-1.4.2/upkeep/commands/ecleans.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess as sp
 
 import click
 
 from ..decorators import umask
 from ..utils import CommandRunner
 
-__all__ = ('ecleans', )
+__all__ = ('ecleans',)
 ECLEANS_COMMANDS = (('emerge', '--depclean',
                      '--quiet'), ('emerge', '--quiet', '@preserved-rebuild'),
                     ('revdep-rebuild', '--quiet'), ('eclean-dist', '--deep'),
                     ('eclean-pkg', '--deep'), ['rm', '-fR'] +
                     [str(s) for s in Path('/var/tmp/portage').glob('*')])
 
 
@@ -28,14 +28,13 @@
     - ``rm -fR /var/tmp/portage/*``
 
     Returns
     -------
     int
         Exit code of the last command.
     """
-    print('@@ runner = ')
     runner = CommandRunner()
     try:
         for command in ECLEANS_COMMANDS:
             runner.check_call(command)
     except sp.CalledProcessError as e:
         raise click.Abort() from e
```

### Comparing `upkeep-1.4.1/upkeep/commands/emerges.py` & `upkeep-1.4.2/upkeep/commands/emerges.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
             exclude: str | None = None) -> None:
     # pylint: disable=line-too-long
     """
     Runs the following steps:
 
     - ``emerge --oneshot --quiet --update portage``
     - ``emerge --keep-going --tree --quiet --update --deep --newuse @world``
-    - ``emerge --keep-going --quiet @live-rebuild``
-    - ``emerge --keep-going --quiet @preserved-rebuild``
+    - ``emerge --usepkg=n --keep-going --quiet @live-rebuild``
+    - ``emerge --usepkg=n --keep-going --quiet @preserved-rebuild``
     - ``systemctl daemon-reexec`` if applicable
     - upgrade kernel
 
     This function understands the following CLI flags:
 
     - ``-a`` / ``--ask``: Pass ``--ask`` to the ``emerge @world`` command
     - ``-L`` / ``--no-live-rebuild``: Skip ``emerge @live-rebuild`` step
@@ -87,21 +87,22 @@
         runner.check_call(['emerge', '--oneshot', '--update', 'portage'] +
                           verbose_arg)
         runner.check_call([
             'emerge', '--keep-going', '--tree', '--update', '--deep',
             '--newuse', '@world'
         ] + ask_arg + verbose_arg + exclude_arg)
         if live_rebuild:
-            runner.check_call(
-                ('emerge', '--keep-going', '--quiet', '@live-rebuild'))
+            runner.check_call(('emerge', '--keep-going', '--quiet',
+                               '--usepkg=n', '@live-rebuild'))
         if preserved_rebuild:
             runner.check_call((
                 'emerge',
                 '--keep-going',
                 '--quiet',
+                '--usepkg=n',
                 '@preserved-rebuild',
             ))
     except sp.CalledProcessError as e:
         raise click.Abort() from e
     if daemon_reexec:
         try:
             runner.suppress_output(('which', 'systemctl'))
```

### Comparing `upkeep-1.4.1/upkeep/commands/esync.py` & `upkeep-1.4.2/upkeep/commands/esync.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import subprocess as sp
 
 from loguru import logger
 import click
 
 from ..utils import CommandRunner
 
-__all__ = ('esync', )
+__all__ = ('esync',)
 
 
 @click.command()
 @click.option('-d', '--debug', is_flag=True)
 @click.option('-l', '--run-layman', is_flag=True)
 def esync(debug: bool = False, run_layman: bool = False) -> None:
     """
@@ -21,27 +21,27 @@
     - ``layman -S`` (if ``-l`` is passed in CLI arguments and if it is
       available)
     - ``eix-sync``
     """
     runner = CommandRunner()
     if run_layman:
         try:
-            runner.run(('which', 'layman'))
+            runner.run(('which', 'layman'), stdout=sp.PIPE)
         except sp.CalledProcessError as e:
             logger.error('You need to have app-portage/layman installed')
             raise click.Abort() from e
         try:
             runner.run(('layman', '-S'))
         except sp.CalledProcessError as e:
             raise click.Abort() from e
     try:
-        runner.run(('which', 'eix-sync'))
+        runner.run(('which', 'eix-sync'), stdout=sp.PIPE)
     except sp.CalledProcessError as e:
         msg: str | None = None
         if e.returncode != 2:
             msg = 'You need to have app-portage/eix installed for this to work'
         raise click.Abort(msg) from e
-    sync_args = ('-a', ) if debug else ('-a', '-q', '-H')
+    sync_args = ('-a',) if debug else ('-a', '-q', '-H')
     try:
-        runner.run(('eix-sync', ) + sync_args, check=True)
+        runner.run(('eix-sync',) + sync_args, check=True)
     except sp.CalledProcessError as e:
         raise click.Abort() from e
```

### Comparing `upkeep-1.4.1/upkeep/commands/kernel.py` & `upkeep-1.4.2/upkeep/commands/kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,20 @@
         optional configuration path string.
 
     Returns
     -------
     callable
         Callable that takes no parameters and returns an integer.
     """
-
     @click.command(func.__name__)
-    @click.option('-c',
-                  '--config',
-                  default=DEFAULT_USER_CONFIG,
-                  help=f'Configuration file. Defaults to {DEFAULT_USER_CONFIG}'
-                  )
+    @click.option(
+        '-c',
+        '--config',
+        default=DEFAULT_USER_CONFIG,
+        help=f'Configuration file. Defaults to {DEFAULT_USER_CONFIG}')
     @click.option('-j',
                   '--number-of-jobs',
                   type=int,
                   default=cpu_count() + 1,
                   help='Number of tasks to run simultaneously')
     @umask(new_umask=0o022)
     def ret(number_of_jobs: int = 0,
```

### Comparing `upkeep-1.4.1/upkeep/constants.py` & `upkeep-1.4.2/upkeep/constants.py`

 * *Files identical despite different names*

### Comparing `upkeep-1.4.1/upkeep/decorators.py` & `upkeep-1.4.2/upkeep/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # SPDX-License-Identifier: MIT
 from functools import wraps
 from os import umask as set_umask
 from typing import Callable, ParamSpec, TypeVar
 
-__all__ = ('umask', )
+__all__ = ('umask',)
 
 P = ParamSpec('P')
 T = TypeVar('T')
 
 
 def umask(new_umask: int,
           restore: bool = False) -> Callable[[Callable[P, T]], Callable[P, T]]:
     """Sets the umask before calling the decorated function."""
-
     def decorator_umask(func: Callable[P, T]) -> Callable[P, T]:
-
         @wraps(func)
         def inner(*args: P.args, **kwargs: P.kwargs) -> T:
             old_umask = set_umask(new_umask)
             ret = func(*args, **kwargs)
             if restore:
                 set_umask(old_umask)
             return ret
```

### Comparing `upkeep-1.4.1/upkeep/utils/__init__.py` & `upkeep-1.4.2/upkeep/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     for key in SPECIAL_ENV:
         if environ.get(key):
             env[key] = environ[key]
     return env
 
 
 class CommandRunner:
-
     def run(self,
             args: Sequence[str],
             *,
             check: bool = True,
             env: Mapping[str, str] | None = None,
             stdout: int | None = None,
             stderr: int | None = None) -> CompletedProcess[str]:
```

### Comparing `upkeep-1.4.1/upkeep/utils/kernel.py` & `upkeep-1.4.2/upkeep/utils/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,14 @@
     rebuild_kernel
     """
     runner = CommandRunner()
     kernel_list = runner.run(('eselect', '--colour=no', 'kernel', 'list'),
                              stdout=sp.PIPE)
     lines = (s.strip() for s in kernel_list.stdout.splitlines() if s)
     if not any(re.search(r'\*$', line) for line in lines):
-        print('lines = ', kernel_list)
         logger.info('Select a kernel to upgrade to (eselect kernel set ...).')
         if fatal:
             raise click.Abort()
         return None
     if (len([
             s for s in runner.run(('eselect', '--colour=no', '--brief',
                                    'kernel', 'list'),
```

### Comparing `upkeep-1.4.1/PKG-INFO` & `upkeep-1.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: upkeep
-Version: 1.4.1
+Version: 1.4.2
 Summary: Portage update helper commands.
 License: MIT
 Author: Andrew Udvare
 Author-email: audvare@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: loguru (>=0.6,<0.8)
 Description-Content-Type: text/markdown
 
 # Easier Gentoo system maintenance
 
 [![Python package](https://github.com/Tatsh/upkeep/workflows/Python%20package/badge.svg)](https://github.com/Tatsh/upkeep/actions?query=workflow%3A%22Python+package%22)
 [![Coverage Status](https://coveralls.io/repos/github/Tatsh/upkeep/badge.svg?branch=master)](https://coveralls.io/github/Tatsh/upkeep?branch=master)
```

