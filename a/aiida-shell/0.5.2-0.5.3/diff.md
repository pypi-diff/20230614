# Comparing `tmp/aiida-shell-0.5.2.tar.gz` & `tmp/aiida_shell-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-shell-0.5.2.tar", last modified: Fri May 12 20:07:03 2023, max compression
+gzip compressed data, was "aiida_shell-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-shell-0.5.2.tar` & `aiida_shell-0.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      230 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/.readthedocs.yml
--rw-r--r--   0        0        0    12194 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/CHANGELOG.md
--rw-r--r--   0        0        0      448 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/CITATION.cff
--rw-r--r--   0        0        0     1076 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0      728 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/README.md
--rw-r--r--   0        0        0      638 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/Makefile
--rw-r--r--   0        0        0     1323 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/source/conf.py
--rw-r--r--   0        0        0    16290 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/source/howto.rst
--rw-r--r--   0        0        0    25440 2023-05-12 20:06:59.037478 aiida-shell-0.5.2/docs/source/images/logo-column.png
--rw-r--r--   0        0        0   164551 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/images/logo-column.svg
--rw-r--r--   0        0        0   167883 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/images/logo-text.svg
--rw-r--r--   0        0        0      429 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/index.rst
--rw-r--r--   0        0        0      590 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/docs/source/installation.rst
--rw-r--r--   0        0        0     3191 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      239 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/__init__.py
--rw-r--r--   0        0        0      127 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/calculations/__init__.py
--rw-r--r--   0        0        0    14339 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/calculations/shell.py
--rw-r--r--   0        0        0      167 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/data/__init__.py
--rw-r--r--   0        0        0     1624 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/data/code.py
--rw-r--r--   0        0        0     5518 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/data/pickled.py
--rw-r--r--   0        0        0      141 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/engine/__init__.py
--rw-r--r--   0        0        0      151 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/engine/launchers/__init__.py
--rw-r--r--   0        0        0     8797 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/engine/launchers/shell_job.py
--rw-r--r--   0        0        0      128 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/parsers/__init__.py
--rw-r--r--   0        0        0     5572 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/parsers/shell.py
--rw-r--r--   0        0        0       26 2023-05-12 20:06:59.041479 aiida-shell-0.5.2/src/aiida_shell/py.typed
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida-shell-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      230 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/.readthedocs.yml
+-rw-r--r--   0        0        0    12395 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/CITATION.cff
+-rw-r--r--   0        0        0     1076 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0      728 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/README.md
+-rw-r--r--   0        0        0      638 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/docs/Makefile
+-rw-r--r--   0        0        0     1323 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/docs/source/conf.py
+-rw-r--r--   0        0        0    19911 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/docs/source/howto.rst
+-rw-r--r--   0        0        0    25440 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/docs/source/images/logo-column.png
+-rw-r--r--   0        0        0   164551 2023-06-14 03:22:17.519949 aiida_shell-0.5.3/docs/source/images/logo-column.svg
+-rw-r--r--   0        0        0   167883 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/docs/source/images/logo-text.svg
+-rw-r--r--   0        0        0      429 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/docs/source/index.rst
+-rw-r--r--   0        0        0      590 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/docs/source/installation.rst
+-rw-r--r--   0        0        0     3191 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/__init__.py
+-rw-r--r--   0        0        0      127 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/calculations/__init__.py
+-rw-r--r--   0        0        0    15608 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/calculations/shell.py
+-rw-r--r--   0        0        0      167 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/data/__init__.py
+-rw-r--r--   0        0        0     1624 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/data/code.py
+-rw-r--r--   0        0        0     5518 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/data/pickled.py
+-rw-r--r--   0        0        0      141 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/engine/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/engine/launchers/__init__.py
+-rw-r--r--   0        0        0     8797 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/engine/launchers/shell_job.py
+-rw-r--r--   0        0        0      128 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/parsers/__init__.py
+-rw-r--r--   0        0        0     5572 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/parsers/shell.py
+-rw-r--r--   0        0        0       26 2023-06-14 03:22:17.523949 aiida_shell-0.5.3/src/aiida_shell/py.typed
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida_shell-0.5.3/PKG-INFO
```

### Comparing `aiida-shell-0.5.2/CHANGELOG.md` & `aiida_shell-0.5.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change log
 
+## `v0.5.3` - 2023-06-13
+
+### Features
+- `ShellJob`: Add support for `FolderData` in `nodes` input [[9587c33]](https://github.com/sphuber/aiida-shell/commit/9587c337cd70b2dadb26a723dfa1ad4691570272)
+
+
 ## `v0.5.2` - 2023-05-12
 
 ### Features
 - `ShellJob`: Add the optional `redirect_stderr` input [[92f726b]](https://github.com/sphuber/aiida-shell/commit/92f726b5fcd631dc4aaa85505869e2dabca9b77c)
 
     A common practice when running shell commands is to redirect the content, written to the stderr file descriptor, to stdout.
     This is normally accomplished as follows:
```

### Comparing `aiida-shell-0.5.2/LICENSE.txt` & `aiida_shell-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/README.md` & `aiida_shell-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/docs/Makefile` & `aiida_shell-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/docs/source/conf.py` & `aiida_shell-0.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/docs/source/howto.rst` & `aiida_shell-0.5.3/docs/source/howto.rst`

 * *Files 16% similar despite different names*

```diff
@@ -110,14 +110,99 @@
 which prints ``string a``.
 Filenames specified in the ``filenames`` input will override the filename of the ``SinglefileData`` nodes.
 Any parent directories in the filepath, for example ``some/nested/path`` in the filename ``some/nested/path/file.txt``, will be automatically created.
 
 The output filename can be anything except for ``stdout``, ``stderr`` and ``status``, which are reserved filenames.
 
 
+Running a shell command with folders as arguments
+=================================================
+
+Certain commands might require the presence of a folder of files in the working directory.
+Just like a file is modeled in AiiDA's provenance graph by a ``SinglefileData`` node, a folder is represented by a ``FolderData`` node.
+The following example shows how a ``FolderData`` can be created to contain multiple files and how it can be passed to ``launch_shell_job`` using the ``nodes`` argument:
+
+.. code-block:: python
+
+    import pathlib
+    import tempfile
+    from aiida.orm import FolderData
+    from aiida_shell import launch_shell_job
+
+    # First create a ``FolderData`` node with some arbitrary files
+    with tempfile.TemporaryDirectory() as tmpdir:
+        dirpath = pathlib.Path(tmpdir)
+        (dirpath / 'file_a.txt').write_text('content a')
+        (dirpath / 'file_b.txt').write_text('content b')
+        folder_data = FolderData(tree=dirpath.absolute())
+
+    results, node = launch_shell_job(
+        'ls',
+        nodes={
+            'directory': folder_data,
+        }
+    )
+    print(results['stdout'].get_content())
+
+which prints:
+
+.. code-block:: console
+
+    _aiidasubmit.sh
+    file_a.txt
+    file_b.txt
+    _scheduler-stderr.txt
+    _scheduler-stdout.txt
+    stderr
+    stdout
+
+The contents of the ``folder_data`` node, the ``file_a.txt`` and ``file_b.txt`` files, were copied to the working directory.
+
+Note that by default, the contents of the ``FolderData`` are copied to the root of the working directory, as shown in the example above.
+If the contents should be written to a directory inside the working directory, use the ``filenames`` argument, as is done for copying ``SinglefileData`` nodes.
+Take for example the ``zip`` command that can create a zip archive from one or many files and folders.
+
+.. code-block:: python
+
+    import pathlib
+    import tempfile
+    from aiida.orm import FolderData
+    from aiida_shell import launch_shell_job
+
+    # First create a ``FolderData`` node with some arbitrary files
+    with tempfile.TemporaryDirectory() as tmpdir:
+        dirpath = pathlib.Path(tmpdir)
+        (dirpath / 'file_a.txt').write_text('content a')
+        (dirpath / 'file_b.txt').write_text('content b')
+        folder_data = FolderData(tree=dirpath.absolute())
+
+    results, node = launch_shell_job(
+        'zip',
+        arguments='-r archive.zip {folder}',
+        outputs=['archive.zip'],
+        nodes={
+            'folder': folder_data,
+        },
+        filenames={
+            'folder': 'directory'
+        }
+    )
+
+In this example, the contents of the ``folder_data`` node were copied to the ``directory`` folder in the working directory.
+The ``results`` dictionary contains the ``archive_zip`` output which is a ``SinglefileData`` node containing the zip archive.
+It can be unzipped as follows: ``verdi node repo cat <IDENTIFIER> | unzip``, where ``<IDENTIFIER>`` should be replaced with the pk or UUID of the ``archive_zip`` node.
+The original files ``file_a.txt`` and ``file_b.txt`` are now written to the current working directory.
+
+.. note::
+
+    It is not required for a ``FolderData`` node, that is specified in the ``nodes`` input, to have a corresponding placeholder in the ``arguments``.
+    Just as with ``SinglefileData`` inputs nodes, if there is no corresponding placeholder, the contents of the folder are simply written to the working directory where the shell command is executed.
+    This is useful for commands that expect a folder to be present in the working directory but whose name is not explicitly defined through a command line argument.
+
+
 Passing other ``Data`` types as input
 =====================================
 
 The ``nodes`` keyword does not only accept ``SinglefileData`` nodes, but it accepts also other ``Data`` types.
 For these node types, the content returned by the ``value`` property is directly cast to ``str``, which is used to replace the corresponding placeholder in the ``arguments``.
 So as long as the ``Data`` type implements this ``value`` property it should be supported.
 Of course, whether it makes sense for the value of the node to be used directly as a command line argument for the shell job, is up to the user.
```

### Comparing `aiida-shell-0.5.2/docs/source/images/logo-column.png` & `aiida_shell-0.5.3/docs/source/images/logo-column.png`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/docs/source/images/logo-column.svg` & `aiida_shell-0.5.3/docs/source/images/logo-column.svg`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/docs/source/images/logo-text.svg` & `aiida_shell-0.5.3/docs/source/images/logo-text.svg`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/docs/source/installation.rst` & `aiida_shell-0.5.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/pyproject.toml` & `aiida_shell-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/src/aiida_shell/calculations/shell.py` & `aiida_shell-0.5.3/src/aiida_shell/calculations/shell.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import inspect
 import pathlib
 import typing as t
 
 from aiida.common.datastructures import CalcInfo, CodeInfo
 from aiida.common.folders import Folder
 from aiida.engine import CalcJob, CalcJobProcessSpec
-from aiida.orm import Data, Dict, List, SinglefileData, to_aiida_type
+from aiida.orm import Data, Dict, FolderData, List, SinglefileData, to_aiida_type
 
 from aiida_shell.data import PickledData
 
 __all__ = ('ShellJob',)
 
 
 class ShellJob(CalcJob):
@@ -129,15 +129,15 @@
             return f'The `parser` has an invalid function signature, it should be: {correct_signature}'
 
     @classmethod
     def validate_nodes(cls, value: t.Mapping[str, Data], _) -> str | None:
         """Validate the ``nodes`` input."""
         for key, node in value.items():
 
-            if isinstance(node, SinglefileData):
+            if isinstance(node, (FolderData, SinglefileData)):
                 continue
 
             try:
                 str(node.value)
             except AttributeError:
                 cls_name = node.__class__.__name__
                 return f'Unsupported node type for `{key}` in `nodes`: {cls_name} does not have the `value` property.'
@@ -285,23 +285,31 @@
                 raise ValueError(f'argument placeholder `{{{placeholder}}}` not specified in `nodes`.')
 
             node = nodes[placeholder]
 
             if isinstance(node, SinglefileData):
                 filename = self.write_single_file_data(dirpath, node, placeholder, filenames)
                 argument_interpolated = argument.format(**{placeholder: filename})
+            elif isinstance(node, FolderData):
+                filename = self.write_folder_data(dirpath, node, placeholder, filenames)
+                argument_interpolated = argument.format(**{placeholder: filename})
             else:
                 argument_interpolated = argument.format(**{placeholder: str(node.value)})
 
             processed_nodes.append(placeholder)
             processed_arguments.append(argument_interpolated)
 
         for key, node in nodes.items():
-            if key not in processed_nodes and isinstance(node, SinglefileData):
+            if key in processed_nodes:
+                continue
+
+            if isinstance(node, SinglefileData):
                 self.write_single_file_data(dirpath, node, key, filenames)
+            elif isinstance(node, FolderData):
+                self.write_folder_data(dirpath, node, key, filenames)
 
         return processed_arguments
 
     @staticmethod
     def write_single_file_data(dirpath: pathlib.Path, node: SinglefileData, key: str, filenames: dict[str, str]) -> str:
         """Write the content of a ``SinglefileData`` node to ``dirpath``.
 
@@ -317,7 +325,29 @@
 
         filepath.parent.mkdir(parents=True, exist_ok=True)
 
         with node.open(mode='rb') as handle:
             filepath.write_bytes(handle.read())
 
         return filename
+
+    @staticmethod
+    def write_folder_data(dirpath: pathlib.Path, node: FolderData, key: str, filenames: dict[str, str]) -> str:
+        """Write the content of a ``FolderData`` node to ``dirpath``.
+
+        :param dirpath: A temporary folder on the local file system.
+        :param node: The node whose content to write.
+        :param key: The relative filename to use.
+        :param filenames: Mapping that can provide explicit filenames for the given key.
+        :returns: The relative filename used to write the content to ``dirpath``.
+        """
+        if key in filenames:
+            filename = filenames[key]
+            filepath = dirpath / filename
+        else:
+            filename = key
+            filepath = dirpath
+
+        filepath.parent.mkdir(parents=True, exist_ok=True)
+        node.base.repository.copy_tree(filepath)
+
+        return filename
```

### Comparing `aiida-shell-0.5.2/src/aiida_shell/data/code.py` & `aiida_shell-0.5.3/src/aiida_shell/data/code.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/src/aiida_shell/data/pickled.py` & `aiida_shell-0.5.3/src/aiida_shell/data/pickled.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/src/aiida_shell/engine/launchers/shell_job.py` & `aiida_shell-0.5.3/src/aiida_shell/engine/launchers/shell_job.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/src/aiida_shell/parsers/shell.py` & `aiida_shell-0.5.3/src/aiida_shell/parsers/shell.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.2/PKG-INFO` & `aiida_shell-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-shell
-Version: 0.5.2
+Version: 0.5.3
 Summary: AiiDA plugin that makes running shell commands easy.
 Keywords: aiida,workflows
 Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
```

