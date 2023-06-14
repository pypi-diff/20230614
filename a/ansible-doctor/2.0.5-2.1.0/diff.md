# Comparing `tmp/ansible_doctor-2.0.5.tar.gz` & `tmp/ansible_doctor-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_doctor-2.0.5.tar", max compression
+gzip compressed data, was "ansible_doctor-2.1.0.tar", max compression
```

## Comparing `ansible_doctor-2.0.5.tar` & `ansible_doctor-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    32460 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/LICENSE
--rw-r--r--   0        0        0     2754 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/README.md
--rw-r--r--   0        0        0       58 2023-05-29 20:03:30.783262 ansible_doctor-2.0.5/ansibledoctor/__init__.py
--rw-r--r--   0        0        0     6263 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/annotation.py
--rw-r--r--   0        0        0     4038 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/cli.py
--rw-r--r--   0        0        0    11842 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/config.py
--rw-r--r--   0        0        0      120 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/contstants.py
--rw-r--r--   0        0        0     7204 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/doc_generator.py
--rw-r--r--   0        0        0     5952 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/doc_parser.py
--rw-r--r--   0        0        0      472 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/exception.py
--rw-r--r--   0        0        0     1734 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/file_registry.py
--rw-r--r--   0        0        0      377 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_meta.j2
--rw-r--r--   0        0        0      173 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_requirements.j2
--rw-r--r--   0        0        0      318 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_tag.j2
--rw-r--r--   0        0        0      371 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_toc.j2
--rw-r--r--   0        0        0      583 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_todo.j2
--rw-r--r--   0        0        0      935 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_vars.j2
--rw-r--r--   0        0        0      847 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/index.md.j2
--rw-r--r--   0        0        0      696 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/README.md.j2
--rw-r--r--   0        0        0      691 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_meta.j2
--rw-r--r--   0        0        0      173 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_requirements.j2
--rw-r--r--   0        0        0      365 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_tag.j2
--rw-r--r--   0        0        0      434 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_toc.j2
--rw-r--r--   0        0        0      583 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_todo.j2
--rw-r--r--   0        0        0      935 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/templates/readme/_vars.j2
--rw-r--r--   0        0        0     9272 2023-05-29 20:02:56.683735 ansible_doctor-2.0.5/ansibledoctor/utils.py
--rw-r--r--   0        0        0     3359 2023-05-29 20:03:30.783262 ansible_doctor-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 ansible_doctor-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    32460 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2754 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/README.md
+-rw-r--r--   0        0        0       58 2023-06-14 19:06:22.470900 ansible_doctor-2.1.0/ansibledoctor/__init__.py
+-rw-r--r--   0        0        0     6263 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/annotation.py
+-rw-r--r--   0        0        0     4038 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/cli.py
+-rw-r--r--   0        0        0    12019 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/config.py
+-rw-r--r--   0        0        0      120 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/contstants.py
+-rw-r--r--   0        0        0     7294 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/doc_generator.py
+-rw-r--r--   0        0        0     5952 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/doc_parser.py
+-rw-r--r--   0        0        0      472 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/exception.py
+-rw-r--r--   0        0        0     1734 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/file_registry.py
+-rw-r--r--   0        0        0      377 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_meta.j2
+-rw-r--r--   0        0        0      173 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_requirements.j2
+-rw-r--r--   0        0        0      318 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_tag.j2
+-rw-r--r--   0        0        0      371 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_toc.j2
+-rw-r--r--   0        0        0      583 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_todo.j2
+-rw-r--r--   0        0        0     1560 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_vars.j2
+-rw-r--r--   0        0        0      847 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/index.md.j2
+-rw-r--r--   0        0        0      696 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/README.md.j2
+-rw-r--r--   0        0        0      691 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/_meta.j2
+-rw-r--r--   0        0        0      173 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/_requirements.j2
+-rw-r--r--   0        0        0      365 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/_tag.j2
+-rw-r--r--   0        0        0      434 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/_toc.j2
+-rw-r--r--   0        0        0      583 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/_todo.j2
+-rw-r--r--   0        0        0     1560 2023-06-14 19:06:08.326843 ansible_doctor-2.1.0/ansibledoctor/templates/readme/_vars.j2
+-rw-r--r--   0        0        0     9272 2023-06-14 19:06:08.330843 ansible_doctor-2.1.0/ansibledoctor/utils.py
+-rw-r--r--   0        0        0     3359 2023-06-14 19:06:22.466900 ansible_doctor-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 ansible_doctor-2.1.0/PKG-INFO
```

### Comparing `ansible_doctor-2.0.5/LICENSE` & `ansible_doctor-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/README.md` & `ansible_doctor-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/annotation.py` & `ansible_doctor-2.1.0/ansibledoctor/annotation.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/cli.py` & `ansible_doctor-2.1.0/ansibledoctor/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/config.py` & `ansible_doctor-2.1.0/ansibledoctor/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,20 @@
         },
         "template": {
             "default": "readme",
             "env": "TEMPLATE",
             "file": True,
             "type": environs.Env().str
         },
+        "template_autotrim": {
+            "default": True,
+            "env": "TEMPLATE_AUTOTRIM",
+            "file": True,
+            "type": environs.Env().bool
+        },
         "force_overwrite": {
             "default": False,
             "env": "FORCE_OVERWRITE",
             "file": True,
             "type": environs.Env().bool
         },
         "custom_header": {
```

### Comparing `ansible_doctor-2.0.5/ansibledoctor/doc_generator.py` & `ansible_doctor-2.1.0/ansibledoctor/doc_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,17 @@
 
     @pass_eval_context
     def _safe_join(self, eval_ctx, value, d=""):
         if isinstance(value, str):
             value = [value]
 
         normalized = jinja2.filters.do_join(eval_ctx, value, d, attribute=None)
-        for s in [r" +(\n|\t| )", r"(\n|\t) +"]:
-            normalized = re.sub(s, "\\1", normalized)
 
-        return normalized
+        if self.config.config["template_autotrim"]:
+            for s in [r" +(\n|\t| )", r"(\n|\t) +"]:
+                normalized = re.sub(s, "\\1", normalized)
+
+        return jinja2.filters.do_mark_safe(normalized)
 
     def render(self):
         self.logger.info(f"Using output dir: {self.config.config.get('output_dir')}")
         self._write_doc()
```

### Comparing `ansible_doctor-2.0.5/ansibledoctor/doc_parser.py` & `ansible_doctor-2.1.0/ansibledoctor/doc_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/file_registry.py` & `ansible_doctor-2.1.0/ansibledoctor/file_registry.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/_todo.j2` & `ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/templates/hugo-book/index.md.j2` & `ansible_doctor-2.1.0/ansibledoctor/templates/hugo-book/index.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/templates/readme/README.md.j2` & `ansible_doctor-2.1.0/ansibledoctor/templates/readme/README.md.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/templates/readme/_meta.j2` & `ansible_doctor-2.1.0/ansibledoctor/templates/readme/_meta.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/templates/readme/_todo.j2` & `ansible_doctor-2.1.0/ansibledoctor/templates/readme/_todo.j2`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/ansibledoctor/utils.py` & `ansible_doctor-2.1.0/ansibledoctor/utils.py`

 * *Files identical despite different names*

### Comparing `ansible_doctor-2.0.5/pyproject.toml` & `ansible_doctor-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,35 +29,35 @@
 license = "GPL-3.0-only"
 name = "ansible-doctor"
 packages = [
   {include = "ansibledoctor"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/ansible-doctor/"
-version = "2.0.5"
+version = "2.1.0"
 
 [tool.poetry.dependencies]
 Jinja2 = "3.1.2"
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
 colorama = "0.4.6"
 environs = "9.5.0"
 jsonschema = "4.17.3"
 nested-lookup = "0.2.25"
 pathspec = "0.11.1"
 python = "^3.7.0"
 python-json-logger = "2.0.7"
-"ruamel.yaml" = "0.17.28"
+"ruamel.yaml" = "0.17.31"
 
 [tool.poetry.scripts]
 ansible-doctor = "ansibledoctor.cli:main"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.0.270"
-pytest = "7.3.1"
+ruff = "0.0.272"
+pytest = "7.3.2"
 pytest-mock = "3.10.0"
 pytest-cov = "4.1.0"
 toml = "0.10.2"
 yapf = "0.33.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `ansible_doctor-2.0.5/PKG-INFO` & `ansible_doctor-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-doctor
-Version: 2.0.5
+Version: 2.1.0
 Summary: Generate documentation from annotated Ansible roles using templates.
 Home-page: https://ansible-doctor.geekdocs.de/
 License: GPL-3.0-only
 Keywords: ansible,role,documentation
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.7.0,<4.0.0
@@ -30,15 +30,15 @@
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.6)
 Requires-Dist: environs (==9.5.0)
 Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: pathspec (==0.11.1)
 Requires-Dist: python-json-logger (==2.0.7)
-Requires-Dist: ruamel.yaml (==0.17.28)
+Requires-Dist: ruamel.yaml (==0.17.31)
 Project-URL: Documentation, https://ansible-doctor.geekdocs.de/
 Project-URL: Repository, https://github.com/thegeeklab/ansible-doctor/
 Description-Content-Type: text/markdown
 
 # ansible-doctor
 
 Annotation based documentation for your Ansible roles
```

