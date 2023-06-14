# Comparing `tmp/b-bugtracker-3.0.0.tar.gz` & `tmp/b-bugtracker-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b-bugtracker-3.0.0.tar", max compression
+gzip compressed data, was "b-bugtracker-3.0.1.tar", max compression
```

## Comparing `b-bugtracker-3.0.0.tar` & `b-bugtracker-3.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1752 2023-05-20 21:25:22.942452 b-bugtracker-3.0.0/b/__init__.py
--rw-r--r--   0        0        0     1234 2023-05-21 02:43:30.317947 b-bugtracker-3.0.0/b/__main__.py
--rw-r--r--   0        0        0    24147 2023-06-14 16:55:55.282431 b-bugtracker-3.0.0/b/bugs.py
--rw-r--r--   0        0        0    15295 2023-06-14 16:49:39.289207 b-bugtracker-3.0.0/b/command.py
--rw-r--r--   0        0        0     4738 2023-05-24 17:10:10.826160 b-bugtracker-3.0.0/b/exceptions.py
--rw-r--r--   0        0        0     8310 2023-05-26 17:45:17.747675 b-bugtracker-3.0.0/b/migrations.py
--rw-r--r--   0        0        0     7030 2023-06-14 16:55:34.418080 b-bugtracker-3.0.0/b/schema/bug.schema.json
--rw-r--r--   0        0        0     4930 2023-05-21 15:11:16.833427 b-bugtracker-3.0.0/b/settings.py
--rw-r--r--   0        0        0      612 2023-05-26 02:37:36.943854 b-bugtracker-3.0.0/b/templates/bug.bug.yaml
--rw-r--r--   0        0        0      396 2023-05-26 02:38:44.471125 b-bugtracker-3.0.0/b/templates/feature.bug.yaml
--rw-r--r--   0        0        0      759 2023-05-20 21:29:21.218897 b-bugtracker-3.0.0/LICENSE
--rw-r--r--   0        0        0      753 2023-06-14 19:43:28.283492 b-bugtracker-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3777 2023-06-14 19:38:54.138195 b-bugtracker-3.0.0/README.md
--rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 b-bugtracker-3.0.0/setup.py
--rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 b-bugtracker-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1752 2023-05-20 21:25:22.942452 b-bugtracker-3.0.1/b/__init__.py
+-rw-r--r--   0        0        0     1234 2023-05-21 02:43:30.317947 b-bugtracker-3.0.1/b/__main__.py
+-rw-r--r--   0        0        0    24147 2023-06-14 16:55:55.282431 b-bugtracker-3.0.1/b/bugs.py
+-rw-r--r--   0        0        0    15324 2023-06-14 19:48:47.225845 b-bugtracker-3.0.1/b/command.py
+-rw-r--r--   0        0        0     4738 2023-05-24 17:10:10.826160 b-bugtracker-3.0.1/b/exceptions.py
+-rw-r--r--   0        0        0     8310 2023-05-26 17:45:17.747675 b-bugtracker-3.0.1/b/migrations.py
+-rw-r--r--   0        0        0     7030 2023-06-14 16:55:34.418080 b-bugtracker-3.0.1/b/schema/bug.schema.json
+-rw-r--r--   0        0        0     4930 2023-05-21 15:11:16.833427 b-bugtracker-3.0.1/b/settings.py
+-rw-r--r--   0        0        0      612 2023-05-26 02:37:36.943854 b-bugtracker-3.0.1/b/templates/bug.bug.yaml
+-rw-r--r--   0        0        0      396 2023-05-26 02:38:44.471125 b-bugtracker-3.0.1/b/templates/feature.bug.yaml
+-rw-r--r--   0        0        0      759 2023-05-20 21:29:21.218897 b-bugtracker-3.0.1/LICENSE
+-rw-r--r--   0        0        0      753 2023-06-14 19:49:41.277331 b-bugtracker-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3777 2023-06-14 19:38:54.138195 b-bugtracker-3.0.1/README.md
+-rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 b-bugtracker-3.0.1/setup.py
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 b-bugtracker-3.0.1/PKG-INFO
```

### Comparing `b-bugtracker-3.0.0/b/__init__.py` & `b-bugtracker-3.0.1/b/__init__.py`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/__main__.py` & `b-bugtracker-3.0.1/b/__main__.py`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/bugs.py` & `b-bugtracker-3.0.1/b/bugs.py`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/command.py` & `b-bugtracker-3.0.1/b/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,16 +67,17 @@
 
 
 
 # ======================================================================================================================
 # Command Line Processing
 # ----------------------------------------------------------------------------------------------------------------------
 def run():
-    description = metadata.metadata('b')['Summary']
-    version = metadata.version('b')
+    name = 'b-bugtracker'
+    description = metadata.metadata(name)['Summary']
+    version = metadata.version(name)
     parser = ArgumentParser(description=description, formatter_class=RichHelpFormatter)
 
     parser.add_argument(
         '-v',
         '--verbose',
         action='count',
         default=0,
```

### Comparing `b-bugtracker-3.0.0/b/exceptions.py` & `b-bugtracker-3.0.1/b/exceptions.py`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/migrations.py` & `b-bugtracker-3.0.1/b/migrations.py`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/schema/bug.schema.json` & `b-bugtracker-3.0.1/b/schema/bug.schema.json`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/settings.py` & `b-bugtracker-3.0.1/b/settings.py`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/b/templates/bug.bug.yaml` & `b-bugtracker-3.0.1/b/templates/bug.bug.yaml`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/LICENSE` & `b-bugtracker-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/pyproject.toml` & `b-bugtracker-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "b-bugtracker"
-version = "3.0.0"
+version = "3.0.1"
 description = "A simple, distributed bug tracker."
 repository = "https://github.com/jwjulien/b"
 homepage = "https://jwjulien.github.io/b"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 authors = [
     "Michael Diamond <michael@digitalgemstones.com>",
```

### Comparing `b-bugtracker-3.0.0/README.md` & `b-bugtracker-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `b-bugtracker-3.0.0/setup.py` & `b-bugtracker-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'rich>=13.3.5,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['b = b.command:run']}
 
 setup_kwargs = {
     'name': 'b-bugtracker',
-    'version': '3.0.0',
+    'version': '3.0.1',
     'description': 'A simple, distributed bug tracker.',
     'long_description': "b, A distributed bug tracker\n========================================================================================================================\nThis version of `b` was forked from [foss.heptapod.net](https://foss.heptapod.net/mercurial/b).  Originally with only minor modifications, but now it's likely safer to say that this tool simply took inspiration from B.\n\nSo, with that stated, full credit for the inspiration for this tool goes to Michael Diamond.  Thank you for taking the time and investing the effort to create `b`, without which this tool I love wouldn't likely exist.\n\nThe original purpose of B was to serve as a low-feature stand-in for a real, convoluted bug tracking system.  I loved that concept, but have taken the tool much further; much beyond the original, modest scope to the point of adding many features and capabilities to rival those of a fully fledged bug tracking system, but still in a distributed package.\n\n- Now a standalone command-line tool with no dependency upon Mercurial allowing it to be used with any VCS.\n    - See the available [commands](https://jwjulien.github.io/b/commands/index) for more info.\n- Supports Rich output to make interacting a bit more friendly.\n- Supports bug templates to offer a better starting point for new bugs.\n    - Also supports customization at the project level - see [templates](https://jwjulien.github.io/b/commands/templates) for more info.\n- Handles it's own configuration, outside of Mercurial, in support of independence.\n    - See [config command](https://jwjulien.github.io/b/commands/config) for more info about the available configuration options and config file location.\n\nSee the [installation](https://jwjulien.github.io/b/installation) and [getting started](https://jwjulien.github.io/b/getting_started) guides for help with installing and using `b` on your project.\n\n\n\n\nIntroduction\n------------------------------------------------------------------------------------------------------------------------\n`b` is a tool for tracking bugs and open issues that works with any distributed version control system.  Bugs are tracked as YAML files (i.e., nearly plain text) directly in the `.bugs` directory of the project.  That means that when a user adds a new bug they will need to add it into the VCS and commit it.  Then, all changes made to the bug during the process of diagnosis and resolution will be tracked.\n\nThe use of YAML files means that bugs can be opened directly in an editor and manually edited.  In fact, `b` itself does not the ability to set many of the attributes in the bug files from the command line.  It is expected that users will manually open bugs (optionally using the `edit` command) and edit their contents directly.  For more info about the format of these YAML files and the supporting schema, have a look at [the bug file format](https://jwjulien.github.io/b/bugs).\n\n\n\n\nSome Suggested Use Cases\n------------------------------------------------------------------------------------------------------------------------\nSmall scripts and tasks deserve version control, even if they're never going to be distributed elsewhere.  This is easy with Mercurial.  With `b` installed you get a fully functional bug tracker along with your VCS, no additional setup required! As soon as you install `b`, every repository on your machine now has issue tracking functionality ready to use.\n\nWorking on a project with a few other team members is ideal for `b`, it's powerful enough to let everyone track what they need to do, and allow everyone to contribute what they can to any of the bugs on file.  They can search titles for matching bugs, and even grep through the details directory to find details matching what they're looking for.\n",
     'author': 'Michael Diamond',
     'author_email': 'michael@digitalgemstones.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://jwjulien.github.io/b',
```

### Comparing `b-bugtracker-3.0.0/PKG-INFO` & `b-bugtracker-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-bugtracker
-Version: 3.0.0
+Version: 3.0.1
 Summary: A simple, distributed bug tracker.
 Home-page: https://jwjulien.github.io/b
 License: GPL-3.0-or-later
 Author: Michael Diamond
 Author-email: michael@digitalgemstones.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

