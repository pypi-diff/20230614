# Comparing `tmp/dsp_tools-2.3.2.tar.gz` & `tmp/dsp_tools-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.3.2.tar", max compression
+gzip compressed data, was "dsp_tools-2.3.3.tar", max compression
```

## Comparing `dsp_tools-2.3.2.tar` & `dsp_tools-2.3.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-06-01 06:56:39.377437 dsp_tools-2.3.2/LICENSE
--rw-r--r--   0        0        0     4373 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/docs/index.md
--rw-r--r--   0        0        0     4836 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    20257 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    88414 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/__init__.py
--rw-r--r--   0        0        0    29382 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/process_files.py
--rw-r--r--   0        0        0    14418 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_files.py
--rw-r--r--   0        0        0     4173 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_xml.py
--rw-r--r--   0        0        0        0 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      962 2023-06-01 06:56:39.393438 dsp_tools-2.3.2/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     9760 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3197 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     9538 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16915 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     9810 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    23066 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      506 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    19744 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2972 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    19128 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1930 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    21129 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1896 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    22134 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    34527 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      419 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0      890 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    27302 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    34725 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     2153 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      747 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0      254 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlerror.py
--rw-r--r--   0        0        0     1841 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2371 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8874 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2614 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0     1488 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23543 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0     2867 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0        0 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15096 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4828 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     7818 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10202 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3174 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0     1157 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/logging.py
--rw-r--r--   0        0        0    40900 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8057 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4617 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18724 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4242 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    12854 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0     6830 2023-06-01 06:56:39.397438 dsp_tools-2.3.2/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    51156 2023-06-01 06:56:39.401439 dsp_tools-2.3.2/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 dsp_tools-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-14 06:25:24.712451 dsp_tools-2.3.3/LICENSE
+-rw-r--r--   0        0        0     4373 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/docs/index.md
+-rw-r--r--   0        0        0     4850 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    20433 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    89229 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    31627 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14293 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4185 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      929 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     9662 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3325 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     9470 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16545 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     9798 2023-06-14 06:25:24.728452 dsp_tools-2.3.3/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    22159 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      506 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    17509 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2956 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    18974 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1914 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    21045 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1897 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    21692 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    34024 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      419 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0      919 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    27078 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    33467 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     2151 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      747 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1841 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2373 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8943 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2613 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0        0 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23543 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42584 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32171 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0     2526 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0        0 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15315 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4886 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     8237 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10530 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3189 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0     1134 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/logging.py
+-rw-r--r--   0        0        0    41163 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8371 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4689 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18807 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4259 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    12793 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0     6988 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    51652 2023-06-14 06:25:24.732452 dsp_tools-2.3.3/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 dsp_tools-2.3.3/PKG-INFO
```

### Comparing `dsp_tools-2.3.2/LICENSE` & `dsp_tools-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/docs/index.md` & `dsp_tools-2.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/pyproject.toml` & `dsp_tools-2.3.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.3.2"
+version = "2.3.3"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 documentation = "https://docs.dasch.swiss/latest/DSP-TOOLS/"
 homepage = "https://www.dasch.swiss/"
 repository = "https://github.com/dasch-swiss/dsp-tools"
-include = ["src/dsp_tools/resources/*"]
+include = [
+    "src/dsp_tools/resources/*",
+    "src/dsp_tools/py.typed"  # see https://mypy.readthedocs.io/en/stable/installed_packages.html#making-pep-561-compatible-packages
+]
 exclude = ["src/dsp_tools/import_scripts/*"]
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = "^3.9"
 jsonpath-ng = "^1.5.3"
 argparse = "^1.4.0"
 lxml = "^4.9.2"
 requests = "^2.30.0"
 jsonschema = "^4.17.3"
 openpyxl = "^3.1.2"
 networkx = "^3.1.0"
 pandas = { version = "^2.0.1", extras = ["excel"] }  # extra package that contains xlrd that is necessary for reading old .xls Excel files
 regex = "^2023.5.5"
 docker = "^6.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.11"
 mkdocs-include-markdown-plugin = "^4.0.4"
 mypy = "^1.3.0"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
 types-requests = "^2.30.0.0"
@@ -75,26 +79,25 @@
 strict = true
 exclude = [
     "src/dsp_tools/models",                # TODO: activate this
     "src/dsp_tools/import_scripts",        # TODO: activate this
 ]
 
 
-[tool.isort]
-multi_line_output = 3
-known_first_party = ["dsp_tools"]
+[tool.black]
+line-length = 120
 
 
 [tool.pylint.MASTER]
 ignore-paths = ["src/dsp_tools/models/.*$"] # TODO: activate this
 suggestion-mode = true
 
 
 [tool.pylint.format]
-max-line-length = 150
+max-line-length = 120
 
 
 [tool.pylint."messages control"]
 disable = [
     "raw-checker-failed",                  # disabled by default
     "bad-inline-option",                   # disabled by default
     "locally-disabled",                    # disabled by default
@@ -117,9 +120,8 @@
     "too-many-arguments",                  # TODO: activate this
     "too-many-branches",                   # TODO: activate this
     "too-many-lines",                      # TODO: activate this
     "too-many-locals",                     # TODO: activate this
     "too-many-nested-blocks",              # TODO: activate this
     "too-many-return-statements",          # TODO: activate this
     "too-many-statements",                 # TODO: activate this
-    "consider-using-f-string",             # in excel2xml, strings with {} in it must be formatted
 ]
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/dsp_tools.py` & `dsp_tools-2.3.3/src/dsp_tools/dsp_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 from importlib.metadata import version
 
 from dsp_tools.excel2xml import excel2xml
 from dsp_tools.fast_xmlupload.process_files import process_files
 from dsp_tools.fast_xmlupload.upload_files import upload_files
 from dsp_tools.fast_xmlupload.upload_xml import fast_xmlupload
 from dsp_tools.models.exceptions import UserError
-from dsp_tools.utils.excel_to_json_lists import (
-    excel2lists,
-    validate_lists_section_with_schema
-)
+from dsp_tools.utils.excel_to_json_lists import excel2lists, validate_lists_section_with_schema
 from dsp_tools.utils.excel_to_json_project import excel2json
 from dsp_tools.utils.excel_to_json_properties import excel2properties
 from dsp_tools.utils.excel_to_json_resources import excel2resources
 from dsp_tools.utils.generate_templates import generate_template_repo
 from dsp_tools.utils.id_to_iri import id_to_iri
 from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.project_create import create_project
@@ -50,182 +47,222 @@
     # default values
     default_dsp_api_url = "http://0.0.0.0:3333"
     default_user = "root@example.com"
     default_pw = "test"
     default_sipi = "http://0.0.0.0:1024"
 
     # make a parser
-    parser = argparse.ArgumentParser(description=f"DSP-TOOLS (version {version('dsp-tools')}, © {datetime.datetime.now().year} by DaSCH)")
-    subparsers = parser.add_subparsers(title="Subcommands", description="Valid subcommands are", help="sub-command help")
+    parser = argparse.ArgumentParser(
+        description=f"DSP-TOOLS (version {version('dsp-tools')}, © {datetime.datetime.now().year} by DaSCH)"
+    )
+    subparsers = parser.add_subparsers(
+        title="Subcommands", description="Valid subcommands are", help="sub-command help"
+    )
 
     # create
     parser_create = subparsers.add_parser(
         name="create",
         help="Create a project defined in a JSON project file on a DSP server. "
-             "A project can consist of lists, groups, users, and ontologies (data models)."
+        "A project can consist of lists, groups, users, and ontologies (data models).",
     )
     parser_create.set_defaults(action="create")
     parser_create.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_create.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_create.add_argument("-p", "--password", default=default_pw, help=password_text)
-    parser_create.add_argument("-V", "--validate-only", action="store_true",
-                               help="validate the JSON file without creating it on the DSP server")
-    parser_create.add_argument("-l", "--lists-only", action="store_true",
-                               help="create only the lists (prerequisite: the project exists on the server)")
+    parser_create.add_argument(
+        "-V",
+        "--validate-only",
+        action="store_true",
+        help="validate the JSON file without creating it on the DSP server",
+    )
+    parser_create.add_argument(
+        "-l",
+        "--lists-only",
+        action="store_true",
+        help="create only the lists (prerequisite: the project exists on the server)",
+    )
     parser_create.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_create.add_argument("-d", "--dump", action="store_true", help="dump test files for DSP-API requests")
     parser_create.add_argument("project_definition", help="path to the JSON project file")
 
     # get
-    parser_get = subparsers.add_parser(name="get", help="Retrieve a project with its data model(s) from a DSP server and write it into a JSON file")
+    parser_get = subparsers.add_parser(
+        name="get",
+        help="Retrieve a project with its data model(s) from a DSP server and write it into a JSON file",
+    )
     parser_get.set_defaults(action="get")
     parser_get.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_get.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_get.add_argument("-p", "--password", default=default_pw, help=password_text)
     parser_get.add_argument("-P", "--project", help="shortcode, shortname or IRI of the project", required=True)
     parser_get.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_get.add_argument("project_definition", help="path to the file the project should be written to")
 
     # xmlupload
     parser_upload = subparsers.add_parser(name="xmlupload", help="Upload data defined in an XML file to a DSP server")
     parser_upload.set_defaults(action="xmlupload")
-    parser_upload.add_argument("-s", "--server", default=default_dsp_api_url, help="URL of the DSP server where DSP-TOOLS sends the data to")
+    parser_upload.add_argument(
+        "-s", "--server", default=default_dsp_api_url, help="URL of the DSP server where DSP-TOOLS sends the data to"
+    )
     parser_upload.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_upload.add_argument("-p", "--password", default=default_pw, help=password_text)
-    parser_upload.add_argument("-S", "--sipi", default=default_sipi,
-                               help="URL of the SIPI server where DSP-TOOLS sends the multimedia files to")
-    parser_upload.add_argument("-i", "--imgdir", default=".", help="folder from where the paths in the <bitstream> tags are evaluated")
-    parser_upload.add_argument("-I", "--incremental", action="store_true",
-                               help="The links in the XML file point to IRIs (on the server) instead of IDs (in the same XML file).")
-    parser_upload.add_argument("-V", "--validate", action="store_true", help="validate the XML file without uploading it")
+    parser_upload.add_argument(
+        "-S",
+        "--sipi",
+        default=default_sipi,
+        help="URL of the SIPI server where DSP-TOOLS sends the multimedia files to",
+    )
+    parser_upload.add_argument(
+        "-i", "--imgdir", default=".", help="folder from where the paths in the <bitstream> tags are evaluated"
+    )
+    parser_upload.add_argument(
+        "-I",
+        "--incremental",
+        action="store_true",
+        help="The links in the XML file point to IRIs (on the server) instead of IDs (in the same XML file).",
+    )
+    parser_upload.add_argument(
+        "-V", "--validate", action="store_true", help="validate the XML file without uploading it"
+    )
     parser_upload.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_upload.add_argument("-m", "--metrics", action="store_true", help="write metrics into a 'metrics' folder")
     parser_upload.add_argument("xmlfile", help="path to the XML file containing the data")
 
     # process-files
     parser_process_files = subparsers.add_parser(
         name="process-files",
-        help="For internal use only: process all files referenced in an XML file"
+        help="For internal use only: process all files referenced in an XML file",
     )
     parser_process_files.set_defaults(action="process-files")
-    parser_process_files.add_argument("--input-dir", help="path to the input directory where the files should be read from")
-    parser_process_files.add_argument("--output-dir", help="path to the output directory where the processed/transformed files should be written to")
+    parser_process_files.add_argument(
+        "--input-dir", help="path to the input directory where the files should be read from"
+    )
+    parser_process_files.add_argument(
+        "--output-dir", help="path to the output directory where the processed/transformed files should be written to"
+    )
     parser_process_files.add_argument("--nthreads", type=int, default=None, help="number of threads to use")
     parser_process_files.add_argument("xml_file", help="path to XML file containing the data")
 
     # upload-files
     parser_upload_files = subparsers.add_parser(
         name="upload-files",
-        help="For internal use only: upload already processed files"
+        help="For internal use only: upload already processed files",
     )
     parser_upload_files.set_defaults(action="upload-files")
     parser_upload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
     parser_upload_files.add_argument("-d", "--processed-dir", help="path to the directory with the processed files")
     parser_upload_files.add_argument("-n", "--nthreads", type=int, default=4, help="number of threads to use")
     parser_upload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_upload_files.add_argument("-S", "--sipi-url", default=default_sipi, help=sipi_text)
     parser_upload_files.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_upload_files.add_argument("-p", "--password", default=default_pw, help=password_text)
 
     # fast-xmlupload
     parser_fast_xmlupload_files = subparsers.add_parser(
         name="fast-xmlupload",
-        help="For internal use only: create resources with already uploaded files"
+        help="For internal use only: create resources with already uploaded files",
     )
     parser_fast_xmlupload_files.set_defaults(action="fast-xmlupload")
     parser_fast_xmlupload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
     parser_fast_xmlupload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_fast_xmlupload_files.add_argument("-S", "--sipi-url", default=default_sipi, help=sipi_text)
     parser_fast_xmlupload_files.add_argument("-u", "--user", default=default_user, help=username_text)
     parser_fast_xmlupload_files.add_argument("-p", "--password", default=default_pw, help=password_text)
     parser_fast_xmlupload_files.add_argument("xml_file", help="path to XML file containing the data")
 
     # excel2json
     parser_excel2json = subparsers.add_parser(
         name="excel2json",
-        help="Create an entire JSON project file from a folder containing the required Excel files"
+        help="Create an entire JSON project file from a folder containing the required Excel files",
     )
     parser_excel2json.set_defaults(action="excel2json")
     parser_excel2json.add_argument("excelfolder", help="path to the folder containing the Excel files")
     parser_excel2json.add_argument("project_definition", help="path to the output JSON file")
 
     # excel2lists
     parser_excel_lists = subparsers.add_parser(
         name="excel2lists",
-        help="Create the 'lists' section of a JSON project file from one or multiple Excel files"
+        help="Create the 'lists' section of a JSON project file from one or multiple Excel files",
     )
     parser_excel_lists.set_defaults(action="excel2lists")
     parser_excel_lists.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_excel_lists.add_argument("excelfolder", help="path to the folder containing the Excel file(s)")
     parser_excel_lists.add_argument("lists_section", help="path to the output JSON file containing the 'lists' section")
 
     # excel2resources
     parser_excel_resources = subparsers.add_parser(
         name="excel2resources",
-        help="Create the 'resources' section of a JSON project file from one or multiple Excel files"
+        help="Create the 'resources' section of a JSON project file from one or multiple Excel files",
     )
     parser_excel_resources.set_defaults(action="excel2resources")
     parser_excel_resources.add_argument("excelfile", help="path to the Excel file containing the resources")
-    parser_excel_resources.add_argument("resources_section", help="path to the output JSON file containing the 'resources' section")
+    parser_excel_resources.add_argument(
+        "resources_section", help="path to the output JSON file containing the 'resources' section"
+    )
 
     # excel2properties
     parser_excel_properties = subparsers.add_parser(
         name="excel2properties",
-        help="Create the 'properties' section of a JSON project file from one or multiple Excel files"
+        help="Create the 'properties' section of a JSON project file from one or multiple Excel files",
     )
     parser_excel_properties.set_defaults(action="excel2properties")
     parser_excel_properties.add_argument("excelfile", help="path to the Excel file containing the properties")
-    parser_excel_properties.add_argument("properties_section", help="path to the output JSON file containing the 'properties' section")
+    parser_excel_properties.add_argument(
+        "properties_section", help="path to the output JSON file containing the 'properties' section"
+    )
 
     # excel2xml
     parser_excel2xml = subparsers.add_parser(
         name="excel2xml",
-        help="Create an XML file from an Excel/CSV file that is already structured according to the DSP specifications"
+        help="Create an XML file from an Excel/CSV file that is already structured according to the DSP specifications",
     )
     parser_excel2xml.set_defaults(action="excel2xml")
     parser_excel2xml.add_argument("data_source", help="path to the CSV or XLS(X) file containing the data")
     parser_excel2xml.add_argument("project_shortcode", help="shortcode of the project that this data belongs to")
     parser_excel2xml.add_argument("ontology_name", help="name of the ontology that this data belongs to")
 
     # id2iri
     parser_id2iri = subparsers.add_parser(
         name="id2iri",
-        help="Replace internal IDs in contained in the <resptr> tags of an XML file by IRIs provided in a mapping file"
+        help="Replace internal IDs in contained in the <resptr> tags of an XML file by IRIs provided in a mapping file",
     )
     parser_id2iri.set_defaults(action="id2iri")
     parser_id2iri.add_argument("--outfile", help="path to the XML output file containing the replaced IDs")
     parser_id2iri.add_argument("-v", "--verbose", action="store_true", help=verbose_text)
     parser_id2iri.add_argument("xmlfile", help="path to the XML file containing the data to be replaced")
     parser_id2iri.add_argument("mapping", help="path to the JSON file containing the mapping of IDs to IRIs")
 
     # startup DSP stack
     parser_stackup = subparsers.add_parser(name="start-stack", help="Run a local instance of DSP-API and DSP-APP")
     parser_stackup.set_defaults(action="start-stack")
-    parser_stackup.add_argument("--max_file_size", type=int, help="max. multimedia file size allowed by SIPI, in MB (default: 250, max: 100'000)")
+    parser_stackup.add_argument(
+        "--max_file_size",
+        type=int,
+        help="max. multimedia file size allowed by SIPI, in MB (default: 250, max: 100'000)",
+    )
     parser_stackup.add_argument("--prune", action="store_true", help="execute 'docker system prune' without asking")
-    parser_stackup.add_argument("--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)")
+    parser_stackup.add_argument(
+        "--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)"
+    )
 
     # shutdown DSP-API
     parser_stackdown = subparsers.add_parser(
-        name="stop-stack",
-        help="Shut down the local instance of DSP-API and DSP-APP, and delete all data in it"
+        name="stop-stack", help="Shut down the local instance of DSP-API and DSP-APP, and delete all data in it"
     )
     parser_stackdown.set_defaults(action="stop-stack")
 
     # create template repo with minimal JSON and XML files
     parser_template = subparsers.add_parser(
-        name="template",
-        help="Create a template repository with a minimal JSON and XML file"
+        name="template", help="Create a template repository with a minimal JSON and XML file"
     )
     parser_template.set_defaults(action="template")
 
     # clone rosetta
     parser_rosetta = subparsers.add_parser(
-        name="rosetta",
-        help="Clone the most up to data rosetta repository, create the data model and upload the data"
+        name="rosetta", help="Clone the most up to data rosetta repository, create the data model and upload the data"
     )
     parser_rosetta.set_defaults(action="rosetta")
 
     return parser
 
 
 def _log_cli_arguments(parsed_args: argparse.Namespace) -> None:
@@ -243,27 +280,27 @@
         if key == "password":
             lines.append(f"***   {key:<{longest_key_length}} = {'*' * len(value)}")
         else:
             lines.append(f"***   {key:<{longest_key_length}} = {value}")
     if not lines:
         lines.append("***   (no parameters)")
     asterisk_count = max(
-        len(msg), 
-        max(len(line) for line in lines)
+        len(msg),
+        max(len(line) for line in lines),
     )
     logger.info("*" * asterisk_count)
     logger.info(msg)
     for line in lines:
         logger.info(line)
     logger.info("*" * asterisk_count)
 
 
 def call_requested_action(
     user_args: list[str],
-    parser: argparse.ArgumentParser
+    parser: argparse.ArgumentParser,
 ) -> bool:
     """
     With the help of the parser, parse the user arguments and call the appropriate method of DSP-TOOLS.
 
     Args:
         user_args: list of arguments passed by the user from the command line
         parser: parser to parse the user arguments
@@ -290,37 +327,37 @@
                 print("'Lists' section of the JSON project file is syntactically correct and passed validation.")
             else:
                 _, success = create_lists(
                     project_file_as_path_or_parsed=args.project_definition,
                     server=args.server,
                     user=args.user,
                     password=args.password,
-                    dump=args.dump
+                    dump=args.dump,
                 )
         else:
             if args.validate_only:
                 success = validate_project(args.project_definition)
                 print("JSON project file is syntactically correct and passed validation.")
             else:
                 success = create_project(
                     project_file_as_path_or_parsed=args.project_definition,
                     server=args.server,
                     user_mail=args.user,
                     password=args.password,
                     verbose=args.verbose,
-                    dump=args.dump
+                    dump=args.dump,
                 )
     elif args.action == "get":
         success = get_project(
             project_identifier=args.project,
             outfile_path=args.project_definition,
             server=args.server,
             user=args.user,
             password=args.password,
-            verbose=args.verbose
+            verbose=args.verbose,
         )
     elif args.action == "xmlupload":
         if args.validate:
             success = validate_xml_against_schema(input_file=args.xmlfile)
         else:
             success = xml_upload(
                 input_file=args.xmlfile,
@@ -328,82 +365,82 @@
                 user=args.user,
                 password=args.password,
                 imgdir=args.imgdir,
                 sipi=args.sipi,
                 verbose=args.verbose,
                 incremental=args.incremental,
                 save_metrics=args.metrics,
-                preprocessing_done=False
+                preprocessing_done=False,
             )
 
     elif args.action == "process-files":
         success = process_files(
             input_dir=args.input_dir,
             output_dir=args.output_dir,
             xml_file=args.xml_file,
-            nthreads=args.nthreads
+            nthreads=args.nthreads,
         )
     elif args.action == "upload-files":
         success = upload_files(
             pkl_file=args.pkl_file,
             dir_with_processed_files=args.processed_dir,
             nthreads=args.nthreads,
             user=args.user,
             password=args.password,
             dsp_url=args.server,
-            sipi_url=args.sipi_url
+            sipi_url=args.sipi_url,
         )
     elif args.action == "fast-xmlupload":
         success = fast_xmlupload(
             xml_file=args.xml_file,
             pkl_file=args.pkl_file,
             user=args.user,
             password=args.password,
             dsp_url=args.server,
-            sipi_url=args.sipi_url
+            sipi_url=args.sipi_url,
         )
     elif args.action == "excel2json":
         success = excel2json(
             data_model_files=args.excelfolder,
-            path_to_output_file=args.project_definition
+            path_to_output_file=args.project_definition,
         )
     elif args.action == "excel2lists":
         _, success = excel2lists(
             excelfolder=args.excelfolder,
             path_to_output_file=args.lists_section,
-            verbose=args.verbose
+            verbose=args.verbose,
         )
     elif args.action == "excel2resources":
         _, success = excel2resources(
             excelfile=args.excelfile,
-            path_to_output_file=args.resources_section
+            path_to_output_file=args.resources_section,
         )
     elif args.action == "excel2properties":
         _, success = excel2properties(
             excelfile=args.excelfile,
-            path_to_output_file=args.properties_section
+            path_to_output_file=args.properties_section,
         )
     elif args.action == "id2iri":
         success = id_to_iri(
             xml_file=args.xmlfile,
             json_file=args.mapping,
             out_file=args.outfile,
-            verbose=args.verbose
+            verbose=args.verbose,
         )
     elif args.action == "excel2xml":
         success = excel2xml(
             datafile=args.data_source,
             shortcode=args.project_shortcode,
-            default_ontology=args.ontology_name
+            default_ontology=args.ontology_name,
         )
     elif args.action == "start-stack":
         success = start_stack(
             max_file_size=args.max_file_size,
             enforce_docker_system_prune=args.prune,
-            suppress_docker_system_prune=args.no_prune
+            suppress_docker_system_prune=args.no_prune,
         )
     elif args.action == "stop-stack":
         success = stop_stack()
     elif args.action == "template":
         success = generate_template_repo()
     elif args.action == "rosetta":
         success = upload_rosetta()
@@ -415,18 +452,15 @@
     return success
 
 
 def main() -> None:
     """Main entry point of the program as referenced in pyproject.toml"""
     parser = make_parser()
     try:
-        success = call_requested_action(
-            user_args=sys.argv[1:],
-            parser=parser
-        )
+        success = call_requested_action(user_args=sys.argv[1:], parser=parser)
     except UserError as err:
         print(err.message)
         sys.exit(1)
     # let BaseError and all unexpected errors escalate, so that a stack trace is printed
 
     if not success:
         sys.exit(1)
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/excel2xml.py` & `dsp_tools-2.3.3/src/dsp_tools/excel2xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=line-too-long,consider-using-f-string
+
 from __future__ import annotations
 
 import dataclasses
 import datetime
 import difflib
 import json
 import os
@@ -13,31 +15,26 @@
 import pandas as pd
 import regex
 from lxml import etree
 from lxml.builder import E  # pylint: disable=no-name-in-module
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import DateTimeStamp
+
 # explicitly export PropertyElement, so that API users can import it from this module
 # (see https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-no-implicit-reexport)
 # doing this requires silencing the corresponding pylint warning
 # (see https://pylint.readthedocs.io/en/latest/user_guide/messages/convention/useless-import-alias.html)
-from dsp_tools.models.propertyelement import \
-    PropertyElement as PropertyElement  # pylint: disable=useless-import-alias
+from dsp_tools.models.propertyelement import PropertyElement as PropertyElement  # pylint: disable=useless-import-alias
 from dsp_tools.models.value import UriValue
-from dsp_tools.utils.shared import \
-    check_notna as check_notna  # pylint: disable=useless-import-alias
-from dsp_tools.utils.shared import \
-    simplify_name as simplify_name  # pylint: disable=useless-import-alias
+from dsp_tools.utils.shared import check_notna as check_notna  # pylint: disable=useless-import-alias
+from dsp_tools.utils.shared import simplify_name as simplify_name  # pylint: disable=useless-import-alias
 from dsp_tools.utils.shared import validate_xml_against_schema
 
-xml_namespace_map = {
-    None: "https://dasch.swiss/schema",
-    "xsi": "http://www.w3.org/2001/XMLSchema-instance"
-}
+xml_namespace_map = {None: "https://dasch.swiss/schema", "xsi": "http://www.w3.org/2001/XMLSchema-instance"}
 
 
 def make_xsd_id_compatible(string: str) -> str:
     """
     Make a string compatible with the constraints of xsd:ID, so that it can be used as "id" attribute of a <resource>
     tag. An xsd:ID must not contain special characters, and it must be unique in the document.
 
@@ -112,15 +109,15 @@
     """
 
     # sanitize input, just in case that the method was called on an empty or N/A cell
     if not check_notna(string):
         return None
     string = str(string)
 
-    monthes_dict = {
+    months_dict = {
         "January": 1,
         "Jan": 1,
         "February": 2,
         "Feb": 2,
         "March": 3,
         "Mar": 3,
         "April": 4,
@@ -151,33 +148,33 @@
     month_regex = r"([0-1]?[0-9])"
     day_regex = r"([0-3]?[0-9])"
     sep_regex = r"[\./]"
     lookbehind = r"(?<![0-9A-Za-z])"
     lookahead = r"(?![0-9A-Za-z])"
 
     # template: 2021-01-01 | 2015_01_02
-    iso_date = re.search(fr"{lookbehind}{year_regex}[_-]([0-1][0-9])[_-]([0-3][0-9]){lookahead}", string)
+    iso_date = re.search(rf"{lookbehind}{year_regex}[_-]([0-1][0-9])[_-]([0-3][0-9]){lookahead}", string)
     # template: 6.-8.3.1948 | 6/2/1947 - 24.03.1948
-    eur_date_range = re.search(
-        pattern=fr"{lookbehind}{day_regex}{sep_regex}(?:{month_regex}{sep_regex}{year_regex}?)? ?(?:-|:|to) ?"
-                fr"{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}{lookahead}",
-        string=string
+    eur_date_range_regex = (
+        rf"{lookbehind}"
+        rf"{day_regex}{sep_regex}(?:{month_regex}{sep_regex}{year_regex}?)? ?(?:-|:|to) ?"
+        rf"{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}"
+        rf"{lookahead}"
     )
+    eur_date_range = re.search(eur_date_range_regex, string)
     # template: 1.4.2021 | 5/11/2021
-    eur_date = re.search(fr"{lookbehind}{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}{lookahead}", string)
+    eur_date = re.search(rf"{lookbehind}{day_regex}{sep_regex}{month_regex}{sep_regex}{year_regex}{lookahead}", string)
     # template: March 9, 1908 | March5,1908 | May 11, 1906
-    monthname_date = re.search(
-        pattern=fr"{lookbehind}(January|Jan|February|Feb|March|Mar|April|Apr|May|June|Jun|July|Jul|August|Aug|September|Sept|"
-                fr"October|Oct|November|Nov|December|Dec) ?{day_regex}, ?{year_regex}{lookahead}",
-        string=string
-    )
+    all_months = "|".join(months_dict)
+    monthname_date_regex = rf"{lookbehind}({all_months}) ?{day_regex}, ?{year_regex}{lookahead}"
+    monthname_date = re.search(monthname_date_regex, string)
     # template: 1849/50 | 1849-50 | 1849/1850
     year_range = re.search(lookbehind + year_regex + r"[/-](\d{2}|\d{4})" + lookahead, string)
     # template: 1907
-    year_only = re.search(fr"{lookbehind}{year_regex}{lookahead}", string)
+    year_only = re.search(rf"{lookbehind}{year_regex}{lookahead}", string)
 
     if iso_date:
         year = int(iso_date.group(1))
         month = int(iso_date.group(2))
         day = int(iso_date.group(3))
         try:
             startdate = datetime.date(year, month, day)
@@ -208,28 +205,28 @@
             startdate = datetime.date(startyear, startmonth, startday)
             enddate = startdate
         except ValueError:
             return None
 
     elif monthname_date:
         day = int(monthname_date.group(2))
-        month = monthes_dict[monthname_date.group(1)]
+        month = months_dict[monthname_date.group(1)]
         year = int(monthname_date.group(3))
         try:
             startdate = datetime.date(year, month, day)
             enddate = startdate
         except ValueError:
             return None
 
     elif year_range:
         startyear = int(year_range.group(1))
         endyear = int(year_range.group(2))
-        if int(endyear/100) == 0:
+        if int(endyear / 100) == 0:
             # endyear is only 2-digit: add the first two digits of startyear
-            endyear = int(startyear/100) * 100 + endyear
+            endyear = int(startyear / 100) * 100 + endyear
 
     elif year_only:
         startyear = int(year_only.group(0))
         endyear = startyear
 
     if startdate and enddate:
         return f"GREGORIAN:CE:{startdate.isoformat()}:CE:{enddate.isoformat()}"
@@ -256,15 +253,18 @@
     if not isinstance(value, Iterable) or isinstance(value, str):
         value = [value]
 
     # make a PropertyElement out of its elements, if necessary.
     return [x if isinstance(x, PropertyElement) else PropertyElement(x) for x in value]
 
 
-def make_root(shortcode: str, default_ontology: str) -> etree._Element:
+def make_root(
+    shortcode: str,
+    default_ontology: str,
+) -> etree._Element:
     """
     Start building your XML document by creating the root element <knora>.
 
     Args:
         shortcode: The shortcode of this project as defined in the JSON project file
         default ontology: one of the ontologies of the JSON project file
 
@@ -273,24 +273,25 @@
 
     Examples:
         >>> root = make_root(shortcode=shortcode, default_ontology=default_ontology)
         >>> root = append_permissions(root)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#the-root-element-knora
     """
-
+    schema_url = "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/data.xsd"
+    schema_location_key = str(etree.QName("http://www.w3.org/2001/XMLSchema-instance", "schemaLocation"))
+    schema_location_value = f"https://dasch.swiss/schema {schema_url}"
     root = etree.Element(
         "{%s}knora" % (xml_namespace_map[None]),
         attrib={
-            str(etree.QName("http://www.w3.org/2001/XMLSchema-instance", "schemaLocation")):
-                "https://dasch.swiss/schema https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/data.xsd",
+            schema_location_key: schema_location_value,
             "shortcode": shortcode,
-            "default-ontology": default_ontology
+            "default-ontology": default_ontology,
         },
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     return root
 
 
 def append_permissions(root_element: etree._Element) -> etree._Element:
     """
     After having created a root element, call this method to append the four permissions "res-default",
@@ -345,19 +346,19 @@
 
     return root_element
 
 
 def make_resource(
     label: str,
     restype: str,
-    id: str,                                     # pylint: disable=redefined-builtin
+    id: str,  # pylint: disable=redefined-builtin
     permissions: str = "res-default",
     ark: Optional[str] = None,
     iri: Optional[str] = None,
-    creation_date: Optional[str] = None
+    creation_date: Optional[str] = None,
 ) -> etree._Element:
     """
     Creates an empty resource element, with the attributes as specified by the arguments
 
     Args:
         The arguments correspond to the attributes of the <resource> element.
 
@@ -376,46 +377,42 @@
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#describing-resources-with-the-resource-element
     """
     if not check_notna(label):
         warnings.warn(f"WARNING: Your resource's label looks suspicious (resource with id '{id}' and label '{label}'")
     if not check_notna(id):
         warnings.warn(f"WARNING: Your resource's id looks suspicious (resource with id '{id}' and label '{label}'")
-    kwargs = {
-        "label": label,
-        "restype": restype,
-        "id": id,
-        "permissions": permissions,
-        "nsmap": xml_namespace_map
-    }
+    kwargs = {"label": label, "restype": restype, "id": id, "permissions": permissions, "nsmap": xml_namespace_map}
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
+        warnings.warn(
+            f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
+            stacklevel=2,
+        )
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The resource '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
-                            f"Did you perhaps forget the timezone?") from None
+            raise BaseError(
+                f"The resource '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                f"Did you perhaps forget the timezone?"
+            ) from None
         kwargs["creation_date"] = creation_date
 
-    resource_ = etree.Element(
-        "{%s}resource" % (xml_namespace_map[None]),
-        **kwargs  # type: ignore
-    )
+    resource_ = etree.Element("{%s}resource" % (xml_namespace_map[None]), **kwargs)  # type: ignore
     return resource_
 
 
 def make_bitstream_prop(
     path: Union[str, os.PathLike[Any]],
     permissions: str = "prop-default",
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Creates a bitstream element that points to "path".
 
     Args:
         path: path to a valid file that will be uploaded
         permissions: permissions string
@@ -432,26 +429,33 @@
         >>> resource.append(make_bitstream_prop("data/images/tree.jpg"))
         >>> root.append(resource)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#bitstream
     """
 
     if not os.path.isfile(path):
-        warnings.warn(f"Failed validation in bitstream tag of resource '{calling_resource}': The following path doesn't point to a file: {path}",
-                      stacklevel=2)
+        warnings.warn(
+            f"Failed validation in bitstream tag of resource '{calling_resource}': "
+            f"The following path doesn't point to a file: {path}",
+            stacklevel=2,
+        )
     prop_ = etree.Element(
         "{%s}bitstream" % (xml_namespace_map[None]),
         permissions=permissions,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     prop_.text = str(path)
     return prop_
 
 
-def _format_bool(unformatted: Union[bool, str, int], name: str, calling_resource: str) -> str:
+def _format_bool(
+    unformatted: Union[bool, str, int],
+    name: str,
+    calling_resource: str,
+) -> str:
     """
     This method takes an unformatted boolean-like value, and transforms it into the string values "true" or "false".
 
     Args:
         unformatted: boolean-like value
         name: property name, for better error messages
         calling_resource: resource name, for better error messages
@@ -465,21 +469,24 @@
     if isinstance(unformatted, str):
         unformatted = unformatted.lower()
     if unformatted in (False, "false", "0", 0, "no"):
         return "false"
     elif unformatted in (True, "true", "1", 1, "yes"):
         return "true"
     else:
-        raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{unformatted}' is not a valid boolean.")
+        raise BaseError(
+            f"Failed validation in resource '{calling_resource}', property '{name}': "
+            f"'{unformatted}' is not a valid boolean."
+        )
 
 
 def make_boolean_prop(
     name: str,
     value: Union[PropertyElement, str, int, bool],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <boolean-prop> from a boolean value. The value can be provided directly or inside a PropertyElement. The
     following formats are supported:
      - true: (True, "true", "True", "1", 1, "yes", "Yes")
      - false: (False, "false", "False", "0", 0, "no", "No")
 
@@ -511,40 +518,42 @@
 
     # validate input
     if isinstance(value, PropertyElement):
         value_new = dataclasses.replace(value, value=_format_bool(value.value, name, calling_resource))  # type: ignore
     elif isinstance(value, (str, bool, int)):
         value_new = PropertyElement(_format_bool(value, name, calling_resource))
     else:
-        raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{value}' is not a valid boolean.")
+        raise BaseError(
+            f"Failed validation in resource '{calling_resource}', property '{name}': '{value}' is not a valid boolean."
+        )
 
     # make xml structure of the value
     prop_ = etree.Element(
         "{%s}boolean-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     kwargs = {"permissions": value_new.permissions}
     if check_notna(value_new.comment):
         kwargs["comment"] = value_new.comment  # type: ignore
     value_ = etree.Element(
         "{%s}boolean" % (xml_namespace_map[None]),
         **kwargs,  # type: ignore
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     value_.text = value_new.value  # type: ignore
     prop_.append(value_)
 
     return prop_
 
 
 def make_color_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <color-prop> from one or more colors. The color(s) can be provided as string or as PropertyElement with a
     string inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
@@ -577,41 +586,44 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not re.search(r"^#[0-9a-f]{6}$", str(val.value).strip(), flags=re.IGNORECASE):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{val.value}' is not a valid color.")
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid color."
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}color-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}color" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = str(val.value).strip()
         prop_.append(value_)
 
     return prop_
 
 
 def make_date_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <date-prop> from one or more dates/date ranges. The date(s) can be provided as string or as PropertyElement
     with a string inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
@@ -648,46 +660,51 @@
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#date-prop
     """
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
+    validation_regex = (
+        r"^(GREGORIAN:|JULIAN:)?(CE:|BCE:)?"
+        + r"(\d{4})(-\d{1,2})?(-\d{1,2})?"
+        + r"((:CE|:BCE)?(:\d{4})(-\d{1,2})?(-\d{1,2})?)?$"
+    )
     for val in values:
-        if not re.search(
-            pattern=r"^(GREGORIAN:|JULIAN:)?(CE:|BCE:)?(\d{4})(-\d{1,2})?(-\d{1,2})?((:CE|:BCE)?(:\d{4})(-\d{1,2})?(-\d{1,2})?)?$",
-            string=str(val.value).strip()
-        ):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': '{val.value}' is not a valid DSP date.")
+        if not re.search(validation_regex, str(val.value).strip()):
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid DSP date."
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}date-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}date" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = str(val.value).strip()
         prop_.append(value_)
 
     return prop_
 
 
 def make_decimal_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <decimal-prop> from one or more decimal numbers. The decimal(s) can be provided as string, float, or as
     PropertyElement with a string/float inside. If provided as string/float, the permissions default to
     "prop-default".
 
     Args:
@@ -723,42 +740,44 @@
     values = prepare_value(value)
 
     # check value type
     for val in values:
         try:
             float(val.value)
         except ValueError:
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid decimal number.") from None
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid decimal number."
+            ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}decimal-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}decimal" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = str(float(val.value))
         prop_.append(value_)
 
     return prop_
 
 
 def make_geometry_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <geometry-prop> from one or more areas of an image. The area(s) can be provided as JSON-string or as
     PropertyElement with the JSON-string inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
@@ -795,50 +814,52 @@
     # check value type
     for val in values:
         try:
             value_as_dict = json.loads(val.value)  # type: ignore
             assert value_as_dict["type"] in ["rectangle", "circle", "polygon"]
             assert isinstance(value_as_dict["points"], list)
         except (json.JSONDecodeError, TypeError, IndexError, KeyError, AssertionError):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid JSON geometry object.") from None
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid JSON geometry object."
+            ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}geometry-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}geometry" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = str(val.value)
         prop_.append(value_)
     return prop_
 
 
 def make_geoname_prop(
     name: str,
     value: Union[PropertyElement, str, int, Iterable[Union[PropertyElement, str, int]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <geoname-prop> from one or more geonames.org IDs. The ID(s) can be provided as string, integer, or as
     PropertyElement with a string/integer inside. If provided as string/integer, the permissions default to
     "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
-        value: one or more geonames.org IDs, as string/int/PropertyElement, or as iterable of strings/ints/PropertyElements
+        value: one or more geonames.org IDs, as str/int/PropertyElement, or as iterable of str/int/PropertyElement
         calling_resource: the name of the parent resource (for better error messages)
 
     Raises:
         BaseError: If the value is not a valid geonames.org identifier
 
     Returns:
         an etree._Element that can be appended to the parent resource with resource.append(make_*_prop(...))
@@ -863,42 +884,44 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not re.search(r"^[0-9]+$", str(val.value)):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a geonames.org identifier.")
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a geonames.org identifier."
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}geoname-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}geoname" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = str(val.value)
         prop_.append(value_)
 
     return prop_
 
 
 def make_integer_prop(
     name: str,
     value: Union[PropertyElement, str, int, Iterable[Union[PropertyElement, str, int]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <integer-prop> from one or more integers. The integers can be provided as string, integer, or as
     PropertyElement with a string/integer inside. If provided as string/integer, the permissions default to
     "prop-default".
 
     Args:
@@ -934,42 +957,44 @@
     values = prepare_value(value)
 
     # check value type
     for val in values:
         try:
             int(val.value)
         except ValueError:
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid integer.") from None
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid integer."
+            ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}integer-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}integer" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = str(int(val.value))
         prop_.append(value_)
 
     return prop_
 
 
 def make_interval_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <interval-prop> from one or more DSP intervals. The interval(s) can be provided as string or as
     PropertyElement with a string inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
@@ -1002,43 +1027,45 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not re.match(r"([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+)):([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+))", str(val.value)):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid DSP interval.")
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid DSP interval."
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}interval-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}interval" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = val.value  # type: ignore
         prop_.append(value_)
 
     return prop_
 
 
 def make_list_prop(
     list_name: str,
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <list-prop> from one or more list nodes. The name(s) of the list node(s) can be provided as string or as
     PropertyElement with a string inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         list_name: the name of the list as defined in the onto
@@ -1072,43 +1099,45 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not isinstance(val.value, str) or not check_notna(val.value):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid name of a list node.")
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid name of a list node."
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}list-prop" % (xml_namespace_map[None]),
         list=list_name,
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}list" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = val.value  # type: ignore
         prop_.append(value_)
 
     return prop_
 
 
 def make_resptr_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <resptr-prop> from one or more IDs of other resources. The ID(s) can be provided as string or as
     PropertyElement with a string inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
@@ -1141,55 +1170,59 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not isinstance(val.value, str) or not check_notna(val.value):
-            raise BaseError(f"Validation Error in resource '{calling_resource}', property '{name}': "
-                            f"The following doesn't seem to be a valid ID of a target resource: '{val.value}'")
+            raise BaseError(
+                f"Validation Error in resource '{calling_resource}', property '{name}': "
+                f"The following doesn't seem to be a valid ID of a target resource: '{val.value}'"
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}resptr-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}resptr" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = val.value  # type: ignore
         prop_.append(value_)
 
     return prop_
 
 
 def make_text_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <text-prop> from one or more strings. The string(s) can be provided as string or as PropertyElement with a
     string inside. If provided as string, the encoding defaults to utf8, and the permissions to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
         value: one or more strings, as string/PropertyElement, or as iterable of strings/PropertyElements
         calling_resource: the name of the parent resource (for better error messages)
 
     Raises:
-        BaseError: if one of the values is not a valid string, or if the XML tags in a richtext property (encoding=xml) are not well-formed
-        Warning: if one of the values doesn't look like a reasonable string (e.g. "<NA>" is a valid string, but probably not intended)
+        BaseError: if one of the values is not a valid string,
+            or if the XML tags in a richtext property (encoding=xml) are not well-formed
+        Warning: if one of the values doesn't look like a reasonable string
+            (e.g. "<NA>" is a valid string, but probably not intended)
 
     Returns:
         an etree._Element that can be appended to the parent resource with resource.append(make_*_prop(...))
 
     Examples:
         >>> make_text_prop(":testproperty", "first text")
                 <text-prop name=":testproperty">
@@ -1210,46 +1243,51 @@
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
     for val in values:
         if not isinstance(val.value, str) or len(val.value) < 1:
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid string.")
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid string."
+            )
         if not check_notna(val.value):
-            warnings.warn(f"Warning for resource '{calling_resource}', property '{name}': "
-                          f"'{val.value}' is probably not a usable string.", stacklevel=2)
+            warnings.warn(
+                f"Warning for resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is probably not a usable string.",
+                stacklevel=2,
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}text-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         if check_notna(val.encoding):
             kwargs["encoding"] = val.encoding  # type: ignore
         else:
             kwargs["encoding"] = "utf8"
         value_ = etree.Element(
             "{%s}text" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         if kwargs["encoding"] == "utf8":
             # write the text into the tag, without validation
             value_.text = str(val.value)
         else:
             # enforce that the text is well-formed XML: serialize tag ...
             content = etree.tostring(value_, encoding="unicode")
-            # ... insert text at the very end of the string, and add an ending tag to the previously single <text/> tag ...
+            # ... insert text at the very end of the string, and add ending tag to the previously single <text/> tag ...
             content = re.sub(r"/>$", f">{val.value}</text>", content)
             # ... try to parse it again
             try:
                 value_ = etree.fromstring(content)
             except etree.XMLSyntaxError:
                 raise BaseError(
                     "The XML tags contained in a richtext property (encoding=xml) must be well-formed. "
@@ -1260,15 +1298,15 @@
 
     return prop_
 
 
 def make_time_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make a <time-prop> from one or more datetime values of the form "2009-10-10T12:00:00-05:00". The time(s) can be
     provided as string or as PropertyElement with a string inside. If provided as string, the permissions default to
     "prop-default".
 
     Args:
@@ -1308,44 +1346,47 @@
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#time-prop
     """
 
     # check the input: prepare a list with valid values
     values = prepare_value(value)
 
     # check value type
+    validation_regex = r"^\d{4}-[0-1]\d-[0-3]\dT[0-2]\d:[0-5]\d:[0-5]\d(.\d{1,12})?(Z|[+-][0-1]\d:[0-5]\d)$"
     for val in values:
-        if not re.search(r"^\d{4}-[0-1]\d-[0-3]\dT[0-2]\d:[0-5]\d:[0-5]\d(.\d{1,12})?(Z|[+-][0-1]\d:[0-5]\d)$", str(val.value)):
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid DSP time.")
+        if not re.search(validation_regex, str(val.value)):
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid DSP time."
+            )
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}time-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}time" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = val.value  # type: ignore
         prop_.append(value_)
 
     return prop_
 
 
 def make_uri_prop(
     name: str,
     value: Union[PropertyElement, str, Iterable[Union[PropertyElement, str]]],
-    calling_resource: str = ""
+    calling_resource: str = "",
 ) -> etree._Element:
     """
     Make an <uri-prop> from one or more URIs. The URI(s) can be provided as string or as PropertyElement with a string
     inside. If provided as string, the permissions default to "prop-default".
 
     Args:
         name: the name of this property as defined in the onto
@@ -1380,45 +1421,47 @@
     values = prepare_value(value)
 
     # check value type
     for val in values:
         try:
             UriValue(str(val.value))
         except BaseError:
-            raise BaseError(f"Failed validation in resource '{calling_resource}', property '{name}': "
-                            f"'{val.value}' is not a valid URI.") from None
+            raise BaseError(
+                f"Failed validation in resource '{calling_resource}', property '{name}': "
+                f"'{val.value}' is not a valid URI."
+            ) from None
 
     # make xml structure of the valid values
     prop_ = etree.Element(
         "{%s}uri-prop" % (xml_namespace_map[None]),
         name=name,
-        nsmap=xml_namespace_map
+        nsmap=xml_namespace_map,
     )
     for val in values:
         kwargs = {"permissions": val.permissions}
         if check_notna(val.comment):
             kwargs["comment"] = val.comment  # type: ignore
         value_ = etree.Element(
             "{%s}uri" % (xml_namespace_map[None]),
             **kwargs,  # type: ignore
-            nsmap=xml_namespace_map
+            nsmap=xml_namespace_map,
         )
         value_.text = val.value  # type: ignore
         prop_.append(value_)
 
     return prop_
 
 
 def make_region(
     label: str,
-    id: str,                                     # pylint: disable=redefined-builtin
+    id: str,  # pylint: disable=redefined-builtin
     permissions: str = "res-default",
     ark: Optional[str] = None,
     iri: Optional[str] = None,
-    creation_date: Optional[str] = None
+    creation_date: Optional[str] = None,
 ) -> etree._Element:
     """
     Creates an empty region element, with the attributes as specified by the arguments
 
     Args:
         The arguments correspond 1:1 to the attributes of the <region> element.
 
@@ -1437,48 +1480,48 @@
         >>> region.append(make_resptr_prop("isRegionOf", "image_0"))
         >>> region.append(make_geometry_prop("hasGeometry", "{...}"))
         >>> root.append(region)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#region
     """
 
-    kwargs = {
-        "label": label,
-        "id": id,
-        "permissions": permissions,
-        "nsmap": xml_namespace_map
-    }
+    kwargs = {"label": label, "id": id, "permissions": permissions, "nsmap": xml_namespace_map}
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
+        warnings.warn(
+            f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
+            stacklevel=2,
+        )
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The region '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
-                            f"Did you perhaps forget the timezone?") from None
+            raise BaseError(
+                f"The region '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                f"Did you perhaps forget the timezone?"
+            ) from None
         kwargs["creation_date"] = creation_date
 
     region_ = etree.Element(
         "{%s}region" % (xml_namespace_map[None]),
-        **kwargs  # type: ignore
+        **kwargs,  # type: ignore
     )
     return region_
 
 
 def make_annotation(
     label: str,
-    id: str,                                     # pylint: disable=redefined-builtin
+    id: str,  # pylint: disable=redefined-builtin
     permissions: str = "res-default",
     ark: Optional[str] = None,
     iri: Optional[str] = None,
-    creation_date: Optional[str] = None
+    creation_date: Optional[str] = None,
 ) -> etree._Element:
     """
     Creates an empty annotation element, with the attributes as specified by the arguments
 
     Args:
         The arguments correspond 1:1 to the attributes of the <annotation> element.
 
@@ -1495,48 +1538,48 @@
         >>> annotation.append(make_text_prop("hasComment", "This is a comment"))
         >>> annotation.append(make_resptr_prop("isAnnotationOf", "resource_0"))
         >>> root.append(annotation)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#annotation
     """
 
-    kwargs = {
-        "label": label,
-        "id": id,
-        "permissions": permissions,
-        "nsmap": xml_namespace_map
-    }
+    kwargs = {"label": label, "id": id, "permissions": permissions, "nsmap": xml_namespace_map}
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
+        warnings.warn(
+            f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
+            stacklevel=2,
+        )
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The annotation '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
-                            f"Did you perhaps forget the timezone?") from None
+            raise BaseError(
+                f"The annotation '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                f"Did you perhaps forget the timezone?"
+            ) from None
         kwargs["creation_date"] = creation_date
 
     annotation_ = etree.Element(
         "{%s}annotation" % (xml_namespace_map[None]),
-        **kwargs  # type: ignore
+        **kwargs,  # type: ignore
     )
     return annotation_
 
 
 def make_link(
     label: str,
-    id: str,                                     # pylint: disable=redefined-builtin
+    id: str,  # pylint: disable=redefined-builtin
     permissions: str = "res-default",
     ark: Optional[str] = None,
     iri: Optional[str] = None,
-    creation_date: Optional[str] = None
+    creation_date: Optional[str] = None,
 ) -> etree._Element:
     """
     Creates an empty link element, with the attributes as specified by the arguments
 
     Args:
         The arguments correspond 1:1 to the attributes of the <link> element.
 
@@ -1553,47 +1596,47 @@
         >>> link.append(make_text_prop("hasComment", "This is a comment"))
         >>> link.append(make_resptr_prop("hasLinkTo", ["resource_0", "resource_1"]))
         >>> root.append(link)
 
     See https://docs.dasch.swiss/latest/DSP-TOOLS/file-formats/xml-data-file/#link
     """
 
-    kwargs = {
-        "label": label,
-        "id": id,
-        "permissions": permissions,
-        "nsmap": xml_namespace_map
-    }
+    kwargs = {"label": label, "id": id, "permissions": permissions, "nsmap": xml_namespace_map}
     if ark:
         kwargs["ark"] = ark
     if iri:
         kwargs["iri"] = iri
     if ark and iri:
-        warnings.warn(f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.", stacklevel=2)
+        warnings.warn(
+            f"Both ARK and IRI were provided for resource '{label}' ({id}). The ARK will override the IRI.",
+            stacklevel=2,
+        )
     if creation_date:
         try:
             DateTimeStamp(creation_date)
         except BaseError:
-            raise BaseError(f"The link '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
-                            f"Did you perhaps forget the timezone?") from None
+            raise BaseError(
+                f"The link '{label}' (ID: {id}) has an invalid creation date '{creation_date}'. "
+                f"Did you perhaps forget the timezone?"
+            ) from None
         kwargs["creation_date"] = creation_date
 
     link_ = etree.Element(
         "{%s}link" % (xml_namespace_map[None]),
-        **kwargs  # type: ignore
+        **kwargs,  # type: ignore
     )
     return link_
 
 
 def create_json_excel_list_mapping(
     path_to_json: str,
     list_name: str,
     excel_values: Iterable[str],
     sep: str = '+"*ç%&/()=',
-    corrections: Optional[dict[str, str]] = None
+    corrections: Optional[dict[str, str]] = None,
 ) -> dict[str, str]:
     """
     Often, data sources contain list values that aren't identical to the name of the node in the list of the JSON
     project file (colloquially: ontology). In order to create a correct XML for the `dsp-tools xmlupload`, a mapping is
     necessary. This function takes a JSON list and an Excel column containing list-values, and tries to match them
     automatically based on similarity. The result is a dict of the form {excel_value: list_node_name}.
 
@@ -1609,30 +1652,37 @@
         corrections: dict with wrong entries, each pointing to its correct counterpart
 
     Raises:
         Warning: if there is an Excel value that couldn't be matched
         Exception: if the path doesn't point to a JSON project file
 
     Returns:
-        dict of the form {excel_value: list_node_name}. Every excel_value is stripped, and also present in a lowercase form.
+        dict of the form ``{excel_value: list_node_name}``.
+            Every excel_value is stripped, and also present in a lowercase form.
 
     Examples:
         >>> json_list_nodes = [
                 {
                     "name": "giraffe",
                     "labels": {"en": "giraffe"}
                 },
                 {
                     "name": "antelope",
                     "labels": {"en": "antelope"}
                 }
             ]
         >>> excel_row_1 = ["Giraffeeh ", " Antiloupe", "Girraffe , Antiloupe "]
-        >>> json_excel_list_mapping = {"Giraffeeh": "giraffe", "Girraffe": "giraffe", "Antiloupe": "antelope",
-        >>>                            "giraffeeh": "giraffe", "girraffe": "giraffe", "antiloupe": "antelope"}
+        >>> json_excel_list_mapping = {
+                "Giraffeeh": "giraffe",
+                "giraffeeh": "giraffe",
+                "Girraffe": "giraffe",
+                "girraffe": "giraffe",
+                "Antiloupe": "antelope",
+                "antiloupe": "antelope"
+            }
     """
 
     # avoid mutable default argument
     corrections = corrections or {}
 
     # split the values, if necessary
     excel_values_new = list()
@@ -1654,45 +1704,48 @@
     for excel_value in excel_values_new:
         excel_value_corrected = corrections.get(excel_value, excel_value)
         excel_value_simpl = simplify_name(excel_value_corrected)  # increase match probability by removing illegal chars
         matches: list[str] = difflib.get_close_matches(
             word=excel_value_simpl,
             possibilities=json_values,
             n=1,
-            cutoff=0.6
+            cutoff=0.6,
         )
         if matches:
             res[excel_value] = matches[0]
             res[excel_value.lower()] = matches[0]
         else:
-            warnings.warn(f"Did not find a close match to the excel list entry '{excel_value}' "
-                          f"among the values in the JSON project list '{list_name}'", stacklevel=2)
+            warnings.warn(
+                f"Did not find a close match to the excel list entry '{excel_value}' "
+                f"among the values in the JSON project list '{list_name}'",
+                stacklevel=2,
+            )
 
     return res
 
 
 def _nested_dict_values_iterator(dicts: list[dict[str, Any]]) -> Iterable[str]:
     """
     This function accepts a list of nested dictionaries as argument
-    and iterates over all values. 
+    and iterates over all values.
     It yields the values iteratively.
     """
     # Credits: https://thispointer.com/python-iterate-loop-over-all-nested-dictionary-values/
     for _dict in dicts:
         if "nodes" in _dict:
             for value in _nested_dict_values_iterator(_dict["nodes"]):
                 yield value
         if "name" in _dict:
             yield _dict["name"]
 
 
 def create_json_list_mapping(
     path_to_json: str,
     list_name: str,
-    language_label: str
+    language_label: str,
 ) -> dict[str, str]:
     """
     Often, data sources contain list values named after the "label" of the JSON project list node, instead of the "name"
     which is needed for the `dsp-tools xmlupload`. In order to create a correct XML, you need a dictionary that maps the
     "labels" to their correct "names".
 
     Alternatively, consider using the method create_json_excel_list_mapping(), which also creates a dictionary, but maps
@@ -1719,15 +1772,18 @@
         if name != list_name:
             res[label] = name
             res[label.strip().lower()] = name
 
     return res
 
 
-def _name_label_mapper_iterator(json_subset: list[dict[str, Any]], language_label: str) -> Iterable[tuple[str, str]]:
+def _name_label_mapper_iterator(
+    json_subset: list[dict[str, Any]],
+    language_label: str,
+) -> Iterable[tuple[str, str]]:
     """
     returns (label, name) pairs of JSON project list entries
     """
     for node in json_subset:
         # node is the json object containing the entire json-list
         if "nodes" in node:
             # "nodes" is the json sub-object containing the entries of the json-list
@@ -1735,38 +1791,49 @@
                 yield value
                 # "value" is a (label, name) pair of a single list entry
         if "name" in node:
             yield (node["labels"][language_label], node["name"])
             # the actual values of the name and the label
 
 
-def write_xml(root: etree._Element, filepath: str) -> None:
+def write_xml(
+    root: etree._Element,
+    filepath: str,
+) -> None:
     """
     Write the finished XML to a file
 
     Args:
         root: etree Element with the entire XML document
         filepath: where to save the file
 
     Raises:
         Warning: if the XML is not valid according to the schema
 
     Returns:
         None
     """
     etree.indent(root, space="    ")
-    xml_string = etree.tostring(root, encoding="unicode", pretty_print=True, doctype='<?xml version="1.0" encoding="UTF-8"?>')
-    xml_string = xml_string.replace("\'", "'")
+    xml_string = etree.tostring(
+        root,
+        encoding="unicode",
+        pretty_print=True,
+        doctype='<?xml version="1.0" encoding="UTF-8"?>',
+    )
+    xml_string = xml_string.replace(r"\'", "'")
     with open(filepath, "w", encoding="utf-8") as f:
         f.write(xml_string)
     try:
         validate_xml_against_schema(input_file=filepath)
         print(f"The XML file was successfully saved to {filepath}")
     except BaseError as err:
-        warnings.warn(f"The XML file was successfully saved to {filepath}, but the following Schema validation error(s) occurred: {err.message}")
+        warnings.warn(
+            f"The XML file was successfully saved to {filepath}, "
+            f"but the following Schema validation error(s) occurred: {err.message}"
+        )
 
 
 def _read_cli_input_file(datafile: str) -> pd.DataFrame:
     """
     Parse the input file from the CLI (in either CSV or Excel format)
 
     Args:
@@ -1776,25 +1843,22 @@
         BaseError: if the input file is neither .csv, .xls nor .xlsx
 
     Returns:
         a pandas DataFrame with the input data
     """
     if re.search(r"\.csv$", datafile):
         dataframe = pd.read_csv(
-            filepath_or_buffer=datafile, 
-            encoding="utf_8_sig",           # utf_8_sig is the default encoding of Excel
-            dtype="str", 
-            sep=None, 
-            engine="python"                 # let the "python" engine detect the separator
+            filepath_or_buffer=datafile,
+            encoding="utf_8_sig",  # utf_8_sig is the default encoding of Excel
+            dtype="str",
+            sep=None,
+            engine="python",  # let the "python" engine detect the separator
         )
     elif re.search(r"(\.xls|\.xlsx)$", datafile):
-        dataframe = pd.read_excel(
-            io=datafile, 
-            dtype="str"
-        )
+        dataframe = pd.read_excel(io=datafile, dtype="str")
     else:
         raise BaseError(f"Cannot open file '{datafile}': Invalid extension. Allowed extensions: 'csv', 'xls', 'xlsx'")
     return dataframe
 
 
 def _validate_and_prepare_cli_input_file(dataframe: pd.DataFrame) -> pd.DataFrame:
     """
@@ -1811,15 +1875,17 @@
 
     Returns:
         the prepared pandas DataFrame
     """
     # make sure that the required columns are present
     required_columns = ["id", "label", "restype", "permissions", "prop name", "prop type", "1_value"]
     if any(req not in dataframe for req in required_columns):
-        raise BaseError(f"Some columns in your input file are missing. The following columns are required: {required_columns}")
+        raise BaseError(
+            f"Some columns in your input file are missing. The following columns are required: {required_columns}"
+        )
 
     # replace NA-like cells by NA
     dataframe = dataframe.applymap(
         lambda x: x if pd.notna(x) and regex.search(r"[\p{L}\d_!?\-]", str(x), flags=regex.U) else pd.NA
     )
 
     # remove empty columns/rows
@@ -1827,27 +1893,28 @@
     dataframe.dropna(axis="index", how="all", inplace=True)
 
     return dataframe
 
 
 def _convert_rows_to_xml(
     dataframe: pd.DataFrame,
-    max_num_of_props: int
+    max_num_of_props: int,
 ) -> list[etree._Element]:
     """
-    Iterate through the rows of the CSV/Excel input file, 
+    Iterate through the rows of the CSV/Excel input file,
     convert every row to either a XML resource or an XML property,
     and return a list of XML resources.
 
     Args:
         dataframe: pandas dataframe with the input data
         max_num_of_props: highest number of properties that a resource in this file has
-    
+
     Raises:
-        BaseError: if one of the rows is neither a resource-row nor a property-row, or if the file starts with a property-row
+        BaseError: if one of the rows is neither a resource-row nor a property-row,
+            or if the file starts with a property-row
 
     Returns:
         a list of XML resources (with their respective properties)
     """
     resources: list[etree._Element] = []
 
     # to start, there is no previous resource
@@ -1859,50 +1926,49 @@
         if check_notna(row["id"]) == check_notna(row["prop name"]):
             raise BaseError(
                 f"Exactly 1 of the 2 columns 'id' and 'prop name' must be filled. "
                 f"Excel row {row_number} has too many/too less entries:\n"
                 f"id:        '{row['id']}'\n"
                 f"prop name: '{row['prop name']}'"
             )
-        
+
         # this is a resource-row
         elif check_notna(row["id"]):
             # the previous resource is finished, a new resource begins: append the previous to the resulting list
             # in all cases (except for the very first iteration), a previous resource exists
             if resource is not None:
                 resources.append(resource)
-            resource = _convert_resource_row_to_xml(
-                row_number=row_number,
-                row=row
-            )
+            resource = _convert_resource_row_to_xml(row_number=row_number, row=row)
 
         # this is a property-row
-        else:  
+        else:
             assert check_notna(row["prop name"])
             if resource is None:
-                raise BaseError("The first row of your Excel/CSV is invalid. The first row must define a resource, not a property.")
+                raise BaseError(
+                    "The first row of your Excel/CSV is invalid. The first row must define a resource, not a property."
+                )
             prop = _convert_property_row_to_xml(
                 row_number=row_number,
                 row=row,
                 max_num_of_props=max_num_of_props,
-                resource_id=resource.attrib["id"]
+                resource_id=resource.attrib["id"],
             )
             resource.append(prop)
 
     # append the resource of the very last iteration of the for loop
     if resource is not None:
         resources.append(resource)
 
     return resources
 
 
 def _append_bitstream_to_resource(
     resource: etree._Element,
     row: pd.Series,
-    row_number: int
+    row_number: int,
 ) -> etree._Element:
     """
     Create a bitstream-prop element, and append it to the resource.
     If the file permissions are missing, try to deduce them from the resource permissions.
 
     Args:
         resource: the resource element to which the bitstream-prop element should be appended
@@ -1920,30 +1986,31 @@
         resource_permissions = row.get("permissions")
         if resource_permissions == "res-default":
             file_permissions = "prop-default"
         elif resource_permissions == "res-restricted":
             file_permissions = "prop-restricted"
         else:
             raise BaseError(
-                f"Missing file permissions for file '{row['file']}' (Resource ID '{row['id']}', Excel row {row_number}). "
+                f"Missing file permissions for file "
+                f"'{row['file']}' (Resource ID '{row['id']}', Excel row {row_number}). "
                 f"An attempt to deduce them from the resource permissions failed."
             )
     resource.append(
         make_bitstream_prop(
             path=str(row["file"]),
             permissions=str(file_permissions),
-            calling_resource=row["id"]
+            calling_resource=row["id"],
         )
     )
     return resource
 
 
 def _convert_resource_row_to_xml(
     row_number: int,
-    row: pd.Series
+    row: pd.Series,
 ) -> etree._Element:
     """
     Convert a resource-row to an XML resource element.
     First, check if the mandatory cells are present.
     Then, call the appropriate function, depending on the restype (Resource, LinkObj, Annotation, Region).
 
     Args:
@@ -1958,60 +2025,61 @@
     """
     # read and check the mandatory columns
     resource_id = row["id"]
     resource_label = row.get("label")
     if pd.isna([resource_label]):
         raise BaseError(f"Missing label for resource '{resource_id}' (Excel row {row_number})")
     if not check_notna(resource_label):
-        warnings.warn(f"The label of resource '{resource_id}' looks suspicious: '{resource_label}' (Excel row {row_number})")
+        warnings.warn(
+            f"The label of resource '{resource_id}' looks suspicious: '{resource_label}' (Excel row {row_number})"
+        )
     resource_restype = row.get("restype")
     if not check_notna(resource_restype):
         raise BaseError(f"Missing restype for resource '{resource_id}' (Excel row {row_number})")
     resource_permissions = row.get("permissions")
     if not check_notna(resource_permissions):
         raise BaseError(f"Missing permissions for resource '{resource_id}' (Excel row {row_number})")
 
     # construct the kwargs for the method call
-    kwargs_resource = {
-        "label": resource_label,
-        "permissions": resource_permissions,
-        "id": resource_id
-    }
+    kwargs_resource = {"label": resource_label, "permissions": resource_permissions, "id": resource_id}
     if check_notna(row.get("ark")):
         kwargs_resource["ark"] = row["ark"]
     if check_notna(row.get("iri")):
         kwargs_resource["iri"] = row["iri"]
     if check_notna(row.get("ark")) and check_notna(row.get("iri")):
-        warnings.warn(f"Both ARK and IRI were provided for resource '{resource_label}' ({resource_id}). The ARK will override the IRI.")
+        warnings.warn(
+            f"Both ARK and IRI were provided for resource '{resource_label}' ({resource_id}). "
+            "The ARK will override the IRI."
+        )
     if check_notna(row.get("created")):
         kwargs_resource["creation_date"] = row["created"]
-    
+
     # call the appropriate method
     if resource_restype == "Region":
         resource = make_region(**kwargs_resource)
     elif resource_restype == "Annotation":
         resource = make_annotation(**kwargs_resource)
     elif resource_restype == "LinkObj":
         resource = make_link(**kwargs_resource)
     else:
         kwargs_resource["restype"] = resource_restype
         resource = make_resource(**kwargs_resource)
         if check_notna(row.get("file")):
             resource = _append_bitstream_to_resource(
                 resource=resource,
                 row=row,
-                row_number=row_number
+                row_number=row_number,
             )
 
     return resource
 
 
 def _get_prop_function(
     row: pd.Series,
-    resource_id: str
+    resource_id: str,
 ) -> Callable[..., etree._Element]:
     """
     Return the function that creates the appropriate property, depending on the proptype.
 
     Args:
         row: row of the CSV/Excel sheet that defines the property
         resource_id: resource ID of the resource to which the property belongs
@@ -2031,32 +2099,32 @@
         "geometry-prop": make_geometry_prop,
         "geoname-prop": make_geoname_prop,
         "integer-prop": make_integer_prop,
         "interval-prop": make_interval_prop,
         "list-prop": make_list_prop,
         "resptr-prop": make_resptr_prop,
         "text-prop": make_text_prop,
-        "uri-prop": make_uri_prop
+        "uri-prop": make_uri_prop,
     }
     if row.get("prop type") not in proptype_2_function:
         raise BaseError(f"Invalid prop type for property {row.get('prop name')} in resource {resource_id}")
     make_prop_function = proptype_2_function[row["prop type"]]
     return make_prop_function
 
 
 def _convert_row_to_property_elements(
     row: pd.Series,
     max_num_of_props: int,
     row_number: int,
-    resource_id: str
+    resource_id: str,
 ) -> list[PropertyElement]:
     """
-    Every property contains i elements, 
-    which are represented in the Excel as groups of columns named 
-    {i_value, i_encoding, i_permissions, i_comment}. 
+    Every property contains i elements,
+    which are represented in the Excel as groups of columns named
+    {i_value, i_encoding, i_permissions, i_comment}.
     Depending on the property type, some of these cells are empty.
     This method converts a row to a list of PropertyElement objects.
 
     Args:
         row: the pandas series representing the current row
         max_num_of_props: highest number of properties that a resource in this file has
         row_number: row number of the CSV/Excel sheet
@@ -2075,49 +2143,54 @@
             # raise error if other cells of this property element are not empty
             # if all other cells are empty, continue with next property element
             other_cell_headers = [f"{i}_{x}" for x in ["encoding", "permissions", "comment"]]
             notna_cell_headers = [x for x in other_cell_headers if check_notna(row.get(x))]
             notna_cell_headers_str = ", ".join([f"'{x}'" for x in notna_cell_headers])
             if notna_cell_headers_str:
                 raise BaseError(
-                    f"Error in resource '{resource_id}': Excel row {row_number} has an entry in column(s) {notna_cell_headers_str}, "
-                    f"but not in '{i}_value'. "
-                    r"Please note that cell contents that don't meet the requirements of the regex [\p{L}\d_!?\-] are considered inexistent."
+                    f"Error in resource '{resource_id}': Excel row {row_number} has an entry "
+                    f"in column(s) {notna_cell_headers_str}, but not in '{i}_value'. "
+                    r"Please note that cell contents that don't meet the requirements of the regex [\p{L}\d_!?\-] "
+                    "are considered inexistent."
                 )
             continue
-        
+
         # construct a PropertyElement from this property element
-        kwargs_propelem = {
-            "value": value,
-            "permissions": str(row.get(f"{i}_permissions"))
-        }
+        kwargs_propelem = {"value": value, "permissions": str(row.get(f"{i}_permissions"))}
         if not check_notna(row.get(f"{i}_permissions")):
-            raise BaseError(f"Missing permissions in column '{i}_permissions' of property '{row['prop name']}' in resource with id '{resource_id}'")
+            raise BaseError(
+                f"Resource '{resource_id}': "
+                f"Missing permissions in column '{i}_permissions' of property '{row['prop name']}'"
+            )
         if check_notna(row.get(f"{i}_comment")):
             kwargs_propelem["comment"] = str(row[f"{i}_comment"])
         if check_notna(row.get(f"{i}_encoding")):
             kwargs_propelem["encoding"] = str(row[f"{i}_encoding"])
         property_elements.append(PropertyElement(**kwargs_propelem))
 
     # validate the end result before returning it
     if len(property_elements) == 0:
-        raise BaseError(f"At least one value per property is required, "
-                        f"but resource '{resource_id}' (Excel row {row_number}) doesn't contain any values.")
+        raise BaseError(
+            f"At least one value per property is required, "
+            f"but resource '{resource_id}' (Excel row {row_number}) doesn't contain any values."
+        )
     if row.get("prop type") == "boolean-prop" and len(property_elements) != 1:
-        raise BaseError(f"A <boolean-prop> can only have a single value, "
-                        f"but resource '{resource_id}' (Excel row {row_number}) contains more than one value.")
-    
+        raise BaseError(
+            f"A <boolean-prop> can only have a single value, "
+            f"but resource '{resource_id}' (Excel row {row_number}) contains more than one value."
+        )
+
     return property_elements
 
 
 def _convert_property_row_to_xml(
     row_number: int,
     row: pd.Series,
     max_num_of_props: int,
-    resource_id: str
+    resource_id: str,
 ) -> etree._Element:
     """
     Convert a property-row of the CSV/Excel sheet to an XML element.
 
     Args:
         row_number: row number of the CSV/Excel sheet
         row: the pandas series representing the current row
@@ -2128,41 +2201,41 @@
         BaseError: if there is inconsistent data in the row / if a validation fails
 
     Returns:
         the resource element with the appended property
     """
     # based on the property type, the right function has to be chosen
     make_prop_function = _get_prop_function(
-        row=row, 
-        resource_id=resource_id
+        row=row,
+        resource_id=resource_id,
     )
 
     # convert the row to a list of PropertyElement objects
     property_elements = _convert_row_to_property_elements(
         row=row,
         max_num_of_props=max_num_of_props,
         row_number=row_number,
-        resource_id=resource_id
+        resource_id=resource_id,
     )
 
     # create the property
     prop = _create_property(
         make_prop_function=make_prop_function,
         row=row,
         property_elements=property_elements,
-        resource_id=resource_id
+        resource_id=resource_id,
     )
     return prop
 
 
 def _create_property(
     make_prop_function: Callable[..., etree._Element],
     row: pd.Series,
     property_elements: list[PropertyElement],
-    resource_id: str
+    resource_id: str,
 ) -> etree._Element:
     """
     Create a property based on the appropriate function and the property elements.
 
     Args:
         make_prop_function: the function to create the property
         row: the pandas series representing the current row of the Excel/CSV
@@ -2170,45 +2243,45 @@
         resource_id: id of resource to which this property belongs to
 
     Returns:
         the resource with the properties appended
     """
     kwargs_propfunc: dict[str, Union[str, PropertyElement, list[PropertyElement]]] = {
         "name": row["prop name"],
-        "calling_resource": resource_id
+        "calling_resource": resource_id,
     }
 
     if row.get("prop type") == "boolean-prop":
         kwargs_propfunc["value"] = property_elements[0]
     else:
         kwargs_propfunc["value"] = property_elements
-    
+
     if check_notna(row.get("prop list")):
         kwargs_propfunc["list_name"] = str(row["prop list"])
 
     prop = make_prop_function(**kwargs_propfunc)
 
     return prop
 
 
 def excel2xml(
-    datafile: str, 
-    shortcode: str, 
-    default_ontology: str
+    datafile: str,
+    shortcode: str,
+    default_ontology: str,
 ) -> bool:
     """
-    This is a method that is called from the command line. 
-    It isn't intended to be used in a Python script. 
-    It takes a tabular data source in CSV/XLS(X) format that is formatted according to the specifications, 
-    and transforms it into a DSP-conforming XML file 
-    that can be uploaded to a DSP server with the xmlupload command. 
-    The output file is saved in the same directory as the input file, 
+    This is a method that is called from the command line.
+    It isn't intended to be used in a Python script.
+    It takes a tabular data source in CSV/XLS(X) format that is formatted according to the specifications,
+    and transforms it into a DSP-conforming XML file
+    that can be uploaded to a DSP server with the xmlupload command.
+    The output file is saved in the same directory as the input file,
     with the name [default_ontology]-data.xml.
 
-    Please note that this method doesn't do any data cleaning or data transformation tasks. 
+    Please note that this method doesn't do any data cleaning or data transformation tasks.
     The input and the output of this method are semantically exactly equivalent.
 
     Args:
         datafile: path to the data file (CSV or XLS(X))
         shortcode: shortcode of the project that this data belongs to
         default_ontology: name of the ontology that this data belongs to
 
@@ -2218,25 +2291,25 @@
     Returns:
         True if everything went well, False otherwise
     """
     # read and prepare the input file
     success = True
     dataframe = _read_cli_input_file(datafile)
     dataframe = _validate_and_prepare_cli_input_file(dataframe)
-    last_column_title = str(list(dataframe)[-1])    # last column title, in the format "i_comment"
+    last_column_title = str(list(dataframe)[-1])  # last column title, in the format "i_comment"
     max_num_of_props = int(last_column_title.split("_")[0])
 
     # create the XML root element
     root = make_root(shortcode=shortcode, default_ontology=default_ontology)
     root = append_permissions(root)
 
     # parse the input file row by row
     resources = _convert_rows_to_xml(
         dataframe=dataframe,
-        max_num_of_props=max_num_of_props
+        max_num_of_props=max_num_of_props,
     )
     for resource in resources:
         root.append(resource)
 
     # write file
     with warnings.catch_warnings(record=True) as w:
         write_xml(root, f"{default_ontology}-data.xml")
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/process_files.py` & `dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/process_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module handles processing of files referenced in the bitstream tags of an XML file."""
 
 import hashlib
 import json
 import pickle
 import shutil
 import subprocess
+import sys
 import uuid
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
 from pathlib import Path, PurePath
 from typing import Any, Optional, Union
 
 import docker
@@ -30,23 +31,23 @@
     """
     user_folder = Path.home() / Path(".dsp-tools/fast-xmlupload")
     user_folder.mkdir(parents=True, exist_ok=True)
     global export_moving_image_frames_script
     export_moving_image_frames_script = user_folder / "export-moving-image-frames.sh"
     script_text = requests.get(
         "https://github.com/dasch-swiss/dsp-api/raw/main/sipi/scripts/export-moving-image-frames.sh",
-        timeout=5
+        timeout=5,
     ).text
     with open(export_moving_image_frames_script, "w", encoding="utf-8") as f:
         f.write(script_text)
 
 
 def _check_if_all_files_were_processed(
     result: list[tuple[Path, Optional[Path]]],
-    all_paths: list[Path]
+    all_paths: list[Path],
 ) -> bool:
     """
     Go through the result list and print all files that could not be processed.
 
     Args:
         result: list of tuples of Paths. If the second Path is None, the file could not be processed.
         all_paths: list of all paths that should have been processed
@@ -57,15 +58,16 @@
     processed_paths = [x[1] for x in result if x[1]]
     if len(processed_paths) == len(all_paths):
         success = True
         print(f"{datetime.now()}: Number of processed files: {len(result)}: Okay")
         logger.info(f"Number of processed files: {len(result)}: Okay")
     else:
         success = False
-        msg = f"Some files could not be processed: Only {len(processed_paths)}/{len(all_paths)} were processed. The failed ones are:"
+        ratio = f"{len(processed_paths)}/{len(all_paths)}"
+        msg = f"Some files could not be processed: Only {ratio} were processed. The failed ones are:"
         print(f"{datetime.now()}: ERROR: {msg}")
         logger.error(msg)
 
     for input_file, output_file in result:
         if not output_file:
             print(f" - {input_file}")
             logger.error(f" - {input_file}")
@@ -73,70 +75,82 @@
     return success
 
 
 def _process_files_in_parallel(
     paths: list[Path],
     input_dir: Path,
     output_dir: Path,
-    nthreads: Optional[int]
-) -> list[tuple[Path, Optional[Path]]]:
+    nthreads: Optional[int],
+) -> tuple[list[tuple[Path, Optional[Path]]], list[Path]]:
     """
     Creates a thread pool and executes the file processing in parallel.
+    If a Docker API error occurs, the SIPI container is restarted,
+    and the unprocessed files are returned,
+    so that this function can be called again with the unprocessed files.
 
     Args:
         paths: a list of all paths to the files that should be processed
         input_dir: the root directory of the input files
         output_dir: the directory where the processed files should be written to
         nthreads: number of threads to use for processing
 
     Returns:
-        a list of tuples with the original file path and the path to the processed file.
-        If a file could not be processed, the second path is None.
+        - a list of tuples with the original file path and the path to the processed file.
+          (if a file could not be processed, the second path is None)
+        - a list of all paths that could not be processed
+          (this list will only have content if a Docker API error led to a restart of the SIPI container)
     """
     with ThreadPoolExecutor(max_workers=nthreads) as pool:
-        processing_jobs = [pool.submit(
-            _process_file,
-            input_file,
-            input_dir,
-            output_dir
-        ) for input_file in paths]
+        processing_jobs = [pool.submit(_process_file, input_file, input_dir, output_dir) for input_file in paths]
 
     orig_filepath_2_uuid: list[tuple[Path, Optional[Path]]] = []
     for processed in as_completed(processing_jobs):
-        orig_filepath_2_uuid.append(processed.result())
+        try:
+            orig_filepath_2_uuid.append(processed.result())
+        except docker.errors.APIError:
+            print(f"{datetime.now()}: ERROR: A Docker exception occurred. Cancel jobs and restart SIPI...")
+            logger.error("A Docker exception occurred. Cancel jobs and restart SIPI...", exc_info=True)
+            for job in processing_jobs:
+                job.cancel()
+            _stop_and_remove_sipi_container()
+            _start_sipi_container_and_mount_volumes(input_dir, output_dir)
+            processed_paths = [x[0] for x in orig_filepath_2_uuid]
+            unprocessed_paths = [x for x in paths if x not in processed_paths]
+            return orig_filepath_2_uuid, unprocessed_paths
 
-    return orig_filepath_2_uuid
+    return orig_filepath_2_uuid, []
 
 
 def _write_result_to_pkl_file(result: list[tuple[Path, Optional[Path]]]) -> bool:
     """
     Writes the processing result to a pickle file.
 
     Args:
         result: the result of the file processing
 
     Returns:
         true if successful, false otherwise
     """
     filename = "processing_result_" + datetime.now().strftime("%Y%m%d_%H%M%S") + ".pkl"
     try:
-        with open(filename, 'wb') as pkl_file:
+        with open(filename, "wb") as pkl_file:
             pickle.dump(result, pkl_file)
         print(f"{datetime.now()}: The result was written to: {filename}")
         return True
     except OSError:
-        print(f"{datetime.now()}: An error occurred while writing the result to the pickle file. Content of file: {result}")
-        logger.error(f"An error occurred while writing the result to the pickle file. Content of file: {result}", exc_info=True)
+        err_msg = f"An error occurred while writing the result to the pickle file. Content of file: {result}"
+        print(f"{datetime.now()}: {err_msg}")
+        logger.error(err_msg, exc_info=True)
         return False
 
 
 def _check_params(
     input_dir: str,
     out_dir: str,
-    xml_file: str
+    xml_file: str,
 ) -> Optional[tuple[Path, Path, Path]]:
     """
     Checks the input parameters provided by the user and transforms them into the expected types.
 
     Args:
         input_dir: the root directory of the input files
         out_dir: the output directory where the created files should be written to
@@ -164,109 +178,101 @@
 
     return input_dir_path, out_dir_path, xml_file_path
 
 
 def _get_file_paths_from_xml(xml_file: Path) -> list[Path]:
     """
     Parse XML file to get all file paths.
+    If the same file is referenced several times in the XML,
+    it is only returned once.
 
     Args:
         xml_file: path to the XML file
 
+    Raises:
+        BaseError: if a referenced file doesn't exist in the file system
+
     Returns:
         list of all paths in the <bitstream> tags
     """
     tree: etree._ElementTree = etree.parse(xml_file)  # type: ignore
-    bitstream_paths: list[Path] = []
+    bitstream_paths: set[Path] = set()
     for x in tree.iter():
         if x.text and etree.QName(x).localname.endswith("bitstream"):
-            if Path(x.text).is_file():
-                bitstream_paths.append(Path(x.text))
+            path = Path(x.text)
+            if path.is_file():
+                bitstream_paths.add(path)
             else:
-                print(f"{datetime.now()}: ERROR: '{x.text}' is referenced in the XML file, but it doesn't exist. Skipping...")
-                logger.error(f"'{x.text}' is referenced in the XML file, but it doesn't exist. Skipping...")
+                err_msg = f"'{path}' is referenced in the XML file, but it doesn't exist. Skipping..."
+                print(f"{datetime.now()}: ERROR: {err_msg}")
+                logger.error(err_msg)
 
-    return bitstream_paths
+    return list(bitstream_paths)
 
 
 def _start_sipi_container_and_mount_volumes(
     input_dir: Path,
-    output_dir: Path
+    output_dir: Path,
 ) -> None:
     """
-    Creates and starts a Sipi container from the provided image. 
-    Checks first if it already exists and if yes, 
+    Creates and starts a Sipi container from the provided image.
+    Checks first if it already exists and if yes,
     if it is already running.
 
     Args:
         input_dir: the root directory of the images that should be processed, is mounted into the container
         output_dir: the output directory where the processed files should be written to, is mounted into the container
     """
+    # prepare parameters for container creation
     container_name = "sipi"
     volumes = [
         f"{input_dir.absolute()}:/sipi/processing-input",
-        f"{output_dir.absolute()}:/sipi/processing-output"
+        f"{output_dir.absolute()}:/sipi/processing-output",
     ]
     entrypoint = ["tail", "-f", "/dev/null"]
     docker_client = docker.from_env()
 
-    # Docker container doesn't exist yet
+    # get container. if it doesn't exist: create and run it
     try:
-        container: Container = docker_client.containers.get(container_name)    # pyright: ignore
-    except docker.errors.NotFound:                                             # pyright: ignore
-        docker_client.containers.run(image="daschswiss/sipi:3.8.1", name=container_name, volumes=volumes, entrypoint=entrypoint, detach=True)
+        container: Container = docker_client.containers.get(container_name)
+    except docker.errors.NotFound:
+        docker_client.containers.run(
+            image="daschswiss/sipi:3.8.1",
+            name=container_name,
+            volumes=volumes,
+            entrypoint=entrypoint,
+            detach=True,
+        )
+        container = docker_client.containers.get(container_name)
         print(f"{datetime.now()}: Created and started Sipi container '{container_name}'.")
         logger.info(f"Created and started Sipi container '{container_name}'.")
-        return
 
-    # Docker container exists
-    if not container:
-        container_running = False
-    elif not container.attrs:
-        container_running = False
-    elif not container.attrs.get("State", {}).get("Running"):
-        container_running = False
-    else:
-        container_running = True
-    if container_running:
-        print(f"{datetime.now()}: Found running Sipi container '{container_name}'.")
-        logger.info(f"Found running Sipi container '{container_name}'.")
-    else:
+    # the container exists. if it is not running, restart it
+    container_running = bool(container.attrs and container.attrs.get("State", {}).get("Running"))
+    if not container_running:
         container.restart()
-        print(f"{datetime.now()}: Restarted existing Sipi container '{container_name}'.")
-        logger.info(f"Restarted existing Sipi container '{container_name}'.")
-
-
-def _get_sipi_container() -> Optional[Container]:
-    """
-    Finds the locally running Sipi container (searches for container name "sipi")
 
-    Returns:
-        the reference to the Sipi container
-    """
-    docker_client = docker.from_env()
-    try:
-        return docker_client.containers.get("sipi")    # pyright: ignore
-    except docker.errors.NotFound:                     # pyright: ignore
-        print(f"{datetime.now()}: ERROR: Couldn't find a running Sipi container.")
-        logger.error("Couldn't find a running Sipi container.", exc_info=True)
-        return None
+    # make container globally available
+    global sipi_container
+    sipi_container = docker_client.containers.get(container_name)
+    print(f"{datetime.now()}: Sipi container is running.")
+    logger.info("Sipi container is running.")
 
 
 def _stop_and_remove_sipi_container() -> None:
     """
     Stop and remove the SIPI container.
     """
     if not sipi_container:
         return
     try:
         sipi_container.stop()
         sipi_container.remove()
         logger.info("Stopped and removed Sipi container.")
-    except docker.errors.APIError:  # pyright: ignore
+    except docker.errors.APIError:
         pass
 
 
 def _compute_sha256(file: Path) -> Optional[str]:
     """
     Calculates SHA256 checksum of a file
 
@@ -287,24 +293,26 @@
     return hash_sha256.hexdigest()
 
 
 def _convert_file_with_sipi(
     in_file_local_path: Path,
     input_dir: Path,
     out_file_local_path: Path,
-    output_dir: Path
+    output_dir: Path,
 ) -> bool:
     """
     Converts a file by calling a locally running Sipi container.
 
     Args:
         in_file_local_path: path to input file
         input_dir: the directory where the input files are located
-        out_file_local_path: path to output file, e.g. tmp/in/te/internal_file_name.jp2 if the internal filename is "internal_file_name"
-        output_dir: the directory where the processed files are written to, e.g. tmp/in/te/ if the internal filename is "internal_file_name"
+        out_file_local_path: path to output file,
+            e.g. tmp/in/te/internal_file_name.jp2 if the internal filename is "internal_file_name"
+        output_dir: the directory where the processed files are written to,
+            e.g. tmp/in/te/ if the internal filename is "internal_file_name"
     """
     original_output_dir = output_dir.parent.parent
     in_file_sipi_path = Path("processing-input") / in_file_local_path.relative_to(input_dir)
     out_file_sipi_path = Path("processing-output") / out_file_local_path.relative_to(original_output_dir)
 
     if not sipi_container:
         print(f"{datetime.now()}: ERROR: Cannot convert file {in_file_local_path} with Sipi: Sipi container not found.")
@@ -317,23 +325,24 @@
         return False
     return True
 
 
 def _create_orig_file(
     in_file: Path,
     internal_file_name: str,
-    out_dir: Path
+    out_dir: Path,
 ) -> bool:
     """
     Creates the .orig file expected by the API.
 
     Args:
         in_file: the input file from which the .orig should be created
         internal_file_name: the internal filename which should be used for the .orig file
-        out_dir: the directory where the .orig file should be written to, e.g. tmp/in/te/ if the internal filename is "internal_file_name"
+        out_dir: the directory where the .orig file should be written to,
+            e.g. tmp/in/te/ if the internal filename is "internal_file_name"
     """
     orig_ext = PurePath(in_file).suffix
     orig_file_full_path = Path(out_dir, f"{internal_file_name}{orig_ext}.orig")
     try:
         shutil.copyfile(in_file, orig_file_full_path)
         logger.info(f"Created .orig file {orig_file_full_path}")
         return True
@@ -353,41 +362,49 @@
     Returns:
         the metadata object as json
     """
     command_array = [
         "ffprobe",
         "-v",
         "error",
-        "-select_streams", "v:0",
+        "-select_streams",
+        "v:0",
         "-show_entries",
         "stream=width,height,bit_rate,duration,nb_frames,r_frame_rate",
-        "-print_format", "json",
+        "-print_format",
+        "json",
         "-i",
-        str(file_path)
+        str(file_path),
     ]
     try:
-        result = subprocess.run(command_array, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, check=False)
+        result = subprocess.run(
+            command_array,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            universal_newlines=True,
+            check=False,
+        )
     except Exception:  # pylint: disable=broad-exception-caught
         print(f"{datetime.now()}: ERROR: Exception occurred while running ffprobe for {file_path}")
         logger.error(f"Exception occurred while running ffprobe for {file_path}", exc_info=True)
         return None
     if result.returncode == 0:
         logger.info(f"Successfully ran ffprobe for {file_path}")
-        video_metadata: dict[str, Any] = json.loads(result.stdout)['streams'][0]  # get first stream
+        video_metadata: dict[str, Any] = json.loads(result.stdout)["streams"][0]  # get first stream
         return video_metadata
     else:
         print(f"{datetime.now()}: ERROR: Couldn't run ffprobe for {file_path}")
         logger.error(f"Couldn't run ffprobe for {file_path}")
         return None
 
 
 def _create_sidecar_file(
     orig_file: Path,
     converted_file: Path,
-    file_category: str
+    file_category: str,
 ) -> bool:
     """
     Creates the sidecar file for a given file. Depending on the file category, it adds category specific metadata.
 
     Args:
         orig_file: path to the original file
         converted_file: path to the converted file, e.g. out_dir/in/te/internal_filename.ext
@@ -415,15 +432,15 @@
     original_extension = PurePath(orig_file).suffix
     original_internal_filename = f"{random_part_of_filename}{original_extension}.orig"
     sidecar_dict: dict[str, Union[str, float]] = {
         "originalFilename": original_filename,
         "checksumOriginal": checksum_original,
         "checksumDerivative": checksum_derivative,
         "internalFilename": internal_filename,
-        "originalInternalFilename": original_internal_filename
+        "originalInternalFilename": original_internal_filename,
     }
 
     # add video specific metadata to sidecar file
     if file_category == "VIDEO":
         video_metadata = _get_video_metadata_with_ffprobe(converted_file)
         if not video_metadata:
             return False
@@ -464,15 +481,17 @@
     extensions["document"] = [".doc", ".docx", ".pdf", ".ppt", ".pptx", ".xls", ".xlsx"]
     extensions["audio"] = [".mp3", ".wav"]
 
     if file.suffix.lower() in extensions["video"]:
         category = "VIDEO"
     elif file.suffix.lower() in extensions["image"]:
         category = "IMAGE"
-    elif file.suffix.lower() in extensions["archive"] + extensions["text"] + extensions["document"] + extensions["audio"]:
+    elif file.suffix.lower() in (
+        extensions["archive"] + extensions["text"] + extensions["document"] + extensions["audio"]
+    ):
         category = "OTHER"
     else:
         category = None
         print(f"{datetime.now()}: ERROR: Couldn't get category for {file}")
         logger.error(f"Couldn't get category for {file}")
     return category
 
@@ -493,15 +512,15 @@
         return False
     else:
         return True
 
 
 def _ensure_directory_exists(path: Path) -> bool:
     """
-    Try to create the directory at the given path. 
+    Try to create the directory at the given path.
     If the directory already exists, nothing happens.
 
     Args:
         path: path to the directory that should be created
 
     Returns:
         True if the directory exists or was created successfully, False if an error occurred during the creation.
@@ -514,30 +533,31 @@
         logger.error(f"Couldn't create directory {path}", exc_info=True)
         return False
 
 
 def _process_file(
     in_file: Path,
     input_dir: Path,
-    output_dir: Path
+    output_dir: Path,
 ) -> tuple[Path, Optional[Path]]:
     """
     Creates all expected derivative files and writes the output into the provided output directory.
 
     In case of image: .orig file, JP2 derivate, sidecar file
     In case of video: .orig file, identical derivate file, sidecar file, folder with 1 preview image
     other files: .orig file, identical derivate file, sidecar file
 
     Args:
         in_file: path to input file that should be processed
         input_dir: root directory of the input files
-        output_dir: target location where the created files are written to, if the directory doesn't exist, it is created
+        output_dir: target location where the created files are written to.
+            If the directory doesn't exist, it is created
 
     Returns:
-        tuple consisting of the original path and the internal filename. 
+        tuple consisting of the original path and the internal filename.
         If there was an error, the internal filename is None.
     """
     # ensure that input file exists
     if not in_file.is_file():
         print(f"{datetime.now()}: ERROR: '{in_file}' does not exist. Skipping...")
         logger.error(f"'{in_file}' does not exist. Skipping...")
         return in_file, None
@@ -547,65 +567,66 @@
     out_dir_full = Path(output_dir, internal_filename[0:2], internal_filename[2:4])
     out_dir_full.mkdir(parents=True, exist_ok=True)
 
     # create .orig file
     if not _create_orig_file(
         in_file=in_file,
         internal_file_name=internal_filename,
-        out_dir=out_dir_full
+        out_dir=out_dir_full,
     ):
         return in_file, None
 
     # convert file (create derivative) and create sidecar file based on category (image, video or other)
     file_category = _get_file_category_from_extension(in_file)
     if not file_category:
         return in_file, None
 
     if file_category == "OTHER":
         result = _process_other_file(
             in_file=in_file,
             internal_filename=internal_filename,
-            out_dir=out_dir_full
+            out_dir=out_dir_full,
         )
     elif file_category == "IMAGE":
         result = _process_image_file(
             in_file=in_file,
             internal_filename=internal_filename,
             out_dir=out_dir_full,
-            input_dir=input_dir
+            input_dir=input_dir,
         )
     elif file_category == "VIDEO":
         result = _process_video_file(
             in_file=in_file,
             internal_filename=internal_filename,
-            out_dir=out_dir_full
+            out_dir=out_dir_full,
         )
     else:
-        print(f"{datetime.now()}: ERROR: Unexpected file category: {file_category}")
-        logger.error(f"Unexpected file category: {file_category}")
+        print(f"{datetime.now()}: ERROR: Unexpected file category for {in_file}: {file_category}")
+        logger.error(f"Unexpected file category for {in_file}: {file_category}")
         return in_file, None
 
     return result
 
 
 def _process_other_file(
     in_file: Path,
     internal_filename: str,
-    out_dir: Path
+    out_dir: Path,
 ) -> tuple[Path, Optional[Path]]:
     """
     Processes a file of file category OTHER.
-    There is no real derivate created, 
-    but the original file is copied, 
+    There is no real derivate created,
+    but the original file is copied,
     and a sidecar file is created.
 
     Args:
         in_file: the input file that should be processed
         internal_filename: the internal filename that should be used for the output file
-        out_dir: the output directory where the processed file should be written to, e.g. tmp/in/te/ if the internal filename is "internal_file_name"
+        out_dir: the output directory where the processed file should be written to,
+            e.g. tmp/in/te/ if the internal filename is "internal_file_name"
 
     Returns:
         a tuple of the original file path and the path to the processed file.
         If there was an error, the internal filename is None.
     """
     converted_file_full_path = out_dir / Path(internal_filename).with_suffix(in_file.suffix)
     try:
@@ -613,75 +634,77 @@
     except Exception:  # pylint: disable=broad-exception-caught
         print(f"{datetime.now()}: ERROR: Couldn't process file of category OTHER: {in_file}")
         logger.error(f"Couldn't process file of category OTHER: {in_file}", exc_info=True)
         return in_file, None
     if not _create_sidecar_file(
         orig_file=in_file,
         converted_file=converted_file_full_path,
-        file_category="OTHER"
+        file_category="OTHER",
     ):
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for: {in_file}")
         logger.error(f"Couldn't create sidecar file for: {in_file}")
         return in_file, None
     return in_file, converted_file_full_path
 
 
 def _process_image_file(
     in_file: Path,
     internal_filename: str,
     out_dir: Path,
-    input_dir: Path
+    input_dir: Path,
 ) -> tuple[Path, Optional[Path]]:
     """
     Processes a file of file category IMAGE
 
     Args:
         in_file: the input file that should be processed
         internal_filename: the internal filename that should be used for the output file
-        out_dir: the output directory where the processed file should be written to, e.g. tmp/in/te/ if the internal filename is "internal_file_name"
+        out_dir: the output directory where the processed file should be written to,
+            e.g. tmp/in/te/ if the internal filename is "internal_file_name"
         input_dir: root directory of the input files
 
     Returns:
         a tuple of the original file path and the path to the processed file.
         If there was an error, the internal filename is None.
     """
     converted_file_full_path = out_dir / Path(internal_filename).with_suffix(".jp2")
     sipi_result = _convert_file_with_sipi(
         in_file_local_path=in_file,
         input_dir=input_dir,
         out_file_local_path=converted_file_full_path,
-        output_dir=out_dir
+        output_dir=out_dir,
     )
     if not sipi_result:
         print(f"{datetime.now()}: ERROR: Couldn't process file of category IMAGE: {in_file}")
         logger.error(f"Couldn't process file of category IMAGE: {in_file}")
         return in_file, None
     if not _create_sidecar_file(
         orig_file=in_file,
         converted_file=converted_file_full_path,
-        file_category="IMAGE"
+        file_category="IMAGE",
     ):
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for: {in_file}")
         logger.error(f"Couldn't create sidecar file for: {in_file}")
         return in_file, None
     return in_file, converted_file_full_path
 
 
 def _process_video_file(
     in_file: Path,
     internal_filename: str,
-    out_dir: Path
+    out_dir: Path,
 ) -> tuple[Path, Optional[Path]]:
     """
     Processes a file of file category VIDEO
 
     Args:
         in_file: the input file that should be processed
         internal_filename: the internal filename that should be used for the output file
-        out_dir: the output directory where the processed file should be written to, e.g. tmp/in/te/ if the internal filename is "internal_file_name"
+        out_dir: the output directory where the processed file should be written to,
+            e.g. tmp/in/te/ if the internal filename is "internal_file_name"
 
     Returns:
         a tuple of the original file path and the path to the processed file.
         If there was an error, the internal filename is None.
     """
     converted_file_full_path = out_dir / Path(internal_filename).with_suffix(in_file.suffix)
     # create derivate file (identical to original file)
@@ -699,33 +722,65 @@
         logger.error(f"Couldn't create preview image for video '{in_file}'")
         return in_file, None
 
     # create sidecar file
     if not _create_sidecar_file(
         orig_file=in_file,
         converted_file=converted_file_full_path,
-        file_category="VIDEO"
+        file_category="VIDEO",
     ):
         print(f"{datetime.now()}: ERROR: Couldn't create sidecar file for video '{in_file}'")
         logger.error(f"Couldn't create sidecar file for video '{in_file}'")
         return in_file, None
 
     return in_file, converted_file_full_path
 
 
+def handle_interruption(
+    all_paths: list[Path],
+    processed_paths: list[Path],
+    exception: BaseException,
+) -> None:
+    """
+    Handles an interruption of the processing.
+    Writes the processed and unprocessed files into two files,
+    and exits the program with exit code 1.
+
+    Args:
+        all_paths: list of all paths that should be processed
+        processed_paths: list of all paths that were processed successfully
+        exception: the exception that was raised
+    """
+    unprocessed_paths = [x for x in all_paths if x not in processed_paths]
+    with open("unprocessed_files.txt", "w", encoding="utf-8") as f:
+        f.write("\n".join([str(x) for x in unprocessed_paths]))
+    with open("processed_files.txt", "w", encoding="utf-8") as f:
+        f.write("\n".join([str(x) for x in processed_paths]))
+
+    msg = (
+        "An error occurred while processing the files. "
+        "2 files were written, listing the processed and the unprocessed files:\n"
+        " - 'processed_files.txt'\n - 'unprocessed_files.txt'."
+    )
+    print(f"{datetime.now()}: ERROR: {msg}. The exception was: {exception}")
+    logger.error(msg, exc_info=exception)
+
+    sys.exit(1)
+
+
 def process_files(
     input_dir: str,
     output_dir: str,
     xml_file: str,
-    nthreads: Optional[int]
+    nthreads: Optional[int],
 ) -> bool:
     """
     Process the files referenced in the given XML file.
-    Writes the processed files 
-    (derivative, .orig file, sidecar file, as well as the preview file for movies) 
+    Writes the processed files
+    (derivative, .orig file, sidecar file, as well as the preview file for movies)
     to the given output directory.
     Additionally, writes a pickle file containing the mapping between the original files and the processed files,
     e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
 
     Args:
         input_dir: path to the directory where the files should be read from
         output_dir: path to the directory where the transformed / created files should be written to
@@ -735,61 +790,72 @@
     Returns:
         success status
     """
     # check the input parameters
     param_check_result = _check_params(
         input_dir=input_dir,
         out_dir=output_dir,
-        xml_file=xml_file
+        xml_file=xml_file,
     )
     if param_check_result:
         input_dir_path, output_dir_path, xml_file_path = param_check_result
     else:
         raise BaseError("Error reading the input parameters. Please check them.")
 
     # startup the SIPI container
     _start_sipi_container_and_mount_volumes(
         input_dir=input_dir_path,
-        output_dir=output_dir_path
+        output_dir=output_dir_path,
     )
-    global sipi_container
-    sipi_container = _get_sipi_container()
 
     # get the paths of the files referenced in the XML file
     all_paths = _get_file_paths_from_xml(xml_file_path)
     print(f"{datetime.now()}: Found {len(all_paths)} bitstreams in the XML file.")
     logger.info(f"Found {len(all_paths)} bitstreams in the XML file.")
 
     # get shell script for processing video files
     if any(path.suffix == ".mp4" for path in all_paths):
         _get_export_moving_image_frames_script()
 
     # process the files in parallel
     start_time = datetime.now()
     print(f"{start_time}: Start local file processing...")
     logger.info("Start local file processing...")
-    result = _process_files_in_parallel(
-        paths=all_paths,
-        input_dir=input_dir_path,
-        output_dir=output_dir_path,
-        nthreads=nthreads
-    )
+    processed_files = []
+    unprocessed_files = all_paths
+    while unprocessed_files:
+        try:
+            result, unprocessed_files = _process_files_in_parallel(
+                paths=all_paths,
+                input_dir=input_dir_path,
+                output_dir=output_dir_path,
+                nthreads=nthreads,
+            )
+            processed_files.extend(result)
+        except BaseException as exc:  # pylint: disable=broad-exception-caught
+            handle_interruption(
+                all_paths=all_paths,
+                processed_paths=[x[1] for x in processed_files if x and x[1]],
+                exception=exc,
+            )
 
     # check if all files were processed
     end_time = datetime.now()
     print(f"{end_time}: Processing files took: {end_time - start_time}")
     logger.info(f"{end_time}: Processing files took: {end_time - start_time}")
     success = _check_if_all_files_were_processed(
-        result=result,
-        all_paths=all_paths
+        result=processed_files,
+        all_paths=all_paths,
     )
 
     # write pickle file
-    if not _write_result_to_pkl_file(result):
+    if not _write_result_to_pkl_file(processed_files):
         success = False
-        print(f"{datetime.now()}: An error occurred while writing the result to the pickle file. The result was: {result}")
-        logger.error(f"An error occurred while writing the result to the pickle file. The result was: {result}")
+        err_msg = f"An error occurred while writing the result to the pickle file. The result was: {processed_files}"
+        print(f"{datetime.now()}: {err_msg}")
+        logger.error(err_msg)
 
     # remove the SIPI container
-    _stop_and_remove_sipi_container()
+    if success:
+        _stop_and_remove_sipi_container()
 
     return success
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_files.py` & `dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/upload_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,49 +14,55 @@
 from dsp_tools.utils.shared import login
 
 logger = get_logger(__name__)
 
 
 def _get_upload_candidates(
     dir_with_processed_files: Path,
-    internal_filename_of_processed_file: Path
+    internal_filename_of_processed_file: Path,
 ) -> list[Path]:
     """
     Based on the base derivate file, get all files based on the same uuid.
     For example, if the base derivate file is tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.jp2,
     the upload candidates are:
     - derivate: tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.jp2
     - original: tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.png.orig
     - sidecar:  tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.info
 
-    In case of video files, there is a preview file in addition to the above files: 
+    In case of video files, there is a preview file in addition to the above files:
      - tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146/1ffbbb30-77e8-414c-94ff-7e1c060f9146_m_0.jpg
 
     Args:
         dir_with_processed_files: path to the directory where the processed files are located
         internal_filename_of_processed_file: processed file (uuid filename)
 
     Returns:
         list of all processed files that belong to the same original file
     """
     upload_candidates: list[str] = []
-    upload_candidates.extend(glob.glob(f"{dir_with_processed_files}/**/**/{internal_filename_of_processed_file.stem}/*.*"))
-    upload_candidates.extend(glob.glob(f"{dir_with_processed_files}/**/**/{internal_filename_of_processed_file.stem}*.*"))
+    upload_candidates.extend(
+        glob.glob(f"{dir_with_processed_files}/**/**/{internal_filename_of_processed_file.stem}/*.*")
+    )
+    upload_candidates.extend(
+        glob.glob(f"{dir_with_processed_files}/**/**/{internal_filename_of_processed_file.stem}*.*")
+    )
     upload_candidates_paths = [Path(c) for c in upload_candidates]
     upload_candidates_as_str = "\n - " + "\n - ".join([str(c) for c in upload_candidates])
-    logger.info(f"Found the following upload candidates for {internal_filename_of_processed_file}: {upload_candidates_as_str}")
+    logger.info(
+        f"Found the following upload candidates for {internal_filename_of_processed_file}: {upload_candidates_as_str}"
+    )
     return upload_candidates_paths
 
 
 def _check_upload_candidates(
     internal_filename_of_processed_file: Path,
-    upload_candidates: list[Path]
+    upload_candidates: list[Path],
 ) -> bool:
     """
-    Make sure that all upload candidates exist, 
+    Make sure that all upload candidates exist,
     and that there are at least 5 candidates for videos and 3 candidates for all other file types.
 
     Args:
         internal_filename_of_processed_file: base derivate file (uuid filename)
         upload_candidates: list of all files that belong to the same original file
 
     Returns:
@@ -64,37 +70,38 @@
     """
     if not internal_filename_of_processed_file.is_file():
         print(f"{datetime.now()}: ERROR: The input file '{internal_filename_of_processed_file}' was not found.")
         logger.error(f"The input file '{internal_filename_of_processed_file}' was not found.")
         return False
 
     if not all(Path(c).is_file() for c in upload_candidates):
-        print(f"{datetime.now()}: ERROR: Not all upload candidates were found for file {internal_filename_of_processed_file}")
-        logger.error(f"Not all upload candidates were found for file {internal_filename_of_processed_file}")
+        err_msg = f"Not all upload candidates were found for file {internal_filename_of_processed_file}"
+        print(f"{datetime.now()}: ERROR: {err_msg}")
+        logger.error(err_msg)
         return False
 
     min_num_of_candidates = 4 if internal_filename_of_processed_file.suffix == ".mp4" else 3
     if len(upload_candidates) < min_num_of_candidates:
-        upload_candidates_as_str = "\n - " + "\n - ".join([str(c) for c in upload_candidates])
-        msg = f"Found the following files for {internal_filename_of_processed_file}, but more were expected: {upload_candidates_as_str}"
+        cand = "\n - " + "\n - ".join([str(c) for c in upload_candidates])
+        msg = f"Found the following files for {internal_filename_of_processed_file}, but more were expected: {cand}"
         print(f"{datetime.now()}: ERROR: {msg}")
         logger.error(msg)
         return False
 
     logger.info(f"Upload candidates for {internal_filename_of_processed_file} are okay.")
     return True
 
 
 def _upload_without_processing(
     file: Path,
     sipi_url: str,
-    con: Connection
+    con: Connection,
 ) -> bool:
     """
-    Send a single file to the "upload_without_processing" route. 
+    Send a single file to the "upload_without_processing" route.
 
     Args:
         file: file to upload
         sipi_url: URL to the sipi server
         con: connection to the DSP server
 
     Returns:
@@ -102,74 +109,78 @@
     """
     try:
         with open(file, "rb") as bitstream:
             try:
                 response_upload = requests.post(
                     url=f"{regex.sub(r'/$', '', sipi_url)}/upload_without_processing?token={con.get_token()}",
                     files={"file": bitstream},
-                    timeout=8*60
+                    timeout=8 * 60,
                 )
             except Exception:  # pylint: disable=broad-exception-caught
-                print(f"{datetime.now()}: ERROR: An exception was raised while calling the /upload_without_processing route for the file {file}")
-                logger.error(f"An exception was raised while calling the /upload_without_processing route for the file {file}", exc_info=True)
+                err_msg = f"An exception was raised while calling the /upload_without_processing route for {file}"
+                print(f"{datetime.now()}: ERROR: {err_msg}")
+                logger.error(err_msg, exc_info=True)
                 return False
     except Exception:  # pylint: disable=broad-exception-caught
-        print(f"{datetime.now()}: ERROR: Cannot send file to /upload_without_processing route, because the file cannot be opened: {file}")
-        logger.error(f"Cannot send file to /upload_without_processing route, because the file cannot be opened: {file}", exc_info=True)
+        err_msg = f"Cannot send file to /upload_without_processing route, because the file cannot be opened: {file}"
+        print(f"{datetime.now()}: ERROR: {err_msg}")
+        logger.error(err_msg, exc_info=True)
         return False
 
     if response_upload.json().get("message") == "server.fs.mkdir() failed: File exists":
         # This error can be safely ignored, since the file was uploaded correctly.
         logger.info(f"In spite of 'server.fs.mkdir() failed: File exists', successfully uploaded file {file}")
     elif response_upload.status_code != 200:
-        print(f"{datetime.now()}: ERROR: An error occurred while uploading the file {file}. The response was {response_upload.json()}")
-        logger.error(f"An error occurred while uploading the file {file}. The response was {response_upload.json()}")
+        err_msg = f"An error occurred while uploading the file {file}. The response was {response_upload.json()}"
+        print(f"{datetime.now()}: ERROR: {err_msg}")
+        logger.error(err_msg)
         return False
     else:
         logger.info(f"Successfully uploaded file {file}")
 
     return True
 
 
 def _upload_file(
     dir_with_processed_files: Path,
     internal_filename_of_processed_file: Path,
     sipi_url: str,
-    con: Connection
+    con: Connection,
 ) -> tuple[Path, bool]:
     """
     Retrieves all derivatives of one file and uploads them to the SIPI server.
 
     Args:
         dir_with_processed_files: path to the directory where the processed files are located
-        internal_filename_of_processed_file: path to the derivate of the original file, i.e. the processed file (uuid filename)
+        internal_filename_of_processed_file: path to the derivate of the original file,
+            i.e. the processed file (uuid filename)
         sipi_url: URL to the sipi server
         con: connection to the DSP server
 
     Returns:
         tuple with the processed file and a boolean indicating if the upload was successful
     """
     upload_candidates = _get_upload_candidates(
         dir_with_processed_files=dir_with_processed_files,
-        internal_filename_of_processed_file=internal_filename_of_processed_file
+        internal_filename_of_processed_file=internal_filename_of_processed_file,
     )
 
     check_result = _check_upload_candidates(
         internal_filename_of_processed_file=internal_filename_of_processed_file,
-        upload_candidates=upload_candidates
+        upload_candidates=upload_candidates,
     )
     if not check_result:
         return internal_filename_of_processed_file, False
 
     results: list[bool] = []
     for candidate in upload_candidates:
         res = _upload_without_processing(
             file=candidate,
             sipi_url=sipi_url,
-            con=con
+            con=con,
         )
         results.append(res)
 
     if not all(results):
         logger.error(f"Could not upload all files for {internal_filename_of_processed_file}.")
         return internal_filename_of_processed_file, False
     else:
@@ -183,15 +194,15 @@
 
     Args:
         pkl_file: pickle file returned by the processing step
 
     Returns:
         list of uuid file paths
     """
-    with open(pkl_file, 'rb') as file:
+    with open(pkl_file, "rb") as file:
         orig_paths_2_processed_paths: list[tuple[Path, Optional[Path]]] = pickle.load(file)
 
     processed_paths: list[Path] = []
     for orig_processed in orig_paths_2_processed_paths:
         if orig_processed[1]:
             processed_paths.append(orig_processed[1])
         else:
@@ -199,15 +210,15 @@
             logger.warning(f"There is no processed file for {orig_processed[0]}")
 
     return processed_paths
 
 
 def _check_params(
     pkl_file: str,
-    dir_with_processed_files: str
+    dir_with_processed_files: str,
 ) -> Optional[tuple[Path, Path]]:
     """
     Checks the input parameters provided by the user and transforms them into the expected types.
 
     Args:
         pkl_file: the XML file the paths are extracted from
         processed_dir: the output directory where the created files should be written to
@@ -229,47 +240,51 @@
 
 
 def _upload_files_in_parallel(
     dir_with_processed_files: Path,
     internal_filenames_of_processed_files: list[Path],
     sipi_url: str,
     con: Connection,
-    nthreads: int
+    nthreads: int,
 ) -> list[tuple[Path, bool]]:
     """
     Use a ThreadPoolExecutor to upload the files in parallel.
 
     Args:
         dir_with_processed_files: path to the directory where the processed files are located
-        internal_filenames_of_processed_files: list of uuid filenames, each filename being the path to the derivate of the original file
+        internal_filenames_of_processed_files: list of uuid filenames,
+            each filename being the path to the derivate of the original file
         sipi_url: URL to the sipi server
         con: connection to the DSP server
         nthreads: number of threads to use for the upload (optimum depends on the number of CPUs on the server)
 
     Returns:
         _description_
     """
     with ThreadPoolExecutor(max_workers=nthreads) as pool:
-        upload_jobs = [pool.submit(
-            _upload_file,
-            dir_with_processed_files,
-            internal_filename_of_processed_file,
-            sipi_url,
-            con
-        ) for internal_filename_of_processed_file in internal_filenames_of_processed_files]
+        upload_jobs = [
+            pool.submit(
+                _upload_file,
+                dir_with_processed_files,
+                internal_filename_of_processed_file,
+                sipi_url,
+                con,
+            )
+            for internal_filename_of_processed_file in internal_filenames_of_processed_files
+        ]
 
     result: list[tuple[Path, bool]] = []
     for uploaded in as_completed(upload_jobs):
         result.append(uploaded.result())
     return result
 
 
 def _check_if_all_files_were_uploaded(
     result: list[tuple[Path, bool]],
-    internal_filenames_of_processed_files: list[Path]
+    internal_filenames_of_processed_files: list[Path],
 ) -> bool:
     """
     Print the files which could not be uploaded.
 
     Args:
         result: list of tuples with the path of the file and the success status
         internal_filenames_of_processed_files: list of files that should have been uploaded (uuid filenames)
@@ -279,16 +294,16 @@
     """
     if len(result) == len(internal_filenames_of_processed_files):
         success = True
         print(f"{datetime.now()}: Number of files of which the derivates were uploaded: {len(result)}: Okay")
         logger.info(f"Number of files of which the derivates were uploaded: {len(result)}: Okay")
     else:
         success = False
-        msg = f"Some derivates of some files could not be uploaded: Only {len(result)}/{len(internal_filenames_of_processed_files)} were uploaded. " \
-            "The failed ones are:"
+        ratio = f"{len(result)}/{len(internal_filenames_of_processed_files)}"
+        msg = f"Some derivates of some files could not be uploaded: Only {ratio} were uploaded. The failed ones are:"
         print(f"{datetime.now()}: ERROR: {msg}")
         logger.error(msg)
 
     for path, res in result:
         if not res:
             print(f" - {path} could not be uploaded.")
             logger.error(f"{path} could not be uploaded.")
@@ -299,37 +314,37 @@
 def upload_files(
     pkl_file: str,
     dir_with_processed_files: str,
     nthreads: int,
     user: str,
     password: str,
     dsp_url: str,
-    sipi_url: str
+    sipi_url: str,
 ) -> bool:
     """
     Uploads the processed files to the DSP server, using multithreading.
     Before using this method, the files must be processed by the processing step.
 
     Args:
         pkl_file: pickle file containing the mapping between the original files and the processed files,
-                  e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
+        e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
         dir_with_processed_files: path to the directory where the processed files are located
         nthreads: number of threads to use for uploading (optimum depends on the number of CPUs on the server)
         user: the user's e-mail for login into DSP
         password: the user's password for login into DSP
         dsp_url: URL to the DSP server
         sipi_url: URL to the Sipi server
 
     Returns:
         success status
     """
     # check the input parameters
     param_check_result = _check_params(
         pkl_file=pkl_file,
-        dir_with_processed_files=dir_with_processed_files
+        dir_with_processed_files=dir_with_processed_files,
     )
     if param_check_result:
         pkl_file_path, dir_with_processed_files_path = param_check_result
     else:
         raise BaseError("Error reading the input parameters. Please check them.")
 
     # read paths from pkl file
@@ -337,32 +352,32 @@
     print(f"{datetime.now()}: Found {len(internal_filenames_of_processed_files)} files to upload...")
     logger.info(f"Found {len(internal_filenames_of_processed_files)} files to upload...")
 
     # create connection to DSP
     con = login(
         server=dsp_url,
         user=user,
-        password=password
+        password=password,
     )
 
     # upload files in parallel
     start_time = datetime.now()
     print(f"{start_time}: Start file uploading...")
     logger.info("Start file uploading...")
     result = _upload_files_in_parallel(
         dir_with_processed_files=dir_with_processed_files_path,
         internal_filenames_of_processed_files=internal_filenames_of_processed_files,
         sipi_url=sipi_url,
         con=con,
-        nthreads=nthreads
+        nthreads=nthreads,
     )
 
     # check if all files were uploaded
     end_time = datetime.now()
     print(f"{datetime.now()}: Uploading files took {end_time - start_time}")
     logger.info(f"Uploading files took {end_time - start_time}")
     success = _check_if_all_files_were_uploaded(
         result=result,
-        internal_filenames_of_processed_files=internal_filenames_of_processed_files
+        internal_filenames_of_processed_files=internal_filenames_of_processed_files,
     )
 
     return success
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/fast_xmlupload/upload_xml.py` & `dsp_tools-2.3.3/src/dsp_tools/fast_xmlupload/upload_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     Args:
         pkl_file: pickle file returned by the processing step
 
     Returns:
         dict of original paths to uuid filenames
     """
-    with open(pkl_file, 'rb') as file:
+    with open(pkl_file, "rb") as file:
         orig_path_2_processed_path: list[tuple[Path, Optional[Path]]] = pickle.load(file)
 
     orig_path_2_uuid_filename: dict[str, str] = {}
     for orig_path, processed_path in orig_path_2_processed_path:
         if processed_path:
             orig_path_2_uuid_filename[str(orig_path)] = str(processed_path.name)
         else:
@@ -36,15 +36,15 @@
             )
 
     return orig_path_2_uuid_filename
 
 
 def replace_bitstream_paths(
     xml_tree: "etree._ElementTree[etree._Element]",
-    orig_path_2_uuid_filename: dict[str, str]
+    orig_path_2_uuid_filename: dict[str, str],
 ) -> "etree._ElementTree[etree._Element]":
     """
     Replace the original filepaths in the <bitstream> Tags by the uuid filenames of the processed files.
 
     Args:
         xml_tree: The parsed original XML tree
         orig_path_2_uuid_filename: Mapping from original filenames to uuid filenames (from the pickle file)
@@ -73,52 +73,55 @@
 
 def fast_xmlupload(
     xml_file: str,
     pkl_file: str,
     user: str,
     password: str,
     dsp_url: str,
-    sipi_url: str
+    sipi_url: str,
 ) -> bool:
     """
-    This function reads an XML file 
-    and imports the data described in it onto the DSP server, 
+    This function reads an XML file
+    and imports the data described in it onto the DSP server,
     using the fast XML upload method.
-    Before using this method, 
-    the original files must be processed by the processing step, 
+    Before using this method,
+    the original files must be processed by the processing step,
     and uploaded by the upoad step.
 
     Args:
         xml_file: path to XML file containing the resources
         pkl_file: pickle file containing the mapping between the original files and the processed files,
-                  e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2')
+        e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2')
         user: the user's e-mail for login into DSP
         password: the user's password for login into DSP
         dsp_url: URL to the DSP server
         sipi_url: URL to the Sipi server
 
     Returns:
         success status
     """
     xml_tree_orig = etree.parse(xml_file)
     orig_path_2_uuid_filename = _get_paths_from_pkl_file(pkl_file=Path(pkl_file))
-    xml_tree_replaced = replace_bitstream_paths(xml_tree=xml_tree_orig, orig_path_2_uuid_filename=orig_path_2_uuid_filename)
+    xml_tree_replaced = replace_bitstream_paths(
+        xml_tree=xml_tree_orig,
+        orig_path_2_uuid_filename=orig_path_2_uuid_filename,
+    )
 
     start_time = datetime.now()
     print(f"{start_time}: Start with fast XML upload...")
 
     xml_upload(
         input_file=xml_tree_replaced,
         server=dsp_url,
         user=user,
         password=password,
         imgdir=".",
         sipi=sipi_url,
         verbose=False,
         incremental=False,
         save_metrics=False,
-        preprocessing_done=True
+        preprocessing_done=True,
     )
 
     end_time = datetime.now()
     print(f"{end_time}: Total time of fast xml upload: {end_time - start_time}")
     return True
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/bitstream.py` & `dsp_tools-2.3.3/src/dsp_tools/models/bitstream.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 from dsp_tools.models.permission import Permissions
 
 
 class Bitstream:
     """
     Represents a bitstream object (file) which is attached to a resource
     """
+
     _value: str
     _permissions: Optional[Permissions]
 
-    def __init__(self,
-                 value: str,
-                 permissions: Optional[Permissions] = None):
+    def __init__(self, value: str, permissions: Optional[Permissions] = None):
         self._value = value
         self._permissions = permissions
 
     @property
     def value(self) -> str:
         return self._value
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/connection.py` & `dsp_tools-2.3.3/src/dsp_tools/models/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,63 +18,61 @@
         BaseError: If the status code of the response is not 200
     """
     if response.status_code != 200:
         raise BaseError(
             message="KNORA-ERROR: status code=" + str(response.status_code) + "\nMessage:" + response.text,
             status_code=response.status_code,
             json_content_of_api_response=response.text,
-            reason_from_api_response=response.reason,
-            api_route=response.url
+            reason_from_api=response.reason,
+            api_route=response.url,
         )
 
 
 class Connection:
     """
-    An Connection instance represents a connection to a Knora server.
+    An Connection instance represents a connection to a DSP server.
 
     Attributes
     ----------
 
     none (internal use attributes should not be modified/set directly)
     """
 
     _server: str
     _prefixes: Union[dict[str, str], None]
     _token: Union[str, None]
     _log: bool
 
     def __init__(self, server: str, prefixes: dict[str, str] = None):
         """
-        Constructor requiring the server address, the user and password of KNORA
+        Constructor requiring the server address, the user and password of DSP
         :param server: Address of the server, e.g https://api.dasch.swiss
         :param prefixes: Ontology prefixes used
         """
 
-        self._server = re.sub(r'\/$', '', server)
+        self._server = re.sub(r"\/$", "", server)
         self._prefixes = prefixes
         self._token = None
         self._log = False
 
     def login(self, email: str, password: str) -> None:
         """
-        Method to login into KNORA which creates a session token.
+        Method to login into DSP which creates a session token.
         :param email: Email of user, e.g., root@example.com
         :param password: Password of the user, e.g. test
         """
 
-        credentials = {
-            "email": email,
-            "password": password
-        }
+        credentials = {"email": email, "password": password}
         jsondata = json.dumps(credentials)
 
         response = requests.post(
-            self._server + '/v2/authentication',
-            headers={'Content-Type': 'application/json; charset=UTF-8'},
-            data=jsondata
+            self._server + "/v2/authentication",
+            headers={"Content-Type": "application/json; charset=UTF-8"},
+            data=jsondata,
+            timeout=5,
         )
         check_for_api_error(response)
         result = response.json()
         self._token = result["token"]
 
     def get_token(self) -> str:
         """
@@ -98,16 +96,17 @@
         """
         Performs a logout
         :return: None
         """
 
         if self._token is not None:
             response = requests.delete(
-                self._server + '/v2/authentication',
-                headers={'Authorization': 'Bearer ' + self._token}
+                self._server + "/v2/authentication",
+                headers={"Authorization": "Bearer " + self._token},
+                timeout=5,
             )
             check_for_api_error(response)
             self._token = None
 
     def __del__(self):
         pass
         # self.logout()
@@ -116,183 +115,169 @@
         """
         Post Json data to a given server using a HTTP POST request
         :param path: Path of RESTful route
         :param jsondata: Valid JSON as string
         :return: Response from server
         """
 
-        if path[0] != '/':
-            path = '/' + path
+        if path[0] != "/":
+            path = "/" + path
         headers = None
         if jsondata is None:
             if self._token is not None:
-                headers = {'Authorization': 'Bearer ' + self._token}
+                headers = {"Authorization": "Bearer " + self._token}
                 response = requests.post(
                     self._server + path,
-                    headers=headers
+                    headers=headers,
+                    timeout=5,
                 )
             else:
-                response = requests.post(self._server + path)
+                response = requests.post(self._server + path, timeout=5)
         else:
             if self._token is not None:
-                headers = {'Content-Type': 'application/json; charset=UTF-8',
-                           'Authorization': 'Bearer ' + self._token}
+                headers = {"Content-Type": "application/json; charset=UTF-8", "Authorization": "Bearer " + self._token}
                 response = requests.post(
                     self._server + path,
                     headers=headers,
-                    data=jsondata
+                    data=jsondata,
+                    timeout=5,
                 )
             else:
-                headers = {'Content-Type': 'application/json; charset=UTF-8'}
+                headers = {"Content-Type": "application/json; charset=UTF-8"}
                 response = requests.post(
                     self._server + path,
                     headers=headers,
-                    data=jsondata
+                    data=jsondata,
+                    timeout=5,
                 )
         if self._log:
             if jsondata:
                 jsonobj = json.loads(jsondata)
             else:
                 jsonobj = None
             logobj = {
                 "method": "POST",
                 "headers": headers,
                 "route": path,
                 "body": jsonobj,
                 "return-headers": dict(response.headers),
-                "return": response.json() if response.status_code == 200 else {"status": str(response.status_code),
-                                                                               "message": response.text}
+                "return": response.json()
+                if response.status_code == 200
+                else {"status": str(response.status_code), "message": response.text},
             }
-            tmp = path.split('/')
+            tmp = path.split("/")
             filename = "POST" + "_".join(tmp) + ".json"
-            with open(filename, 'w') as f:
+            with open(filename, "w", encoding="utf8") as f:
                 json.dump(logobj, f, indent=4)
         check_for_api_error(response)
         result = response.json()
         return result
 
     def get(self, path: str, headers: Optional[dict[str, str]] = None) -> dict[str, Any]:
         """
         Get data from a server using a HTTP GET request
         :param path: Path of RESTful route
         :param headers: ...
         :return: Response from server
         """
 
-        if path[0] != '/':
-            path = '/' + path
+        if path[0] != "/":
+            path = "/" + path
         if not self._token:
             if not headers:
-                response = requests.get(self._server + path)
+                response = requests.get(self._server + path, timeout=5)
             else:
-                response = requests.get(self._server + path, headers)
+                response = requests.get(self._server + path, headers, timeout=5)
         else:
             if not headers:
-                response = requests.get(self._server + path, headers={'Authorization': 'Bearer ' + self._token})
+                response = requests.get(
+                    self._server + path,
+                    headers={"Authorization": "Bearer " + self._token},
+                    timeout=5,
+                )
             else:
-                headers['Authorization'] = 'Bearer ' + self._token
-                response = requests.get(self._server + path, headers)
+                headers["Authorization"] = "Bearer " + self._token
+                response = requests.get(self._server + path, headers, timeout=5)
 
         check_for_api_error(response)
         json_response = response.json()
         return json_response
 
-    def put(self, path: str, jsondata: Optional[str] = None, content_type: str = 'application/json'):
+    def put(self, path: str, jsondata: Optional[str] = None, content_type: str = "application/json"):
         """
         Send data to a RESTful server using a HTTP PUT request
         :param path: Path of RESTful route
         :param jsondata: Valid JSON as string
         :param content_type: HTTP Content-Type [default: 'application/json']
         :return:
         """
 
-        if path[0] != '/':
-            path = '/' + path
+        if path[0] != "/":
+            path = "/" + path
         if jsondata is None:
             response = requests.put(
                 self._server + path,
-                headers={'Authorization': 'Bearer ' + self._token}
+                headers={"Authorization": "Bearer " + self._token},
+                timeout=5,
             )
         else:
             response = requests.put(
                 self._server + path,
-                headers={
-                    'Content-Type': content_type + '; charset=UTF-8',
-                    'Authorization': 'Bearer ' + self._token
-                },
-                data=jsondata)
+                headers={"Content-Type": content_type + "; charset=UTF-8", "Authorization": "Bearer " + self._token},
+                data=jsondata,
+                timeout=5,
+            )
         check_for_api_error(response)
         result = response.json()
         return result
 
     def delete(self, path: str, params: Optional[any] = None):
         """
         Send a delete request using the HTTP DELETE request
         :param path: Path of RESTful route
         :return: Response from server
         """
 
-        if path[0] != '/':
-            path = '/' + path
+        if path[0] != "/":
+            path = "/" + path
         if params is not None:
             response = requests.delete(
                 self._server + path,
-                headers={'Authorization': 'Bearer ' + self._token},
-                params=params
+                headers={"Authorization": "Bearer " + self._token},
+                params=params,
+                timeout=5,
             )
 
         else:
             response = requests.delete(
                 self._server + path,
-                headers={'Authorization': 'Bearer ' + self._token}
+                headers={"Authorization": "Bearer " + self._token},
+                timeout=5,
             )
         check_for_api_error(response)
         result = response.json()
         return result
 
     def reset_triplestore_content(self):
         rdfdata = [
-            {
-                "path": "./knora-ontologies/knora-admin.ttl",
-                "name": "http://www.knora.org/ontology/knora-admin"
-            },
-            {
-                "path": "./knora-ontologies/knora-base.ttl",
-                "name": "http://www.knora.org/ontology/knora-base"
-            },
-            {
-                "path": "./knora-ontologies/standoff-onto.ttl",
-                "name": "http://www.knora.org/ontology/standoff"
-            },
-            {
-                "path": "./knora-ontologies/standoff-data.ttl",
-                "name": "http://www.knora.org/data/standoff"
-            },
-            {
-                "path": "./knora-ontologies/salsah-gui.ttl",
-                "name": "http://www.knora.org/ontology/salsah-gui"
-            },
-            {
-                "path": "./_test_data/all_data/admin-data.ttl",
-                "name": "http://www.knora.org/data/admin"
-            },
-            {
-                "path": "./_test_data/all_data/permissions-data.ttl",
-                "name": "http://www.knora.org/data/permissions"
-            },
-            {
-                "path": "./_test_data/all_data/system-data.ttl",
-                "name": "http://www.knora.org/data/0000/SystemProject"
-            }
+            {"path": "./knora-ontologies/knora-admin.ttl", "name": "http://www.knora.org/ontology/knora-admin"},
+            {"path": "./knora-ontologies/knora-base.ttl", "name": "http://www.knora.org/ontology/knora-base"},
+            {"path": "./knora-ontologies/standoff-onto.ttl", "name": "http://www.knora.org/ontology/standoff"},
+            {"path": "./knora-ontologies/standoff-data.ttl", "name": "http://www.knora.org/data/standoff"},
+            {"path": "./knora-ontologies/salsah-gui.ttl", "name": "http://www.knora.org/ontology/salsah-gui"},
+            {"path": "./_test_data/all_data/admin-data.ttl", "name": "http://www.knora.org/data/admin"},
+            {"path": "./_test_data/all_data/permissions-data.ttl", "name": "http://www.knora.org/data/permissions"},
+            {"path": "./_test_data/all_data/system-data.ttl", "name": "http://www.knora.org/data/0000/SystemProject"},
         ]
         jsondata = json.dumps(rdfdata)
-        url = self._server + '/admin/store/ResetTriplestoreContent?prependdefaults=false'
+        url = self._server + "/admin/store/ResetTriplestoreContent?prependdefaults=false"
 
         response = requests.post(
             url,
-            headers={'Content-Type': 'application/json; charset=UTF-8'},
-            data=jsondata
+            headers={"Content-Type": "application/json; charset=UTF-8"},
+            data=jsondata,
+            timeout=5,
         )
         check_for_api_error(response)
         res = response.json()
         #  pprint(res)
         return res
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/exceptions.py` & `dsp_tools-2.3.3/src/dsp_tools/models/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,74 +4,86 @@
 
 
 class BaseError(Exception):
     """
     A basic error class for DSP-TOOLS.
 
     Attributes:
+
         message: A message that describes the error
-        status_code: HTTP status code of the response from DSP-API (only applicable if the error comes from DSP-API)
-        json_content_of_api_response: The message that DSP-API returns (only applicable if the error comes from DSP-API)
-        original_error_msg_from_api: The original error message that DSP-API returns (only applicable if the error comes from DSP-API)
-        reason_from_api_response: The reason for the failure that DSP-API returns (only applicable if the error comes from DSP-API)
+        status_code: HTTP status code of the response from DSP-API (only applicable if error comes from DSP-API)
+        json_content_of_api_response: The message that DSP-API returns (only applicable if error comes from DSP-API)
+        orig_err_msg_from_api: Original error message that DSP-API returns (only applicable if error comes from DSP-API)
+        reason_from_api: Reason for the failure that DSP-API returns (only applicable if error comes from DSP-API)
         api_route: The route that was called (only applicable if the error comes from DSP-API)
     """
+
     message: str
     status_code: Optional[int]
     json_content_of_api_response: Optional[str]
-    original_error_msg_from_api: Optional[str] = None
-    reason_from_api_response: Optional[str]
+    orig_err_msg_from_api: Optional[str] = None
+    reason_from_api: Optional[str]
     api_route: Optional[str]
 
     def __init__(
         self,
         message: str,
         status_code: Optional[int] = None,
         json_content_of_api_response: Optional[str] = None,
-        reason_from_api_response: Optional[str] = None,
-        api_route: Optional[str] = None
+        reason_from_api: Optional[str] = None,
+        api_route: Optional[str] = None,
     ) -> None:
         """
         A basic error class for DSP-TOOLS.
 
         Args:
             message: A message that describes the error
-            status_code: HTTP status code of the response from DSP-API (only applicable if the error comes from DSP-API)
-            json_content_of_api_response: The message that DSP-API returns (only applicable if the error comes from DSP-API)
-            reason_from_api_response: The reason for the failure that DSP-API returns (only applicable if the error comes from DSP-API)
+            status_code: HTTP status code of the response from DSP-API (only applicable if error comes from DSP-API)
+            json_content_of_api_response: The message that DSP-API returns (only applicable if error comes from DSP-API)
+            reason_from_api: Reason for the failure that DSP-API returns (only applicable if error comes from DSP-API)
             api_route: The route that was called (only applicable if the error comes from DSP-API)
         """
         super().__init__()
         self.message = message
         self.status_code = status_code
         if json_content_of_api_response:
             self.json_content_of_api_response = json_content_of_api_response
             try:
                 parsed_json = json.loads(json_content_of_api_response)
                 if "knora-api:error" in parsed_json:
                     knora_api_error = parsed_json["knora-api:error"]
                     knora_api_error = re.sub(r"^dsp\.errors\.[A-Za-z]+?: ?", "", knora_api_error)
-                    self.original_error_msg_from_api = knora_api_error
+                    self.orig_err_msg_from_api = knora_api_error
             except json.JSONDecodeError:
                 pass
-        self.reason_from_api_response = reason_from_api_response
+        self.reason_from_api = reason_from_api
         self.api_route = api_route
 
     def __str__(self) -> str:
         return self.message
 
 
 class InternalError(BaseError):
     """
     Class for errors that will be handled by a higher level function
     """
-    pass
 
 
 class UserError(BaseError):
     """
-    Class for errors that are intended for user feedback. 
-    Typically, a UserError is raised when the execution of a program must be interrupted 
+    Class for errors that are intended for user feedback.
+    Typically, a UserError is raised when the execution of a program must be interrupted
     due to a bad condition in the input data that prevents further processing.
     The message should be as user-friendly as possible.
     """
-    pass
+
+
+class XmlError(Exception):
+    """Represents an error raised in the context of the XML import"""
+
+    _message: str
+
+    def __init__(self, msg: str):
+        self._message = msg
+
+    def __str__(self) -> str:
+        return "XML-ERROR: " + self._message
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/group.py` & `dsp_tools-2.3.3/src/dsp_tools/models/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from __future__ import annotations
-
-import json
-from typing import Any, Optional, Union
-from urllib.parse import quote_plus
-
-from dsp_tools.models.connection import Connection
-from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.helpers import Actions
-from dsp_tools.models.langstring import LangString
-from dsp_tools.models.model import Model
-from dsp_tools.models.project import Project
-
 """
-This module implements the handling (CRUD) of Knora groups.
+This module implements the handling (CRUD) of DSP groups.
 
 CREATE:
     * Instantiate a new object of the class Group with all required parameters
     * Call the ``create``-method on the instance
 
 READ:
-    * Instantiate a new object with ``id``(IRI of group) given
+    * Instantiate a new object with ``iri``(IRI of group) given
     * Call the ``read``-method on the instance
     * Access the information that has been provided to the instance
 
 UPDATE:
     * You need an instance of an existing Project by reading an instance
     * Change the attributes by assigning the new values
     * Call the ``update```method on the instance
 
 DELETE
-    * Instantiate a new objects with ``id``(IRI of group) given, or use any instance that has the id set
+    * Instantiate a new objects with ``iri``(IRI of group) given, or use any instance that has the iri set
     * Call the ``delete``-method on the instance
 
 """
 
+from __future__ import annotations
+
+import json
+from typing import Any, Optional, Union
+from urllib.parse import quote_plus
+
+from dsp_tools.models.connection import Connection
+from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import Actions
+from dsp_tools.models.langstring import LangString
+from dsp_tools.models.model import Model
+from dsp_tools.models.project import Project
+
 
 class Group(Model):
     """
-    This class represents a Knora group
+    This class represents a DSP group
 
     Attributes
     ----------
 
     con : Connection
-        A connection instance to a Knora server
+        A connection instance to a DSP server
 
-    id : str
+    iri : str
         IRI of the group [get only, cannot be modified after creation of instance]
 
     name : str
         Name of the group
 
     descriptions : LangString
         Group descriptions in a given language (Languages.EN, Languages.DE, Languages.FR, Languages.IT, Languages.RM).
@@ -68,179 +68,183 @@
 
     PROJECT_MEMBER_GROUP: str = "http://www.knora.org/ontology/knora-admin#ProjectMember"
     PROJECT_ADMIN_GROUP: str = "http://www.knora.org/ontology/knora-admin#ProjectAdmin"
     PROJECT_SYSTEMADMIN_GROUP: str = "http://www.knora.org/ontology/knora-admin#SystemAdmin"
     ROUTE: str = "/admin/groups"
     ROUTE_SLASH: str = ROUTE + "/"
 
-    _id: str
+    _iri: Optional[str]
     _name: str
     _descriptions: LangString
     _project: str
     _selfjoin: bool
     _status: bool
 
-    def __init__(self,
-                 con: Connection,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None,
-                 descriptions: Optional[LangString] = None,
-                 project: Optional[Union[str, Project]] = None,
-                 selfjoin: Optional[bool] = None,
-                 status: Optional[bool] = None):
+    def __init__(
+        self,
+        con: Connection,
+        iri: Optional[str] = None,
+        name: Optional[str] = None,
+        descriptions: Optional[LangString] = None,
+        project: Optional[Union[str, Project]] = None,
+        selfjoin: Optional[bool] = None,
+        status: Optional[bool] = None,
+    ) -> None:
         super().__init__(con)
-        self._id = str(id) if id is not None else None
+        self._iri = iri
         self._name = str(name) if name is not None else None
         self._descriptions = LangString(descriptions)
         if project is not None and isinstance(project, Project):
             self._project = project.id
         else:
             self._project = str(project) if project is not None else None
         self._selfjoin = bool(selfjoin) if selfjoin is not None else None
         self._status = bool(status) if status is not None else None
 
     @property
-    def id(self) -> Optional[str]:
-        return self._id
+    def iri(self) -> Optional[str]:
+        return self._iri
 
-    @id.setter
-    def id(self, value: str) -> None:
-        raise BaseError('Group id cannot be modified!')
+    @iri.setter
+    def iri(self, value: str) -> None:
+        raise BaseError("Group iri cannot be modified!")
 
     @property
     def name(self) -> Optional[str]:
         return self._name
 
     @name.setter
     def name(self, value: str):
         self._name = value
-        self._changed.add('name')
+        self._changed.add("name")
 
     @property
     def descriptions(self) -> LangString:
         return self._descriptions
 
     @descriptions.setter
     def descriptions(self, value: Optional[LangString]) -> None:
         self._descriptions = LangString(value)
-        self._changed.add('descriptions')
+        self._changed.add("descriptions")
 
     @property
     def project(self):
         return self._project
 
     @project.setter
     def project(self, value: str):
-        raise BaseError('project id cannot be modified!')
+        raise BaseError("project id cannot be modified!")
 
     @property
     def selfjoin(self) -> bool:
         return self._selfjoin
 
     @selfjoin.setter
     def selfjoin(self, value: bool) -> None:
         self._selfjoin = value
-        self._changed.add('selfjoin')
+        self._changed.add("selfjoin")
 
     @property
     def status(self) -> bool:
         return self._status
 
     @status.setter
     def status(self, value: bool) -> None:
         self._status = value
-        self._changed.add('status')
+        self._changed.add("status")
 
     def has_changed(self) -> bool:
         if self._changed:
             return True
         else:
             return False
 
     @classmethod
     def fromJsonObj(cls, con: Connection, json_obj: Any):
-        group_id = json_obj.get('id')
+        group_id = json_obj.get("id")
         if group_id is None:
             raise BaseError('Group "id" is missing')
-        name = json_obj.get('name')
+        name = json_obj.get("name")
         if name is None:
             raise BaseError('Group "name" is missing')
-        descriptions = LangString.fromJsonObj(json_obj.get('descriptions'))
-        tmp = json_obj.get('project')
+        descriptions = LangString.fromJsonObj(json_obj.get("descriptions"))
+        tmp = json_obj.get("project")
         if tmp is None:
             raise BaseError('Group "project" is missing')
-        project = tmp.get('id')
+        project = tmp.get("id")
         if project is None:
             raise BaseError('Group "project" has no "id"')
-        selfjoin = json_obj.get('selfjoin')
+        selfjoin = json_obj.get("selfjoin")
         if selfjoin is None:
             raise BaseError("selfjoin is missing")
-        status = json_obj.get('status')
+        status = json_obj.get("status")
         if status is None:
             raise BaseError("Status is missing")
-        return cls(con=con,
-                   name=name,
-                   id=group_id,
-                   descriptions=descriptions,
-                   project=project,
-                   selfjoin=selfjoin,
-                   status=status)
+        return cls(
+            con=con,
+            name=name,
+            iri=group_id,
+            descriptions=descriptions,
+            project=project,
+            selfjoin=selfjoin,
+            status=status,
+        )
 
     def toJsonObj(self, action: Actions):
         tmp = {}
         if action == Actions.Create:
             if self._name is None:
                 raise BaseError("There must be a valid name!")
-            tmp['name'] = self._name
+            tmp["name"] = self._name
             if not self._descriptions.isEmpty():
-                tmp['descriptions'] = self._descriptions.toJsonObj()
+                tmp["descriptions"] = self._descriptions.toJsonObj()
             if self._project is None:
                 raise BaseError("There must be a valid project!")
-            tmp['project'] = self._project
+            tmp["project"] = self._project
             if self._selfjoin is None:
                 raise BaseError("There must be a valid value for selfjoin!")
-            tmp['selfjoin'] = self._selfjoin
+            tmp["selfjoin"] = self._selfjoin
             if self._status is None:
                 raise BaseError("There must be a valid value for status!")
-            tmp['status'] = self._status
+            tmp["status"] = self._status
         else:
-            if self._name is not None and 'name' in self._changed:
-                tmp['name'] = self._name
-            if not self._descriptions.isEmpty() and 'descriptions' in self._changed:
-                tmp['descriptions'] = self._descriptions.toJsonObj()
-            if self._selfjoin is not None and 'selfjoin' in self._changed:
-                tmp['selfjoin'] = self._selfjoin
+            if self._name is not None and "name" in self._changed:
+                tmp["name"] = self._name
+            if not self._descriptions.isEmpty() and "descriptions" in self._changed:
+                tmp["descriptions"] = self._descriptions.toJsonObj()
+            if self._selfjoin is not None and "selfjoin" in self._changed:
+                tmp["selfjoin"] = self._selfjoin
         return tmp
 
     def create(self) -> Group:
         jsonobj = self.toJsonObj(Actions.Create)
         jsondata = json.dumps(jsonobj)
         result = self._con.post(Group.ROUTE, jsondata)
-        return Group.fromJsonObj(self._con, result['group'])
+        return Group.fromJsonObj(self._con, result["group"])
 
     def read(self) -> Group:
-        result = self._con.get(Group.ROUTE_SLASH + quote_plus(self._id))
-        return Group.fromJsonObj(self._con, result['group'])
+        result = self._con.get(Group.ROUTE_SLASH + quote_plus(self._iri))
+        return Group.fromJsonObj(self._con, result["group"])
 
     def update(self) -> Optional[Group]:
         updated_group = None
         jsonobj = self.toJsonObj(Actions.Update)
         if jsonobj:
             jsondata = json.dumps(jsonobj)
-            result = self._con.put(Group.ROUTE_SLASH + quote_plus(self._id), jsondata)
-            updated_group = Group.fromJsonObj(self._con, result['group'])
-        if self._status is not None and 'status' in self._changed:
-            jsondata = json.dumps({'status': self._status})
-            result = self._con.put(Group.ROUTE_SLASH + quote_plus(self._id) + '/status', jsondata)
-            updated_group = Group.fromJsonObj(self._con, result['group'])
+            result = self._con.put(Group.ROUTE_SLASH + quote_plus(self._iri), jsondata)
+            updated_group = Group.fromJsonObj(self._con, result["group"])
+        if self._status is not None and "status" in self._changed:
+            jsondata = json.dumps({"status": self._status})
+            result = self._con.put(Group.ROUTE_SLASH + quote_plus(self._iri) + "/status", jsondata)
+            updated_group = Group.fromJsonObj(self._con, result["group"])
         return updated_group
 
     def delete(self) -> Group:
-        result = self._con.delete(Group.ROUTE_SLASH + quote_plus(self._id))
-        return Group.fromJsonObj(self._con, result['group'])
+        result = self._con.delete(Group.ROUTE_SLASH + quote_plus(self._iri))
+        return Group.fromJsonObj(self._con, result["group"])
 
     @staticmethod
     def getAllGroups(con: Connection) -> list[Group]:
         result = con.get(Group.ROUTE)
         return [Group.fromJsonObj(con, group_item) for group_item in result["groups"]]
 
     @staticmethod
@@ -248,24 +252,24 @@
         return [g for g in Group.getAllGroups(con) if g.project == proj_iri]
 
     def createDefinitionFileObj(self) -> dict[str, Any]:
         group = {
             "name": self.name,
             "descriptions": self.descriptions.createDefinitionFileObj(),
             "selfjoin": self.selfjoin,
-            "status": self.status
+            "status": self.status,
         }
         return group
 
     def print(self) -> None:
-        print('Group Info:')
-        print('  Id:          {}'.format(self._id))
-        print('  Name:        {}'.format(self._name))
+        print("Group Info:")
+        print("  IRI:         {}".format(self._iri))
+        print("  Name:        {}".format(self._name))
         if self._descriptions is not None:
-            print('  Descriptions:')
+            print("  Descriptions:")
             for descr in self._descriptions.items():
-                print('    {}: {}'.format(descr[0], descr[1]))
+                print("    {}: {}".format(descr[0], descr[1]))
         else:
-            print('  Descriptions: None')
-        print('  Project:     {}'.format(self._project))
-        print('  Selfjoin:    {}'.format(self._selfjoin))
-        print('  Status:      {}'.format(self._status))
+            print("  Descriptions: None")
+        print("  Project:     {}".format(self._project))
+        print("  Selfjoin:    {}".format(self._selfjoin))
+        print("  Status:      {}".format(self._status))
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/helpers.py` & `dsp_tools-2.3.3/src/dsp_tools/models/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
-import sys
 from dataclasses import dataclass
 from enum import Enum, unique
-from typing import Any, NewType, Optional, Pattern, Union
+from typing import Any, Optional, Pattern, Union
 
 from dsp_tools.models.exceptions import BaseError
 
 #
 # here we do some data typing that should help
 #
 
@@ -16,23 +15,20 @@
     """
     Holds an ontology IRI
 
     Attributes:
         iri: the ontology IRI
         hashtag: True if "#" is used to separate elements, False if element name is appended after "/"
     """
+
     iri: str
     hashtag: bool
 
 
-ContextType = NewType("ContextType", dict[str, OntoIri])
-
-
-def LINE() -> int:
-    return sys._getframe(1).f_lineno
+ContextType = dict[str, OntoIri]
 
 
 class IriTest:
     __iri_regexp = re.compile("^(http)s?://([\\w\\.\\-~]+)?(:\\d{,6})?(/[\\w\\-~]+)*(#[\\w\\-~]*)?")
 
     @classmethod
     def test(cls, val: str) -> bool:
@@ -53,19 +49,19 @@
     C_1 = "1"
     C_0_1 = "0-1"
     C_1_n = "1-n"
     C_0_n = "0-n"
 
 
 class ContextIterator:
-    _context: 'Context'
+    _context: "Context"
     _prefixes: list[str]
     _index: int
 
-    def __init__(self, context: 'Context'):
+    def __init__(self, context: "Context"):
         self._context = context
         self._prefixes = [x for x in self._context.context]
         self._index = 0
 
     def __next__(self) -> tuple[Optional[str], Optional[OntoIri]]:
         if len(self._context.context) == 0 and self._index == 0:
             return None, None
@@ -77,54 +73,50 @@
             raise StopIteration
 
 
 class Context:
     """
     This class holds a JSON-LD context with the ontology IRI's and the associated prefixes
     """
+
     _context: ContextType
     _rcontext: dict[str, str]
     _exp: Pattern[str]
 
-    common_ontologies = ContextType({
-        "foaf": OntoIri("http://xmlns.com/foaf/0.1/", False),
-        "dc": OntoIri("http://purl.org/dc/elements/1.1/", False),
-        "dcterms": OntoIri("http://purl.org/dc/terms/", False),
-        "dcmi": OntoIri("http://purl.org/dc/dcmitype/", False),
-        "skos": OntoIri("http://www.w3.org/2004/02/skos/core", True),
-        "bibtex": OntoIri("http://purl.org/net/nknouf/ns/bibtex", True),
-        "bibo": OntoIri("http://purl.org/ontology/bibo/", False),
-        "cidoc": OntoIri("http://purl.org/NET/cidoc-crm/core", True),
-        "schema": OntoIri("https://schema.org/", False),
-        "edm": OntoIri("http://www.europeana.eu/schemas/edm/", False),
-        "ebucore": OntoIri("http://www.ebu.ch/metadata/ontologies/ebucore/ebucore", True)
-    })
-
-    knora_ontologies = ContextType({
-        "knora-api": OntoIri("http://api.knora.org/ontology/knora-api/v2", True),
-        "salsah-gui": OntoIri("http://api.knora.org/ontology/salsah-gui/v2", True)
-    })
-
-    base_ontologies = ContextType({
-        "rdf": OntoIri("http://www.w3.org/1999/02/22-rdf-syntax-ns", True),
-        "rdfs": OntoIri("http://www.w3.org/2000/01/rdf-schema", True),
-        "owl": OntoIri("http://www.w3.org/2002/07/owl", True),
-        "xsd": OntoIri("http://www.w3.org/2001/XMLSchema", True)
-    })
-
-    def __is_iri(self, val: str) -> bool:
-        """
-        Test if string has a valid IRI pattern
+    common_ontologies = ContextType(
+        {
+            "foaf": OntoIri("http://xmlns.com/foaf/0.1/", False),
+            "dc": OntoIri("http://purl.org/dc/elements/1.1/", False),
+            "dcterms": OntoIri("http://purl.org/dc/terms/", False),
+            "dcmi": OntoIri("http://purl.org/dc/dcmitype/", False),
+            "skos": OntoIri("http://www.w3.org/2004/02/skos/core", True),
+            "bibtex": OntoIri("http://purl.org/net/nknouf/ns/bibtex", True),
+            "bibo": OntoIri("http://purl.org/ontology/bibo/", False),
+            "cidoc": OntoIri("http://purl.org/NET/cidoc-crm/core", True),
+            "schema": OntoIri("https://schema.org/", False),
+            "edm": OntoIri("http://www.europeana.eu/schemas/edm/", False),
+            "ebucore": OntoIri("http://www.ebu.ch/metadata/ontologies/ebucore/ebucore", True),
+        }
+    )
 
-        :param val: Input string
-        :return: True, if val corresponds to IRI pattern
-        """
+    knora_ontologies = ContextType(
+        {
+            "knora-api": OntoIri("http://api.knora.org/ontology/knora-api/v2", True),
+            "salsah-gui": OntoIri("http://api.knora.org/ontology/salsah-gui/v2", True),
+        }
+    )
 
-        m = self._exp.match(val)
-        return m.span()[1] == len(val) if m else False
+    base_ontologies = ContextType(
+        {
+            "rdf": OntoIri("http://www.w3.org/1999/02/22-rdf-syntax-ns", True),
+            "rdfs": OntoIri("http://www.w3.org/2000/01/rdf-schema", True),
+            "owl": OntoIri("http://www.w3.org/2002/07/owl", True),
+            "xsd": OntoIri("http://www.w3.org/2001/XMLSchema", True),
+        }
+    )
 
     def __init__(self, context: Optional[dict[str, str]] = None):
         """
         THe Constructor of the Context. It takes one optional parameter which as a dict of
         prefix - ontology-iri pairs. If the hashtag "#" is used to append element name, the
         ontology-iri *must* end with "#"!
         :param context: A dict of prefix - ontology-iri pairs
@@ -132,15 +124,15 @@
         # regexp to test for a complete IRI (including fragment identifier)
         self._exp = re.compile("^(http)s?://([\\w\\.\\-~]+)?(:\\d{,6})?(/[\\w\\-~]+)*(#[\\w\\-~]*)?")
         self._context = ContextType({})
 
         # add ontologies from context, if any
         if context:
             for prefix, onto in context.items():
-                self._context[prefix] = OntoIri(onto.removesuffix('#'), onto.endswith('#') or onto.endswith('/v2'))
+                self._context[prefix] = OntoIri(onto.removesuffix("#"), onto.endswith("#") or onto.endswith("/v2"))
 
         # add standard ontologies (rdf, rdfs, owl, xsl)
         for k, v in self.base_ontologies.items():
             if not self._context.get(k):
                 self._context[k] = v
 
         # add DSP-API internal ontologies (knora-api, salsah-gui)
@@ -259,15 +251,15 @@
             entrylist = list(filter(lambda x: x[1].iri == iri, self.common_ontologies.items()))
             if len(entrylist) == 1:
                 entry = entrylist[0]
                 self._context[entry[0]] = entry[1]  # add to list of prefixes used
                 self._rcontext[entry[1].iri] = entry[0]
                 result = entry[0]
             else:
-                tmp = iri.split('/')
+                tmp = iri.split("/")
                 if tmp[-1] == "v2":
                     #
                     # we have a knora ontology name "http://server/ontology/shortcode/shortname/v2"
                     self._context[tmp[-2]] = OntoIri(iri, True)  # add to list of prefixes used
                     self._rcontext[iri] = tmp[-2]
                 else:
                     raise BaseError("Iri cannot be resolved to a well-known prefix!")
@@ -283,29 +275,29 @@
         Returns:
             the fully qualified IRI
         """
         if not val:
             return None
         if IriTest.test(val):
             return val
-        tmp = val.split(':')
+        tmp = val.split(":")
         if len(tmp) < 2:
             raise BaseError("There is no separator to identify the prefix: " + val)
         iri_info = self._context.get(tmp[0])
         if iri_info is None:
             entrylist = list(filter(lambda x: x[1].iri == tmp[0], self.common_ontologies.items()))
             if len(entrylist) == 1:
                 entry = entrylist[0]
                 self._context[entry[0]] = entry[1]  # add to list of prefixes used
                 self._rcontext[entry[1].iri] = entry[0]
                 iri_info = entry[1]
             else:
                 raise BaseError("Ontology not known! Cannot generate fully qualified IRI")
         if iri_info.hashtag:
-            return iri_info.iri + '#' + tmp[1]
+            return iri_info.iri + "#" + tmp[1]
         else:
             return iri_info.iri + tmp[1]
 
     def get_prefixed_iri(self, iri: Optional[str]) -> Optional[str]:
         """
         We reduce a fully qualified IRI to a short one in the form "prefix:name"
 
@@ -319,34 +311,34 @@
         m = re.match("([\\w-]+):([\\w-]+)", iri)
         if m and m.span()[1] == len(iri):
             return iri
 
         if not IriTest.test(iri):
             raise BaseError(f"The IRI '{iri}' does not conform to the IRI pattern.")
 
-        split_point = iri.find('#')
+        split_point = iri.find("#")
         if split_point == -1:
-            split_point = iri.rfind('/')
-            onto_part = iri[:split_point + 1]
-            element = iri[split_point + 1:]
+            split_point = iri.rfind("/")
+            onto_part = iri[: split_point + 1]
+            element = iri[split_point + 1 :]
         else:
             onto_part = iri[:split_point]
-            element = iri[split_point + 1:]
+            element = iri[split_point + 1 :]
 
         prefix = self._rcontext.get(onto_part)
         if prefix is None:
             entry_list = list(filter(lambda x: x[1].iri == onto_part, self.common_ontologies.items()))
             if len(entry_list) == 1:
                 entry = entry_list[0]
                 self._context[entry[0]] = entry[1]  # add to list of prefixes used
                 self._rcontext[entry[1].iri] = entry[0]
                 prefix = entry[0]
             else:
                 return None
-        return prefix + ':' + element
+        return prefix + ":" + element
 
     def reduce_iri(self, iri_str: str, onto_name: Optional[str] = None) -> str:
         """
         Reduces an IRI to the form that is used within the definition JSON file. It expects the context object to have
         entries (prefixes) for all IRIs:
         - if it's an external IRI and the ontology can be extracted as prefix it returns: "prefix:name"
         - if it's in the same ontology, it returns: ":name"
@@ -362,49 +354,51 @@
         """
         knora_api = self.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
         salsah_gui = self.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
 
         if IriTest.test(iri_str):
             if self.get_prefixed_iri(iri_str):
                 iri_str = self.get_prefixed_iri(iri_str)
-        tmp = iri_str.split(':')
+        tmp = iri_str.split(":")
         if tmp[0] == knora_api or tmp[0] == salsah_gui:
             return tmp[1]
         elif tmp[0] == onto_name:
-            return ':' + tmp[1]
+            return ":" + tmp[1]
         else:
             return iri_str
 
     def toJsonObj(self) -> dict[str, str]:
         """
         Return a python object that can be jsonfied...
         :return: Object to be jsonfied
         """
-        return {prefix: oinfo.iri + '#' if oinfo.hashtag else oinfo.iri
-                for prefix, oinfo in self._context.items()}
+        return {prefix: oinfo.iri + "#" if oinfo.hashtag else oinfo.iri for prefix, oinfo in self._context.items()}
 
     def get_externals_used(self) -> dict[str, str]:
         exclude = ["rdf", "rdfs", "owl", "xsd", "knora-api", "salsah-gui"]
         return {prefix: onto.iri for prefix, onto in self._context.items() if prefix not in exclude}
 
     def print(self) -> None:
         for a in self._context.items():
             print(a[0] + ': "' + a[1].iri + '"')
 
 
 class DateTimeStamp:
     """
     Class to hold and process an xsd:dateTimeStamp
     """
+
     _dateTimeStamp: str
-    _validation_regex = r"^-?([1-9][0-9]{3,}|0[0-9]{3})" \
-                        r"-(0[1-9]|1[0-2])" \
-                        r"-(0[1-9]|[12][0-9]|3[01])" \
-                        r"T(([01][0-9]|2[0-3]):[0-5][0-9]:[0-5][0-9](\.[0-9]+)?|(24:00:00(\.0+)?))" \
-                        r"(Z|(\+|-)((0[0-9]|1[0-3]):[0-5][0-9]|14:00))$"
+    _validation_regex = (
+        r"^-?([1-9][0-9]{3,}|0[0-9]{3})"
+        r"-(0[1-9]|1[0-2])"
+        r"-(0[1-9]|[12][0-9]|3[01])"
+        r"T(([01][0-9]|2[0-3]):[0-5][0-9]:[0-5][0-9](\.[0-9]+)?|(24:00:00(\.0+)?))"
+        r"(Z|(\+|-)((0[0-9]|1[0-3]):[0-5][0-9]|14:00))$"
+    )
 
     def __init__(self, val: Any):
         """
         The constructor works for different inputs:
         - a string
         - an instance of "DateTimeStamp"
         - json-ld construct of the form { "@type": "xsd:dateTimeStamp", "@value": "date-str" }
@@ -418,60 +412,58 @@
             self._dateTimeStamp = str(val)
         else:
             if val.get("@type") == "xsd:dateTimeStamp" and re.search(self._validation_regex, str(val.get("@value"))):
                 self._dateTimeStamp = val["@value"]
             else:
                 raise BaseError(f"Invalid xsd:dateTimeStamp: '{val}'")
 
-    def __eq__(self, other: Union[str, 'DateTimeStamp']) -> bool:
+    def __eq__(self, other: Union[str, "DateTimeStamp"]) -> bool:
         if isinstance(other, str):
             other = DateTimeStamp(other)
         return self._dateTimeStamp == other._dateTimeStamp
 
-    def __lt__(self, other: 'DateTimeStamp') -> bool:
+    def __lt__(self, other: "DateTimeStamp") -> bool:
         if isinstance(other, str):
             other = DateTimeStamp(other)
         return self._dateTimeStamp < other._dateTimeStamp
 
-    def __le__(self, other: 'DateTimeStamp') -> bool:
+    def __le__(self, other: "DateTimeStamp") -> bool:
         if isinstance(other, str):
             other = DateTimeStamp(other)
         return self._dateTimeStamp <= other._dateTimeStamp
 
-    def __gt__(self, other: 'DateTimeStamp') -> bool:
+    def __gt__(self, other: "DateTimeStamp") -> bool:
         if isinstance(other, str):
             other = DateTimeStamp(other)
         return self._dateTimeStamp > other._dateTimeStamp
 
-    def __ge__(self, other: 'DateTimeStamp') -> bool:
+    def __ge__(self, other: "DateTimeStamp") -> bool:
         if isinstance(other, str):
             other = DateTimeStamp(other)
         return self._dateTimeStamp >= other._dateTimeStamp
 
-    def __ne__(self, other: 'DateTimeStamp') -> bool:
+    def __ne__(self, other: "DateTimeStamp") -> bool:
         if isinstance(other, str):
             other = DateTimeStamp(other)
         return self._dateTimeStamp != other._dateTimeStamp
 
-    def __str__(self: 'DateTimeStamp') -> Union[None, str]:
+    def __str__(self: "DateTimeStamp") -> Union[None, str]:
         return self._dateTimeStamp
 
     def toJsonObj(self):
-        return {
-            "@type": "xsd:dateTimeStamp",
-            "@value": self._dateTimeStamp
-        }
+        return {"@type": "xsd:dateTimeStamp", "@value": self._dateTimeStamp}
 
 
 class WithId:
     """
     Class helper to get json-ld "@id" thingies
     """
+
     _tmp: str = None
 
     def __init__(self, obj: Optional[dict[str, str]]):
         if obj is None:
             return
-        self._tmp = obj.get('@id')
+        self._tmp = obj.get("@id")
 
     def str(self) -> Optional[str]:
         return self._tmp
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/langstring.py` & `dsp_tools-2.3.3/src/dsp_tools/models/langstring.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 from typing import Any, Optional, Union
 
 from dsp_tools.models.exceptions import BaseError
 
 
 @unique
 class Languages(Enum):
-    EN = 'en'
-    DE = 'de'
-    FR = 'fr'
-    IT = 'it'
-    RM = 'rm'
+    EN = "en"
+    DE = "de"
+    FR = "fr"
+    IT = "it"
+    RM = "rm"
 
 
 LangStringParam = Optional[Union[dict[Union[Languages, str], str], str]]
 
 
 class LangStringIterator:
     """Iterator class for LangString class."""
 
-    _langstring: 'LangString'
+    _langstring: "LangString"
     _index: int
 
-    def __init__(self, langstring: 'LangString'):
+    def __init__(self, langstring: "LangString"):
         self._langstring = langstring
         self._langlist = list(map(lambda a: a[0], self._langstring.items()))
         self._index = 0
 
     def __next__(self):
         if len(self._langlist) == 0 and self._index == 0:
             return None, self._langstring[None]
@@ -50,19 +50,19 @@
     ```
 
     or a simple string without language:
     ```
     "some:thing": "a string without language specificer"
     ```
     """
+
     _langstrs: dict[Languages, str]
     _simplestring: str
 
     def __init__(self, initvalue: LangStringParam = None):
-
         def mymapper(p: tuple[Union[Languages, str], str]) -> tuple[Languages, str]:
             lmap = dict(map(lambda a: (a.value, a), Languages))
             if isinstance(p[0], str) and p[0] in lmap:
                 lang = lmap[p[0].lower()]
             elif isinstance(p[0], Languages):
                 lang = p[0]
             else:
@@ -80,27 +80,26 @@
             self._langstrs = dict(map(mymapper, initvalue.items()))
         elif isinstance(initvalue, LangString):
             self._simplestring = initvalue._simplestring
             self._langstrs = initvalue._langstrs
         else:
             raise BaseError("Not a valid language definition!")
 
-    def __getitem__(self, key: Optional[Union[Languages, str]] = None) -> str:
+    def __getitem__(self, key: Optional[Union[Languages, str]] = None) -> Optional[str]:
         #
         # First deal with simple strings (no language given). We return, if existing, the simple string
         # or just the first language dependent string
         #
         if key is None:
-            if self._simplestring is not None:
+            if self._simplestring:
                 return self._simplestring
+            elif len(self._langstrs) != 0:
+                return list(self._langstrs)[0]
             else:
-                try:
-                    return list(self._langstrs)[0]
-                except:
-                    return None
+                return None
         else:
             pass
             # self._simplestring = None  # Let's delete the string without language if there is one...
         if isinstance(key, Enum):
             if self._langstrs.get(key) is None:
                 for l in self._langstrs:
                     if self._langstrs.get(l) is not None:
@@ -143,24 +142,24 @@
         else:
             lmap = dict(map(lambda a: (a.value, a), Languages))
             if lmap.get(key.lower()) is None:
                 raise BaseError('Invalid language string "' + key + '"!')
             del self._langstrs[lmap[key.lower()]]
 
     def __str__(self):
-        tmpstr = '{'
+        tmpstr = "{"
         for p in self._langstrs:
-            tmpstr += '=' + p.value + ':' + self._langstrs[p]
-        tmpstr += '}'
+            tmpstr += "=" + p.value + ":" + self._langstrs[p]
+        tmpstr += "}"
         return tmpstr
 
     def __iter__(self):
         return LangStringIterator(self)
 
-    def __eq__(self, other: 'LangString'):
+    def __eq__(self, other: "LangString"):
         equal = self._simplestring == other._simplestring
         if equal:
             for lang in Languages:
                 equal = self._langstrs.get(lang) == other._langstrs.get(lang)
                 if not equal:
                     break
         return equal
@@ -189,89 +188,89 @@
 
     def toJsonObj(self) -> Optional[Union[str, list[dict[str, str]]]]:
         if self.isEmpty():
             return None
         if self._simplestring is not None:
             return self._simplestring
         else:
-            return list(map(lambda a: {'language': a[0].value, 'value': a[1] if a[1] else "-"}, self._langstrs.items()))
+            return list(map(lambda a: {"language": a[0].value, "value": a[1] if a[1] else "-"}, self._langstrs.items()))
 
     def toJsonLdObj(self) -> Optional[Union[str, list[dict[str, str]]]]:
         if self.isEmpty():
             return None
         if self._simplestring is not None:
             return self._simplestring
         else:
-            return [{'@language': a[0].value, '@value': a[1]} for a in self._langstrs.items()]
+            return [{"@language": a[0].value, "@value": a[1]} for a in self._langstrs.items()]
             # return list(map(lambda a: {'@language': a[0].value, '@value': a[1]}, self._langstrs.items()))
 
     @classmethod
-    def fromJsonLdObj(cls, obj: Optional[Union[list[dict[str, str]], str]]) -> 'LangString':
+    def fromJsonLdObj(cls, obj: Optional[Union[list[dict[str, str]], str]]) -> "LangString":
         if obj is None:
             return None
         if isinstance(obj, str):
             return cls(obj)
         if isinstance(obj, list):
             objs = obj
         else:
             objs = [obj]
         lstrs: dict[Languages, str] = {}
         for o in objs:
-            lang = o.get('@language')
-            if lang == 'en':
-                lstrs[Languages.EN] = o.get('@value')
-            elif lang == 'de':
-                lstrs[Languages.DE] = o.get('@value')
-            elif lang == 'fr':
-                lstrs[Languages.FR] = o.get('@value')
-            elif lang == 'it':
-                lstrs[Languages.IT] = o.get('@value')
-            elif lang == 'rm':
-                lstrs[Languages.RM] = o.get('@value')
+            lang = o.get("@language")
+            if lang == "en":
+                lstrs[Languages.EN] = o.get("@value")
+            elif lang == "de":
+                lstrs[Languages.DE] = o.get("@value")
+            elif lang == "fr":
+                lstrs[Languages.FR] = o.get("@value")
+            elif lang == "it":
+                lstrs[Languages.IT] = o.get("@value")
+            elif lang == "rm":
+                lstrs[Languages.RM] = o.get("@value")
             else:
-                if o.get('@value') is not None:
-                    return cls(o.get('@value'))
+                if o.get("@value") is not None:
+                    return cls(o.get("@value"))
         return cls(lstrs)
 
     @classmethod
-    def fromJsonObj(cls, obj: Optional[Any]) -> 'LangString':
+    def fromJsonObj(cls, obj: Optional[Any]) -> "LangString":
         if obj is None:
             return None
         if isinstance(obj, str):
             return cls(obj)
         if isinstance(obj, list):
             objs = obj
         else:
             objs = [obj]
         lstrs: dict[Languages, str] = {}
         for o in objs:
-            lang = o.get('language')
-            if lang == 'en':
-                lstrs[Languages.EN] = o.get('value')
-            elif lang == 'de':
-                lstrs[Languages.DE] = o.get('value')
-            elif lang == 'fr':
-                lstrs[Languages.FR] = o.get('value')
-            elif lang == 'it':
-                lstrs[Languages.IT] = o.get('value')
-            elif lang == 'rm':
-                lstrs[Languages.RM] = o.get('value')
+            lang = o.get("language")
+            if lang == "en":
+                lstrs[Languages.EN] = o.get("value")
+            elif lang == "de":
+                lstrs[Languages.DE] = o.get("value")
+            elif lang == "fr":
+                lstrs[Languages.FR] = o.get("value")
+            elif lang == "it":
+                lstrs[Languages.IT] = o.get("value")
+            elif lang == "rm":
+                lstrs[Languages.RM] = o.get("value")
             else:
-                if o.get('value') is not None:
-                    return cls(o.get('value'))
+                if o.get("value") is not None:
+                    return cls(o.get("value"))
         return cls(lstrs)
 
     def print(self, offset: Optional[int] = None):
-        blank = ' '
+        blank = " "
         # print(f'{blank:>{offset}}LangString:')
         if self._simplestring is not None:
-            print(f'{blank:>{offset + 2}}{self._simplestring}')
+            print(f"{blank:>{offset + 2}}{self._simplestring}")
         else:
             for p in self._langstrs.items():
-                print(f'{blank:>{offset + 2}}{p[0]} : {p[1]}')
+                print(f"{blank:>{offset + 2}}{p[0]} : {p[1]}")
 
     @property
     def langstrs(self):
         return self._langstrs
 
     def createDefinitionFileObj(self) -> Union[str, dict[str, str]]:
         if self._simplestring:
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/listnode.py` & `dsp_tools-2.3.3/src/dsp_tools/models/listnode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,58 @@
-import json
-from pprint import pprint
-from typing import Any, Optional, Union
-from urllib.parse import quote_plus
-
-from dsp_tools.models.connection import Connection
-from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.helpers import Actions
-from dsp_tools.models.langstring import LangString, Languages
-from dsp_tools.models.model import Model
-from dsp_tools.models.project import Project
-from dsp_tools.models.set_encoder import SetEncoder
-
 """
 This module implements the handling (CRUD) of list nodes and adds some function to read whole lists.
 
 CREATE:
     * Instantiate a new object of the class ListNode
     * Call the ``create`` method on the instance
 
 READ:
-    * Instantiate a new object with ``id`` (IRI of listnode)
+    * Instantiate a new object with ``iri`` (IRI of listnode)
     * Call the ``read`` method on the instance
     * Access information about the instance
 
 UPDATE:
     * Only partially implemented. Only "label" and "comment" attributes may be changed.
     * You need an instance of an existing ListNode by reading an instance
     * Change the attributes by assigning the new values
     * Call the ``update`` method on the instance
 
 DELETE
     * NOT YET IMPLEMENTED!
 """
 
+import json
+from pprint import pprint
+from typing import Any, Optional, Union
+from urllib.parse import quote_plus
 
-def list_creator(con: Connection,
-                 project: Project,
-                 parent_node: 'ListNode',
-                 nodes: list[dict]) -> list['ListNode']:
+from dsp_tools.models.connection import Connection
+from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import Actions
+from dsp_tools.models.langstring import LangString, Languages
+from dsp_tools.models.model import Model
+from dsp_tools.models.project import Project
+from dsp_tools.models.set_encoder import SetEncoder
+
+
+def list_creator(con: Connection, project: Project, parent_node: "ListNode", nodes: list[dict]) -> list["ListNode"]:
     nodelist: list[ListNode] = []
 
     for node in nodes:
         new_node = ListNode(
             con=con,
             project=project,
             label=node["labels"],
             comments=node.get("comments"),
             name=node["name"],
-            parent=parent_node
+            parent=parent_node,
         )
 
-        if node.get('nodes'):
-            new_node.children = list_creator(con, project, new_node, node['nodes'])
+        if node.get("nodes"):
+            new_node.children = list_creator(con, project, new_node, node["nodes"])
 
         nodelist.append(new_node)
 
     return nodelist
 
 
 class ListNode(Model):
@@ -64,15 +61,15 @@
 
     Attributes
     ----------
 
     con : Connection
         A Connection instance to a DSP server (for some operation a login has to be performed with valid credentials)
 
-    id : str
+    iri : str
         IRI of the list node [readonly, cannot be modified after creation of instance]
 
     project : str
         IRI of project. Only used for the creation of a new list (root node) [write].
 
     label : LangString
         A LangString instance with language dependent labels. Setting this attribute overwrites all entries
@@ -134,227 +131,234 @@
     _id: Optional[str]
     _project: Optional[str]
     _label: Optional[LangString]
     _comments: Optional[LangString]
     _name: Optional[str]
     _parent: Optional[str]
     _isRootNode: bool
-    _children: Optional[list['ListNode']]
+    _children: Optional[list["ListNode"]]
     _rootNodeIri: Optional[str]
 
-    def __init__(self,
-                 con: Connection,
-                 id: Optional[str] = None,
-                 project: Optional[Union[Project, str]] = None,
-                 label: Optional[LangString] = None,
-                 comments: Optional[LangString] = None,
-                 name: Optional[str] = None,
-                 parent: Optional[Union['ListNode', str]] = None,
-                 isRootNode: bool = False,
-                 children: Optional[list['ListNode']] = None,
-                 rootNodeIri: Optional[str] = None):
+    def __init__(
+        self,
+        con: Connection,
+        iri: Optional[str] = None,
+        project: Optional[Union[Project, str]] = None,
+        label: Optional[LangString] = None,
+        comments: Optional[LangString] = None,
+        name: Optional[str] = None,
+        parent: Optional[Union["ListNode", str]] = None,
+        isRootNode: bool = False,
+        children: Optional[list["ListNode"]] = None,
+        rootNodeIri: Optional[str] = None,
+    ) -> None:
         """
         This is the constructor for the ListNode object. For
 
         CREATE:
             * The "con" and at least one "label" are required
         READ:
-            * The "con" and "id" attributes are required
+            * The "con" and "iri" attributes are required
         UPDATE:
             * Only "label", "comments" and "name" may be changed
         DELETE:
             * Not yet implemented
 
-        :param con: A valid Connection instance with a user logged in that has the appropriate permissions
-        :param id: IRI of the project [readonly, cannot be modified after creation of instance]
-        :param project: IRI of project. Only used for the creation of a new list (root node) [write].
-        :param label: A LangString instance with language dependent labels. Setting this attributes overwites all entries with the new ones. In order to add/remove a specific entry, use "addLabel" or "rmLabel". At least one label is required [read/write].
-        :param comments: A LangString instance with language dependent comments. Setting this attributes overwites all entries with the new ones.In order to add/remove a specific entry, use "addComment" or "rmComment".
-        :param name: A unique name for the ListNode (unique regarding the whole list) [read/write].
-        :param parent: Is required and allowed only for the CREATE operation. Otherwise use the "children" attribute [write].
-        :param isRootNode: Is True if the ListNode is a root node of a list Cannot be set [read].
-        :param children: Contains a list of children nodes. This attribute is only available for nodes that have been read by the method "getAllNodes()"! [read]
-        :param rootNodeIri: IRI of the root node. This attribute is only available for nodes that have been read by the method "getAllNodes()"! [read]
+        Setting a label overwites all entries. To add/remove a specific entry, use "addLabel" or "rmLabel".
+        Setting a comment overwites all entries. To add/remove a specific entry, use "addComment" or "rmComment".
+
+        Args:
+            con: A valid Connection instance with a user logged in that has the appropriate permissions
+            iri: IRI of the project [readonly, cannot be modified after creation of instance]
+            project: IRI of project. Only used for the creation of a new list (root node) [write].
+            label: LangString with lang dependent labels. At least one label is required [read/write].
+            comments:  A LangString instance with language dependent comments.
+            name: A unique name for the ListNode (unique regarding the whole list) [read/write].
+            parent: Required and allowed only for the CREATE operation. Otherwise use the "children" attribute [write].
+            isRootNode: Is True if the ListNode is a root node of a list Cannot be set [read].
+            children: list of children nodes. Only available for nodes that have been read by getAllNodes()
+            rootNodeIri: IRI of the root node. Only available for nodes that have been read by the method getAllNodes()
         """
 
         super().__init__(con)
 
         self._project = project.id if isinstance(project, Project) else str(project) if project else None
-        self._id = str(id) if id else None
+        self._id = iri
         self._label = LangString(label)
         self._comments = LangString(comments) if comments else None
-        self._name = str(name) if name else None
+        self._name = name
         if parent and isinstance(parent, ListNode):
-            self._parent = parent.id
+            self._parent = parent.iri
         else:
             self._parent = str(parent) if parent else None
         self._isRootNode = isRootNode
         if children:
             if isinstance(children, list) and len(children) > 0 and isinstance(children[0], ListNode):
                 self._children = children
             else:
-                raise BaseError('ERROR Children must be list of ListNodes!')
+                raise BaseError("ERROR Children must be list of ListNodes!")
         else:
             self._children = None
         if not isinstance(rootNodeIri, str) and rootNodeIri:
-            raise BaseError('ERROR rootNodeIri must be of type string')
+            raise BaseError("ERROR rootNodeIri must be of type string")
         self._rootNodeIri = rootNodeIri
 
     @property
-    def id(self) -> Optional[str]:
+    def iri(self) -> Optional[str]:
         return self._id
 
-    @id.setter
-    def id(self, value: str) -> None:
-        raise BaseError('ListNode id cannot be modified!')
+    @iri.setter
+    def iri(self, value: str) -> None:
+        raise BaseError("ListNode iri cannot be modified!")
 
     @property
     def project(self) -> Optional[str]:
         return self._project
 
     @project.setter
     def project(self, value: str) -> None:
         if self._project:
-            raise BaseError('Project id cannot be modified!')
+            raise BaseError("Project id cannot be modified!")
         else:
             self._project = value
 
     @property
     def label(self) -> LangString:
         return self._label or LangString({})
 
     @label.setter
     def label(self, value: Optional[Union[LangString, str]]) -> None:
         self._label = LangString(value)
-        self._changed.add('label')
+        self._changed.add("label")
 
     def addLabel(self, lang: Union[Languages, str], value: str) -> None:
         """
         Add/replace a node label with the given language (executed at next update)
 
         :param lang: The language the label, either a string "EN", "DE", "FR", "IT" or a Language instance
         :param value: The text of the label
         :return: None
         """
 
         self._label[lang] = value
-        self._changed.add('label')
+        self._changed.add("label")
 
     def rmLabel(self, lang: Union[Languages, str]) -> None:
         """
         Remove a label from a list node (executed at next update)
 
-        :param lang: The language the label to be removed is in, either a string "EN", "DE", "FR", "IT" or a Language instance
-        :return: None
+        Args:
+            lang: language of the label (string "EN", "DE", "FR", "IT", "RM", or a Language instance)
         """
         del self._label[lang]
-        self._changed.add('label')
+        self._changed.add("label")
 
     @property
     def comments(self) -> LangString:
         return self._comments or LangString({})
 
     @comments.setter
     def comments(self, value: Optional[Union[LangString, str]]) -> None:
         self._comments = LangString(value)
-        self._changed.add('comments')
+        self._changed.add("comments")
 
     def addComment(self, lang: Union[Languages, str], value: str) -> None:
         """
         Add/replace a node comments with the given language (executed at next update)
 
         :param lang: The language the comments, either a string "EN", "DE", "FR", "IT" or a Language instance
         :param value: The text of the comments
         :return: None
         """
 
         self._comments[lang] = value
-        self._changed.add('comments')
+        self._changed.add("comments")
 
     def rmComment(self, lang: Union[Languages, str]) -> None:
         """
         Remove a comments from a list node (executed at next update)
 
-        :param lang: The language the comment to be removed is in, either a string "EN", "DE", "FR", "IT" or a Language instance
+        :param lang: language of the comment (string "EN", "DE", "FR", "IT", "RM", or a Language instance)
         :return: None
         """
         del self._comments[lang]
-        self._changed.add('comments')
+        self._changed.add("comments")
 
     @property
     def name(self) -> Optional[str]:
         return self._name
 
     @name.setter
     def name(self, value: str) -> None:
-        self._name = str(value)
-        self._changed.add('name')
+        self._name = value
+        self._changed.add("name")
 
     @property
     def parent(self) -> Optional[str]:
         return self._parent if self._parent else None
 
     @parent.setter
-    def parent(self, value: Union[str, 'ListNode']):
+    def parent(self, value: Union[str, "ListNode"]):
         if isinstance(value, ListNode):
-            self._parent = value.id
+            self._parent = value.iri
         else:
             self._parent = value
 
     @property
     def isRootNode(self) -> Optional[bool]:
         return self._isRootNode
 
     @isRootNode.setter
     def isRootNode(self, value: bool) -> None:
-        raise BaseError('Property isRootNode cannot be set!')
+        raise BaseError("Property isRootNode cannot be set!")
 
     @property
-    def children(self) -> list['ListNode']:
+    def children(self) -> list["ListNode"]:
         return self._children or []
 
     @children.setter
-    def children(self, value: list['ListNode']) -> None:
+    def children(self, value: list["ListNode"]) -> None:
         self._children = value
 
     @staticmethod
-    def __getChildren(con: Connection,
-                      parent_iri: str,
-                      project_iri: str,
-                      children: list[Any]) -> Optional[list['ListNode']]:
+    def __getChildren(
+        con: Connection,
+        parent_iri: str,
+        project_iri: str,
+        children: list[Any],
+    ) -> Optional[list["ListNode"]]:
         """
         Internal method! Should not be used directly!
 
         Static method gets a recursive List of children nodes
 
         :param con: Valid Connection instance
         :param children: json object of children
         :return: List of ListNode instances
         """
         if children:
             child_nodes: list[Any] = []
             for child in children:
-
-                if 'parentNodeIri' not in child:
-                    child['parentNodeIri'] = parent_iri
-                if 'projectIri' not in child:
-                    child['projectIri'] = project_iri
+                if "parentNodeIri" not in child:
+                    child["parentNodeIri"] = parent_iri
+                if "projectIri" not in child:
+                    child["projectIri"] = project_iri
                 child_node = ListNode.fromJsonObj(con, child)
                 child_nodes.append(child_node)
             return child_nodes
         else:
             return None
 
     @property
     def rootNodeIri(self) -> Optional[str]:
         return self._rootNodeIri
 
     @rootNodeIri.setter
     def rootNodeIri(self, value: str):
-        raise BaseError('rootNodeIri cannot be set!')
+        raise BaseError("rootNodeIri cannot be set!")
 
     def has_changed(self) -> bool:
         if self._changed:
             return True
         else:
             return False
 
@@ -366,46 +370,45 @@
         This method is used to create a ListNode instance from the JSON data returned by DSP
 
         :param con: Connection instance
         :param json_obj: JSON data returned by DSP as python3 object
         :return: ListNode instance
         """
 
-        id = json_obj.get('id')
-        if id is None:
-            raise BaseError('ListNode id is missing')
-        project = json_obj.get('projectIri')
-        label = LangString.fromJsonObj(json_obj.get('labels'))
-        comments = LangString.fromJsonObj(json_obj.get('comments'))
-        if json_obj.get('name'):
-            name = json_obj['name']
-        else:
-            name = id.rsplit('/', 1)[-1]
-        parent = json_obj.get('parentNodeIri')
-        isRootNode = json_obj.get('isRootNode')
+        iri = json_obj.get("id")
+        if iri is None:
+            raise BaseError("ListNode id is missing")
+        project = json_obj.get("projectIri")
+        label = LangString.fromJsonObj(json_obj.get("labels"))
+        comments = LangString.fromJsonObj(json_obj.get("comments"))
+        if json_obj.get("name"):
+            name = json_obj["name"]
+        else:
+            name = iri.rsplit("/", 1)[-1]
+        parent = json_obj.get("parentNodeIri")
+        isRootNode = json_obj.get("isRootNode")
 
-        child_info = json_obj.get('children')
+        child_info = json_obj.get("children")
         children = None
         if child_info:
-            children = ListNode.__getChildren(con=con,
-                                              parent_iri=id,
-                                              project_iri=project,
-                                              children=child_info)
-        rootNodeIri = json_obj.get('hasRootNode')
-
-        return cls(con=con,
-                   id=id,
-                   project=project,
-                   label=label,
-                   comments=comments,
-                   name=name,
-                   parent=parent,
-                   isRootNode=isRootNode,
-                   children=children,
-                   rootNodeIri=rootNodeIri)
+            children = ListNode.__getChildren(con=con, parent_iri=iri, project_iri=project, children=child_info)
+        rootNodeIri = json_obj.get("hasRootNode")
+
+        return cls(
+            con=con,
+            iri=iri,
+            project=project,
+            label=label,
+            comments=comments,
+            name=name,
+            parent=parent,
+            isRootNode=isRootNode,
+            children=children,
+            rootNodeIri=rootNodeIri,
+        )
 
     def toJsonObj(self, action: Actions, listIri: str = None) -> Any:
         """
         Internal method! Should not be used directly!
 
         Creates a JSON-object from the ListNode instance that can be used to call DSP-API
 
@@ -416,136 +419,132 @@
         """
 
         tmp = {}
 
         if action == Actions.Create:
             if self._project is None:
                 raise BaseError("There must be a project id given!")
-            tmp['projectIri'] = self._project
+            tmp["projectIri"] = self._project
             if self._label.isEmpty():
                 raise BaseError("There must be a valid ListNode label!")
-            tmp['labels'] = self._label.toJsonObj()
+            tmp["labels"] = self._label.toJsonObj()
             if self._comments:
-                tmp['comments'] = self._comments.toJsonObj()
+                tmp["comments"] = self._comments.toJsonObj()
             if self._name:
-                tmp['name'] = self._name
+                tmp["name"] = self._name
             if self._parent:
-                tmp['parentNodeIri'] = self._parent
+                tmp["parentNodeIri"] = self._parent
 
         elif action == Actions.Update:
-            if self.id is None:
-                raise BaseError("There must be a node id given!")
-            tmp['listIri'] = listIri
+            if self.iri is None:
+                raise BaseError("There must be a node iri given!")
+            tmp["listIri"] = listIri
             if self._project is None:
                 raise BaseError("There must be a project id given!")
-            tmp['projectIri'] = self._project
-            if not self._label.isEmpty() and 'label' in self._changed:
-                tmp['labels'] = self._label.toJsonObj()
-            if not self._comments.isEmpty() and 'comments' in self._changed:
-                tmp['comments'] = self._comments.toJsonObj()
-            if self._name and 'name' in self._changed:
-                tmp['name'] = self._name
+            tmp["projectIri"] = self._project
+            if not self._label.isEmpty() and "label" in self._changed:
+                tmp["labels"] = self._label.toJsonObj()
+            if not self._comments.isEmpty() and "comments" in self._changed:
+                tmp["comments"] = self._comments.toJsonObj()
+            if self._name and "name" in self._changed:
+                tmp["name"] = self._name
 
         return tmp
 
-    def create(self) -> 'ListNode':
+    def create(self) -> "ListNode":
         """
         Create a new List
 
         :return: JSON-object from DSP-API
         """
 
         jsonobj = self.toJsonObj(Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder)
         if self._parent:
             result = self._con.post(ListNode.ROUTE_SLASH + quote_plus(self._parent), jsondata)
-            return ListNode.fromJsonObj(self._con, result['nodeinfo'])
+            return ListNode.fromJsonObj(self._con, result["nodeinfo"])
         else:
             result = self._con.post(ListNode.ROUTE, jsondata)
-            return ListNode.fromJsonObj(self._con, result['list']['listinfo'])
+            return ListNode.fromJsonObj(self._con, result["list"]["listinfo"])
 
     def read(self) -> Any:
         """
         Read a project from DSP-API
 
         :return: JSON-object from DSP-API
         """
 
-        result = self._con.get(ListNode.ROUTE_SLASH + 'nodes/' + quote_plus(self._id))
-        if result.get('nodeinfo'):
-            return self.fromJsonObj(self._con, result['nodeinfo'])
-        elif result.get('listinfo'):
-            return self.fromJsonObj(self._con, result['listinfo'])
+        result = self._con.get(ListNode.ROUTE_SLASH + "nodes/" + quote_plus(self._id))
+        if result.get("nodeinfo"):
+            return self.fromJsonObj(self._con, result["nodeinfo"])
+        elif result.get("listinfo"):
+            return self.fromJsonObj(self._con, result["listinfo"])
         else:
             return None
 
     def update(self) -> Union[Any, None]:
         """
         Update the ListNode info in DSP with the modified data in this ListNode instance
 
         :return: JSON-object from DSP-API reflecting the update
         """
 
-        jsonobj = self.toJsonObj(Actions.Update, self.id)
+        jsonobj = self.toJsonObj(Actions.Update, self.iri)
         if jsonobj:
             jsondata = json.dumps(jsonobj, cls=SetEncoder)
-            result = self._con.put(ListNode.ROUTE_SLASH + quote_plus(self.id), jsondata)
+            result = self._con.put(ListNode.ROUTE_SLASH + quote_plus(self.iri), jsondata)
             pprint(result)
-            return ListNode.fromJsonObj(self._con, result['listinfo'])
+            return ListNode.fromJsonObj(self._con, result["listinfo"])
         else:
             return None
 
     def delete(self) -> None:
         """
         Delete the given ListNode
 
         :return: DSP-API response
         """
         raise BaseError("NOT YET IMPLEMENTED")
-        result = self._con.delete(ListNode.ROUTE_SLASH + quote_plus(self._id))
-        return result
-        # return Project.fromJsonObj(self.con, result['project'])
 
-    def getAllNodes(self) -> 'ListNode':
+    def getAllNodes(self) -> "ListNode":
         """
         Get all nodes of the list. Must be called from a ListNode instance that has at least set the
         list iri!
 
         :return: Root node of list with recursive ListNodes ("children"-attributes)
         """
 
         result = self._con.get(ListNode.ROUTE_SLASH + quote_plus(self._id))
-        if 'list' not in result:
+        if "list" not in result:
             raise BaseError("Request got no list!")
-        if 'listinfo' not in result['list']:
+        if "listinfo" not in result["list"]:
             raise BaseError("Request got no proper list information!")
-        root = ListNode.fromJsonObj(self._con, result['list']['listinfo'])
-        if 'children' in result['list']:
-            root._children = ListNode.__getChildren(con=self._con,
-                                                    parent_iri=root.id,
-                                                    project_iri=root.project,
-                                                    children=result['list']['children'])
+        root = ListNode.fromJsonObj(self._con, result["list"]["listinfo"])
+        if "children" in result["list"]:
+            root.children = ListNode.__getChildren(
+                con=self._con, parent_iri=root.iri, project_iri=root.project, children=result["list"]["children"]
+            )
         return root
 
     @staticmethod
-    def getAllLists(con: Connection, project_iri: Optional[str] = None) -> list['ListNode']:
+    def getAllLists(con: Connection, project_iri: Optional[str] = None) -> list["ListNode"]:
         """
         Get all lists. If a project IRI is given, it returns the lists of the specified project
 
         :param con: Connection instance
         :param project_iri: Iri/id of project
         :return: list of ListNodes
         """
         if project_iri is None:
             result = con.get(ListNode.ROUTE)
         else:
-            result = con.get(ListNode.ROUTE + '?projectIri=' + quote_plus(project_iri))
-        if 'lists' not in result:
+            result = con.get(ListNode.ROUTE + "?projectIri=" + quote_plus(project_iri))
+        if "lists" not in result:
             raise BaseError("Request got no lists!")
-        return list(map(lambda a: ListNode.fromJsonObj(con, a), result['lists']))
+        return list(map(lambda a: ListNode.fromJsonObj(con, a), result["lists"]))
 
     def _createDefinitionFileObj(self, children: list["ListNode"]):
         """
         Create an object that corresponds to the syntax of the input to "create_onto".
         Node: This method must be used only internally (for recursion)!!
 
         :param children: List of children nodes
@@ -561,32 +560,28 @@
                 listnodeobj["comments"] = listnode.comments.createDefinitionFileObj()
             if listnode.children:
                 listnodeobj["nodes"] = self._createDefinitionFileObj(listnode.children)
             listnodeobjs.append(listnodeobj)
         return listnodeobjs
 
     @staticmethod
-    def readDefinitionFileObj(con: Connection, project: Project, rootnode: Any) -> 'ListNode':
+    def readDefinitionFileObj(con: Connection, project: Project, rootnode: Any) -> "ListNode":
         """
         Reads a JSON obj that corresponds to the syntax of the input to "create_onto".
 
         :param self:
         :param con: Connection object
         :param project: Project instance
         :param rootnode: root node of the list
         :return: an instance of ListNode corresponding to the root node
         """
         root_list_node = ListNode(
-            con=con,
-            project=project,
-            label=rootnode['labels'],
-            comments=rootnode.get('comments'),
-            name=rootnode['name']
+            con=con, project=project, label=rootnode["labels"], comments=rootnode.get("comments"), name=rootnode["name"]
         )
-        listnodes = list_creator(con, project, root_list_node, rootnode.get('nodes'))
+        listnodes = list_creator(con, project, root_list_node, rootnode.get("nodes"))
         root_list_node.children = listnodes
         return root_list_node
 
     def createDefinitionFileObj(self) -> dict[str, Any]:
         """
         Create an object that corresponds to the syntax of the input to "create_onto".
         :return: A python object that can be jsonfied to correspond to the syntax of the input to "create_onto".
@@ -604,25 +599,25 @@
     def print(self):
         """
         print info to stdout
 
         :return: None
         """
 
-        print('Node Info:')
-        print('  Id:        {}'.format(self._id))
-        print('  Project:   {}'.format(self._project))
-        print('  Name:      {}'.format(self._name))
-        print('  Label:     ')
+        print("Node Info:")
+        print("  IRI:       {}".format(self._id))
+        print("  Project:   {}".format(self._project))
+        print("  Name:      {}".format(self._name))
+        print("  Label:     ")
         if self._label:
             for lbl in self._label.items():
-                print('             {}: {}'.format(lbl[0], lbl[1]))
+                print("             {}: {}".format(lbl[0], lbl[1]))
         else:
-            print('             None')
-        print('  Comments:   ')
+            print("             None")
+        print("  Comments:   ")
         if self._comments.isEmpty():
             for lbl in self._comments.items():
-                print('             {}: {}'.format(lbl[0], lbl[1]))
+                print("             {}: {}".format(lbl[0], lbl[1]))
         else:
-            print('             None')
-        print('  Parent', self._parent)
-        print('  IsRootNode: {}'.format(self._isRootNode))
+            print("             None")
+        print("  Parent", self._parent)
+        print("  IsRootNode: {}".format(self._isRootNode))
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/ontology.py` & `dsp_tools-2.3.3/src/dsp_tools/models/ontology.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,104 +1,106 @@
-import copy
-import json
-import re
-from typing import Any, Optional, Union
-from urllib.parse import quote_plus
-
-from dsp_tools.models.connection import Connection
-from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
-from dsp_tools.models.model import Model
-from dsp_tools.models.project import Project
-from dsp_tools.models.propertyclass import PropertyClass
-from dsp_tools.models.resourceclass import ResourceClass
-from dsp_tools.models.set_encoder import SetEncoder
-
 """
 This model implements the handling of ontologies. It is to note that ResourceClasses, PropertyClasses
 as well as the assignment of PropertyCLasses to the ResourceClasses (with a given cardinality)
 is handled in "cooperation" with the propertyclass.py (PropertyClass) and resourceclass.py (ResourceClass
 and HasProperty) modules.
 
 CREATE:
     * Instantiate a new object of the Ontology class with all required parameters
     * Call the ``create``-method on the instance to create the ontology withing the backend
 
 READ:
-    * Instantiate a new object with ``id``(IRI of ontology) given
+    * Instantiate a new object with ``iri``(IRI of ontology) given
     * Call the ``read``-method on the instance. Reading the ontology also reads all
       associated PropertyClasses and ResourceClasses as well as the assignments.
     * Access the information that has been provided to the instance
 
 UPDATE:
     * You need an instance of an existing Ontology by reading an instance
     * Change the attributes by assigning the new values
     * Call the ``update```method on the instance
 
 DELETE
-    * Instantiate a new objects with ``id``(IRI of group) given, or use any instance that has the id set,
+    * Instantiate a new objects with ``iri``(IRI of group) given, or use any instance that has the iri set,
       that is, that You've read before
     * Call the ``delete``-method on the instance
 """
 
+import copy
+import json
+import re
+from typing import Any, Optional, Union
+from urllib.parse import quote_plus
+
+from dsp_tools.models.connection import Connection
+from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.helpers import Actions, Context, DateTimeStamp, WithId
+from dsp_tools.models.model import Model
+from dsp_tools.models.project import Project
+from dsp_tools.models.propertyclass import PropertyClass
+from dsp_tools.models.resourceclass import ResourceClass
+from dsp_tools.models.set_encoder import SetEncoder
+
 
 class Ontology(Model):
-    ROUTE: str = '/v2/ontologies'
-    METADATA: str = '/metadata/'
-    ALL_LANGUAGES: str = '?allLanguages=true'
+    ROUTE: str = "/v2/ontologies"
+    METADATA: str = "/metadata/"
+    ALL_LANGUAGES: str = "?allLanguages=true"
 
-    _id: str
+    _iri: str
     _project: str
     _name: str
     _label: str
     _comment: str
     _lastModificationDate: DateTimeStamp
     _resource_classes: list[ResourceClass]
     _property_classes: list[PropertyClass]
     _context: Context
     _skiplist: list[str]
 
-    def __init__(self,
-                 con: Connection,
-                 id: Optional[str] = None,
-                 project: Optional[Union[str, Project]] = None,
-                 name: Optional[str] = None,
-                 label: Optional[str] = None,
-                 comment: Optional[str] = None,
-                 lastModificationDate: Optional[Union[str, DateTimeStamp]] = None,
-                 resource_classes: list[ResourceClass] = [],
-                 property_classes: list[PropertyClass] = [],
-                 context: Context = None):
+    def __init__(
+        self,
+        con: Connection,
+        iri: Optional[str] = None,
+        project: Optional[Union[str, Project]] = None,
+        name: Optional[str] = None,
+        label: Optional[str] = None,
+        comment: Optional[str] = None,
+        lastModificationDate: Optional[Union[str, DateTimeStamp]] = None,
+        resource_classes: Optional[list[ResourceClass]] = None,
+        property_classes: Optional[list[PropertyClass]] = None,
+        context: Context = None,
+    ):
         super().__init__(con)
-        self._id = id
+        self._iri = iri
         if isinstance(project, Project):
             self._project = project.id
         else:
             self._project = project
         self._name = name
         self._label = label
         self._comment = comment
         if lastModificationDate is None:
             self._lastModificationDate = None
         elif isinstance(lastModificationDate, DateTimeStamp):
             self._lastModificationDate = lastModificationDate
         else:
             self._lastModificationDate = DateTimeStamp(lastModificationDate)
-        self._resource_classes = resource_classes
-        self._property_classes = property_classes
+        self._resource_classes = resource_classes or []
+        self._property_classes = property_classes or []
         self._context = context if context is not None else Context()
         self._skiplist = []
 
     @property
-    def id(self) -> str:
-        return self._id
+    def iri(self) -> str:
+        return self._iri
 
-    @id.setter
-    def id(self, value: str):
-        raise BaseError('Ontology id cannot be modified!')
+    @iri.setter
+    def iri(self, value: str):
+        raise BaseError("Ontology iri cannot be modified!")
 
     @property
     def project(self) -> str:
         return self._project
 
     @project.setter
     def project(self, value: str):
@@ -115,24 +117,24 @@
     @property
     def label(self):
         return self._label
 
     @label.setter
     def label(self, value: str):
         self._label = str(value)
-        self._changed.add('label')
+        self._changed.add("label")
 
     @property
     def comment(self):
         return self._comment
 
     @comment.setter
     def comment(self, value: str):
         self._comment = str(value)
-        self._changed.add('comment')
+        self._changed.add("comment")
 
     @property
     def lastModificationDate(self) -> DateTimeStamp:
         return self._lastModificationDate
 
     @lastModificationDate.setter
     def lastModificationDate(self, value: Union[str, DateTimeStamp]):
@@ -144,15 +146,15 @@
 
     @resource_classes.setter
     def resource_classes(self, value: list[ResourceClass]) -> None:
         self._resource_classes = value
 
     def addResourceClass(self, resourceclass: ResourceClass, create: bool = False) -> tuple[int, ResourceClass]:
         if create:
-            print('Calling resourceclass.create in Ontology.addResourceClass')
+            print("Calling resourceclass.create in Ontology.addResourceClass")
             lmd, resourceclass = resourceclass.create(self._lastModificationDate)
             self._lastModificationDate = lmd
         self._resource_classes.append(resourceclass)
         index = len(self._resource_classes) - 1
         return index, resourceclass
 
     def updateResourceClass(self, index: int, resourceclass: ResourceClass) -> ResourceClass:
@@ -200,250 +202,235 @@
         return self._context
 
     @context.setter
     def context(self, value: Context):
         raise BaseError('"Context" cannot be set!')
 
     @classmethod
-    def fromJsonObj(cls, con: Connection, json_obj: Any) -> 'Ontology':
+    def fromJsonObj(cls, con: Connection, json_obj: Any) -> "Ontology":
         #
         # First let's get the ID (IRI) of the ontology
         #
-        id = json_obj.get('@id')
-        if id is None:
-            raise BaseError('Ontology id is missing')
+        iri = json_obj.get("@id")
+        if iri is None:
+            raise BaseError("Ontology iri is missing")
 
         #
         # evaluate the JSON-LD context to get the proper prefixes
         #
-        context = Context(json_obj.get('@context'))
-        onto_name = id.split('/')[-2]
-        context.add_context(onto_name, id + '#')
-        rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
+        context = Context(json_obj.get("@context"))
+        onto_name = iri.split("/")[-2]
+        context.add_context(onto_name, iri + "#")
         rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
-        owl = context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
-        xsd = context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
         knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
-        salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
-        this_onto = context.prefix_from_iri(id + "#")
+        this_onto = context.prefix_from_iri(iri + "#")
 
-        label = json_obj.get(rdfs + ':label')
+        label = json_obj.get(rdfs + ":label")
         if label is None:
-            raise BaseError('Ontology label is missing')
-        comment = json_obj.get(rdfs + ':comment')
-        if json_obj.get(knora_api + ':attachedToProject') is None:
-            raise BaseError('Ontology not attached to a project')
-        if json_obj[knora_api + ':attachedToProject'].get('@id') is None:
-            raise BaseError('Ontology not attached to a project')
-        project = json_obj[knora_api + ':attachedToProject']['@id']
-        tmp = json_obj.get(knora_api + ':lastModificationDate')
+            raise BaseError("Ontology label is missing")
+        comment = json_obj.get(rdfs + ":comment")
+        if json_obj.get(knora_api + ":attachedToProject") is None:
+            raise BaseError("Ontology not attached to a project")
+        if json_obj[knora_api + ":attachedToProject"].get("@id") is None:
+            raise BaseError("Ontology not attached to a project")
+        project = json_obj[knora_api + ":attachedToProject"]["@id"]
+        tmp = json_obj.get(knora_api + ":lastModificationDate")
         if tmp is not None:
-            last_modification_date = DateTimeStamp(json_obj.get(knora_api + ':lastModificationDate'))
+            last_modification_date = DateTimeStamp(json_obj.get(knora_api + ":lastModificationDate"))
         else:
             last_modification_date = None
         resource_classes = None
         property_classes = None
-        if json_obj.get('@graph') is not None:
+        if json_obj.get("@graph") is not None:
             resclasses_obj = list(
-                filter(lambda a: a.get(knora_api + ':isResourceClass') is not None, json_obj.get('@graph')))
-            resource_classes = list(map(lambda a: ResourceClass.fromJsonObj(con=con,
-                                                                            context=context,
-                                                                            json_obj=a), resclasses_obj))
-            standoffclasses_obj = list(
-                filter(lambda a: a.get(knora_api + ':isStandoffClass') is not None, json_obj.get('@graph')))
-            # ToDo: parse standoff classes
+                filter(lambda a: a.get(knora_api + ":isResourceClass") is not None, json_obj.get("@graph"))
+            )
+            resource_classes = list(
+                map(lambda a: ResourceClass.fromJsonObj(con=con, context=context, json_obj=a), resclasses_obj)
+            )
 
             properties_obj = list(
-                filter(lambda a: a.get(knora_api + ':isResourceProperty') is not None, json_obj.get('@graph')))
-            # property_classes = list(map(lambda a: PropertyClass.fromJsonObj(con=con,
-            #                                                                context=context,
-            #                                                                json_obj=a), properties_obj))
-            property_classes = [PropertyClass.fromJsonObj(con=con, context=context, json_obj=a) for a in properties_obj
-                                if WithId(a.get(knora_api + ':objectType')).str() != "knora-api:LinkValue"]
-        return cls(con=con,
-                   id=id,
-                   label=label,
-                   project=project,
-                   name=this_onto,  # TODO: corresponds the prefix always to the ontology name?
-                   comment=comment,
-                   lastModificationDate=last_modification_date,
-                   resource_classes=resource_classes,
-                   property_classes=property_classes,
-                   context=context)
+                filter(lambda a: a.get(knora_api + ":isResourceProperty") is not None, json_obj.get("@graph"))
+            )
+            property_classes = [
+                PropertyClass.fromJsonObj(con=con, context=context, json_obj=a)
+                for a in properties_obj
+                if WithId(a.get(knora_api + ":objectType")).str() != "knora-api:LinkValue"
+            ]
+        return cls(
+            con=con,
+            iri=iri,
+            label=label,
+            project=project,
+            name=this_onto,
+            comment=comment,
+            lastModificationDate=last_modification_date,
+            resource_classes=resource_classes,
+            property_classes=property_classes,
+            context=context,
+        )
 
     @classmethod
-    def __oneOntologiesFromJsonObj(cls, con: Connection, json_obj: Any, context: Context) -> 'Ontology':
-        rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
+    def __oneOntologiesFromJsonObj(cls, con: Connection, json_obj: Any, context: Context) -> "Ontology":
         rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
         owl = context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
-        xsd = context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
         knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
-        salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
-        if json_obj.get('@type') != owl + ':Ontology':
+        if json_obj.get("@type") != owl + ":Ontology":
             return None
-        id = json_obj.get('@id')
-        if id is None:
-            raise BaseError('Ontology id is missing')
-        if json_obj.get(knora_api + ':attachedToProject') is None:
-            raise BaseError('Ontology not attached to a project (1)')
-        if json_obj[knora_api + ':attachedToProject'].get('@id') is None:
-            raise BaseError('Ontology not attached to a project (2)')
-        project = json_obj[knora_api + ':attachedToProject']['@id']
-        tmp = json_obj.get(knora_api + ':lastModificationDate')
+        iri = json_obj.get("@id")
+        if iri is None:
+            raise BaseError("Ontology iri is missing")
+        if json_obj.get(knora_api + ":attachedToProject") is None:
+            raise BaseError("Ontology not attached to a project (1)")
+        if json_obj[knora_api + ":attachedToProject"].get("@id") is None:
+            raise BaseError("Ontology not attached to a project (2)")
+        project = json_obj[knora_api + ":attachedToProject"]["@id"]
+        tmp = json_obj.get(knora_api + ":lastModificationDate")
         if tmp is not None:
-            last_modification_date = DateTimeStamp(json_obj.get(knora_api + ':lastModificationDate'))
+            last_modification_date = DateTimeStamp(json_obj.get(knora_api + ":lastModificationDate"))
         else:
             last_modification_date = None
-        label = json_obj.get(rdfs + ':label')
+        label = json_obj.get(rdfs + ":label")
         if label is None:
-            raise BaseError('Ontology label is missing')
-        comment = json_obj.get(rdfs + ':comment')
-        this_onto = id.split('/')[-2]
+            raise BaseError("Ontology label is missing")
+        comment = json_obj.get(rdfs + ":comment")
+        this_onto = iri.split("/")[-2]
         context2 = copy.deepcopy(context)
-        context2.add_context(this_onto, id)
-        return cls(con=con,
-                   id=id,
-                   label=label,
-                   project=project,
-                   name=this_onto,
-                   comment=comment,
-                   lastModificationDate=last_modification_date,
-                   context=context2)
+        context2.add_context(this_onto, iri)
+        return cls(
+            con=con,
+            iri=iri,
+            label=label,
+            project=project,
+            name=this_onto,
+            comment=comment,
+            lastModificationDate=last_modification_date,
+            context=context2,
+        )
 
     @classmethod
-    def allOntologiesFromJsonObj(cls, con: Connection, json_obj: Any) -> list['Ontology']:
-        context = Context(json_obj.get('@context'))
-        rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-        rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
-        owl = context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
-        xsd = context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
-        knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
-        salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
-        ontos: list['Ontology'] = []
-        if json_obj.get('@graph') is not None:
-            for o in json_obj['@graph']:
+    def allOntologiesFromJsonObj(cls, con: Connection, json_obj: Any) -> list["Ontology"]:
+        context = Context(json_obj.get("@context"))
+        ontos: list["Ontology"] = []
+        if json_obj.get("@graph") is not None:
+            for o in json_obj["@graph"]:
                 ontos.append(Ontology.__oneOntologiesFromJsonObj(con, o, context))
         else:
             onto = Ontology.__oneOntologiesFromJsonObj(con, json_obj, context)
             if onto is not None:
                 ontos.append(onto)
         return ontos
 
     def toJsonObj(self, action: Actions) -> Any:
-        rdf = self._context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
         rdfs = self._context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
-        owl = self._context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
-        xsd = self._context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
         knora_api = self._context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
-        salsah_gui = self._context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
-        # this_onto = self._context.prefixFromIri(self._id + "#")
         tmp = {}
         if action == Actions.Create:
             if self._name is None:
-                raise BaseError('There must be a valid name given!')
+                raise BaseError("There must be a valid name given!")
             if self._label is None:
-                raise BaseError('There must be a valid label given!')
+                raise BaseError("There must be a valid label given!")
             if self._project is None:
-                raise BaseError('There must be a valid project given!')
+                raise BaseError("There must be a valid project given!")
             tmp = {
                 knora_api + ":ontologyName": self._name,
-                knora_api + ":attachedToProject": {
-                    "@id": self._project
-                },
+                knora_api + ":attachedToProject": {"@id": self._project},
                 rdfs + ":label": self._label,
-                "@context": self._context.toJsonObj()
+                "@context": self._context.toJsonObj(),
             }
             if self._comment is not None:
                 tmp[rdfs + ":comment"] = self._comment
         elif action == Actions.Update:
             if self._lastModificationDate is None:
                 raise BaseError("'last_modification_date' must be in ontology!")
             tmp = {
-                '@id': self._id,
-                rdfs + ':label': self._label,
-                knora_api + ':lastModificationDate': self._lastModificationDate.toJsonObj(),
-                "@context": self._context.toJsonObj()
+                "@id": self._iri,
+                rdfs + ":label": self._label,
+                knora_api + ":lastModificationDate": self._lastModificationDate.toJsonObj(),
+                "@context": self._context.toJsonObj(),
             }
-            if self._label is not None and 'label' in self._changed:
-                tmp[rdfs + ':label'] = self._label
-            if self._comment is not None and 'comment' in self._changed:
-                tmp[rdfs + ':comment'] = self._comment
+            if self._label is not None and "label" in self._changed:
+                tmp[rdfs + ":label"] = self._label
+            if self._comment is not None and "comment" in self._changed:
+                tmp[rdfs + ":comment"] = self._comment
         return tmp
 
-    def create(self, dumpjson: Optional[str] = None) -> 'Ontology':
+    def create(self) -> "Ontology":
         jsonobj = self.toJsonObj(Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
         result = self._con.post(Ontology.ROUTE, jsondata)
         return Ontology.fromJsonObj(self._con, result)
 
-    def update(self) -> 'Ontology':
+    def update(self) -> "Ontology":
         jsonobj = self.toJsonObj(Actions.Update)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
-        result = self._con.put(Ontology.ROUTE + '/metadata', jsondata, 'application/ld+json')
+        result = self._con.put(Ontology.ROUTE + "/metadata", jsondata, "application/ld+json")
         return Ontology.fromJsonObj(self._con, result)
 
-    def read(self) -> 'Ontology':
-        result = self._con.get(Ontology.ROUTE + '/allentities/' + quote_plus(self._id) + Ontology.ALL_LANGUAGES)
+    def read(self) -> "Ontology":
+        result = self._con.get(Ontology.ROUTE + "/allentities/" + quote_plus(self._iri) + Ontology.ALL_LANGUAGES)
         return Ontology.fromJsonObj(self._con, result)
 
     def delete(self) -> Optional[str]:
-        result = self._con.delete(Ontology.ROUTE + '/' + quote_plus(self._id),
-                                  params={'lastModificationDate': str(self._lastModificationDate)})
-        return result.get('knora-api:result')
+        result = self._con.delete(
+            Ontology.ROUTE + "/" + quote_plus(self._iri),
+            params={"lastModificationDate": str(self._lastModificationDate)},
+        )
+        return result.get("knora-api:result")
 
     @staticmethod
-    def getAllOntologies(con: Connection) -> list['Ontology']:
+    def getAllOntologies(con: Connection) -> list["Ontology"]:
         result = con.get(Ontology.ROUTE + Ontology.METADATA)
         return Ontology.allOntologiesFromJsonObj(con, result)
 
     @staticmethod
-    def getProjectOntologies(con: Connection, project_id: str) -> list['Ontology']:
+    def getProjectOntologies(con: Connection, project_id: str) -> list["Ontology"]:
         if project_id is None:
-            raise BaseError('Project ID must be defined!')
+            raise BaseError("Project ID must be defined!")
         result = con.get(Ontology.ROUTE + Ontology.METADATA + quote_plus(project_id) + Ontology.ALL_LANGUAGES)
         return Ontology.allOntologiesFromJsonObj(con, result)
 
     @staticmethod
-    def getOntologyFromServer(con: Connection, shortcode: str, name: str) -> 'Ontology':
-        if re.search(r'[0-9A-F]{4}', shortcode):
+    def getOntologyFromServer(con: Connection, shortcode: str, name: str) -> "Ontology":
+        if re.search(r"[0-9A-F]{4}", shortcode):
             result = con.get("/ontology/" + shortcode + "/" + name + "/v2" + Ontology.ALL_LANGUAGES)
         else:
             result = con.get("/ontology/" + name + "/v2" + Ontology.ALL_LANGUAGES)
         return Ontology.fromJsonObj(con, result)
 
     def createDefinitionFileObj(self) -> dict[str, Any]:
         ontology = {
             "name": self.name,
             "label": self.label,
             "comment": self.comment,
             "properties": [],
-            "resources": []
+            "resources": [],
         }
         if not self.comment:
             ontology.pop("comment")
         for prop in self.property_classes:
             if "knora-api:hasLinkToValue" in prop.superproperties:
-                self.skiplist.append(self.name + ":" + prop.name)
+                self._skiplist.append(self.name + ":" + prop.name)
                 continue
             ontology["properties"].append(prop.createDefinitionFileObj(self.context, self.name))
 
         for res in self.resource_classes:
             ontology["resources"].append(res.createDefinitionFileObj(self.context, self.name, self._skiplist))
 
         return ontology
 
     def print(self, short: bool = True) -> None:
-        print('Ontology Info:')
-        print('  Id:                   {}'.format(self._id))
-        print('  Label:                {}'.format(self._label))
-        print('  Name:                 {}'.format(self._name))
-        print('  Project:              {}'.format(self._project))
-        print('  LastModificationDate: {}'.format(str(self._lastModificationDate)))
+        print("Ontology Info:")
+        print("  IRI:                  {}".format(self._iri))
+        print("  Label:                {}".format(self._label))
+        print("  Name:                 {}".format(self._name))
+        print("  Project:              {}".format(self._project))
+        print("  LastModificationDate: {}".format(str(self._lastModificationDate)))
         if not short:
-            print('  Property Classes:')
+            print("  Property Classes:")
             if self._property_classes:
                 for pc in self._property_classes:
                     pc.print(4)
-            print('  Resource Classes:')
+            print("  Resource Classes:")
             if self._resource_classes:
                 for rc in self._resource_classes:
                     rc.print(4)
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/permission.py` & `dsp_tools-2.3.3/src/dsp_tools/models/permission.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,29 @@
     V = 2
     M = 4
     D = 8
     CR = 16
 
     def __str__(self):
         tmp = {
-            1: 'RV',
-            2: 'V',
-            4: 'M',
-            8: 'D',
-            16: 'CR'
+            1: "RV",
+            2: "V",
+            4: "M",
+            8: "D",
+            16: "CR",
         }
         return tmp[self.value]
 
 
 class PermissionsIterator:
-    _permissions: 'Permissions'
+    _permissions: "Permissions"
     _group: list[str]
     _index: int
 
-    def __init__(self, permissions: 'Permissions'):
+    def __init__(self, permissions: "Permissions"):
         self._permissions = permissions
         self._index = 0
 
     def __next__(self):
         if len(self._permissions.permissions) == 0 and self._index == 0:
             return None, None
         elif self._index < len(self._permissions.permissions):
@@ -41,16 +41,15 @@
         else:
             raise StopIteration
 
 
 class Permissions:
     _permissions: Union[dict[PermissionValue, list[str]], None]
 
-    def __init__(self,
-                 permissions: Optional[dict[PermissionValue, list[str]]] = None):
+    def __init__(self, permissions: Optional[dict[PermissionValue, list[str]]] = None):
         if permissions is None:
             self._permissions = {}
         else:
             self._permissions = permissions
 
     def __getitem__(self, key: PermissionValue) -> Union[list[str], None]:
         return self._permissions.get(key)
@@ -67,38 +66,38 @@
     def __iter__(self) -> PermissionsIterator:
         return PermissionsIterator(self)
 
     def __contains__(self, key: PermissionValue) -> bool:
         return key in self._permissions
 
     def __str__(self):
-        tmpstr = ''
+        tmpstr = ""
         for permission, groups in self._permissions.items():
             if tmpstr:
-                tmpstr += '|'
-            tmpstr += str(permission) + ' ' + ",".join(groups)
+                tmpstr += "|"
+            tmpstr += str(permission) + " " + ",".join(groups)
         return tmpstr
 
     def add(self, key: PermissionValue, val: str):
         if self._permissions.get(key) is None:
             self._permissions[key] = [val]
         else:
             self._permissions[key].append(val)
 
     def toJsonLdObj(self):
-        tmpstr = ''
+        tmpstr = ""
         for permission, groups in self._permissions.items():
             if tmpstr:
-                tmpstr += '|'
-            tmpstr += str(permission) + ' ' + ",".join(groups)
+                tmpstr += "|"
+            tmpstr += str(permission) + " " + ",".join(groups)
         return tmpstr
 
     @classmethod
     def fromString(cls, permstr: str):
-        tmpstr = permstr.split('|')
+        tmpstr = permstr.split("|")
         permissions: dict[PermissionValue, list[str]] = {}
         for s in tmpstr:
             key, *vals = re.split("[\\s,]+", s)
             permissions[PermissionValue[key]] = vals
         return cls(permissions)
 
     @property
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/project.py` & `dsp_tools-2.3.3/src/dsp_tools/models/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.helpers import Actions
 from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.model import Model
 from dsp_tools.models.set_encoder import SetEncoder
 
 """
-This module implements the handling (CRUD) of Knora projects.
+This module implements the handling (CRUD) of DSP projects.
 
 CREATE:
     * Instantiate a new object of the class Project with all required parameters
     * Call the ``create``-method on the instance
 
 READ:
     * Instantiate a new object with ``id``(IRI of project) given
@@ -35,36 +35,36 @@
 
 In addition there is a static methods ``getAllProjects`` which returns a list of all projects
 """
 
 
 class Project(Model):
     """
-    This class represents a project in Knora.
+    This class represents a project in DSP.
 
     Attributes
     ----------
 
     con : Connection
-        A Connection instance to a Knora server
+        A Connection instance to a DSP server
 
     id : str
         IRI of the project [readonly, cannot be modified after creation of instance]
 
     shortcode : str
-        Knora project shortcode [readonly, cannot be modified after creation of instance]
+        DSP project shortcode [readonly, cannot be modified after creation of instance]
 
     shortname : str
-        Knora project shortname [read/write]
+        DSP project shortname [read/write]
 
     longname : str
-        Knora project longname [read/write]
+        DSP project longname [read/write]
 
     description : LangString
-        Knora project description in a given language (Languages.EN, Languages.DE, Languages.FR, Languages.IT).
+        DSP project description in a given language (Languages.EN, Languages.DE, Languages.FR, Languages.IT).
         A desciption can be add/replaced or removed with the methods ``addDescription``and ``rmDescription``.
 
     keywords : set[str]
         Set of keywords describing the project. Keywords can be added/removed by the methods ``addKeyword``
         and ``rmKeyword``
 
     ontologies : set[str]
@@ -73,24 +73,24 @@
     selfjoin : bool
         Boolean if the project allows selfjoin
 
 
     Methods
     -------
 
-    create : Knora project information object
-        Creates a new project and returns the information from the project as it is in Knora
+    create : DSP project information object
+        Creates a new project and returns the information from the project as it is in DSP
 
-    read : Knora project information object
+    read : DSP project information object
         Read project data from an existing project
 
-    update : Knora project information object
-        Updates the changed attributes and returns the updated information from the project as it is in Knora
+    update : DSP project information object
+        Updates the changed attributes and returns the updated information from the project as it is in DSP
 
-    delete : Knora result code
+    delete : DSP result code
         Deletes a project and returns the result code
 
     getAllprojects [static]: List of all projects
         Returns a list of all projects available
 
     print : None
         Prints the project information to stdout
@@ -109,26 +109,28 @@
     _ontologies: set[str]
     _selfjoin: bool
     _status: bool
     _logo: Optional[str]
 
     SYSTEM_PROJECT: str = "http://www.knora.org/ontology/knora-admin#SystemProject"
 
-    def __init__(self,
-                 con: Connection,
-                 id: Optional[str] = None,
-                 shortcode: Optional[str] = None,
-                 shortname: Optional[str] = None,
-                 longname: Optional[str] = None,
-                 description: LangString = None,
-                 keywords: Optional[set[str]] = None,
-                 ontologies: Optional[set[str]] = None,
-                 selfjoin: Optional[bool] = None,
-                 status: Optional[bool] = None,
-                 logo: Optional[str] = None):
+    def __init__(
+        self,
+        con: Connection,
+        id: Optional[str] = None,
+        shortcode: Optional[str] = None,
+        shortname: Optional[str] = None,
+        longname: Optional[str] = None,
+        description: LangString = None,
+        keywords: Optional[set[str]] = None,
+        ontologies: Optional[set[str]] = None,
+        selfjoin: Optional[bool] = None,
+        status: Optional[bool] = None,
+        logo: Optional[str] = None,
+    ):
         """
         Constructor for Project
 
         :param con: Connection instance
         :param id: IRI of the project [required for CREATE, READ]
         :param shortcode: Shortcode of the project. String inf the form 'XXXX' where each X is a hexadezimal sign 0-1,A,B,C,D,E,F. [required for CREATE]
         :param shortname: Shortname of the project [required for CREATE]
@@ -144,15 +146,15 @@
         self._id = id
         self._shortcode = shortcode
         self._shortname = shortname
         self._longname = longname
         self._description = LangString(description)
         self._keywords = keywords
         if not isinstance(ontologies, set) and ontologies is not None:
-            raise BaseError('Ontologies must be a set of strings or None!')
+            raise BaseError("Ontologies must be a set of strings or None!")
         self._ontologies = ontologies
         self._selfjoin = selfjoin
         self._status = status
         self._logo = logo
 
     def __str__(self):
         tmpstr = self._id + "\n  " + self._shortcode + "\n  " + self._shortname
@@ -163,327 +165,331 @@
     #
     @property
     def id(self) -> Optional[str]:
         return self._id
 
     @id.setter
     def id(self, value: str) -> None:
-        raise BaseError('Project id cannot be modified!')
+        raise BaseError("Project id cannot be modified!")
 
     @property
     def shortcode(self) -> Optional[str]:
         return self._shortcode
 
     @shortcode.setter
     def shortcode(self, value: str) -> None:
-        raise BaseError('Shortcode id cannot be modified!')
+        raise BaseError("Shortcode id cannot be modified!")
 
     @property
     def shortname(self) -> Optional[str]:
         return self._shortname
 
     @shortname.setter
     def shortname(self, value: str) -> None:
         if self._shortname != str(value):
             self._shortname = str(value)
-            self._changed.add('shortname')
+            self._changed.add("shortname")
 
     @property
     def longname(self) -> Optional[str]:
         return self._longname
 
     @longname.setter
     def longname(self, value: str) -> None:
         if self._longname != str(value):
             self._longname = str(value)
-            self._changed.add('longname')
+            self._changed.add("longname")
 
     @property
     def description(self) -> LangString:
         return self._description or LangString({})
 
     @description.setter
     def description(self, value: Optional[LangString]) -> None:
         self._description = LangString(value)
-        self._changed.add('description')
+        self._changed.add("description")
 
     def addDescription(self, lang: Union[Languages, str], value: str) -> None:
         """
         Add/replace a project description with the given language (executed at next update)
 
         :param lang: The language the description is in, either a string "EN", "DE", "FR", "IT" or a Language instance
         :param value: The text of the description
         :return: None
         """
 
         self._description[lang] = value
-        self._changed.add('description')
+        self._changed.add("description")
 
     def rmDescription(self, lang: Union[Languages, str]) -> None:
         """
         Remove a description from a project (executed at next update)
 
         :param lang: The language the description to be removed is in, either a string "EN", "DE", "FR", "IT" or a Language instance
         :return: None
         """
 
         del self._description[lang]
-        self._changed.add('description')
+        self._changed.add("description")
 
     @property
     def keywords(self) -> set[str]:
         return self._keywords
 
     @keywords.setter
     def keywords(self, value: Union[list[str], set[str]]):
         if isinstance(value, set):
             self._keywords = value
-            self._changed.add('keywords')
+            self._changed.add("keywords")
         elif isinstance(value, list):
             self._keywords = set(value)
-            self._changed.add('keywords')
+            self._changed.add("keywords")
         else:
-            raise BaseError('Must be a set of strings!')
+            raise BaseError("Must be a set of strings!")
 
     def addKeyword(self, value: str):
         """
         Add a new keyword to the set of keywords. (executed at next update)
         May raise a BaseError
 
         :param value: keyword
         :return: None
         """
 
         self._keywords.add(value)
-        self._changed.add('keywords')
+        self._changed.add("keywords")
 
     def rmKeyword(self, value: str):
         """
         Remove a keyword from the list of keywords (executed at next update)
         May raise a BaseError
 
         :param value: keyword
         :return: None
         """
         try:
             self._keywords.remove(value)
         except KeyError as ke:
             raise BaseError('Keyword "' + value + '" is not in keyword set')
-        self._changed.add('keywords')
+        self._changed.add("keywords")
 
     @property
     def ontologies(self) -> set[str]:
         return self._ontologies
 
     @ontologies.setter
     def ontologies(self, value: set[str]) -> None:
-        raise BaseError('Cannot add a ontology!')
+        raise BaseError("Cannot add a ontology!")
 
     @property
     def selfjoin(self) -> Optional[bool]:
         return self._selfjoin
 
     @selfjoin.setter
     def selfjoin(self, value: bool) -> None:
         if self._selfjoin != value:
-            self._changed.add('selfjoin')
+            self._changed.add("selfjoin")
             self._selfjoin = value
 
     @property
     def status(self) -> bool:
         return self._status
 
     @status.setter
     def status(self, value: bool) -> None:
         if self._status != value:
             self._status = value
-            self._changed.add('status')
+            self._changed.add("status")
 
     @property
     def logo(self) -> str:
         return self._logo
 
     @logo.setter
     def logo(self, value: str) -> None:
         if self._logo != value:
             self._logo = value
-            self._changed.add('logo')
+            self._changed.add("logo")
 
     @classmethod
     def fromJsonObj(cls, con: Connection, json_obj: Any) -> Project:
         """
         Internal method! Should not be used directly!
 
-        This method is used to create a Project instance from the JSON data returned by Knora
+        This method is used to create a Project instance from the JSON data returned by DSP
 
         :param con: Connection instance
-        :param json_obj: JSON data returned by Knora as python3 object
+        :param json_obj: JSON data returned by DSP as python3 object
         :return: Project instance
         """
-        id = json_obj.get('id')
+        id = json_obj.get("id")
         if id is None:
-            raise BaseError('Project id is missing')
-        shortcode = json_obj.get('shortcode')
+            raise BaseError("Project id is missing")
+        shortcode = json_obj.get("shortcode")
         if shortcode is None:
             raise BaseError("Shortcode is missing")
-        shortname = json_obj.get('shortname')
+        shortname = json_obj.get("shortname")
         if shortname is None:
             raise BaseError("Shortname is missing")
-        longname = json_obj.get('longname')
+        longname = json_obj.get("longname")
         if longname is None:
             raise BaseError("Longname is missing")
-        description = LangString.fromJsonObj(json_obj.get('description'))
-        keywords = set(json_obj.get('keywords'))
+        description = LangString.fromJsonObj(json_obj.get("description"))
+        keywords = set(json_obj.get("keywords"))
         if keywords is None:
             raise BaseError("Keywords are missing")
-        ontologies = set(json_obj.get('ontologies'))
+        ontologies = set(json_obj.get("ontologies"))
         if ontologies is None:
             raise BaseError("ontologies are missing")
-        selfjoin = json_obj.get('selfjoin')
+        selfjoin = json_obj.get("selfjoin")
         if selfjoin is None:
             raise BaseError("Selfjoin is missing")
-        status = json_obj.get('status')
+        status = json_obj.get("status")
         if status is None:
             raise BaseError("Status is missing")
-        logo = json_obj.get('logo')
-        return cls(con=con,
-                   id=id,
-                   shortcode=shortcode,
-                   shortname=shortname,
-                   longname=longname,
-                   description=description,
-                   keywords=keywords,
-                   ontologies=ontologies,
-                   selfjoin=selfjoin,
-                   status=status,
-                   logo=logo)
+        logo = json_obj.get("logo")
+        return cls(
+            con=con,
+            id=id,
+            shortcode=shortcode,
+            shortname=shortname,
+            longname=longname,
+            description=description,
+            keywords=keywords,
+            ontologies=ontologies,
+            selfjoin=selfjoin,
+            status=status,
+            logo=logo,
+        )
 
     def toJsonObj(self, action: Actions) -> dict[str, str]:
         """
         Internal method! Should not be used directly!
 
-        Creates a JSON-object from the Project instance that can be used to call Knora
+        Creates a JSON-object from the Project instance that can be used to call DSP
 
         :param action: Action the object is used for (Action.CREATE or Action.UPDATE)
         :return: JSON-object
         """
 
         tmp = {}
         if action == Actions.Create:
             if self._shortcode is None:
                 raise BaseError("There must be a valid project shortcode!")
-            tmp['shortcode'] = self._shortcode
+            tmp["shortcode"] = self._shortcode
             if self._shortname is None:
                 raise BaseError("There must be a valid project shortname!")
-            tmp['shortname'] = self._shortname
+            tmp["shortname"] = self._shortname
             if self._longname is None:
                 raise BaseError("There must be a valid project longname!")
-            tmp['longname'] = self._longname
+            tmp["longname"] = self._longname
             if self._description.isEmpty():
                 raise BaseError("There must be a valid project description!")
-            tmp['description'] = self._description.toJsonObj()
+            tmp["description"] = self._description.toJsonObj()
             if self._keywords is not None and len(self._keywords) > 0:
-                tmp['keywords'] = self._keywords
+                tmp["keywords"] = self._keywords
             if self._selfjoin is None:
                 raise BaseError("selfjoin must be defined (True or False!")
-            tmp['selfjoin'] = self._selfjoin
+            tmp["selfjoin"] = self._selfjoin
             if self._status is None:
                 raise BaseError("status must be defined (True or False!")
-            tmp['status'] = self._status
+            tmp["status"] = self._status
 
         elif action == Actions.Update:
-            if self._shortcode is not None and 'shortcode' in self._changed:
-                tmp['shortcode'] = self._shortcode
-            if self._shortname is not None and 'shortname' in self._changed:
-                tmp['shortname'] = self._shortname
-            if self._longname is not None and 'longname' in self._changed:
-                tmp['longname'] = self._longname
-            if not self._description.isEmpty() and 'description' in self._changed:
-                tmp['description'] = self._description.toJsonObj()
-            if len(self._keywords) > 0 and 'keywords' in self._changed:
-                tmp['keywords'] = self._keywords
-            if self._selfjoin is not None and 'selfjoin' in self._changed:
-                tmp['selfjoin'] = self._selfjoin
-            if self._status is not None and 'status' in self._changed:
-                tmp['status'] = self._status
+            if self._shortcode is not None and "shortcode" in self._changed:
+                tmp["shortcode"] = self._shortcode
+            if self._shortname is not None and "shortname" in self._changed:
+                tmp["shortname"] = self._shortname
+            if self._longname is not None and "longname" in self._changed:
+                tmp["longname"] = self._longname
+            if not self._description.isEmpty() and "description" in self._changed:
+                tmp["description"] = self._description.toJsonObj()
+            if len(self._keywords) > 0 and "keywords" in self._changed:
+                tmp["keywords"] = self._keywords
+            if self._selfjoin is not None and "selfjoin" in self._changed:
+                tmp["selfjoin"] = self._selfjoin
+            if self._status is not None and "status" in self._changed:
+                tmp["status"] = self._status
         return tmp
 
     def createDefinitionFileObj(self) -> dict[str, Any]:
         return {
             "shortcode": self._shortcode,
             "shortname": self._shortname,
             "longname": self._longname,
             "descriptions": self._description.createDefinitionFileObj(),
-            "keywords": [kw for kw in self._keywords]
+            "keywords": [kw for kw in self._keywords],
         }
 
     def create(self) -> Project:
         """
-        Create a new project in Knora
+        Create a new project in DSP
 
-        :return: JSON-object from Knora
+        :return: JSON-object from DSP
         """
 
         jsonobj = self.toJsonObj(Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder)
         result = self._con.post(Project.ROUTE, jsondata)
-        return Project.fromJsonObj(self._con, result['project'])
+        return Project.fromJsonObj(self._con, result["project"])
 
     def read(self) -> Project:
         """
-        Read a project from Knora
+        Read a project from DSP
 
-        :return: JSON-object from Knora
+        :return: JSON-object from DSP
         """
         result = None
         if self._id is not None:
             result = self._con.get(Project.IRI + quote_plus(self._id))
         elif self._shortcode is not None:
-            result = self._con.get(Project.ROUTE + '/shortcode/' + quote_plus(self._shortcode))
+            result = self._con.get(Project.ROUTE + "/shortcode/" + quote_plus(self._shortcode))
         elif self._shortname is not None:
-            result = self._con.get(Project.ROUTE + '/shortname/' + quote_plus(self._shortname))
+            result = self._con.get(Project.ROUTE + "/shortname/" + quote_plus(self._shortname))
         if result is not None:
-            return Project.fromJsonObj(self._con, result['project'])
+            return Project.fromJsonObj(self._con, result["project"])
         else:
-            raise BaseError(f"ERROR: Could not read project '{self.shortname}' ({self.shortcode}) with IRI {self._id} "
-                            f"from DSP server.")
+            raise BaseError(
+                f"ERROR: Could not read project '{self.shortname}' ({self.shortcode}) with IRI {self._id} "
+                f"from DSP server."
+            )
 
     def update(self) -> Project:
         """
         Update the project information on the DSP with the modified data in this project instance
 
         Returns: JSON object returned as response from DSP reflecting the update
         """
 
         jsonobj = self.toJsonObj(Actions.Update)
         jsondata = json.dumps(jsonobj, cls=SetEncoder)
         result = self._con.put(Project.IRI + quote_plus(self.id), jsondata)
-        return Project.fromJsonObj(self._con, result['project'])
+        return Project.fromJsonObj(self._con, result["project"])
 
     def delete(self) -> Project:
         """
-        Delete the given Knora project
+        Delete the given DSP project
 
-        :return: Knora response
+        :return: DSP response
         """
 
         result = self._con.delete(Project.IRI + quote_plus(self._id))
-        return Project.fromJsonObj(self._con, result['project'])
+        return Project.fromJsonObj(self._con, result["project"])
 
     def set_default_permissions(self, group_id: str) -> None:
         permobj = {
             "forGroup": "http://www.knora.org/ontology/knora-admin#ProjectMember",
             "forProject": self._id,
             "hasPermissions": [
                 {
                     "additionalInformation": None,
                     "name": "ProjectResourceCreateAllPermission",
-                    "permissionCode": None
+                    "permissionCode": None,
                 }
-            ]
+            ],
         }
         jsondata = json.dumps(permobj, indent=4)
         print(jsondata)
         result = self._con.post("/admin/permissions/ap", jsondata)
         pprint(result)
 
         return
@@ -492,56 +498,56 @@
             "forProject": self._id,
             "forProperty": None,
             "forResourceClass": None,
             "hasPermissions": [
                 {
                     "additionalInformation": "http://www.knora.org/ontology/knora-admin#ProjectMember",
                     "name": "D",
-                    "permissionCode": 7
+                    "permissionCode": 7,
                 }
-            ]
+            ],
         }
         jsondata = json.dumps(permobj)
         result = self._con.post("/admin/permissions/ap", jsondata)
         pprint(result)
 
     @staticmethod
     def getAllProjects(con: Connection) -> list[Project]:
         """
-        Get all existing projects in Knora
+        Get all existing projects in DSP
 
         :param con: Connection instance
         :return:
         """
         result = con.get(Project.ROUTE)
-        if 'projects' not in result:
+        if "projects" not in result:
             raise BaseError("Request got no projects!")
-        return [Project.fromJsonObj(con, a) for a in result['projects']]
+        return [Project.fromJsonObj(con, a) for a in result["projects"]]
 
     def print(self) -> None:
         """
         print info to stdout
 
         :return: None
         """
 
-        print('Project Info:')
-        print('  Id:         {}'.format(self._id))
-        print('  Shortcode:  {}'.format(self._shortcode))
-        print('  Shortname:  {}'.format(self._shortname))
-        print('  Longname:   {}'.format(self._longname))
+        print("Project Info:")
+        print("  Id:         {}".format(self._id))
+        print("  Shortcode:  {}".format(self._shortcode))
+        print("  Shortname:  {}".format(self._shortname))
+        print("  Longname:   {}".format(self._longname))
         if self._description is not None:
-            print('  Description:')
+            print("  Description:")
             for descr in self._description.items():
-                print('    {}: {}'.format(descr[0], descr[1]))
+                print("    {}: {}".format(descr[0], descr[1]))
         else:
-            print('  Description: None')
+            print("  Description: None")
         if self._keywords is not None:
-            print('  Keywords:   {}'.format(' '.join(self._keywords)))
+            print("  Keywords:   {}".format(" ".join(self._keywords)))
         else:
-            print('  Keywords:   None')
+            print("  Keywords:   None")
         if self._ontologies is not None:
-            print('  Ontologies: {}'.format(' '.join(self._ontologies)))
+            print("  Ontologies: {}".format(" ".join(self._ontologies)))
         else:
-            print('  Ontologies: None')
-        print('  Selfjoin:   {}'.format(self._selfjoin))
-        print('  Status:     {}'.format(self._status))
+            print("  Ontologies: None")
+        print("  Selfjoin:   {}".format(self._selfjoin))
+        print("  Status:     {}".format(self._status))
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/projectContext.py` & `dsp_tools-2.3.3/src/dsp_tools/models/projectContext.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,17 @@
         self._project_map: dict[str, str] = {x.shortname: x.id for x in self._projects}
         self._inv_project_map: dict[str, str] = {x.id: x.shortname for x in self._projects}
         try:
             self._groups = Group.getAllGroups(con=con)
         except BaseError:
             self._groups = None
         if self._groups:
-            self._group_map: dict[str, str] = {self._inv_project_map[x.project] + ':' + x.name: x.id for x in
-                                               self._groups}
+            self._group_map: dict[str, str] = {
+                self._inv_project_map[x.project] + ":" + x.name: x.iri for x in self._groups
+            }
         else:
             self._group_map = None
         self._project_name = None
         # get the project name from the shortcode
         if self._shortcode:
             for p in self._projects:
                 if p.shortcode == self._shortcode:
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/propertyclass.py` & `dsp_tools-2.3.3/src/dsp_tools/models/propertyclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,29 +25,31 @@
     _gui_element: str
     _gui_attributes: dict[str, str]
     _label: LangString
     _comment: LangString
     _editable: bool
     _linkvalue: bool
 
-    def __init__(self,
-                 con: Connection,
-                 context: Context,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None,
-                 ontology_id: Optional[str] = None,
-                 superproperties: Optional[Sequence[Union['PropertyClass', str]]] = None,
-                 object: Optional[str] = None,
-                 subject: Optional[str] = None,
-                 gui_element: Optional[str] = None,
-                 gui_attributes: Optional[dict[str, str]] = None,
-                 label: Optional[Union[LangString, str]] = None,
-                 comment: Optional[Union[LangString, str]] = None,
-                 editable: Optional[bool] = None,
-                 linkvalue: Optional[bool] = None):
+    def __init__(
+        self,
+        con: Connection,
+        context: Context,
+        id: Optional[str] = None,
+        name: Optional[str] = None,
+        ontology_id: Optional[str] = None,
+        superproperties: Optional[Sequence[Union["PropertyClass", str]]] = None,
+        object: Optional[str] = None,
+        subject: Optional[str] = None,
+        gui_element: Optional[str] = None,
+        gui_attributes: Optional[dict[str, str]] = None,
+        label: Optional[Union[LangString, str]] = None,
+        comment: Optional[Union[LangString, str]] = None,
+        editable: Optional[bool] = None,
+        linkvalue: Optional[bool] = None,
+    ):
         super().__init__(con)
         if not isinstance(context, Context):
             raise BaseError('"context"-parameter must be an instance of Context')
         self._context = context
         self._id = id
         self._name = name
         self._ontology_id = ontology_id
@@ -64,27 +66,27 @@
         #
         if label is not None:
             if isinstance(label, str):
                 self._label = LangString(label)
             elif isinstance(label, LangString):
                 self._label = label
             else:
-                raise BaseError('Invalid LangString for label!')
+                raise BaseError("Invalid LangString for label!")
         else:
             self._label = LangString({})
         #
         # process comment
         #
         if comment is not None:
             if isinstance(comment, str):
                 self._comment = LangString(comment)
             elif isinstance(comment, LangString):
                 self._comment = comment
             else:
-                raise BaseError('Invalid LangString for comment!')
+                raise BaseError("Invalid LangString for comment!")
         else:
             self._comment = LangString({})
 
         self._editable = editable
         self._linkvalue = linkvalue
 
     #
@@ -141,33 +143,33 @@
     @property
     def gui_element(self) -> Optional[str]:
         return self._gui_element
 
     @gui_element.setter
     def gui_element(self, value: str) -> None:
         self._gui_element = value
-        self._changed.append('gui_element')
+        self._changed.append("gui_element")
 
     @property
     def gui_attributes(self) -> Optional[dict[str, str]]:
         return self._gui_attributes
 
     @gui_attributes.setter
     def gui_attributes(self, value: list[dict[str, str]]) -> None:
         self._gui_attributes = value
-        self._changed.append('gui_attributes')
+        self._changed.append("gui_attributes")
 
     def addGuiAttribute(self, key: str, value: str) -> None:
         self._gui_attributes[key] = value
-        self._changed.append('gui_attributes')
+        self._changed.append("gui_attributes")
 
     def rmGuiAttribute(self, key: str) -> None:
         if self._gui_attributes.get(key) is not None:
             del self._gui_attributes[key]
-            self._changed.append('gui_attributes')
+            self._changed.append("gui_attributes")
 
     @property
     def label(self) -> LangString:
         return self._label
 
     @label.setter
     def label(self, value: Optional[Union[LangString, str]]) -> None:
@@ -175,24 +177,24 @@
             self._label.empty()  # clear all labels
         else:
             if isinstance(value, LangString):
                 self._label = value
             elif isinstance(value, str):
                 self._label = LangString(value)
             else:
-                raise BaseError('Not a valid LangString')
-        self._changed.add('label')
+                raise BaseError("Not a valid LangString")
+        self._changed.add("label")
 
     def addLabel(self, lang: Union[Languages, str], value: str) -> None:
         self._label[lang] = value
-        self._changed.add('label')
+        self._changed.add("label")
 
     def rmLabel(self, lang: Union[Languages, str]) -> None:
         del self._label[lang]
-        self._changed.add('label')
+        self._changed.add("label")
 
     @property
     def comment(self) -> LangString:
         return self._comment
 
     @comment.setter
     def comment(self, value: Optional[LangString]) -> None:
@@ -200,24 +202,24 @@
             self._comment.empty()  # clear all comments!
         else:
             if isinstance(value, LangString):
                 self._comment = value
             elif isinstance(value, str):
                 self._comment = LangString(value)
             else:
-                raise BaseError('Not a valid LangString')
-        self._changed.add('comment')
+                raise BaseError("Not a valid LangString")
+        self._changed.add("comment")
 
     def addComment(self, lang: Union[Languages, str], value: str) -> None:
         self._comment[lang] = value
-        self._changed.add('comment')
+        self._changed.add("comment")
 
     def rmComment(self, lang: Union[Languages, str]) -> None:
         del self._comment[lang]
-        self._changed.add('comment')
+        self._changed.add("comment")
 
     @property
     def editable(self) -> bool:
         return self._editable
 
     @editable.setter
     def editable(self, value: bool) -> None:
@@ -242,86 +244,89 @@
         rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
         rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
         owl = context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
         xsd = context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
         knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
         salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
 
-        if not (json_obj.get(knora_api + ':isResourceProperty')):
+        if not (json_obj.get(knora_api + ":isResourceProperty")):
             raise BaseError("This is not a property!")
-        if json_obj.get('@id') is None:
+        if json_obj.get("@id") is None:
             raise BaseError('Property class has no "@id"!')
-        tmp_id = json_obj.get('@id').split(':')
-        id = context.iri_from_prefix(tmp_id[0]) + '#' + tmp_id[1]
+        tmp_id = json_obj.get("@id").split(":")
+        id = context.iri_from_prefix(tmp_id[0]) + "#" + tmp_id[1]
         ontology_id = tmp_id[0]
         name = tmp_id[1]
-        superproperties_obj = json_obj.get(rdfs + ':subPropertyOf')
+        superproperties_obj = json_obj.get(rdfs + ":subPropertyOf")
         superproperties: list[Union[None, str]]
         if not isinstance(superproperties_obj, list):
             superproperties_obj = [superproperties_obj]  # make a list out of it
         if superproperties_obj:
-            superproperties = [x['@id'] for x in superproperties_obj if x and x.get('@id')]
+            superproperties = [x["@id"] for x in superproperties_obj if x and x.get("@id")]
         else:
             superproperties = None
-        object = WithId(json_obj.get(knora_api + ':objectType')).str()
-        subject = WithId(json_obj.get(knora_api + ':subjectType')).str()
-        label = LangString.fromJsonLdObj(json_obj.get(rdfs + ':label'))
-        comment = LangString.fromJsonLdObj(json_obj.get(rdfs + ':comment'))
+        object = WithId(json_obj.get(knora_api + ":objectType")).str()
+        subject = WithId(json_obj.get(knora_api + ":subjectType")).str()
+        label = LangString.fromJsonLdObj(json_obj.get(rdfs + ":label"))
+        comment = LangString.fromJsonLdObj(json_obj.get(rdfs + ":comment"))
         gui_element = None
-        if json_obj.get(salsah_gui + ':guiElement') is not None:
-            gui_element = WithId(json_obj.get(salsah_gui + ':guiElement')).str()
+        if json_obj.get(salsah_gui + ":guiElement") is not None:
+            gui_element = WithId(json_obj.get(salsah_gui + ":guiElement")).str()
             gui_element = gui_element.replace("Pulldown", "List")
             gui_element = gui_element.replace("Radio", "List")
-        gui_attributes_list = json_obj.get(salsah_gui + ':guiAttribute')
+        gui_attributes_list = json_obj.get(salsah_gui + ":guiAttribute")
         gui_attributes: Union[None, dict[str, str]] = None
         if gui_attributes_list is not None:
             gui_attributes = {}
             if not isinstance(gui_attributes_list, list):
                 gui_attributes_list = [gui_attributes_list]
             for ga in gui_attributes_list:
-                tmp = ga.split('=')
+                tmp = ga.split("=")
                 if len(tmp) == 1:
-                    gui_attributes[tmp[0]] = ''
+                    gui_attributes[tmp[0]] = ""
                 else:
                     gui_attributes[tmp[0]] = tmp[1]
 
-        editable = json_obj.get(knora_api + ':isEditable')
-        linkvalue = json_obj.get(knora_api + ':isLinkProperty')
-        return cls(con=con,
-                   context=context,
-                   id=id,
-                   name=name,
-                   ontology_id=ontology_id,
-                   superproperties=superproperties,
-                   object=object,
-                   subject=subject,
-                   gui_element=gui_element,
-                   gui_attributes=gui_attributes,
-                   label=label,
-                   comment=comment,
-                   editable=editable,
-                   linkvalue=linkvalue)
+        editable = json_obj.get(knora_api + ":isEditable")
+        linkvalue = json_obj.get(knora_api + ":isLinkProperty")
+        return cls(
+            con=con,
+            context=context,
+            id=id,
+            name=name,
+            ontology_id=ontology_id,
+            superproperties=superproperties,
+            object=object,
+            subject=subject,
+            gui_element=gui_element,
+            gui_attributes=gui_attributes,
+            label=label,
+            comment=comment,
+            editable=editable,
+            linkvalue=linkvalue,
+        )
 
     def toJsonObj(self, lastModificationDate: DateTimeStamp, action: Actions, what: Optional[str] = None) -> Any:
-
         def resolve_propref(resref: str):
-            tmp = resref.split(':')
+            tmp = resref.split(":")
             if len(tmp) > 1:
                 if tmp[0]:
                     #                    return {"@id": resref}  # fully qualified name in the form "prefix:name"
-                    return {"@id": self._context.get_qualified_iri(
-                        resref)}  # fully qualified name in the form "prefix:name"
+                    return {
+                        "@id": self._context.get_qualified_iri(resref)
+                    }  # fully qualified name in the form "prefix:name"
                 else:
-                    return {"@id": self._context.prefix_from_iri(self._ontology_id) + ':' + tmp[
-                        1]}  # ":name" in current ontology
+                    return {
+                        "@id": self._context.prefix_from_iri(self._ontology_id) + ":" + tmp[1]
+                    }  # ":name" in current ontology
             else:
                 return {"@id": "knora-api:" + resref}  # no ":", must be from knora-api!
 
         tmp = {}
-        exp = re.compile('^http.*')  # It is already a fully IRI
+        exp = re.compile("^http.*")  # It is already a fully IRI
         if exp.match(self._ontology_id):
             propid = self._context.prefix_from_iri(self._ontology_id) + ":" + self._name
             ontid = self._ontology_id
         else:
             propid = self._ontology_id + ":" + self._name
             ontid = self._context.iri_from_prefix(self._ontology_id)
         if action == Actions.Create:
@@ -334,101 +339,102 @@
             else:
                 superproperties = list(map(resolve_propref, self._superproperties))
 
             tmp = {
                 "@id": ontid,  # self._ontology_id,
                 "@type": "owl:Ontology",
                 "knora-api:lastModificationDate": lastModificationDate.toJsonObj(),
-                "@graph": [{
-                    "@id": propid,
-                    "@type": "owl:ObjectProperty",
-                    "rdfs:label": self._label.toJsonLdObj(),
-                    "rdfs:subPropertyOf": superproperties
-                }],
-                "@context": self._context.toJsonObj()
+                "@graph": [
+                    {
+                        "@id": propid,
+                        "@type": "owl:ObjectProperty",
+                        "rdfs:label": self._label.toJsonLdObj(),
+                        "rdfs:subPropertyOf": superproperties,
+                    }
+                ],
+                "@context": self._context.toJsonObj(),
             }
             if self._comment:
-                tmp['@graph'][0]["rdfs:comment"] = self._comment.toJsonLdObj()
+                tmp["@graph"][0]["rdfs:comment"] = self._comment.toJsonLdObj()
             if self._subject:
-                tmp['@graph'][0]["knora-api:subjectType"] = resolve_propref(self._subject)
+                tmp["@graph"][0]["knora-api:subjectType"] = resolve_propref(self._subject)
             if self._object:
-                tmp['@graph'][0]["knora-api:objectType"] = resolve_propref(self._object)
+                tmp["@graph"][0]["knora-api:objectType"] = resolve_propref(self._object)
             if self._gui_element:
-                tmp['@graph'][0]["salsah-gui:guiElement"] = {
-                    "@id": self._gui_element
-                }
+                tmp["@graph"][0]["salsah-gui:guiElement"] = {"@id": self._gui_element}
             if self._gui_attributes:
-                ga = list(map(lambda x: x[0] + '=' + str(x[1]), self._gui_attributes.items()))
-                tmp['@graph'][0]["salsah-gui:guiAttribute"] = ga
+                ga = list(map(lambda x: x[0] + "=" + str(x[1]), self._gui_attributes.items()))
+                tmp["@graph"][0]["salsah-gui:guiAttribute"] = ga
         elif action == Actions.Update:
             tmp = {
                 "@id": ontid,  # self._ontology_id,
                 "@type": "owl:Ontology",
                 "knora-api:lastModificationDate": lastModificationDate.toJsonObj(),
-                "@graph": [{
-                    "@id": propid,
-                    "@type": "owl:ObjectProperty",
-                }],
+                "@graph": [
+                    {
+                        "@id": propid,
+                        "@type": "owl:ObjectProperty",
+                    }
+                ],
                 "@context": self._context.toJsonObj(),
             }
-            if what == 'label':
-                if not self._label.isEmpty() and 'label' in self._changed:
-                    tmp['@graph'][0]['rdfs:label'] = self._label.toJsonLdObj()
-            if what == 'comment':
-                if not self._comment.isEmpty() and 'comment' in self._changed:
-                    tmp['@graph'][0]['rdfs:comment'] = self._comment.toJsonLdObj()
+            if what == "label":
+                if not self._label.isEmpty() and "label" in self._changed:
+                    tmp["@graph"][0]["rdfs:label"] = self._label.toJsonLdObj()
+            if what == "comment":
+                if not self._comment.isEmpty() and "comment" in self._changed:
+                    tmp["@graph"][0]["rdfs:comment"] = self._comment.toJsonLdObj()
 
         return tmp
 
-    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'PropertyClass']:
+    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, "PropertyClass"]:
         jsonobj = self.toJsonObj(last_modification_date, Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=2)
         result = self._con.post(PropertyClass.ROUTE, jsondata)
-        last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
-        return last_modification_date, PropertyClass.fromJsonObj(self._con, self._context, result['@graph'])
+        last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
+        return last_modification_date, PropertyClass.fromJsonObj(self._con, self._context, result["@graph"])
 
-    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
+    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, "ResourceClass"]:
         #
-        # Note: Knora is able to change only one thing per call, either label or comment!
+        # Note: DSP is able to change only one thing per call, either label or comment!
         #
         result = None
         something_changed = False
-        if 'label' in self._changed:
-            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, 'label')
+        if "label" in self._changed:
+            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, "label")
             jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
             result = self._con.put(PropertyClass.ROUTE, jsondata)
-            last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
+            last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
             something_changed = True
-        if 'comment' in self._changed:
-            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, 'comment')
+        if "comment" in self._changed:
+            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, "comment")
             jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
             result = self._con.put(PropertyClass.ROUTE, jsondata)
-            last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
+            last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
             something_changed = True
         if something_changed:
-            return last_modification_date, PropertyClass.fromJsonObj(self._con, self._context, result['@graph'])
+            return last_modification_date, PropertyClass.fromJsonObj(self._con, self._context, result["@graph"])
         else:
             return last_modification_date, self
 
     def delete(self, last_modification_date: DateTimeStamp) -> DateTimeStamp:
-        result = self._con.delete(PropertyClass.ROUTE + '/' + quote_plus(self._id) + '?lastModificationDate=' + str(
-            last_modification_date))
-        return DateTimeStamp(result['knora-api:lastModificationDate'])
+        result = self._con.delete(
+            PropertyClass.ROUTE + "/" + quote_plus(self._id) + "?lastModificationDate=" + str(last_modification_date)
+        )
+        return DateTimeStamp(result["knora-api:lastModificationDate"])
 
     def createDefinitionFileObj(self, context: Context, shortname: str):
         """
         Create an object that can be used as input for `create_onto()` to create an ontology on a DSP server
 
         :param context: Context of the ontology
         :param shortname: Shortname of the ontology
         :return: Python object to be jsonfied
         """
-        property = {
-            "name": self.name
-        }
+        property = {"name": self.name}
         if self.object:
             property["name"] = self.name
         if self.superproperties:
             superprops = []
             for sc in self.superproperties:
                 superprops.append(context.reduce_iri(sc, shortname))
             property["super"] = superprops
@@ -440,24 +446,24 @@
             property["labels"] = self.label.createDefinitionFileObj()
         if not self.comment.isEmpty():
             property["comments"] = self.comment.createDefinitionFileObj()
         if self.gui_element:
             property["gui_element"] = context.reduce_iri(self.gui_element, shortname)
         if self.gui_attributes:
             gui_elements = {}
-            for (attname, attvalue) in self.gui_attributes.items():
+            for attname, attvalue in self.gui_attributes.items():
                 if attname == "size":
                     gui_elements[attname] = int(attvalue)
                 elif attname == "maxlength":
                     gui_elements[attname] = int(attvalue)
                 elif attname == "maxsize":
                     gui_elements[attname] = int(attvalue)
                 elif attname == "hlist":
                     iri = attvalue[1:-1]
-                    rootnode = ListNode(con=self._con, id=iri).read()
+                    rootnode = ListNode(con=self._con, iri=iri).read()
                     gui_elements[attname] = rootnode.name
                 elif attname == "numprops":
                     gui_elements[attname] = int(attvalue)
                 elif attname == "ncolors":
                     gui_elements[attname] = int(attvalue)
                 elif attname == "cols":
                     gui_elements[attname] = int(attvalue)
@@ -473,36 +479,36 @@
                     gui_elements[attname] = float(attvalue)
                 else:
                     gui_elements[attname] = str(attvalue)
             property["gui_attributes"] = gui_elements
         return property
 
     def print(self, offset: int = 0):
-        blank = ' '
-        print(f'{blank:>{offset}}Property Class Info')
-        print(f'{blank:>{offset + 2}}Name:            {self._name}')
-        print(f'{blank:>{offset + 2}}Ontology prefix: {self._ontology_id}')
-        print(f'{blank:>{offset + 2}}Superproperties:')
+        blank = " "
+        print(f"{blank:>{offset}}Property Class Info")
+        print(f"{blank:>{offset + 2}}Name:            {self._name}")
+        print(f"{blank:>{offset + 2}}Ontology prefix: {self._ontology_id}")
+        print(f"{blank:>{offset + 2}}Superproperties:")
         if self._superproperties is not None:
             for sc in self._superproperties:
-                print(f'{blank:>{offset + 4}}{sc}')
+                print(f"{blank:>{offset + 4}}{sc}")
         if self._label is not None:
-            print(f'{blank:>{offset + 2}}Labels:')
+            print(f"{blank:>{offset + 2}}Labels:")
             self._label.print(offset + 4)
         if self._subject is not None:
-            print(f'{blank:>{offset + 4}}Subject: {self._subject}')
+            print(f"{blank:>{offset + 4}}Subject: {self._subject}")
         if self._object is not None:
-            print(f'{blank:>{offset + 4}}Object: {self._object}')
+            print(f"{blank:>{offset + 4}}Object: {self._object}")
         if self._gui_element is not None:
-            print(f'{blank:>{offset + 4}}Guielement: {self._gui_element}')
+            print(f"{blank:>{offset + 4}}Guielement: {self._gui_element}")
         if self._gui_attributes is not None:
-            print(f'{blank:>{offset + 4}}Gui Attributes:')
+            print(f"{blank:>{offset + 4}}Gui Attributes:")
             if self._gui_attributes is not None:
-                for (attname, attvalue) in self._gui_attributes.items():
-                    print(f'{blank:>{offset + 6}}Attribute: {attname} Value: {attvalue}')
+                for attname, attvalue in self._gui_attributes.items():
+                    print(f"{blank:>{offset + 6}}Attribute: {attname} Value: {attvalue}")
         if self._comment is not None:
-            print(f'{blank:>{offset + 2}}Comments:')
+            print(f"{blank:>{offset + 2}}Comments:")
             self._comment.print(offset + 4)
         if self._editable is not None:
-            print(f'{blank:>{offset + 4}}Editable: {self._editable}')
+            print(f"{blank:>{offset + 4}}Editable: {self._editable}")
         if self._linkvalue is not None:
-            print(f'{blank:>{offset + 4}}Editable: {self._linkvalue}')
+            print(f"{blank:>{offset + 4}}Editable: {self._linkvalue}")
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/propertyelement.py` & `dsp_tools-2.3.3/src/dsp_tools/models/propertyelement.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         >>> make_text_prop(":testproperty", PropertyElement("first text", permissions="prop-restricted", encoding="xml"))
                 <text-prop name=":testproperty">
                     <text encoding="xml" permissions="prop-restricted">
                         first text
                     </text>
                 </text-prop>
     """
+
     value: Union[str, int, float, bool]
     permissions: str = "prop-default"
     comment: Optional[str] = None
     encoding: Optional[str] = None
 
     def __post_init__(self) -> None:
         if self.encoding not in ["utf8", "xml", None]:
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/resource.py` & `dsp_tools-2.3.3/src/dsp_tools/models/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 from dataclasses import dataclass
 from typing import Any, Optional, Type, Union
 from urllib.parse import quote_plus
 
 from dsp_tools.models.bitstream import Bitstream
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.helpers import (
-    Actions,
-    Cardinality,
-    Context,
-    DateTimeStamp,
-    OntoIri
-)
+from dsp_tools.models.helpers import Actions, Cardinality, Context, DateTimeStamp, OntoIri
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.model import Model
 from dsp_tools.models.ontology import Ontology
 from dsp_tools.models.permission import Permissions, PermissionValue
 from dsp_tools.models.project import Project
 from dsp_tools.models.resourceclass import HasProperty
 from dsp_tools.models.value import (
@@ -33,24 +27,24 @@
     KnoraStandoffXml,
     LinkValue,
     ListValue,
     TextValue,
     TimeValue,
     UriValue,
     Value,
-    fromJsonLdObj
+    fromJsonLdObj,
 )
 
 
 class KnoraStandoffXmlEncoder(json.JSONEncoder):
-    """Classes used as wrapper for knora standoff-XML"""
+    """Classes used as wrapper for DSP standoff-XML"""
 
     def default(self, obj) -> str:
         if isinstance(obj, KnoraStandoffXml):
-            return '<?xml version="1.0" encoding="UTF-8"?>\n<text>' + str(obj) + '</text>'
+            return '<?xml version="1.0" encoding="UTF-8"?>\n<text>' + str(obj) + "</text>"
         elif isinstance(obj, OntoIri):
             return obj.iri + "#" if obj.hashtag else ""
         elif isinstance(obj, DateTimeStamp):
             return str(obj)
         return json.JSONEncoder.default(self, obj)
 
 
@@ -66,70 +60,76 @@
     """
     Represents a resource instance
     """
 
     ROUTE: str = "/v2/resources"
 
     baseclasses_with_bitstream: set[str] = {
-        'StillImageRepresentation',
-        'AudioRepresentation',
-        'DocumentRepresentation',
-        'MovingImageRepresentation',
-        'ArchiveRepresentation',
-        'DDDRepresentation',
-        'TextRepresentation'
+        "StillImageRepresentation",
+        "AudioRepresentation",
+        "DocumentRepresentation",
+        "MovingImageRepresentation",
+        "ArchiveRepresentation",
+        "DDDRepresentation",
+        "TextRepresentation",
     }
     knora_properties: set[str] = {
         "knora-api:hasLinkTo",
         "knora-api:hasColor",
         "knora-api:hasComment",
         "knora-api:hasGeometry",
         "knora-api:isPartOf",
         "knora-api:isRegionOf",
         "knora-api:isAnnotationOf",
         "knora-api:seqnum",
         "knora-api:isSequenceOf",
-        "knora-api:hasSequenceBounds"
+        "knora-api:hasSequenceBounds",
     }
     _iri: Optional[str]
     _ark: Optional[str]
     _version_ark: Optional[str]
     _creation_date: Optional[DateTimeStamp]
     _label: Optional[str]
     _permissions: Optional[Permissions]
     _user_permission: Optional[PermissionValue]
     _bitstream: Optional[Bitstream]
     _values: Optional[dict[Value, list[Value]]]
 
-    def __init__(self,
-                 con: Connection,
-                 iri: Optional[str] = None,
-                 ark: Optional[str] = None,
-                 version_ark: Optional[str] = None,
-                 creation_date: Optional[DateTimeStamp] = None,
-                 label: Optional[str] = None,
-                 permissions: Optional[Permissions] = None,
-                 user_permission: Optional[PermissionValue] = None,
-                 bitstream: Optional[str] = None,
-                 values: Optional[dict[
-                     str, Union[str, list[str], dict[str, str], list[dict[str, str]], Value, list[Value]]]] = None):
-
+    def __init__(
+        self,
+        con: Connection,
+        iri: Optional[str] = None,
+        ark: Optional[str] = None,
+        version_ark: Optional[str] = None,
+        creation_date: Optional[DateTimeStamp] = None,
+        label: Optional[str] = None,
+        permissions: Optional[Permissions] = None,
+        user_permission: Optional[PermissionValue] = None,
+        bitstream: Optional[str] = None,
+        values: Optional[
+            dict[str, Union[str, list[str], dict[str, str], list[dict[str, str]], Value, list[Value]]]
+        ] = None,
+    ):
         super().__init__(con)
         self._iri = iri
         self._ark = ark
         self._version_ark = version_ark
         self._creation_date = creation_date
         self._label = label
         self._permissions = permissions
         self._user_permission = user_permission
 
         if self.baseclass in self.baseclasses_with_bitstream and bitstream is None:
-            raise BaseError(f"ERROR in resource with label '{self._label}': Baseclass '{self.baseclass}' requires a bitstream value")
+            raise BaseError(
+                f"ERROR in resource with label '{self._label}': Baseclass '{self.baseclass}' requires a bitstream value"
+            )
         if self.baseclass not in self.baseclasses_with_bitstream and bitstream:
-            raise BaseError(f"ERROR in resource with label '{self._label}': Baseclass '{self.baseclass}' does not allow a bitstream value")
+            raise BaseError(
+                f"ERROR in resource with label '{self._label}': Baseclass '{self.baseclass}' does not allow a bitstream value"
+            )
         if self.baseclass in self.baseclasses_with_bitstream and bitstream:
             self._bitstream = bitstream
         else:
             self._bitstream = None
 
         self._values = {}
         if values:
@@ -149,46 +149,48 @@
                                 )
 
                             if type(val) is Value:
                                 self._values[property_name].append(val)
 
                             elif type(val) is dict:
                                 if value_type is ListValue:
-                                    val['lists'] = self.lists
+                                    val["lists"] = self.lists
                                 self._values[property_name].append(value_type(**val))
 
                             else:
                                 if value_type is ListValue:
-                                    val = {'value': val, 'lists': self.lists}
+                                    val = {"value": val, "lists": self.lists}
                                 self._values[property_name].append(value_type(val))
                     # property has one value
                     else:
                         if type(value) is Value:
                             self._values[property_name] = value
 
                         elif type(value) is dict:
                             if value_type is ListValue:
-                                value['lists'] = self.lists
+                                value["lists"] = self.lists
                             self._values[property_name] = value_type(**value)
 
                         else:
                             if value_type is ListValue:
-                                value = {'value': value, 'lists': self.lists}
+                                value = {"value": value, "lists": self.lists}
                                 self._values[property_name] = value_type(**value)
                             else:
                                 self._values[property_name] = value_type(value)
                 else:
                     if cardinality == Cardinality.C_1 or cardinality == Cardinality.C_1_n:
                         raise BaseError(
                             f"ERROR in resource with label '{self._label}': The ontology requires at least one value for '{property_name}'"
                         )
 
             for property_name in values:
                 if property_name not in self.knora_properties and not self.properties.get(property_name):
-                    raise BaseError(f"ERROR in resource with label '{self._label}': Property '{property_name}' is not part of ontology")
+                    raise BaseError(
+                        f"ERROR in resource with label '{self._label}': Property '{property_name}' is not part of ontology"
+                    )
 
     def value(self, item) -> Optional[list[Value]]:
         if self._values.get(item):
             value = self._values[item]
 
             # value has multiple values
             if isinstance(value, list):
@@ -214,157 +216,158 @@
     def creation_date(self) -> Optional[DateTimeStamp]:
         return self._creation_date
 
     @property
     def vark(self) -> str:
         return self._version_ark
 
-    def clone(self) -> 'ResourceInstance':
+    def clone(self) -> "ResourceInstance":
         return deepcopy(self)
 
-    def fromJsonLdObj(self, con: Connection, jsonld_obj: Any) -> 'ResourceInstance':
+    def fromJsonLdObj(self, con: Connection, jsonld_obj: Any) -> "ResourceInstance":
         newinstance = self.clone()
-        newinstance._iri = jsonld_obj.get('@id')
-        resclass = jsonld_obj.get('@type')
-        context = Context(jsonld_obj.get('@context'))
+        newinstance._iri = jsonld_obj.get("@id")
+        resclass = jsonld_obj.get("@type")
+        context = Context(jsonld_obj.get("@context"))
         newinstance._label = jsonld_obj.get("rdfs:label")
         newinstance._ark = Value.get_typed_value("knora-api:arkUrl", jsonld_obj)
         newinstance._version_ark = Value.get_typed_value("knora-api:versionArkUrl", jsonld_obj)
         newinstance._permissions = Permissions.fromString(jsonld_obj.get("knora-api:hasPermissions"))
         newinstance._user_permission = PermissionValue[jsonld_obj.get("knora-api:userHasPermission", jsonld_obj)]
         creation_date = Value.get_typed_value("knora-api:creationDate", jsonld_obj)
         user = Value.get_typed_value("knora-api:attachedToUser", jsonld_obj)
         project = Value.get_typed_value("knora-api:attachedToProject", jsonld_obj)
         to_be_ignored = [
-            '@id', '@type', '@context', "rdfs:label", "knora-api:arkUrl", "knora-api:versionArkUrl",
-            "knora-api:creationDate", "knora-api:attachedToUser", "knora-api:attachedToProject",
-            "knora-api:hasPermissions", "knora-api:userHasPermission"
+            "@id",
+            "@type",
+            "@context",
+            "rdfs:label",
+            "knora-api:arkUrl",
+            "knora-api:versionArkUrl",
+            "knora-api:creationDate",
+            "knora-api:attachedToUser",
+            "knora-api:attachedToProject",
+            "knora-api:hasPermissions",
+            "knora-api:userHasPermission",
         ]
         if id is None:
             raise BaseError('Resource "id" is missing in JSON-LD from DSP-API')
-        type = jsonld_obj.get('@type')
+        type = jsonld_obj.get("@type")
         newinstance._values: dict[str, Union[Value, list[Value]]] = {}
         for key, obj in jsonld_obj.items():
             if key in to_be_ignored:
                 continue
             try:
                 if isinstance(obj, list):
                     newinstance._values[key] = []
                     for o in obj:
                         newinstance._values[key].append(fromJsonLdObj(o))
                 else:
                     newinstance._values[key] = fromJsonLdObj(obj)
             except KeyError as kerr:
-                raise BaseError("Invalid data in JSON-LD: \"{}\" has value class \"{}\"!".format(key, obj.get("@type")))
+                raise BaseError('Invalid data in JSON-LD: "{}" has value class "{}"!'.format(key, obj.get("@type")))
         return newinstance
 
     def toJsonLdObj(self, action: Actions) -> Any:
         tmp = {}
         if action == Actions.Create:
             # if a custom IRI is provided, use it
             if self._iri:
-                tmp['@id'] = self._iri
-            tmp['@type'] = self.classname
-            tmp["knora-api:attachedToProject"] = {
-                "@id": self.project
-            }
-            tmp['rdfs:label'] = self._label
+                tmp["@id"] = self._iri
+            tmp["@type"] = self.classname
+            tmp["knora-api:attachedToProject"] = {"@id": self.project}
+            tmp["rdfs:label"] = self._label
 
             if self._permissions:
                 tmp["knora-api:hasPermissions"] = self._permissions.toJsonLdObj()
 
             if self._bitstream:
-                bitstream_attributes = {
-                    "knora-api:fileValueHasFilename": self._bitstream["internal_file_name"]
-                }
+                bitstream_attributes = {"knora-api:fileValueHasFilename": self._bitstream["internal_file_name"]}
 
                 permissions = self._bitstream.get("permissions")
                 if permissions:
                     bitstream_attributes["knora-api:hasPermissions"] = permissions.toJsonLdObj()
 
-                if self.baseclass == 'StillImageRepresentation':
+                if self.baseclass == "StillImageRepresentation":
                     bitstream_attributes["@type"] = "knora-api:StillImageFileValue"
                     tmp["knora-api:hasStillImageFileValue"] = bitstream_attributes
-                elif self.baseclass == 'DocumentRepresentation':
+                elif self.baseclass == "DocumentRepresentation":
                     bitstream_attributes["@type"] = "knora-api:DocumentFileValue"
                     tmp["knora-api:hasDocumentFileValue"] = bitstream_attributes
-                elif self.baseclass == 'TextRepresentation':
+                elif self.baseclass == "TextRepresentation":
                     bitstream_attributes["@type"] = "knora-api:TextFileValue"
                     tmp["knora-api:hasTextFileValue"] = bitstream_attributes
-                elif self.baseclass == 'AudioRepresentation':
+                elif self.baseclass == "AudioRepresentation":
                     bitstream_attributes["@type"] = "knora-api:AudioFileValue"
                     tmp["knora-api:hasAudioFileValue"] = bitstream_attributes
-                elif self.baseclass == 'ArchiveRepresentation':
+                elif self.baseclass == "ArchiveRepresentation":
                     bitstream_attributes["@type"] = "knora-api:ArchiveFileValue"
                     tmp["knora-api:hasArchiveFileValue"] = bitstream_attributes
-                elif self.baseclass == 'MovingImageRepresentation':
+                elif self.baseclass == "MovingImageRepresentation":
                     bitstream_attributes["@type"] = "knora-api:MovingImageFileValue"
                     tmp["knora-api:hasMovingImageFileValue"] = bitstream_attributes
                 else:
                     raise BaseError(f"Baseclass '{self.baseclass}' not yet supported!")
 
             for property_name, value in self._values.items():
                 # if the property has several values
                 if type(value) is list:
                     if type(value[0]) is LinkValue:
-                        property_name += 'Value'
+                        property_name += "Value"
                     # append all values to that property
                     tmp[property_name] = []
                     for vt in value:
                         tmp[property_name].append(vt.toJsonLdObj(action))
                 # if property is a link
                 elif type(value) is LinkValue:
-                    property_name += 'Value'
+                    property_name += "Value"
                     tmp[property_name] = value.toJsonLdObj(action)
                 else:
                     tmp[property_name] = value.toJsonLdObj(action)
 
-            tmp['@context'] = self.context
+            tmp["@context"] = self.context
 
             if self._creation_date:
-                tmp['knora-api:creationDate'] = {
-                    '@type': 'xsd:dateTimeStamp',
-                    '@value': self._creation_date
-                }
+                tmp["knora-api:creationDate"] = {"@type": "xsd:dateTimeStamp", "@value": self._creation_date}
         return tmp
 
-    def create(self) -> 'ResourceInstance':
+    def create(self) -> "ResourceInstance":
         jsonobj = self.toJsonLdObj(Actions.Create)
-        jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '), cls=KnoraStandoffXmlEncoder)
+        jsondata = json.dumps(jsonobj, indent=4, separators=(",", ": "), cls=KnoraStandoffXmlEncoder)
         result = self._con.post(ResourceInstance.ROUTE, jsondata)
         newinstance = self.clone()
-        newinstance._iri = result['@id']
-        newinstance._ark = result['knora-api:arkUrl']['@value']
-        newinstance._version_ark = result['knora-api:versionArkUrl']['@value']
+        newinstance._iri = result["@id"]
+        newinstance._ark = result["knora-api:arkUrl"]["@value"]
+        newinstance._version_ark = result["knora-api:versionArkUrl"]["@value"]
         return newinstance
 
-    def read(self) -> 'ResourceInstance':
-        result = self._con.get(ResourceInstance.ROUTE + '/' + quote_plus(self._iri))
+    def read(self) -> "ResourceInstance":
+        result = self._con.get(ResourceInstance.ROUTE + "/" + quote_plus(self._iri))
         return self.fromJsonLdObj(con=self._con, jsonld_obj=result)
 
     def update(self):
         pass
 
     def delete(self):
         pass
 
     def print(self):
-        print('IRI:', self._iri)
-        print('ARK:', self._ark)
-        print('Version ARK:', self._version_ark)
-        print('Label:', self._label)
-        print('Permissions:', str(self._permissions))
-        print('User permission:', str(self._user_permission))
+        print("IRI:", self._iri)
+        print("ARK:", self._ark)
+        print("Version ARK:", self._version_ark)
+        print("Label:", self._label)
+        print("Permissions:", str(self._permissions))
+        print("User permission:", str(self._user_permission))
         for name, val in self._values.items():
             if isinstance(val, list):
                 tmp = [str(x) for x in val]
-                print(name, ':', " | ".join(tmp))
+                print(name, ":", " | ".join(tmp))
                 pass
             else:
-                print(name, ':', str(val))
+                print(name, ":", str(val))
 
 
 class ResourceInstanceFactory:
     _con: Connection
     _project: Project
     _lists = list[ListNode]
     _ontologies = dict[str, Ontology]
@@ -387,26 +390,26 @@
 
         tmp_ontologies = Ontology.getProjectOntologies(con=con, project_id=self._project.id)
         shared_project = Project(con=con, shortcode="0000").read()
         shared_ontologies = Ontology.getProjectOntologies(con=con, project_id=shared_project.id)
         tmp_ontologies.extend(shared_ontologies)
         knora_api_onto = [x for x in Ontology.getAllOntologies(con=con) if x.name == "knora-api"][0]
         tmp_ontologies.append(knora_api_onto)
-        self._ontoname2iri = {x.name: x.id for x in tmp_ontologies}
+        self._ontoname2iri = {x.name: x.iri for x in tmp_ontologies}
 
-        ontology_ids = [x.id for x in tmp_ontologies]
+        ontology_ids = [x.iri for x in tmp_ontologies]
         self._ontologies = {}
         self._properties = {}
         self._context = {}
         for onto in ontology_ids:
             oparts = onto.split("/")
             name = oparts[len(oparts) - 2]
             shortcode = oparts[len(oparts) - 3]
             self._ontologies[name] = Ontology.getOntologyFromServer(con=con, shortcode=shortcode, name=name)
-            self._properties.update({name + ':' + x.name: x for x in self._ontologies[name].property_classes})
+            self._properties.update({name + ":" + x.name: x for x in self._ontologies[name].property_classes})
             self._context.update(self._ontologies[name].context)
 
     @property
     def lists(self) -> list[ListNode]:
         return self._lists
 
     def get_resclass_names(self) -> list[str]:
@@ -414,90 +417,103 @@
         for name, onto in self._ontologies.items():
             for resclass in onto.resource_classes:
                 resclass_names.append(onto.context.get_prefixed_iri(resclass.id))
         return resclass_names
 
     def _get_baseclass(self, superclasses: list[str]) -> Union[str, None]:
         for sc in superclasses:
-            ontoname, classname = sc.split(':')
-            if ontoname == 'knora-api':
+            ontoname, classname = sc.split(":")
+            if ontoname == "knora-api":
                 return classname
             o = self._ontologies.get(ontoname)
             if o is None:
                 continue
             gaga = [x for x in o.resource_classes if x.name == classname][0]
             return self._get_baseclass(gaga.superclasses)
         return None
 
     def get_resclass_type(self, prefixedresclass: str) -> Type:
-        prefix, resclass_name = prefixedresclass.split(':')
+        prefix, resclass_name = prefixedresclass.split(":")
         resclass = [x for x in self._ontologies[prefix].resource_classes if x.name == resclass_name][0]
         baseclass = self._get_baseclass(resclass.superclasses)
         props: dict[str, Propinfo] = {}
         switcher = {
-            'knora-api:TextValue': TextValue,
-            'knora-api:ColorValue': ColorValue,
-            'knora-api:DateValue': DateValue,
-            'knora-api:DecimalValue': DecimalValue,
-            'knora-api:GeomValue': GeomValue,
-            'knora-api:GeonameValue': GeonameValue,
-            'knora-api:IntValue': IntValue,
-            'knora-api:BooleanValue': BooleanValue,
-            'knora-api:UriValue': UriValue,
-            'knora-api:TimeValue': TimeValue,
-            'knora-api:IntervalValue': IntervalValue,
-            'knora-api:ListValue': ListValue,
-            'knora-api:LinkValue': LinkValue,
+            "knora-api:TextValue": TextValue,
+            "knora-api:ColorValue": ColorValue,
+            "knora-api:DateValue": DateValue,
+            "knora-api:DecimalValue": DecimalValue,
+            "knora-api:GeomValue": GeomValue,
+            "knora-api:GeonameValue": GeonameValue,
+            "knora-api:IntValue": IntValue,
+            "knora-api:BooleanValue": BooleanValue,
+            "knora-api:UriValue": UriValue,
+            "knora-api:TimeValue": TimeValue,
+            "knora-api:IntervalValue": IntervalValue,
+            "knora-api:ListValue": ListValue,
+            "knora-api:LinkValue": LinkValue,
         }
         for propname, has_property in resclass.has_properties.items():
-            if propname in ["knora-api:isAnnotationOf", "knora-api:isRegionOf", "knora-api:isPartOf",
-                            "knora-api:hasLinkTo", "knora-api:isSequenceOf"]:
+            if propname in [
+                "knora-api:isAnnotationOf",
+                "knora-api:isRegionOf",
+                "knora-api:isPartOf",
+                "knora-api:hasLinkTo",
+                "knora-api:isSequenceOf",
+            ]:
                 valtype = LinkValue
-                props[propname] = Propinfo(valtype=valtype,
-                                           cardinality=has_property.cardinality,
-                                           gui_order=has_property.gui_order)
+                props[propname] = Propinfo(
+                    valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                )
 
             elif propname == "knora-api:hasGeometry":
                 valtype = GeomValue
-                props[propname] = Propinfo(valtype=valtype,
-                                           cardinality=has_property.cardinality,
-                                           gui_order=has_property.gui_order)
+                props[propname] = Propinfo(
+                    valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                )
             elif propname == "knora-api:hasColor":
                 valtype = ColorValue
-                props[propname] = Propinfo(valtype=valtype,
-                                           cardinality=has_property.cardinality,
-                                           gui_order=has_property.gui_order)
+                props[propname] = Propinfo(
+                    valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                )
             elif propname == "knora-api:seqnum":
                 valtype = IntValue
-                props[propname] = Propinfo(valtype=valtype,
-                                           cardinality=has_property.cardinality,
-                                           gui_order=has_property.gui_order)
+                props[propname] = Propinfo(
+                    valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                )
             elif propname == "knora-api:hasComment":
                 valtype = TextValue
-                props[propname] = Propinfo(valtype=valtype,
-                                           cardinality=has_property.cardinality,
-                                           gui_order=has_property.gui_order)
+                props[propname] = Propinfo(
+                    valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                )
             elif propname == "knora-api:hasSequenceBounds":
                 valtype = IntervalValue
-                props[propname] = Propinfo(valtype=valtype,
-                                           cardinality=has_property.cardinality,
-                                           gui_order=has_property.gui_order)
+                props[propname] = Propinfo(
+                    valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                )
             elif has_property.ptype == HasProperty.Ptype.other:
                 valtype = switcher.get(self._properties[propname].object)
                 if valtype == LinkValue:
                     continue  # we have the Link to the LinkValue which we do not use
                 if valtype is None:
                     valtype = LinkValue
-                    props[propname] = Propinfo(valtype=valtype,
-                                               cardinality=has_property.cardinality,
-                                               gui_order=has_property.gui_order,
-                                               attributes=self._properties[propname].object)
+                    props[propname] = Propinfo(
+                        valtype=valtype,
+                        cardinality=has_property.cardinality,
+                        gui_order=has_property.gui_order,
+                        attributes=self._properties[propname].object,
+                    )
                 else:
-                    props[propname] = Propinfo(valtype=valtype,
-                                               cardinality=has_property.cardinality,
-                                               gui_order=has_property.gui_order)
-        return type(resclass_name, (ResourceInstance,), {'project': self._project.id,
-                                                         'classname': prefixedresclass,
-                                                         'baseclass': baseclass,
-                                                         'context': self._context,
-                                                         'properties': props,
-                                                         'lists': self._lists})
+                    props[propname] = Propinfo(
+                        valtype=valtype, cardinality=has_property.cardinality, gui_order=has_property.gui_order
+                    )
+        return type(
+            resclass_name,
+            (ResourceInstance,),
+            {
+                "project": self._project.id,
+                "classname": prefixedresclass,
+                "baseclass": baseclass,
+                "context": self._context,
+                "properties": props,
+                "lists": self._lists,
+            },
+        )
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/resourceclass.py` & `dsp_tools-2.3.3/src/dsp_tools/models/resourceclass.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,24 @@
 import re
 from enum import Enum
 from typing import Any, Optional, Sequence, Union
 from urllib.parse import quote_plus
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.helpers import (
-    Actions,
-    Cardinality,
-    Context,
-    DateTimeStamp
-)
+from dsp_tools.models.helpers import Actions, Cardinality, Context, DateTimeStamp
 from dsp_tools.models.langstring import LangString, Languages
 from dsp_tools.models.model import Model
 from dsp_tools.models.set_encoder import SetEncoder
 
 """
 This model implements the handling of resource classes. It contains two classes that work closely together:
     * "HasProperty" deals with the association of Property-instances with the Resource-instances. This association
       is done using the "cardinality"-clause
-    * "ResourceClass" is the main class representing a knora resource class.
+    * "ResourceClass" is the main class representing a DSP resource class.
 """
 
 
 class HasProperty(Model):
     ROUTE: str = "/v2/ontologies/cardinalities"
 
     class Ptype(Enum):
@@ -37,24 +32,26 @@
     _property_id: str
     _resclass_id: str
     _cardinality: Cardinality
     _gui_order: int
     _is_inherited: bool
     _ptype: Ptype
 
-    def __init__(self,
-                 con: Connection,
-                 context: Context,
-                 ontology_id: Optional[str] = None,
-                 property_id: Optional[str] = None,
-                 resclass_id: Optional[str] = None,
-                 cardinality: Optional[Cardinality] = None,
-                 gui_order: Optional[int] = None,
-                 is_inherited: Optional[bool] = None,
-                 ptype: Optional[Ptype] = None):
+    def __init__(
+        self,
+        con: Connection,
+        context: Context,
+        ontology_id: Optional[str] = None,
+        property_id: Optional[str] = None,
+        resclass_id: Optional[str] = None,
+        cardinality: Optional[Cardinality] = None,
+        gui_order: Optional[int] = None,
+        is_inherited: Optional[bool] = None,
+        ptype: Optional[Ptype] = None,
+    ):
         super().__init__(con)
         if not isinstance(context, Context):
             raise BaseError('"context"-parameter must be an instance of Context')
         self._context = context
         if ontology_id is not None:
             self._ontology_id = context.iri_from_prefix(ontology_id)
         else:
@@ -97,226 +94,228 @@
     @property
     def cardinality(self) -> Optional[Cardinality]:
         return self._cardinality
 
     @cardinality.setter
     def cardinality(self, value: Optional[Cardinality]) -> None:
         self._cardinality = value
-        self._changed.add('cardinality')
+        self._changed.add("cardinality")
 
     @property
     def gui_order(self) -> Optional[int]:
         return self._gui_order
 
     @gui_order.setter
     def gui_order(self, value: int) -> None:
         self._gui_order = value
-        self._changed.add('gui_order')
+        self._changed.add("gui_order")
 
     @property
     def ptype(self) -> Ptype:
         return self._ptype
 
     @classmethod
-    def fromJsonObj(cls, con: Connection, context: Context, jsonld_obj: Any) -> tuple[str, 'HasProperty']:
+    def fromJsonObj(cls, con: Connection, context: Context, jsonld_obj: Any) -> tuple[str, "HasProperty"]:
         if not isinstance(con, Connection):
             raise BaseError('"con"-parameter must be an instance of Connection')
         if not isinstance(context, Context):
             raise BaseError('"context"-parameter must be an instance of Context')
 
         rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
         rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
         owl = context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
         xsd = context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
         knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
         salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
 
-        if jsonld_obj.get('@type') is None or jsonld_obj.get('@type') != owl + ":Restriction":
-            raise BaseError('Expected restriction type')
+        if jsonld_obj.get("@type") is None or jsonld_obj.get("@type") != owl + ":Restriction":
+            raise BaseError("Expected restriction type")
 
         #
         # let's get the inherited field...
         #
-        tmp = jsonld_obj.get(knora_api + ':isInherited')
+        tmp = jsonld_obj.get(knora_api + ":isInherited")
         is_inherited = tmp if tmp is not None else False
 
         #
         # let's get the cardinality
         #
         cardinality: Cardinality
-        if jsonld_obj.get(owl + ':cardinality') is not None:
+        if jsonld_obj.get(owl + ":cardinality") is not None:
             cardinality = Cardinality.C_1
-        elif jsonld_obj.get(owl + ':maxCardinality') is not None:
+        elif jsonld_obj.get(owl + ":maxCardinality") is not None:
             cardinality = Cardinality.C_0_1
-        elif jsonld_obj.get(owl + ':minCardinality') is not None:
-            if jsonld_obj.get(owl + ':minCardinality') == 0:
+        elif jsonld_obj.get(owl + ":minCardinality") is not None:
+            if jsonld_obj.get(owl + ":minCardinality") == 0:
                 cardinality = Cardinality.C_0_n
-            elif jsonld_obj.get(owl + ':minCardinality') == 1:
+            elif jsonld_obj.get(owl + ":minCardinality") == 1:
                 cardinality = Cardinality.C_1_n
             else:
-                raise BaseError('Problem with cardinality')
+                raise BaseError("Problem with cardinality")
         else:
-            raise BaseError('Problem with cardinality')
+            raise BaseError("Problem with cardinality")
 
         #
         # Now let's get the property IRI
         #
         property_id: str
         ptype: HasProperty.Ptype
         ontology_id: Optional[str] = None
-        if jsonld_obj.get(owl + ':onProperty') is None:
-            raise BaseError('No property IRI given')
-        p = jsonld_obj[owl + ':onProperty'].get('@id')
+        if jsonld_obj.get(owl + ":onProperty") is None:
+            raise BaseError("No property IRI given")
+        p = jsonld_obj[owl + ":onProperty"].get("@id")
         if p is None:
-            raise BaseError('No property IRI given')
-        pp = p.split(':')
+            raise BaseError("No property IRI given")
+        pp = p.split(":")
         if pp[0] == rdf or pp[0] == rdfs or pp[0] == owl:
             ptype = HasProperty.Ptype.system
         elif pp[0] == knora_api:
             ptype = HasProperty.Ptype.knora
         else:
             ptype = HasProperty.Ptype.other
             ontology_id = context.iri_from_prefix(pp[0])
         property_id = p
 
         gui_order: int = None
-        if jsonld_obj.get(salsah_gui + ':guiOrder') is not None:
-            gui_order = jsonld_obj[salsah_gui + ':guiOrder']
-        return property_id, cls(con=con,
-                                context=context,
-                                ontology_id=ontology_id,
-                                property_id=property_id,
-                                cardinality=cardinality,
-                                gui_order=gui_order,
-                                is_inherited=is_inherited,
-                                ptype=ptype)
+        if jsonld_obj.get(salsah_gui + ":guiOrder") is not None:
+            gui_order = jsonld_obj[salsah_gui + ":guiOrder"]
+        return property_id, cls(
+            con=con,
+            context=context,
+            ontology_id=ontology_id,
+            property_id=property_id,
+            cardinality=cardinality,
+            gui_order=gui_order,
+            is_inherited=is_inherited,
+            ptype=ptype,
+        )
 
     def toJsonObj(self, lastModificationDate: DateTimeStamp, action: Actions) -> Any:
         if self._cardinality is None:
             raise BaseError("There must be a cardinality given!")
         tmp = {}
         switcher = {
             Cardinality.C_1: ("owl:cardinality", 1),
             Cardinality.C_0_1: ("owl:maxCardinality", 1),
             Cardinality.C_0_n: ("owl:minCardinality", 0),
-            Cardinality.C_1_n: ("owl:minCardinality", 1)
+            Cardinality.C_1_n: ("owl:minCardinality", 1),
         }
         occurrence = switcher.get(self._cardinality)
         if action == Actions.Create:
             tmp = {
                 "@id": self._ontology_id,
                 "@type": "owl:Ontology",
                 "knora-api:lastModificationDate": lastModificationDate.toJsonObj(),
-                "@graph": [{
-                    "@id": self._resclass_id,
-                    "@type": "owl:Class",
-                    "rdfs:subClassOf": {
-                        "@type": "owl:Restriction",
-                        occurrence[0]: occurrence[1],
-                        "owl:onProperty": {
-                            "@id": self._property_id
-                        }
+                "@graph": [
+                    {
+                        "@id": self._resclass_id,
+                        "@type": "owl:Class",
+                        "rdfs:subClassOf": {
+                            "@type": "owl:Restriction",
+                            occurrence[0]: occurrence[1],
+                            "owl:onProperty": {"@id": self._property_id},
+                        },
                     }
-                }],
-                "@context": self._context.toJsonObj()
+                ],
+                "@context": self._context.toJsonObj(),
             }
             if self._gui_order is not None:
                 tmp["@graph"][0]["rdfs:subClassOf"]["salsah-gui:guiOrder"] = self._gui_order
         elif action == Actions.Update:
             tmp = {
                 "@id": self._ontology_id,
                 "@type": "owl:Ontology",
                 "knora-api:lastModificationDate": lastModificationDate.toJsonObj(),
-                "@graph": [{
-                    "@id": self._resclass_id,
-                    "@type": "owl:Class",
-                    "rdfs:subClassOf": {
-                        "@type": "owl:Restriction",
-                        occurrence[0]: occurrence[1],
-                        "owl:onProperty": {
-                            "@id": self._property_id
-                        }
+                "@graph": [
+                    {
+                        "@id": self._resclass_id,
+                        "@type": "owl:Class",
+                        "rdfs:subClassOf": {
+                            "@type": "owl:Restriction",
+                            occurrence[0]: occurrence[1],
+                            "owl:onProperty": {"@id": self._property_id},
+                        },
                     }
-                }],
-                "@context": self._context.toJsonObj()
+                ],
+                "@context": self._context.toJsonObj(),
             }
-            if self._gui_order is not None and 'gui_order' in self._changed:
+            if self._gui_order is not None and "gui_order" in self._changed:
                 tmp["@graph"][0]["rdfs:subClassOf"]["salsah-gui:guiOrder"] = self._gui_order
         return tmp
 
-    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
+    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, "ResourceClass"]:
         if self._ontology_id is None:
             raise BaseError("Ontology id required")
         if self._property_id is None:
             raise BaseError("Property id required")
         if self._cardinality is None:
             raise BaseError("Cardinality id required")
 
         jsonobj = self.toJsonObj(last_modification_date, Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=2)
         result = self._con.post(HasProperty.ROUTE, jsondata)
-        last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
-        return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result['@graph'])
+        last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
+        return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result["@graph"])
 
-    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
+    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, "ResourceClass"]:
         if self._ontology_id is None:
             raise BaseError("Ontology id required")
         if self._property_id is None:
             raise BaseError("Property id required")
         if self._cardinality is None:
             raise BaseError("Cardinality id required")
         jsonobj = self.toJsonObj(last_modification_date, Actions.Update)
         jsondata = json.dumps(jsonobj, indent=4, cls=SetEncoder)
         result = self._con.put(HasProperty.ROUTE, jsondata)
-        last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
+        last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
         # TODO: self._changed = str()
-        return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result['@graph'])
+        return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result["@graph"])
 
     def delete(self, last_modification_date: DateTimeStamp) -> DateTimeStamp:
         raise BaseError("Cannot remove a single property from a class!")
         # ToDo: Check with Ben if we could add this feature...
 
     def createDefinitionFileObj(self, context: Context, shortname: str):
         cardinality = {}
         if self._ptype == HasProperty.Ptype.other or self.property_id in [
             "knora-api:isSequenceOf",
             "knora-api:hasSequenceBounds",
             "knora-api:isPartOf",
-            "knora-api:seqnum"
+            "knora-api:seqnum",
         ]:
             cardinality["propname"] = context.reduce_iri(self._property_id, shortname)
             cardinality["cardinality"] = self._cardinality.value
             if self._gui_order is not None:
                 cardinality["gui_order"] = self._gui_order
         return cardinality
 
     def print(self, offset: int = 0):
-        blank = ' '
+        blank = " "
         if self._ptype == HasProperty.Ptype.system:
-            print(f'{blank:>{offset}}Has Property (system)')
+            print(f"{blank:>{offset}}Has Property (system)")
         elif self._ptype == HasProperty.Ptype.knora:
-            print(f'{blank:>{offset}}Has Property (knora)')
+            print(f"{blank:>{offset}}Has Property (knora)")
         else:
-            print(f'{blank:>{offset}}Has Property (project)')
-        print(f'{blank:>{offset + 2}}Property: {self._property_id}')
-        print(f'{blank:>{offset + 2}}Cardinality: {self._cardinality.value}')
+            print(f"{blank:>{offset}}Has Property (project)")
+        print(f"{blank:>{offset + 2}}Property: {self._property_id}")
+        print(f"{blank:>{offset + 2}}Cardinality: {self._cardinality.value}")
         if self._ptype == HasProperty.Ptype.other:
-            print(f'{blank:>{offset + 2}}Ontology_id: {self._ontology_id}')
-        print(f'{blank:>{offset + 2}}Resclass: {self._resclass_id}')
+            print(f"{blank:>{offset + 2}}Ontology_id: {self._ontology_id}")
+        print(f"{blank:>{offset + 2}}Resclass: {self._resclass_id}")
 
 
 class ResourceClass(Model):
     """
-    This class represents a knora resource class
+    This class represents a DSP resource class
 
     Attributes
     ----------
 
     con : Connection
-        A Connection instance to a Knora server
+        A Connection instance to a DSP server
 
     id : str
         IRI of the ResourceClass [readonly, cannot be modified after creation of instance]
 
     name: str
         The name of the resource class, e.g. "Book", "Person", "Portait". Usually these names start
         with a capital letter
@@ -375,15 +374,15 @@
 
     create: Create a new resource class on the connected server
 
     update: Update the information of a resource class on the connected server
 
     delete: Mark a resource class as deleted (on the connected server)
 
-    createDefinitionFileObj: Create an object suitable for jsonification that conforms the the knora-py ontology tools
+    createDefinitionFileObj: Create an object suitable for jsonification that conforms the the DSP-TOOLS ontology tools
 
     print: Print the content of this class to the console
 
     """
 
     ROUTE: str = "/v2/ontologies/classes"
 
@@ -393,25 +392,27 @@
     _ontology_id: str
     _superclasses: list[str]
     _label: LangString
     _comment: LangString
     _permissions: str
     _has_properties: dict[str, HasProperty]
 
-    def __init__(self,
-                 con: Connection,
-                 context: Context,
-                 id: Optional[str] = None,
-                 name: Optional[str] = None,
-                 ontology_id: Optional[str] = None,
-                 superclasses: Optional[Sequence[Union['ResourceClass', str]]] = None,
-                 label: Optional[Union[LangString, str]] = None,
-                 comment: Optional[Union[LangString, str]] = None,
-                 permissions: Optional[str] = None,
-                 has_properties: Optional[dict[str, HasProperty]] = None):
+    def __init__(
+        self,
+        con: Connection,
+        context: Context,
+        id: Optional[str] = None,
+        name: Optional[str] = None,
+        ontology_id: Optional[str] = None,
+        superclasses: Optional[Sequence[Union["ResourceClass", str]]] = None,
+        label: Optional[Union[LangString, str]] = None,
+        comment: Optional[Union[LangString, str]] = None,
+        permissions: Optional[str] = None,
+        has_properties: Optional[dict[str, HasProperty]] = None,
+    ):
         """
         Create an instance of  ResourceClass
 
         :param con:
         :param context:
         :param id:
         :param name:
@@ -441,27 +442,27 @@
         #
         if label is not None:
             if isinstance(label, str):
                 self._label = LangString(label)
             elif isinstance(label, LangString):
                 self._label = label
             else:
-                raise BaseError('Invalid LangString for label!')
+                raise BaseError("Invalid LangString for label!")
         else:
             self._label = LangString({})
         #
         # process comment
         #
         if comment is not None:
             if isinstance(comment, str):
                 self._comment = LangString(comment)
             elif isinstance(comment, LangString):
                 self._comment = comment
             else:
-                raise BaseError('Invalid LangString for comment!')
+                raise BaseError("Invalid LangString for comment!")
         else:
             self._comment = LangString({})
         self._permissions = permissions
         self._has_properties = has_properties
         self._changed = set()
 
     #
@@ -509,24 +510,24 @@
             self._label.empty()  # clear all labels
         else:
             if isinstance(value, LangString):
                 self._label = value
             elif isinstance(value, str):
                 self._label = LangString(value)
             else:
-                raise BaseError('Not a valid LangString')
-        self._changed.add('label')
+                raise BaseError("Not a valid LangString")
+        self._changed.add("label")
 
     def addLabel(self, lang: Union[Languages, str], value: str) -> None:
         self._label[lang] = value
-        self._changed.add('label')
+        self._changed.add("label")
 
     def rmLabel(self, lang: Union[Languages, str]) -> None:
         del self._label[lang]
-        self._changed.add('label')
+        self._changed.add("label")
 
     @property
     def comment(self) -> LangString:
         return self._comment
 
     @comment.setter
     def comment(self, value: Optional[LangString]) -> None:
@@ -534,24 +535,24 @@
             self._comment.empty()  # clear all comments!
         else:
             if isinstance(value, LangString):
                 self._comment = value
             elif isinstance(value, str):
                 self._comment = LangString(value)
             else:
-                raise BaseError('Not a valid LangString')
-        self._changed.add('comment')
+                raise BaseError("Not a valid LangString")
+        self._changed.add("comment")
 
     def addComment(self, lang: Union[Languages, str], value: str) -> None:
         self._comment[lang] = value
-        self._changed.add('comment')
+        self._changed.add("comment")
 
     def rmComment(self, lang: Union[Languages, str]) -> None:
         del self._comment[lang]
-        self._changed.add('comment')
+        self._changed.add("comment")
 
     @property
     def permissions(self) -> Optional[str]:
         return self._permissions
 
     @permissions.setter
     def permissions(self, value: str) -> None:
@@ -567,42 +568,46 @@
 
     def getProperty(self, property_id) -> Optional[HasProperty]:
         if self._has_properties is None:
             return None
         else:
             return self._has_properties.get(self._context.get_prefixed_iri(property_id))
 
-    def addProperty(self,
-                    last_modification_date: DateTimeStamp,
-                    property_id: str,
-                    cardinality: Cardinality,
-                    gui_order: Optional[int] = None,
-                    ) -> DateTimeStamp:
+    def addProperty(
+        self,
+        last_modification_date: DateTimeStamp,
+        property_id: str,
+        cardinality: Cardinality,
+        gui_order: Optional[int] = None,
+    ) -> DateTimeStamp:
         if self._has_properties.get(property_id) is None:
-            latest_modification_date, resclass = HasProperty(con=self._con,
-                                                             context=self._context,
-                                                             ontology_id=self._ontology_id,
-                                                             property_id=property_id,
-                                                             resclass_id=self.id,
-                                                             cardinality=cardinality,
-                                                             gui_order=gui_order).create(last_modification_date)
+            latest_modification_date, resclass = HasProperty(
+                con=self._con,
+                context=self._context,
+                ontology_id=self._ontology_id,
+                property_id=property_id,
+                resclass_id=self.id,
+                cardinality=cardinality,
+                gui_order=gui_order,
+            ).create(last_modification_date)
             hp = resclass.getProperty(property_id)
             hp._ontology_id = self._context.iri_from_prefix(self._ontology_id)
             hp._resclass_id = self._id
             self._has_properties[hp.property_id] = hp
             return latest_modification_date
         else:
             raise BaseError("Property already has cardinality in this class! " + property_id)
 
-    def updateProperty(self,
-                       last_modification_date: DateTimeStamp,
-                       property_id: str,
-                       cardinality: Optional[Cardinality],
-                       gui_order: Optional[int] = None,
-                       ) -> Optional[DateTimeStamp]:
+    def updateProperty(
+        self,
+        last_modification_date: DateTimeStamp,
+        property_id: str,
+        cardinality: Optional[Cardinality],
+        gui_order: Optional[int] = None,
+    ) -> Optional[DateTimeStamp]:
         property_id = self._context.get_prefixed_iri(property_id)
         if self._has_properties.get(property_id) is not None:
             has_properties = self._has_properties[property_id]
             # onto_id = has_properties.ontology_id  # save for later user
             # rescl_id = has_properties.resclass_id  # save for later user
             has_properties.ontology_id = self._ontology_id
             has_properties.resclass_id = self._id
@@ -630,28 +635,28 @@
         rdf = context.prefix_from_iri("http://www.w3.org/1999/02/22-rdf-syntax-ns#")
         rdfs = context.prefix_from_iri("http://www.w3.org/2000/01/rdf-schema#")
         owl = context.prefix_from_iri("http://www.w3.org/2002/07/owl#")
         xsd = context.prefix_from_iri("http://www.w3.org/2001/XMLSchema#")
         knora_api = context.prefix_from_iri("http://api.knora.org/ontology/knora-api/v2#")
         salsah_gui = context.prefix_from_iri("http://api.knora.org/ontology/salsah-gui/v2#")
 
-        if not (json_obj.get(knora_api + ':isResourceClass') or json_obj.get(knora_api + ':isStandoffClass')):
+        if not (json_obj.get(knora_api + ":isResourceClass") or json_obj.get(knora_api + ":isStandoffClass")):
             raise BaseError("This is not a resource!")
 
-        if json_obj.get('@id') is None:
+        if json_obj.get("@id") is None:
             raise BaseError('Resource class has no "@id"!')
-        tmp_id = json_obj.get('@id').split(':')
-        id = context.iri_from_prefix(tmp_id[0]) + '#' + tmp_id[1]
+        tmp_id = json_obj.get("@id").split(":")
+        id = context.iri_from_prefix(tmp_id[0]) + "#" + tmp_id[1]
         ontology_id = tmp_id[0]
         name = tmp_id[1]
-        superclasses_obj = json_obj.get(rdfs + ':subClassOf')
+        superclasses_obj = json_obj.get(rdfs + ":subClassOf")
         if superclasses_obj is not None:
-            supercls: list[Any] = list(filter(lambda a: a.get('@id') is not None, superclasses_obj))
-            superclasses: list[str] = list(map(lambda a: a['@id'], supercls))
-            has_props: list[Any] = list(filter(lambda a: a.get('@type') == (owl + ':Restriction'), superclasses_obj))
+            supercls: list[Any] = list(filter(lambda a: a.get("@id") is not None, superclasses_obj))
+            superclasses: list[str] = list(map(lambda a: a["@id"], supercls))
+            has_props: list[Any] = list(filter(lambda a: a.get("@type") == (owl + ":Restriction"), superclasses_obj))
             has_properties: dict[HasProperty] = dict(map(lambda a: HasProperty.fromJsonObj(con, context, a), has_props))
             #
             # now remove the ...Value stuff from resource pointers: A resource pointer is returned as 2 properties:
             # one a direct link, the other the pointer to a link value
             #
             tmp = dict(has_properties)
             for key in tmp.keys():
@@ -660,42 +665,44 @@
                     key = key.removesuffix("Value")
                     if key in has_properties:
                         del has_properties[key_with_value]
         else:
             superclasses = None
             has_properties = None
 
-        label = LangString.fromJsonLdObj(json_obj.get(rdfs + ':label'))
-        comment = LangString.fromJsonLdObj(json_obj.get(rdfs + ':comment'))
-        return cls(con=con,
-                   context=context,
-                   name=name,
-                   id=id,
-                   ontology_id=ontology_id,
-                   superclasses=superclasses,
-                   label=label,
-                   comment=comment,
-                   has_properties=has_properties)
+        label = LangString.fromJsonLdObj(json_obj.get(rdfs + ":label"))
+        comment = LangString.fromJsonLdObj(json_obj.get(rdfs + ":comment"))
+        return cls(
+            con=con,
+            context=context,
+            name=name,
+            id=id,
+            ontology_id=ontology_id,
+            superclasses=superclasses,
+            label=label,
+            comment=comment,
+            has_properties=has_properties,
+        )
 
     def toJsonObj(self, lastModificationDate: DateTimeStamp, action: Actions, what: Optional[str] = None) -> Any:
-
         def resolve_resref(resref: str):
-            tmp = resref.split(':')
+            tmp = resref.split(":")
             if len(tmp) > 1:
                 if tmp[0] and self._context.iri_from_prefix(tmp[0]) != self._ontology_id:
                     self._context.add_context(tmp[0])
                     return {"@id": resref}  # fully qualified name in the form "prefix:name"
                 else:
-                    return {"@id": self._context.prefix_from_iri(self._ontology_id) + ':' + tmp[
-                        1]}  # ":name" in current ontology
+                    return {
+                        "@id": self._context.prefix_from_iri(self._ontology_id) + ":" + tmp[1]
+                    }  # ":name" in current ontology
             else:
                 return {"@id": "knora-api:" + resref}  # no ":", must be from knora-api!
 
         tmp = {}
-        exp = re.compile('^http.*')  # It is already a fully IRI
+        exp = re.compile("^http.*")  # It is already a fully IRI
         if exp.match(self._ontology_id):
             resid = self._context.prefix_from_iri(self._ontology_id) + ":" + self._name
             ontid = self._ontology_id
         else:
             resid = self._ontology_id + ":" + self._name
             ontid = self._context.iri_from_prefix(self._ontology_id)
         if action == Actions.Create:
@@ -709,78 +716,83 @@
                 superclasses = list(map(resolve_resref, self._superclasses))
             if self._label is None or self._label.isEmpty():
                 self._label = LangString("no label available")
             tmp = {
                 "@id": ontid,  # self._ontology_id,
                 "@type": "owl:Ontology",
                 "knora-api:lastModificationDate": lastModificationDate.toJsonObj(),
-                "@graph": [{
-                    "@id": resid,
-                    "@type": "owl:Class",
-                    "rdfs:label": self._label.toJsonLdObj(),
-                    "rdfs:subClassOf": superclasses
-                }],
+                "@graph": [
+                    {
+                        "@id": resid,
+                        "@type": "owl:Class",
+                        "rdfs:label": self._label.toJsonLdObj(),
+                        "rdfs:subClassOf": superclasses,
+                    }
+                ],
                 "@context": self._context.toJsonObj(),
             }
             if self._comment:
                 tmp["@graph"][0]["rdfs:comment"] = self._comment.toJsonLdObj()
 
         elif action == Actions.Update:
             tmp = {
                 "@id": ontid,  # self._ontology_id,
                 "@type": "owl:Ontology",
                 "knora-api:lastModificationDate": lastModificationDate.toJsonObj(),
-                "@graph": [{
-                    "@id": resid,
-                    "@type": "owl:Class",
-                }],
+                "@graph": [
+                    {
+                        "@id": resid,
+                        "@type": "owl:Class",
+                    }
+                ],
                 "@context": self._context.toJsonObj(),
             }
-            if what == 'label':
-                if not self._label.isEmpty() and 'label' in self._changed:
-                    tmp['@graph'][0]['rdfs:label'] = self._label.toJsonLdObj()
-            if what == 'comment':
-                if not self._comment.isEmpty() and 'comment' in self._changed:
-                    tmp['@graph'][0]['rdfs:comment'] = self._comment.toJsonLdObj()
+            if what == "label":
+                if not self._label.isEmpty() and "label" in self._changed:
+                    tmp["@graph"][0]["rdfs:label"] = self._label.toJsonLdObj()
+            if what == "comment":
+                if not self._comment.isEmpty() and "comment" in self._changed:
+                    tmp["@graph"][0]["rdfs:comment"] = self._comment.toJsonLdObj()
         return tmp
 
-    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
+    def create(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, "ResourceClass"]:
         jsonobj = self.toJsonObj(last_modification_date, Actions.Create)
         jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
         result = self._con.post(ResourceClass.ROUTE, jsondata)
-        last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
-        return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result['@graph'])
+        last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
+        return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result["@graph"])
 
-    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, 'ResourceClass']:
+    def update(self, last_modification_date: DateTimeStamp) -> tuple[DateTimeStamp, "ResourceClass"]:
         #
-        # Note: Knora is able to change only one thing per call, either label or comment!
+        # Note: DSP is able to change only one thing per call, either label or comment!
         #
         result = None
         something_changed = False
-        if 'label' in self._changed:
-            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, 'label')
+        if "label" in self._changed:
+            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, "label")
             jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
             result = self._con.put(ResourceClass.ROUTE, jsondata)
-            last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
+            last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
             something_changed = True
-        if 'comment' in self._changed:
-            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, 'comment')
+        if "comment" in self._changed:
+            jsonobj = self.toJsonObj(last_modification_date, Actions.Update, "comment")
             jsondata = json.dumps(jsonobj, cls=SetEncoder, indent=4)
             result = self._con.put(ResourceClass.ROUTE, jsondata)
-            last_modification_date = DateTimeStamp(result['knora-api:lastModificationDate'])
+            last_modification_date = DateTimeStamp(result["knora-api:lastModificationDate"])
             something_changed = True
         if something_changed:
-            return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result['@graph'])
+            return last_modification_date, ResourceClass.fromJsonObj(self._con, self._context, result["@graph"])
         else:
             return last_modification_date, self
 
     def delete(self, last_modification_date: DateTimeStamp) -> DateTimeStamp:
         result = self._con.delete(
-            ResourceClass.ROUTE + '/' + quote_plus(self._id) + '?lastModificationDate=' + str(last_modification_date))
-        return DateTimeStamp(result['knora-api:lastModificationDate'])
+            ResourceClass.ROUTE + "/" + quote_plus(self._id) + "?lastModificationDate=" + str(last_modification_date)
+        )
+        return DateTimeStamp(result["knora-api:lastModificationDate"])
 
     def createDefinitionFileObj(self, context: Context, shortname: str, skiplist: list[str]):
         resource = {"name": self._name}
         if self._superclasses:
             if len(self._superclasses) > 1:
                 superclasses = []
                 for sc in self._superclasses:
@@ -796,35 +808,35 @@
             for pid, hp in self._has_properties.items():
                 if hp.property_id in skiplist:
                     continue
                 if hp.ptype == HasProperty.Ptype.other or hp.property_id in [
                     "knora-api:isSequenceOf",
                     "knora-api:hasSequenceBounds",
                     "knora-api:isPartOf",
-                    "knora-api:seqnum"
+                    "knora-api:seqnum",
                 ]:
                     cardinalities.append(hp.createDefinitionFileObj(context, shortname))
             if cardinalities:
                 resource["cardinalities"] = cardinalities
 
         return resource
 
     def print(self, offset: int = 0):
-        blank = ' '
-        print(f'{blank:>{offset}}Resource Class Info')
-        print(f'{blank:>{offset + 2}}Name:            {self._name}')
-        print(f'{blank:>{offset + 2}}Ontology prefix: {self._ontology_id}')
-        print(f'{blank:>{offset + 2}}Superclasses:')
+        blank = " "
+        print(f"{blank:>{offset}}Resource Class Info")
+        print(f"{blank:>{offset + 2}}Name:            {self._name}")
+        print(f"{blank:>{offset + 2}}Ontology prefix: {self._ontology_id}")
+        print(f"{blank:>{offset + 2}}Superclasses:")
         if self._superclasses is not None:
             for sc in self._superclasses:
-                print(f'{blank:>{offset + 4}}{sc}')
+                print(f"{blank:>{offset + 4}}{sc}")
         if self._label is not None:
-            print(f'{blank:>{offset + 2}}Labels:')
+            print(f"{blank:>{offset + 2}}Labels:")
             self._label.print(offset + 4)
         if self._comment is not None:
-            print(f'{blank:>{offset + 2}}Comments:')
+            print(f"{blank:>{offset + 2}}Comments:")
             self._comment.print(offset + 4)
         if self._has_properties is not None:
-            print(f'{blank:>{offset + 2}}Has properties:')
+            print(f"{blank:>{offset + 2}}Has properties:")
             if self._has_properties is not None:
                 for pid, hp in self._has_properties.items():
                     hp.print(offset + 4)
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/sipi.py` & `dsp_tools-2.3.3/src/dsp_tools/models/sipi.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,13 +19,15 @@
 
         Args:
             filepath: path to the file, could be either absolute or relative
 
         Returns:
             API response
         """
-        with open(filepath, 'rb') as bitstream_file:
-            files = {'file': (os.path.basename(filepath), bitstream_file), }
+        with open(filepath, "rb") as bitstream_file:
+            files = {
+                "file": (os.path.basename(filepath), bitstream_file),
+            }
             response = requests.post(self.sipi_server + "/upload?token=" + self.token, files=files)
         check_for_api_error(response)
         res: dict[Any, Any] = response.json()
         return res
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/user.py` & `dsp_tools-2.3.3/src/dsp_tools/models/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 (head, tail) = os.path.split(path)
 if not head in sys.path:
     sys.path.insert(0, head)
 if not path in sys.path:
     sys.path.insert(0, path)
 
 """
-This module implements the handling (CRUD) of Knora users.
+This module implements the handling (CRUD) of DSP users.
 
 CREATE:
     * Instantiate a new object of the class User with all required parameters
     * Call the ``create``-method on the instance to create the new user
 
 READ:
     * Instantiate a new objects with ``id``(IRI of user) given
@@ -45,15 +45,15 @@
 
 In addition there is a static methods ``getAllProjects`` which returns a list of all projects
 """
 
 
 class User(Model):
     """
-    This class represents a user in Knora.
+    This class represents a user in DSP.
 
     Attributes
     ----------
 
     id : str
         IRI of the user [readonly, cannot be modified after creation of instance]
 
@@ -89,24 +89,24 @@
         Set of project IRI's the user belongs to
         Use ``addToproject``and ``rmFromproject`` to modify project membership
 
 
     Methods
     -------
 
-    create : Knora user information object
-        Creates a new user and returns the information about this user as it is in Knora
+    create : DSP user information object
+        Creates a new user and returns the information about this user as it is in DSP
 
-    read : Knora user information object
+    read : DSP user information object
         Read user data
 
-    update : Knora user information object
-        Updates the changed attributes of a user and returns the updated information  as it is in Knora
+    update : DSP user information object
+        Updates the changed attributes of a user and returns the updated information  as it is in DSP
 
-    delete : Knora result code
+    delete : DSP result code
         Deletes a user and returns the result code
 
     addToGroup : None
         Add the user to the given group (will be executed when calling ``update``)
 
     rmFromGroup : None
         Remove a user from a group (will be executed when calling ``update``)
@@ -151,31 +151,33 @@
     _in_projects: dict[str, bool]
     _add_to_project: dict[str, bool]
     _rm_from_project: dict[str, bool]
     _add_to_group: set[str]
     _rm_from_group: set[str]
     _change_admin: dict[str, bool]
 
-    def __init__(self,
-                 con: Connection,
-                 id: Optional[str] = None,
-                 username: Optional[str] = None,
-                 email: Optional[str] = None,
-                 givenName: Optional[str] = None,
-                 familyName: Optional[str] = None,
-                 password: Optional[str] = None,
-                 lang: Optional[Union[str, Languages]] = None,
-                 status: Optional[bool] = None,
-                 sysadmin: Optional[bool] = None,
-                 in_projects: Optional[dict[str, bool]] = None,
-                 in_groups: Optional[set[str]] = None):
+    def __init__(
+        self,
+        con: Connection,
+        id: Optional[str] = None,
+        username: Optional[str] = None,
+        email: Optional[str] = None,
+        givenName: Optional[str] = None,
+        familyName: Optional[str] = None,
+        password: Optional[str] = None,
+        lang: Optional[Union[str, Languages]] = None,
+        status: Optional[bool] = None,
+        sysadmin: Optional[bool] = None,
+        in_projects: Optional[dict[str, bool]] = None,
+        in_groups: Optional[set[str]] = None,
+    ):
         """
         Constructor for User
 
-        The constructor is user internally or externally, when a new user should be created in Knora.
+        The constructor is user internally or externally, when a new user should be created in DSP.
 
         :param con: Connection instance [required]
         :param id: IRI of the user [required for CREATE, READ]
         :param username: Username [required for CREATE]
         :param email: Email address [required for CREATE]
         :param givenName: Given name (firstname) of user [required for CREATE]
         :param familyName: Family name (lastname) of user [required for CREATE]
@@ -209,123 +211,123 @@
             self._in_projects = in_projects if in_projects is not None else {}
         else:
             raise BaseError("In_project must be tuple (project-iri: str, is-admin: bool)!")
 
         if in_groups is None or isinstance(in_groups, set):
             self._in_groups = in_groups if in_groups is not None else set()
         else:
-            raise BaseError('In_groups must be a set of strings or None!')
+            raise BaseError("In_groups must be a set of strings or None!")
 
         self._sysadmin = None if sysadmin is None else bool(sysadmin)
         self._add_to_project = {}
         self._rm_from_project = {}
         self._change_admin = {}
         self._add_to_group = set()
         self._rm_from_group = set()
 
     @property
     def id(self) -> Optional[str]:
         return self._id
 
     @id.setter
     def id(self, value: str) -> None:
-        raise BaseError('User id cannot be modified!')
+        raise BaseError("User id cannot be modified!")
 
     @property
     def username(self) -> Optional[str]:
         return self._username
 
     @username.setter
     def username(self, value: Optional[str]):
         if value is None:
             return
         self._username = str(value)
-        self._changed.add('username')
+        self._changed.add("username")
 
     @property
     def email(self) -> Optional[str]:
         return self._email
 
     @email.setter
     def email(self, value: Optional[str]):
         if value is None:
             return
         self._email = str(value)
-        self._changed.add('email')
+        self._changed.add("email")
 
     @property
     def givenName(self) -> Optional[str]:
         return self._givenName
 
     @givenName.setter
     def givenName(self, value: Optional[str]):
         if value is None:
             return
         self._givenName = str(value)
-        self._changed.add('givenName')
+        self._changed.add("givenName")
 
     @property
     def familyName(self) -> Optional[str]:
         return self._familyName
 
     @familyName.setter
     def familyName(self, value: Optional[str]):
         if value is None:
             return
         self._familyName = str(value)
-        self._changed.add('familyName')
+        self._changed.add("familyName")
 
     @property
     def password(self) -> Optional[str]:
         return None
 
     @password.setter
     def password(self, value: Optional[str]):
         if value is None:
             return
         self._password = str(value)
-        self._changed.add('password')
+        self._changed.add("password")
 
     @property
     def lang(self) -> Optional[Languages]:
         return self._lang
 
     @lang.setter
     def lang(self, value: Optional[Union[str, Languages]]):
         if value is None:
             return
         if isinstance(value, Languages):
             self._lang = value
-            self._changed.add('lang')
+            self._changed.add("lang")
         else:
             lmap = {a.value: a for a in Languages}
             if lmap.get(value) is None:
                 raise BaseError('Invalid language string "' + value + '"!')
             self._lang = lmap[value]
-            self._changed.add('lang')
+            self._changed.add("lang")
 
     @property
     def status(self) -> bool:
         return self._status
 
     @status.setter
     def status(self, value: Optional[bool]) -> None:
         self._status = None if value is None else bool(value)
         if value is not None:
-            self._changed.add('status')
+            self._changed.add("status")
 
     @property
     def sysadmin(self) -> bool:
         return self._sysadmin
 
     @sysadmin.setter
     def sysadmin(self, value: bool):
         self._sysadmin = None if value is None else bool(value)
         if value is not None:
-            self._changed.add('sysadmin')
+            self._changed.add("sysadmin")
 
     @property
     def in_groups(self) -> set[str]:
         return self._in_groups
 
     @in_groups.setter
     def in_groups(self, value: Any):
@@ -339,15 +341,15 @@
         :return: None
         """
 
         if value in self._rm_from_group:
             self._rm_from_group.pop(value)
         elif value not in self._in_groups:
             self._add_to_group.add(value)
-            self._changed.add('in_groups')
+            self._changed.add("in_groups")
         else:
             raise BaseError("Already member of this group!")
 
     def rmFromGroup(self, value: str):
         """
         Remove the user from the given group (executed at next update)
 
@@ -355,41 +357,42 @@
         :return: None
         """
 
         if value in self._add_to_group:
             self._add_to_group.discard(value)
         elif value in self._in_groups:
             self._rm_from_group.add(value)
-            self._changed.add('in_groups')
+            self._changed.add("in_groups")
         else:
             raise BaseError("User is not in groups!")
 
     @property
     def in_projects(self) -> dict[str, bool]:
         return self._in_projects
 
     @in_projects.setter
     def in_projects(self, value: Any):
         raise BaseError(
-            'Project membership cannot be modified directly! Use methods "addToProject" and "rmFromProject"')
+            'Project membership cannot be modified directly! Use methods "addToProject" and "rmFromProject"'
+        )
 
     def addToProject(self, value: str, padmin: bool = False):
         """
         Add the user to the given project (executed at next update)
 
         :param value: project IRI
         :param padmin: True, if user should be project admin, False otherwise
         :return: None
         """
 
         if value in self._rm_from_project:
             self._rm_from_project.pop(value)
         elif value not in self._in_projects:
             self._add_to_project[value] = padmin
-            self._changed.add('in_projects')
+            self._changed.add("in_projects")
         else:
             raise BaseError("Already member of this project!")
 
     def rmFromProject(self, value: str):
         """
         Remove the user from the given project (executed at next update)
 
@@ -397,44 +400,44 @@
         :return: None
         """
 
         if value in self._add_to_project:
             self._add_to_project.pop(value)
         elif value in self._in_projects:
             self._rm_from_project[value] = self._in_projects[value]
-            self._changed.add('in_projects')
+            self._changed.add("in_projects")
         else:
             raise BaseError("Project is not in list of member projects!")
 
     def makeProjectAdmin(self, value: str):
         """
         Make the user project administrator in the given project  (executed at next update)
 
         :param value: Project IRI
         :return: None
         """
 
         if value in self._in_projects:
             self._change_admin[value] = True
-            self._changed.add('in_projects')
+            self._changed.add("in_projects")
         elif value in self._add_to_project:
             self._add_to_project[value] = True
         else:
             raise BaseError("User is not member of project!")
 
     def unmakeProjectAdmin(self, value: str):
         """
         Revoke project administrator right for the user from the given project  (executed at next update)
 
         :param value: Project IRI
         :return: None
         """
         if value in self._in_projects:
             self._change_admin[value] = False
-            self._changed.add('in_projects')
+            self._changed.add("in_projects")
         elif value in self._add_to_project:
             self._add_to_project[value] = False
         else:
             raise BaseError("User is not member of project!")
 
     @property
     def changed(self) -> set[str]:
@@ -444,279 +447,278 @@
         return name in self._changed
 
     @classmethod
     def fromJsonObj(cls, con: Connection, json_obj: Any) -> User:
         """
         Internal method! Should not be used directly!
 
-        This method is used to create a User instance from the JSON data returned by Knora
+        This method is used to create a User instance from the JSON data returned by DSP
 
         :param con: Connection instance
-        :param json_obj: JSON data returned by Knora as python3 object
+        :param json_obj: JSON data returned by DSP as python3 object
         :return: User instance
         """
 
-        id = json_obj.get('id')
+        id = json_obj.get("id")
         if id is None:
-            raise BaseError('User "id" is missing in JSON from knora')
-        email = json_obj.get('email')
+            raise BaseError('User "id" is missing in JSON from DSP')
+        email = json_obj.get("email")
         if email is None:
-            raise BaseError('User "email" is missing in JSON from knora')
-        username = json_obj.get('username')
+            raise BaseError('User "email" is missing in JSON from DSP')
+        username = json_obj.get("username")
         if username is None:
-            raise BaseError('User "username" is missing in JSON from knora')
-        familyName = json_obj.get('familyName')
-        givenName = json_obj.get('givenName')
-        lang = json_obj.get('lang')
-        status = json_obj.get('status')
+            raise BaseError('User "username" is missing in JSON from DSP')
+        familyName = json_obj.get("familyName")
+        givenName = json_obj.get("givenName")
+        lang = json_obj.get("lang")
+        status = json_obj.get("status")
         if status is None:
-            raise BaseError("Status is missing in JSON from knora")
+            raise BaseError("Status is missing in JSON from DSP")
 
         in_projects: dict[str, bool] = {}
         in_groups: set[str] = set()
-        if json_obj.get('permissions') is not None and json_obj['permissions'].get('groupsPerProject') is not None:
+        if json_obj.get("permissions") is not None and json_obj["permissions"].get("groupsPerProject") is not None:
             sysadmin = False
-            for project_iri, group_memberships in json_obj['permissions']['groupsPerProject'].items():
+            for project_iri, group_memberships in json_obj["permissions"]["groupsPerProject"].items():
                 if project_iri == Project.SYSTEM_PROJECT:
                     if Group.PROJECT_SYSTEMADMIN_GROUP in group_memberships:
                         sysadmin = True
                 else:
                     for group in group_memberships:
                         if group == Group.PROJECT_MEMBER_GROUP:
                             if in_projects.get(project_iri) is None:
                                 in_projects[project_iri] = False
                         elif group == Group.PROJECT_ADMIN_GROUP:
                             in_projects[project_iri] = True
                         else:
                             in_groups.add(group)
-        return cls(con=con,
-                   id=id,
-                   username=username,
-                   email=email,
-                   givenName=givenName,
-                   familyName=familyName,
-                   lang=lang,
-                   status=status,
-                   sysadmin=sysadmin,
-                   in_projects=in_projects,
-                   in_groups=in_groups)
+        return cls(
+            con=con,
+            id=id,
+            username=username,
+            email=email,
+            givenName=givenName,
+            familyName=familyName,
+            lang=lang,
+            status=status,
+            sysadmin=sysadmin,
+            in_projects=in_projects,
+            in_groups=in_groups,
+        )
 
     def toJsonObj(self, action: Actions):
         """
         Internal method! Should not be used directly!
 
-        Creates a JSON-object from the Project instance that can be used to call Knora
+        Creates a JSON-object from the Project instance that can be used to call DSP
 
         :param action: Action the object is used for (Action.CREATE or Action.UPDATE)
         :return: JSON-object
         """
 
         tmp = {}
         if action == Actions.Create:
             if self._username is None:
                 raise BaseError("There must be a valid username!")
-            tmp['username'] = self._username
+            tmp["username"] = self._username
             if self._email is None:
                 raise BaseError("'email' is mandatory!")
-            tmp['email'] = self._email
+            tmp["email"] = self._email
             if self._givenName is None:
                 raise BaseError("'givenName is mandatory!")
-            tmp['givenName'] = self._givenName
+            tmp["givenName"] = self._givenName
             if self._familyName is None:
                 raise BaseError("'familyName' is mandatory!")
-            tmp['familyName'] = self._familyName
+            tmp["familyName"] = self._familyName
             if self._password is None:
                 raise BaseError("'password' is mandatory!")
-            tmp['password'] = self._password
+            tmp["password"] = self._password
             if self._lang is None:
                 raise BaseError("'language' is mandatory!")
-            tmp['lang'] = self._lang.value
-            tmp['status'] = True if self._status is None else self._status
-            tmp['systemAdmin'] = False if self._sysadmin is None else self._sysadmin
+            tmp["lang"] = self._lang.value
+            tmp["status"] = True if self._status is None else self._status
+            tmp["systemAdmin"] = False if self._sysadmin is None else self._sysadmin
         elif action == Actions.Update:
             tmp_changed = False
-            if self._username is not None and 'username' in self._changed:
-                tmp['username'] = self._username
+            if self._username is not None and "username" in self._changed:
+                tmp["username"] = self._username
                 tmp_changed = self._username
-            if self._email is not None and 'email' in self._changed:
-                tmp['email'] = self._email
+            if self._email is not None and "email" in self._changed:
+                tmp["email"] = self._email
                 tmp_changed = True
-            if self._givenName is not None and 'givenName' in self._changed:
-                tmp['givenName'] = self._givenName
+            if self._givenName is not None and "givenName" in self._changed:
+                tmp["givenName"] = self._givenName
                 tmp_changed = True
-            if self._familyName is not None and 'familyName' in self._changed:
-                tmp['familyName'] = self._familyName
+            if self._familyName is not None and "familyName" in self._changed:
+                tmp["familyName"] = self._familyName
                 tmp_changed = True
-            if self._lang is not None and 'lang' in self._changed:
-                tmp['lang'] = self._lang.value
+            if self._lang is not None and "lang" in self._changed:
+                tmp["lang"] = self._lang.value
                 tmp_changed = True
             if not tmp_changed:
                 tmp = {}
         return tmp
 
     def create(self) -> Any:
         """
-        Create new user in Knora
+        Create new user in DSP
 
-        :return: JSON-object from Knora
+        :return: JSON-object from DSP
         """
 
         jsonobj = self.toJsonObj(Actions.Create)
         jsondata = json.dumps(jsonobj)
         result = self._con.post(User.ROUTE, jsondata)
-        id = result['user']['id']
+        id = result["user"]["id"]
         if self._in_projects is not None:
             for project in self._in_projects:
-                result = self._con.post(
-                    User.IRI + quote_plus(id) + User.PROJECT_MEMBERSHIPS + quote_plus(project))
+                result = self._con.post(User.IRI + quote_plus(id) + User.PROJECT_MEMBERSHIPS + quote_plus(project))
                 if self._in_projects[project]:
                     result = self._con.post(
-                        User.IRI + quote_plus(id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(project))
+                        User.IRI + quote_plus(id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(project)
+                    )
         if self._in_groups is not None:
             for group in self._in_groups:
-                result = self._con.post(
-                    User.IRI + quote_plus(id) + User.GROUP_MEMBERSHIPS + quote_plus(group))
-        return User.fromJsonObj(self._con, result['user'])
+                result = self._con.post(User.IRI + quote_plus(id) + User.GROUP_MEMBERSHIPS + quote_plus(group))
+        return User.fromJsonObj(self._con, result["user"])
 
     def read(self) -> Any:
         """
-        Read the user information from Knora. The User object must have a valid id or email!
+        Read the user information from DSP. The User object must have a valid id or email!
 
-        :return: JSON-object from Knora
+        :return: JSON-object from DSP
         """
         if self._id is not None:
             result = self._con.get(User.IRI + quote_plus(self._id))
         elif self._email is not None:
-            result = self._con.get(User.ROUTE + '/email/' + quote_plus(self._email))
+            result = self._con.get(User.ROUTE + "/email/" + quote_plus(self._email))
         elif self._username is not None:
-            result = self._con.get(User.ROUTE + '/username/' + quote_plus(self._username))
+            result = self._con.get(User.ROUTE + "/username/" + quote_plus(self._username))
         else:
-            raise BaseError('Either user-id or email is required!')
-        return User.fromJsonObj(self._con, result['user'])
+            raise BaseError("Either user-id or email is required!")
+        return User.fromJsonObj(self._con, result["user"])
 
     def update(self, requesterPassword: Optional[str] = None) -> Any:
         """
-        Udate the user info in Knora with the modified data in this user instance
+        Udate the user info in DSP with the modified data in this user instance
 
         :param requesterPassword: Old password if a user wants to change it's own password
-        :return: JSON-object from Knora
+        :return: JSON-object from DSP
         """
 
         jsonobj = self.toJsonObj(Actions.Update)
         if jsonobj:
             jsondata = json.dumps(jsonobj)
-            result = self._con.put(User.IRI + quote_plus(self.id) + '/BasicUserInformation', jsondata)
-        if 'status' in self._changed:
-            jsonobj = {'status': self._status}
+            result = self._con.put(User.IRI + quote_plus(self.id) + "/BasicUserInformation", jsondata)
+        if "status" in self._changed:
+            jsonobj = {"status": self._status}
             jsondata = json.dumps(jsonobj)
-            result = self._con.put(User.IRI + quote_plus(self.id) + '/Status', jsondata)
-        if 'password' in self._changed:
+            result = self._con.put(User.IRI + quote_plus(self.id) + "/Status", jsondata)
+        if "password" in self._changed:
             if requesterPassword is None:
                 raise BaseError("Requester's password is missing!")
-            jsonobj = {
-                "requesterPassword": requesterPassword,
-                "newPassword": self._password
-            }
+            jsonobj = {"requesterPassword": requesterPassword, "newPassword": self._password}
             jsondata = json.dumps(jsonobj)
-            result = self._con.put(User.IRI + quote_plus(self.id) + '/Password', jsondata)
-        if 'sysadmin' in self._changed:
-            jsonobj = {'systemAdmin': self._sysadmin}
+            result = self._con.put(User.IRI + quote_plus(self.id) + "/Password", jsondata)
+        if "sysadmin" in self._changed:
+            jsonobj = {"systemAdmin": self._sysadmin}
             jsondata = json.dumps(jsonobj)
-            result = self._con.put(User.IRI + quote_plus(self.id) + '/SystemAdmin', jsondata)
+            result = self._con.put(User.IRI + quote_plus(self.id) + "/SystemAdmin", jsondata)
         for p in self._add_to_project.items():
-            result = self._con.post(
-                User.IRI + quote_plus(self._id) + User.PROJECT_MEMBERSHIPS + quote_plus(p[0]))
+            result = self._con.post(User.IRI + quote_plus(self._id) + User.PROJECT_MEMBERSHIPS + quote_plus(p[0]))
             if p[1]:
                 result = self._con.post(
-                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0]))
+                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0])
+                )
 
         for p in self._rm_from_project:
             if self._in_projects.get(p) is not None and self._in_projects[p]:
                 result = self._con.delete(
-                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p))
-            result = self._con.delete(
-                User.IRI + quote_plus(self._id) + User.PROJECT_MEMBERSHIPS + quote_plus(p))
+                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p)
+                )
+            result = self._con.delete(User.IRI + quote_plus(self._id) + User.PROJECT_MEMBERSHIPS + quote_plus(p))
 
         for p in self._change_admin.items():
             if not p[0] in self._in_projects:
-                raise BaseError('user must be member of project!')
+                raise BaseError("user must be member of project!")
             if p[1]:
                 result = self._con.post(
-                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0]))
+                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0])
+                )
             else:
                 result = self._con.delete(
-                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0]))
+                    User.IRI + quote_plus(self._id) + User.PROJECT_ADMIN_MEMBERSHIPS + quote_plus(p[0])
+                )
 
         for p in self._add_to_group:
             result = self._con.post(User.IRI + quote_plus(self._id) + User.GROUP_MEMBERSHIPS + quote_plus(p))
         for p in self._rm_from_group:
-            result = self._con.delete(
-                User.IRI + quote_plus(self._id) + User.GROUP_MEMBERSHIPS + quote_plus(p))
+            result = self._con.delete(User.IRI + quote_plus(self._id) + User.GROUP_MEMBERSHIPS + quote_plus(p))
         user = User(con=self._con, id=self._id).read()
         return user
 
     def delete(self):
         """
         Delete the user in nore (NOT YET IMPLEMENTED)
         :return: None
         """
         result = self._con.delete(User.IRI + quote_plus(self._id))
-        return User.fromJsonObj(self._con, result['user'])
+        return User.fromJsonObj(self._con, result["user"])
 
     @staticmethod
     def getAllUsers(con: Connection) -> list[Any]:
         """
         Get a list of all users (static method)
 
         :param con: Connection instance
         :return: List of users
         """
 
         result = con.get(User.ROUTE)
-        if 'users' not in result:
+        if "users" not in result:
             raise BaseError("Request got no users!")
-        return [User.fromJsonObj(con, a) for a in result['users']]
+        return [User.fromJsonObj(con, a) for a in result["users"]]
 
     @staticmethod
     def getAllUsersForProject(con: Connection, proj_shortcode: str) -> Optional[list[User]]:
         """
         Get a list of all users that belong to a project (static method)
 
         :param con: Connection instance
         :project_shortcode: Shortcode of the project
         :return: List of users belonging to that project
         """
-        members = con.get(f'/admin/projects/shortcode/{proj_shortcode}/members')
+        members = con.get(f"/admin/projects/shortcode/{proj_shortcode}/members")
         if members is None or len(members) < 1:
             return None
-        res: list[User] = [User.fromJsonObj(con, a) for a in members['members']]
+        res: list[User] = [User.fromJsonObj(con, a) for a in members["members"]]
         res.reverse()
         return res
 
     def createDefinitionFileObj(
         self,
         con: Connection,
         proj_shortname: str,
-        proj_iri: str
+        proj_iri: str,
     ) -> dict[str, Union[str, list[str], None]]:
         user: dict[str, Union[str, list[str], bool, None]] = {
             "username": self.username,
             "email": self.email,
             "givenName": self.givenName,
             "familyName": self.familyName,
             "password": "",
         }
         if self.lang:
             user["lang"] = self.lang.value
         groups = list()
         for group_iri in self._in_groups:
-            group_info = con.get(f'/admin/groups/{urllib.parse.quote_plus(group_iri)}')
-            if 'group' in group_info and 'name' in group_info['group']:
-                groupname = group_info['group']['name']
-                groups.append(f'{proj_shortname}:{groupname}')
+            group_info = con.get(f"/admin/groups/{urllib.parse.quote_plus(group_iri)}")
+            if "group" in group_info and "name" in group_info["group"]:
+                groupname = group_info["group"]["name"]
+                groups.append(f"{proj_shortname}:{groupname}")
         if self.sysadmin:
             groups.append("SystemAdmin")
         user["groups"] = groups
         user["projects"] = list()
         for proj, is_admin in self._in_projects.items():
             if proj == proj_iri:
                 if is_admin:
@@ -729,23 +731,23 @@
     def print(self) -> None:
         """
         Prin user info to stdout
 
         :return: None
         """
 
-        print('User info:')
-        print('  Id:          {}'.format(self._id))
-        print('  Username:    {}'.format(self._username))
-        print('  Family name: {}'.format(self._familyName))
-        print('  Given name:  {}'.format(self._givenName))
-        print('  Language:    {}'.format(self._lang.value))
-        print('  Status:      {}'.format(self._status))
-        print('  Sysadmin:    {}'.format(self._sysadmin))
-        print('  In projects:')
+        print("User info:")
+        print("  Id:          {}".format(self._id))
+        print("  Username:    {}".format(self._username))
+        print("  Family name: {}".format(self._familyName))
+        print("  Given name:  {}".format(self._givenName))
+        print("  Language:    {}".format(self._lang.value))
+        print("  Status:      {}".format(self._status))
+        print("  Sysadmin:    {}".format(self._sysadmin))
+        print("  In projects:")
         if self._in_projects is not None:
             for p in self._in_projects:
-                print('    {} : project admin: {}'.format(p, self._in_projects[p]))
-        print('   In groups:')
+                print("    {} : project admin: {}".format(p, self._in_projects[p]))
+        print("   In groups:")
         if self._in_groups is not None:
             for g in self._in_groups:
-                print('    {}'.format(g))
+                print("    {}".format(g))
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/value.py` & `dsp_tools-2.3.3/src/dsp_tools/models/value.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.permission import Permissions, PermissionValue
 
 
 class KnoraStandoffXml:
     """Used to handle XML strings for standoff markup"""
 
-    __iriregexp = re.compile(r'IRI:[^:]*:IRI')
+    __iriregexp = re.compile(r"IRI:[^:]*:IRI")
     __xmlstr: str
 
     def __init__(self, xmlstr: str) -> None:
         self.__xmlstr = str(xmlstr)
 
     def __str__(self) -> str:
         return self.__xmlstr
@@ -32,40 +32,43 @@
         self.__xmlstr = re.sub(pattern=repr(pattern)[1:-1], repl=repl, string=self.__xmlstr)
 
 
 class Value:
     """
     Represents a value
     """
+
     _iri: Optional[str]
     _comment: Optional[str]
     _permissions: Optional[Permissions]
     _upermission: Optional[PermissionValue]
     _ark_url: Optional[str]
     _vark_url: Optional[str]
 
-    def __init__(self,
-                 iri: Optional[str] = None,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        iri: Optional[str] = None,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         self._iri = iri
         self._comment = str(comment) if comment else None
         self._permissions = permissions
         self._upermission = upermission
         self._ark_url = ark_url
         self._vark_url = vark_url
 
     def __str__(self):
         if self._iri:
             tmpstr = "(iri: " + self._iri
         else:
-            tmpstr = ('(iri: -')
+            tmpstr = "(iri: -"
         if self._permissions:
             tmpstr = ", permissions: " + str(self._permissions)
         if self._comment:
             tmpstr += ", comment: " + self._comment
         tmpstr += ")"
         return tmpstr
 
@@ -115,237 +118,278 @@
             elif tmp.get("@type") == "xsd:anyURI":
                 result = str(tmp["@value"])
             elif tmp.get("@type") == "xsd:dateTimeStamp":
                 result = str(tmp["@value"])
             elif tmp.get("@id"):
                 result = tmp["@id"]
             else:
-                raise BaseError("Invalid data type in JSON-LD: \"{}\"!".format(tmp["@type"]))
+                raise BaseError('Invalid data type in JSON-LD: "{}"!'.format(tmp["@type"]))
             return result
         except KeyError as kerr:
             raise BaseError("Error in JSON-LD returned!") from kerr
 
     @staticmethod
     def getFromJsonLd(jsonld_obj) -> dict[str, Any]:
-
         return {
-            'iri': jsonld_obj.get("@id"),
-            'comment': jsonld_obj.get("knora-api:valueHasComment"),
-            'ark_url': Value.get_typed_value("knora-api:arkUrl", jsonld_obj),
-            'vark_url': Value.get_typed_value("knora-api:versionArkUrl", jsonld_obj),
-            'permissions': Permissions.fromString(jsonld_obj.get("knora-api:hasPermissions")),
-            'upermission': PermissionValue[jsonld_obj.get("knora-api:userHasPermission", jsonld_obj)]
+            "iri": jsonld_obj.get("@id"),
+            "comment": jsonld_obj.get("knora-api:valueHasComment"),
+            "ark_url": Value.get_typed_value("knora-api:arkUrl", jsonld_obj),
+            "vark_url": Value.get_typed_value("knora-api:versionArkUrl", jsonld_obj),
+            "permissions": Permissions.fromString(jsonld_obj.get("knora-api:hasPermissions")),
+            "upermission": PermissionValue[jsonld_obj.get("knora-api:userHasPermission", jsonld_obj)],
         }
 
 
 class TextValue(Value):
     _value: Union[str, KnoraStandoffXml]
     _mapping: str
 
-    def __init__(self,
-                 value: Union[str, KnoraStandoffXml],
-                 mapping: Optional[str] = None,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: Union[str, KnoraStandoffXml],
+        mapping: Optional[str] = None,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         self._value = value
         self._mapping = mapping
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @property
     def mapping(self) -> str:
         return self._mapping
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
 
         if jsonld_obj.get("knora-api:textValueAsXml") is not None:
-            tmp['mapping'] = jsonld_obj.get("knora-api:textValueHasMapping")
-            tmp['value'] = jsonld_obj.get("knora-api:textValueAsXml")
+            tmp["mapping"] = jsonld_obj.get("knora-api:textValueHasMapping")
+            tmp["value"] = jsonld_obj.get("knora-api:textValueAsXml")
         else:
-            tmp['mapping'] = None
-            tmp['value'] = jsonld_obj.get("knora-api:valueAsString")
+            tmp["mapping"] = None
+            tmp["value"] = jsonld_obj.get("knora-api:valueAsString")
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = 'knora-api:TextValue'
+            tmp["@type"] = "knora-api:TextValue"
             if isinstance(self._value, KnoraStandoffXml):
-                tmp['knora-api:textValueAsXml'] = self._value
-                tmp['knora-api:textValueHasMapping'] = {
-                    '@id': 'http://rdfh.ch/standoff/mappings/StandardMapping' if self._mapping is None else self._mapping
+                tmp["knora-api:textValueAsXml"] = self._value
+                tmp["knora-api:textValueHasMapping"] = {
+                    "@id": "http://rdfh.ch/standoff/mappings/StandardMapping"
+                    if self._mapping is None
+                    else self._mapping
                 }
             else:
-                tmp['knora-api:valueAsString'] = str(self._value)
+                tmp["knora-api:valueAsString"] = str(self._value)
         return tmp
 
     def __str__(self) -> str:
         return str(self._value)
 
 
 class ColorValue(Value):
     _value: str
 
-    def __init__(self,
-                 value: str,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: str,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         #
         # a color value as used in HTML (e.g. "#aaccff"
         #
-        m = re.match('^#(?:[0-9a-fA-F]{3}){1,2}$', str(value))
+        m = re.match("^#(?:[0-9a-fA-F]{3}){1,2}$", str(value))
         if not m:
             raise BaseError("Invalid ColorValue format! " + str(value))
         self._value = str(value)
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = jsonld_obj.get("knora-api:colorValueAsColor")
+        tmp["value"] = jsonld_obj.get("knora-api:colorValueAsColor")
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:ColorValue"
-            tmp['knora-api:colorValueAsColor'] = self._value
+            tmp["@type"] = "knora-api:ColorValue"
+            tmp["knora-api:colorValueAsColor"] = self._value
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 class DateValue(Value):
     _calendar: str
     _e1: str
     _y1: int
     _m1: int
     _d1: int
     _e2: str
     _y2: int
     _m2: int
     _d2: int
 
-    def __init__(self,
-                 value: str,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: str,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         #
-        # A knora date value
+        # A DSP date value
         #
         m = re.match(
             r"^(GREGORIAN:|JULIAN:)?(CE:|BCE:)?(\d{4})(-\d{1,2})?(-\d{1,2})?((:CE|:BCE)?(:\d{4})(-\d{1,2})?(-\d{1,2})?)?$",
-            str(value))
+            str(value),
+        )
         if not m:
-            raise BaseError("Invalid date format: \"{}\"!".format(str(value)))
+            raise BaseError('Invalid date format: "{}"!'.format(str(value)))
         dp = m.groups()
-        self._calendar = 'GREGORIAN' if dp[0] is None else dp[0].strip('-: ')
-        self._e1 = 'CE' if dp[1] is None else dp[1].strip('-: ')
-        self._y1 = None if dp[2] is None else int(dp[2].strip('-: '))
-        self._m1 = None if dp[3] is None else int(dp[3].strip('-: '))
-        self._d1 = None if dp[4] is None else int(dp[4].strip('-: '))
-        self._e2 = 'CE' if dp[6] is None else dp[6].strip('-: ')
-        self._y2 = None if dp[7] is None else int(dp[7].strip('-: '))
-        self._m2 = None if dp[8] is None else int(dp[8].strip('-: '))
-        self._d2 = None if dp[9] is None else int(dp[9].strip('-: '))
+        self._calendar = "GREGORIAN" if dp[0] is None else dp[0].strip("-: ")
+        self._e1 = "CE" if dp[1] is None else dp[1].strip("-: ")
+        self._y1 = None if dp[2] is None else int(dp[2].strip("-: "))
+        self._m1 = None if dp[3] is None else int(dp[3].strip("-: "))
+        self._d1 = None if dp[4] is None else int(dp[4].strip("-: "))
+        self._e2 = "CE" if dp[6] is None else dp[6].strip("-: ")
+        self._y2 = None if dp[7] is None else int(dp[7].strip("-: "))
+        self._m2 = None if dp[8] is None else int(dp[8].strip("-: "))
+        self._d2 = None if dp[9] is None else int(dp[9].strip("-: "))
         if self._y1 is None:
             raise BaseError("Invalid date format! " + str(value))
 
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
-        datestr = ''
+        datestr = ""
         if self._calendar:
-            datestr += self._calendar + ':'
+            datestr += self._calendar + ":"
         if self._e1:
-            datestr += self._e1 + ':'
+            datestr += self._e1 + ":"
         if self._y1:
-            datestr += str(self._y1) + '-'
+            datestr += str(self._y1) + "-"
         if self._m1:
-            datestr += str(self._m1) + '-'
+            datestr += str(self._m1) + "-"
         if self._d1:
             datestr += str(self._d1)
         if self._e2:
-            datestr += ':' + str(self._e2)
+            datestr += ":" + str(self._e2)
         if self._y2:
-            datestr += ':' + str(self._y2)
+            datestr += ":" + str(self._y2)
         if self._m2:
-            datestr += '-' + str(self._m2)
+            datestr += "-" + str(self._m2)
         if self._d2:
-            datestr += '-' + str(self._d2)
+            datestr += "-" + str(self._d2)
         return datestr
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
 
         datestr = ""
-        datestr += jsonld_obj.get("knora-api:dateValueHasCalendar") + ":" \
-            if jsonld_obj.get("knora-api:dateValueHasCalendar") is not None else ""
-        datestr += jsonld_obj.get("knora-api:dateValueHasStartEra") + ":" \
-            if jsonld_obj.get("knora-api:dateValueHasStartEra") is not None else ""
-        datestr += str(jsonld_obj.get("knora-api:dateValueHasStartYear")) \
-            if jsonld_obj.get("knora-api:dateValueHasStartYear") is not None else ""
-        datestr += "-" + str(jsonld_obj.get("knora-api:dateValueHasStartMonth")) \
-            if jsonld_obj.get("knora-api:dateValueHasStartMonth") is not None else ""
-        datestr += "-" + str(jsonld_obj.get("knora-api:dateValueHasStartDay")) \
-            if jsonld_obj.get("knora-api:dateValueHasStartDay") is not None else ""
-        datestr += ":" + jsonld_obj.get("knora-api:dateValueHasEndEra") \
-            if jsonld_obj.get("knora-api:dateValueHasEndEra") is not None else ""
-        datestr += ":" + str(jsonld_obj.get("knora-api:dateValueHasEndYear")) \
-            if jsonld_obj.get("knora-api:dateValueHasEndYear") is not None else ""
-        datestr += "-" + str(jsonld_obj.get("knora-api:dateValueHasEndMonth")) \
-            if jsonld_obj.get("knora-api:dateValueHasEndMonth") is not None else ""
-        datestr += "-" + str(jsonld_obj.get("knora-api:dateValueHasEndDay")) \
-            if jsonld_obj.get("knora-api:dateValueHasEndDay") is not None else ""
-        tmp['value'] = datestr
+        datestr += (
+            jsonld_obj.get("knora-api:dateValueHasCalendar") + ":"
+            if jsonld_obj.get("knora-api:dateValueHasCalendar") is not None
+            else ""
+        )
+        datestr += (
+            jsonld_obj.get("knora-api:dateValueHasStartEra") + ":"
+            if jsonld_obj.get("knora-api:dateValueHasStartEra") is not None
+            else ""
+        )
+        datestr += (
+            str(jsonld_obj.get("knora-api:dateValueHasStartYear"))
+            if jsonld_obj.get("knora-api:dateValueHasStartYear") is not None
+            else ""
+        )
+        datestr += (
+            "-" + str(jsonld_obj.get("knora-api:dateValueHasStartMonth"))
+            if jsonld_obj.get("knora-api:dateValueHasStartMonth") is not None
+            else ""
+        )
+        datestr += (
+            "-" + str(jsonld_obj.get("knora-api:dateValueHasStartDay"))
+            if jsonld_obj.get("knora-api:dateValueHasStartDay") is not None
+            else ""
+        )
+        datestr += (
+            ":" + jsonld_obj.get("knora-api:dateValueHasEndEra")
+            if jsonld_obj.get("knora-api:dateValueHasEndEra") is not None
+            else ""
+        )
+        datestr += (
+            ":" + str(jsonld_obj.get("knora-api:dateValueHasEndYear"))
+            if jsonld_obj.get("knora-api:dateValueHasEndYear") is not None
+            else ""
+        )
+        datestr += (
+            "-" + str(jsonld_obj.get("knora-api:dateValueHasEndMonth"))
+            if jsonld_obj.get("knora-api:dateValueHasEndMonth") is not None
+            else ""
+        )
+        datestr += (
+            "-" + str(jsonld_obj.get("knora-api:dateValueHasEndDay"))
+            if jsonld_obj.get("knora-api:dateValueHasEndDay") is not None
+            else ""
+        )
+        tmp["value"] = datestr
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:DateValue"
+            tmp["@type"] = "knora-api:DateValue"
             tmp["knora-api:dateValueHasCalendar"] = self._calendar
             tmp["knora-api:dateValueHasStartEra"] = self._e1
             tmp["knora-api:dateValueHasStartYear"] = self._y1
             if self._m1:
                 tmp["knora-api:dateValueHasStartMonth"] = self._m1
             if self._d1:
                 tmp["knora-api:dateValueHasStartDay"] = self._d1
@@ -357,551 +401,571 @@
             if self._m2:
                 tmp["knora-api:dateValueHasEndMonth"] = self._m2
             if self._d2:
                 tmp["knora-api:dateValueHasEndDay"] = self._d2
         return tmp
 
     def __str__(self):
-        datestr = ''
+        datestr = ""
         if self._calendar:
-            datestr += self._calendar + ':'
+            datestr += self._calendar + ":"
         if self._e1:
-            datestr += self._e1 + ':'
+            datestr += self._e1 + ":"
         if self._y1:
-            datestr += str(self._y1) + '-'
+            datestr += str(self._y1) + "-"
         if self._m1:
-            datestr += str(self._m1) + '-'
+            datestr += str(self._m1) + "-"
         if self._d1:
             datestr += str(self._d1)
         if self._e2:
-            datestr += ':' + str(self._e2)
+            datestr += ":" + str(self._e2)
         if self._y2:
-            datestr += ':' + str(self._y2)
+            datestr += ":" + str(self._y2)
         if self._m2:
-            datestr += '-' + str(self._m2)
+            datestr += "-" + str(self._m2)
         if self._d2:
-            datestr += '-' + str(self._d2)
-        return datestr + ' ' + super().__str__()
+            datestr += "-" + str(self._d2)
+        return datestr + " " + super().__str__()
 
 
 class DecimalValue(Value):
     _value: float
 
-    def __init__(self,
-                 value: Union[float, int, str],
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: Union[float, int, str],
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         self._value = value
         if isinstance(value, str):
-            m = re.match(r'^[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?$', value)
+            m = re.match(r"^[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?$", value)
             if m:
                 self._value = float(value)
             else:
-                raise BaseError("String does not represent decimal/float number! \"" + value + "\"")
+                raise BaseError('String does not represent decimal/float number! "' + value + '"')
         elif isinstance(value, float):
             self._value = value
         elif isinstance(value, int):
             self._value = float(value)
         else:
-            raise BaseError("String does not represent decimal/float number! \"" + value + "\"")
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+            raise BaseError('String does not represent decimal/float number! "' + value + '"')
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> float:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = Value.get_typed_value("knora-api:decimalValueAsDecimal", jsonld_obj)
+        tmp["value"] = Value.get_typed_value("knora-api:decimalValueAsDecimal", jsonld_obj)
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:DecimalValue"
-            tmp['knora-api:decimalValueAsDecimal'] = {
-                '@type': 'xsd:decimal',
-                '@value': str(self._value)
-            }
+            tmp["@type"] = "knora-api:DecimalValue"
+            tmp["knora-api:decimalValueAsDecimal"] = {"@type": "xsd:decimal", "@value": str(self._value)}
         return tmp
 
     def __str__(self) -> str:
-        return str(self._value) + ' ' + super().__str__()
+        return str(self._value) + " " + super().__str__()
 
 
 class GeomValue(Value):
     _value: str
 
-    def __init__(self,
-                 value: str,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: str,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         self._value = str(value)
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = jsonld_obj.get('knora-api:geometryValueAsGeometry')
+        tmp["value"] = jsonld_obj.get("knora-api:geometryValueAsGeometry")
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:GeomValue"
-            tmp['knora-api:geometryValueAsGeometry'] = self._value
+            tmp["@type"] = "knora-api:GeomValue"
+            tmp["knora-api:geometryValueAsGeometry"] = self._value
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 class GeonameValue(Value):
     _value: str
 
-    def __init__(self,
-                 value: str,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: str,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         self._value = str(value)
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = jsonld_obj.get('knora-api:geonameValueAsGeonameCode')
+        tmp["value"] = jsonld_obj.get("knora-api:geonameValueAsGeonameCode")
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:GeonameValue"
-            tmp['knora-api:geonameValueAsGeonameCode'] = self._value
+            tmp["@type"] = "knora-api:GeonameValue"
+            tmp["knora-api:geonameValueAsGeonameCode"] = self._value
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 class IntValue(Value):
     _value: int
 
-    def __init__(self,
-                 value: Union[int, str],
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: Union[int, str],
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         if isinstance(value, str):
-            m = re.match('^[-+]?[0-9]+$', value)
+            m = re.match("^[-+]?[0-9]+$", value)
             if m and m.span()[1] == len(str(value)):
                 self._value = int(value)
             else:
-                raise BaseError("String does not represent integer number! \"" + value + "\"")
+                raise BaseError('String does not represent integer number! "' + value + '"')
         elif isinstance(value, int):
             self._value = value
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> int:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = jsonld_obj.get("knora-api:intValueAsInt")
+        tmp["value"] = jsonld_obj.get("knora-api:intValueAsInt")
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:IntValue"
-            tmp['knora-api:intValueAsInt'] = self._value
+            tmp["@type"] = "knora-api:IntValue"
+            tmp["knora-api:intValueAsInt"] = self._value
         return tmp
 
     def __str__(self) -> str:
-        return str(self._value) + ' ' + super().__str__()
+        return str(self._value) + " " + super().__str__()
 
 
 class BooleanValue(Value):
     _value: bool
 
-    def __init__(self,
-                 value: Union[bool, int, str],
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
-
+    def __init__(
+        self,
+        value: Union[bool, int, str],
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         if type(value) is bool:
             self._value = value
         else:
-            if value == 1 or value.upper() == 'TRUE' or value == '1':
+            if value == 1 or value.upper() == "TRUE" or value == "1":
                 self._value = True
-            elif value == 0 or value.upper() == 'FALSE' or value == '0':
+            elif value == 0 or value.upper() == "FALSE" or value == "0":
                 self._value = False
             else:
                 raise BaseError(f"ERROR Invalid boolean format {value}!")
 
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> bool:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = jsonld_obj.get("knora-api:booleanValueAsBoolean")
+        tmp["value"] = jsonld_obj.get("knora-api:booleanValueAsBoolean")
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:BooleanValue"
-            tmp['knora-api:booleanValueAsBoolean'] = self._value
+            tmp["@type"] = "knora-api:BooleanValue"
+            tmp["knora-api:booleanValueAsBoolean"] = self._value
         return tmp
 
     def __str__(self) -> str:
-        return str(self._value) + ' ' + super().__str__()
+        return str(self._value) + " " + super().__str__()
 
 
 class UriValue(Value):
     _value: str
 
-    def __init__(self,
-                 value: str,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: str,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         # URI = scheme ":" ["//" host [":" port]] path ["?" query] ["#" fragment]
         scheme = r"(?<scheme>[a-z][a-z0-9+.\-]*)"
         host = r"(?<host>[\w_.\-~:\[\]]+)"
         port = r"(?<port>:\d{0,6})"
         path = r"(?<path>/[\w_.\-~:%()]*)"
         query = r"(?<query>\?[\w_.\-%=*&]+)"
         fragment = r"(?<fragment>#[\w_.\-~:/]*)"
-        m = regex.match(fr"{scheme}:(//{host}{port}?){path}*{query}*{fragment}?", str(value), flags=regex.UNICODE)
+        m = regex.match(rf"{scheme}:(//{host}{port}?){path}*{query}*{fragment}?", str(value), flags=regex.UNICODE)
         if m:
             self._value = str(value)
         else:
-            raise BaseError("Invalid IRI/URI! \"" + value + "\"")
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+            raise BaseError('Invalid IRI/URI! "' + value + '"')
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = Value.get_typed_value("knora-api:uriValueAsUri", jsonld_obj)
+        tmp["value"] = Value.get_typed_value("knora-api:uriValueAsUri", jsonld_obj)
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:UriValue"
-            tmp['knora-api:uriValueAsUri'] = {
-                "@type": "xsd:anyURI",
-                "@value": self._value
-            }
+            tmp["@type"] = "knora-api:UriValue"
+            tmp["knora-api:uriValueAsUri"] = {"@type": "xsd:anyURI", "@value": self._value}
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 class TimeValue(Value):
     _value: str
 
     @property
     def value(self) -> str:
         return self._value
 
-    def __init__(self,
-                 value: str,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
-        m = re.match(r"^\d{4}-[0-1]\d-[0-3]\dT[0-2]\d:[0-5]\d:[0-5]\d(.\d{1,12})?(Z|[+-][0-1]\d:[0-5]\d)$",
-                     str(value))
+    def __init__(
+        self,
+        value: str,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
+        m = re.match(r"^\d{4}-[0-1]\d-[0-3]\dT[0-2]\d:[0-5]\d:[0-5]\d(.\d{1,12})?(Z|[+-][0-1]\d:[0-5]\d)$", str(value))
         if m:
             self._value = str(value)
         else:
-            raise BaseError("Invalid time value! \"" + value + "\"")
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+            raise BaseError('Invalid time value! "' + value + '"')
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = Value.get_typed_value("knora-api:timeValueAsTimeStamp", jsonld_obj)
+        tmp["value"] = Value.get_typed_value("knora-api:timeValueAsTimeStamp", jsonld_obj)
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:TimeValue"
-            tmp['knora-api:timeValueAsTimeStamp'] = {
-                "@type": "xsd:dateTimeStamp",
-                "@value": self._value
-            }
+            tmp["@type"] = "knora-api:TimeValue"
+            tmp["knora-api:timeValueAsTimeStamp"] = {"@type": "xsd:dateTimeStamp", "@value": self._value}
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 class IntervalValue(Value):
     _iv_start: str
     _iv_end: str
 
-    def __init__(self,
-                 value: Optional[str] = None,
-                 iv_start: Optional[float] = None,
-                 iv_end: Optional[float] = None,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: Optional[str] = None,
+        iv_start: Optional[float] = None,
+        iv_end: Optional[float] = None,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         if value is not None:
-            startval, endval = value.split(':')
+            startval, endval = value.split(":")
             self._iv_start = float(startval)
             self._iv_end = float(endval)
         else:
             if iv_start is None or iv_end is None:
-                raise BaseError("\"value\" or \"iv_start\" and \"iv_end\" must be given to constructor!")
+                raise BaseError('"value" or "iv_start" and "iv_end" must be given to constructor!')
             self._iv_start = iv_start
             self._iv_end = iv_end
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
-        return str(self._iv_start) + ':' + str(self._iv_end)
+        return str(self._iv_start) + ":" + str(self._iv_end)
 
     @property
     def iv_start(self) -> float:
         return self._iv_start
 
     @property
     def iv_end(self) -> float:
         return self._iv_end
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
         start = Value.get_typed_value("knora-api:intervalValueHasStart", jsonld_obj)
         end = Value.get_typed_value("knora-api:intervalValueHasEnd", jsonld_obj)
-        tmp['value'] = str(start) + ":" + str(end)
+        tmp["value"] = str(start) + ":" + str(end)
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:IntervalValue"
-            tmp["knora-api:intervalValueHasStart"] = {
-                "@type": "xsd:decimal",
-                "@value": str(self._iv_start)
-            }
-            tmp["knora-api:intervalValueHasEnd"] = {
-                "@type": "xsd:decimal",
-                "@value": str(self._iv_end)
-            }
+            tmp["@type"] = "knora-api:IntervalValue"
+            tmp["knora-api:intervalValueHasStart"] = {"@type": "xsd:decimal", "@value": str(self._iv_start)}
+            tmp["knora-api:intervalValueHasEnd"] = {"@type": "xsd:decimal", "@value": str(self._iv_end)}
         return tmp
 
     def __str__(self) -> str:
-        interval = str(self._iv_start) + ':' + str(self._iv_end)
-        return interval + ' ' + super().__str__()
+        interval = str(self._iv_start) + ":" + str(self._iv_end)
+        return interval + " " + super().__str__()
 
 
 class ListValue(Value):
     _value: str
 
-    def __init__(self,
-                 value: str,
-                 lists: list[ListNode] = None,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
-
+    def __init__(
+        self,
+        value: str,
+        lists: list[ListNode] = None,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         def find_listnode(nodes: list[ListNode], name: str) -> Optional[str]:
             for node in nodes:
                 if node.name == name:
-                    return node.id
+                    return node.iri
                 else:
                     if node.children is not None:
                         node_id = find_listnode(node.children, name)
                         if node_id is not None:
                             return node_id
             return None
 
         if IriTest.test(str(value)):
             self._value = str(value)
         else:
-            tmp = str(value).split(':')
+            tmp = str(value).split(":")
             if len(tmp) > 1:
                 if tmp[0]:
                     listname = tmp[0]
                     nodename = tmp[1]
                 else:
-                    raise BaseError("Invalid list node: \"" + str(value) + "\" !")
+                    raise BaseError('Invalid list node: "' + str(value) + '" !')
             else:
-                raise BaseError("Invalid list node: \"" + str(value) + "\" !")
+                raise BaseError('Invalid list node: "' + str(value) + '" !')
             if lists is None:
                 raise BaseError("Lists from ResourceInstanceFactory must be provided!")
             node_iri = None
             for list_item in lists:
                 if list_item.name == listname:
                     node_iri = find_listnode(list_item.children, nodename)
             if node_iri is not None:
                 self._value = node_iri
             else:
-                raise BaseError("Listnode \"{}\" not found".format(value))
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+                raise BaseError('Listnode "{}" not found'.format(value))
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     def print(self, offset: int = 0):
-        blank = ' '
-        print(f'{blank:>{offset}}{self._value}')
+        blank = " "
+        print(f"{blank:>{offset}}{self._value}")
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
-        tmp['value'] = Value.get_typed_value("knora-api:listValueAsListNode", jsonld_obj)
+        tmp["value"] = Value.get_typed_value("knora-api:listValueAsListNode", jsonld_obj)
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:ListValue"
-            tmp['knora-api:listValueAsListNode'] = {
-                '@id': self._value
-            }
+            tmp["@type"] = "knora-api:ListValue"
+            tmp["knora-api:listValueAsListNode"] = {"@id": self._value}
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 class LinkValue(Value):
     _value: str
     _restype: str
     _reslabel: str
 
-    def __init__(self,
-                 value: str,
-                 restype: Optional[str] = None,
-                 reslabel: Optional[str] = None,
-                 comment: Optional[LangString] = None,
-                 permissions: Optional[Permissions] = None,
-                 upermission: Optional[PermissionValue] = None,
-                 iri: Optional[str] = None,
-                 ark_url: Optional[str] = None,
-                 vark_url: Optional[str] = None):
+    def __init__(
+        self,
+        value: str,
+        restype: Optional[str] = None,
+        reslabel: Optional[str] = None,
+        comment: Optional[LangString] = None,
+        permissions: Optional[Permissions] = None,
+        upermission: Optional[PermissionValue] = None,
+        iri: Optional[str] = None,
+        ark_url: Optional[str] = None,
+        vark_url: Optional[str] = None,
+    ):
         m = re.match("^(http)s?://([\\w\\.\\-~]+)?(:\\d{,6})?(/[\\w\\-~]+)*(#[\\w\\-~]*)?", str(value))
         if m:
             self._value = str(value)
         else:
-            raise BaseError("Target of link is not a IRI: \"" + str(value) + "\"")
+            raise BaseError('Target of link is not a IRI: "' + str(value) + '"')
         self._restype = restype
         self._reslabel = reslabel
-        super().__init__(iri=iri,
-                         comment=comment,
-                         permissions=permissions,
-                         upermission=upermission,
-                         ark_url=ark_url,
-                         vark_url=vark_url)
+        super().__init__(
+            iri=iri,
+            comment=comment,
+            permissions=permissions,
+            upermission=upermission,
+            ark_url=ark_url,
+            vark_url=vark_url,
+        )
 
     @property
     def value(self) -> str:
         return self._value
 
     @property
     def restype(self) -> str:
@@ -912,56 +976,52 @@
         return self._reslabel
 
     @classmethod
     def fromJsonLdObj(cls, jsonld_obj: Any) -> dict[str, Any]:
         tmp = Value.getFromJsonLd(jsonld_obj)
         linked_resource = jsonld_obj.get("knora-api:linkValueHasTarget")
         if linked_resource is not None:
-            tmp['value'] = linked_resource['@id']
-            tmp['restype'] = linked_resource["@type"]
-            tmp['reslabel'] = linked_resource["rdfs:label"]
+            tmp["value"] = linked_resource["@id"]
+            tmp["restype"] = linked_resource["@type"]
+            tmp["reslabel"] = linked_resource["rdfs:label"]
         return cls(**tmp)
 
     def toJsonLdObj(self, action: Actions) -> dict[str, Any]:
         tmp = super().toJsonLdObj(action)
         if action == Actions.Create:
-            tmp['@type'] = "knora-api:LinkValue"
-            tmp['knora-api:linkValueHasTargetIri'] = {
-                '@id': self._value
-            }
+            tmp["@type"] = "knora-api:LinkValue"
+            tmp["knora-api:linkValueHasTargetIri"] = {"@id": self._value}
         return tmp
 
     def __str__(self) -> str:
-        return self._value + ' ' + super().__str__()
+        return self._value + " " + super().__str__()
 
 
 def fromJsonLdObj(jsonld_obj: str) -> Value:
     switcher = {
-        'knora-api:TextValue': TextValue,
-        'knora-api:ColorValue': ColorValue,
-        'knora-api:DateValue': DateValue,
-        'knora-api:DecimalValue': DecimalValue,
-        'knora-api:GeomValue': GeomValue,
-        'knora-api:GeonameValue': GeonameValue,
-        'knora-api:IntValue': IntValue,
-        'knora-api:BooleanValue': BooleanValue,
-        'knora-api:UriValue': UriValue,
-        'knora-api:TimeValue': TimeValue,
-        'knora-api:IntervalValue': IntervalValue,
-        'knora-api:ListValue': ListValue,
-        'knora-api:LinkValue': LinkValue,
+        "knora-api:TextValue": TextValue,
+        "knora-api:ColorValue": ColorValue,
+        "knora-api:DateValue": DateValue,
+        "knora-api:DecimalValue": DecimalValue,
+        "knora-api:GeomValue": GeomValue,
+        "knora-api:GeonameValue": GeonameValue,
+        "knora-api:IntValue": IntValue,
+        "knora-api:BooleanValue": BooleanValue,
+        "knora-api:UriValue": UriValue,
+        "knora-api:TimeValue": TimeValue,
+        "knora-api:IntervalValue": IntervalValue,
+        "knora-api:ListValue": ListValue,
+        "knora-api:LinkValue": LinkValue,
     }
-    return switcher[jsonld_obj.get('@type')].fromJsonLdObj(jsonld_obj)
+    return switcher[jsonld_obj.get("@type")].fromJsonLdObj(jsonld_obj)
 
 
 def make_value(
-    value: Union[Value, str],
-    comment: Optional[str] = None,
-    permissions: Optional[Permissions] = None
+    value: Union[Value, str], comment: Optional[str] = None, permissions: Optional[Permissions] = None
 ) -> dict[str, Any]:
     res = {}
-    res['value'] = value
+    res["value"] = value
     if comment:
-        res['comment'] = comment
+        res["comment"] = comment
     if permissions:
-        res['permissions'] = permissions
+        res["permissions"] = permissions
     return res
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/xmlallow.py` & `dsp_tools-2.3.3/src/dsp_tools/models/xmlallow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from lxml import etree
 
 from dsp_tools.models.projectContext import ProjectContext
-from dsp_tools.models.xmlerror import XmlError
+from dsp_tools.models.exceptions import XmlError
 
 
 class XmlAllow:
     """Represents the allow element of the XML used for data import"""
 
     _group: str
     _permission: str
@@ -17,33 +17,33 @@
         Args:
             node: The DOM node to be processed (represents a single right in a permission set)
             project_context: Context for DOM node traversal
 
         Returns:
             None
         """
-        tmp = node.attrib['group'].split(':')
-        sysgroups = ['UnknownUser', 'KnownUser', 'ProjectMember', 'Creator', 'ProjectAdmin', 'SystemAdmin']
+        tmp = node.attrib["group"].split(":")
+        sysgroups = ["UnknownUser", "KnownUser", "ProjectMember", "Creator", "ProjectAdmin", "SystemAdmin"]
         if len(tmp) > 1:
             if tmp[0]:
-                if tmp[0] == 'knora-admin' and tmp[1] in sysgroups:
-                    self._group = node.attrib['group']
+                if tmp[0] == "knora-admin" and tmp[1] in sysgroups:
+                    self._group = node.attrib["group"]
                 else:
-                    self._group = project_context.group_map.get(node.attrib['group'])
+                    self._group = project_context.group_map.get(node.attrib["group"])
                     if self._group is None:
-                        raise XmlError("Group \"{}\" is not known: Cannot find project!".format(node.attrib['group']))
+                        raise XmlError('Group "{}" is not known: Cannot find project!'.format(node.attrib["group"]))
             else:
                 if project_context.project_name is None:
                     raise XmlError("Project shortcode has not been set in ProjectContext")
-                self._group = project_context.project_name + ':' + tmp[1]
+                self._group = project_context.project_name + ":" + tmp[1]
         else:
             if tmp[0] in sysgroups:
-                self._group = 'knora-admin:' + node.attrib['group']
+                self._group = "knora-admin:" + node.attrib["group"]
             else:
-                raise XmlError("Group \"{}\" is not known: ".format(node.attrib['group']))
+                raise XmlError('Group "{}" is not known: '.format(node.attrib["group"]))
         self._permission = node.text
 
     @property
     def group(self) -> str:
         """The group specified in the allow element"""
         return self._group
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-2.3.3/src/dsp_tools/models/xmlbitstream.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     """Represents a bitstream object (file) of a resource in the XML used for data import"""
 
     _value: str
     _permissions: str
 
     def __init__(self, node: etree.Element) -> None:
         self._value = node.text
-        self._permissions = node.get('permissions')
+        self._permissions = node.get("permissions")
 
     @property
     def value(self) -> str:
         """The file path of the bitstream object"""
         return self._value
 
     @property
     def permissions(self) -> str:
         """Reference to the set of permissions for the bitstream object"""
         return self._permissions
 
     def print(self) -> None:
         """Prints the bitstream object and its attributes."""
-        print('   Bitstream file path: ' + str(self._value))
+        print("   Bitstream file path: " + str(self._value))
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-2.3.3/src/dsp_tools/models/xmlpermission.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         Constructor which parses a XML DOM permissions element representing an named permission set
 
         Args:
             node: The DOM node to be processed (representing an a permission set)
             project_context: Context for DOM node traversal
         """
         self._allows = []
-        self._id = node.attrib['id']
+        self._id = node.attrib["id"]
         for allow_node in node:
             self._allows.append(XmlAllow(allow_node, project_context))
 
     @property
     def id(self) -> str:
         """The id of the permission set, p.ex. res-default"""
         return self._id
@@ -41,14 +41,14 @@
             permissions.add(allow.permission, allow.group)
         return permissions
 
     def __str__(self) -> str:
         allow_str: list[str] = []
         for allow in self._allows:
             allow_str.append("{} {}".format(allow.permission, allow.group))
-        return '|'.join(allow_str)
+        return "|".join(allow_str)
 
     def print(self) -> None:
         """Prints the permission set"""
-        print('Permission: ', self._id)
+        print("Permission: ", self._id)
         for a in self._allows:
             a.print()
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-2.3.3/src/dsp_tools/models/xmlproperty.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 from lxml import etree
 
-from dsp_tools.models.xmlerror import XmlError
+from dsp_tools.models.exceptions import XmlError
 from dsp_tools.models.xmlvalue import XMLValue
 
 
 class XMLProperty:
     """Represents a property of a resource in the XML used for data import"""
 
     _name: str
@@ -19,24 +19,24 @@
 
         Args:
             node: the property node, p.ex. <decimal-prop></decimal-prop>
             valtype: the type of value given by the name of the property node, p.ex. decimal in <decimal-prop>
             default_ontology: the name of the ontology
         """
         # get the property name which is in format namespace:propertyname, p.ex. rosetta:hasName
-        tmp_prop_name = node.attrib['name'].split(':')
+        tmp_prop_name = node.attrib["name"].split(":")
         if len(tmp_prop_name) > 1:
             if tmp_prop_name[0]:
-                self._name = node.attrib['name']
+                self._name = node.attrib["name"]
             else:
                 # replace an empty namespace with the default ontology name
-                self._name = default_ontology + ':' + tmp_prop_name[1]
+                self._name = default_ontology + ":" + tmp_prop_name[1]
         else:
-            self._name = 'knora-api:' + tmp_prop_name[0]
-        listname = node.attrib.get('list')  # safe the list name if given (only for lists)
+            self._name = "knora-api:" + tmp_prop_name[0]
+        listname = node.attrib.get("list")  # safe the list name if given (only for lists)
         self._valtype = valtype
         self._values = []
 
         # parse the subnodes of the property nodes which contain the actual values of the property
         for subnode in node:
             if subnode.tag == valtype:  # the subnode must correspond to the expected value type
                 self._values.append(XMLValue(subnode, valtype, listname))
@@ -56,10 +56,10 @@
     @property
     def values(self) -> list[XMLValue]:
         """List of values of this property"""
         return self._values
 
     def print(self) -> None:
         """Prints the property."""
-        print('  Property: {} Type: {}'.format(self._name, self._valtype))
+        print("  Property: {} Type: {}".format(self._name, self._valtype))
         for value in self._values:
             value.print()
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/xmlresource.py` & `dsp_tools-2.3.3/src/dsp_tools/models/xmlresource.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,48 +24,48 @@
     _properties: list[XMLProperty]
 
     def __init__(self, node: etree.Element, default_ontology: str) -> None:
         """
         Constructor that parses a resource node from the XML DOM
 
         Args:
-            node: The DOM node to be processed representing a resource (which is a child of the knora element)
-            default_ontology: The default ontology (given in the attribute default-ontology of the knora element)
+            node: The DOM node to be processed representing a resource (which is a child of the DSP element)
+            default_ontology: The default ontology (given in the attribute default-ontology of the DSP element)
 
         Returns:
             None
         """
-        self._id = node.attrib['id']
-        self._iri = node.attrib.get('iri')
-        self._ark = node.attrib.get('ark')
+        self._id = node.attrib["id"]
+        self._iri = node.attrib.get("iri")
+        self._ark = node.attrib.get("ark")
         self._creation_date = None
-        if node.attrib.get('creation_date'):
-            self._creation_date = DateTimeStamp(node.attrib.get('creation_date'))
-        self._label = node.attrib['label']
+        if node.attrib.get("creation_date"):
+            self._creation_date = DateTimeStamp(node.attrib.get("creation_date"))
+        self._label = node.attrib["label"]
         # get the resource type which is in format namespace:resourcetype, p.ex. rosetta:Image
-        tmp_res_type = node.attrib['restype'].split(':')
+        tmp_res_type = node.attrib["restype"].split(":")
         if len(tmp_res_type) > 1:
             if tmp_res_type[0]:
-                self._restype = node.attrib['restype']
+                self._restype = node.attrib["restype"]
             else:
                 # replace an empty namespace with the default ontology name
-                self._restype = default_ontology + ':' + tmp_res_type[1]
+                self._restype = default_ontology + ":" + tmp_res_type[1]
         else:
-            self._restype = 'knora-api:' + tmp_res_type[0]
+            self._restype = "knora-api:" + tmp_res_type[0]
         self._permissions = node.attrib.get("permissions")
         self._bitstream = None
         self._properties = []
         for subnode in node:
             if subnode.tag is etree.Comment:
                 continue
-            elif subnode.tag == 'bitstream':
+            elif subnode.tag == "bitstream":
                 self._bitstream = XMLBitstream(subnode)
             else:
                 # get the property type which is in format type-prop, p.ex. <decimal-prop>
-                prop_type, _ = subnode.tag.split('-')
+                prop_type, _ = subnode.tag.split("-")
                 self._properties.append(XMLProperty(subnode, prop_type, default_ontology))
 
     @property
     def id(self) -> str:
         """The unique id of the resource"""
         return self._id
 
@@ -110,30 +110,30 @@
 
     @properties.setter
     def properties(self, new_properties: list[XMLProperty]) -> None:
         self._properties = new_properties
 
     def print(self) -> None:
         """Prints the resource and its attributes."""
-        print(f'Resource: id={self._id}, restype: {self._restype}, label: {self._label}')
+        print(f"Resource: id={self._id}, restype: {self._restype}, label: {self._label}")
         if self._bitstream:
-            print('  Bitstream: ' + self._bitstream.value)
+            print("  Bitstream: " + self._bitstream.value)
         for prop in self._properties:
             prop.print()
 
     def get_props_with_links(self) -> list[XMLProperty]:
         """
         Get a list of all XMLProperties that have an outgoing link to another resource, be it a resptr-prop link
         or a standoff link in a text.
         """
         link_properties: list[XMLProperty] = []
         for prop in self._properties:
-            if prop.valtype == 'resptr':
+            if prop.valtype == "resptr":
                 link_properties.append(prop)
-            elif prop.valtype == 'text':
+            elif prop.valtype == "text":
                 for value in prop.values:
                     if value.resrefs:
                         link_properties.append(prop)
                         break
         return link_properties
 
     def get_resptrs(self) -> list[str]:
@@ -141,27 +141,27 @@
         Get a list of all resource id's that are referenced by this resource
 
         Returns:
             List of resources identified by their unique id's (as given in the XML)
         """
         resptrs: list[str] = []
         for prop in self._properties:
-            if prop.valtype == 'resptr':
+            if prop.valtype == "resptr":
                 for value in prop.values:
                     resptrs.append(str(value.value))
-            elif prop.valtype == 'text':
+            elif prop.valtype == "text":
                 for value in prop.values:
                     if value.resrefs:
                         resptrs.extend(value.resrefs)
         return resptrs
 
     def get_propvals(
         self,
         resiri_lookup: dict[str, str],
-        permissions_lookup: dict[str, Permissions]
+        permissions_lookup: dict[str, Permissions],
     ) -> dict[str, Union[list[Union[str, dict[str, str]]], str, dict[str, str]]]:
         """
         Get a dictionary of the property names and their values. Replace the internal ids by their IRI first.
 
         Args:
             resiri_lookup: Is used to solve internal unique id's of resources to real IRI's
             permissions_lookup: Is used to resolve the permission id's to permission sets
@@ -170,59 +170,63 @@
             A dict of values with the property name as key and a single value. This dict represents the JSON structure
             that Knora.create_resource() expects.
         """
         prop_data = {}
         for prop in self._properties:
             vals: list[Union[str, dict[str, str]]] = []
             for value in prop.values:
-                if prop.valtype == 'resptr':  # we have a resptr, therefore simple lookup or IRI
+                if prop.valtype == "resptr":  # we have a resptr, therefore simple lookup or IRI
                     iri = resiri_lookup.get(value.value)
                     if iri:
                         v = iri
                     else:
                         v = value.value  # if we do not find the id, we assume it's a valid DSP IRI
-                elif prop.valtype == 'text':
+                elif prop.valtype == "text":
                     if isinstance(value.value, KnoraStandoffXml):
                         iri_refs = value.value.get_all_iris()
                         for iri_ref in iri_refs:
-                            res_id = iri_ref.split(':')[1]
+                            res_id = iri_ref.split(":")[1]
                             iri = resiri_lookup.get(res_id)
                             if not iri:
-                                raise BaseError(f'Resource cannot be created, because it contains a salsah-Link to '
-                                                f'the following invalid resource: {res_id}.')
+                                raise BaseError(
+                                    f"Resource cannot be created, because it contains a salsah-Link to "
+                                    f"the following invalid resource: {res_id}."
+                                )
                             value.value.replace(iri_ref, iri)
                     v = value.value
                 else:
                     v = value.value
 
                 if value.comment is None and value.permissions is None:
                     # no comment or permissions
                     vals.append(v)
                 else:
                     # we have comment or permissions
-                    tmp = {'value': v}
+                    tmp = {"value": v}
                     if value.comment:
-                        tmp['comment'] = value.comment
+                        tmp["comment"] = value.comment
                     if value.permissions:
-                        tmp['permissions'] = permissions_lookup.get(value.permissions)
+                        tmp["permissions"] = permissions_lookup.get(value.permissions)
                     vals.append(tmp)
             prop_data[prop.name] = vals if len(vals) > 1 else vals[0]
         return prop_data
 
-    def get_bitstream(self, internal_file_name_bitstream: str, permissions_lookup: dict[str, Permissions]) -> Optional[dict[str, Union[str, Permissions]]]:
+    def get_bitstream(
+        self, internal_file_name_bitstream: str, permissions_lookup: dict[str, Permissions]
+    ) -> Optional[dict[str, Union[str, Permissions]]]:
         """
         Get the bitstream object belonging to the resource
 
         Args:
             internal_file_name_bitstream: Internal file name of bitstream object as returned from Sipi
             permissions_lookup: Is used to resolve the permission id's to permission sets
 
         Returns:
             A dict of the bitstream object
         """
         tmp = None
         if self._bitstream:
             bitstream = self._bitstream
-            tmp = {'value': bitstream.value, 'internal_file_name': internal_file_name_bitstream}
+            tmp = {"value": bitstream.value, "internal_file_name": internal_file_name_bitstream}
             if bitstream.permissions:
-                tmp['permissions'] = permissions_lookup.get(bitstream.permissions)
+                tmp["permissions"] = permissions_lookup.get(bitstream.permissions)
         return tmp
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-2.3.3/src/dsp_tools/models/xmlvalue.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,33 +11,32 @@
     _value: Union[str, KnoraStandoffXml]
     _resrefs: Optional[list[str]]
     _comment: str
     _permissions: str
     _is_richtext: bool
 
     def __init__(self, node: etree.Element, val_type: str, listname: Optional[str] = None) -> None:
-
         self._resrefs = None
-        self._comment = node.get('comment')
-        self._permissions = node.get('permissions')
-        if node.get('encoding') == 'xml':
+        self._comment = node.get("comment")
+        self._permissions = node.get("permissions")
+        if node.get("encoding") == "xml":
             node.attrib.clear()
             xmlstr = etree.tostring(node, encoding="unicode", method="xml")
-            xmlstr = xmlstr.replace('<text xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">', '')
-            xmlstr = xmlstr.replace('</text>', '')
+            xmlstr = xmlstr.replace('<text xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">', "")
+            xmlstr = xmlstr.replace("</text>", "")
             self._value = KnoraStandoffXml(xmlstr)
             tmp_id_list = self._value.get_all_iris()
             if tmp_id_list:
                 refs = set()
                 for tmp_id in tmp_id_list:
-                    refs.add(tmp_id.split(':')[1])
+                    refs.add(tmp_id.split(":")[1])
                 self._resrefs = list(refs)
         else:
-            if val_type == 'list':
-                self._value = listname + ':' + "".join(node.itertext())
+            if val_type == "list":
+                self._value = listname + ":" + "".join(node.itertext())
             else:
                 self._value = "".join(node.itertext())
 
     @property
     def value(self) -> Union[str, KnoraStandoffXml]:
         """The actual value of the value instance"""
         return self._value
@@ -68,13 +67,13 @@
     @property
     def is_richtext(self) -> bool:
         """true if text value is of type richtext, false otherwise"""
         return self._is_richtext
 
     def print(self) -> None:
         """Prints the value and its attributes."""
-        print('   Value: ' + str(self._value))
+        print("   Value: " + str(self._value))
         if self._comment:
-            print('   Comment:' + self._comment)
+            print("   Comment:" + self._comment)
         if self._resrefs is not None:
             for i in self._resrefs:
-                print('   res_ref: ' + i)
+                print("   res_ref: " + i)
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-2.3.3/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-2.3.3/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-2.3.3/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-2.3.3/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/schema/project.json` & `dsp_tools-2.3.3/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-2.3.3/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-2.3.3/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-2.3.3/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 ---
 
 version: '3.7'
 
 services:
 
   app:
-    image: daschswiss/dsp-app:v10.20.1  # on the verge of every deployment (fortnightly),
-                                        # take the tag of https://hub.docker.com/r/daschswiss/dsp-app/tags
-                                        # that corresponds to the version on https://admin.staging.dasch.swiss/help
-                                        # (see also https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json)
+    image: daschswiss/dsp-app:v10.20.3  # on the verge of every deployment (fortnightly), update this from the "app" value of
+                                        # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
     ports:
       - "4200:4200"
     networks:
       - knora-net
 
   db:
-    image: daschswiss/apache-jena-fuseki:2.0.11  # on the verge of every deployment (fortnightly),
-                                                 # take the tag used in docker-compose.yml of the DSP-API repository
+    image: daschswiss/apache-jena-fuseki:2.0.11  # on the verge of every deployment (fortnightly), update this from the "db" value of
+                                                 # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
     ports:
       - "3030:3030"
     networks:
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
-    image: daschswiss/knora-sipi:28.3.0  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
+    image: daschswiss/knora-sipi:29.0.0  # on the verge of every deployment (fortnightly), take the same tag as DSP-API
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -42,18 +40,16 @@
       - SIPI_WEBAPI_HOSTNAME=api
       - SIPI_WEBAPI_PORT=3333
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
-    image: daschswiss/knora-api:28.3.0  # on the verge of every deployment (fortnightly),
-                                        # take the tag of https://hub.docker.com/r/daschswiss/knora-api/tags
-                                        # that corresponds to the version on https://admin.staging.dasch.swiss/help
-                                        # (see also https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json)
+    image: daschswiss/knora-api:29.0.0  # on the verge of every deployment (fortnightly), update this from the "api" value of
+                                        # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
     depends_on:
       - sipi
       - db
     ports:
       - "3333:3333"
     networks:
       - knora-net
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,50 +19,53 @@
 """Module level variable used to ensure that there are no duplicate node names"""
 
 list_of_previous_node_names: list[str] = []
 """Module level variable used to ensure that there are no duplicate node names"""
 
 
 def expand_lists_from_excel(
-    lists_section: list[dict[str, Union[str, dict[str, Any]]]]
+    lists_section: list[dict[str, Union[str, dict[str, Any]]]],
 ) -> list[dict[str, Any]]:
     """
     Checks if the "lists" section of a JSON project file contains references to Excel files. Expands all Excel files to
     JSON, and returns the expanded "lists" section. If there are no references to Excel files, the "lists" section is
     returned as is.
     Returns a tuple consisting of the expanded "lists" section and a boolean value: True if everything went smoothly,
     False if one of the lists couldn't be expanded correctly.
 
     Args:
-        lists_section: the "lists" section of a parsed JSON project file. If this is an empty list, an empty list will be returned.
+        lists_section: the "lists" section of a parsed JSON project file.
+            If this is an empty list, an empty list will be returned.
 
     Raises:
         BaseError: if a problem occurred while trying to expand the Excel files
 
     Returns:
         the same "lists" section, but without references to Excel files
     """
     new_lists = []
     for _list in lists_section:
         if "folder" not in _list["nodes"]:
             # this list is a JSON list: return it as it is
             new_lists.append(_list)
         else:
             # this is a reference to a folder with Excel files
-            foldername = _list["nodes"]["folder"]   # type: ignore
+            foldername = _list["nodes"]["folder"]  # type: ignore
             excel_file_paths = _extract_excel_file_paths(foldername)
             try:
                 returned_lists_section = _make_json_lists_from_excel(excel_file_paths, verbose=False)
                 # we only need the "nodes" section of the first element of the returned "lists" section. This "nodes"
                 # section needs to replace the Excel folder reference. But the rest of the user-defined list element
                 # needs to stay intact, e.g. the labels and comments.
                 _list["nodes"] = returned_lists_section[0]["nodes"]
                 new_lists.append(_list)
-                print(f"\tThe list '{_list['name']}' contains a reference to the folder '{foldername}'. The Excel "
-                      f"files therein have been temporarily expanded into the 'lists' section of your project.")
+                print(
+                    f"\tThe list '{_list['name']}' contains a reference to the folder '{foldername}'. The Excel "
+                    f"files therein have been temporarily expanded into the 'lists' section of your project."
+                )
             except BaseError as err:
                 raise BaseError(
                     f"\tWARNING: The list '{_list['name']}' contains a reference to the folder '{foldername}', but a "
                     f"problem occurred while trying to expand the Excel files therein into the 'lists' section of "
                     f"your project: {err.message}"
                 ) from None
 
@@ -72,15 +75,15 @@
 def _get_values_from_excel(
     excelfiles: dict[str, Worksheet],
     base_file: dict[str, Worksheet],
     parentnode: dict[str, Any],
     row: int,
     col: int,
     preval: list[str],
-    verbose: bool = False
+    verbose: bool = False,
 ) -> tuple[int, dict[str, Any]]:
     """
     This function calls itself recursively to go through the Excel files. It extracts the cell values and composes
     the JSON list.
 
     Args:
         excelfiles: List of Excel files with the values in different languages
@@ -111,46 +114,50 @@
                 f" - Cell A1: '{excelfile['A1'].value}'\n"
                 f" - Cell B1: '{excelfile['B1'].value}'"
             )
 
     if col > 1:
         # append the cell value of the parent node (which is one value to the left of the current cell) to the list of
         # previous values
-        preval.append(str(base_file_ws.cell(column=col-1, row=row).value).strip())
+        preval.append(str(base_file_ws.cell(column=col - 1, row=row).value).strip())
 
     while cell.value and regex.search(r"\p{L}", str(cell.value), flags=re.UNICODE):
         # check if all predecessors in row (values to the left) are consistent with the values in preval list
         for idx, val in enumerate(preval[:-1]):
-            if val != str(base_file_ws.cell(column=idx+1, row=row).value).strip():
-                raise BaseError("ERROR: Inconsistency in Excel list: "
-                                f"{val} not equal to {str(base_file_ws.cell(column=idx+1, row=row).value).strip()}")
+            if val != str(base_file_ws.cell(column=idx + 1, row=row).value).strip():
+                raise BaseError(
+                    "ERROR: Inconsistency in Excel list: "
+                    f"{val} not equal to {str(base_file_ws.cell(column=idx+1, row=row).value).strip()}"
+                )
 
         # loop through the row until the last (furthest right) value is found
-        next_value = base_file_ws.cell(column=col+1, row=row).value
+        next_value = base_file_ws.cell(column=col + 1, row=row).value
         if next_value and regex.search(r"\p{L}", str(next_value), flags=re.UNICODE):
             row, _ = _get_values_from_excel(
                 excelfiles=excelfiles,
                 base_file=base_file,
                 parentnode=currentnode,
-                col=col+1,
+                col=col + 1,
                 row=row,
                 preval=preval,
-                verbose=verbose
+                verbose=verbose,
             )
 
         # if value was last in row (no further values to the right), it's a node, continue here
         else:
             # check if there are duplicate nodes (i.e. identical rows), raise a BaseError if so
             new_check_list = preval.copy()
             new_check_list.append(str(cell.value).strip())
             list_of_lists_of_previous_cell_values.append(new_check_list)
 
             if any(list_of_lists_of_previous_cell_values.count(x) > 1 for x in list_of_lists_of_previous_cell_values):
-                raise BaseError(f"ERROR: There is at least one duplicate node in the list. "
-                                f"Found duplicate in column {cell.column}, row {cell.row}:\n'{str(cell.value).strip()}'")
+                raise BaseError(
+                    f"ERROR: There is at least one duplicate node in the list. "
+                    f"Found duplicate in column {cell.column}, row {cell.row}:\n'{str(cell.value).strip()}'"
+                )
 
             # create a simplified version of the cell value and use it as name of the node
             nodename = simplify_name(str(cell.value).strip())
             list_of_previous_node_names.append(nodename)
 
             # append a number (p.ex. node-name-2) if there are list nodes with identical names
             n = list_of_previous_node_names.count(nodename)
@@ -158,16 +165,18 @@
                 nodename = nodename + "-" + str(n)
 
             # read label values from the other Excel files (other languages)
             labels_dict: dict[str, str] = {}
             for other_lang, ws_other_lang in excelfiles.items():
                 cell_value = ws_other_lang.cell(column=col, row=row).value
                 if not (isinstance(cell_value, str) and len(cell_value) > 0):
-                    raise BaseError("ERROR: Malformed Excel file: The Excel file with the language code "
-                                    f"'{other_lang}' should have a value in row {row}, column {col}")
+                    raise BaseError(
+                        "ERROR: Malformed Excel file: The Excel file with the language code "
+                        f"'{other_lang}' should have a value in row {row}, column {col}"
+                    )
                 else:
                     labels_dict[other_lang] = cell_value.strip()
 
             # create current node from extracted cell values and append it to the nodes list
             currentnode = {"name": nodename, "labels": labels_dict}
             nodes.append(currentnode)
             if verbose:
@@ -182,15 +191,18 @@
 
     # add the new nodes to the parentnode
     parentnode["nodes"] = nodes
 
     return row - 1, parentnode
 
 
-def _make_json_lists_from_excel(excel_file_paths: list[str], verbose: bool = False) -> list[dict[str, Any]]:
+def _make_json_lists_from_excel(
+    excel_file_paths: list[str],
+    verbose: bool = False,
+) -> list[dict[str, Any]]:
     """
     Reads Excel files and transforms them into a list of dictionaries that can be used as "lists" array of a JSON
     project file.
 
     Args:
         excel_file_paths: Excel files to be processed
         verbose: verbose switch
@@ -224,36 +236,36 @@
     _, _list = _get_values_from_excel(
         excelfiles=lang_to_worksheet,
         base_file=base_file,
         parentnode={},
         row=startrow,
         col=startcol,
         preval=[],
-        verbose=verbose
+        verbose=verbose,
     )
 
     # extract the children of the fictive dummy parent node
     finished_lists: list[dict[str, Any]] = _list["nodes"]
 
     # the "comments" section is mandatory for the root node of each list, so make a copy of "labels" and insert it at
     # the right place
     for i, _list in enumerate(finished_lists):
         finished_lists[i] = {
             "name": _list["name"],
             "labels": _list["labels"],
             "comments": _list["labels"],
-            "nodes": _list["nodes"]
+            "nodes": _list["nodes"],
         }
 
     return finished_lists
 
 
 def validate_lists_section_with_schema(
     path_to_json_project_file: Optional[str] = None,
-    lists_section: Optional[list[dict[str, Any]]] = None
+    lists_section: Optional[list[dict[str, Any]]] = None,
 ) -> bool:
     """
     This function checks if a "lists" section of a JSON project is valid according to the schema. The "lists" section
     can be passed as path to the JSON project file, or as Python object. Only one of the two arguments should be passed.
 
     Args:
         path_to_json_project_file: path to the JSON project file that contains the "lists" section to validate
@@ -264,30 +276,35 @@
 
     Returns:
         True if the "lists" section passed validation
     """
     if bool(path_to_json_project_file) == bool(lists_section):
         raise BaseError("Validation of the 'lists' section works only if exactly one of the two arguments is given.")
 
-    with importlib.resources.files("dsp_tools").joinpath("resources/schema/lists-only.json").open(encoding="utf-8") as schema_file:
+    with importlib.resources.files("dsp_tools").joinpath("resources/schema/lists-only.json").open(
+        encoding="utf-8"
+    ) as schema_file:
         lists_schema = json.load(schema_file)
 
     if path_to_json_project_file:
         with open(path_to_json_project_file, encoding="utf-8") as f:
             project = json.load(f)
             lists_section = project["project"].get("lists")
             if not lists_section:
-                raise BaseError(f"Cannot validate \"lists\" section of {path_to_json_project_file}, "
-                                "because there is no \"lists\" section in this file.")
+                raise BaseError(
+                    f"Cannot validate 'lists' section of {path_to_json_project_file}, "
+                    "because there is no 'lists' section in this file."
+                )
 
     try:
         jsonschema.validate(instance={"lists": lists_section}, schema=lists_schema)
     except jsonschema.ValidationError as err:
         raise BaseError(
-            f'"lists" section did not pass validation. The error message is: {err.message}\nThe error occurred at {err.json_path}'
+            f"'lists' section did not pass validation. The error message is: {err.message}\n"
+            f"The error occurred at {err.json_path}"
         ) from None
 
     return True
 
 
 def _extract_excel_file_paths(excelfolder: str) -> list[str]:
     """
@@ -303,29 +320,30 @@
     Returns:
         list of the Excel file paths to process
     """
     if not os.path.isdir(excelfolder):
         raise BaseError(f"ERROR: {excelfolder} is not a directory.")
 
     excel_file_paths = [
-        filename for filename in glob.iglob(f"{excelfolder}/*.xlsx")
+        filename
+        for filename in glob.iglob(f"{excelfolder}/*.xlsx")
         if not os.path.basename(filename).startswith("~$") and os.path.isfile(filename)
     ]
 
     for filepath in excel_file_paths:
-        if not re.search(r'^(de|en|fr|it|rm)\.xlsx$', os.path.basename(filepath)):
+        if not re.search(r"^(de|en|fr|it|rm)\.xlsx$", os.path.basename(filepath)):
             raise BaseError(f"Invalid file name '{filepath}'. Expected format: 'languagecode.xlsx'")
 
     return excel_file_paths
 
 
 def excel2lists(
     excelfolder: str,
     path_to_output_file: Optional[str] = None,
-    verbose: bool = False
+    verbose: bool = False,
 ) -> tuple[list[dict[str, Any]], bool]:
     """
     Converts lists described in Excel files into a "lists" section that can be inserted into a JSON project file.
 
     Args:
         excelfolder: path to the folder containing the Excel file(s)
         path_to_output_file: if provided, the output is written into this JSON file
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dsp_tools.utils.excel_to_json_lists import excel2lists
 from dsp_tools.utils.excel_to_json_properties import excel2properties
 from dsp_tools.utils.excel_to_json_resources import excel2resources
 
 
 def excel2json(
     data_model_files: str,
-    path_to_output_file: str
+    path_to_output_file: str,
 ) -> bool:
     """
     Converts a folder containing Excel files into a JSON data model file. The folder must be structured like this:
 
     ::
 
         data_model_files
@@ -46,32 +46,40 @@
     if not os.path.isdir(data_model_files):
         raise BaseError(f"ERROR: {data_model_files} is not a directory.")
     folder = [x for x in os.scandir(data_model_files) if not re.search(r"^(\.|~\$).+", x.name)]
 
     processed_files = []
     onto_folders = [x for x in folder if os.path.isdir(x) and re.search(r"([\w.-]+) (\([\w.\- ]+\))", x.name)]
     if len(onto_folders) == 0:
-        raise BaseError(f"'{data_model_files}' must contain at least one subfolder named after the pattern 'onto_name (onto_label)'")
+        raise BaseError(
+            f"'{data_model_files}' must contain at least one subfolder named after the pattern 'onto_name (onto_label)'"
+        )
     for onto_folder in onto_folders:
         contents = sorted([x.name for x in os.scandir(onto_folder) if not re.search(r"^(\.|~\$).+", x.name)])
         if contents != ["properties.xlsx", "resources.xlsx"]:
-            raise BaseError(f"ERROR: '{data_model_files}/{onto_folder.name}' must contain one file 'properties.xlsx' "
-                            "and one file 'resources.xlsx', but nothing else.")
+            raise BaseError(
+                f"ERROR: '{data_model_files}/{onto_folder.name}' must contain one file 'properties.xlsx' "
+                "and one file 'resources.xlsx', but nothing else."
+            )
         processed_files.extend([f"{data_model_files}/{onto_folder.name}/{file}" for file in contents])
 
     listfolder = [x for x in folder if os.path.isdir(x) and x.name == "lists"]
     if listfolder:
         listfolder_contents = [x for x in os.scandir(listfolder[0]) if not re.search(r"^(\.|~\$).+", x.name)]
         if not all(re.search(r"(de|en|fr|it|rm).xlsx", file.name) for file in listfolder_contents):
-            raise BaseError(f"The only files allowed in '{data_model_files}/lists' are en.xlsx, de.xlsx, fr.xlsx, it.xlsx, rm.xlsx")
+            raise BaseError(
+                f"The only files allowed in '{data_model_files}/lists' are en.xlsx, de.xlsx, fr.xlsx, it.xlsx, rm.xlsx"
+            )
         processed_files = [f"{data_model_files}/lists/{file.name}" for file in listfolder_contents] + processed_files
 
     if len(onto_folders) + len(listfolder) != len(folder):
-        raise BaseError(f"The only allowed subfolders in '{data_model_files}' are 'lists' "
-                        "and folders that match the pattern 'onto_name (onto_label)'")
+        raise BaseError(
+            f"The only allowed subfolders in '{data_model_files}' are 'lists' "
+            "and folders that match the pattern 'onto_name (onto_label)'"
+        )
 
     print("The following files will be processed:")
     print(*(f" - {file}" for file in processed_files), sep="\n")
 
     # create output
     # -------------
     lists, success = excel2lists(excelfolder=f"{data_model_files}/lists") if listfolder else (None, True)
@@ -81,40 +89,37 @@
     ontologies = []
     for onto_folder in onto_folders:
         name, label = re.search(r"([\w.-]+) \(([\w.\- ]+)\)", onto_folder.name).groups()  # type: ignore
         resources, success1 = excel2resources(f"{data_model_files}/{onto_folder.name}/resources.xlsx")
         properties, success2 = excel2properties(f"{data_model_files}/{onto_folder.name}/properties.xlsx")
         if not success1 or not success2:
             overall_success = False
-        ontologies.append({
-            "name": name,
-            "label": label,
-            "properties": properties,
-            "resources": resources
-        })
+        ontologies.append(
+            {
+                "name": name,
+                "label": label,
+                "properties": properties,
+                "resources": resources,
+            }
+        )
 
+    schema = "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/project.json"
     project = {
-        "prefixes": {
-            "": ""
-        },
-        "$schema": "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/project.json",
+        "prefixes": {"": ""},
+        "$schema": schema,
         "project": {
             "shortcode": "",
             "shortname": "",
             "longname": "",
-            "descriptions": {
-                "en": ""
-            },
-            "keywords": [
-                ""
-            ]
-        }
+            "descriptions": {"en": ""},
+            "keywords": [""],
+        },
     }
     if lists:
-        project["project"]["lists"] = lists        # type: ignore
+        project["project"]["lists"] = lists  # type: ignore
     project["project"]["ontologies"] = ontologies  # type: ignore
 
     with open(path_to_output_file, "w", encoding="utf-8") as f:
         json.dump(project, f, indent=4, ensure_ascii=False)
 
     print(f"JSON project file successfully saved at {path_to_output_file}")
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,63 +10,83 @@
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.shared import check_notna, prepare_dataframe
 
 languages = ["en", "de", "fr", "it", "rm"]
 
 
-def _validate_properties(properties_list: list[dict[str, Any]], excelfile: str) -> bool:
+def _validate_properties(
+    properties_list: list[dict[str, Any]],
+    excelfile: str,
+) -> bool:
     """
     This function checks if the "properties" section of a JSON project file is valid according to the JSON schema,
     and if the property names are unique.
 
     Args:
         properties_list: the "properties" section of a JSON project as a list of dicts
         excelfile: path to the Excel file containing the properties
 
     Raises:
         BaseError with a detailed error report if the validation fails
 
     Returns:
         True if the "properties" section passed validation
     """
-    with importlib.resources.files("dsp_tools").joinpath("resources/schema/properties-only.json").open(encoding="utf-8") as schema_file:
+    with importlib.resources.files("dsp_tools").joinpath("resources/schema/properties-only.json").open(
+        encoding="utf-8"
+    ) as schema_file:
         properties_schema = json.load(schema_file)
     try:
         jsonschema.validate(instance=properties_list, schema=properties_schema)
     except jsonschema.ValidationError as err:
         err_msg = f"The 'properties' section defined in the Excel file '{excelfile}' did not pass validation. "
         json_path_to_property = re.search(r"^\$\[(\d+)\]", err.json_path)
         if json_path_to_property:
-            wrong_property_name = jsonpath_ng.ext.parse(json_path_to_property.group(0)).find(properties_list)[0].value["name"]
+            # fmt: off
+            wrong_property_name = (
+                jsonpath_ng.ext.parse(json_path_to_property.group(0))
+                .find(properties_list)[0]
+                .value["name"]
+            )
+            # fmt: on
             excel_row = int(json_path_to_property.group(1)) + 2
             err_msg += f"The problematic property is '{wrong_property_name}' in Excel row {excel_row}. "
-            affected_field = re.search(r"name|labels|comments|super|subject|object|gui_element|gui_attributes", err.json_path)
+            affected_field = re.search(
+                r"name|labels|comments|super|subject|object|gui_element|gui_attributes",
+                err.json_path,
+            )
             if affected_field:
-                err_msg += f"The problem is that the column '{affected_field.group(0)}' has an invalid value: {err.message}"
+                err_msg += (
+                    f"The problem is that the column '{affected_field.group(0)}' has an invalid value: {err.message}"
+                )
         else:
             err_msg += f"The error message is: {err.message}\nThe error occurred at {err.json_path}"
         raise BaseError(err_msg) from None
 
     # check if property names are unique
     all_names = [p["name"] for p in properties_list]
     duplicates: dict[int, str] = dict()
     for index, propdef in enumerate(properties_list):
         if all_names.count(propdef["name"]) > 1:
-            duplicates[index+2] = propdef["name"]
+            duplicates[index + 2] = propdef["name"]
     if duplicates:
-        err_msg = f"Property names must be unique inside every ontology, but your Excel file '{excelfile}' contains duplicates:\n"
+        err_msg = f"Property names must be unique inside every ontology, but '{excelfile}' contains duplicates:\n"
         for row_no, propname in duplicates.items():
             err_msg += f" - Row {row_no}: {propname}\n"
         raise BaseError(err_msg)
 
     return True
 
 
-def _row2prop(row: pd.Series, row_count: int, excelfile: str) -> dict[str, Any]:
+def _row2prop(
+    row: pd.Series,
+    row_count: int,
+    excelfile: str,
+) -> dict[str, Any]:
     """
     Takes a row from a pandas DataFrame, reads its content, and returns a dict object of the property
 
     Args:
         row: row from a pandas DataFrame that defines a property
         row_count: row number of Excel file
         excelfile: name of the original Excel file
@@ -90,93 +110,107 @@
     gui_attributes = dict()
     if row.get("hlist"):
         gui_attributes["hlist"] = row["hlist"]
     if row.get("gui_attributes"):
         pairs = row["gui_attributes"].split(",")
         for pair in pairs:
             if pair.count(":") != 1:
-                raise BaseError(f"Row {row_count} of Excel file {excelfile} contains invalid data in column 'gui_attributes'. "
-                                "The expected format is 'attribute: value[, attribute: value]'.")
+                raise BaseError(
+                    f"Row {row_count} of Excel file {excelfile} contains invalid data in column 'gui_attributes'. "
+                    "The expected format is 'attribute: value[, attribute: value]'."
+                )
             attr, val = [x.strip() for x in pair.split(":")]
             if re.search(r"^\d+\.\d+$", val):
                 val = float(val)
             elif re.search(r"^\d+$", val):
                 val = int(val)
             gui_attributes[attr] = val
 
     # build the dict structure of this property
-    _property = {
-        "name": name,
-        "super": supers,
-        "object": _object,
-        "labels": labels
-    }
+    _property = {"name": name, "super": supers, "object": _object, "labels": labels}
     if comments:
         _property["comments"] = comments
     _property["gui_element"] = gui_element
     if gui_attributes:
         _property["gui_attributes"] = gui_attributes
 
     return _property
 
 
-def excel2properties(excelfile: str, path_to_output_file: Optional[str] = None) -> tuple[list[dict[str, Any]], bool]:
+def excel2properties(
+    excelfile: str,
+    path_to_output_file: Optional[str] = None,
+) -> tuple[list[dict[str, Any]], bool]:
     """
     Converts properties described in an Excel file into a "properties" section which can be inserted into a JSON
     project file.
 
     Args:
         excelfile: path to the Excel file containing the properties
         path_to_output_file: if provided, the output is written into this JSON file
 
     Raises:
         BaseError if something went wrong
 
     Returns:
-        a tuple consisting of the "properties" section as Python list, and the success status (True if everything went well)
+        a tuple consisting of the "properties" section as Python list,
+            and the success status (True if everything went well)
     """
 
     # load file
     try:
         df: pd.DataFrame = pd.read_excel(excelfile)
     except ValueError:
         # Pandas relies on openpyxl to parse XLSX files.
         # A strange behaviour of openpyxl prevents pandas from opening files with some formatting properties
         # (unclear which formatting properties exactly).
         # Apparently, the excel2json test files have one of the unsupported formatting properties.
         # The following two lines of code help out.
         # Credits: https://stackoverflow.com/a/70537454/14414188
         # pylint: disable-next=import-outside-toplevel
         from unittest import mock
-        p = mock.patch('openpyxl.styles.fonts.Font.family.max', new=100)
+
+        p = mock.patch("openpyxl.styles.fonts.Font.family.max", new=100)
         p.start()
         df = pd.read_excel(excelfile)
         p.stop()
     df = prepare_dataframe(
         df=df,
         required_columns=["name"],
-        location_of_sheet=f"File '{excelfile}'"
+        location_of_sheet=f"File '{excelfile}'",
     )
 
     # validation of input
     required = ["super", "object", "gui_element"]
     for index, row in df.iterrows():
         index = int(str(index))  # index is a label/index/hashable, but we need an int
         for req in required:
             if not check_notna(row[req]):
                 raise BaseError(f"'{excelfile}' has a missing value in row {index + 2}, column '{req}'")
     if any(df.get(lang) is not None for lang in languages):
-        warnings.warn(f"The file '{excelfile}' uses {languages} as column titles, which is deprecated. "
-                      f"Please use {[f'label_{lang}' for lang in languages]}")
+        warnings.warn(
+            f"The file '{excelfile}' uses {languages} as column titles, which is deprecated. "
+            f"Please use {[f'label_{lang}' for lang in languages]}"
+        )
     if df.get("hlist"):
-        warnings.warn(f"The file '{excelfile}' has a column 'hlist', which is deprecated. "
-                      f"Please use the column 'gui_attributes' for the attribute 'hlist'.")
+        warnings.warn(
+            f"The file '{excelfile}' has a column 'hlist', which is deprecated. "
+            f"Please use the column 'gui_attributes' for the attribute 'hlist'."
+        )
 
     # transform every row into a property
-    props = [_row2prop(row, int(str(index)), excelfile) for index, row in df.iterrows()]   # index is a label/index/hashable, but we need an int
+    props: list[dict[str, Any]] = []
+    for index, row in df.iterrows():
+        props.append(
+            _row2prop(
+                row=row,
+                row_count=int(str(index)),  # index is a label/index/hashable, but we need an int
+                excelfile=excelfile,
+            )
+        )
 
     # write final JSON file
     _validate_properties(properties_list=props, excelfile=excelfile)
     if path_to_output_file:
         with open(file=path_to_output_file, mode="w", encoding="utf-8") as file:
             json.dump(props, file, indent=4, ensure_ascii=False)
             print('"properties" section was created successfully and written to file:', path_to_output_file)
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,74 +10,97 @@
 
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.shared import check_notna, prepare_dataframe
 
 languages = ["en", "de", "fr", "it", "rm"]
 
 
-def _validate_resources(resources_list: list[dict[str, Any]], excelfile: str) -> bool:
+def _validate_resources(
+    resources_list: list[dict[str, Any]],
+    excelfile: str,
+) -> bool:
     """
     This function checks if the "resources" section of a JSON project file is valid according to the JSON schema,
     and if the resource names are unique.
 
     Args:
         resources_list: the "resources" section of a JSON project as a list of dicts
         excelfile: path to the Excel file containing the resources
 
     Raises:
         BaseError with a detailed error report if the validation fails
 
     Returns:
         True if the "resources" section passed validation
     """
-    with importlib.resources.files("dsp_tools").joinpath("resources/schema/resources-only.json").open(encoding="utf-8") as schema_file:
+    with importlib.resources.files("dsp_tools").joinpath("resources/schema/resources-only.json").open(
+        encoding="utf-8"
+    ) as schema_file:
         resources_schema = json.load(schema_file)
     try:
         jsonschema.validate(instance=resources_list, schema=resources_schema)
     except jsonschema.ValidationError as err:
         err_msg = f"The 'resources' section defined in the Excel file '{excelfile}' did not pass validation. "
         json_path_to_resource = regex.search(r"^\$\[(\d+)\]", err.json_path)
         if json_path_to_resource:
-            wrong_resource_name = jsonpath_ng.ext.parse(json_path_to_resource.group(0)).find(resources_list)[0].value["name"]
+            # fmt: off
+            wrong_resource_name = (
+                jsonpath_ng.ext.parse(json_path_to_resource.group(0))
+                .find(resources_list)[0]
+                .value["name"]
+            )
+            # fmt: on
             affected_field = regex.search(r"name|labels|comments|super|cardinalities\[(\d+)\]", err.json_path)
             if affected_field and affected_field.group(0) in ["name", "labels", "comments", "super"]:
                 excel_row = int(json_path_to_resource.group(1)) + 2
-                err_msg += f"The problem is that the Excel sheet 'classes' contains an invalid value for resource '{wrong_resource_name}', " \
-                           f"in row {excel_row}, column '{affected_field.group(0)}': {err.message}"
+                err_msg += (
+                    f"The problem is that the Excel sheet 'classes' contains an invalid value for resource "
+                    f"'{wrong_resource_name}', in row {excel_row}, column '{affected_field.group(0)}': {err.message}"
+                )
             elif affected_field and "cardinalities" in affected_field.group(0):
                 excel_row = int(affected_field.group(1)) + 2
                 if err.json_path.endswith("cardinality"):
-                    err_msg += f"The problem is that the Excel sheet '{wrong_resource_name}' contains an invalid value " \
-                               f"in row {excel_row}, column 'Cardinality': {err.message}"
+                    err_msg += (
+                        f"The problem is that the Excel sheet '{wrong_resource_name}' contains an invalid value "
+                        f"in row {excel_row}, column 'Cardinality': {err.message}"
+                    )
                 elif err.json_path.endswith("propname"):
-                    err_msg += f"The problem is that the Excel sheet '{wrong_resource_name}' contains an invalid value " \
-                               f"in row {excel_row}, column 'Property': {err.message}"
+                    err_msg += (
+                        f"The problem is that the Excel sheet '{wrong_resource_name}' contains an invalid value "
+                        f"in row {excel_row}, column 'Property': {err.message}"
+                    )
         else:
             err_msg += f"The error message is: {err.message}\nThe error occurred at {err.json_path}"
         raise BaseError(err_msg) from None
 
     # check if resource names are unique
     all_names = [r["name"] for r in resources_list]
     duplicates: dict[int, str] = dict()
     for index, resdef in enumerate(resources_list):
         if all_names.count(resdef["name"]) > 1:
-            duplicates[index+2] = resdef["name"]
+            duplicates[index + 2] = resdef["name"]
     if duplicates:
-        err_msg = f"Resource names must be unique inside every ontology, but your Excel file '{excelfile}' contains duplicates:\n"
+        err_msg = (
+            f"Resource names must be unique inside every ontology, "
+            f"but your Excel file '{excelfile}' contains duplicates:\n"
+        )
         for row_no, resname in duplicates.items():
             err_msg += f" - Row {row_no}: {resname}\n"
         raise BaseError(err_msg)
 
     return True
 
 
-def _row2resource(row: pd.Series, excelfile: str) -> dict[str, Any]:
+def _row2resource(
+    row: pd.Series,
+    excelfile: str,
+) -> dict[str, Any]:
     """
-    Method that reads one row from the "classes" DataFrame, 
-    opens the corresponding details DataFrame, 
+    Method that reads one row from the "classes" DataFrame,
+    opens the corresponding details DataFrame,
     and builds a dict object of the resource.
 
     Args:
         row: row from the "classes" DataFrame
         excelfile: Excel file where the data comes from
 
     Raises:
@@ -102,25 +125,26 @@
         # A strange behaviour of openpyxl prevents pandas from opening files with some formatting properties
         # (unclear which formatting properties exactly).
         # Apparently, the excel2json test files have one of the unsupported formatting properties.
         # The following two lines of code help out.
         # Credits: https://stackoverflow.com/a/70537454/14414188
         # pylint: disable-next=import-outside-toplevel
         from unittest import mock
-        p = mock.patch('openpyxl.styles.fonts.Font.family.max', new=100)
+
+        p = mock.patch("openpyxl.styles.fonts.Font.family.max", new=100)
         p.start()
         try:
             details_df = pd.read_excel(excelfile, sheet_name=name)
         except ValueError as err:
             raise BaseError(str(err)) from None
         p.stop()
     details_df = prepare_dataframe(
         df=details_df,
         required_columns=["Property", "Cardinality"],
-        location_of_sheet=f"Sheet '{name}' in file '{excelfile}'"
+        location_of_sheet=f"Sheet '{name}' in file '{excelfile}'",
     )
 
     # validation
     # 4 cases:
     #  - column gui_order absent
     #  - column gui_order empty
     #  - column gui_order present but not properly filled in (missing values / not integers)
@@ -135,88 +159,94 @@
         try:
             [int(float(x)) for x in details_df["gui_order"]]
         except ValueError:
             validation_passed = False
     else:  # column gui_order present but not properly filled in (missing values)
         validation_passed = False
     if not validation_passed:
-        raise BaseError(f"Sheet '{name}' in file '{excelfile}' has invalid content in column 'gui_order': "
-                        f"only positive integers allowed (or leave column empty altogether)")
+        raise BaseError(
+            f"Sheet '{name}' in file '{excelfile}' has invalid content in column 'gui_order': "
+            f"only positive integers allowed (or leave column empty altogether)"
+        )
 
     cards = []
     for j, detail_row in details_df.iterrows():
         j = int(str(j))  # j is a label/index/hashable, but we need an int
         gui_order = detail_row.get("gui_order", "")
         gui_order = regex.sub(r"\.0+", "", str(gui_order))
         property_ = {
             "propname": ":" + detail_row["property"],
             "cardinality": detail_row["cardinality"].lower(),
-            "gui_order": int(gui_order or j + 1)  # if gui_order not given: take sheet order
+            "gui_order": int(gui_order or j + 1),  # if gui_order not given: take sheet order
         }
         cards.append(property_)
 
     # build the dict structure of this resource and append it to the list of resources
-    resource = {
-        "name": name,
-        "super": supers,
-        "labels": labels
-    }
+    resource = {"name": name, "super": supers, "labels": labels}
     if comments:
         resource["comments"] = comments
     resource["cardinalities"] = cards
 
     return resource
 
 
-def excel2resources(excelfile: str, path_to_output_file: Optional[str] = None) -> tuple[list[dict[str, Any]], bool]:
+def excel2resources(
+    excelfile: str,
+    path_to_output_file: Optional[str] = None,
+) -> tuple[list[dict[str, Any]], bool]:
     """
     Converts resources described in an Excel file into a "resources" section which can be inserted into a JSON
     project file.
 
     Args:
         excelfile: path to the Excel file containing the resources
-        path_to_output_file: if provided, the output is written into this JSON file (otherwise, it's only returned as return value)
+        path_to_output_file: if provided, the output is written into this JSON file
+            (otherwise, it's only returned as return value)
 
     Raises:
         BaseError if something went wrong
 
     Returns:
-        a tuple consisting of the "resources" section as Python list, and the success status (True if everything went well)
+        a tuple consisting of the "resources" section as Python list,
+            and the success status (True if everything went well)
     """
 
     # load file
     try:
         all_classes_df: pd.DataFrame = pd.read_excel(excelfile)
     except ValueError:
         # Pandas relies on openpyxl to parse XLSX files.
         # A strange behaviour of openpyxl prevents pandas from opening files with some formatting properties
         # (unclear which formatting properties exactly).
         # Apparently, the excel2json test files have one of the unsupported formatting properties.
         # The following two lines of code help out.
         # Credits: https://stackoverflow.com/a/70537454/14414188
         # pylint: disable-next=import-outside-toplevel
         from unittest import mock
-        p = mock.patch('openpyxl.styles.fonts.Font.family.max', new=100)
+
+        p = mock.patch("openpyxl.styles.fonts.Font.family.max", new=100)
         p.start()
         all_classes_df = pd.read_excel(excelfile)
         p.stop()
     all_classes_df = prepare_dataframe(
         df=all_classes_df,
         required_columns=["name"],
-        location_of_sheet=f"Sheet 'classes' in file '{excelfile}'"
+        location_of_sheet=f"Sheet 'classes' in file '{excelfile}'",
     )
 
     # validation
     for index, row in all_classes_df.iterrows():
         index = int(str(index))  # index is a label/index/hashable, but we need an int
         if not check_notna(row["super"]):
             raise BaseError(f"Sheet 'classes' of '{excelfile}' has a missing value in row {index + 2}, column 'super'")
     if any(all_classes_df.get(lang) is not None for lang in languages):
-        warnings.warn(f"The file {excelfile} uses {languages} as column titles, which is deprecated. "
-                      f"Please use {[f'label_{lang}' for lang in languages]}")
+        warnings.warn(
+            f"The file {excelfile} uses {languages} as column titles, which is deprecated. "
+            f"Please use {[f'label_{lang}' for lang in languages]}"
+        )
 
     # transform every row into a resource
     resources = [_row2resource(row, excelfile) for i, row in all_classes_df.iterrows()]
 
     # write final "resources" section into a JSON file
     _validate_resources(resources_list=resources, excelfile=excelfile)
     if path_to_output_file:
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/id_to_iri.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,28 @@
 from typing import Optional
 
 from lxml import etree
 
 from dsp_tools.models.exceptions import BaseError
 
 
-def id_to_iri(xml_file: str, json_file: str, out_file: Optional[str], verbose: bool) -> bool:
+def id_to_iri(
+    xml_file: str,
+    json_file: str,
+    out_file: Optional[str],
+    verbose: bool,
+) -> bool:
     """
     This function replaces all occurrences of internal IDs with their respective IRIs inside an XML file. It gets the
     mapping from the JSON file provided as parameter for this function.
 
     Args:
         xml_file: the XML file with the data to be replaced
         json_file: the JSON file with the mapping (dict) of internal IDs to IRIs
-        out_file: path to the output XML file with replaced IDs (optional), default "id2iri_replaced_" + timestamp + ".xml"
+        out_file: path to output XML file with replaced IDs (optional), default "id2iri_replaced_" + timestamp + ".xml"
         verbose: verbose feedback if set to True
 
     Raises:
         BaseError if one of the two input files is not a valid file
 
     Returns:
         True if everything went well, False otherwise
@@ -35,15 +40,15 @@
     if not os.path.isfile(xml_file):
         raise BaseError(f"File {xml_file} could not be found.")
 
     if not os.path.isfile(json_file):
         raise BaseError(f"File {json_file} could not be found.")
 
     # load JSON from provided json file to dict
-    with open(json_file, encoding="utf-8", mode='r') as file:
+    with open(json_file, encoding="utf-8", mode="r") as file:
         mapping = json.load(file)
 
     # parse XML from provided xml file
     tree = etree.parse(xml_file)
 
     # iterate through all XML elements and remove namespace declarations
     for elem in tree.iter():
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/logging.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import logging
 import logging.handlers
 from pathlib import Path
 
 
 def get_logger(name: str) -> logging.Logger:
     """
-    Create a logger instance, 
+    Create a logger instance,
     set its level to INFO,
     and configure it to write to a file in the user's home directory.
-    
+
     Args:
         name: name of the logger
 
     Returns:
         the logger instance
     """
     _logger = logging.getLogger(name)
     _logger.setLevel(logging.INFO)
-    formatter = logging.Formatter(
-        fmt="{asctime} {filename: <20} {levelname: <8} {message}",
-        style="{"
-    )
-    # a RotatingFileHandler fills "filename" until it is "maxBytes" big, 
+    formatter = logging.Formatter(fmt="{asctime} {filename: <20} {levelname: <8} {message}", style="{")
+    # a RotatingFileHandler fills "filename" until it is "maxBytes" big,
     # then appends ".1" to it and starts with a new file "filename",
     # fills it until it is "maxBytes" big,
     # then appends ".1" to it (replacing the old ".1" file)
     logfile_directory = Path.home() / Path(".dsp-tools")
     logfile_directory.mkdir(exist_ok=True)
     handler = logging.handlers.RotatingFileHandler(
         filename=logfile_directory / "logging.log",
         mode="a",
-        maxBytes=3*1024*1024,
-        backupCount=1
+        maxBytes=5 * 1024 * 1024,
+        backupCount=4,
     )
     handler.setFormatter(formatter)
     _logger.addHandler(handler)
     return _logger
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/project_create.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/project_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 logger = get_logger(__name__)
 
 
 def _create_project_on_server(
     project_definition: dict[str, Any],
     con: Connection,
-    verbose: bool
+    verbose: bool,
 ) -> tuple[Project, bool]:
     """
-    Create the project on the DSP server. 
+    Create the project on the DSP server.
     If it already exists: update its longname, description and keywords.
 
     Args:
         project_definition: parsed JSON project definition
         con: connection to the DSP server
         verbose: verbose switch
 
@@ -43,66 +43,74 @@
     Returns:
         a tuple of the remote project and the success status (True if everything went smoothly, False otherwise)
     """
     try:
         # the normal, expected case is that this try block fails
         project_local = Project(con=con, shortcode=project_definition["project"]["shortcode"])
         project_remote: Project = try_network_action(project_local.read)
-        print(f"\tWARNING: Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP server. Updating it...")
-        logger.warning(f"Project '{project_remote.shortname}' ({project_remote.shortcode}) already exists on the DSP server. Updating it...")
+        proj_designation = f"'{project_remote.shortname}' ({project_remote.shortcode})"
+        msg = f"Project {proj_designation} already exists on the DSP server. Updating it..."
+        print(f"\tWARNING: {msg}")
+        logger.warning(msg)
         # try to update the basic info
-        project_remote, _ = _update_basic_info_of_project(project=project_remote, project_definition=project_definition, verbose=verbose)
+        project_remote, _ = _update_basic_info_of_project(
+            project=project_remote, project_definition=project_definition, verbose=verbose
+        )
         # It doesn't matter if the update is successful or not: continue anyway, because success is anyways false.
-        # There are other things from this file that can be created on the server, e.g. the groups and users, so the process must continue.
+        # There are other things from this file that can be created on the server,
+        # e.g. the groups and users, so the process must continue.
         return project_remote, False
     except BaseError:
         pass
 
     success = True
     project_local = Project(
         con=con,
         shortcode=project_definition["project"]["shortcode"],
         shortname=project_definition["project"]["shortname"],
         longname=project_definition["project"]["longname"],
         description=LangString(project_definition["project"].get("descriptions")),
         keywords=set(project_definition["project"].get("keywords")),
         selfjoin=False,
-        status=True
+        status=True,
     )
     try:
         project_remote = try_network_action(project_local.create)
     except BaseError:
-        err_msg = f"Cannot create project '{project_definition['project']['shortname']}' " \
-                  f"({project_definition['project']['shortcode']}) on DSP server."
+        err_msg = (
+            f"Cannot create project '{project_definition['project']['shortname']}' "
+            f"({project_definition['project']['shortcode']}) on DSP server."
+        )
         logger.error(err_msg, exc_info=True)
         raise UserError(err_msg) from None
     print(f"\tCreated project '{project_remote.shortname}' ({project_remote.shortcode}).")
     return project_remote, success
 
 
 def _update_basic_info_of_project(
     project: Project,
     project_definition: dict[str, Any],
-    verbose: bool
+    verbose: bool,
 ) -> tuple[Project, bool]:
     """
-    Updates the longname, description and keywords of a project on a DSP server. 
-    Returns the updated project (or the unchanged project if not successful) and a boolean saying if the update was successful or not. 
+    Updates the longname, description and keywords of a project on a DSP server.
+    Returns the updated project (or the unchanged project if not successful)
+    and a boolean saying if the update was successful or not.
     If the update was not successful, an error message is printed to stdout.
 
     Args:
         project: the project to be updated (must exist on the DSP server)
         project_definition: a parsed JSON project file with the same shortname and shortcode than the existing project
 
     Returns:
         tuple of (updated project, success status)
     """
     # store in variables for convenience
-    shortcode = project_definition['project']['shortcode']
-    shortname = project_definition['project']['shortname']
+    shortcode = project_definition["project"]["shortcode"]
+    shortname = project_definition["project"]["shortname"]
 
     # update the local "project" object
     project.longname = project_definition["project"]["longname"]
     project.description = project_definition["project"].get("descriptions")
     project.keywords = project_definition["project"].get("keywords")
 
     # make the call to DSP-API
@@ -114,41 +122,48 @@
         return project_remote, True
     except BaseError:
         print(f"WARNING: Could not update project '{shortname}' ({shortcode}).")
         logger.warning(f"Could not update project '{shortname}' ({shortcode}).", exc_info=True)
         return project, False
 
 
-def _create_groups(con: Connection, groups: list[dict[str, str]], project: Project) -> tuple[dict[str, Group], bool]:
+def _create_groups(
+    con: Connection,
+    groups: list[dict[str, str]],
+    project: Project,
+) -> tuple[dict[str, Group], bool]:
     """
     Creates groups on a DSP server from the "groups" section of a JSON project file. If a group cannot be created, it is
     skipped and a warning is printed, but such a group will still be part of the returned dict.
     Returns a tuple consisting of a dict and a bool. The dict contains the groups that have successfully been created
     (or already exist). The bool indicates if everything went smoothly during the process. If a warning or error
     occurred, it is False.
 
     Args:
         con: connection instance to connect to the DSP server
         groups: "groups" section of a parsed JSON project file
         project: Project the group(s) should be added to (must exist on DSP server)
 
     Returns:
-        A tuple consisting of a dict and the success status. 
-        The dict has the form ``{group name: group object}`` for all groups that have successfully been created (or already exist). 
+        A tuple consisting of a dict and the success status.
+        The dict has the form ``{group name: group object}``
+        for all groups that have successfully been created (or already exist).
         The dict is empty if no group was created.
     """
     overall_success = True
     current_project_groups: dict[str, Group] = {}
     try:
         remote_groups: list[Group] = try_network_action(
             lambda: Group.getAllGroupsForProject(con=con, proj_iri=project.id)  # type: ignore
         )
     except BaseError:
-        err_msg = "Unable to check if group names are already existing on DSP server, because it is " \
-                  "not possible to retrieve the remote groups from the DSP server."
+        err_msg = (
+            "Unable to check if group names are already existing on DSP server, because it is "
+            "not possible to retrieve the remote groups from the DSP server."
+        )
         print(f"WARNING: {err_msg}")
         logger.warning(err_msg, exc_info=True)
         remote_groups = []
         overall_success = False
 
     for group in groups:
         group_name = group["name"]
@@ -164,15 +179,15 @@
         # create the group
         group_local = Group(
             con=con,
             name=group_name,
             descriptions=LangString(group["descriptions"]),
             project=project,
             status=bool(group.get("status", True)),
-            selfjoin=bool(group.get("selfjoin", False))
+            selfjoin=bool(group.get("selfjoin", False)),
         )
         try:
             group_remote: Group = try_network_action(group_local.create)
         except BaseError:
             print(f"\tWARNING: Unable to create group '{group_name}'.")
             logger.warning(f"Unable to create group '{group_name}'.", exc_info=True)
             overall_success = False
@@ -185,89 +200,97 @@
 
 
 def _get_group_iris_for_user(
     json_user_definition: dict[str, str],
     current_project: Project,
     current_project_groups: dict[str, Group],
     con: Connection,
-    verbose: bool
+    verbose: bool,
 ) -> tuple[set[str], bool, bool]:
     """
     Retrieve the IRIs of the groups that the user belongs to.
 
     Args:
         json_user_definition: the section of the JSON file that defines a user
         current_project: the Project object
-        current_project_groups: dict of the form ``{group name: group object}`` with the groups that exist on the DSP server
+        current_project_groups: dict of the form ``{group name: group object}``
+            with the groups that exist on the DSP server
         con: connection to the DSP server
         verbose: verbose switch
 
     Returns:
-        a tuple consisting of the group IRIs, 
-        the system admin status (True if the user is sysadmin, False otherwise), 
+        a tuple consisting of the group IRIs,
+        the system admin status (True if the user is sysadmin, False otherwise),
         and the success status (True if everything went well)
     """
     success = True
     username = json_user_definition["username"]
     group_iris: set[str] = set()
     sysadmin = False
     remote_groups: list[Group] = []
     for full_group_name in json_user_definition.get("groups", []):
         # full_group_name has the form '[project_shortname]:group_name' or 'SystemAdmin'
+        inexisting_group_msg = (
+            f"User {username} cannot be added to group {full_group_name}, because such a group doesn't exist."
+        )
         if ":" not in full_group_name and full_group_name != "SystemAdmin":
-            print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a group doesn't exist.")
+            print(f"\tWARNING: {inexisting_group_msg}")
             success = False
             continue
 
         if full_group_name == "SystemAdmin":
             sysadmin = True
             if verbose:
                 print(f"\tAdded user '{username}' to group 'SystemAdmin'.")
             continue
 
         # all other cases (":" in full_group_name)
         project_shortname, group_name = full_group_name.split(":")
         if not project_shortname:
             # full_group_name refers to a group inside the same project
             if group_name not in current_project_groups:
-                print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a group doesn't exist.")
+                print(f"\tWARNING: {inexisting_group_msg}")
                 success = False
                 continue
             group = current_project_groups[group_name]
         else:
             # full_group_name refers to an already existing group on DSP
             try:
                 # "remote_groups" might be available from a previous loop cycle
                 remote_groups = remote_groups or try_network_action(lambda: Group.getAllGroups(con=con))
             except BaseError:
-                err_msg = f"User '{username}' is referring to the group {full_group_name} that " \
-                          f"exists on the DSP server, but no groups could be retrieved from the DSP server."
+                err_msg = (
+                    f"User '{username}' is referring to the group {full_group_name} that "
+                    f"exists on the DSP server, but no groups could be retrieved from the DSP server."
+                )
                 print(f"\tWARNING: {err_msg}")
                 logger.warning(err_msg, exc_info=True)
                 success = False
                 continue
             existing_group = [g for g in remote_groups if g.project == current_project.id and g.name == group_name]
             if not existing_group:
-                print(f"\tWARNING: User {username} cannot be added to group {full_group_name}, because such a group doesn't exist.")
+                print(f"\tWARNING: {inexisting_group_msg}")
                 success = False
                 continue
             group = existing_group[0]
 
-        group_iris.add(group.id)  # type: ignore
+        if not group.iri:
+            raise BaseError(f"Group '{group}' has no IRI.")
+        group_iris.add(group.iri)
         if verbose:
             print(f"\tAdded user '{username}' to group '{full_group_name}'.")
 
     return group_iris, sysadmin, success
 
 
 def _get_projects_where_user_is_admin(
     json_user_definition: dict[str, str],
     current_project: Project,
     con: Connection,
-    verbose: bool
+    verbose: bool,
 ) -> tuple[dict[str, bool], bool]:
     """
     Create a dict that tells for every project if the user is administrator in that project or not.
 
     Args:
         json_user_definition: the section of the JSON file that defines a user
         current_project: the Project object
@@ -294,23 +317,27 @@
             in_project = current_project
         else:
             # full_project_name refers to an already existing project on DSP
             try:
                 # "remote_projects" might be available from a previous loop cycle
                 remote_projects = remote_projects or try_network_action(lambda: current_project.getAllProjects(con=con))
             except BaseError:
-                err_msg = f"User '{username}' cannot be added to the projects {json_user_definition['projects']} " \
-                          f"because the projects cannot be retrieved from the DSP server."
+                err_msg = (
+                    f"User '{username}' cannot be added to the projects {json_user_definition['projects']} "
+                    f"because the projects cannot be retrieved from the DSP server."
+                )
                 print(f"\tWARNING: {err_msg}")
                 logger.warning(err_msg, exc_info=True)
                 success = False
                 continue
             in_project_list = [p for p in remote_projects if p.shortname == project_name]
             if not in_project_list:
-                print(f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. Skipping...")
+                print(
+                    f"\tWARNING: Provided project '{full_project_name}' for user '{username}' is not valid. Skipping..."
+                )
                 success = False
                 continue
             in_project = in_project_list[0]
 
         project_info[in_project.id] = bool(project_role == "admin")  # type: ignore
         if verbose:
             print(f"\tAdded user '{username}' as {project_role} to project '{in_project.shortname}'.")
@@ -319,24 +346,25 @@
 
 
 def _create_users(
     con: Connection,
     users_section: list[dict[str, str]],
     current_project_groups: dict[str, Group],
     current_project: Project,
-    verbose: bool
+    verbose: bool,
 ) -> bool:
     """
-    Creates users on a DSP server from the "users" section of a JSON project file. 
+    Creates users on a DSP server from the "users" section of a JSON project file.
     If a user cannot be created, a warning is printed and the user is skipped.
 
     Args:
         con: connection instance to connect to the DSP server
         users_section: "users" section of a parsed JSON project file
-        current_project_groups: groups defined in the current project, {group name: group object} (must exist on DSP server)
+        current_project_groups: groups defined in the current project, in the form ``{group name: group object}``
+            (must exist on DSP server)
         current_project: "project" object of the current project (must exist on DSP server)
         verbose: Prints more information if set to True
 
     Returns:
         True if all users could be created without any problems. False if a warning/error occurred.
     """
     overall_success = True
@@ -356,25 +384,25 @@
 
         # add user to the group(s)
         group_iris, sysadmin, success = _get_group_iris_for_user(
             json_user_definition=json_user_definition,
             current_project=current_project,
             current_project_groups=current_project_groups,
             con=con,
-            verbose=verbose
+            verbose=verbose,
         )
         if not success:
             overall_success = False
 
         # add user to the project(s)
         project_info, success = _get_projects_where_user_is_admin(
             json_user_definition=json_user_definition,
             current_project=current_project,
             con=con,
-            verbose=verbose
+            verbose=verbose,
         )
         if not success:
             overall_success = False
 
         # create the user
         user_local = User(
             con=con,
@@ -383,29 +411,32 @@
             givenName=json_user_definition["givenName"],
             familyName=json_user_definition["familyName"],
             password=json_user_definition["password"],
             status=bool(json_user_definition.get("status", True)),
             lang=json_user_definition.get("lang", "en"),
             sysadmin=sysadmin,
             in_projects=project_info,
-            in_groups=group_iris
+            in_groups=group_iris,
         )
         try:
             try_network_action(user_local.create)
         except BaseError:
             print(f"\tWARNING: Unable to create user '{username}'.")
             logger.warning(f"Unable to create user '{username}'.", exc_info=True)
             overall_success = False
             continue
         print(f"\tCreated user '{username}'.")
 
     return overall_success
 
 
-def _sort_resources(unsorted_resources: list[dict[str, Any]], onto_name: str) -> list[dict[str, Any]]:
+def _sort_resources(
+    unsorted_resources: list[dict[str, Any]],
+    onto_name: str,
+) -> list[dict[str, Any]]:
     """
     This method sorts the resource classes in an ontology according to their inheritance order (parent classes first).
 
     Args:
         unsorted_resources: list of resources from a parsed JSON project file
         onto_name: name of the onto
 
@@ -417,27 +448,30 @@
     resources_to_sort = unsorted_resources.copy()
     sorted_resources: list[dict[str, Any]] = list()
     ok_resource_names: list[str] = list()
     while len(resources_to_sort) > 0:
         # inside the for loop, resources_to_sort is modified, so a copy must be made to iterate over
         for res in resources_to_sort.copy():
             res_name = f'{onto_name}:{res["name"]}'
-            parent_classes = res['super']
+            parent_classes = res["super"]
             if isinstance(parent_classes, str):
                 parent_classes = [parent_classes]
-            parent_classes = [re.sub(r'^:([^:]+)$', f'{onto_name}:\\1', elem) for elem in parent_classes]
+            parent_classes = [re.sub(r"^:([^:]+)$", f"{onto_name}:\\1", elem) for elem in parent_classes]
             parent_classes_ok = [not p.startswith(onto_name) or p in ok_resource_names for p in parent_classes]
             if all(parent_classes_ok):
                 sorted_resources.append(res)
                 ok_resource_names.append(res_name)
                 resources_to_sort.remove(res)
     return sorted_resources
 
 
-def _sort_prop_classes(unsorted_prop_classes: list[dict[str, Any]], onto_name: str) -> list[dict[str, Any]]:
+def _sort_prop_classes(
+    unsorted_prop_classes: list[dict[str, Any]],
+    onto_name: str,
+) -> list[dict[str, Any]]:
     """
     In case of inheritance, parent properties must be uploaded before their children. This method sorts the
     properties.
 
     Args:
         unsorted_prop_classes: list of properties from a parsed JSON project file
         onto_name: name of the onto
@@ -450,18 +484,18 @@
     prop_classes_to_sort = unsorted_prop_classes.copy()
     sorted_prop_classes: list[dict[str, Any]] = list()
     ok_propclass_names: list[str] = list()
     while len(prop_classes_to_sort) > 0:
         # inside the for loop, resources_to_sort is modified, so a copy must be made to iterate over
         for prop in prop_classes_to_sort.copy():
             prop_name = f'{onto_name}:{prop["name"]}'
-            parent_classes = prop.get('super', 'hasValue')
+            parent_classes = prop.get("super", "hasValue")
             if isinstance(parent_classes, str):
                 parent_classes = [parent_classes]
-            parent_classes = [re.sub(r'^:([^:]+)$', f'{onto_name}:\\1', elem) for elem in parent_classes]
+            parent_classes = [re.sub(r"^:([^:]+)$", f"{onto_name}:\\1", elem) for elem in parent_classes]
             parent_classes_ok = [not p.startswith(onto_name) or p in ok_propclass_names for p in parent_classes]
             if all(parent_classes_ok):
                 sorted_prop_classes.append(prop)
                 ok_propclass_names.append(prop_name)
                 prop_classes_to_sort.remove(prop)
     return sorted_prop_classes
 
@@ -469,15 +503,15 @@
 def _create_ontologies(
     con: Connection,
     context: Context,
     knora_api_prefix: str,
     list_root_nodes: dict[str, Any],
     project_definition: dict[str, Any],
     project_remote: Project,
-    verbose: bool
+    verbose: bool,
 ) -> bool:
     """
     Iterates over the ontologies in a JSON project file and creates the ontologies that don't exist on the DSP server
     yet. For every ontology, it first creates the resource classes, then the properties, and then adds the cardinalities
     to the resource classes.
 
     Args:
@@ -486,31 +520,32 @@
         knora_api_prefix: the prefix that stands for the knora-api ontology
         list_root_nodes: the IRIs of the list nodes that were already created and are now available on the DSP server
         project_definition: the parsed JSON project file
         project_remote: representation of the project on the DSP server
         verbose: verbose switch
 
     Raises:
-        UserError if an error occurs during the creation of an ontology. 
+        UserError if an error occurs during the creation of an ontology.
         All other errors are printed, the process continues, but the success status will be false.
 
     Returns:
         True if everything went smoothly, False otherwise
     """
 
     overall_success = True
 
     print("Create ontologies...")
     try:
         project_ontologies: list[Ontology] = try_network_action(
             lambda: Ontology.getProjectOntologies(con=con, project_id=project_remote.id)  # type: ignore
         )
     except BaseError:
-        print("WARNING: Unable to retrieve remote ontologies. Cannot check if your ontology already exists.")
-        logger.warning("Unable to retrieve remote ontologies. Cannot check if your ontology already exists.", exc_info=True)
+        err_msg = "Unable to retrieve remote ontologies. Cannot check if your ontology already exists."
+        print("WARNING: {err_msg}")
+        logger.warning(err_msg, exc_info=True)
         project_ontologies = []
     for ontology_definition in project_definition.get("project", {}).get("ontologies", {}):
         ontology_definition = cast(dict[str, Any], ontology_definition)
         if ontology_definition["name"] in [onto.name for onto in project_ontologies]:
             print(f"\tWARNING: Ontology '{ontology_definition['name']}' already exists on the DSP server. Skipping...")
             overall_success = False
             continue
@@ -518,25 +553,25 @@
         # create the ontology
         print(f"Create ontology '{ontology_definition['name']}'...")
         ontology_local = Ontology(
             con=con,
             project=project_remote,
             label=ontology_definition["label"],
             name=ontology_definition["name"],
-            comment=ontology_definition.get("comment")
+            comment=ontology_definition.get("comment"),
         )
         # if ontology cannot be created, let the error escalate
         try:
             ontology_remote: Ontology = try_network_action(ontology_local.create)
         except BaseError:
             logger.error(f"ERROR while trying to create ontology '{ontology_definition['name']}'.", exc_info=True)
             raise UserError(f"ERROR while trying to create ontology '{ontology_definition['name']}'.") from None
         context.add_context(
             ontology_remote.name,
-            ontology_remote.id + ('#' if not ontology_remote.id.endswith('#') else '')
+            ontology_remote.iri + ("#" if not ontology_remote.iri.endswith("#") else ""),
         )
         last_modification_date = ontology_remote.lastModificationDate
         if verbose:
             print(f"\tCreated ontology '{ontology_definition['name']}'.")
 
         # add the prefixes defined in the JSON file
         for onto_prefix, onto_info in context:
@@ -546,53 +581,53 @@
 
         # add the empty resource classes to the remote ontology
         last_modification_date, remote_res_classes, success = _add_resource_classes_to_remote_ontology(
             ontology_definition=ontology_definition,
             ontology_remote=ontology_remote,
             con=con,
             last_modification_date=last_modification_date,
-            verbose=verbose
+            verbose=verbose,
         )
         if not success:
             overall_success = False
 
         # add the property classes to the remote ontology
         last_modification_date, success = _add_property_classes_to_remote_ontology(
             ontology_definition=ontology_definition,
             ontology_remote=ontology_remote,
             list_root_nodes=list_root_nodes,
             con=con,
             last_modification_date=last_modification_date,
             knora_api_prefix=knora_api_prefix,
-            verbose=verbose
+            verbose=verbose,
         )
         if not success:
             overall_success = False
 
         # Add cardinalities to class
         success = _add_cardinalities_to_resource_classes(
             ontology_definition=ontology_definition,
             ontology_remote=ontology_remote,
             remote_res_classes=remote_res_classes,
             last_modification_date=last_modification_date,
             knora_api_prefix=knora_api_prefix,
-            verbose=verbose
+            verbose=verbose,
         )
         if not success:
             overall_success = False
 
     return overall_success
 
 
 def _add_resource_classes_to_remote_ontology(
     ontology_definition: dict[str, Any],
     ontology_remote: Ontology,
     con: Connection,
     last_modification_date: DateTimeStamp,
-    verbose: bool
+    verbose: bool,
 ) -> tuple[DateTimeStamp, dict[str, ResourceClass], bool]:
     """
     Creates the resource classes (without cardinalities) defined in the "resources" section of an ontology. The
     containing project and the containing ontology must already be existing on the DSP server.
     If an error occurs during creation of a resource class, it is printed out, the process continues, but the success
     status will be false.
 
@@ -616,22 +651,24 @@
     for res_class in sorted_resources:
         super_classes = res_class["super"]
         if isinstance(super_classes, str):
             super_classes = [super_classes]
         res_class_local = ResourceClass(
             con=con,
             context=ontology_remote.context,
-            ontology_id=ontology_remote.id,
+            ontology_id=ontology_remote.iri,
             name=res_class["name"],
             superclasses=super_classes,
             label=LangString(res_class.get("labels")),
-            comment=LangString(res_class.get("comments")) if res_class.get("comments") else None
+            comment=LangString(res_class.get("comments")) if res_class.get("comments") else None,
         )
         try:
-            last_modification_date, res_class_remote = try_network_action(res_class_local.create, last_modification_date)
+            last_modification_date, res_class_remote = try_network_action(
+                res_class_local.create, last_modification_date
+            )
             res_class_remote = cast(ResourceClass, res_class_remote)
             new_res_classes[str(res_class_remote.id)] = res_class_remote
             ontology_remote.lastModificationDate = last_modification_date
             if verbose:
                 print(f"\tCreated resource class '{res_class['name']}'")
         except BaseError:
             print(f"WARNING: Unable to create resource class '{res_class['name']}'.")
@@ -644,15 +681,15 @@
 def _add_property_classes_to_remote_ontology(
     ontology_definition: dict[str, Any],
     ontology_remote: Ontology,
     list_root_nodes: dict[str, Any],
     con: Connection,
     last_modification_date: DateTimeStamp,
     knora_api_prefix: str,
-    verbose: bool
+    verbose: bool,
 ) -> tuple[DateTimeStamp, bool]:
     """
     Creates the property classes defined in the "properties" section of an ontology. The
     containing project and the containing ontology must already be existing on the DSP server.
     If an error occurs during creation of a property class, it is printed out, the process continues, but the success
     status will be false.
 
@@ -668,15 +705,14 @@
     Returns:
         a tuple consisting of the last modification date of the ontology, and the success status
     """
     overall_success = True
     print("\tCreate property classes...")
     sorted_prop_classes = _sort_prop_classes(ontology_definition["properties"], ontology_definition["name"])
     for prop_class in sorted_prop_classes:
-
         # get the super-property/ies, valid forms are:
         #   - "prefix:super-property" : fully qualified name of property in another ontology. The prefix has to be
         #     defined in the prefixes part.
         #   - ":super-property" : super-property defined in current ontology
         #   - "super-property" : super-property defined in the knora-api ontology
         #   - if omitted, "knora-api:hasValue" is assumed
         if prop_class.get("super"):
@@ -691,36 +727,36 @@
             super_props = ["knora-api:hasValue"]
 
         # get the "object", valid forms are:
         #   - "prefix:object_name" : fully qualified object. The prefix has to be defined in the prefixes part.
         #   - ":object_name" : The object is defined in the current ontology.
         #   - "object_name" : The object is defined in "knora-api"
         if ":" in prop_class["object"]:
-            prefix, _object = prop_class["object"].split(':')
+            prefix, _object = prop_class["object"].split(":")
             prop_object = f"{prefix}:{_object}" if prefix else f"{ontology_remote.name}:{_object}"
         else:
             prop_object = knora_api_prefix + prop_class["object"]
 
         gui_attributes = prop_class.get("gui_attributes")
         if gui_attributes and gui_attributes.get("hlist"):
             gui_attributes["hlist"] = "<" + list_root_nodes[gui_attributes["hlist"]]["id"] + ">"
 
         # create the property class
         prop_class_local = PropertyClass(
             con=con,
             context=ontology_remote.context,
             label=LangString(prop_class.get("labels")),
             name=prop_class["name"],
-            ontology_id=ontology_remote.id,
+            ontology_id=ontology_remote.iri,
             superproperties=super_props,
             object=prop_object,
             subject=prop_class.get("subject"),
             gui_element="salsah-gui:" + prop_class["gui_element"],
             gui_attributes=gui_attributes,
-            comment=LangString(prop_class["comments"]) if prop_class.get("comments") else None
+            comment=LangString(prop_class["comments"]) if prop_class.get("comments") else None,
         )
         try:
             last_modification_date, _ = try_network_action(prop_class_local.create, last_modification_date)
             ontology_remote.lastModificationDate = last_modification_date
             if verbose:
                 print(f"\tCreated property class '{prop_class['name']}'")
         except BaseError:
@@ -733,18 +769,18 @@
 
 def _add_cardinalities_to_resource_classes(
     ontology_definition: dict[str, Any],
     ontology_remote: Ontology,
     remote_res_classes: dict[str, ResourceClass],
     last_modification_date: DateTimeStamp,
     knora_api_prefix: str,
-    verbose: bool
+    verbose: bool,
 ) -> bool:
     """
-    Iterates over the resource classes of an ontology of a JSON project definition, and adds the cardinalities to each 
+    Iterates over the resource classes of an ontology of a JSON project definition, and adds the cardinalities to each
     resource class. The resource classes and the properties must already be existing on the DSP server.
     If an error occurs during creation of a cardinality, it is printed out, the process continues, but the success
     status will be false.
 
     Args:
         ontology_definition: the part of the parsed JSON project file that contains the current ontology
         ontology_remote: representation of the current ontology on the DSP server
@@ -758,20 +794,23 @@
     """
     overall_success = True
     print("\tAdd cardinalities to resource classes...")
     switcher = {
         "1": Cardinality.C_1,
         "0-1": Cardinality.C_0_1,
         "0-n": Cardinality.C_0_n,
-        "1-n": Cardinality.C_1_n
+        "1-n": Cardinality.C_1_n,
     }
     for res_class in ontology_definition.get("resources", []):
-        res_class_remote = remote_res_classes.get(ontology_remote.id + "#" + res_class["name"])
+        res_class_remote = remote_res_classes.get(ontology_remote.iri + "#" + res_class["name"])
         if not res_class_remote:
-            print(f"WARNING: Unable to add cardinalities to resource class '{res_class['name']}': This class doesn't exist on the DSP server.")
+            print(
+                f"WARNING: Unable to add cardinalities to resource class '{res_class['name']}': "
+                f"This class doesn't exist on the DSP server."
+            )
             overall_success = False
             continue
         for card_info in res_class.get("cardinalities", []):
             if ":" in card_info["propname"]:
                 prefix, prop = card_info["propname"].split(":")
                 qualified_propname = card_info["propname"] if prefix else f"{ontology_remote.name}:{prop}"
             else:
@@ -779,151 +818,156 @@
 
             try:
                 last_modification_date = try_network_action(
                     res_class_remote.addProperty,
                     property_id=qualified_propname,
                     cardinality=switcher[card_info["cardinality"]],
                     gui_order=card_info.get("gui_order"),
-                    last_modification_date=last_modification_date
+                    last_modification_date=last_modification_date,
                 )
                 if verbose:
                     print(f"\tAdded cardinality '{card_info['propname']}' to resource class '{res_class['name']}'")
             except BaseError:
-                print(f"WARNING: Unable to add cardinality '{qualified_propname}' to resource class {res_class['name']}.")
-                logger.warning(f"Unable to add cardinality '{qualified_propname}' to resource class {res_class['name']}.", exc_info=True)
+                err_msg = f"Unable to add cardinality '{qualified_propname}' to resource class {res_class['name']}."
+                print(f"WARNING: {err_msg}")
+                logger.warning(err_msg, exc_info=True)
                 overall_success = False
 
             ontology_remote.lastModificationDate = last_modification_date
 
     return overall_success
 
 
 def create_project(
     project_file_as_path_or_parsed: Union[str, Path, dict[str, Any]],
     server: str,
     user_mail: str,
     password: str,
     verbose: bool,
-    dump: bool
+    dump: bool,
 ) -> bool:
     """
-    Creates a project from a JSON project file on a DSP server. 
-    A project must contain at least one ontology, 
+    Creates a project from a JSON project file on a DSP server.
+    A project must contain at least one ontology,
     and it may contain lists, users, and groups.
-    Severe errors lead to a BaseError, 
+    Severe errors lead to a BaseError,
     while other errors are printed without interrupting the process.
 
     Args:
         project_file_as_path_or_parsed: path to the JSON project definition, or parsed JSON object
         server: the URL of the DSP server on which the project should be created
         user_mail: a username (e-mail) who has the permission to create a project
         password: the user's password
         verbose: prints more information if set to True
         dump: dumps test files (JSON) for DSP API requests if set to True
 
     Raises:
-        UserError: 
+        UserError:
            - if the project cannot be created
            - if the login fails
            - if an ontology cannot be created
-        BaseError: 
+        BaseError:
            - if the input is invalid
            - if an Excel file referenced in the "lists" section cannot be expanded
            - if the validation doesn't pass
 
     Returns:
         True if everything went smoothly, False if a warning or error occurred
     """
 
     knora_api_prefix = "knora-api:"
     overall_success = True
 
     project_definition = parse_json_input(project_file_as_path_or_parsed=project_file_as_path_or_parsed)
-    proj_shortname = project_definition['project']['shortname']
-    proj_shortcode = project_definition['project']['shortcode']
+    proj_shortname = project_definition["project"]["shortname"]
+    proj_shortcode = project_definition["project"]["shortcode"]
     context = Context(project_definition.get("prefixes", {}))
 
     # expand the Excel files referenced in the "lists" section of the project (if any), and add them to the project
     new_lists = expand_lists_from_excel(project_definition.get("project", {}).get("lists", []))
     if new_lists:
         project_definition["project"]["lists"] = new_lists
 
     # validate against JSON schema
     validate_project(project_definition, expand_lists=False)
-    print('\tJSON project file is syntactically correct and passed validation.')
+    print("\tJSON project file is syntactically correct and passed validation.")
     print(f"Create project '{proj_shortname}' ({proj_shortcode})...")
 
     # establish connection to DSP server
     con = login(server=server, user=user_mail, password=password)
     if dump:
         con.start_logging()
 
     # create project on DSP server
     project_remote, success = _create_project_on_server(
         project_definition=project_definition,
         con=con,
-        verbose=verbose
+        verbose=verbose,
     )
     if not success:
         overall_success = False
 
     # create the lists
     list_root_nodes: dict[str, Any] = {}
     if project_definition["project"].get("lists"):
         print("Create lists...")
         list_root_nodes, success = create_lists_on_server(
             lists_to_create=project_definition["project"]["lists"],
             con=con,
-            project_remote=project_remote
+            project_remote=project_remote,
         )
         if not success:
             overall_success = False
 
     # create the groups
     current_project_groups: dict[str, Group] = {}
     if project_definition["project"].get("groups"):
         print("Create groups...")
         current_project_groups, success = _create_groups(
             con=con,
             groups=project_definition["project"]["groups"],
-            project=project_remote
+            project=project_remote,
         )
         if not success:
             overall_success = False
 
     # create or update the users
     if project_definition["project"].get("users"):
         print("Create users...")
         success = _create_users(
             con=con,
             users_section=project_definition["project"]["users"],
             current_project_groups=current_project_groups,
             current_project=project_remote,
-            verbose=verbose
+            verbose=verbose,
         )
         if not success:
             overall_success = False
 
     # create the ontologies
     success = _create_ontologies(
         con=con,
         context=context,
         knora_api_prefix=knora_api_prefix,
         list_root_nodes=list_root_nodes,
         project_definition=project_definition,
         project_remote=project_remote,
-        verbose=verbose
+        verbose=verbose,
     )
     if not success:
         overall_success = False
 
     # final steps
     if overall_success:
-        print("========================================================\n",
-              f"Successfully created project '{proj_shortname}' ({proj_shortcode}) with all its ontologies. "
-              f"There were no problems during the creation process.")
+        print(
+            "========================================================\n",
+            f"Successfully created project '{proj_shortname}' ({proj_shortcode}) with all its ontologies. "
+            f"There were no problems during the creation process.",
+        )
     else:
-        print("========================================================\n",
-              f"WARNING: The project '{proj_shortname}' ({proj_shortcode}) with its ontologies could be created, but during the creation process, "
-              f"some problems occurred. Please carefully check the console output.")
+        print(
+            "========================================================\n",
+            f"WARNING: The project '{proj_shortname}' ({proj_shortcode}) with its ontologies could be created, "
+            f"but during the creation process, some problems occurred. Please carefully check the console output.",
+        )
 
     return overall_success
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/project_create_lists.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 logger = get_logger(__name__)
 
 
 def _create_list_node(
     con: Connection,
     project: Project,
     node: dict[str, Any],
-    parent_node: Optional[ListNode] = None
+    parent_node: Optional[ListNode] = None,
 ) -> tuple[dict[str, Any], bool]:
     """
     Creates a list node on the DSP server, recursively scanning through all its subnodes, creating them as well.
     If a node cannot be created, an error message is printed, but the process continues.
 
     Args:
         con: connection to the DSP server
         project: project that holds the list where this node should be added to
         node: the node to be created
         parent_node: parent node of the node to be created (optional)
 
     Returns:
-        Returns a tuple consisting of a dict and a bool. 
+        Returns a tuple consisting of a dict and a bool.
         The dict contains the IRIs of the created list nodes,
         nested according to their hierarchy structure,
         i.e. ``{nodename: {"id": IRI, "nodes": {...}}}``.
-        The bool is True if all nodes could be created, 
+        The bool is True if all nodes could be created,
         False if any node could not be created.
     """
-    new_node = ListNode(
+    new_node: ListNode = ListNode(
         con=con,
         project=project,
         label=node["labels"],
         comments=node.get("comments"),
         name=node["name"],
-        parent=parent_node
+        parent=parent_node,
     )
     try:
         new_node = try_network_action(new_node.create)
     except BaseError:
         print(f"WARNING: Cannot create list node '{node['name']}'.")
         logger.warning("Cannot create list node '{node['name']}'.", exc_info=True)
         return {}, False
@@ -56,23 +56,27 @@
         overall_success = True
         subnode_list = []
         for subnode in node["nodes"]:
             created_subnode, success = _create_list_node(con=con, project=project, node=subnode, parent_node=new_node)
             subnode_list.append(created_subnode)
             if not success:
                 overall_success = False
-        return {new_node.name: {"id": new_node.id, "nodes": subnode_list}}, overall_success  # type: ignore
+        if not new_node.name:
+            raise BaseError(f"Node {new_node} has no name.")
+        return {new_node.name: {"id": new_node.iri, "nodes": subnode_list}}, overall_success
     else:
-        return {new_node.name: {"id": new_node.id}}, True  # type: ignore
+        if not new_node.name:
+            raise BaseError(f"Node {new_node} has no name.")
+        return {new_node.name: {"id": new_node.iri}}, True
 
 
 def create_lists_on_server(
     lists_to_create: list[dict[str, Any]],
     con: Connection,
-    project_remote: Project
+    project_remote: Project,
 ) -> tuple[dict[str, Any], bool]:
     """
     Creates the "lists" section of a JSON project definition on a DSP server.
     If a list with the same name is already existing in this project on the DSP server, this list is skipped.
     If a node or an entire list cannot be created, an error message is printed, but the process continues.
 
     Args:
@@ -88,25 +92,32 @@
 
     # retrieve existing lists
     try:
         existing_lists: list[ListNode] = try_network_action(
             lambda: ListNode.getAllLists(con=con, project_iri=project_remote.id)
         )
     except BaseError:
-        print("WARNING: Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing.")
-        logger.warning("Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing.", exc_info=True)
+        err_msg = "Unable to retrieve existing lists on DSP server. Cannot check if your lists are already existing."
+        print("WARNING: " + err_msg)
+        logger.warning(err_msg, exc_info=True)
         existing_lists = []
         overall_success = False
 
     current_project_lists: dict[str, Any] = {}
     for new_list in lists_to_create:
         # if list exists already, add it to "current_project_lists" (for later usage), then skip it
         existing_list = [x for x in existing_lists if x.project == project_remote.id and x.name == new_list["name"]]
         if existing_list:
-            current_project_lists[existing_list[0].name] = {"id": existing_list[0].id, "nodes": new_list["nodes"]}  # type: ignore
+            existing_list_name = existing_list[0].name
+            if not existing_list_name:
+                raise BaseError(f"Node {existing_list[0]} has no name.")
+            current_project_lists[existing_list_name] = {
+                "id": existing_list[0].iri,
+                "nodes": new_list["nodes"],
+            }
             print(f"\tWARNING: List '{new_list['name']}' already exists on the DSP server. Skipping...")
             overall_success = False
             continue
 
         created_list, success = _create_list_node(con=con, project=project_remote, node=new_list)
         current_project_lists.update(created_list)
         if not success:
@@ -117,21 +128,21 @@
 
 
 def create_lists(
     project_file_as_path_or_parsed: Union[str, dict[str, Any]],
     server: str,
     user: str,
     password: str,
-    dump: bool = False
+    dump: bool = False,
 ) -> tuple[dict[str, Any], bool]:
     """
-    This method accepts a JSON project definition, 
+    This method accepts a JSON project definition,
     expands the Excel sheets referenced in its "lists" section,
     connects to a DSP server,
-    and uploads the "lists" section to the server. 
+    and uploads the "lists" section to the server.
 
     The project must already exist on the DSP server.
     If a list with the same name is already existing in this project on the DSP server, this list is skipped.
 
     Args:
         project_file_as_path_or_parsed: path to the JSON project definition, or parsed JSON object
         server: URL of the DSP server
@@ -139,54 +150,59 @@
         password: Password of the user
         dump: if True, the request is dumped as JSON (used for testing)
 
     Raises:
         UserError:
            - if the project cannot be read from the server
            - if the connection to the DSP server cannot be established
-        BaseError: 
+        BaseError:
            - if the input is invalid
            - if a problem occurred while trying to expand the Excel files
            - if the JSON file is invalid according to the schema
 
     Returns:
-        Returns a tuple consisting of a dict and a bool. 
+        Returns a tuple consisting of a dict and a bool.
         The dict contains the IRIs of the created list nodes,
         nested according to their hierarchy structure,
         i.e. ``{nodename: {"id": IRI, "nodes": {...}}}``.
-        If there are no lists in the project definition, 
-        an empty dictionary is returned. 
-        The bool indicates if everything went smoothly during the process. 
-        If a warning or error occurred (e.g. one of the lists already exists, 
-        or one of the nodes could not be created), 
+        If there are no lists in the project definition,
+        an empty dictionary is returned.
+        The bool indicates if everything went smoothly during the process.
+        If a warning or error occurred (e.g. one of the lists already exists,
+        or one of the nodes could not be created),
         it is False.
     """
     overall_success = True
 
     project_definition = parse_json_input(project_file_as_path_or_parsed=project_file_as_path_or_parsed)
     if not project_definition.get("project", {}).get("lists"):
         return {}, True
     lists_to_create = expand_lists_from_excel(project_definition["project"]["lists"])
     project_definition["project"]["lists"] = lists_to_create
     validate_project(project_definition, expand_lists=False)
-    print('JSON project file is syntactically correct and passed validation.')
+    print("JSON project file is syntactically correct and passed validation.")
 
     # connect to the DSP server
     con = login(server, user, password)
     if dump:
         con.start_logging()
 
     # retrieve the project
-    project_local = Project(con=con, shortcode=project_definition["project"]["shortcode"])
+    shortcode = project_definition["project"]["shortcode"]
+    project_local = Project(con=con, shortcode=shortcode)
     try:
         project_remote = try_network_action(project_local.read)
     except BaseError:
-        err_msg = f"Unable to create the lists: The project {project_definition['project']['shortcode']} cannot be found on the DSP server."
+        err_msg = f"Unable to create the lists: The project {shortcode} cannot be found on the DSP server."
         logger.error(err_msg, exc_info=True)
         raise UserError(err_msg) from None
 
     # create new lists
-    current_project_lists, success = create_lists_on_server(lists_to_create=lists_to_create, con=con, project_remote=project_remote)
+    current_project_lists, success = create_lists_on_server(
+        lists_to_create=lists_to_create,
+        con=con,
+        project_remote=project_remote,
+    )
     if not success:
         overall_success = False
 
     return current_project_lists, overall_success
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/project_get.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/project_get.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from dsp_tools.models.group import Group
 from dsp_tools.models.listnode import ListNode
 from dsp_tools.models.ontology import Ontology
 from dsp_tools.models.project import Project
 from dsp_tools.models.user import User
 
 
-def get_project(project_identifier: str, outfile_path: str, server: str, user: str, password: str, verbose: bool) -> bool:
+def get_project(
+    project_identifier: str,
+    outfile_path: str,
+    server: str,
+    user: str,
+    password: str,
+    verbose: bool,
+) -> bool:
     """
     This function writes a project from a DSP server into a JSON file.
 
     Args:
         project_identifier : the project identifier, either shortcode, shortname or IRI of the project
         outfile_path : the output file the JSON content should be written to
         server : the DSP server where the data should be read from
@@ -37,15 +44,17 @@
     if re.match("[0-9A-F]{4}", project_identifier):  # shortcode
         project = Project(con=con, shortcode=project_identifier)
     elif re.match("^[\\w-]+$", project_identifier):  # shortname
         project = Project(con=con, shortname=project_identifier.lower())
     elif re.match("^(http)s?://([\\w\\.\\-~]+:?\\d{,4})(/[\\w\\-~]+)+$", project_identifier):  # iri
         project = Project(con=con, shortname=project_identifier)
     else:
-        raise BaseError(f"ERROR Invalid project identifier '{project_identifier}'. Use the project's shortcode, shortname or IRI.")
+        raise BaseError(
+            f"ERROR Invalid project identifier '{project_identifier}'. Use the project's shortcode, shortname or IRI."
+        )
 
     project = project.read()
     project_obj = project.createDefinitionFileObj()
 
     # get groups
     if verbose:
         print("Getting groups...")
@@ -65,15 +74,15 @@
     users = User.getAllUsersForProject(con=con, proj_shortcode=str(project.shortcode))
     if users:
         for usr in users:
             users_obj.append(
                 usr.createDefinitionFileObj(
                     con=con,
                     proj_shortname=str(project.shortname),
-                    proj_iri=str(project.id)
+                    proj_iri=str(project.id),
                 )
             )
             if verbose:
                 print(f"\tGot user '{usr.username}'")
         project_obj["users"] = users_obj
 
     # get the lists
@@ -91,28 +100,29 @@
 
     # get the ontologies
     if verbose:
         print("Getting ontologies...")
     project_obj["ontologies"] = []
     prefixes: dict[str, str] = dict()
     ontologies = Ontology.getProjectOntologies(con, str(project.id))
-    ontology_ids = [onto.id for onto in ontologies]
+    ontology_ids = [onto.iri for onto in ontologies]
     for ontology_id in ontology_ids:
         onto_url_parts = ontology_id.split("/")  # an id has the form http://0.0.0.0:3333/ontology/4123/testonto/v2
         name = onto_url_parts[len(onto_url_parts) - 2]
         shortcode = onto_url_parts[len(onto_url_parts) - 3]
         ontology = Ontology.getOntologyFromServer(con=con, shortcode=shortcode, name=name)
         project_obj["ontologies"].append(ontology.createDefinitionFileObj())
         prefixes.update(ontology.context.get_externals_used())
         if verbose:
             print(f"\tGot ontology '{name}'")
 
+    schema = "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/project.json"
     outfile_content = {
         "prefixes": prefixes,
-        "$schema": "https://raw.githubusercontent.com/dasch-swiss/dsp-tools/main/src/dsp_tools/resources/schema/project.json",
-        "project": project_obj
+        "$schema": schema,
+        "project": project_obj,
     }
 
-    with open(outfile_path, 'w', encoding='utf8') as f:
+    with open(outfile_path, "w", encoding="utf8") as f:
         json.dump(outfile_content, f, indent=4, ensure_ascii=False)
 
     return True
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/project_validate.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/project_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,24 @@
     propnames_duplicates: dict[str, set[str]] = dict()
     for onto in project_definition["project"]["ontologies"]:
         resnames = [r["name"] for r in onto["resources"]]
         if len(set(resnames)) != len(resnames):
             for elem in resnames:
                 if resnames.count(elem) > 1:
                     if not resnames_duplicates.get(onto["name"]):
-                        resnames_duplicates[onto["name"]] = {elem, }
+                        resnames_duplicates[onto["name"]] = {elem}
                     else:
                         resnames_duplicates[onto["name"]].add(elem)
 
         propnames = [p["name"] for p in onto["properties"]]
         if len(set(propnames)) != len(propnames):
             for elem in propnames:
                 if propnames.count(elem) > 1:
                     if not propnames_duplicates.get(onto["name"]):
-                        propnames_duplicates[onto["name"]] = {elem, }
+                        propnames_duplicates[onto["name"]] = {elem}
                     else:
                         propnames_duplicates[onto["name"]].add(elem)
 
     if not resnames_duplicates and not propnames_duplicates:
         return True
 
     err_msg = "Resource names and property names must be unique inside every ontology.\n"
@@ -77,15 +77,15 @@
         True if the superresource are valid
     """
     errors: dict[str, list[str]] = dict()
     for onto in project_definition["project"]["ontologies"]:
         ontoname = onto["name"]
         resnames = [r["name"] for r in onto["resources"]]
         for res in onto["resources"]:
-            supers = res["super"] if isinstance(res["super"], list) else [res["super"],]
+            supers = res["super"] if isinstance(res["super"], list) else [res["super"]]
             # form of supers:
             #  - Resource      # DSP base resource
             #  - other:res     # other onto
             #  - same:res      # same onto
             #  - :res          # same onto (short form)
 
             # filter out DSP base resources
@@ -153,15 +153,15 @@
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
 def _check_for_undefined_cardinalities(project_definition: dict[str, Any]) -> bool:
     """
-    Check if the propnames that are used in the cardinalities of each resource are defined in the "properties" 
+    Check if the propnames that are used in the cardinalities of each resource are defined in the "properties"
     section. (DSP base properties and properties from other ontologies are not considered.)
 
     Args:
         project_definition: parsed JSON project definition
 
     Raises:
         BaseError: detailed error message if a cardinality is used that is not defined
@@ -199,68 +199,76 @@
         err_msg += "\n".join(f" - {loc}: {invalids}" for loc, invalids in errors.items())
         raise BaseError(err_msg)
     return True
 
 
 def validate_project(
     input_file_or_json: Union[dict[str, Any], str],
-    expand_lists: bool = True
+    expand_lists: bool = True,
 ) -> bool:
     """
-    Validates a JSON project definition file. 
+    Validates a JSON project definition file.
 
     First, the Excel file references in the "lists" section are expanded
-    (unless this behaviour is disabled). 
+    (unless this behaviour is disabled).
 
-    Then, the project is validated against the JSON schema. 
+    Then, the project is validated against the JSON schema.
 
     Next, some checks are performed that are too complex for JSON schema.
 
     At last, a check is performed
-    if this project's ontologies contain properties derived from hasLinkTo 
+    if this project's ontologies contain properties derived from hasLinkTo
     that form a circular reference.
-    If so, these properties must have the cardinality 0-1 or 0-n, 
-    because during the xmlupload process, 
+    If so, these properties must have the cardinality 0-1 or 0-n,
+    because during the xmlupload process,
     these values are temporarily removed.
 
     Args:
         input_file_or_json: the project to be validated, can either be a file path or a parsed JSON file
         expand_lists: if True, the Excel file references in the "lists" section will be expanded
 
     Raises:
         BaseError: detailed error report if the validation doesn't pass
 
     Returns:
-        True if the project passed validation. 
+        True if the project passed validation.
     """
 
     # parse input
     if isinstance(input_file_or_json, dict) and "project" in input_file_or_json:
         project_definition = input_file_or_json
-    elif isinstance(input_file_or_json, str) and os.path.isfile(input_file_or_json) and regex.search(r"\.json$", input_file_or_json):
+    elif (
+        isinstance(input_file_or_json, str)
+        and os.path.isfile(input_file_or_json)
+        and regex.search(r"\.json$", input_file_or_json)
+    ):
         with open(input_file_or_json, encoding="utf-8") as f:
             project_definition = json.load(f)
     else:
         raise BaseError(f"Input '{input_file_or_json}' is neither a file path nor a JSON object.")
 
-    # expand all lists referenced in the "lists" section of the project definition, and add them to the project definition
+    # expand all lists referenced in the "lists" section of the project definition,
+    # and add them to the project definition
     if expand_lists:
         new_lists = expand_lists_from_excel(project_definition["project"].get("lists", []))
         if new_lists:
             project_definition["project"]["lists"] = new_lists
 
     # validate the project definition against the schema
-    with importlib.resources.files("dsp_tools").joinpath("resources/schema/project.json").open(encoding="utf-8") as schema_file:
+    with importlib.resources.files("dsp_tools").joinpath("resources/schema/project.json").open(
+        encoding="utf-8"
+    ) as schema_file:
         project_schema = json.load(schema_file)
     try:
         jsonschema.validate(instance=project_definition, schema=project_schema)
     except jsonschema.ValidationError as err:
-        raise BaseError(f"The JSON project file cannot be created due to the following validation error: {err.message}.\n"
-                        f"The error occurred at {err.json_path}:\n"
-                        f"{err.instance}") from None
+        raise BaseError(
+            f"The JSON project file cannot be created due to the following validation error: {err.message}.\n"
+            f"The error occurred at {err.json_path}:\n{err.instance}"
+        ) from None
 
     # make some checks that are too complex for JSON schema
     _check_for_undefined_super_property(project_definition)
     _check_for_undefined_super_resource(project_definition)
     _check_for_undefined_cardinalities(project_definition)
     _check_for_duplicate_names(project_definition)
 
@@ -286,21 +294,22 @@
 
     link_properties = _collect_link_properties(project_definition)
     errors = _identify_problematic_cardinalities(project_definition, link_properties)
 
     if len(errors) == 0:
         return True
     else:
-        error_message = \
-            "ERROR: Your ontology contains properties derived from 'hasLinkTo' that allow circular references " \
-            "between resources. This is not a problem in itself, but if you try to upload data that actually " \
-            "contains circular references, these 'hasLinkTo' properties will be temporarily removed from the " \
-            "affected resources. Therefore, it is necessary that all involved 'hasLinkTo' properties have a " \
-            "cardinality of 0-1 or 0-n. \n" \
+        error_message = (
+            "ERROR: Your ontology contains properties derived from 'hasLinkTo' that allow circular references "
+            "between resources. This is not a problem in itself, but if you try to upload data that actually "
+            "contains circular references, these 'hasLinkTo' properties will be temporarily removed from the "
+            "affected resources. Therefore, it is necessary that all involved 'hasLinkTo' properties have a "
+            "cardinality of 0-1 or 0-n. \n"
             "Please make sure that the following properties have a cardinality of 0-1 or 0-n:"
+        )
         for error in errors:
             error_message = f"{error_message}\n\t- Resource {error[0]}, property {error[1]}"
         raise BaseError(error_message)
 
 
 def _collect_link_properties(project_definition: dict[Any, Any]) -> dict[str, list[str]]:
     """
@@ -316,17 +325,19 @@
     hasLinkTo_props = {"hasLinkTo", "isPartOf", "isRegionOf", "isAnnotationOf"}
     link_properties: dict[str, list[str]] = dict()
     for index, onto in enumerate(ontos):
         hasLinkTo_matches = list()
         # look for child-properties down to 5 inheritance levels that are derived from hasLinkTo-properties
         for _ in range(5):
             for hasLinkTo_prop in hasLinkTo_props:
-                hasLinkTo_matches.extend(jsonpath_ng.ext.parse(
-                    f"$.project.ontologies[{index}].properties[?super[*] == {hasLinkTo_prop}]"
-                ).find(project_definition))
+                hasLinkTo_matches.extend(
+                    jsonpath_ng.ext.parse(
+                        f"$.project.ontologies[{index}].properties[?super[*] == {hasLinkTo_prop}]"
+                    ).find(project_definition)
+                )
             # make the children from this iteration to the parents of the next iteration
             hasLinkTo_props = {x.value["name"] for x in hasLinkTo_matches}
         prop_obj_pair: dict[str, list[str]] = dict()
         for match in hasLinkTo_matches:
             prop = onto["name"] + ":" + match.value["name"]
             target = match.value["object"]
             if target != "Resource":
@@ -346,22 +357,23 @@
             link_properties[prop] = all_res_names
 
     return link_properties
 
 
 def _identify_problematic_cardinalities(
     project_definition: dict[Any, Any],
-    link_properties: dict[str, list[str]]
+    link_properties: dict[str, list[str]],
 ) -> list[tuple[str, str]]:
     """
     Make an error list with all cardinalities that are part of a circle but have a cardinality of "1" or "1-n".
 
     Args:
         project_definition: parsed JSON file
-        link_properties: mapping of hasLinkTo-properties to classes they point to, e.g. {"rosetta:hasImage2D": ["rosetta:Image2D"], ...}
+        link_properties: mapping of hasLinkTo-properties to classes they point to,
+            e.g. {"rosetta:hasImage2D": ["rosetta:Image2D"], ...}
 
     Returns:
         a (possibly empty) list of (resource, problematic_cardinality) tuples
     """
     # make 2 dicts of the following form:
     # dependencies = {"rosetta:Text": {"rosetta:hasImage2D": ["rosetta:Image2D"], ...}}
     # cardinalities = {"rosetta:Text": {"rosetta:hasImage2D": "0-1", ...}}
@@ -399,15 +411,15 @@
                 graph.add_edge(start, target, edge)
 
     # find elements of circles that have a cardinality of "1" or "1-n"
     errors: set[tuple[str, str]] = set()
     circles = list(nx.algorithms.cycles.simple_cycles(graph))
     for circle in circles:
         for index, resource in enumerate(circle):
-            target = circle[(index+1) % len(circle)]
+            target = circle[(index + 1) % len(circle)]
             prop = ""
             for _property, targets in dependencies[resource].items():
                 if target in targets:
                     prop = _property
             if cardinalities[resource].get(prop) not in ["0-1", "0-n"]:
                 errors.add((resource, prop))
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/rosetta.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/rosetta.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,31 +27,34 @@
             is_rosetta_up_to_date = False
     else:
         is_rosetta_up_to_date = False
 
     return is_rosetta_up_to_date
 
 
-def _clone_repo(rosetta_folder: Path, enclosing_folder: Path) -> None:
+def _clone_repo(
+    rosetta_folder: Path,
+    enclosing_folder: Path,
+) -> None:
     """
     Clones the rosetta repo into the enclosing folder.
 
     Args:
-        rosetta_folder: path to the (not yet existing) clone 
+        rosetta_folder: path to the (not yet existing) clone
         enclosing_folder: path to the (existing) destination where rosetta should be cloned into
 
     Raises:
         UserError: If rosetta cannot be cloned
     """
     print(f"Clone into {rosetta_folder}...")
     completed_process = subprocess.run(
         "git clone https://github.com/dasch-swiss/082E-rosetta-scripts.git",
         shell=True,
         cwd=enclosing_folder,
-        check=False
+        check=False,
     )
     if not completed_process or completed_process.returncode != 0:
         raise UserError("There was a problem while cloning the rosetta test project")
 
 
 def _create_json(rosetta_folder: Path) -> bool:
     """
@@ -61,20 +64,20 @@
         rosetta_folder: path to the clone
 
     Returns:
         True if the project could be created without problems, False if something went wrong during the creation process
     """
     print("Execute 'dsp-tools create rosetta.json'...")
     success = create_project(
-        project_file_as_path_or_parsed=rosetta_folder/"rosetta.json",
+        project_file_as_path_or_parsed=rosetta_folder / "rosetta.json",
         server="http://0.0.0.0:3333",
         user_mail="root@example.com",
         password="test",
         verbose=False,
-        dump=False
+        dump=False,
     )
     return success
 
 
 def _upload_xml(rosetta_folder: Path) -> bool:
     """
     Uplaod the rosetta data on the locally running DSP stack.
@@ -83,24 +86,24 @@
         rosetta_folder: path to the clone
 
     Returns:
         True if all data could be uploaded without problems, False if something went wrong during the upload process
     """
     print("Execute 'dsp-tools xmlupload rosetta.xml'...")
     success = xml_upload(
-        input_file=rosetta_folder/"rosetta.xml",
+        input_file=rosetta_folder / "rosetta.xml",
         server="http://0.0.0.0:3333",
         user="root@example.com",
         password="test",
         imgdir=str(rosetta_folder),
         sipi="http://0.0.0.0:1024",
         verbose=False,
         incremental=False,
         save_metrics=False,
-        preprocessing_done=False
+        preprocessing_done=False,
     )
     return success
 
 
 def upload_rosetta() -> bool:
     """
     This method clones https://github.com/dasch-swiss/082E-rosetta-scripts
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/shared.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.propertyelement import PropertyElement
 from dsp_tools.utils.logging import get_logger
 
 logger = get_logger(__name__)
 
 
-def login(server: str, user: str, password: str) -> Connection:
+def login(
+    server: str,
+    user: str,
+    password: str,
+) -> Connection:
     """
-    Creates a connection, 
+    Creates a connection,
     makes a login (handling temporary network interruptions),
     and returns the active connection.
 
     Args:
         server: URL of the DSP server to connect to
         user: Username (e-mail)
         password: Password of the user
@@ -47,20 +51,20 @@
         raise UserError("Cannot login to DSP server") from None
     return con
 
 
 def try_network_action(
     action: Callable[..., Any],
     *args: Any,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> Any:
     """
-    Helper method that tries 7 times to execute an action. 
-    If a ConnectionError, a requests.exceptions.RequestException, or a non-permanent BaseError occors, 
-    it waits and retries. 
+    Helper method that tries 7 times to execute an action.
+    If a ConnectionError, a requests.exceptions.RequestException, or a non-permanent BaseError occors,
+    it waits and retries.
     The waiting times are 1, 2, 4, 8, 16, 32, 64 seconds.
     If another exception occurs, it escalates.
 
     Args:
         action: a lambda with the code to be executed, or a function
         args: positional arguments for the action
         kwargs: keyword arguments for the action
@@ -81,25 +85,26 @@
             elif args and kwargs:
                 return action(*args, **kwargs)
             else:
                 return action()
         except (ConnectionError, RequestException):
             print(f"{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...")
             logger.error(f"Try reconnecting to DSP server, next attempt in {2 ** i} seconds...", exc_info=True)
-            time.sleep(2 ** i)
+            time.sleep(2**i)
             continue
         except BaseError as err:
             in_500_range = False
             if err.status_code:
                 in_500_range = 500 <= err.status_code < 600
             try_again_later = "try again later" in err.message
             if try_again_later or in_500_range:
-                print(f"{datetime.now().isoformat()}: Try reconnecting to DSP server, next attempt in {2 ** i} seconds...")
-                logger.error(f"Try reconnecting to DSP server, next attempt in {2 ** i} seconds...", exc_info=True)
-                time.sleep(2 ** i)
+                msg = f"Try reconnecting to DSP server, next attempt in {2 ** i} seconds..."
+                print(f"{datetime.now().isoformat()}: {msg}")
+                logger.error(msg, exc_info=True)
+                time.sleep(2**i)
                 continue
             else:
                 raise err
 
     logger.error("Permanently unable to execute the network action. See logs for more details.")
     raise BaseError("Permanently unable to execute the network action. See logs for more details.")
 
@@ -113,15 +118,17 @@
 
     Raises:
         UserError with a detailed error log if the XML file is invalid
 
     Returns:
         True if the XML file is valid
     """
-    with importlib.resources.files("dsp_tools").joinpath("resources/schema/data.xsd").open(encoding="utf-8") as schema_file:
+    with importlib.resources.files("dsp_tools").joinpath("resources/schema/data.xsd").open(
+        encoding="utf-8"
+    ) as schema_file:
         xmlschema = etree.XMLSchema(etree.parse(schema_file))
     if isinstance(input_file, (str, Path)):
         try:
             doc = etree.parse(source=input_file)
         except etree.XMLSyntaxError as err:
             logger.error(f"The XML file contains the following syntax error: {err.msg}", exc_info=True)
             raise UserError(f"The XML file contains the following syntax error: {err.msg}") from None
@@ -143,22 +150,22 @@
     print("The XML file is syntactically correct and passed validation.")
     return True
 
 
 def _validate_xml_tags_in_text_properties(doc: Union[etree._ElementTree[etree._Element], etree._Element]) -> bool:
     """
     Makes sure that there are no XML tags in simple texts.
-    This can only be done with a regex, 
-    because even if the simple text contains some XML tags, 
+    This can only be done with a regex,
+    because even if the simple text contains some XML tags,
     the simple text itself is not valid XML that could be parsed.
-    The extra challenge is that lxml transforms 
-    "pebble (&lt;2cm) and boulder (&gt;20cm)" into 
-    "pebble (<2cm) and boulder (>20cm)" 
+    The extra challenge is that lxml transforms
+    "pebble (&lt;2cm) and boulder (&gt;20cm)" into
+    "pebble (<2cm) and boulder (>20cm)"
     (but only if &gt; follows &lt;).
-    This forces us to write a regex that carefully distinguishes 
+    This forces us to write a regex that carefully distinguishes
     between a real tag (which is not allowed) and a false-positive-tag.
 
     Args:
         doc: parsed XML file
 
     Raises:
         UserError: if there is an XML tag in one of the simple texts
@@ -173,33 +180,43 @@
         if not isinstance(elem, (etree._Comment, etree._ProcessingInstruction)):
             elem.tag = etree.QName(elem).localname
 
     # then: make the test
     resources_with_illegal_xml_tags = list()
     for text in doc_without_namespace.findall(path="resource/text-prop/text"):
         if text.attrib["encoding"] == "utf8":
-            if regex.search(r'<([a-zA-Z/"]+|[^\s0-9].*[^\s0-9])>', str(text.text)) or len(list(text.iterchildren())) > 0:
+            if (
+                regex.search(r'<([a-zA-Z/"]+|[^\s0-9].*[^\s0-9])>', str(text.text))
+                or len(list(text.iterchildren())) > 0
+            ):
                 sourceline = f" line {text.sourceline}: " if text.sourceline else " "
-                propname = text.getparent().attrib["name"]           # type: ignore
+                propname = text.getparent().attrib["name"]  # type: ignore
                 resname = text.getparent().getparent().attrib["id"]  # type: ignore
                 resources_with_illegal_xml_tags.append(f" -{sourceline}resource '{resname}', property '{propname}'")
     if resources_with_illegal_xml_tags:
-        err_msg = "XML-tags are not allowed in text properties with encoding=utf8. The following resources of your XML file violate this rule:\n"
+        err_msg = (
+            "XML-tags are not allowed in text properties with encoding=utf8. "
+            "The following resources of your XML file violate this rule:\n"
+        )
         err_msg += "\n".join(resources_with_illegal_xml_tags)
         logger.error(err_msg, exc_info=True)
         raise UserError(err_msg)
 
     return True
 
 
-def prepare_dataframe(df: pd.DataFrame, required_columns: list[str], location_of_sheet: str) -> pd.DataFrame:
+def prepare_dataframe(
+    df: pd.DataFrame,
+    required_columns: list[str],
+    location_of_sheet: str,
+) -> pd.DataFrame:
     """
-    Takes a pandas DataFrame, 
+    Takes a pandas DataFrame,
     strips the column headers from whitespaces and transforms them to lowercase,
-    strips every cell from whitespaces and inserts "" if there is no string in it, 
+    strips every cell from whitespaces and inserts "" if there is no string in it,
     and deletes the rows that don't have a value in one of the required cells.
 
     Args:
         df: pandas DataFrame
         required_columns: headers of the columns where a value is required
         location_of_sheet: for better error messages, provide this information of the caller
 
@@ -281,52 +298,47 @@
         >>> check_notna("-")    == False
         >>> check_notna(" ")    == False
     """
 
     if isinstance(value, PropertyElement):
         value = value.value
 
-    if any([
-        isinstance(value, int),
-        isinstance(value, float) and pd.notna(value),   # necessary because isinstance(np.nan, float)
-        isinstance(value, bool)
-    ]):
+    if isinstance(value, (bool, int)) or (
+        isinstance(value, float) and pd.notna(value)
+    ):  # necessary because isinstance(np.nan, float)
         return True
     elif isinstance(value, str):
-        return all([
-            regex.search(r"[\p{L}\d_!?]", value, flags=regex.UNICODE),
-            not bool(regex.search(r"^(none|<NA>|-|n/a)$", value, flags=regex.IGNORECASE))
-        ])
+        return bool(regex.search(r"[\p{L}\d_!?]", value, flags=regex.UNICODE)) and not bool(
+            regex.search(r"^(none|<NA>|-|n/a)$", value, flags=regex.IGNORECASE)
+        )
     else:
         return False
 
 
 def parse_json_input(project_file_as_path_or_parsed: Union[str, Path, dict[str, Any]]) -> dict[str, Any]:
     """
-    Check the input for a method that expects a JSON project definition, either as file path or as parsed JSON object: 
+    Check the input for a method that expects a JSON project definition, either as file path or as parsed JSON object:
     If it is parsed already, return it unchanged.
     If the input is a file path, parse it.
 
     Args:
         project_file_as_path_or_parsed: path to the JSON project definition, or parsed JSON object
 
     Raises:
         BaseError: if the input is invalid
 
     Returns:
         the parsed JSON object
     """
     if isinstance(project_file_as_path_or_parsed, dict):
         project_definition: dict[str, Any] = project_file_as_path_or_parsed
-    elif all([
-        isinstance(project_file_as_path_or_parsed, (str, Path)),
-        Path(project_file_as_path_or_parsed).exists()
-    ]):
+    elif isinstance(project_file_as_path_or_parsed, (str, Path)) and Path(project_file_as_path_or_parsed).exists():
         with open(project_file_as_path_or_parsed, encoding="utf-8") as f:
             try:
                 project_definition = json.load(f)
             except:
-                logger.error(f"The input file '{project_file_as_path_or_parsed}' cannot be parsed to a JSON object.", exc_info=True)
-                raise BaseError(f"The input file '{project_file_as_path_or_parsed}' cannot be parsed to a JSON object.") from None
+                msg = f"The input file '{project_file_as_path_or_parsed}' cannot be parsed to a JSON object."
+                logger.error(msg, exc_info=True)
+                raise BaseError(msg) from None
     else:
         raise BaseError("Invalid input: The input must be a path to a JSON file or a parsed JSON object.")
     return project_definition
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/stack_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 docker_path_of_user = Path.home() / Path(".dsp-tools/start-stack")
 docker_path_of_user.mkdir(parents=True, exist_ok=True)
 
 
 def start_stack(
     max_file_size: Optional[int] = None,
     enforce_docker_system_prune: bool = False,
-    suppress_docker_system_prune: bool = False
+    suppress_docker_system_prune: bool = False,
 ) -> bool:
     """
     Start the Docker containers of DSP-API and DSP-APP, and load some basic data models and data. After startup, ask
     user if Docker should be pruned or not.
 
     Args:
         max_file_size: max. multimedia file size allowed by SIPI, in MB (max: 100'000)
@@ -45,22 +45,27 @@
     docker_path_of_distribution = importlib.resources.files("dsp_tools").joinpath("resources/start-stack")
     for file in docker_path_of_distribution.iterdir():
         with importlib.resources.as_file(file) as f:
             file_path = Path(f)
         shutil.copy(file_path, docker_path_of_user / file.name)
 
     # get sipi.docker-config.lua
-    commit_of_used_api_version = "783428ebc84d974b82452e3d7358b946ae40588c"      # gitleaks:allow
+    # take commit hash of latest DSP-API release from https://github.com/dasch-swiss/dsp-api/commits/main
+    commit_of_used_api_version = "29b437e14b4d6382c3ffb2981a68f1bfac0a6212"
     url_prefix = f"https://github.com/dasch-swiss/dsp-api/raw/{commit_of_used_api_version}/"
     docker_config_lua_text = requests.get(f"{url_prefix}sipi/config/sipi.docker-config.lua", timeout=5).text
     if max_file_size:
         max_post_size_regex = r"max_post_size ?= ?[\'\"]\d+M[\'\"]"
         if not re.search(max_post_size_regex, docker_config_lua_text):
             raise BaseError("Unable to set max_file_size. Please try again without this flag.")
-        docker_config_lua_text = re.sub(max_post_size_regex, f"max_post_size = '{max_file_size}M'", docker_config_lua_text)
+        docker_config_lua_text = re.sub(
+            max_post_size_regex,
+            f"max_post_size = '{max_file_size}M'",
+            docker_config_lua_text,
+        )
     with open(docker_path_of_user / "sipi.docker-config.lua", "w", encoding="utf-8") as f:
         f.write(docker_config_lua_text)
 
     # start up the fuseki database
     completed_process = subprocess.run("docker compose up db -d", shell=True, cwd=docker_path_of_user, check=False)
     if not completed_process or completed_process.returncode != 0:
         raise BaseError("Cannot start the API: Error while executing 'docker compose up db -d'")
@@ -79,41 +84,43 @@
     # (same behaviour as dsp-api/webapi/target/docker/stage/opt/docker/scripts/fuseki-init-knora-test.sh)
     repo_template = requests.get(f"{url_prefix}webapi/scripts/fuseki-repository-config.ttl.template", timeout=5).text
     repo_template = repo_template.replace("@REPOSITORY@", "knora-test")
     response = requests.post(
         url="http://0.0.0.0:3030/$/datasets",
         files={"file": ("file.ttl", repo_template, "text/turtle; charset=utf8")},
         auth=("admin", "test"),
-        timeout=5
+        timeout=5,
     )
     if not response.ok:
-        raise BaseError("Cannot start DSP-API: Error when creating the 'knora-test' repository. Is DSP-API perhaps "
-                        "running already?")
+        raise BaseError(
+            "Cannot start DSP-API: Error when creating the 'knora-test' repository. "
+            "Is DSP-API perhaps running already?"
+        )
 
     # load some basic ontos and data into the repository
     # (same behaviour as dsp-api/webapi/target/docker/stage/opt/docker/scripts/fuseki-init-knora-test.sh)
     graph_prefix = "http://0.0.0.0:3030/knora-test/data?graph="
     ttl_files = [
         ("knora-ontologies/knora-admin.ttl", "http://www.knora.org/ontology/knora-admin"),
         ("knora-ontologies/knora-base.ttl", "http://www.knora.org/ontology/knora-base"),
         ("knora-ontologies/standoff-onto.ttl", "http://www.knora.org/ontology/standoff"),
         ("knora-ontologies/standoff-data.ttl", "http://www.knora.org/data/standoff"),
         ("knora-ontologies/salsah-gui.ttl", "http://www.knora.org/ontology/salsah-gui"),
         ("test_data/all_data/admin-data.ttl", "http://www.knora.org/data/admin"),
         ("test_data/all_data/permissions-data.ttl", "http://www.knora.org/data/permissions"),
         ("test_data/ontologies/anything-onto.ttl", "http://www.knora.org/ontology/0001/anything"),
-        ("test_data/all_data/anything-data.ttl", "http://www.knora.org/data/0001/anything")
+        ("test_data/all_data/anything-data.ttl", "http://www.knora.org/data/0001/anything"),
     ]
     for ttl_file, graph in ttl_files:
         ttl_text = requests.get(url_prefix + ttl_file, timeout=5).text
         response = requests.post(
             url=graph_prefix + graph,
             files={"file": ("file.ttl", ttl_text, "text/turtle; charset: utf-8")},
             auth=("admin", "test"),
-            timeout=5
+            timeout=5,
         )
         if not response.ok:
             raise BaseError(f"Cannot start DSP-API: Error when creating graph '{graph}'")
 
     # startup all other components
     subprocess.run("docker compose up -d", shell=True, cwd=docker_path_of_user, check=True)
     print("DSP-API is now running on http://0.0.0.0:3333/ and DSP-APP on http://0.0.0.0:4200/")
@@ -122,16 +129,18 @@
     if enforce_docker_system_prune:
         prune_docker = "y"
     elif suppress_docker_system_prune:
         prune_docker = "n"
     else:
         prune_docker = None
         while prune_docker not in ["y", "n"]:
-            prune_docker = input("Allow dsp-tools to execute 'docker system prune'? This is necessary to keep your "
-                                 "Docker clean. If you are unsure what that means, just type y and press Enter. [y/n]")
+            prune_docker = input(
+                "Allow dsp-tools to execute 'docker system prune'? This is necessary to keep your Docker clean. "
+                "If you are unsure what that means, just type y and press Enter. [y/n]"
+            )
     if prune_docker == "y":
         subprocess.run("docker system prune -f", shell=True, cwd=docker_path_of_user, check=False)
 
     return True
 
 
 def stop_stack() -> bool:
```

### Comparing `dsp_tools-2.3.2/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-2.3.3/src/dsp_tools/utils/xml_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,22 @@
 import pandas as pd
 from lxml import etree
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.permission import Permissions
 from dsp_tools.models.projectContext import ProjectContext
-from dsp_tools.models.resource import (
-    KnoraStandoffXmlEncoder,
-    ResourceInstance,
-    ResourceInstanceFactory
-)
+from dsp_tools.models.resource import KnoraStandoffXmlEncoder, ResourceInstance, ResourceInstanceFactory
 from dsp_tools.models.sipi import Sipi
 from dsp_tools.models.value import KnoraStandoffXml
 from dsp_tools.models.xmlpermission import XmlPermission
 from dsp_tools.models.xmlproperty import XMLProperty
 from dsp_tools.models.xmlresource import XMLResource
 from dsp_tools.utils.logging import get_logger
-from dsp_tools.utils.shared import (
-    login,
-    try_network_action,
-    validate_xml_against_schema
-)
+from dsp_tools.utils.shared import login, try_network_action, validate_xml_against_schema
 
 MetricRecord = namedtuple("MetricRecord", ["res_id", "filetype", "filesize_mb", "event", "duration_ms", "mb_per_sec"])
 
 logger = get_logger(__name__)
 
 
 def _transform_server_url_to_foldername(server: str) -> str:
@@ -56,40 +48,40 @@
         simplified version, e.g. "test.dasch.swiss" or "localhost"
     """
     server_substitutions = {
         r"https?://": "",
         r"^api\.": "",
         r":\d{2,5}/?$": "",
         r"/$": "",
-        r"0.0.0.0": "localhost"
+        r"0.0.0.0": "localhost",
     }
     for pattern, repl in server_substitutions.items():
         server = re.sub(pattern, repl, server)
     return server
 
 
 def _determine_save_location_of_diagnostic_info(
     server: str,
     proj_shortcode: str,
-    onto_name: str
+    onto_name: str,
 ) -> tuple[Path, str, str]:
     """
     Determine the save location for diagnostic info that will be used if the xmlupload is interrupted.
     They are going to be stored in ~/.dsp-tools/xmluploads/server/shortcode/ontoname.
     This path is computed and created.
 
     Args:
         server: URL of the DSP server where the data is uploaded to
         proj_shortcode: 4-digit hexadecimal shortcode of the project
         onto_name: name of the ontology that the data belongs to
 
     Returns:
-        a tuple consisting of the absolute full path to the storage location, 
+        a tuple consisting of the absolute full path to the storage location,
         a version of the server URL that can be used as foldername,
-        and the timestamp string that can be used as component of file names 
+        and the timestamp string that can be used as component of file names
         (so that different diagnostic files of the same xmlupload have the same timestamp)
     """
     server_as_foldername = _transform_server_url_to_foldername(server)
     timestamp_str = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     save_location = Path.home() / Path(".dsp-tools") / "xmluploads" / server_as_foldername / proj_shortcode / onto_name
     save_location.mkdir(parents=True, exist_ok=True)
     return save_location, server_as_foldername, timestamp_str
@@ -97,15 +89,15 @@
 
 def _write_id2iri_mapping_and_metrics(
     id2iri_mapping: dict[str, str],
     metrics: Optional[list[MetricRecord]],
     failed_uploads: list[str],
     input_file: Union[str, Path, etree._ElementTree[Any]],
     timestamp_str: str,
-    server_as_foldername: str
+    server_as_foldername: str,
 ) -> bool:
     """
     Writes the id2iri mapping and the metrics into the current working directory,
     and prints the failed uploads (if applicable).
 
     Args:
         id2iri_mapping: mapping of ids from the XML file to IRIs in DSP (initially empty, gets filled during the upload)
@@ -143,19 +135,19 @@
         print(f"Total time of xmlupload: {sum(int(record.duration_ms) for record in metrics) / 1000:.1f} seconds")
 
     return success
 
 
 def _remove_circular_references(
     resources: list[XMLResource],
-    verbose: bool
+    verbose: bool,
 ) -> tuple[
     list[XMLResource],
     dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
-    dict[XMLResource, dict[XMLProperty, list[str]]]
+    dict[XMLResource, dict[XMLProperty, list[str]]],
 ]:
     """
     Temporarily removes problematic resource-references from a list of resources. A reference is problematic if
     it creates a circle (circular references).
 
     Args:
         resources: list of resources that possibly contain circular references
@@ -198,64 +190,70 @@
                     ok_resources.append(resource)
                     ok_res_ids.append(resource.id)
                 else:
                     nok_resources.append(resource)
         resources = nok_resources
         if len(nok_resources) == nok_len:
             # there are circular references. go through all problematic resources, and stash the problematic references.
-            nok_resources, ok_res_ids, ok_resources, stashed_xml_texts, stashed_resptr_props = _stash_circular_references(
+            (
                 nok_resources,
                 ok_res_ids,
                 ok_resources,
                 stashed_xml_texts,
-                stashed_resptr_props
+                stashed_resptr_props,
+            ) = _stash_circular_references(
+                nok_resources=nok_resources,
+                ok_res_ids=ok_res_ids,
+                ok_resources=ok_resources,
+                stashed_xml_texts=stashed_xml_texts,
+                stashed_resptr_props=stashed_resptr_props,
             )
         nok_len = len(nok_resources)
         nok_resources = []
         cnt += 1
         if verbose:
-            print(f'{cnt}. ordering pass finished.')
-            logger.info(f'{cnt}. ordering pass finished.')
+            print(f"{cnt}. ordering pass finished.")
+            logger.info(f"{cnt}. ordering pass finished.")
     return ok_resources, stashed_xml_texts, stashed_resptr_props
 
 
 def _stash_circular_references(
     nok_resources: list[XMLResource],
     ok_res_ids: list[str],
     ok_resources: list[XMLResource],
     stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
-    stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]]
+    stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]],
 ) -> tuple[
     list[XMLResource],
     list[str],
     list[XMLResource],
     dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
-    dict[XMLResource, dict[XMLProperty, list[str]]]
+    dict[XMLResource, dict[XMLProperty, list[str]]],
 ]:
     """
     Raises:
         BaseError
     """
     for res in nok_resources.copy():
         for link_prop in res.get_props_with_links():
-            if link_prop.valtype == 'text':
+            if link_prop.valtype == "text":
                 for value in link_prop.values:
                     if value.resrefs and not all(_id in ok_res_ids for _id in value.resrefs):
                         # stash this XML text, replace it by its hash, and remove the
                         # problematic resrefs from the XMLValue's resrefs list
-                        value_hash = str(hash(f'{value.value}{datetime.now()}'))
+                        value_hash = str(hash(f"{value.value}{datetime.now()}"))
                         if res not in stashed_xml_texts:
                             stashed_xml_texts[res] = {link_prop: {value_hash: cast(KnoraStandoffXml, value.value)}}
                         elif link_prop not in stashed_xml_texts[res]:
                             stashed_xml_texts[res][link_prop] = {value_hash: cast(KnoraStandoffXml, value.value)}
                         else:
                             stashed_xml_texts[res][link_prop][value_hash] = cast(KnoraStandoffXml, value.value)
                         value.value = KnoraStandoffXml(value_hash)
                         value.resrefs = [_id for _id in value.resrefs if _id in ok_res_ids]
-            elif link_prop.valtype == 'resptr':
+            elif link_prop.valtype == "resptr":
                 for value in link_prop.values.copy():
                     if value.value not in ok_res_ids:
                         # value.value is the id of the target resource. stash it, then delete it
                         if res not in stashed_resptr_props:
                             stashed_resptr_props[res] = {}
                             stashed_resptr_props[res][link_prop] = [str(value.value)]
                         else:
@@ -313,28 +311,29 @@
     if not re.match("^[0-9a-fA-F]{4}$", project_id):
         logger.error(f"while converting ARK '{ark}'. Invalid project shortcode '{project_id}'")
         raise BaseError(f"while converting ARK '{ark}'. Invalid project shortcode '{project_id}'")
     if not re.match("^[0-9A-Za-z]+$", resource_id):
         logger.error(f"while converting ARK '{ark}'. Invalid Salsah ID '{resource_id}'")
         raise BaseError(f"while converting ARK '{ark}'. Invalid Salsah ID '{resource_id}'")
 
-    # make a UUID v5 from the namespace created above (which is a UUID itself) and the resource ID and encode it to base64
+    # make a UUID v5 from the namespace created above (which is a UUID itself) and the resource ID
+    # and encode it to base64
     dsp_uuid = base64.urlsafe_b64encode(uuid.uuid5(dasch_uuid_ns, resource_id).bytes).decode("utf-8")
     dsp_uuid = dsp_uuid[:-2]
 
     # use the new UUID to create the resource IRI
     return "http://rdfh.ch/" + project_id + "/" + dsp_uuid
 
 
 def _parse_xml_file(input_file: Union[str, Path, etree._ElementTree[Any]]) -> etree._Element:
     """
-    Parse an XML file with DSP-conform data, 
-    remove namespace URI from the elements' names, 
-    and transform the special tags <annotation>, <region>, and <link> 
-    to their technically correct form 
+    Parse an XML file with DSP-conform data,
+    remove namespace URI from the elements' names,
+    and transform the special tags <annotation>, <region>, and <link>
+    to their technically correct form
     <resource restype="Annotation">, <resource restype="Region">, and <resource restype="LinkObj">.
 
     Args:
         input_file: path to the XML file, or parsed ElementTree
 
     Returns:
         the root element of the parsed XML file
@@ -342,22 +341,22 @@
 
     # remove comments and processing instructions (commented out properties break the XMLProperty constructor)
     if isinstance(input_file, (str, Path)):
         parser = etree.XMLParser(remove_comments=True, remove_pis=True)
         tree = etree.parse(source=input_file, parser=parser)
     else:
         tree = copy.deepcopy(input_file)
-        for c in tree.xpath('//comment()'):
+        for c in tree.xpath("//comment()"):
             c.getparent().remove(c)
-        for c in tree.xpath('//processing-instruction()'):
+        for c in tree.xpath("//processing-instruction()"):
             c.getparent().remove(c)
 
     # remove namespace URI from the elements' names and transform the special tags to their technically correct form
     for elem in tree.iter():
-        elem.tag = etree.QName(elem).localname   # remove namespace URI in the element's name
+        elem.tag = etree.QName(elem).localname  # remove namespace URI in the element's name
         if elem.tag == "annotation":
             elem.attrib["restype"] = "Annotation"
             elem.tag = "resource"
         elif elem.tag == "link":
             elem.attrib["restype"] = "LinkObj"
             elem.tag = "resource"
         elif elem.tag == "region":
@@ -371,71 +370,91 @@
 
 
 def _check_consistency_with_ontology(
     resources: list[XMLResource],
     resclass_name_2_type: dict[str, type],
     shortcode: str,
     ontoname: str,
-    verbose: bool = False
+    verbose: bool = False,
 ) -> None:
     """
     Checks if the resource types and properties in the XML are consistent with the ontology.
 
     Args:
         resources: a list of parsed XMLResources
         resclass_name_2_type: infos about the resource classes that exist on the DSP server for the current ontology
-        shortcode: the shortcode of the project as referenced in the attribute "shortcode" of the <knora> tag of the XML file
-        ontoname: the name of the ontology as referenced in the attribute "default-ontology" of the <knora> tag of the XML file
+        shortcode: the shortcode of the project
+            as referenced in the attribute "shortcode" of the <knora> tag of the XML file
+        ontoname: the name of the ontology
+            as referenced in the attribute "default-ontology" of the <knora> tag of the XML file
         verbose: verbose switch
 
     Raises:
         UserError with a detailed error message if there is an inconsistency between the ontology and the data
 
     Returns:
         None if everything is okay
     """
     if verbose:
         print("Check if the resource types and properties are consistent with the ontology...")
         logger.info("Check if the resource types and properties are consistent with the ontology...")
     if not any(x.startswith(ontoname) for x in resclass_name_2_type.keys()):
-        err_msg = f"The <knora> tag of your XML file references the ontology '{ontoname}', " \
-                  f"but the project {shortcode} on the DSP server doesn't contain an ontology with this name."
+        err_msg = (
+            f"The <knora> tag of your XML file references the ontology '{ontoname}', "
+            f"but the project {shortcode} on the DSP server doesn't contain an ontology with this name."
+        )
         logger.error(err_msg)
         raise UserError(err_msg)
     knora_properties = resclass_name_2_type[resources[0].restype].knora_properties  # type: ignore
 
     for resource in resources:
-
         # check that the resource type is consistent with the ontology
         if resource.restype not in resclass_name_2_type:
-            err_msg = f"=========================\n" \
-                      f"ERROR: Resource '{resource.label}' (ID: {resource.id}) has an invalid resource type '{resource.restype}'. " \
-                      f"Is your syntax correct? Remember the rules:\n" \
-                      f" - DSP-API internals: <resource restype=\"restype\">         " \
-                            f"(will be interpreted as 'knora-api:restype')\n" \
-                      f" - current ontology:  <resource restype=\":restype\">        " \
-                            f"('restype' must be defined in the 'resources' section of your ontology)\n" \
-                      f" - other ontology:    <resource restype=\"other:restype\">   " \
-                            f"(not yet implemented: 'other' must be defined in the same JSON project file as your ontology)"
+            res_syntaxes = [
+                'DSP-API internals: <resource restype="restype">',
+                'current ontology:  <resource restype=":restype">',
+                'other ontology:    <resource restype="other:restype">',
+            ]
+            res_explanations = [
+                'will be interpreted as "knora-api:restype"',
+                '"restype" must be defined in the "resources" section of your ontology',
+                'not yet implemented: "other" must be defined in the same JSON project file as your ontology',
+            ]
+            err_msg = (
+                f"=========================\n"
+                f"ERROR: Resource '{resource.label}' (ID: {resource.id}) "
+                f"has an invalid resource type '{resource.restype}'. "
+                "Is your syntax correct? Remember the rules:\n"
+            )
+            for res_syntax, res_explanation in zip(res_syntaxes, res_explanations):
+                err_msg += f" - {res_syntax:<55} ({res_explanation})\n"
             logger.error(err_msg)
             raise UserError(err_msg)
 
         # check that the property types are consistent with the ontology
         resource_properties = resclass_name_2_type[resource.restype].properties.keys()  # type: ignore
         for propname in [prop.name for prop in resource.properties]:
             if propname not in knora_properties and propname not in resource_properties:
-                err_msg = f"=========================\n" \
-                          f"ERROR: Resource '{resource.label}' (ID: {resource.id}) has an invalid property '{propname}'. " \
-                          f"Is your syntax correct? Remember the rules:\n" \
-                          f" - DSP-API internals: <text-prop name=\"propname\">         " \
-                                f"(will be interpreted as 'knora-api:propname')\n" \
-                          f" - current ontology:  <text-prop name=\":propname\">        " \
-                                f"('propname' must be defined in the 'properties' section of your ontology)\n" \
-                          f" - other ontology:    <text-prop name=\"other:propname\">   " \
-                                f"(not yet implemented: 'other' must be defined in the same JSON project file than your ontology)"
+                prop_syntaxes = [
+                    'DSP-API internals: <text-prop name="propname">',
+                    'current ontology:  <text-prop name=":propname">',
+                    'other ontology:    <text-prop name="other:propname">',
+                ]
+                prop_explanations = [
+                    'will be interpreted as "knora-api:propname"',
+                    '"propname" must be defined in the "properties" section of your ontology',
+                    'not yet implemented: "other" must be defined in the same JSON project file as your ontology',
+                ]
+                err_msg = (
+                    f"=========================\n"
+                    f"ERROR: Resource '{resource.label}' (ID: {resource.id}) has an invalid property '{propname}'. "
+                    f"Is your syntax correct? Remember the rules:\n"
+                )
+                for prop_syntax, prop_explanation in zip(prop_syntaxes, prop_explanations):
+                    err_msg += f" - {prop_syntax:<55} ({prop_explanation})\n"
                 logger.error(err_msg)
                 raise UserError(err_msg)
 
     print("Resource types and properties are consistent with the ontology.")
     logger.info("Resource types and properties are consistent with the ontology.")
 
 
@@ -445,15 +464,15 @@
     user: str,
     password: str,
     imgdir: str,
     sipi: str,
     verbose: bool,
     incremental: bool,
     save_metrics: bool,
-    preprocessing_done: bool
+    preprocessing_done: bool,
 ) -> bool:
     """
     This function reads an XML file and imports the data described in it onto the DSP server.
 
     Args:
         input_file: path to the XML file or parsed ElementTree
         server: the DSP server where the data should be imported
@@ -473,23 +492,23 @@
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
     # parse the XML file
     validate_xml_against_schema(input_file=input_file)
     root = _parse_xml_file(input_file=input_file)
-    shortcode = root.attrib['shortcode']
-    default_ontology = root.attrib['default-ontology']
+    shortcode = root.attrib["shortcode"]
+    default_ontology = root.attrib["default-ontology"]
     logger.info(f"Validated and parsed the XML file. Shortcode='{shortcode}' and default_ontology='{default_ontology}'")
 
     # determine save location that will be used for diagnostic info if the xmlupload is interrupted
     save_location, server_as_foldername, timestamp_str = _determine_save_location_of_diagnostic_info(
         server=server,
         proj_shortcode=shortcode,
-        onto_name=default_ontology
+        onto_name=default_ontology,
     )
     logger.info(f"save_location='{save_location}'")
 
     # start metrics
     metrics: list[MetricRecord] = []
     preparation_start = datetime.now()
 
@@ -515,23 +534,25 @@
     # get the project information and project ontology from the server
     try:
         res_inst_factory = try_network_action(lambda: ResourceInstanceFactory(con, shortcode))
     except BaseError:
         logger.error(f"A project with shortcode {shortcode} could not be found on the DSP server", exc_info=True)
         raise UserError(f"A project with shortcode {shortcode} could not be found on the DSP server") from None
     permissions_lookup: dict[str, Permissions] = {s: perm.get_permission_instance() for s, perm in permissions.items()}
-    resclass_name_2_type: dict[str, type] = {s: res_inst_factory.get_resclass_type(s) for s in res_inst_factory.get_resclass_names()}
+    resclass_name_2_type: dict[str, type] = {
+        s: res_inst_factory.get_resclass_type(s) for s in res_inst_factory.get_resclass_names()
+    }
 
     # check if the data in the XML is consistent with the ontology
     _check_consistency_with_ontology(
         resources=resources,
         resclass_name_2_type=resclass_name_2_type,
         shortcode=shortcode,
         ontoname=default_ontology,
-        verbose=verbose
+        verbose=verbose,
     )
 
     # temporarily remove circular references, but only if not an incremental upload
     if not incremental:
         resources, stashed_xml_texts, stashed_resptr_props = _remove_circular_references(resources, verbose)
     else:
         stashed_xml_texts = dict()
@@ -553,54 +574,56 @@
             sipi_server=sipi_server,
             permissions_lookup=permissions_lookup,
             resclass_name_2_type=resclass_name_2_type,
             id2iri_mapping=id2iri_mapping,
             con=con,
             failed_uploads=failed_uploads,
             metrics=metrics,
-            preprocessing_done=preprocessing_done
+            preprocessing_done=preprocessing_done,
         )
         if stashed_xml_texts:
             nonapplied_xml_texts = _upload_stashed_xml_texts(
                 verbose=verbose,
                 id2iri_mapping=id2iri_mapping,
                 con=con,
-                stashed_xml_texts=stashed_xml_texts
+                stashed_xml_texts=stashed_xml_texts,
             )
         if stashed_resptr_props:
             nonapplied_resptr_props = _upload_stashed_resptr_props(
                 verbose=verbose,
                 id2iri_mapping=id2iri_mapping,
                 con=con,
-                stashed_resptr_props=stashed_resptr_props
+                stashed_resptr_props=stashed_resptr_props,
             )
         if nonapplied_resptr_props or nonapplied_xml_texts:
-            logger.error("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
-            raise BaseError("Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server.")
-    except BaseException as err:      # pylint: disable=broad-except
-        # The forseeable errors are already handled by the variables failed_uploads, nonapplied_xml_texts, and nonapplied_resptr_props.
+            msg = "Some stashed resptrs or XML texts could not be reapplied to their resources on the DSP server."
+            logger.error(msg)
+            raise BaseError(msg)
+    except BaseException as err:  # pylint: disable=broad-except
+        # The forseeable errors are already handled by the variables
+        # failed_uploads, nonapplied_xml_texts, and nonapplied_resptr_props.
         # Here we catch the unforseeable exceptions, hence BaseException (=the base class of all exceptions)
         _handle_upload_error(
             err=err,
             id2iri_mapping=id2iri_mapping,
             failed_uploads=failed_uploads,
             stashed_xml_texts=nonapplied_xml_texts or stashed_xml_texts,
             stashed_resptr_props=nonapplied_resptr_props or stashed_resptr_props,
             save_location=save_location,
-            timestamp_str=timestamp_str
+            timestamp_str=timestamp_str,
         )
 
     # write id2iri mapping, metrics, and print some final info
     success = _write_id2iri_mapping_and_metrics(
         id2iri_mapping=id2iri_mapping,
         failed_uploads=failed_uploads,
         metrics=metrics if save_metrics else None,
         input_file=input_file,
         timestamp_str=timestamp_str,
-        server_as_foldername=server_as_foldername
+        server_as_foldername=server_as_foldername,
     )
     if success:
         print("All resources have successfully been uploaded.")
         logger.info("All resources have successfully been uploaded.")
     return success
 
 
@@ -610,15 +633,15 @@
     sipi_server: Sipi,
     permissions_lookup: dict[str, Permissions],
     resclass_name_2_type: dict[str, type],
     id2iri_mapping: dict[str, str],
     con: Connection,
     failed_uploads: list[str],
     metrics: list[MetricRecord],
-    preprocessing_done: bool
+    preprocessing_done: bool,
 ) -> tuple[dict[str, str], list[str], list[MetricRecord]]:
     """
     Iterates through all resources and tries to upload them to DSP.
     If a temporary exception occurs, the action is repeated until success,
     and if a permanent exception occurs, the resource is skipped.
 
     Args:
@@ -633,17 +656,20 @@
         metrics: list with the metric records collected until now (gets filled during the upload)
 
     Returns:
         id2iri_mapping, failed_uploads, metrics
     """
 
     # If there are multimedia files: calculate their total size
-    bitstream_all_sizes_mb = [Path(Path(imgdir) / Path(res.bitstream.value)).stat().st_size / 1000000
-                              if res.bitstream and not preprocessing_done else 0.0
-                              for res in resources]
+    bitstream_all_sizes_mb = [
+        Path(Path(imgdir) / Path(res.bitstream.value)).stat().st_size / 1000000
+        if res.bitstream and not preprocessing_done
+        else 0.0
+        for res in resources
+    ]
     if sum(bitstream_all_sizes_mb) > 0:
         bitstream_size_total_mb = round(sum(bitstream_all_sizes_mb), 1)
         bitstream_size_uploaded_mb = 0.0
         print(f"This xmlupload contains multimedia files with a total size of {bitstream_size_total_mb} MB.")
         logger.info(f"This xmlupload contains multimedia files with a total size of {bitstream_size_total_mb} MB.")
     else:  # make Pylance happy
         bitstream_size_total_mb = 0.0
@@ -659,179 +685,194 @@
             resource_iri = _convert_ark_v0_to_resource_iri(resource.ark)
 
         # in case of a multimedia resource: upload the multimedia file
         resource_bitstream = None
         if preprocessing_done and resource.bitstream:
             resource_bitstream = resource.get_bitstream(resource.bitstream.value, permissions_lookup)
         elif resource.bitstream:
+            pth = resource.bitstream.value
             try:
                 bitstream_start = datetime.now()
-                filetype = Path(resource.bitstream.value).suffix[1:]
+                filetype = Path(pth).suffix[1:]
                 img: Optional[dict[Any, Any]] = try_network_action(
                     sipi_server.upload_bitstream,
-                    filepath=str(Path(imgdir) / Path(resource.bitstream.value))
+                    filepath=str(Path(imgdir) / Path(pth)),
                 )
                 bitstream_duration = datetime.now() - bitstream_start
                 bitstream_duration_ms = bitstream_duration.seconds * 1000 + int(bitstream_duration.microseconds / 1000)
                 mb_per_sec = round((filesize / bitstream_duration_ms) * 1000, 1)
-                metrics.append(MetricRecord(resource.id, filetype, filesize, "bitstream upload", bitstream_duration_ms, mb_per_sec))
+                metrics.append(
+                    MetricRecord(resource.id, filetype, filesize, "bitstream upload", bitstream_duration_ms, mb_per_sec)
+                )
             except BaseError as err:
-                err_msg = err.original_error_msg_from_api or err.message
-                print(f'WARNING: Unable to upload file "{resource.bitstream.value}" of resource "{resource.label}" ({resource.id}): {err_msg}')
-                logger.warning(f'Unable to upload file "{resource.bitstream.value}" of resource "{resource.label}" ({resource.id}).', exc_info=True)
+                err_msg = err.orig_err_msg_from_api or err.message
+                msg = f"Unable to upload file '{pth}' of resource '{resource.label}' ({resource.id})"
+                print(f"WARNING: {msg}: {err_msg}")
+                logger.warning(msg, exc_info=True)
                 failed_uploads.append(resource.id)
                 continue
             bitstream_size_uploaded_mb += bitstream_all_sizes_mb[i]
-            print(f"Uploaded file '{resource.bitstream.value}' ({bitstream_size_uploaded_mb:.1f} MB / {bitstream_size_total_mb} MB)")
-            logger.info(f"Uploaded file '{resource.bitstream.value}' ({bitstream_size_uploaded_mb:.1f} MB / {bitstream_size_total_mb} MB)")
-            internal_file_name_bitstream = img['uploadedFiles'][0]['internalFilename']  # type: ignore
+            msg = f"Uploaded file '{pth}' ({bitstream_size_uploaded_mb:.1f} MB / {bitstream_size_total_mb} MB)"
+            print(msg)
+            logger.info(msg)
+            internal_file_name_bitstream = img["uploadedFiles"][0]["internalFilename"]  # type: ignore
             resource_bitstream = resource.get_bitstream(internal_file_name_bitstream, permissions_lookup)
 
         # create the resource in DSP
         resclass_type = resclass_name_2_type[resource.restype]
         properties = resource.get_propvals(id2iri_mapping, permissions_lookup)
         try:
             resource_instance: ResourceInstance = resclass_type(
                 con=con,
                 label=resource.label,
                 iri=resource_iri,
                 permissions=permissions_lookup.get(resource.permissions),  # type: ignore
                 creation_date=resource.creation_date,
                 bitstream=resource_bitstream,
-                values=properties
+                values=properties,
             )
             resource_creation_start = datetime.now()
             created_resource: ResourceInstance = try_network_action(resource_instance.create)
             resource_creation_duration = datetime.now() - resource_creation_start
-            resource_creation_duration_ms = resource_creation_duration.seconds * 1000 + int(resource_creation_duration.microseconds / 1000)
-            metrics.append(MetricRecord(resource.id, filetype, filesize, "resource creation", resource_creation_duration_ms, ""))
+            resource_creation_duration_ms = resource_creation_duration.seconds * 1000 + int(
+                resource_creation_duration.microseconds / 1000
+            )
+            metrics.append(
+                MetricRecord(resource.id, filetype, filesize, "resource creation", resource_creation_duration_ms, "")
+            )
         except BaseError as err:
-            err_msg = err.original_error_msg_from_api or err.message
+            err_msg = err.orig_err_msg_from_api or err.message
             print(f"WARNING: Unable to create resource '{resource.label}' ({resource.id}): {err_msg}")
             logger.warning(f"Unable to create resource '{resource.label}' ({resource.id}).", exc_info=True)
             failed_uploads.append(resource.id)
             continue
         id2iri_mapping[resource.id] = created_resource.iri
-        print(f"Created resource {i+1}/{len(resources)}: '{created_resource.label}' (ID: '{resource.id}', IRI: '{created_resource.iri}')")
-        logger.info(f"Created resource {i+1}/{len(resources)}: '{created_resource.label}' (ID: '{resource.id}', IRI: '{created_resource.iri}')")
+        resource_designation = f"'{created_resource.label}' (ID: '{resource.id}', IRI: '{created_resource.iri}')"
+        print(f"Created resource {i+1}/{len(resources)}: {resource_designation}")
+        logger.info(f"Created resource {i+1}/{len(resources)}: {resource_designation}")
         resource_duration = datetime.now() - resource_start
         resource_duration_ms = resource_duration.seconds * 1000 + int(resource_duration.microseconds / 1000)
         looping_overhead_ms = resource_duration_ms - resource_creation_duration_ms - (bitstream_duration_ms or 0)
         metrics.append(MetricRecord(resource.id, filetype, filesize, "looping overhead", looping_overhead_ms, ""))
 
     return id2iri_mapping, failed_uploads, metrics
 
 
 def _upload_stashed_xml_texts(
     verbose: bool,
     id2iri_mapping: dict[str, str],
     con: Connection,
-    stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]]
+    stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
 ) -> dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]]:
     """
     After all resources are uploaded, the stashed xml texts must be applied to their resources in DSP.
 
     Args:
         verbose: bool
         id2iri_mapping: mapping of ids from the XML file to IRIs in DSP
         con: connection to DSP
         stashed_xml_texts: all xml texts that have been stashed
 
     Returns:
         nonapplied_xml_texts: the xml texts that could not be uploaded
     """
 
-    print('Upload the stashed XML texts...')
-    logger.info('Upload the stashed XML texts...')
+    print("Upload the stashed XML texts...")
+    logger.info("Upload the stashed XML texts...")
     nonapplied_xml_texts = stashed_xml_texts.copy()
     for resource, link_props in stashed_xml_texts.items():
         if resource.id not in id2iri_mapping:
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
-            # no action necessary: this resource will remain in nonapplied_xml_texts, which will be handled by the caller
+            # no action necessary: this resource will remain in nonapplied_xml_texts,
+            # which will be handled by the caller
             continue
         res_iri = id2iri_mapping[resource.id]
         try:
-            existing_resource = try_network_action(con.get, path=f'/v2/resources/{quote_plus(res_iri)}')
+            existing_resource = try_network_action(con.get, path=f"/v2/resources/{quote_plus(res_iri)}")
         except BaseError as err:
             # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
             # this resource will remain in nonapplied_xml_texts, which will be handled by the caller
-            orig_err_msg = err.original_error_msg_from_api or err.message
-            err_msg = f"Unable to upload XML texts of resource '{resource.id}', because the resource cannot be retrieved from the DSP server."
+            orig_err_msg = err.orig_err_msg_from_api or err.message
+            err_msg = (
+                f"Unable to upload XML texts of resource '{resource.id}', "
+                "because the resource cannot be retrieved from the DSP server."
+            )
             print(f"  WARNING: {err_msg} Original error message: {orig_err_msg}")
             logger.warning(err_msg, exc_info=True)
             continue
         print(f'  Upload XML text(s) of resource "{resource.id}"...')
         logger.info(f'  Upload XML text(s) of resource "{resource.id}"...')
         for link_prop, hash_to_value in link_props.items():
             existing_values = existing_resource[link_prop.name]
             if not isinstance(existing_values, list):
-                existing_values = [existing_values, ]
+                existing_values = [existing_values]
             for existing_value in existing_values:
                 old_xmltext = existing_value.get("knora-api:textValueAsXml")
                 if not old_xmltext:
-                    # no action necessary: this property will remain in nonapplied_xml_texts, which will be handled by the caller
+                    # no action necessary: this property will remain in nonapplied_xml_texts,
+                    # which will be handled by the caller
                     continue
 
                 # strip all xml tags from the old xmltext, so that the pure text itself remains
-                pure_text = re.sub(r'(<\?xml.+>\s*)?<text>\s*(.+)\s*<\/text>', r'\2', old_xmltext)
+                pure_text = re.sub(r"(<\?xml.+>\s*)?<text>\s*(.+)\s*<\/text>", r"\2", old_xmltext)
 
                 # if the pure text is a hash, the replacement must be made. This hash originates from
                 # _stash_circular_references(), and identifies the XML texts
                 if pure_text not in hash_to_value:
-                    # no action necessary: this property will remain in nonapplied_xml_texts, which will be handled by the caller
+                    # no action necessary: this property will remain in nonapplied_xml_texts,
+                    # which will be handled by the caller
                     continue
                 new_xmltext = hash_to_value[pure_text]
 
                 # replace the outdated internal ids by their IRI
                 for _id, _iri in id2iri_mapping.items():
                     new_xmltext.regex_replace(f'href="IRI:{_id}:IRI"', f'href="{_iri}"')
 
                 # prepare API call
                 jsonobj = {
                     "@id": res_iri,
                     "@type": resource.restype,
                     link_prop.name: {
-                        "@id": existing_value['@id'],
+                        "@id": existing_value["@id"],
                         "@type": "knora-api:TextValue",
                         "knora-api:textValueAsXml": new_xmltext,
-                        "knora-api:textValueHasMapping": {
-                            '@id': 'http://rdfh.ch/standoff/mappings/StandardMapping'
-                        }
+                        "knora-api:textValueHasMapping": {"@id": "http://rdfh.ch/standoff/mappings/StandardMapping"},
                     },
-                    "@context": existing_resource['@context']
+                    "@context": existing_resource["@context"],
                 }
-                jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '), cls=KnoraStandoffXmlEncoder)
+                jsondata = json.dumps(jsonobj, indent=4, separators=(",", ": "), cls=KnoraStandoffXmlEncoder)
 
                 # execute API call
                 try:
-                    try_network_action(con.put, path='/v2/values', jsondata=jsondata)
+                    try_network_action(con.put, path="/v2/values", jsondata=jsondata)
                 except BaseError as err:
-                    # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
+                    # print the message to keep track of the cause for the failure.
+                    # Apart from that, no action is necessary:
                     # this resource will remain in nonapplied_xml_texts, which will be handled by the caller
-                    orig_err_msg = err.original_error_msg_from_api or err.message
+                    orig_err_msg = err.orig_err_msg_from_api or err.message
                     err_msg = f"Unable to upload the xml text of '{link_prop.name}' of resource '{resource.id}'."
                     print(f"    WARNING: {err_msg} Original error message: {orig_err_msg}")
                     logger.warning(err_msg, exc_info=True)
                     continue
                 nonapplied_xml_texts[resource][link_prop].pop(pure_text)
                 if verbose:
                     print(f'  Successfully uploaded xml text of "{link_prop.name}"\n')
                     logger.info(f'  Successfully uploaded xml text of "{link_prop.name}"\n')
 
     # make a purged version of nonapplied_xml_texts, without empty entries
     nonapplied_xml_texts = _purge_stashed_xml_texts(
         stashed_xml_texts=nonapplied_xml_texts,
-        id2iri_mapping=id2iri_mapping
+        id2iri_mapping=id2iri_mapping,
     )
     return nonapplied_xml_texts
 
 
 def _purge_stashed_xml_texts(
     stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
-    id2iri_mapping: dict[str, str]
+    id2iri_mapping: dict[str, str],
 ) -> dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]]:
     """
     Accepts a stash of XML texts and purges it of resources that could not be uploaded (=don't exist in DSP), and of
     resources that had all their XML texts reapplied. It returns a new dict with only the resources that exist in DSP,
     but whose XML texts could not all be uploaded.
 
     Args:
@@ -855,92 +896,97 @@
     return nonapplied_xml_texts
 
 
 def _upload_stashed_resptr_props(
     verbose: bool,
     id2iri_mapping: dict[str, str],
     con: Connection,
-    stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]]
+    stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]],
 ) -> dict[XMLResource, dict[XMLProperty, list[str]]]:
     """
     After all resources are uploaded, the stashed resptr props must be applied to their resources in DSP.
 
     Args:
         verbose: bool
         id2iri_mapping: mapping of ids from the XML file to IRIs in DSP
         con: connection to DSP
         stashed_resptr_props: all resptr props that have been stashed
 
     Returns:
         nonapplied_resptr_props: the resptr props that could not be uploaded
     """
 
-    print('Upload the stashed resptrs...')
-    logger.info('Upload the stashed resptrs...')
+    print("Upload the stashed resptrs...")
+    logger.info("Upload the stashed resptrs...")
     nonapplied_resptr_props = stashed_resptr_props.copy()
     for resource, prop_2_resptrs in stashed_resptr_props.items():
         if resource.id not in id2iri_mapping:
             # resource could not be uploaded to DSP, so the stash cannot be uploaded either
-            # no action necessary: this resource will remain in nonapplied_resptr_props, which will be handled by the caller
+            # no action necessary: this resource will remain in nonapplied_resptr_props,
+            # which will be handled by the caller
             continue
         res_iri = id2iri_mapping[resource.id]
         try:
-            existing_resource = try_network_action(con.get, path=f'/v2/resources/{quote_plus(res_iri)}')
+            existing_resource = try_network_action(con.get, path=f"/v2/resources/{quote_plus(res_iri)}")
         except BaseError as err:
             # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
             # this resource will remain in nonapplied_resptr_props, which will be handled by the caller
-            orig_err_msg = err.original_error_msg_from_api or err.message
-            err_msg = f"Unable to upload resptrs of resource '{resource.id}', because the resource cannot be retrieved from the DSP server."
+            orig_err_msg = err.orig_err_msg_from_api or err.message
+            err_msg = (
+                f"Unable to upload resptrs of resource '{resource.id}', "
+                "because the resource cannot be retrieved from the DSP server."
+            )
             print(f"  WARNING: {err_msg} Original error message: {orig_err_msg}")
             logger.warning(err_msg, exc_info=True)
             continue
         print(f'  Upload resptrs of resource "{resource.id}"...')
         logger.info(f'  Upload resptrs of resource "{resource.id}"...')
         for link_prop, resptrs in prop_2_resptrs.items():
             for resptr in resptrs.copy():
                 jsonobj = {
-                    '@id': res_iri,
-                    '@type': resource.restype,
-                    f'{link_prop.name}Value': {
-                        '@type': 'knora-api:LinkValue',
-                        'knora-api:linkValueHasTargetIri': {
-                            # if target doesn't exist in DSP, send the (invalid) resource ID of target to DSP, which
-                            # will produce an understandable error message
-                            '@id': id2iri_mapping.get(resptr, resptr)
-                        }
+                    "@id": res_iri,
+                    "@type": resource.restype,
+                    f"{link_prop.name}Value": {
+                        "@type": "knora-api:LinkValue",
+                        "knora-api:linkValueHasTargetIri": {
+                            # if target doesn't exist in DSP, send the (invalid) resource ID of target to DSP,
+                            # which will produce an understandable error message
+                            "@id": id2iri_mapping.get(resptr, resptr)
+                        },
                     },
-                    '@context': existing_resource['@context']
+                    "@context": existing_resource["@context"],
                 }
-                jsondata = json.dumps(jsonobj, indent=4, separators=(',', ': '))
+                jsondata = json.dumps(jsonobj, indent=4, separators=(",", ": "))
                 try:
-                    try_network_action(con.post, path='/v2/values', jsondata=jsondata)
+                    try_network_action(con.post, path="/v2/values", jsondata=jsondata)
                 except BaseError as err:
-                    # print the message to keep track of the cause for the failure. Apart from that, no action is necessary:
+                    # print the message to keep track of the cause for the failure.
+                    # Apart from that, no action is necessary:
                     # this resource will remain in nonapplied_resptr_props, which will be handled by the caller
-                    orig_err_msg = err.original_error_msg_from_api or err.message
+                    orig_err_msg = err.orig_err_msg_from_api or err.message
                     err_msg = f"Unable to upload the resptr prop of '{link_prop.name}' of resource '{resource.id}'."
                     print(f"    WARNING: {err_msg} Original error message: {orig_err_msg}")
                     logger.warning(err_msg, exc_info=True)
                     continue
                 nonapplied_resptr_props[resource][link_prop].remove(resptr)
                 if verbose:
                     print(f'  Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
                     logger.info(f'Successfully uploaded resptr-prop of "{link_prop.name}". Value: {resptr}')
 
     # make a purged version of nonapplied_resptr_props, without empty entries
     nonapplied_resptr_props = _purge_stashed_resptr_props(
         stashed_resptr_props=nonapplied_resptr_props,
-        id2iri_mapping=id2iri_mapping
+        id2iri_mapping=id2iri_mapping,
     )
     return nonapplied_resptr_props
 
 
 def _purge_stashed_resptr_props(
     stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]],
-    id2iri_mapping: dict[str, str]
+    id2iri_mapping: dict[str, str],
 ) -> dict[XMLResource, dict[XMLProperty, list[str]]]:
     """
     Accepts a stash of resptrs and purges it of resources that could not be uploaded (=don't exist in DSP), and of
     resources that had all their resptrs reapplied. It returns a new dict with only the resources that exist in DSP,
     but whose resptrs could not all be uploaded.
 
     Args:
@@ -967,22 +1013,22 @@
 def _handle_upload_error(
     err: BaseException,
     id2iri_mapping: dict[str, str],
     failed_uploads: list[str],
     stashed_xml_texts: dict[XMLResource, dict[XMLProperty, dict[str, KnoraStandoffXml]]],
     stashed_resptr_props: dict[XMLResource, dict[XMLProperty, list[str]]],
     save_location: Path,
-    timestamp_str: str
+    timestamp_str: str,
 ) -> None:
     """
-    In case the xmlupload must be interrupted, 
-    e.g. because of an error that could not be handled, 
-    or due to keyboard interrupt, 
-    this method ensures 
-    that all information about what is already in DSP 
+    In case the xmlupload must be interrupted,
+    e.g. because of an error that could not be handled,
+    or due to keyboard interrupt,
+    this method ensures
+    that all information about what is already in DSP
     is written into diagnostic files.
 
     It then re-raises the original error.
 
     Args:
         err: error that was the cause of the abort
         id2iri_mapping: mapping of ids from the XML file to IRIs in DSP (only successful uploads appear here)
@@ -992,71 +1038,78 @@
         save_location: path where to save the diagnostic info
         timestamp_str: timestamp for the name of the diagnostic files
 
     Returns:
         None
     """
 
-    print("\n=========================================="
-          "\nxmlupload must be aborted because of an error")
+    print("\n==========================================\nxmlupload must be aborted because of an error")
     logger.info("xmlupload must be aborted because of an error")
 
     # only stashed properties of resources that already exist in DSP are of interest
     stashed_xml_texts = _purge_stashed_xml_texts(
         stashed_xml_texts=stashed_xml_texts,
-        id2iri_mapping=id2iri_mapping
+        id2iri_mapping=id2iri_mapping,
     )
     stashed_resptr_props = _purge_stashed_resptr_props(
         stashed_resptr_props=stashed_resptr_props,
-        id2iri_mapping=id2iri_mapping
+        id2iri_mapping=id2iri_mapping,
     )
 
     if id2iri_mapping:
         id2iri_mapping_file = f"{save_location}/{timestamp_str}_id2iri_mapping.json"
         with open(id2iri_mapping_file, "x", encoding="utf-8") as f:
             json.dump(id2iri_mapping, f, ensure_ascii=False, indent=4)
         print(f"The mapping of internal IDs to IRIs was written to {id2iri_mapping_file}")
         logger.info(f"The mapping of internal IDs to IRIs was written to {id2iri_mapping_file}")
 
     if stashed_xml_texts:
-        stashed_xml_texts_serializable = {r.id: {p.name: xml for p, xml in rdict.items()} for r, rdict in stashed_xml_texts.items()}
+        stashed_xml_texts_serializable = {
+            r.id: {p.name: xml for p, xml in rdict.items()} for r, rdict in stashed_xml_texts.items()
+        }
         xml_filename = f"{save_location}/{timestamp_str}_stashed_text_properties.json"
         with open(xml_filename, "x", encoding="utf-8") as f:
             json.dump(
                 obj=stashed_xml_texts_serializable,
                 fp=f,
                 ensure_ascii=False,
                 indent=4,
-                cls=KnoraStandoffXmlEncoder
+                cls=KnoraStandoffXmlEncoder,
             )
-        msg = f"There are stashed text properties that could not be reapplied to the resources they were stripped from. " \
-              f"They were saved to {xml_filename}."
+        msg = (
+            f"There are stashed text properties that could not be reapplied to the resources they were stripped from. "
+            f"They were saved to {xml_filename}."
+        )
         print(msg)
         logger.info(msg)
 
     if stashed_resptr_props:
-        stashed_resptr_props_serializable = {r.id: {p.name: plist for p, plist in rdict.items()} for r, rdict in stashed_resptr_props.items()}
+        stashed_resptr_props_serializable = {
+            r.id: {p.name: plist for p, plist in rdict.items()} for r, rdict in stashed_resptr_props.items()
+        }
         resptr_filename = f"{save_location}/{timestamp_str}_stashed_resptr_properties.json"
         with open(resptr_filename, "x", encoding="utf-8") as f:
             json.dump(
                 obj=stashed_resptr_props_serializable,
                 fp=f,
                 ensure_ascii=False,
-                indent=4
+                indent=4,
             )
-        msg = f"There are stashed resptr properties that could not be reapplied to the resources they were stripped from. " \
-              f"They were saved to {resptr_filename}"
+        msg = (
+            f"There are stashed resptr properties that could not be reapplied "
+            f"to the resources they were stripped from. They were saved to {resptr_filename}"
+        )
         print(msg)
         logger.info(msg)
 
     # print the resources that threw an error when they were tried to be uploaded
     if failed_uploads:
-        print(f"Independently of this error, there were some resources that could not be uploaded: {failed_uploads}")
-        logger.info(f"Independently of this error, there were some resources that could not be uploaded: {failed_uploads}")
+        msg = f"Independently of this error, there were some resources that could not be uploaded: {failed_uploads}"
+        print(msg)
+        logger.info(msg)
 
     if isinstance(err, KeyboardInterrupt):
         sys.exit(1)
     else:
-        print("The error will now be raised again:\n"
-              "==========================================\n")
+        print("The error will now be raised again:\n==========================================\n")
         logger.info("The error will now be raised again")
         raise err
```

### Comparing `dsp_tools-2.3.2/PKG-INFO` & `dsp_tools-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.3.2
+Version: 2.3.3
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
```

