# Comparing `tmp/pipdeptree-2.9.0.tar.gz` & `tmp/pipdeptree-2.9.1.tar.gz`

## Comparing `pipdeptree-2.9.0.tar` & `pipdeptree-2.9.1.tar`

### file list

```diff
@@ -1,22 +1,18 @@
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.prettierrc.toml
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/CHANGES.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/tox.ini
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/whitelist.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/workflows/check.yml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.github/workflows/release.yml
--rw-r--r--   0        0        0    97568 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/docs/twine-pdt.png
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/docs/v2beta-opts.org
--rw-r--r--   0        0        0    37997 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/src/pipdeptree/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/src/pipdeptree/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/src/pipdeptree/version.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/tests/guess_version_setuptools.py
--rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/tests/test_pipdeptree.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/LICENSE
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/README.md
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/pyproject.toml
--rw-r--r--   0        0        0    15544 2020-02-02 00:00:00.000000 pipdeptree-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/CHANGES.md
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/tox.ini
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    38762 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/src/pipdeptree/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/src/pipdeptree/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/src/pipdeptree/version.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/tests/guess_version_setuptools.py
+-rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/tests/test_pipdeptree.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/LICENSE
+-rw-r--r--   0        0        0    12705 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/README.md
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 pipdeptree-2.9.1/PKG-INFO
```

### Comparing `pipdeptree-2.9.0/CHANGES.md` & `pipdeptree-2.9.1/CHANGES.md`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.0/tox.ini` & `pipdeptree-2.9.1/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       tests}
     diff-cover --compare-branch {env:DIFF_AGAINST:origin/main} {toxworkdir}{/}coverage.{envname}.xml
 
 [testenv:fix]
 description = format the code base to adhere to our styles, and complain about what we cannot do automatically
 skip_install = true
 deps =
-    pre-commit>=3.2.2
+    pre-commit>=3.3.2
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:readme]
 description = check that the long description is valid
 base_python = python3.10
 skip_install = true
```

### Comparing `pipdeptree-2.9.0/.github/workflows/check.yml` & `pipdeptree-2.9.1/.github/workflows/check.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 concurrency:
   group: check-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   test:
     name: test ${{ matrix.py }}
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         py:
-          - "3.12.0-beta.1"
+          - "3.12.0-beta.2"
           - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
     steps:
       - name: Install OS dependencies
@@ -79,15 +79,15 @@
         run: python -m tox -e ${{ matrix.tox_env }}
         env:
           UPGRADE_ADVISORY: "yes"
 
   publish:
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     needs: [check, test]
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     steps:
       - name: setup python to build package
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - name: install build
         run: python -m pip install build
```

### Comparing `pipdeptree-2.9.0/.github/workflows/release.yml` & `pipdeptree-2.9.1/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Release to PyPI
 on:
   push:
     tags: ["*"]
 
 jobs:
   release:
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     environment:
       name: release
       url: https://pypi.org/p/pipdeptree
     permissions:
       id-token: write
     steps:
       - name: Setup python to build package
```

### Comparing `pipdeptree-2.9.0/src/pipdeptree/__init__.py` & `pipdeptree-2.9.1/src/pipdeptree/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from __future__ import annotations
+
 import argparse
 import fnmatch
 import inspect
 import json
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
 from collections import defaultdict, deque
 from collections.abc import Mapping
 from importlib import import_module
 from itertools import chain
+from pathlib import Path
 from textwrap import dedent
 
 from pip._vendor import pkg_resources
 
 from .version import version as __version__
 
 try:
@@ -32,15 +35,16 @@
     :returns: sorted tree
     :rtype: dict
     """
     return {k: sorted(v) for k, v in sorted(tree.items())}
 
 
 def guess_version(pkg_key, default="?"):
-    """Guess the version of a pkg when pip doesn't provide it
+    """
+    Guess the version of a pkg when pip doesn't provide it.
 
     :param str pkg_key: key of the package
     :param str default: default version to return if unable to find
     :returns: version
     :rtype: string
     """
     try:
@@ -58,16 +62,15 @@
         m = import_module(pkg_key)
     except ImportError:
         return default
     else:
         v = getattr(m, "__version__", default)
         if inspect.ismodule(v):
             return getattr(v, "__version__", default)
-        else:
-            return v
+        return v
 
 
 def frozen_req_from_dist(dist):
     # The `pip._internal.metadata` modules were introduced in 21.1.1
     # and the `pip._internal.operations.freeze.FrozenRequirement`
     # class now expects dist to be a subclass of
     # `pip._internal.metadata.BaseDistribution`, however the
@@ -92,79 +95,76 @@
 
 class Package:
     """
     Abstract class for wrappers around objects that pip returns. This class needs to be subclassed with implementations
     for `render_as_root` and `render_as_branch` methods.
     """
 
-    def __init__(self, obj):
+    def __init__(self, obj) -> None:
         self._obj = obj
         self.project_name = obj.project_name
         self.key = obj.key
 
-    def render_as_root(self, frozen):  # noqa: U100
+    def render_as_root(self, frozen):  # noqa: ARG002
         return NotImplementedError
 
-    def render_as_branch(self, frozen):  # noqa: U100
+    def render_as_branch(self, frozen):  # noqa: ARG002
         return NotImplementedError
 
-    def render(self, parent=None, frozen=False):
+    def render(self, parent=None, frozen=False):  # noqa: FBT002
         if not parent:
             return self.render_as_root(frozen)
-        else:
-            return self.render_as_branch(frozen)
+        return self.render_as_branch(frozen)
 
     @staticmethod
     def frozen_repr(obj):
         fr = frozen_req_from_dist(obj)
         return str(fr).strip()
 
     def __getattr__(self, key):
         return getattr(self._obj, key)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<{self.__class__.__name__}("{self.key}")>'
 
     def __lt__(self, rhs):
         return self.key < rhs.key
 
 
 class DistPackage(Package):
     """
-    Wrapper class for pkg_resources.Distribution instances
+    Wrapper class for pkg_resources.Distribution instances.
 
     :param obj: pkg_resources.Distribution to wrap over
     :param req: optional ReqPackage object to associate this DistPackage with. This is useful for displaying the tree
         in reverse
     """
 
-    def __init__(self, obj, req=None):
+    def __init__(self, obj, req=None) -> None:
         super().__init__(obj)
         self.version_spec = None
         self.req = req
 
     def render_as_root(self, frozen):
         if not frozen:
             return f"{self.project_name}=={self.version}"
-        else:
-            return self.__class__.frozen_repr(self._obj)
+        return self.__class__.frozen_repr(self._obj)
 
     def render_as_branch(self, frozen):
-        assert self.req is not None
+        assert self.req is not None  # noqa: S101
         if not frozen:
             parent_ver_spec = self.req.version_spec
             parent_str = self.req.project_name
             if parent_ver_spec:
                 parent_str += parent_ver_spec
             return f"{self.project_name}=={self.version} [requires: {parent_str}]"
-        else:
-            return self.render_as_root(frozen)
+        return self.render_as_root(frozen)
 
     def as_requirement(self):
-        """Return a ReqPackage representation of this DistPackage"""
+        """Return a ReqPackage representation of this DistPackage."""
         return ReqPackage(self._obj.as_requirement(), dist=self)
 
     def as_parent_of(self, req):
         """
         Return a DistPackage instance associated to a requirement. This association is necessary for reversing the
         PackageDAG.
 
@@ -180,23 +180,23 @@
 
     def as_dict(self):
         return {"key": self.key, "package_name": self.project_name, "installed_version": self.version}
 
 
 class ReqPackage(Package):
     """
-    Wrapper class for Requirements instance
+    Wrapper class for Requirements instance.
 
     :param obj: The `Requirements` instance to wrap over
     :param dist: optional `pkg_resources.Distribution` instance for this requirement
     """
 
     UNKNOWN_VERSION = "?"
 
-    def __init__(self, obj, dist=None):
+    def __init__(self, obj, dist=None) -> None:
         super().__init__(obj)
         self.dist = dist
 
     @property
     def version_spec(self):
         specs = sorted(self._obj.specs, reverse=True)  # `reverse` makes '>' prior to '<'
         return ",".join(["".join(sp) for sp in specs]) if specs else None
@@ -208,37 +208,35 @@
         return self.dist.version
 
     @property
     def is_missing(self):
         return self.installed_version == self.UNKNOWN_VERSION
 
     def is_conflicting(self):
-        """If installed version conflicts with required version"""
+        """If installed version conflicts with required version."""
         # unknown installed version is also considered conflicting
         if self.installed_version == self.UNKNOWN_VERSION:
             return True
         ver_spec = self.version_spec if self.version_spec else ""
         req_version_str = f"{self.project_name}{ver_spec}"
         req_obj = pkg_resources.Requirement.parse(req_version_str)
         return self.installed_version not in req_obj
 
     def render_as_root(self, frozen):
         if not frozen:
             return f"{self.project_name}=={self.installed_version}"
-        elif self.dist:
-            return self.__class__.frozen_repr(self.dist._obj)
-        else:
-            return self.project_name
+        if self.dist:
+            return self.__class__.frozen_repr(self.dist._obj)  # noqa: SLF001
+        return self.project_name
 
     def render_as_branch(self, frozen):
         if not frozen:
             req_ver = self.version_spec if self.version_spec else "Any"
             return f"{self.project_name} [required: {req_ver}, installed: {self.installed_version}]"
-        else:
-            return self.render_as_root(frozen)
+        return self.render_as_root(frozen)
 
     def as_dict(self):
         return {
             "key": self.key,
             "package_name": self.project_name,
             "installed_version": self.installed_version,
             "required_version": self.version_spec,
@@ -271,16 +269,17 @@
     @classmethod
     def from_pkgs(cls, pkgs):
         pkgs = [DistPackage(p) for p in pkgs]
         idx = {p.key: p for p in pkgs}
         m = {p: [ReqPackage(r, idx.get(r.key)) for r in p.requires()] for p in pkgs}
         return cls(m)
 
-    def __init__(self, m):
-        """Initialize the PackageDAG object
+    def __init__(self, m) -> None:
+        """
+        Initialize the PackageDAG object.
 
         :param dict m: dict of node objects (refer class docstring)
         :returns: None
         :rtype: NoneType
 
         """
         self._obj = m
@@ -300,26 +299,26 @@
         try:
             return self._index[node_key]
         except KeyError:
             return None
 
     def get_children(self, node_key):
         """
-        Get child nodes for a node by its key
+        Get child nodes for a node by its key.
 
         :param str node_key: key of the node to get children of
         :returns: list of child nodes
         :rtype: ReqPackage[]
         """
         node = self.get_node_as_parent(node_key)
         return self._obj[node] if node else []
 
-    def filter(self, include, exclude):
+    def filter_nodes(self, include, exclude):  # noqa: C901, PLR0912
         """
-        Filters nodes in a graph by given parameters
+        Filters nodes in a graph by given parameters.
 
         If a node is included, then all it's children are also included.
 
         :param set include: set of node keys to include (or None)
         :param set exclude: set of node keys to exclude (or None)
         :returns: filtered version of the graph
         :rtype: PackageDAG
@@ -331,30 +330,27 @@
         # Note: In following comparisons, we use lower cased values so
         # that user may specify `key` or `project_name`. As per the
         # documentation, `key` is simply
         # `project_name.lower()`. Refer:
         # https://setuptools.readthedocs.io/en/latest/pkg_resources.html#distribution-objects
         if include:
             include = {s.lower() for s in include}
-        if exclude:
-            exclude = {s.lower() for s in exclude}
-        else:
-            exclude = set()
+        exclude = {s.lower() for s in exclude} if exclude else set()
 
         # Check for mutual exclusion of show_only and exclude sets
         # after normalizing the values to lowercase
         if include and exclude:
-            assert not (include & exclude)
+            assert not (include & exclude)  # noqa: S101
 
         # Traverse the graph in a depth first manner and filter the
         # nodes according to `show_only` and `exclude` sets
         stack = deque()
         m = {}
         seen = set()
-        for node in self._obj.keys():
+        for node in self._obj:
             if any(fnmatch.fnmatch(node.key, e) for e in exclude):
                 continue
             if include is None or any(fnmatch.fnmatch(node.key, i) for i in include):
                 stack.append(node)
             while True:
                 if len(stack) > 0:
                     n = stack.pop()
@@ -394,15 +390,15 @@
         child_keys = {r.key for r in chain.from_iterable(self._obj.values())}
         for k, vs in self._obj.items():
             for v in vs:
                 # if v is already added to the dict, then ensure that
                 # we are using the same object. This check is required
                 # as we're using array mutation
                 try:
-                    node = [p for p in m.keys() if p.key == v.key][0]
+                    node = [p for p in m if p.key == v.key][0]
                 except IndexError:
                     node = v
                 m[node].append(k.as_parent_of(v))
             if k.key not in child_keys:
                 m[k.as_requirement()] = []
         return ReversedPackageDAG(dict(m))
 
@@ -417,50 +413,52 @@
     # Methods required by the abstract base class Mapping
     def __getitem__(self, *args):
         return self._obj.get(*args)
 
     def __iter__(self):
         return self._obj.__iter__()
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._obj)
 
 
 class ReversedPackageDAG(PackageDAG):
-    """Representation of Package dependencies in the reverse order.
+    """
+    Representation of Package dependencies in the reverse order.
 
     Similar to it's super class `PackageDAG`, the underlying datastructure is a dict, but here the keys are expected to
     be of type `ReqPackage` and each item in the values of type `DistPackage`.
 
     Typically, this object will be obtained by calling `PackageDAG.reverse`.
     """
 
     def reverse(self):
         """
-        Reverse the already reversed DAG to get the PackageDAG again
+        Reverse the already reversed DAG to get the PackageDAG again.
 
         :returns: reverse of the reversed DAG
         :rtype: PackageDAG
         """
         m = defaultdict(list)
         child_keys = {r.key for r in chain.from_iterable(self._obj.values())}
         for k, vs in self._obj.items():
             for v in vs:
                 try:
-                    node = [p for p in m.keys() if p.key == v.key][0]
+                    node = [p for p in m if p.key == v.key][0]
                 except IndexError:
                     node = v.as_parent_of(None)
                 m[node].append(k)
             if k.key not in child_keys:
                 m[k.dist] = []
         return PackageDAG(dict(m))
 
 
-def render_text(tree, max_depth, list_all=True, frozen=False):
-    """Print tree as text on console
+def render_text(tree, max_depth, list_all=True, frozen=False):  # noqa: FBT002
+    """
+    Print tree as text on console.
 
     :param dict tree: the package tree
     :param bool list_all: whether to list all the pgks at the root level or only those that are the sub-dependencies
     :param bool frozen: show the names of the pkgs in the output that's favourable to pip --freeze
     :returns: None
     """
     tree = tree.sort()
@@ -475,24 +473,24 @@
     else:
         _render_text_without_unicode(tree, nodes, max_depth, frozen)
 
 
 def _render_text_with_unicode(tree, nodes, max_depth, frozen):
     use_bullets = not frozen
 
-    def aux(
+    def aux(  # noqa: PLR0913
         node,
         parent=None,
         indent=0,
         cur_chain=None,
         prefix="",
         depth=0,
-        has_grand_parent=False,
-        is_last_child=False,
-        parent_is_last_child=False,
+        has_grand_parent=False,  # noqa: FBT002
+        is_last_child=False,  # noqa: FBT002
+        parent_is_last_child=False,  # noqa: FBT002
     ):
         cur_chain = cur_chain or []
         node_str = node.render(parent, frozen)
         next_prefix = ""
         next_indent = indent + 2
 
         if parent:
@@ -521,52 +519,52 @@
 
         children = tree.get_children(node.key)
         children_strings = [
             aux(
                 c,
                 node,
                 indent=next_indent,
-                cur_chain=cur_chain + [c.project_name],
+                cur_chain=[*cur_chain, c.project_name],
                 prefix=next_prefix,
                 depth=depth + 1,
                 has_grand_parent=parent is not None,
                 is_last_child=c is children[-1],
                 parent_is_last_child=is_last_child,
             )
             for c in children
             if c.project_name not in cur_chain and depth + 1 <= max_depth
         ]
 
         result += list(chain.from_iterable(children_strings))
         return result
 
     lines = chain.from_iterable([aux(p) for p in nodes])
-    print("\n".join(lines))
+    print("\n".join(lines))  # noqa: T201
 
 
 def _render_text_without_unicode(tree, nodes, max_depth, frozen):
     use_bullets = not frozen
 
     def aux(node, parent=None, indent=0, cur_chain=None, depth=0):
         cur_chain = cur_chain or []
         node_str = node.render(parent, frozen)
         if parent:
             prefix = " " * indent + ("- " if use_bullets else "")
             node_str = prefix + node_str
         result = [node_str]
         children = [
-            aux(c, node, indent=indent + 2, cur_chain=cur_chain + [c.project_name], depth=depth + 1)
+            aux(c, node, indent=indent + 2, cur_chain=[*cur_chain, c.project_name], depth=depth + 1)
             for c in tree.get_children(node.key)
             if c.project_name not in cur_chain and depth + 1 <= max_depth
         ]
         result += list(chain.from_iterable(children))
         return result
 
     lines = chain.from_iterable([aux(p) for p in nodes])
-    print("\n".join(lines))
+    print("\n".join(lines))  # noqa: T201
 
 
 def render_json(tree, indent):
     """
     Converts the tree into a flat json representation.
 
     The json repr will be a list of hashes, each hash having 2 fields:
@@ -576,15 +574,16 @@
     :param dict tree: dependency tree
     :param int indent: no. of spaces to indent json
     :returns: json representation of the tree
     :rtype: str
     """
     tree = tree.sort()
     return json.dumps(
-        [{"package": k.as_dict(), "dependencies": [v.as_dict() for v in vs]} for k, vs in tree.items()], indent=indent
+        [{"package": k.as_dict(), "dependencies": [v.as_dict() for v in vs]} for k, vs in tree.items()],
+        indent=indent,
     )
 
 
 def render_json_tree(tree, indent):
     """
     Converts the tree into a nested json representation.
 
@@ -599,39 +598,40 @@
     :param dict tree: dependency tree
     :param int indent: no. of spaces to indent json
     :returns: json representation of the tree
     :rtype: str
     """
     tree = tree.sort()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
-    nodes = [p for p in tree.keys() if p.key not in branch_keys]
+    nodes = [p for p in tree if p.key not in branch_keys]
 
     def aux(node, parent=None, cur_chain=None):
         if cur_chain is None:
             cur_chain = [node.project_name]
 
         d = node.as_dict()
         if parent:
             d["required_version"] = node.version_spec if node.version_spec else "Any"
         else:
             d["required_version"] = d["installed_version"]
 
         d["dependencies"] = [
-            aux(c, parent=node, cur_chain=cur_chain + [c.project_name])
+            aux(c, parent=node, cur_chain=[*cur_chain, c.project_name])
             for c in tree.get_children(node.key)
             if c.project_name not in cur_chain
         ]
 
         return d
 
     return json.dumps([aux(p) for p in nodes], indent=indent)
 
 
-def render_mermaid(tree) -> str:
-    """Produce a Mermaid flowchart from the dependency graph.
+def render_mermaid(tree) -> str:  # noqa: C901
+    """
+    Produce a Mermaid flowchart from the dependency graph.
 
     :param dict tree: dependency graph
     """
     # List of reserved keywords in Mermaid that cannot be used as node names.
     # See: https://github.com/mermaid-js/mermaid/issues/4182#issuecomment-1454787806
     reserved_ids: set[str] = {
         "C4Component",
@@ -679,25 +679,25 @@
     # Use a sets to avoid duplicate entries.
     nodes: set[str] = set()
     edges: set[str] = set()
 
     if isinstance(tree, ReversedPackageDAG):
         for package, reverse_dependencies in tree.items():
             package_label = "\\n".join(
-                (package.project_name, "(missing)" if package.is_missing else package.installed_version)
+                (package.project_name, "(missing)" if package.is_missing else package.installed_version),
             )
             package_key = mermaid_id(package.key)
             nodes.add(f'{package_key}["{package_label}"]')
             for reverse_dependency in reverse_dependencies:
                 edge_label = reverse_dependency.req.version_spec or "any"
                 reverse_dependency_key = mermaid_id(reverse_dependency.key)
                 edges.add(f'{package_key} -- "{edge_label}" --> {reverse_dependency_key}')
     else:
         for package, dependencies in tree.items():
-            package_label = "\\n".join((package.project_name, package.version))
+            package_label = f"{package.project_name}\\n{package.version}"
             package_key = mermaid_id(package.key)
             nodes.add(f'{package_key}["{package_label}"]')
             for dependency in dependencies:
                 edge_label = dependency.version_spec or "any"
                 dependency_key = mermaid_id(dependency.key)
                 if dependency.is_missing:
                     dependency_label = f"{dependency.project_name}\\n(missing)"
@@ -708,59 +708,63 @@
 
     # Produce the Mermaid Markdown.
     indent = " " * 4
     output = dedent(
         f"""\
         flowchart TD
         {indent}classDef missing stroke-dasharray: 5
-        """
+        """,
     )
     # Sort the nodes and edges to make the output deterministic.
     output += indent
     output += f"\n{indent}".join(node for node in sorted(nodes))
     output += "\n" + indent
     output += f"\n{indent}".join(edge for edge in sorted(edges))
     output += "\n"
     return output
 
 
-def dump_graphviz(tree, output_format="dot", is_reverse=False):
-    """Output dependency graph as one of the supported GraphViz output formats.
+def dump_graphviz(tree, output_format="dot", is_reverse=False):  # noqa: C901, FBT002, PLR0912
+    """
+    Output dependency graph as one of the supported GraphViz output formats.
 
     :param dict tree: dependency graph
     :param string output_format: output format
     :param bool is_reverse: reverse or not
     :returns: representation of tree in the specified output format
     :rtype: str or binary representation depending on the output format
 
     """
     try:
         from graphviz import Digraph
-    except ImportError:
-        print("graphviz is not available, but necessary for the output " "option. Please install it.", file=sys.stderr)
-        sys.exit(1)
+    except ImportError as exc:
+        print(  # noqa: T201
+            "graphviz is not available, but necessary for the output option. Please install it.",
+            file=sys.stderr,
+        )
+        raise SystemExit(1) from exc
 
     try:
         from graphviz import parameters
     except ImportError:
         from graphviz import backend
 
         valid_formats = backend.FORMATS
-        print(
+        print(  # noqa: T201
             "Deprecation warning! Please upgrade graphviz to version >=0.18.0 "
             "Support for older versions will be removed in upcoming release",
             file=sys.stderr,
         )
     else:
         valid_formats = parameters.FORMATS
 
     if output_format not in valid_formats:
-        print(f"{output_format} is not a supported output format.", file=sys.stderr)
-        print(f"Supported formats are: {', '.join(sorted(valid_formats))}", file=sys.stderr)
-        sys.exit(1)
+        print(f"{output_format} is not a supported output format.", file=sys.stderr)  # noqa: T201
+        print(f"Supported formats are: {', '.join(sorted(valid_formats))}", file=sys.stderr)  # noqa: T201
+        raise SystemExit(1)
 
     graph = Digraph(format=output_format)
 
     if not is_reverse:
         for pkg, deps in tree.items():
             pkg_label = f"{pkg.project_name}\\n{pkg.version}"
             graph.node(pkg.key, label=pkg_label)
@@ -785,15 +789,15 @@
 
     # Allow output of dot format, even if GraphViz isn't installed.
     if output_format == "dot":
         # Emulates graphviz.dot.Dot.__iter__() to force the sorting of graph.body.
         # Fixes https://github.com/tox-dev/pipdeptree/issues/188
         # That way we can guarantee the output of the dot format is deterministic
         # and stable.
-        return "".join([tuple(graph)[0]] + sorted(graph.body) + [graph._tail])
+        return "".join([tuple(graph)[0], *sorted(graph.body), graph._tail])  # noqa: SLF001
 
     # As it's unknown if the selected output format is binary or not, try to
     # decode it as UTF8 and only print it out in binary if that's not possible.
     try:
         return graph.pipe().decode("utf-8")
     except UnicodeDecodeError:
         return graph.pipe()
@@ -802,15 +806,15 @@
 def print_graphviz(dump_output):
     """
     Dump the data generated by GraphViz to stdout.
 
     :param dump_output: The output from dump_graphviz
     """
     if hasattr(dump_output, "encode"):
-        print(dump_output)
+        print(dump_output)  # noqa: T201
     else:
         with os.fdopen(sys.stdout.fileno(), "wb") as bytestream:
             bytestream.write(dump_output)
 
 
 def conflicting_deps(tree):
     """
@@ -828,28 +832,28 @@
             if req.is_conflicting():
                 conflicting[p].append(req)
     return conflicting
 
 
 def render_conflicts_text(conflicts):
     if conflicts:
-        print("Warning!!! Possibly conflicting dependencies found:", file=sys.stderr)
+        print("Warning!!! Possibly conflicting dependencies found:", file=sys.stderr)  # noqa: T201
         # Enforce alphabetical order when listing conflicts
         pkgs = sorted(conflicts.keys())
         for p in pkgs:
-            pkg = p.render_as_root(False)
-            print(f"* {pkg}", file=sys.stderr)
+            pkg = p.render_as_root(False)  # noqa: FBT003
+            print(f"* {pkg}", file=sys.stderr)  # noqa: T201
             for req in conflicts[p]:
-                req_str = req.render_as_branch(False)
-                print(f" - {req_str}", file=sys.stderr)
+                req_str = req.render_as_branch(False)  # noqa: FBT003
+                print(f" - {req_str}", file=sys.stderr)  # noqa: T201
 
 
 def cyclic_deps(tree):
     """
-    Return cyclic dependencies as list of tuples
+    Return cyclic dependencies as list of tuples.
 
     :param PackageDAG tree: package tree/dag
     :returns: list of tuples representing cyclic dependencies
     :rtype: list
     """
     index = {p.key: {r.key for r in rs} for p, rs in tree.items()}
     cyclic = []
@@ -859,37 +863,37 @@
                 p_as_dep_of_r = [x for x in tree.get(tree.get_node_as_parent(r.key)) if x.key == p.key][0]
                 cyclic.append((p, r, p_as_dep_of_r))
     return cyclic
 
 
 def render_cycles_text(cycles):
     if cycles:
-        print("Warning!! Cyclic dependencies found:", file=sys.stderr)
+        print("Warning!! Cyclic dependencies found:", file=sys.stderr)  # noqa: T201
         # List in alphabetical order of the dependency that's cycling
         # (2nd item in the tuple)
         cycles = sorted(cycles, key=lambda xs: xs[1].key)
         for a, b, c in cycles:
-            print(f"* {a.project_name} => {b.project_name} => {c.project_name}", file=sys.stderr)
+            print(f"* {a.project_name} => {b.project_name} => {c.project_name}", file=sys.stderr)  # noqa: T201
 
 
 def get_parser():
     parser = argparse.ArgumentParser(description="Dependency tree of the installed python packages")
     parser.add_argument("-v", "--version", action="version", version=f"{__version__}")
     parser.add_argument("-f", "--freeze", action="store_true", help="Print names so as to write freeze files")
     parser.add_argument(
         "--python",
         default=sys.executable,
-        help="Python to use to look for packages in it (default: where" " installed)",
+        help="Python to use to look for packages in it (default: where installed)",
     )
     parser.add_argument("-a", "--all", action="store_true", help="list all deps at top level")
     parser.add_argument(
         "-l",
         "--local-only",
         action="store_true",
-        help="If in a virtualenv that has global access " "do not show globally installed packages",
+        help="If in a virtualenv that has global access do not show globally installed packages",
     )
     parser.add_argument("-u", "--user-only", action="store_true", help="Only show installations in the user site dir")
     parser.add_argument(
         "-w",
         "--warn",
         action="store",
         dest="warn",
@@ -956,15 +960,15 @@
             "This option overrides all other options (except --json)."
         ),
     )
     parser.add_argument(
         "--mermaid",
         action="store_true",
         default=False,
-        help=("Display dependency tree as a Mermaid graph. " "This option overrides all other options."),
+        help="Display dependency tree as a Mermaid graph. This option overrides all other options.",
     )
     parser.add_argument(
         "--graph-output",
         dest="output_format",
         help=(
             "Print a dependency graph in the specified output "
             "format. Available are all formats supported by "
@@ -986,107 +990,115 @@
 
 def _get_args():
     parser = get_parser()
     return parser.parse_args()
 
 
 def handle_non_host_target(args):
-    of_python = os.path.abspath(args.python)
     # if target is not current python re-invoke it under the actual host
-    if of_python != os.path.abspath(sys.executable):
+    if Path(args.python).absolute() != Path(sys.executable).absolute():
         # there's no way to guarantee that graphviz is available, so refuse
         if args.output_format:
-            print("graphviz functionality is not supported when querying" " non-host python", file=sys.stderr)
+            print(  # noqa: T201
+                "graphviz functionality is not supported when querying non-host python",
+                file=sys.stderr,
+            )
             raise SystemExit(1)
         argv = sys.argv[1:]  # remove current python executable
         for py_at, value in enumerate(argv):
             if value == "--python":
                 del argv[py_at]
                 del argv[py_at]
             elif value.startswith("--python"):
                 del argv[py_at]
 
         main_file = inspect.getsourcefile(sys.modules[__name__])
         with tempfile.TemporaryDirectory() as project:
-            dest = os.path.join(project, "pipdeptree")
-            shutil.copytree(os.path.dirname(main_file), dest)
+            shutil.copytree(Path(main_file).parent, Path(project) / "pipdeptree")
             # invoke from an empty folder to avoid cwd altering sys.path
             env = os.environ.copy()
             env["PYTHONPATH"] = project
-            cmd = [of_python, "-m", "pipdeptree"]
+            cmd = [args.python, "-m", "pipdeptree"]
             cmd.extend(argv)
-            return subprocess.call(cmd, cwd=project, env=env)
+            return subprocess.call(cmd, cwd=project, env=env)  # noqa: S603
     return None
 
 
-def get_installed_distributions(local_only=False, user_only=False):
+def get_installed_distributions(local_only=False, user_only=False):  # noqa: FBT002
     try:
         from pip._internal.metadata import pkg_resources
     except ImportError:
         # For backward compatibility with python ver. 2.7 and pip
         # version 20.3.4 (the latest pip version that works with python
         # version 2.7)
         from pip._internal.utils import misc
 
         return misc.get_installed_distributions(local_only=local_only, user_only=user_only)
     else:
         dists = pkg_resources.Environment.from_paths(None).iter_installed_distributions(
-            local_only=local_only, skip=(), user_only=user_only
+            local_only=local_only,
+            skip=(),
+            user_only=user_only,
         )
-        return [d._dist for d in dists]
+        return [d._dist for d in dists]  # noqa: SLF001
 
 
 def main():
     args = _get_args()
     result = handle_non_host_target(args)
     if result is not None:
         return result
 
     pkgs = get_installed_distributions(local_only=args.local_only, user_only=args.user_only)
-
     tree = PackageDAG.from_pkgs(pkgs)
-
     is_text_output = not any([args.json, args.json_tree, args.output_format])
 
-    return_code = 0
+    return_code = _check_cycle_conflict(args, is_text_output, tree)
+
+    # Reverse the tree (if applicable) before filtering, thus ensuring
+    # that the filter will be applied on ReverseTree
+    if args.reverse:
+        tree = tree.reverse()
+
+    show_only = set(args.packages.split(",")) if args.packages else None
+    exclude = set(args.exclude.split(",")) if args.exclude else None
+
+    if show_only is not None or exclude is not None:
+        tree = tree.filter_nodes(show_only, exclude)
+
+    _render(args, tree)
+
+    return return_code
 
+
+def _check_cycle_conflict(args, is_text_output, tree):
     # Before any reversing or filtering, show warnings to console
     # about possibly conflicting or cyclic deps if found and warnings
     # are enabled (i.e. only if output is to be printed to console)
     if is_text_output and args.warn != "silence":
         conflicts = conflicting_deps(tree)
         if conflicts:
             render_conflicts_text(conflicts)
-            print("-" * 72, file=sys.stderr)
+            print("-" * 72, file=sys.stderr)  # noqa: T201
 
         cycles = cyclic_deps(tree)
         if cycles:
             render_cycles_text(cycles)
-            print("-" * 72, file=sys.stderr)
+            print("-" * 72, file=sys.stderr)  # noqa: T201
 
         if args.warn == "fail" and (conflicts or cycles):
-            return_code = 1
-
-    # Reverse the tree (if applicable) before filtering, thus ensuring
-    # that the filter will be applied on ReverseTree
-    if args.reverse:
-        tree = tree.reverse()
+            return 1
+    return 0
 
-    show_only = set(args.packages.split(",")) if args.packages else None
-    exclude = set(args.exclude.split(",")) if args.exclude else None
-
-    if show_only is not None or exclude is not None:
-        tree = tree.filter(show_only, exclude)
 
+def _render(args, tree):
     if args.json:
-        print(render_json(tree, indent=4))
+        print(render_json(tree, indent=4))  # noqa: T201
     elif args.json_tree:
-        print(render_json_tree(tree, indent=4))
+        print(render_json_tree(tree, indent=4))  # noqa: T201
     elif args.mermaid:
-        print(render_mermaid(tree))
+        print(render_mermaid(tree))  # noqa: T201
     elif args.output_format:
         output = dump_graphviz(tree, output_format=args.output_format, is_reverse=args.reverse)
         print_graphviz(output)
     else:
         render_text(tree, args.depth, args.all, args.freeze)
-
-    return return_code
```

### Comparing `pipdeptree-2.9.0/tests/test_pipdeptree.py` & `pipdeptree-2.9.1/tests/test_pipdeptree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+from __future__ import annotations
+
 import platform
 import random
 import subprocess
 import sys
-from contextlib import contextmanager
 from itertools import chain
 from pathlib import Path
-from tempfile import NamedTemporaryFile
 from textwrap import dedent, indent
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 try:
     from unittest import mock
 except ImportError:
     from unittest import mock
 
 import pytest
 import virtualenv
 
 import pipdeptree as p
 
+if TYPE_CHECKING:
+    from pytest_mock import MockerFixture
+
 # Tests for DAG classes
 
 
 def mock_pkgs(simple_graph):
     for node, children in simple_graph.items():
         nk, nv = node
         m = mock.Mock(key=nk, project_name=nk, version=nv)
@@ -40,15 +43,15 @@
 def mock_package_dag(simple_graph):
     pkgs = list(mock_pkgs(simple_graph))
     return p.PackageDAG.from_pkgs(pkgs)
 
 
 # util for comparing tree contents with a simple graph
 def dag_to_dict(g):
-    return {k.key: [v.key for v in vs] for k, vs in g._obj.items()}
+    return {k.key: [v.key for v in vs] for k, vs in g._obj.items()}  # noqa: SLF001
 
 
 def sort_map_values(m):
     return {k: sorted(v) for k, v in m.items()}
 
 
 t = mock_package_dag(
@@ -56,136 +59,135 @@
         ("a", "3.4.0"): [("b", [(">=", "2.0.0")]), ("c", [(">=", "5.7.1")])],
         ("b", "2.3.1"): [("d", [(">=", "2.30"), ("<", "2.42")])],
         ("c", "5.10.0"): [("d", [(">=", "2.30")]), ("e", [(">=", "0.12.1")])],
         ("d", "2.35"): [("e", [(">=", "0.9.0")])],
         ("e", "0.12.1"): [],
         ("f", "3.1"): [("b", [(">=", "2.1.0")])],
         ("g", "6.8.3rc1"): [("e", [(">=", "0.9.0")]), ("f", [(">=", "3.0.0")])],
-    }
+    },
 )
 
 
 def test_package_dag_get_node_as_parent():
-    assert "b" == t.get_node_as_parent("b").key
-    assert "c" == t.get_node_as_parent("c").key
+    assert t.get_node_as_parent("b").key == "b"
+    assert t.get_node_as_parent("c").key == "c"
 
 
 def test_package_dag_filter():
     # When both show_only and exclude are not specified, same tree
-    # object is returned
-    assert t.filter(None, None) is t
+    assert t.filter_nodes(None, None) is t
 
     # when show_only is specified
-    g1 = dag_to_dict(t.filter({"a", "d"}, None))
+    g1 = dag_to_dict(t.filter_nodes({"a", "d"}, None))
     expected = {"a": ["b", "c"], "b": ["d"], "c": ["d", "e"], "d": ["e"], "e": []}
     assert expected == g1
 
     # when exclude is specified
-    g2 = dag_to_dict(t.filter(None, ["d"]))
+    g2 = dag_to_dict(t.filter_nodes(None, ["d"]))
     expected = {"a": ["b", "c"], "b": [], "c": ["e"], "e": [], "f": ["b"], "g": ["e", "f"]}
     assert expected == g2
 
     # when both show_only and exclude are specified
-    g3 = dag_to_dict(t.filter({"a", "g"}, {"d", "e"}))
+    g3 = dag_to_dict(t.filter_nodes({"a", "g"}, {"d", "e"}))
     expected = {"a": ["b", "c"], "b": [], "c": [], "f": ["b"], "g": ["f"]}
     assert expected == g3
 
     # when conflicting values in show_only and exclude, AssertionError
     # is raised
     with pytest.raises(AssertionError):
-        dag_to_dict(t.filter({"d"}, {"D", "e"}))
+        dag_to_dict(t.filter_nodes({"d"}, {"D", "e"}))
 
 
 @pytest.fixture(scope="session")
 def t_fnmatch() -> Any:
     return mock_package_dag(
         {
             ("a.a", "1"): [("a.b", []), ("a.c", [])],
             ("a.b", "1"): [("a.c", [])],
             ("b.a", "1"): [("b.b", [])],
             ("b.b", "1"): [("a.b", [])],
-        }
+        },
     )
 
 
 def test_package_dag_filter_fnmatch_include_a(t_fnmatch: Any) -> None:
     # test include for a.*in the result we got only a.* nodes
-    graph = dag_to_dict(t_fnmatch.filter({"a.*"}, None))
+    graph = dag_to_dict(t_fnmatch.filter_nodes({"a.*"}, None))
     assert graph == {"a.a": ["a.b", "a.c"], "a.b": ["a.c"]}
 
 
 def test_package_dag_filter_fnmatch_include_b(t_fnmatch: Any) -> None:
     # test include for b.*, which has a.b and a.c in tree, but not a.a
     # in the result we got the b.* nodes plus the a.b node as child in the tree
-    graph = dag_to_dict(t_fnmatch.filter({"b.*"}, None))
+    graph = dag_to_dict(t_fnmatch.filter_nodes({"b.*"}, None))
     assert graph == {"b.a": ["b.b"], "b.b": ["a.b"], "a.b": ["a.c"]}
 
 
 def test_package_dag_filter_fnmatch_exclude_c(t_fnmatch: Any) -> None:
     # test exclude for b.* in the result we got only a.* nodes
-    graph = dag_to_dict(t_fnmatch.filter(None, {"b.*"}))
+    graph = dag_to_dict(t_fnmatch.filter_nodes(None, {"b.*"}))
     assert graph == {"a.a": ["a.b", "a.c"], "a.b": ["a.c"]}
 
 
 def test_package_dag_filter_fnmatch_exclude_a(t_fnmatch: Any) -> None:
     # test exclude for a.* in the result we got only b.* nodes
-    graph = dag_to_dict(t_fnmatch.filter(None, {"a.*"}))
+    graph = dag_to_dict(t_fnmatch.filter_nodes(None, {"a.*"}))
     assert graph == {"b.a": ["b.b"], "b.b": []}
 
 
 def test_package_dag_reverse():
     t1 = t.reverse()
     expected = {"a": [], "b": ["a", "f"], "c": ["a"], "d": ["b", "c"], "e": ["c", "d", "g"], "f": ["g"], "g": []}
     assert isinstance(t1, p.ReversedPackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t1))
-    assert all(isinstance(k, p.ReqPackage) for k in t1.keys())
+    assert all(isinstance(k, p.ReqPackage) for k in t1)
     assert all(isinstance(v, p.DistPackage) for v in chain.from_iterable(t1.values()))
 
     # testing reversal of ReversedPackageDAG instance
     expected = {"a": ["b", "c"], "b": ["d"], "c": ["d", "e"], "d": ["e"], "e": [], "f": ["b"], "g": ["e", "f"]}
     t2 = t1.reverse()
     assert isinstance(t2, p.PackageDAG)
     assert sort_map_values(expected) == sort_map_values(dag_to_dict(t2))
-    assert all(isinstance(k, p.DistPackage) for k in t2.keys())
+    assert all(isinstance(k, p.DistPackage) for k in t2)
     assert all(isinstance(v, p.ReqPackage) for v in chain.from_iterable(t2.values()))
 
 
 # Tests for Package classes
 #
 # Note: For all render methods, we are only testing for frozen=False
 # as mocks with frozen=True are a lot more complicated
 
 
 def test_dist_package_render_as_root():
     foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
     dp = p.DistPackage(foo)
     is_frozen = False
-    assert "foo==20.4.1" == dp.render_as_root(is_frozen)
+    assert dp.render_as_root(is_frozen) == "foo==20.4.1"
 
 
 def test_dist_package_render_as_branch():
     foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = p.ReqPackage(bar_req, dist=bar)
     dp = p.DistPackage(foo).as_parent_of(rp)
     is_frozen = False
-    assert "foo==20.4.1 [requires: bar>=4.0]" == dp.render_as_branch(is_frozen)
+    assert dp.render_as_branch(is_frozen) == "foo==20.4.1 [requires: bar>=4.0]"
 
 
 def test_dist_package_as_parent_of():
     foo = mock.Mock(key="foo", project_name="foo", version="20.4.1")
     dp = p.DistPackage(foo)
     assert dp.req is None
 
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = p.ReqPackage(bar_req, dist=bar)
     dp1 = dp.as_parent_of(rp)
-    assert dp1._obj == dp._obj
+    assert dp1._obj == dp._obj  # noqa: SLF001
     assert dp1.req is rp
 
     dp2 = dp.as_parent_of(None)
     assert dp2 is dp
 
 
 def test_dist_package_as_dict():
@@ -197,23 +199,23 @@
 
 
 def test_req_package_render_as_root():
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = p.ReqPackage(bar_req, dist=bar)
     is_frozen = False
-    assert "bar==4.1.0" == rp.render_as_root(is_frozen)
+    assert rp.render_as_root(is_frozen) == "bar==4.1.0"
 
 
 def test_req_package_render_as_branch():
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = p.ReqPackage(bar_req, dist=bar)
     is_frozen = False
-    assert "bar [required: >=4.0, installed: 4.1.0]" == rp.render_as_branch(is_frozen)
+    assert rp.render_as_branch(is_frozen) == "bar [required: >=4.0, installed: 4.1.0]"
 
 
 def test_req_package_as_dict():
     bar = mock.Mock(key="bar", project_name="bar", version="4.1.0")
     bar_req = mock.Mock(key="bar", project_name="bar", version="4.1.0", specs=[(">=", "4.0")])
     rp = p.ReqPackage(bar_req, dist=bar)
     result = rp.as_dict()
@@ -226,15 +228,15 @@
 
 class MockStdout:
     """
     A wrapper to stdout that mocks the `encoding` attribute (to have `render_text()` render with unicode/non-unicode)
     and `write()` (so that `print()` calls can write to stdout).
     """
 
-    def __init__(self, encoding):
+    def __init__(self, encoding) -> None:
         self.stdout = sys.stdout
         self.encoding = encoding
 
     def encoding(self):
         return self.encoding
 
     def write(self, text):
@@ -573,21 +575,21 @@
 # Tests for graph outputs
 
 
 def randomized_dag_copy(t):
     """Returns a copy of the package tree fixture with dependencies in randomized order."""
     # Extract the dependency graph from the package tree and randomize it.
     randomized_graph = {}
-    randomized_nodes = list(t._obj.keys())
+    randomized_nodes = list(t._obj.keys())  # noqa: SLF001
     random.shuffle(randomized_nodes)
     for node in randomized_nodes:
-        edges = t._obj[node]
+        edges = t._obj[node]  # noqa: SLF001
         random.shuffle(edges)
         randomized_graph[node] = edges
-    assert set(randomized_graph) == set(t._obj)
+    assert set(randomized_graph) == set(t._obj)  # noqa: SLF001
 
     # Create a randomized package tree.
     randomized_dag = p.PackageDAG(randomized_graph)
     assert len(t) == len(randomized_dag)
     return randomized_dag
 
 
@@ -608,29 +610,29 @@
             a["a\\n3.4.0"]
             b["b\\n2.3.1"]
             c["c\\n5.10.0"]
             d["d\\n2.35"]
             e["e\\n0.12.1"]
             f["f\\n3.1"]
             g["g\\n6.8.3rc1"]
-        """
+        """,
     )
     dependency_edges = indent(
         dedent(
             """\
             a -- ">=2.0.0" --> b
             a -- ">=5.7.1" --> c
             b -- ">=2.30,<2.42" --> d
             c -- ">=0.12.1" --> e
             c -- ">=2.30" --> d
             d -- ">=0.9.0" --> e
             f -- ">=2.1.0" --> b
             g -- ">=0.9.0" --> e
             g -- ">=3.0.0" --> f
-        """
+        """,
         ),
         " " * 4,
     ).rstrip()
     reverse_dependency_edges = indent(
         dedent(
             """\
             b -- ">=2.0.0" --> a
@@ -638,15 +640,15 @@
             c -- ">=5.7.1" --> a
             d -- ">=2.30" --> c
             d -- ">=2.30,<2.42" --> b
             e -- ">=0.12.1" --> c
             e -- ">=0.9.0" --> d
             e -- ">=0.9.0" --> g
             f -- ">=3.0.0" --> g
-        """
+        """,
         ),
         " " * 4,
     ).rstrip()
 
     for package_tree in (t, randomized_dag_copy(t)):
         output = p.render_mermaid(package_tree)
         assert output.rstrip() == nodes + dependency_edges
@@ -654,25 +656,25 @@
         assert reversed_output.rstrip() == nodes + reverse_dependency_edges
 
 
 def test_mermaid_reserved_ids():
     package_tree = mock_package_dag(
         {
             ("click", "3.4.0"): [("click-extra", [(">=", "2.0.0")])],
-        }
+        },
     )
     output = p.render_mermaid(package_tree)
     assert output == dedent(
         """\
         flowchart TD
             classDef missing stroke-dasharray: 5
             click-extra["click-extra\\n(missing)"]:::missing
             click_0["click\\n3.4.0"]
             click_0 -.-> click-extra
-        """
+        """,
     )
 
 
 def test_render_dot(capsys):
     # Check both the sorted and randomized package tree produces the same sorted
     # graphviz output.
     for package_tree in (t, randomized_dag_copy(t)):
@@ -696,35 +698,26 @@
             \tf -> b [label=">=2.1.0"]
             \tf [label="f\\n3.1"]
             \tg -> e [label=">=0.9.0"]
             \tg -> f [label=">=3.0.0"]
             \tg [label="g\\n6.8.3rc1"]
             }
 
-            """
+            """,
         )
 
 
-def test_render_pdf():
+def test_render_pdf(tmp_path: Path, mocker: MockerFixture) -> None:
     output = p.dump_graphviz(t, output_format="pdf")
-
-    @contextmanager
-    def redirect_stdout(new_target):
-        old_target, sys.stdout = sys.stdout, new_target
-        try:
-            yield new_target
-        finally:
-            sys.stdout = old_target
-
-    with NamedTemporaryFile(delete=True) as f:
-        with redirect_stdout(f):
+    res = tmp_path / "file"
+    with pytest.raises(OSError, match="Bad file descriptor"):  # noqa: PT012, SIM117 # because we reopen the file
+        with res.open("wb") as buf:
+            mocker.patch.object(sys, "stdout", buf)
             p.print_graphviz(output)
-        rf = open(f.name, "rb")
-        assert b"%PDF" == rf.read()[:4]
-        # @NOTE: rf is not closed to avoid "bad filedescriptor" error
+    assert res.read_bytes()[:4] == b"%PDF"
 
 
 def test_render_svg(capsys):
     output = p.dump_graphviz(t, output_format="svg")
     p.print_graphviz(output)
     out, _ = capsys.readouterr()
     assert out.startswith("<?xml")
@@ -910,20 +903,20 @@
         expected = {"cffi", "greenlet", "pip", "readline", "setuptools", "wheel"}
     else:
         raise ValueError(implementation)
     if sys.version_info >= (3, 12):
         expected -= {"setuptools", "wheel"}
     assert found == expected, out
 
-    monkeypatch.setattr(sys, "argv", cmd + ["--graph-output", "something"])
+    monkeypatch.setattr(sys, "argv", [*cmd, "--graph-output", "something"])
     with pytest.raises(SystemExit) as context:
         p.main()
     out, err = capfd.readouterr()
     assert context.value.code == 1
     assert not out
-    assert err == "graphviz functionality is not supported when querying" " non-host python\n"
+    assert err == "graphviz functionality is not supported when querying non-host python\n"
 
 
 def test_guess_version_setuptools():
     script = Path(__file__).parent / "guess_version_setuptools.py"
     output = subprocess.check_output([sys.executable, script], text=True)
     assert output == "?"
```

### Comparing `pipdeptree-2.9.0/LICENSE` & `pipdeptree-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipdeptree-2.9.0/README.md` & `pipdeptree-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,14 @@
 
 ```bash
 $ pipdeptree --json-tree
 ```
 
 ## Visualizing the dependency graph
 
-![image](https://raw.githubusercontent.com/tox-dev/pipdeptree/main/docs/twine-pdt.png)
-
 The dependency graph can also be visualized using [GraphViz](http://www.graphviz.org/):
 
 ```bash
 $ pipdeptree --graph-output dot > dependencies.dot
 $ pipdeptree --graph-output pdf > dependencies.pdf
 $ pipdeptree --graph-output png > dependencies.png
 $ pipdeptree --graph-output svg > dependencies.svg
```

### Comparing `pipdeptree-2.9.0/PKG-INFO` & `pipdeptree-2.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipdeptree
-Version: 2.9.0
+Version: 2.9.1
 Summary: Command line utility to show dependency tree of packages.
 Project-URL: Changelog, https://github.com/tox-dev/pipdeptree/blob/main/CHANGES.md
 Project-URL: Documentation, https://github.com/tox-dev/pipdeptree/blob/main/README.md#pipdeptree
 Project-URL: Homepage, https://github.com/tox-dev/pipdeptree
 Project-URL: Source, https://github.com/tox-dev/pipdeptree
 Project-URL: Tracker, https://github.com/tox-dev/pipdeptree/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Vineet Naik <naikvin@gmail.com>
@@ -32,27 +32,32 @@
 Keywords: application,cache,directory,log,user
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Provides-Extra: graphviz
 Requires-Dist: graphviz>=0.20.1; extra == 'graphviz'
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: diff-cover>=7.5; extra == 'test'
-Requires-Dist: pip>=23.1; extra == 'test'
-Requires-Dist: pytest-cov>=4; extra == 'test'
+Requires-Dist: pip>=23.1.2; extra == 'test'
+Requires-Dist: pytest-cov>=4.1; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
 Requires-Dist: pytest>=7.3.1; extra == 'test'
-Requires-Dist: virtualenv<21,>=20.21; extra == 'test'
+Requires-Dist: virtualenv<21,>=20.23; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pipdeptree
 
 [![check](https://github.com/tox-dev/pipdeptree/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pipdeptree/actions/workflows/check.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/tox-dev/pipdeptree/main.svg)](https://results.pre-commit.ci/latest/github/tox-dev/pipdeptree/main)
 
@@ -248,16 +253,14 @@
 
 ```bash
 $ pipdeptree --json-tree
 ```
 
 ## Visualizing the dependency graph
 
-![image](https://raw.githubusercontent.com/tox-dev/pipdeptree/main/docs/twine-pdt.png)
-
 The dependency graph can also be visualized using [GraphViz](http://www.graphviz.org/):
 
 ```bash
 $ pipdeptree --graph-output dot > dependencies.dot
 $ pipdeptree --graph-output pdf > dependencies.pdf
 $ pipdeptree --graph-output png > dependencies.png
 $ pipdeptree --graph-output svg > dependencies.svg
```

