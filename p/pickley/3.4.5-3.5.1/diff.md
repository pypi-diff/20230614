# Comparing `tmp/pickley-3.4.5.tar.gz` & `tmp/pickley-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.4.5.tar", last modified: Thu May 11 23:00:46 2023, max compression
+gzip compressed data, was "pickley-3.5.1.tar", last modified: Tue Jun 13 22:03:07 2023, max compression
```

## Comparing `pickley-3.4.5.tar` & `pickley-3.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.485475 pickley-3.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 22:58:55.000000 pickley-3.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 22:58:55.000000 pickley-3.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-11 23:00:46.485475 pickley-3.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-11 22:58:55.000000 pickley-3.4.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 22:58:55.000000 pickley-3.4.5/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 22:58:55.000000 pickley-3.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 23:00:46.485475 pickley-3.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-11 22:58:55.000000 pickley-3.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.481475 pickley-3.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.481475 pickley-3.4.5/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36403 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30237 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.481475 pickley-3.4.5/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.485475 pickley-3.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 22:01:36.000000 pickley-3.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 22:01:36.000000 pickley-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:03:07.618745 pickley-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 22:01:36.000000 pickley-3.5.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 22:01:36.000000 pickley-3.5.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:01:36.000000 pickley-3.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 22:03:07.618745 pickley-3.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 22:01:36.000000 pickley-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31262 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-06-13 22:01:36.000000 pickley-3.5.1/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 22:03:07.000000 pickley-3.5.1/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 22:03:07.618745 pickley-3.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-13 22:01:36.000000 pickley-3.5.1/tests/test_venv.py
```

### Comparing `pickley-3.4.5/LICENSE` & `pickley-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.4.5/PKG-INFO` & `pickley-3.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.4.5
+Version: 3.5.1
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
@@ -51,21 +51,19 @@
     :target: https://github.com/codrsquad/pickley
     :alt: Python versions tested (link to github project)
 
 
 Overview
 ========
 
-See: `major changes in v3.0 <https://github.com/codrsquad/pickley/discussions/9>`_
-
 **pickley** allows to install and keep up-to-date standalone pip-installable python CLIs
-such as tox_, twine_, etc. A bit like brew_ or apt_, but based solely on pypi_
+such as tox_, hatch_, etc.
 
-It is similar to pipx_, but supports any python (including py2), offers self-auto-upgrade, and
-can ``package`` folders as well (for deployment, as venv or pex_ currently).
+It is `similar to pipx`_, main difference being installed CLIs automatically self-upgrade
+as you use them.
 
 It can work out of the box, **without any configuration**:
 
 - **pickley** is portable, it will run and install other CLIs in the same folder it's running from
   (drop it in ``~/.local/bin`` or ``/usr/local/bin`` for example)
 
 - All pypi packages with ``console_scripts`` entry point(s) can be immediately installed
@@ -84,41 +82,41 @@
 
 - You can use the **symlink** delivery method, which will use symlinks instead of self-upgrading wrapper
 
 
 Example
 =======
 
-Once you have pickley_, you can get other python CLIs and use them as standalone programs, for example::
+Once you have ``pickley``, you can get other python CLIs and use them as standalone programs, for example::
 
     # One-liner to grab pickley, and drop it in ~/.local/bin
     $ curl -fsSL https://raw.githubusercontent.com/codrsquad/pickley/master/src/pickley/bstrap.py | /usr/bin/python3 -
 
     # Double-check you do have ~/.local/bin in your PATH
     $ which -a pickley
     ~/.local/bin/pickley
 
     $ pickley base
     ~/.local/bin
 
-    $ pickley install tox twine
-    Installed tox v3.21.4 in 6 seconds 501 ms
-    Installed twine v3.3.0 in 6 seconds 901 ms
+    $ pickley install tox hatch
+    Installed tox v4.5.2 in 6 seconds 501 ms
+    Installed hatch v1.7.0 in 15 seconds
 
     $ which tox
     ~/.local/bin/tox
 
     $ tox --version
     tox version 3.21.4
 
     $ pickley list
     | Package    | Version |
     -------------|----------
-    | tox        | 3.21.4  |
-    | twine      | 3.3.0   |
+    | tox        | 4.5.2   |
+    | hatch      | 1.7.0   |
 
 
 Configuration
 =============
 
 See config_
 
@@ -169,30 +167,16 @@
 
     git clone https://github.com/codrsquad/pickley.git
     cd pickley
     tox -e venv
     .venv/bin/pickley --help
 
 
-.. _pickley: https://pypi.org/project/pickley/
-
 .. _pypi: https://pypi.org/
 
-.. _pip: https://pypi.org/project/pip/
-
-.. _pipx: https://pypi.org/project/pipx/
-
-.. _pex: https://pypi.org/project/pex/
-
-.. _virtualenv: https://pypi.org/project/virtualenv/
-
-.. _shiv: https://pypi.org/project/shiv/
-
-.. _brew: https://brew.sh/
-
-.. _apt: https://en.wikipedia.org/wiki/APT_(Debian)
-
 .. _tox: https://pypi.org/project/tox/
 
-.. _twine: https://pypi.org/project/twine/
+.. _hatch: https://pypi.org/project/hatch/
 
 .. _config: https://github.com/codrsquad/pickley/wiki/Config
+
+.. _similar to pipx: https://github.com/codrsquad/pickley/wiki/Pickley-vs-pipx
```

### Comparing `pickley-3.4.5/README.rst` & `pickley-3.5.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,21 +17,19 @@
     :target: https://github.com/codrsquad/pickley
     :alt: Python versions tested (link to github project)
 
 
 Overview
 ========
 
-See: `major changes in v3.0 <https://github.com/codrsquad/pickley/discussions/9>`_
-
 **pickley** allows to install and keep up-to-date standalone pip-installable python CLIs
-such as tox_, twine_, etc. A bit like brew_ or apt_, but based solely on pypi_
+such as tox_, hatch_, etc.
 
-It is similar to pipx_, but supports any python (including py2), offers self-auto-upgrade, and
-can ``package`` folders as well (for deployment, as venv or pex_ currently).
+It is `similar to pipx`_, main difference being installed CLIs automatically self-upgrade
+as you use them.
 
 It can work out of the box, **without any configuration**:
 
 - **pickley** is portable, it will run and install other CLIs in the same folder it's running from
   (drop it in ``~/.local/bin`` or ``/usr/local/bin`` for example)
 
 - All pypi packages with ``console_scripts`` entry point(s) can be immediately installed
@@ -50,41 +48,41 @@
 
 - You can use the **symlink** delivery method, which will use symlinks instead of self-upgrading wrapper
 
 
 Example
 =======
 
-Once you have pickley_, you can get other python CLIs and use them as standalone programs, for example::
+Once you have ``pickley``, you can get other python CLIs and use them as standalone programs, for example::
 
     # One-liner to grab pickley, and drop it in ~/.local/bin
     $ curl -fsSL https://raw.githubusercontent.com/codrsquad/pickley/master/src/pickley/bstrap.py | /usr/bin/python3 -
 
     # Double-check you do have ~/.local/bin in your PATH
     $ which -a pickley
     ~/.local/bin/pickley
 
     $ pickley base
     ~/.local/bin
 
-    $ pickley install tox twine
-    Installed tox v3.21.4 in 6 seconds 501 ms
-    Installed twine v3.3.0 in 6 seconds 901 ms
+    $ pickley install tox hatch
+    Installed tox v4.5.2 in 6 seconds 501 ms
+    Installed hatch v1.7.0 in 15 seconds
 
     $ which tox
     ~/.local/bin/tox
 
     $ tox --version
     tox version 3.21.4
 
     $ pickley list
     | Package    | Version |
     -------------|----------
-    | tox        | 3.21.4  |
-    | twine      | 3.3.0   |
+    | tox        | 4.5.2   |
+    | hatch      | 1.7.0   |
 
 
 Configuration
 =============
 
 See config_
 
@@ -135,30 +133,16 @@
 
     git clone https://github.com/codrsquad/pickley.git
     cd pickley
     tox -e venv
     .venv/bin/pickley --help
 
 
-.. _pickley: https://pypi.org/project/pickley/
-
 .. _pypi: https://pypi.org/
 
-.. _pip: https://pypi.org/project/pip/
-
-.. _pipx: https://pypi.org/project/pipx/
-
-.. _pex: https://pypi.org/project/pex/
-
-.. _virtualenv: https://pypi.org/project/virtualenv/
-
-.. _shiv: https://pypi.org/project/shiv/
-
-.. _brew: https://brew.sh/
-
-.. _apt: https://en.wikipedia.org/wiki/APT_(Debian)
-
 .. _tox: https://pypi.org/project/tox/
 
-.. _twine: https://pypi.org/project/twine/
+.. _hatch: https://pypi.org/project/hatch/
 
 .. _config: https://github.com/codrsquad/pickley/wiki/Config
+
+.. _similar to pipx: https://github.com/codrsquad/pickley/wiki/Pickley-vs-pipx
```

### Comparing `pickley-3.4.5/setup.py` & `pickley-3.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.5/src/pickley/__init__.py` & `pickley-3.5.1/src/pickley/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.4.5"
+__version__ = "3.5.1"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
-DOT_META = ".pickley"
+DOT_META = ".pk"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
     "facultative", "install_timeout", "min_python", "preferred_min_python", "preferred_pythons", "pyenv", "version", "version_check_delay"
 }
 PLATFORM = platform.system().lower()
@@ -198,22 +198,14 @@
         )
 
     @runez.cached_property
     def pinned(self):
         return self.cfg.pinned_version(self)
 
     @runez.cached_property
-    def _pickley_dev_mode(self):
-        """Path to pickley source folder, if we're running in dev mode"""
-        if self.dashed == PICKLEY:
-            dev_path = self.cfg.pickley_dev_path()
-            if dev_path:
-                return dev_path
-
-    @runez.cached_property
     def index(self):
         """Index to use for this package spec"""
         return self.cfg.index(self)
 
     @property
     def desired_track(self):
         if self._desired_track is None:
@@ -251,40 +243,44 @@
         if self._manifest is None:
             self._manifest = TrackedManifest.from_file(self.manifest_path)
 
         return self._manifest
 
     @runez.cached_property
     def manifest_path(self):
-        return self.cfg.meta.full_path(self.dashed, ".manifest.json")
-
-    @runez.cached_property
-    def meta_path(self):
-        return self.cfg.meta.full_path(self.dashed)
+        return self.cfg.meta.full_path(f"{self.dashed}.manifest.json")
 
     @runez.cached_property
     def ping_path(self):
         """Path to .ping file (for throttle auto-upgrade checks)"""
         return self.cfg.cache.full_path(f"{self.dashed}.ping")
 
+    @runez.cached_property
+    def active_install_path(self):
+        """Currently active installed venv (symlink)"""
+        return self.cfg.meta.full_path(self.dashed)
+
     @property
     def is_currently_installed(self):
         manifest = self.manifest
         return manifest and manifest.version
 
     @runez.cached_property
     def is_already_installed_by_pickley(self):
         """bool: True if this package was already installed by pickley once"""
         return self.dashed == PICKLEY or os.path.exists(self.manifest_path)
 
-    def get_install_path(self, version):
-        if self._pickley_dev_mode:
-            return self.cfg.meta.full_path(PICKLEY, f"{PICKLEY}-dev")
+    def pip_spec(self):
+        if self.folder:
+            return [self.folder]
+
+        if self.dashed == PICKLEY and runez.DEV.project_folder:
+            return ["-e", runez.DEV.project_folder]
 
-        return self.cfg.meta.full_path(self.dashed, f"{self.dashed}-{version}")
+        return [f"{self.dashed}=={self.desired_track.version}"]
 
     def get_lock_path(self):
         """str: Path to lock file used during installation for this package"""
         return self.cfg.meta.full_path(f"{self.dashed}.lock")
 
     def skip_reason(self, force=False):
         """str: Reason for skipping installation, when applicable"""
@@ -325,16 +321,15 @@
         if manifest and manifest.version:
             if manifest.entrypoints:
                 for name in manifest.entrypoints:
                     exe_path = self.exe_path(name)
                     if not runez.is_executable(exe_path):
                         return False
 
-            install_folder = self.get_install_path(manifest.version)
-            py_path = self.cfg.available_pythons.resolved_python_exe(install_folder)
+            py_path = self.cfg.available_pythons.resolved_python_exe(self.active_install_path)
             if py_path:
                 return runez.run(py_path, "--version", dryrun=False, fatal=False, logger=False).succeeded
 
     def find_wheel(self, folder, fatal=True):
         """list[str]: Wheel for this package found in 'folder', if any"""
         if runez.DRYRUN:
             return [f"{self.wheelified}-{self.desired_track.version}-py3-none-any.whl"]
@@ -347,76 +342,63 @@
                     result.append(os.path.join(folder, fname))
 
             if len(result) == 1:
                 return result[0]
 
         return runez.abort(f"Expecting 1 wheel, found: {runez.short(result)}", fatal=fatal, return_value=None)
 
+    def delete_all_files(self):
+        """Delete all files in DOT_META/ folder related to this package spec"""
+        runez.delete(self.manifest_path, fatal=False)
+        for candidate, version in self.installed_sibling_folders():
+            runez.delete(candidate, fatal=False)
+
+    def installed_sibling_folders(self):
+        folder = runez.to_path(self.cfg.meta.path)
+        if folder.is_dir():
+            prefix = f"{self.dashed}-"
+            for item in folder.iterdir():
+                if item.name.startswith(prefix):
+                    yield item, item.name[len(prefix):]
+
     def groom_installation(self, keep_for=60):
         """
         Args:
             keep_for (int): Minimum time in minutes for how long to keep the previous latest version
         """
-        if self._pickley_dev_mode:
+        candidates = []
+        manifest = self.manifest
+        now = time.time()
+        for candidate, version in self.installed_sibling_folders():
+            age = now - os.path.getmtime(candidate)
+            if version != manifest.version:
+                candidates.append((age, candidate))
+
+        if not candidates:
             return
 
-        if self.cfg.cache.contains(self.folder):
-            runez.delete(self.folder, logger=False)
+        candidates = sorted(candidates)
+        youngest = candidates[0]
+        for candidate in candidates[1:]:
+            runez.delete(candidate[1], fatal=False)
 
-        meta_path = self.meta_path
-        current_age = None
-        manifest = self.manifest
-        if manifest and os.path.isdir(meta_path):
-            now = time.time()
-            candidates = []
-            for fname in os.listdir(meta_path):
-                if fname.startswith("."):  # Pickley meta files start with '.'
-                    continue
-
-                fpath = os.path.join(meta_path, fname)
-                vpart = fname[len(self.dashed) + 1:]
-                age = now - os.path.getmtime(fpath)
-                if vpart == manifest.version:
-                    current_age = age
-
-                else:
-                    version = Version(vpart)
-                    if not version.is_valid:
-                        # Not a proper installation
-                        runez.delete(fpath, fatal=False)
-                        continue
-
-                    # Different version, previously installed
-                    candidates.append((age, version, fpath))
-
-            if not candidates:
-                return
-
-            candidates = sorted(candidates)
-            youngest = candidates[0]
-            for candidate in candidates[1:]:
-                runez.delete(candidate[2], fatal=False)
-
-            if current_age:
-                current_age = min(current_age, youngest[0])
-                if current_age > (keep_for * runez.date.SECONDS_IN_ONE_MINUTE):
-                    runez.delete(youngest[2], fatal=False)
+        if youngest[0] > (keep_for * runez.date.SECONDS_IN_ONE_MINUTE):
+            runez.delete(youngest[1], fatal=False)
 
     def save_manifest(self, entry_points):
         manifest = TrackedManifest(
             self.manifest_path,
             self.settings,
             entry_points,
             pinned=self.pinned,
             version=self.desired_track.version,
         )
         payload = manifest.to_dict()
         runez.save_json(payload, self.manifest_path)
-        path = self.get_install_path(self.desired_track.version)
-        runez.save_json(payload, os.path.join(path, ".manifest.json"))
+        runez.save_json(payload, os.path.join(self.active_install_path, ".manifest.json"))
         self._manifest = manifest
         return manifest
 
     def get_latest(self, force=False):
         """Tracked in DOT_META/.cache/<package>.latest"""
         if force or self._latest is None:
             path = self.cfg.cache.full_path(f"{self.dashed}.latest")
@@ -443,37 +425,22 @@
         index = conf.get("global", {}).get("index-url")
         if index:
             return path, index
 
     return None, None
 
 
-def get_program_path(path=None):
-    if path is None:
-        path = runez.resolved_path(sys.argv[0])
-
-    if path.endswith(".py") or path.endswith(".pyc"):
-        packaged = runez.SYS_INFO.venv_bin_path(PICKLEY)
-        if runez.is_executable(packaged):
-            path = packaged  # Convenience when running from debugger
-
-    return path
-
-
 class PickleyConfig:
     """Pickley configuration"""
 
     base = None  # type: FolderBase # Installation folder
     meta = None  # type: FolderBase # DOT_META subfolder
     cache = None  # type: FolderBase # DOT_META/.cache subfolder
     cli = None  # type: TrackedSettings # Tracks any custom CLI cfg flags given, such as --index, --python or --delivery
     configs = None  # type: list
-    program_path = get_program_path()
-
-    _pickley_dev_path = None
 
     def __init__(self):
         self.configs = []
         self.config_path = None
         self.pip_conf, self.pip_conf_index = get_default_index("~/.config/pip/pip.conf", "/etc/pip.conf")
         self.default_index = self.pip_conf_index or DEFAULT_PYPI
         self._explored = set()
@@ -489,28 +456,21 @@
         depot.find_preferred_python(
             self.get_value("preferred_pythons"),
             min_python=self.get_value("min_python"),
             preferred_min_python=self.get_value("preferred_min_python")
         )
         return depot
 
-    @classmethod
-    def pickley_dev_path(cls):
-        if cls._pickley_dev_path is None:
-            cls._pickley_dev_path = runez.DEV.project_folder
-
-        return cls._pickley_dev_path
-
     def set_base(self, base_path):
         """
         Args:
             base_path (str): Path to pickley base installation
         """
         self.configs = []
-        self.base = FolderBase("base", base_path)
+        self.base = FolderBase("base", runez.resolved_path(base_path))
         self.meta = FolderBase("meta", os.path.join(self.base.path, DOT_META))
         self.cache = FolderBase("cache", os.path.join(self.meta.path, ".cache"))
         if self.cli:
             cli = runez.serialize.json_sanitized(self.cli.to_dict())
             self.configs.append(RawConfig(self, "cli", cli))
 
         self._add_config_file(self.config_path)
@@ -606,24 +566,50 @@
             if include_pickley and PICKLEY not in names:
                 names.append(PICKLEY)
 
             result = [self.resolved_bundle(name) for name in names]
             result = runez.flattened(result, unique=True)
             return [PackageSpec(self, name) for name in result]
 
-        result = []
-        if os.path.isdir(self.meta.path):
-            for fname in sorted(os.listdir(self.meta.path)):
-                if include_pickley or fname != PICKLEY:
-                    fpath = os.path.join(self.meta.path, fname)
-                    if os.path.isdir(fpath):
-                        if os.path.exists(os.path.join(fpath, ".manifest.json")):
-                            result.append(PackageSpec(self, fname))
+        return self.installed_specs()
 
-        return result
+    @runez.cached_property
+    def _wrapped_canonical_regex(self):
+        # TODO: Remove once pickley 3.4 is phased out
+        return re.compile(r"\.pickley/([^/]+)/.+/bin/")
+
+    def _wrapped_canonical(self, path):
+        """(str | None): Canonical name of installed python package, if installed via pickley wrapper"""
+        if runez.is_executable(path):
+            for line in runez.readlines(path, first=12):
+                if line.startswith("# pypi-package:"):
+                    return line[15:].strip()
+
+                # TODO: Remove once pickley 3.4 is phased out
+                m = self._wrapped_canonical_regex.search(line)
+                if m:
+                    return m.group(1)
+
+    def scan_installed(self):
+        """Scan installed"""
+        for item in self.base.iterdir():
+            spec_name = self._wrapped_canonical(item)
+            if spec_name:
+                yield spec_name
+
+        for item in self.meta.iterdir():
+            if item.name.endswith(".manifest.json"):
+                spec_name = item.name[:-14]
+                if spec_name:
+                    yield spec_name
+
+    def installed_specs(self):
+        """(list[PackageSpec]): Currently installed package specs"""
+        spec_names = set(self.scan_installed())
+        return [PackageSpec(self, x) for x in sorted(spec_names)]
 
     def get_nested(self, section, key):
         """
         Args:
             section (str): Nested section to examine
             key (str): Key to look up in nested section
 
@@ -956,31 +942,31 @@
     def __init__(self, name, path):
         """
         Args:
             name (str): Internal name of this folder
             path (str): Path to folder
         """
         self.name = name
-        self.path = runez.resolved_path(path)
+        self.path = path
 
     def __repr__(self):
         return self.path
 
-    def contains(self, path):
-        if path:
-            path = runez.resolved_path(path)
-            return path.startswith(self.path)
+    def iterdir(self):
+        path = runez.to_path(self.path)
+        if path.is_dir():
+            yield from path.iterdir()
 
     def full_path(self, *relative):
         """
         Args:
             *relative: Relative path components
 
         Returns:
-            (str): Full path based on self.path
+            (str): Full path based on `self.path`
         """
         return os.path.join(self.path, *relative)
 
 
 def _log_to_file(message, error=False):
     if runez.log.file_handler is not None:
         # Avoid to log twice to console
```

### Comparing `pickley-3.4.5/src/pickley/bstrap.py` & `pickley-3.5.1/src/pickley/bstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 
 def seed_config(pickley_base, desired_cfg, force=False):
     """Seed pickley config"""
     if desired_cfg:
         desired_cfg = read_json(desired_cfg)
         if desired_cfg and isinstance(desired_cfg, dict):
-            pickley_config = os.path.join(pickley_base, ".pickley", "config.json")
+            pickley_config = os.path.join(pickley_base, ".pk", "config.json")
             cfg = read_optional_json(pickley_config)
             if force or cfg != desired_cfg:
                 msg = "%s with %s" % (short(pickley_config), desired_cfg)
                 if not hdry("Would seed %s" % msg):
                     print("Seeding %s" % msg)
                     ensure_folder(os.path.dirname(pickley_config))
                     with open(pickley_config, "wt") as fh:
@@ -219,16 +219,14 @@
 
     Returns:
         (str | None): Pinned pip version to use, if applicable
     """
     if python_version and python_version < (3, 7):
         return "21.3.1"
 
-    return "22.2.2"  # TODO: pip started looking for <whl>.metadata all of the sudden... what the heck?
-
 
 def create_virtualenv(tmp_folder, python_version, python_exe, venv_folder, virtualenv_version="20.10.0", runner=None, dryrun=None):
     """
     Args:
         tmp_folder (str): Temp folder to use, virtualenv.pyz is downloaded there
         python_version (tuple): Target python version
         python_exe (str): Target python executable
@@ -313,15 +311,15 @@
             if v == pickley_version:
                 print("%s version %s is already installed" % (short(pickley_exe), v))
                 sys.exit(0)
 
             if v and len(v) < 24:  # If long output -> old pickley is busted (stacktrace)
                 print("Replacing older pickley %s" % v)
 
-        pickley_venv = os.path.join(pickley_base, ".pickley", "pickley", "pickley-%s" % pickley_version)
+        pickley_venv = os.path.join(pickley_base, ".pk", "pickley-%s" % pickley_version)
         pv = get_python_version(python3)
         needs_virtualenv = True
         if pv and pv >= (3, 7):
             needs_virtualenv = run_program(python3, "-mvenv", "--clear", pickley_venv, fatal=False)
             if not needs_virtualenv and not DRYRUN:
                 needs_virtualenv = not find_venv_exe(pickley_venv, "pip")
```

### Comparing `pickley-3.4.5/src/pickley/cli.py` & `pickley-3.5.1/src/pickley/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 from collections import namedtuple
 
 import click
 import runez
 from runez.pyenv import Version
 from runez.render import PrettyTable
 
-from pickley import __version__, abort, despecced, DOT_META, inform, PackageSpec, PickleyConfig, specced
-from pickley.delivery import PICKLEY
+from pickley import __version__, abort, despecced, DOT_META, inform, PackageSpec, PICKLEY, PickleyConfig, specced
 from pickley.package import PexPackager, PythonVenv, VenvPackager
 
 
 LOG = logging.getLogger(__name__)
 PACKAGER = VenvPackager  # Packager to use for this run
 CFG = PickleyConfig()
 
@@ -128,55 +127,59 @@
 
         if CFG.base:
             runez.Anchored.pop(CFG.base.path)
 
         runez.delete(self.lock_path, logger=False)
 
 
-def perform_install(pspec, is_upgrade=False, force=False, quiet=False, no_binary=None):
+def perform_install(pspec, is_upgrade=False, force=False, quiet=False, no_binary=None, verb=None):
     """
     Args:
         pspec (PackageSpec): Package spec to install
         is_upgrade (bool): If True, intent is an upgrade (not a new install)
         force (bool): If True, check latest version even if recently checked
         quiet (bool): If True, don't chatter
+        verb (str): Verb to use to convey what kind of installation is being done (ex: auto-heal)
 
     Returns:
         (pickley.TrackedManifest): Manifest is successfully installed (or was already up-to-date)
     """
+    if not verb:
+        verb = "upgrade" if is_upgrade else "install"
+
     with SoftLock(pspec):
         started = time.time()
         skip_reason = pspec.skip_reason(force)
         if skip_reason:
             inform(f"Skipping installation of {pspec}: {runez.bold(skip_reason)}")
             return None
 
         if is_upgrade and not pspec.is_currently_installed and not quiet:
             abort(f"'{runez.red(pspec)}' is not installed")
 
         if force:
             pspec.get_latest(force=force)
 
         if pspec.desired_track.problem:
-            action = "upgrade" if is_upgrade else "install"
-            abort(f"Can't {action} {pspec}: {runez.red(pspec.desired_track.problem)}")
+            abort(f"Can't {verb} {pspec}: {runez.red(pspec.desired_track.problem)}")
 
         if not force and pspec.is_up_to_date:
             if not quiet:
                 status = "up-to-date" if is_upgrade else "installed"
                 inform(f"{pspec.dashed} v{runez.bold(pspec.desired_track.version)} is already {status}")
 
             pspec.groom_installation()
             return
 
         setup_audit_log()
         manifest = PACKAGER.install(pspec, no_binary=no_binary)
         if manifest and not quiet:
             note = f" in {runez.represented_duration(time.time() - started)}"
-            action = "Upgraded" if is_upgrade else "Installed"
+            verb += "d" if verb.endswith("e") else "ed"
+            action = "%s%s" % (verb[0].upper(), verb[1:])
             if runez.DRYRUN:
                 action = f"Would state: {action}"
 
             inform(f"{action} {pspec.dashed} v{runez.bold(pspec.desired_track.version)}{runez.dim(note)}")
 
         pspec.groom_installation()
 
@@ -193,24 +196,24 @@
 
         if basename == ".venv":
             return os.path.join(path, "root")  # Convenience for development
 
     return _find_base_from_program_path(dirpath)
 
 
-def find_base():
+def find_base(path=None):
     base_path = runez.resolved_path(os.environ.get("PICKLEY_ROOT"))
     if base_path:
         if not os.path.isdir(base_path):
             abort(f"PICKLEY_ROOT points to non-existing directory {runez.red(base_path)}")
 
         return runez.resolved_path(base_path)
 
-    program_path = PickleyConfig.program_path
-    return _find_base_from_program_path(program_path) or os.path.dirname(program_path)
+    path = path or runez.resolved_path(sys.argv[0])
+    return _find_base_from_program_path(path) or os.path.dirname(path)
 
 
 def clean_env_vars(*keys):
     """Ensure given env vars are removed if present"""
     for key in keys:
         if key in os.environ:
             runez.log.trace(f"Unsetting env var {key}")
@@ -255,15 +258,38 @@
         os.environ["ARCHFLAGS"] = archflags
 
     CFG.set_cli(config, delivery, index, python, virtualenv)
     if ctx.invoked_subcommand != "package":
         CFG.set_base(find_base())
 
 
-@main.command(name="auto-upgrade")
+@main.command()
+def auto_heal():
+    """
+    Automatically re-install packages that have stopped working.
+
+    \b
+    Reasons a package wouldn't be "healthy" anymore:
+    - Base python used to install the packages' venv is not available anymore
+    - The pickley-generated wrapper points to files that have now been deleted
+    """
+    total = healed = 0
+    for spec in CFG.installed_specs():
+        total += 1
+        if spec.is_healthily_installed():
+            print("%s is healthy" % runez.bold(spec))
+            continue
+
+        healed += 1
+        perform_install(spec, verb="auto-heal")
+
+    print("Auto-healed %s / %s packages" % (healed, total))
+
+
+@main.command()
 @click.option("--force", is_flag=True, help="Force auto-upgrade check, even if recently checked")
 @click.argument("package", required=True)
 def auto_upgrade(force, package):
     """Background auto-upgrade command (called by wrapper)"""
     pspec = PackageSpec(CFG, package)
     ping = pspec.ping_path
     if not force and runez.file.is_younger(ping, 5):  # 5 seconds cool down on version check to avoid bursts
@@ -285,17 +311,24 @@
     """Show pickley base folder"""
     path = CFG.base.path
     if what == "bootstrap-own-wrapper":
         # Internal: called by bootstrap script
         from pickley.delivery import DeliveryMethodWrap
 
         pspec = PackageSpec(CFG, f"{PICKLEY}=={__version__}")
-        venv = PythonVenv(CFG.meta.full_path(PICKLEY, f"{PICKLEY}-{__version__}"), pspec, create=False)
+        venv = PythonVenv(CFG.meta.full_path(f"{PICKLEY}-{__version__}"), pspec, create=False)
         wrap = DeliveryMethodWrap()
         wrap.install(venv, {PICKLEY: PICKLEY})
+
+        # TODO: Remove once pickley 3.4 is phased out
+        old_meta = CFG.base.full_path(".pickley")
+        if os.path.isdir(old_meta):
+            runez.delete(old_meta)
+            runez.run(os.path.join(venv.folder, "bin", PICKLEY), "auto-heal")
+
         return
 
     if what:
         paths = {
             "audit": CFG.meta.full_path("audit.log"),
             "cache": CFG.cache.path,
             "config": CFG.meta.full_path("config.json"),
@@ -584,15 +617,15 @@
     for pspec in CFG.package_specs(packages):
         if not pspec.is_already_installed_by_pickley:
             abort(f"{runez.bold(pspec.dashed)} was not installed with pickley")
 
         for ep in pspec.manifest.entrypoints:
             runez.delete(pspec.exe_path(ep))
 
-        runez.delete(pspec.meta_path)
+        pspec.delete_all_files()
         action = "Would uninstall" if runez.DRYRUN else "Uninstalled"
         inform(f"{action} {pspec}")
 
     if all:
         runez.delete(CFG.base.full_path(PICKLEY))
         runez.delete(CFG.meta.path)
         inform(f"pickley is now {runez.red('uninstalled')}")
```

### Comparing `pickley-3.4.5/src/pickley/delivery.py` & `pickley-3.5.1/src/pickley/delivery.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 LOG = logging.getLogger(__name__)
 
 WRAPPER_MARK = "# Wrapper generated by https://pypi.org/project/pickley/"
 
 GENERIC_WRAPPER = """
 #!/bin/bash
 
+# pypi-package: {name}
 %s
 
 if [[ -x {pickley} ]]; then
     {hook}nohup {pickley} auto-upgrade {name}{bg}
 fi
 if [[ -x {source} ]]; then
     {hook}exec {source} "$@"
@@ -28,14 +29,15 @@
 fi
 """ % WRAPPER_MARK
 
 # Specific wrapper for pickley itself (avoid calling ourselves back recursively for auto-upgrade)
 PICKLEY_WRAPPER = """
 #!/bin/bash
 
+# pypi-package: pickley
 %s
 
 if [[ -x {source} ]]; then
     if [[ "$*" != *"auto-"* ]]; then
         {hook}nohup {source} auto-upgrade {name}{bg}
     fi
     {hook}exec {source} "$@"
@@ -78,20 +80,20 @@
     def install(self, venv, entry_points):
         """
         Args:
             venv (pickley.package.PythonVenv): Virtual env where executables reside (DOT_META/<package>/...)
             entry_points (dict | list): Full path of executable to deliver (<base>/<entry_point>)
         """
         if not venv.pspec.is_clear_for_installation():
-            auto_uninstall(venv.pspec.exe_path(venv.pspec.dashed))
+            abort(f"{runez.short(venv.pspec.exe_path(venv.pspec.dashed))} exists and was not installed by pickley")
 
         try:
             prev_manifest = venv.pspec.manifest
             for name in entry_points:
-                src = venv.bin_path(name)
+                src = os.path.join(venv.pspec.active_install_path, "bin", name)
                 dest = venv.pspec.exe_path(name)
                 ssrc = runez.short(src)
                 sdest = runez.short(dest)
                 if runez.DRYRUN:
                     print(f"Would {self.short_name} {sdest} -> {ssrc}")
                     continue
 
@@ -161,48 +163,7 @@
             name=runez.quoted(pspec.dashed, adapter=None),
             pickley=runez.quoted(pickley, adapter=None),
             source=runez.quoted(source, adapter=None),
         )
         runez.delete(target, logger=False)
         runez.write(target, contents, logger=False)
         runez.make_executable(target, logger=False)
-
-
-def auto_uninstall(target):
-    """
-    Args:
-        target (str): Path to executable to auto-uninstall if needed
-
-    Returns:
-        Aborts if uninstallation was not possible
-    """
-    brew, name = find_brew_name(target)
-    if brew and name:
-        result = runez.run(brew, "uninstall", "-f", name, fatal=False, logger=LOG.info)
-        if result.succeeded:
-            LOG.info(f"Auto-uninstalled brew formula '{name}'")
-            return
-
-        command = f"{brew} uninstall {name}"
-        abort(f"'{runez.bold(command)}' failed, please check")
-
-    abort(f"Can't automatically uninstall {runez.short(target)}")
-
-
-def find_brew_name(target):
-    """
-    Args:
-        target (str): Path to executable file
-
-    Returns:
-        (str, str): Name of brew formula, if target was installed with brew
-    """
-    if os.path.islink(target):
-        path = os.path.realpath(target)
-        folder = runez.parent_folder(target)
-        cellar = os.path.join(runez.parent_folder(folder), "Cellar")
-        if path.startswith(cellar):
-            brew = os.path.join(folder, "brew")
-            name, _, _ = path[len(cellar) + 1:].partition("/")
-            return brew, name
-
-    return None, None
```

### Comparing `pickley-3.4.5/src/pickley/package.py` & `pickley-3.5.1/src/pickley/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     def package(pspec, build_folder, dist_folder, requirements, run_compile_all):
         """Package current folder
 
         Args:
             pspec (pickley.PackageSpec): Targeted package spec
             build_folder (str): Folder to use as build cache
             dist_folder (str): Folder where to produce package
-            requirements (list): Additional requirements (same convention as pip, can be package names or package specs)
+            requirements (pickley.cli.Requirements): Additional requirements (same convention as pip, can be package names or package specs)
             run_compile_all (bool): Call 'compileall' on generated package?
 
         Returns:
             (list | None): List of packaged executables
         """
         raise NotImplementedError("Packaging with packager '{packager}' is not supported")
 
@@ -316,30 +316,23 @@
         delivery = DeliveryMethod.delivery_method_by_name(pspec.settings.delivery)
         delivery.ping = ping
         args = []
         if no_binary:
             args.append("--no-binary")
             args.append(no_binary)
 
-        venv_folder = pspec.get_install_path(pspec.desired_track.version)
-        if pspec.folder:
-            args.append(pspec.folder)
-
-        elif pspec._pickley_dev_mode:
-            args.append("-e")
-            args.append(pspec._pickley_dev_mode)
-
-        else:
-            args.append(f"{pspec.dashed}=={pspec.desired_track.version}")
-
+        version = "dev" if pspec.dashed == PICKLEY and runez.DEV.project_folder else pspec.desired_track.version
+        venv_folder = pspec.cfg.meta.full_path(f"{pspec.dashed}-{version}")
         venv = PythonVenv(venv_folder, pspec)
+        args.extend(pspec.pip_spec())
         venv.pip_install(*args)
+        runez.symlink(venv_folder, pspec.active_install_path)
         contents = PackageContents(venv)
         if not contents.entry_points:
-            runez.delete(pspec.meta_path)
+            pspec.delete_all_files()
             abort(f"Can't install '{runez.bold(pspec.dashed)}', it is {runez.red('not a CLI')}")
 
         return delivery.install(venv, contents.entry_points)
 
     @staticmethod
     def package(pspec, build_folder, dist_folder, requirements, run_compile_all):
         runez.ensure_folder(dist_folder, clean=True, logger=False)
```

### Comparing `pickley-3.4.5/src/pickley.egg-info/PKG-INFO` & `pickley-3.5.1/src/pickley.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.4.5
+Version: 3.5.1
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
@@ -51,21 +51,19 @@
     :target: https://github.com/codrsquad/pickley
     :alt: Python versions tested (link to github project)
 
 
 Overview
 ========
 
-See: `major changes in v3.0 <https://github.com/codrsquad/pickley/discussions/9>`_
-
 **pickley** allows to install and keep up-to-date standalone pip-installable python CLIs
-such as tox_, twine_, etc. A bit like brew_ or apt_, but based solely on pypi_
+such as tox_, hatch_, etc.
 
-It is similar to pipx_, but supports any python (including py2), offers self-auto-upgrade, and
-can ``package`` folders as well (for deployment, as venv or pex_ currently).
+It is `similar to pipx`_, main difference being installed CLIs automatically self-upgrade
+as you use them.
 
 It can work out of the box, **without any configuration**:
 
 - **pickley** is portable, it will run and install other CLIs in the same folder it's running from
   (drop it in ``~/.local/bin`` or ``/usr/local/bin`` for example)
 
 - All pypi packages with ``console_scripts`` entry point(s) can be immediately installed
@@ -84,41 +82,41 @@
 
 - You can use the **symlink** delivery method, which will use symlinks instead of self-upgrading wrapper
 
 
 Example
 =======
 
-Once you have pickley_, you can get other python CLIs and use them as standalone programs, for example::
+Once you have ``pickley``, you can get other python CLIs and use them as standalone programs, for example::
 
     # One-liner to grab pickley, and drop it in ~/.local/bin
     $ curl -fsSL https://raw.githubusercontent.com/codrsquad/pickley/master/src/pickley/bstrap.py | /usr/bin/python3 -
 
     # Double-check you do have ~/.local/bin in your PATH
     $ which -a pickley
     ~/.local/bin/pickley
 
     $ pickley base
     ~/.local/bin
 
-    $ pickley install tox twine
-    Installed tox v3.21.4 in 6 seconds 501 ms
-    Installed twine v3.3.0 in 6 seconds 901 ms
+    $ pickley install tox hatch
+    Installed tox v4.5.2 in 6 seconds 501 ms
+    Installed hatch v1.7.0 in 15 seconds
 
     $ which tox
     ~/.local/bin/tox
 
     $ tox --version
     tox version 3.21.4
 
     $ pickley list
     | Package    | Version |
     -------------|----------
-    | tox        | 3.21.4  |
-    | twine      | 3.3.0   |
+    | tox        | 4.5.2   |
+    | hatch      | 1.7.0   |
 
 
 Configuration
 =============
 
 See config_
 
@@ -169,30 +167,16 @@
 
     git clone https://github.com/codrsquad/pickley.git
     cd pickley
     tox -e venv
     .venv/bin/pickley --help
 
 
-.. _pickley: https://pypi.org/project/pickley/
-
 .. _pypi: https://pypi.org/
 
-.. _pip: https://pypi.org/project/pip/
-
-.. _pipx: https://pypi.org/project/pipx/
-
-.. _pex: https://pypi.org/project/pex/
-
-.. _virtualenv: https://pypi.org/project/virtualenv/
-
-.. _shiv: https://pypi.org/project/shiv/
-
-.. _brew: https://brew.sh/
-
-.. _apt: https://en.wikipedia.org/wiki/APT_(Debian)
-
 .. _tox: https://pypi.org/project/tox/
 
-.. _twine: https://pypi.org/project/twine/
+.. _hatch: https://pypi.org/project/hatch/
 
 .. _config: https://github.com/codrsquad/pickley/wiki/Config
+
+.. _similar to pipx: https://github.com/codrsquad/pickley/wiki/Pickley-vs-pipx
```

### Comparing `pickley-3.4.5/src/pickley.egg-info/SOURCES.txt` & `pickley-3.5.1/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.4.5/tests/test_bootstrap.py` & `pickley-3.5.1/tests/test_bootstrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from unittest.mock import patch
 
 import pytest
 import runez
 
-from pickley import __version__, bstrap
+from pickley import __version__, bstrap, DOT_META
 
 
 def mocked_expanduser(path):
     if path and path.startswith("~/"):
         path = path[2:]
 
     return path
@@ -25,66 +25,69 @@
 
 
 def mocked_which(program):
     return None if program == "pickley" else program
 
 
 def test_bootstrap(cli, monkeypatch):
+    runez.touch(".pickley/foo")
     cli.run("-n base bootstrap-own-wrapper")
     assert cli.succeeded
-    assert f"Would save .pickley/pickley/pickley-{__version__}/.manifest.json" in cli.logged
+    assert f"Would save {DOT_META}/pickley.manifest.json" in cli.logged
+    assert "Would delete .pickley" in cli.logged
+    assert f"Would run: .pk/pickley-{__version__}/bin/pickley auto-heal" in cli.logged
 
     with patch("pickley.bstrap.which", side_effect=mocked_which):
         with patch("pickley.bstrap.os.path.expanduser", side_effect=mocked_expanduser):
             runez.write(".local/bin/pickley", "#!/bin/sh\necho 0.1")  # Pretend we have an old pickley
             runez.make_executable(".local/bin/pickley")
 
             with patch("pickley.bstrap.get_python_version", return_value=(3, 6)):  # urllib fails
                 monkeypatch.setenv("__PYVENV_LAUNCHER__", "oh apple, why?")  # macos oddity env var, should be removed
                 monkeypatch.setenv("PATH", ".local/bin:%s" % os.environ["PATH"])
                 cli.run("-n", main=bstrap.main)
                 assert cli.succeeded
                 assert "__PYVENV_LAUNCHER__" not in os.environ
                 assert "Replacing older pickley 0.1" in cli.logged
                 assert "Would run: python virtualenv-20.10.0.pyz -q --clear --pip 21.3.1 -p " in cli.logged
-                assert "Would run: .local/bin/.pickley/pickley/pickley-" in cli.logged
+                assert f"Would run: .local/bin/{DOT_META}/pickley-" in cli.logged
                 monkeypatch.undo()
 
             # Simulate multiple base candidates given
             cli.run("-n", "-b", "~/.local/bin:foo/bar", main=bstrap.main)
             assert cli.failed
             assert "Make sure ~/.local/bin is writeable and in your PATH variable." in cli.logged
 
             # Simulate seeding
             monkeypatch.setenv("PATH", ".local/bin:%s" % os.environ["PATH"])
             cli.run("0.1", "-b", "~/.local/bin", "-m", "my-mirror", "-c", '{"pyenv":"~/.pyenv"}', main=bstrap.main)
             assert cli.succeeded
-            assert "Seeding .local/bin/.pickley/config.json with {'pyenv': '~/.pyenv'}" in cli.logged
+            assert f"Seeding .local/bin/{DOT_META}/config.json with {{'pyenv': '~/.pyenv'}}" in cli.logged
             assert "Seeding .config/pip/pip.conf with my-mirror" in cli.logged
             assert "pickley version 0.1 is already installed" in cli.logged
             assert list(runez.readlines(".config/pip/pip.conf")) == ["[global]", "index-url = my-mirror"]
-            assert list(runez.readlines(".local/bin/.pickley/config.json")) == ["{", '  "pyenv": "~/.pyenv"', "}"]
+            assert list(runez.readlines(f".local/bin/{DOT_META}/config.json")) == ["{", '  "pyenv": "~/.pyenv"', "}"]
 
             monkeypatch.setenv("PATH", "foo/bar:%s" % os.environ["PATH"])
             runez.ensure_folder("foo/bar", logger=None)
             cli.run("-n", "-b", "bar/baz:foo/bar", main=bstrap.main)
             assert cli.succeeded
             assert "base: foo/bar" in cli.logged
 
             with patch("pickley.bstrap.built_in_download"):
                 with patch("pickley.bstrap.get_python_version", return_value=(3, 10)):
                     with patch("pickley.bstrap.run_program", side_effect=mocked_logged_run):
                         # Verify that a python without ensurepip still works (via virtualenv)
                         cli.run("1.0", main=bstrap.main)
                         assert cli.succeeded
                         assert " -mvenv --clear " in cli.logged
-                        assert "virtualenv-20.10.0.pyz -q --clear --pip 22.2.2 -p " in cli.logged
+                        assert "virtualenv-20.10.0.pyz -q --clear --download -p " in cli.logged
 
                         # When pip available, don't use virtualenv
-                        pip = ".local/bin/.pickley/pickley/pickley-1.0/bin/pip3"
+                        pip = f".local/bin/{DOT_META}/pickley-1.0/bin/pip3"
                         runez.touch(pip)
                         runez.make_executable(pip)
                         cli.run("1.0", main=bstrap.main)
                         assert cli.succeeded
                         assert "virtualenv" not in cli.logged
                         assert "pip -q install pickley==1.0" in cli.logged
                         assert "pickley base bootstrap-own-wrapper" in cli.logged
@@ -103,15 +106,15 @@
 
 
 def test_edge_cases(temp_folder, monkeypatch, logged):
     monkeypatch.setattr(bstrap, "DRYRUN", True)
     cmd = bstrap.virtualenv_cmd("vv", (3, 6), "pyexe", "venv")
     assert cmd == [sys.executable, "vv", "-q", "--clear", "--pip", "21.3.1", "-p", "pyexe", "venv"]
     cmd = bstrap.virtualenv_cmd("vv", (3, 7), "pyexe", "venv")
-    assert cmd == [sys.executable, "vv", "-q", "--clear", "--pip", "22.2.2", "-p", "pyexe", "venv"]
+    assert cmd == [sys.executable, "vv", "-q", "--clear", "--download", "-p", "pyexe", "venv"]
 
     monkeypatch.setattr(bstrap, "DRYRUN", False)
     assert bstrap.which("python3")  # Check that which() works
 
     monkeypatch.setattr(bstrap, "RUNNING_FROM_VENV", False)
     assert bstrap.find_python3() == sys.executable
```

### Comparing `pickley-3.4.5/tests/test_config.py` & `pickley-3.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.5/tests/test_ops.py` & `pickley-3.5.1/tests/test_ops.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
-import sys
 import time
 from unittest.mock import patch
 
 import pytest
 import runez
 from runez.http import GlobalHttpCalls
 from runez.pyenv import Version
 
-from pickley import __version__, get_program_path, PackageSpec, PICKLEY, PickleyConfig, TrackedManifest, TrackedVersion
+from pickley import __version__, PackageSpec, PICKLEY, PickleyConfig, TrackedManifest, TrackedVersion
 from pickley.cli import clean_compiled_artifacts, find_base, PackageFinalizer, Requirements, SoftLock, SoftLockException
 from pickley.delivery import WRAPPER_MARK
 from pickley.package import Packager
 
 from .conftest import dot_meta
 
 
@@ -32,25 +31,18 @@
     monkeypatch.setenv("PICKLEY_ROOT", "temp-base")
     with pytest.raises(SystemExit):  # Env var points to a non-existing folder
         find_base()
 
     runez.ensure_folder("temp-base")
     assert find_base() == runez.resolved_path("temp-base")
 
-    assert sys.prefix in get_program_path("foo/bar.py")
-
     monkeypatch.delenv("PICKLEY_ROOT")
-    monkeypatch.setattr(PickleyConfig, "program_path", "/foo/.venv/bin/pickley")
-    assert find_base() == "/foo/.venv/root"
-
-    monkeypatch.setattr(PickleyConfig, "program_path", dot_meta("pickley-0.0.0/bin/pickley", parent="foo"))
-    assert find_base() == "foo"
-
-    monkeypatch.setattr(PickleyConfig, "program_path", "foo/bar")
-    assert find_base() == "foo"
+    assert find_base("/foo/.venv/bin/pickley") == "/foo/.venv/root"
+    assert find_base(dot_meta("pickley-0.0.0/bin/pickley", parent="foo")) == "foo"
+    assert find_base("foo/bar") == "foo"
 
 
 def dummy_finalizer(cfg, dist, symlink="root:root/usr/local/bin"):
     p = PackageFinalizer("foo", dist, symlink, None, None, cfg=cfg)
     p.resolve()
     assert p.pspec.dashed == "foo"
     return p
@@ -104,18 +96,21 @@
     assert not cli.logged.stderr
     assert "cli:  # empty" in cli.logged.stdout
     assert "defaults:" in cli.logged.stdout
 
     cli.run("-n --color config")
     assert cli.succeeded
 
+    cli.expect_success("-n auto-heal", "Auto-healed 0 / 0 packages")
+
     cli.expect_success("-n -Pfoo diagnostics", "desired python : foo", "foo [not available]", "sys.executable")
     cli.run("-n install git@github.com:zsimic/mgit.git")
     assert cli.succeeded
-    assert "pip install .pickley/.cache/checkout/git-github-com-zsimic-mgit-git" in cli.logged
+    checkout = dot_meta(".cache/checkout")
+    assert f"pip install {checkout}/git-github-com-zsimic-mgit-git" in cli.logged
 
     cli.expect_success("-n list", "No packages installed")
 
     cli.expect_failure("-n package foo", "Folder ... does not exist")
     cli.expect_failure("-n package . -sfoo", "Invalid symlink specification")
     cli.expect_failure("-n package . -sroot:root/usr/local/bin", "No setup.py in ")
 
@@ -150,43 +145,43 @@
         assert "Lock file present, another installation is in progress" in cli.logged
 
         cli.expect_success("-n check", "No packages installed")
         cli.expect_failure("-n check foo+bar", "'foo+bar' is not a valid pypi package name")
         cli.expect_failure("-n check mgit pickley2-a", "not installed", "pickley2-a: does not exist")
 
         # Simulate an old entry point that was now removed
-        runez.write(dot_meta("mgit/.manifest.json"), '{"entrypoints": ["bogus-mgit"]}')
+        runez.write(dot_meta("mgit.manifest.json"), '{"entrypoints": ["bogus-mgit"]}')
         cli.expect_failure("-n install mgit pickley2.a", "Would state: Installed mgit v", "'pickley2.a' is not pypi canonical")
 
         cli.expect_failure("check", "not installed")
         cli.expect_success("list", "mgit")
         cli.expect_success("list -fcsv", "mgit")
         cli.expect_success("list -fjson", "mgit")
         cli.expect_success("list -ftsv", "mgit")
         cli.expect_success("list -fyaml", "mgit")
         runez.delete(dot_meta("mgit"))
 
         cli.run("-n --virtualenv latest -Pinvoker install --no-binary :all: mgit==1.3.0")
         assert cli.succeeded
         assert " --no-binary :all: mgit==1.3.0" in cli.logged
         assert cli.match("Would wrap mgit -> %s" % dot_meta("mgit"))
-        assert cli.match("Would save %s" % dot_meta("mgit/.manifest.json"))
+        assert cli.match("Would save %s" % dot_meta("mgit.manifest.json"))
         assert cli.match("Would state: Installed mgit v1.3.0")
 
         cli.expect_failure("-n -dfoo install mgit", "Unknown delivery method 'foo'")
 
 
 def test_dev_mode(cli, monkeypatch):
-    monkeypatch.setattr(PickleyConfig, "_pickley_dev_path", None)
     with patch("runez.pyenv.PypiStd.latest_pypi_version", side_effect=mock_latest_pypi_version):
         cli.run("-n install pickley")
         assert cli.succeeded
-        assert "pip install -e " in cli.logged
-        assert "pickley-dev/bin/pickley" in cli.logged
+        assert ".pk/pickley-dev/bin/pip install -e " in cli.logged
+        assert "Would symlink .pk/pickley-dev <- .pk/pickley" in cli.logged
         assert "pickley-100.0" not in cli.logged
+        assert "Would state: Installed pickley v100.0 in "
 
 
 def test_edge_cases(temp_cfg, logged):
     tv = TrackedVersion(version="1.2")
     assert str(tv) == "1.2"
     pspec = PackageSpec(temp_cfg, PICKLEY)
 
@@ -228,15 +223,15 @@
     cli.expect_success("-n install virtualenv", "Skipping installation of virtualenv: not installed by pickley")
     cli.expect_success("-n check virtualenv", "skipped, not installed by pickley")
 
     # --force ignores 'facultative' setting
     with patch("runez.pyenv.PypiStd.latest_pypi_version", side_effect=mock_latest_pypi_version):
         cli.run("-n install --force virtualenv")
         assert cli.failed
-        assert "Can't automatically uninstall virtualenv" in cli.logged
+        assert "virtualenv exists and was not installed by pickley" in cli.logged
 
         # Simulate pickley symlink delivery
         dummy_target = dot_meta("foo")
         runez.touch(dummy_target)
         runez.symlink(dummy_target, "virtualenv")
         cli.run("-n install virtualenv")
         assert cli.succeeded
@@ -259,94 +254,110 @@
         contents = runez.readlines(path)
         assert WRAPPER_MARK in contents
 
     r = runez.run(path, "--version")
     assert r.succeeded
 
 
-def check_install_from_pypi(cli, delivery, package, simulate_version=None):
-    cli.run("--debug", "-d%s" % delivery, "install", package)
+def check_install_from_pypi(cli, delivery, package, version, simulate_version=None):
+    runez.write(".pk/.cache/mgit.latest", f'{{"version": "{version}"}}')
+    cli.run("--debug", f"-d{delivery}", "install", package)
     assert cli.succeeded
-    assert cli.match("Installed %s" % package)
+    assert cli.match(f"Installed {package} v{version}")
     assert runez.is_executable(package)
-    m = TrackedManifest.from_file(dot_meta("%s/.manifest.json" % package))
+    m = TrackedManifest.from_file(dot_meta(f"{package}.manifest.json"))
     assert str(m)
     assert m.entrypoints[package]
     assert m.install_info.args == runez.quoted(cli.args)
     assert m.install_info.timestamp
     assert m.install_info.vpickley == __version__
     assert m.settings.delivery == delivery
     assert m.settings.python
-    assert m.version
+    assert m.version == version
 
-    r = runez.run(package, "--version")
+    r = runez.run(f"./{package}", "--version")
     assert r.succeeded
+    assert version in r.full_output
 
-    cli.expect_success("--debug auto-upgrade %s" % package, "Skipping auto-upgrade, checked recently")
-    cli.expect_success("install %s" % package, "is already installed")
+    cli.expect_success(f"--debug auto-upgrade {package}", "Skipping auto-upgrade, checked recently")
+    cli.expect_success(f"install {package}", "is already installed")
     if simulate_version:
         # Edge case: simulated user manually deletes the installed wrapper or symlink
         assert os.path.exists(package)
         os.unlink(package)
-        cli.run("--debug", "-d%s" % delivery, "install", package)
+        cli.run("--debug", f"-d{delivery}", "install", package)
         assert cli.succeeded
-        assert cli.match("Installed %s" % package)
+        assert cli.match(f"Installed {package} v{version}")
 
     cli.expect_success("check", " up-to-date")
     cli.expect_success("list", package)
     cli.expect_success("upgrade", "is already up-to-date")
 
     if simulate_version:
         installed_version = m.version
         m.version = simulate_version
-        runez.save_json(m.to_dict(), dot_meta("%s/.manifest.json" % package))
-        cli.expect_success("check", "%s (currently unhealthy)" % installed_version)
+        runez.save_json(m.to_dict(), dot_meta(f"{package}.manifest.json"))
+        cli.expect_success("check", f"{installed_version} (currently {simulate_version})")
 
 
-@GlobalHttpCalls.allowed
 def test_install_pypi(cli):
-    cli.expect_failure("--color install six", "it is not a CLI")
-    assert not os.path.exists(dot_meta("six"))
-
-    cli.expect_failure("install mgit+foo", "not a valid pypi package name")
-
-    runez.touch(dot_meta("mgit/.foo"))  # Should stay because name starts with '.'
-    runez.touch(dot_meta("mgit/mgit-foo"))  # Bogus installation
-    runez.touch(dot_meta("mgit/mgit-0.0.1/foo"))  # Oldest should be deleted
+    runez.touch(dot_meta("mgit-0.0.1/pyenv.cfg"))
+    time.sleep(0.01)  # Ensure 0.0.1 is older than 0.0.2
+    runez.touch(dot_meta("mgit-0.0.2/pyenv.cfg"))
 
     # Simulate the presence of an old entry point
-    manifest_path = dot_meta("mgit/.manifest.json")
+    manifest_path = dot_meta("mgit.manifest.json")
     runez.save_json(dict(entrypoints=["mgit", "old-mgit-entrypoint"]), manifest_path)
     runez.touch("old-mgit-entrypoint")
-    assert os.path.exists("old-mgit-entrypoint")
 
-    time.sleep(0.01)  # Ensure 0.0.1 is older than 0.0.2
-    runez.touch(dot_meta("mgit/mgit-0.0.2/foo"))  # Youngest should remain for an hour
-    check_install_from_pypi(cli, "symlink", "mgit")
+    check_install_from_pypi(cli, "symlink", "mgit", "1.3.0")
     assert not os.path.exists("old-mgit-entrypoint")
     assert os.path.islink("mgit")
-    assert os.path.exists(dot_meta("mgit/.manifest.json"))
-    assert os.path.exists(dot_meta("mgit/.foo"))
-    assert os.path.exists(dot_meta("mgit/mgit-0.0.2"))
-    assert not os.path.exists(dot_meta("mgit/mgit-foo"))
-    assert not os.path.exists(dot_meta("mgit/mgit-0.0.1"))
+    assert os.path.exists(dot_meta("mgit.manifest.json"))
+    assert not os.path.exists(dot_meta("mgit-0.0.1"))
+    assert os.path.exists(dot_meta("mgit-0.0.2"))
+    assert os.path.exists(dot_meta("mgit-1.3.0"))
+
+    cli.run("-n auto-heal")
+    assert cli.succeeded
+    assert "mgit is healthy" in cli.logged
+    assert "Auto-healed 0 / 1 packages" in cli.logged
 
     cfg = PickleyConfig()
     cfg.set_base(".")
-    pspec = PackageSpec(cfg, "mgit")
+    pspec = PackageSpec(cfg, "mgit==1.3.0")
     pspec.groom_installation(keep_for=0)
-    assert not os.path.exists(dot_meta("mgit/mgit-0.0.2"))
+    assert not os.path.exists(dot_meta("mgit-0.0.2"))
+    assert os.path.exists(dot_meta("mgit-1.3.0"))
 
     cli.expect_success("uninstall mgit", "Uninstalled mgit")
     assert not runez.is_executable("mgit")
-    assert not os.path.exists(dot_meta("mgit"))
+    assert not os.path.exists(dot_meta("mgit.manifest.json"))
+    assert not os.path.exists(dot_meta("mgit-1.3.0"))
     assert os.path.exists(dot_meta("audit.log"))
 
-    check_install_from_pypi(cli, "wrap", "mgit", simulate_version="0.0.0")
-    check_is_wrapper("mgit", True)
+    check_install_from_pypi(cli, "wrap", "mgit", "1.3.0", simulate_version="0.0.0")
+    check_is_wrapper("./mgit", True)
+
+    runez.delete(dot_meta("mgit-1.3.0"))
+    cli.run("-n auto-heal")
+    assert cli.succeeded
+    assert "Auto-healed 1 / 1 packages" in cli.logged
+
+
+@GlobalHttpCalls.allowed
+def test_invalid(cli):
+    cli.run("--color install six")
+    assert cli.failed
+    assert "not a CLI" in cli.logged
+    assert not os.path.exists(dot_meta("six.manifest.json"))
+
+    cli.expect_failure("install mgit+foo")
+    assert cli.failed
+    assert "not a valid pypi package name" in cli.logged
 
 
 def test_lock(temp_cfg, logged):
     pspec = PackageSpec(temp_cfg, "foo")
     lock_path = dot_meta("foo.lock")
     with SoftLock(pspec, give_up=600) as lock:
         assert str(lock) == "lock foo"
```

### Comparing `pickley-3.4.5/tests/test_run.py` & `pickley-3.5.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.5/tests/test_venv.py` & `pickley-3.5.1/tests/test_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from unittest.mock import patch
 
 import pytest
 import runez
 
-from pickley import PackageSpec, RawConfig
+from pickley import DOT_META, PackageSpec, RawConfig
 from pickley.package import PackageContents, PythonVenv
 
 
 PIP_SHOW_OUTPUT = """
 Name: ansible
 Version: 1.0.0
 Location: .
@@ -31,22 +31,22 @@
 
     pspec = PackageSpec(temp_cfg, "mgit==1.3.0")
     venv = PythonVenv("venv", pspec, create=False)
     assert not venv.pip_path
     runez.touch("venv/bin/pip3")
     assert venv.pip_path == "venv/bin/pip3"
 
-    runez.touch(".pickley/.cache/virtualenv-20.13.0.pyz")
+    runez.touch(f"{DOT_META}/.cache/virtualenv-20.13.0.pyz")
     with patch("runez.run", return_value=runez.program.RunResult(code=0)):
         cmd = venv._create_virtualenv(runner=lambda *x: x)
         if temp_cfg.available_pythons.invoker.version < "3.7":
             assert cmd[4] == "--pip"
 
         else:
-            assert cmd[4] == "--pip"
+            assert cmd[4] == "--download"
 
 
 def simulated_run(*args, **_):
     if "ansible-core" in args:
         return runez.program.RunResult(PIP_SHOW_OUTPUT, code=0)
 
     if "no-location" in args:
```

