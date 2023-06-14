# Comparing `tmp/docleaf-0.3.0-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.4.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1075788 bytes, number of entries: 10
--rw-r--r--  4.6 unx     4459 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx     3774 b- defN 23-Jun-10 16:49 docleaf/copied.py
--rw-r--r--  4.6 unx     2954 b- defN 23-Jun-10 16:49 docleaf/domains.py
--rw-r--r--  4.6 unx    17005 b- defN 23-Jun-10 16:49 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jun-10 16:49 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-10 16:49 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3038208 b- defN 23-Jun-10 16:49 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      775 b- defN 23-Jun-10 16:49 docleaf-0.3.0.dist-info/RECORD
-10 files, 3070943 bytes uncompressed, 1074482 bytes compressed:  65.0%
+Zip file size: 1081228 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     6708 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3573 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx     3836 b- defN 23-Jun-14 16:33 docleaf/copied.py
+-rw-r--r--  4.6 unx     3709 b- defN 23-Jun-14 16:33 docleaf/domains.py
+-rw-r--r--  4.6 unx    18910 b- defN 23-Jun-14 16:33 docleaf/doxygen.py
+-rw-r--r--  4.6 unx       99 b- defN 23-Jun-14 16:33 docleaf/errors.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-14 16:33 docleaf/__init__.py
+-rwxr-xr-x  4.6 unx  3051520 b- defN 23-Jun-14 16:33 docleaf/backend.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      775 b- defN 23-Jun-14 16:33 docleaf-0.4.0.dist-info/RECORD
+10 files, 3089226 bytes uncompressed, 1079922 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: docleaf-0.3.0.dist-info/METADATA
+Filename: docleaf-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.3.0.dist-info/WHEEL
+Filename: docleaf-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.3.0.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.4.0.dist-info/license_files/LICENSE.md
 Comment: 
 
 Filename: docleaf/copied.py
 Comment: 
 
 Filename: docleaf/domains.py
 Comment: 
@@ -21,11 +21,11 @@
 
 Filename: docleaf/__init__.py
 Comment: 
 
 Filename: docleaf/backend.cp39-win_amd64.pyd
 Comment: 
 
-Filename: docleaf-0.3.0.dist-info/RECORD
+Filename: docleaf-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docleaf/copied.py

```diff
@@ -4,21 +4,23 @@
 
 class NodeFinder(nodes.SparseNodeVisitor):
     """Find the Docutils desc_signature declarator and desc_content nodes."""
 
     def __init__(self, document):
         super().__init__(document)
         self.declarator = None
+        self.signature = None
         self.content = None
 
     def visit_desc_signature(self, node):
         # Find the last signature node because it contains the actual declarator
         # rather than "template <...>". In Sphinx 1.4.1 we'll be able to use sphinx_cpp_tagname:
         # https://github.com/michaeljones/breathe/issues/242
         self.declarator = node
+        self.signature = node
 
     def visit_desc_signature_line(self, node):
         # In sphinx 1.5, there is now a desc_signature_line node within the desc_signature
         # This should be used instead
         self.declarator = node
 
     def visit_desc_content(self, node):
```

## docleaf/domains.py

```diff
@@ -2,51 +2,84 @@
 
 from sphinx.domains import cpp, c
 from docutils import nodes
 
 from . import copied
 from .errors import DocleafError
 
-null_handler = lambda finder: finder
 
+def null_handler(finder, location):
+    return
 
-def strip_desc_addname(finder):
+
+def strip_desc_addname(finder, location):
     # We pass qualified values to the domain directives but we don't always want Sphinx to show the qualified part
     # in the output as normally it is shown but the nesting of the entities so we strip it out which involes removing
     # the 'desc_addname' node in the output
     finder.declarator.children = [
         node for node in finder.declarator.children if node.tagname != "desc_addname"
     ]
 
 
+def add_location_via_names(finder, location):
+    if finder.signature and location:
+        finder.signature["names"] = f"{location['path']}:{location['line']}"
+
+
+def chain(*funcs):
+    def inner(finder, location):
+        for func in funcs:
+            func(finder, location)
+
+    return inner
+
+
 cpp_domain = {
-    "class": (cpp.CPPClassObject, "class", null_handler),
-    "enum": (cpp.CPPEnumObject, "enum", null_handler),
-    "enumerator": (cpp.CPPEnumeratorObject, "enumerator", strip_desc_addname),
-    "function": (cpp.CPPFunctionObject, "function", strip_desc_addname),
-    "member": (cpp.CPPMemberObject, "member", strip_desc_addname),
-    "struct": (cpp.CPPClassObject, "struct", null_handler),
+    "class": (cpp.CPPClassObject, "class", add_location_via_names),
+    "enum": (cpp.CPPEnumObject, "enum", add_location_via_names),
+    "enumerator": (
+        cpp.CPPEnumeratorObject,
+        "enumerator",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "function": (
+        cpp.CPPFunctionObject,
+        "function",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "member": (cpp.CPPMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
+    "struct": (cpp.CPPClassObject, "struct", add_location_via_names),
 }
 
 c_domain = {
-    "define": (c.CMacroObject, "macro", null_handler),
-    "enum": (c.CEnumObject, "enum", null_handler),
-    "enumerator": (c.CEnumeratorObject, "enumerator", strip_desc_addname),
-    "function": (c.CFunctionObject, "function", null_handler),
-    "member": (c.CMemberObject, "member", strip_desc_addname),
-    "struct": (c.CStructObject, "struct", null_handler),
-    "typedef": (c.CTypeObject, "type", null_handler),
-    "union": (c.CUnionObject, "union", strip_desc_addname),
+    "define": (c.CMacroObject, "macro", add_location_via_names),
+    "enum": (c.CEnumObject, "enum", add_location_via_names),
+    "enumerator": (
+        c.CEnumeratorObject,
+        "enumerator",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "function": (c.CFunctionObject, "function", add_location_via_names),
+    "member": (c.CMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
+    "struct": (c.CStructObject, "struct", add_location_via_names),
+    "typedef": (c.CTypeObject, "type", add_location_via_names),
+    "union": (c.CUnionObject, "union", chain(strip_desc_addname, add_location_via_names)),
 }
 
 domains = {"cpp": cpp_domain, "c": c_domain}
 
 
 def render_domain_entry(
-    domain_name: str, type: str, declaration: str, target, directive_args: list, content: list
+    domain_name: str,
+    type: str,
+    declaration: str,
+    location,
+    target,
+    directive_args: list,
+    content: list,
 ):
     # print("render_domain_entry", domain_name, type, declaration)
     try:
         domain = domains[domain_name]
     except KeyError:
         raise DocleafError(f"Unsupported domain: {domain_name}")
 
@@ -65,15 +98,15 @@
     rst_node = nodes[1]
     finder = copied.NodeFinder(rst_node.document)
     rst_node.walk(finder)
 
     set_children(finder.content, content)
     finder.declarator.children.insert(0, target)
 
-    handler(finder)
+    handler(finder, location)
 
     return nodes
 
 
 def set_children(node, children):
     """
     The children have to be informed of the parent and that happens in the parents helper methods like 'append' and
```

## docleaf/doxygen.py

```diff
@@ -1,9 +1,10 @@
 from typing import List
 from collections import defaultdict
+from pathlib import Path
 import itertools
 import textwrap
 import hashlib
 import pprint
 import time
 import sys
 import os
@@ -26,14 +27,57 @@
 from .errors import DocleafError
 
 __version__ = "0.0.0"
 
 logger = logging.getLogger(__name__)
 
 
+class GitHubLinkResolver:
+    """
+    This works on the assumption that we can insert our own data into the 'names' field of desc_signature nodes in
+    domain entries. That assumption might fail or clash with other things so we try to be careful when extracting the
+    data from 'names' and fail early and quietly.
+    """
+
+    def __init__(self, *, root, user, repo, tag=None, branch=None, revision=None):
+        self.root = Path(root).resolve()
+        self.user = user
+        self.repo = repo
+        self.tag = tag
+        self.branch = branch
+        self.revision = revision
+
+    def __call__(self, domain, info):
+        if domain not in ["c", "cpp"]:
+            return None
+
+        names = info.get("names")
+        if not names:
+            return None
+
+        entries = names.rsplit(":", 1)
+        if len(entries) != 2:
+            return None
+
+        path = Path(entries[0]).resolve()
+        relative = path.relative_to(self.root)
+
+        try:
+            line = int(entries[1])
+        except ValueError:
+            # Unable to get line number - exit quietly
+            return None
+
+        reference = self.tag or self.branch or self.revision
+        if not reference:
+            return None
+
+        return f"https://github.com/{self.user}/{self.repo}/blob/{reference}/{relative}#L{line}"
+
+
 def as_list(node):
     def wrapper(*children, **attributes):
         return [node(*children, **attributes)]
 
     return wrapper
 
 
@@ -99,14 +143,15 @@
         return target
 
     def build_domain_entry(self, *children, **attributes):
         return domains.render_domain_entry(
             attributes["domain"],
             attributes["type"],
             attributes["declaration"],
+            attributes.get("location"),
             self.build_target(**attributes["target"]),
             self.directive_arguments,
             children,
         )
 
     def build_restructured_text_block(self, *children, **attributes):
         text = textwrap.dedent(children[0])
@@ -193,19 +238,26 @@
     final_argument_whitespace = True
     option_spec = {
         "project": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
-        project = self.options["project"] or self.app.config.docleaf_default_project
-        path = self.app.config.docleaf_projects[project]
+        project_name = self.options["project"] or self.app.config.docleaf_default_project
+        project = self.app.config.docleaf_projects[project_name]
+
+        skip_settings = get_skip_settings(self.app, self.options)
+        context = backend.Context(
+            project["root"],
+            skip_settings,
+            self.app.config.docleaf_domain_by_extension,
+        )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_class(name, path, tracked_cache)
+        node_list = backend.render_class(name, project["xml"], context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class StructDirective(BaseDirective):
@@ -215,24 +267,25 @@
     final_argument_whitespace = True
     option_spec = {
         "project": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
-        project = self.options["project"] or self.app.config.docleaf_default_project
-        path = self.app.config.docleaf_projects[project]
+        project_name = self.options["project"] or self.app.config.docleaf_default_project
+        project = self.app.config.docleaf_projects[project_name]
         skip_settings = get_skip_settings(self.app, self.options)
         context = backend.Context(
+            project["root"],
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_struct(name, path, context, tracked_cache)
+        node_list = backend.render_struct(name, project["xml"], context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class EnumDirective(BaseDirective):
@@ -243,25 +296,26 @@
     option_spec = {
         "project": directives.unchanged,
         "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
-        project = self.options["project"] or self.app.config.docleaf_default_project
-        path = self.app.config.docleaf_projects[project]
+        project_name = self.options["project"] or self.app.config.docleaf_default_project
+        project = self.app.config.docleaf_projects[project_name]
         skip_settings = get_skip_settings(self.app, self.options)
 
         context = backend.Context(
+            project["root"],
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_enum(name, path, context, tracked_cache)
+        node_list = backend.render_enum(name, project["xml"], context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class FunctionDirective(BaseDirective):
@@ -272,25 +326,26 @@
     option_spec = {
         "project": directives.unchanged,
         "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
-        project = self.options["project"] or self.app.config.docleaf_default_project
-        path = self.app.config.docleaf_projects[project]
+        project_name = self.options["project"] or self.app.config.docleaf_default_project
+        project = self.app.config.docleaf_projects[project_name]
         skip_settings = get_skip_settings(self.app, self.options)
 
         context = backend.Context(
+            project["root"],
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_function(name, path, context, tracked_cache)
+        node_list = backend.render_function(name, project["xml"], context, tracked_cache)
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
 
         node_builder = NodeManager(self.state, self.get_directive_args())
         return render_node_list(node_list, node_builder)
 
 
 class GroupDirective(BaseDirective):
@@ -303,29 +358,30 @@
         "content-only": directives.flag,  # TODO: Implement
         "inner": directives.flag,  # TODO: Implement
         "skip-xml-nodes": directives.unchanged,
     }
 
     def run(self) -> List[Node]:
         name = self.arguments[0]
-        project = self.options.get("project", self.app.config.docleaf_default_project)
-        path = self.app.config.docleaf_projects[project]
+        project_name = self.options.get("project", self.app.config.docleaf_default_project)
+        project = self.app.config.docleaf_projects[project_name]
 
         skip_settings = get_skip_settings(self.app, self.options)
         content_only = "content-only" in self.options
         inner_group = "inner" in self.options
         context = backend.Context(
+            project["root"],
             skip_settings,
             self.app.config.docleaf_domain_by_extension,
         )
 
         tracked_cache = backend.TrackedCache(self.cache)
         node_list = backend.render_group(
             name,
-            path,
+            project["xml"],
             context,
             content_only,
             inner_group,
             tracked_cache,
         )
         update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
```

## Comparing `docleaf-0.3.0.dist-info/METADATA` & `docleaf-0.4.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,51 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.3.0
+Version: 0.4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Sphinx :: Extension
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Documentation
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,<6,!=5.0.0
 License-File: LICENSE.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
-Author: Michael Jones
+Keywords: sphinx,doxygen
+Author-email: Michael Jones <michael.jones@docleaf.io>
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
 Project-URL: repository, https://github.com/docleaf-labs/docleaf
+Project-URL: homepage, https://docleaf.io
 
-
-# Docleaf
+<h1 align="center">
+  Docleaf
+</h1>
+
+<p align="center">
+   Your technical docs, beautifully integrated
+</p>
 
 Docleaf smoothly integrates your technical and long-form documentation. It is a Sphinx extension which reads Doxygen
 XML output and formats the information seamlessly with your user documentation.
 
 ## License
 
 Docleaf is licensed under the [Parity Public License](./LICENSE.md). The Parity license allows permissive use of 
 Docleaf to help document open source projects. If you have a closed source project that you would like to document with
-Docleaf then you must purchase a commercial license. For further information please email
-[support@docleaf.io](mailto:support@docleaf.io).
+Docleaf then you must purchase a commercial license.
+
+For further information please email: [support@docleaf.io](mailto:support@docleaf.io)
+
+## Features
+
+- Custom directives allowing you to target various parts of C and C++ code bases.
+- Integration with Sphinx C and C++ domains to support easily linking to your generated output.
+- Integration with the `sphinx.ext.linkcode` extension to support links to source code locations in a GitHub
+  repository.
 
 ## Installation
 
 Docleaf can be installed from [PyPI](https://pypi.org/project/docleaf/):
 
 ```
 pip install docleaf
@@ -34,20 +55,24 @@
 
 Include `docleaf.doxygen` as an extension in your Sphinx `conf.py` file:
 
 ```python
 extensions = ["docleaf.doxygen"]
 ```
 
-Configure the extenion to know where the Doxygen XML output has been generated for your project and optionally set the
-default project:
+Configure the extension to know where your source code is stored and the Doxygen XML output has been generated for
+your project. Optionally set the default project:
 
 ```python
 docleaf_projects = {
-  "my_project": "../doxygen/xml"
+  "my_project": {
+    "root": "../src",
+    "xml": "../doxygen/xml"
+  }
+
 }
 docleaf_default_project = "my_project"
 ```
 
 The use the provided directives in your reStructuredText files:
 
 ```rst
@@ -84,19 +109,22 @@
 
 Generate documentation for specific group as specified within your Doxygen set up and code comments.
 
 ```rst
 .. doxygengroup:: group_name
 ```
 
+All directives take a `:project:` option to specify the project to use from your `conf.py` if you don't want to use
+the default project.
+
 ### Settings
 
 - `docleaf_projects` 
 
-  A Python dictionary mapping each project name to the folder where its Doxygen XML output is stored.
+  A Python dictionary mapping each project name to the folders where its source code and Doxygen XML output are stored.
 
 - `docleaf_default_project`
 
   The default project to use when none is specified on the directive itself.
   
 - `docleaf_domain_by_extension`
 
@@ -118,14 +146,44 @@
 
   - `members:all_caps` - Skips any function or variable members (as defined as a 'memberdef' by Doxygen) which have 
     names which are all capital letters and underscores. This is to allow users to filter our unprocessed C/C++ macros
     if desirable.
   - `xml-nodes:<node name>` - Skips reading and process of the given XML node and its children in the Doxygen XML 
     output. Support is limited to the `htmlonly` node.
 
+### Integration with `sphinx.ext.linkcode`
+
+Docleaf can integrate with the `sphinx.ext.linkcode` extension in order to add `[source]` links next to various
+supported entries in your documentation. Linking to GitHub based repositories is supported.
+
+In order to use it, add the `sphinx.ext.linkcode` extension to the `extensions` list in your Sphinx `conf.py` and use
+the `docleaf.doxygen.GitHubLinkResolver` with appropriate parameters for your repository.
+
+```python
+extensions = [
+  "docleaf.doxygen",
+  "sphinx.ext.linkcode",
+  ]
+
+linkcode_resolve = docleaf.doxygen.GitHubLinkResolver(
+    root="../../../", user="docleaf-labs", repo="docleaf", branch="main"
+)
+```
+
+Where:
+- `root` is the relative path to the root of your repository.
+- `user` is the user or organisation name for your GitHub repository.
+- `repo` is the name of your GitHub repository.
+- `tag` is the git tag that you would like the generated link URLs to target.
+- `branch` is the git branch that you would like the generated link URLs to target.
+- `commit` is the git commit SHA that you would like the generated link URLs to target.
+
+Only one of `tag`, `branch` and `commit` is necessary.
+
+
 ## Performance
 
 When doing a clean build of the Zephyr RTOS documentation suite, Docleaf is 2.1x faster than Breathe.
 
 ```
 Benchmark: docleaf
   Time (mean ± σ):     180.383 s ±  3.213 s    [User: 448.242 s, System: 12.908 s]
@@ -138,9 +196,9 @@
   Range (min … max):   379.093 s … 394.315 s    10 runs
 ```
 
 ## History
 
 Docleaf is written and maintained by the creator of the [Breathe](https://github.com/breathe-doc/breathe) project.
 It was created to resolve some of the performance and memory consumption issues with Breathe by re-writing the code
-base to use Rust. The user experience is designed to match Breathe.
+base to use Rust. The user experience is designed to match and improve on Breathe.
```

## Comparing `docleaf-0.3.0.dist-info/license_files/LICENSE.md` & `docleaf-0.4.0.dist-info/license_files/LICENSE.md`

 * *Files identical despite different names*

## Comparing `docleaf-0.3.0.dist-info/RECORD` & `docleaf-0.4.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-docleaf-0.3.0.dist-info/METADATA,sha256=Fh17ag_4xvsnhT8ilPge7lbOfBdJ59TYZYYQUI2hIyE,4459
-docleaf-0.3.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
-docleaf-0.3.0.dist-info/license_files/LICENSE.md,sha256=ffIj5xgqX0xL1nd3_5YbHFc3paR7y61W6f1780Gp3lE,3573
-docleaf/copied.py,sha256=fIQgdMKJYpQbE08lNhe7Xva9sN-pRgK6ZGj2ABM_EN4,3774
-docleaf/domains.py,sha256=6zPyDrgK53W20lOZdwJWAGwrsIMaZ44YlXhIl2hcKhc,2954
-docleaf/doxygen.py,sha256=9Pq1Gu-O0_E0Qoupi3Z20TsVhFf7wRHGerVgbdmeDtw,17005
+docleaf-0.4.0.dist-info/METADATA,sha256=V6uzWbe5qKkDJ76LL9wFfLMQNtmz5Y4oWKR9711rJMc,6708
+docleaf-0.4.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+docleaf-0.4.0.dist-info/license_files/LICENSE.md,sha256=ffIj5xgqX0xL1nd3_5YbHFc3paR7y61W6f1780Gp3lE,3573
+docleaf/copied.py,sha256=YRObp4s8bDjbMZJFQD36HyLkx64U35QkUsb3MCf4tPs,3836
+docleaf/domains.py,sha256=5My3c04BEfWSBngVYiZqgxvkh_F09GfEmzgKiJkOa0o,3709
+docleaf/doxygen.py,sha256=80Wo24pfOuP228OEy90xYF0BIYjswNR_rd5fjS4FljM,18910
 docleaf/errors.py,sha256=sUYIqy64k8zKQ-cZjVzF6auax0klQ9FibFmKOCD9v2Y,99
 docleaf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-docleaf/backend.cp39-win_amd64.pyd,sha256=VRB5Jjr7d-kDEK4d-C_wKZTa5CBRinpBqmZFuT90HRA,3038208
-docleaf-0.3.0.dist-info/RECORD,,
+docleaf/backend.cp39-win_amd64.pyd,sha256=euLzJmc-4_hU7ZgAVfRN5jk8MfrFkEHF0DKBENWIPBo,3051520
+docleaf-0.4.0.dist-info/RECORD,,
```

