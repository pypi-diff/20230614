# Comparing `tmp/ilcdlib-0.5.0.tar.gz` & `tmp/ilcdlib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-0.5.0.tar", max compression
+gzip compressed data, was "ilcdlib-0.6.0.tar", max compression
```

## Comparing `ilcdlib-0.5.0.tar` & `ilcdlib-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/LICENSE
--rw-r--r--   0        0        0     4949 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/README.md
--rw-r--r--   0        0        0     3424 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    13825 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1334 2023-06-01 11:06:00.958141 ilcdlib-0.5.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     2883 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     2665 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     5369 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     7981 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     5749 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3650 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3774 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0     8343 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     2596 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     1185 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    19523 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     7667 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1900 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1899 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1212 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     1737 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7086 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     5103 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0      837 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0     8127 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     1206 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     1976 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2023-06-01 11:06:00.962141 ilcdlib-0.5.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6054 1970-01-01 00:00:00.000000 ilcdlib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-14 09:45:31.524799 ilcdlib-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4949 2023-06-14 09:45:31.524799 ilcdlib-0.6.0/README.md
+-rw-r--r--   0        0        0     3425 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17034 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1357 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     3121 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6395 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     2665 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     5639 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     3648 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     2748 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3924 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3774 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     2596 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     1991 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    30739 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     1707 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2023-06-14 09:45:31.528799 ilcdlib-0.6.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0      837 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0     8855 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     1206 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3329 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-06-14 09:45:31.532800 ilcdlib-0.6.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6055 1970-01-01 00:00:00.000000 ilcdlib-0.6.0/PKG-INFO
```

### Comparing `ilcdlib-0.5.0/LICENSE` & `ilcdlib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/README.md` & `ilcdlib-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/pyproject.toml` & `ilcdlib-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "0.5.0"
+version = "0.6.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -22,15 +22,15 @@
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
 requests = { version = ">=2.1.0,<3.0.0" }
-openepd = { version = ">=0.5.0,<1.0.0" }
+openepd = { version = ">=0.10.0,<1.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 # Unit tests
@@ -59,15 +59,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "0.5.0"
+version = "0.6.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/__main__.py` & `ilcdlib-0.6.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/__version__.py` & `ilcdlib-0.6.0/src/ilcdlib/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.5.0"
+VERSION = "0.6.0"
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/cli.py` & `ilcdlib-0.6.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/common.py` & `ilcdlib-0.6.0/src/ilcdlib/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  Find out more at www.BuildingTransparency.org
 #
 import abc
 import datetime
 from typing import IO, Literal, Self, Sequence, TextIO, overload
 
 from openepd.model.epd import Epd
-from openepd.model.lcia import ImpactSet
+from openepd.model.lcia import Impacts
 from openepd.model.org import Org
 from openepd.model.pcr import Pcr
 
 from ilcdlib.const import IlcdDatasetType
 from ilcdlib.dto import IlcdReference
 from ilcdlib.reference_data import get_ilcd_epd_reference_data_provider
 from ilcdlib.type import LangDef, LocalizedStr
@@ -68,14 +68,24 @@
         :param entity_version: The version of the entity e.g. 12.34.56
         :param binary: If True, the stream is opened in binary mode, otherwise in text mode.
         :raise: ValueError if the entity does not exist.
         """
         pass
 
     @abc.abstractmethod
+    def get_binary_stream_by_name(self, name: str, entity_type: str | None = None) -> IO[bytes] | None:
+        """
+        Get binary stream for the given file name.
+
+        :param name: The name of the file.
+        :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
+        """
+        pass
+
+    @abc.abstractmethod
     def entity_exists(self, entity_type: str, entity_id: str, entity_version: str | None = None) -> bool:
         """
         Check if the given entity exists.
 
         If you want to refer file by name only, you can use the entity_id and skip version parameter.
 
         :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
@@ -98,14 +108,29 @@
         """
         List all entities of the given type.
 
         :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
         """
         pass
 
+    def resolve_entity_url(self, ref: IlcdReference, digital_file: str | None) -> str | None:
+        """
+        Resolve the url of the given entity.
+
+        If `digital_file` parameter is set, the link to the associated digital file is returned.
+
+        :param ref: reference to the entity
+        :param digital_file: optional name of the file, if link to the file is needed.
+        """
+        return None
+
+    def get_pdf_url(self) -> str | None:
+        """Resolve URL to the PDF file associated with this EPD."""
+        return None
+
     def __enter__(self) -> Self:
         return self
 
     def __exit__(self, _type, value, traceback):
         self.close()
 
 
@@ -126,14 +151,18 @@
 
     def get_entity_stream(
         self, entity_type: str, entity_id: str, entity_version: str | None = None, *, binary: bool = False
     ) -> IO[bytes] | TextIO:
         """Generate exception. This class does not support get_entity_stream."""
         raise ValueError("NoopBaseReader does not support get_entity_stream")
 
+    def get_binary_stream_by_name(self, name: str, entity_type: str | None = None) -> IO[bytes] | None:
+        """Return None regardless of parameters for this implementation."""
+        return None
+
     def entity_exists(self, entity_type: str, entity_id: str, entity_version: str | None = None) -> bool:
         """Return False regardless of parameters for this implementation."""
         return False
 
     def close(self):
         """Do nothing. This implementation does not need to be closed."""
         pass
@@ -190,14 +219,15 @@
                 for dataset_name, dataset_provider in self.reference_data_providers.items():
                     if dataset_provider.entity_exists(entity_type, entity_id, entity_version):
                         with dataset_provider.get_entity_stream(entity_type, entity_id, entity_version) as stream:
                             return self.xml_parser.get_xml_tree(stream)
         raise ValueError(f"Entity {entity_id} version {entity_version} (type: {entity_type}) does not exist.")
 
     def _preprocess_path(self, path: XmlPath) -> str:
+        """Convert XPath defined in a form of tuple or string into a string representation."""
         if not isinstance(path, str):
             str_path = "/".join(path)
         else:
             str_path = path
         return str_path
 
     def _get_el(
@@ -286,14 +316,23 @@
             else:
                 continue
         return default_value
 
     def _get_reference(
         self, root: T_ET.Element, path: XmlPath, default_value: IlcdReference | None = None
     ) -> IlcdReference | None:
+        """
+        Extract reference data from XML element specified by XPath.
+
+        If the element doesn't hold reference information of doesn't exist - `default_value` is returned.
+
+        :param root: The root element to search in.
+        :param path: The path to the reference element (xpath in a form of tuple or string).
+        :param default_value: Default value to return if reference is not found.
+        """
         xpath = f"{self._preprocess_path(path)}"
         el = self.xml_parser.get_el(root, xpath)
         if el is None or el.attrib is None:
             return default_value
         ref_id = el.attrib.get("refObjectId", None)
         ref_type = el.attrib.get("type", None)
         if ref_id is None or ref_type is None:
@@ -301,53 +340,83 @@
         try:
             ref_type = IlcdDatasetType(ref_type)
         except ValueError:
             pass
         return IlcdReference(ref_type, ref_id, entity_version=None)
 
     def _get_external_tree(self, root: T_ET.Element, path: XmlPath) -> T_ET.Element | None:
+        """
+        Read XML document referenced by given path and return root XML element as result.
+
+        Path param must point to the reference element (xml element with refObjectId, type, [version]) attributes.
+        This method will locate the reference, and then read XML stream and parse it into XML tree.
+        For reading binary objects use _get_external_binary() instead.
+        See also _get_reference() for more details on how reference elements are parsed.
+
+        :param root: The root element to search in.
+        :param path: The path to the reference element (xpath in a form of tuple or string).
+        :return: XML Element or None if not found.
+        """
         ref = self._get_reference(root, path)
         if ref is None:
             return None
         return self.get_xml_tree(ref.entity_type, ref.entity_id, ref.entity_version, allow_static_datasets=True)
 
     def _get_external_binary(self, root: T_ET.Element, path: XmlPath) -> IO[bytes] | None:
+        """
+        Read binary object from element reference.
+
+        Path param must point to the reference element (xml element with refObjectId, type, [version]) attributes.
+        This method will locate the reference, and then read the binary object from the referenced entity.
+        For reading references to XML objects use _get_external_tree() instead.
+        See also _get_reference() for more details on how reference elements are parsed.
+
+        :param root: The root element to search in.
+        :param path: The path to the reference element (xpath in a form of tuple or string).
+        :return: The binary object or None if not found.
+        """
         ref = self._get_reference(root, path)
         if ref is None:
             return None
         return self.data_provider.get_entity_stream(ref.entity_type, ref.entity_id, ref.entity_version, binary=True)
 
 
 class OpenEpdContactSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding OpenEPD export support."""
 
     @abc.abstractmethod
-    def to_openepd_org(self, lang: LangDef, base_url: str | None = None) -> Org:
+    def to_openepd_org(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Org:
         """Read as openEPD Org object."""
         pass
 
 
 class OpenEpdPcrSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding openEPD export support."""
 
     @abc.abstractmethod
-    def to_openepd_pcr(self, lang: LangDef, base_url: str | None = None) -> Pcr:
+    def to_openepd_pcr(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Pcr:
         """Read as openEPD Pcr object."""
         pass
 
 
 class OpenEpdEdpSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding openEPD export support to EPD documents."""
 
     @abc.abstractmethod
-    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None) -> Epd:
+    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Epd:
         """Read as OpenEPD EPD object."""
         pass
 
 
 class OpenEpdImpactSetSupportReader(metaclass=abc.ABCMeta):
     """Base class for adding openEPD export support to LCIAResults."""
 
     @abc.abstractmethod
-    def to_openepd_impact_set(self, lang: LangDef, base_url: str | None = None) -> ImpactSet:
+    def to_openepd_impacts(
+        self,
+        scenario_names: dict[str, str],
+        lcia_method: str | None = None,
+        base_url: str | None = None,
+        provider_domain: str | None = None,
+    ) -> Impacts:
         """Read as openEPD ImpactSet object."""
         pass
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/const.py` & `ilcdlib-0.6.0/src/ilcdlib/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
 ILCD_IDENTIFICATION: tuple[str] = ("ILCD_EPD",)
+PDF_ATTACHMENT = "PDF"
 
 
 class IlcdContactClass(StrEnum):
     """Enumeration of ILCD contact classes."""
 
     Person = "Persons"
     Company = "Organisations"
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-0.6.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/dto.py` & `ilcdlib-0.6.0/src/ilcdlib/dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from dataclasses import dataclass
 from typing import Any, Generic, NamedTuple
 
+from openepd.model.org import Org
+
 from ilcdlib.utils import T
 
 
 class IlcdReference(NamedTuple):
     """A reference to an ILCD entity."""
 
     entity_type: str
@@ -93,7 +95,18 @@
         self.items = items
 
 
 class ProcessSearchResponse(BaseSearchResponse[ProcessBasicInfo]):
     """A search response for processes."""
 
     pass
+
+
+@dataclass(kw_only=True)
+class ComplianceDto:
+    """Basic information about a Compliance."""
+
+    uuid: str
+    short_name: str | None
+    name: str | None
+    link: str | None
+    issuer: Org | None
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/category.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/contact.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/contact.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdContactSupportReader
 from ilcdlib.const import IlcdContactClass
 from ilcdlib.dto import IlcdReference
 from ilcdlib.sanitizing.domain import domain_from_url
 from ilcdlib.sanitizing.phone import cleanup_phone
 from ilcdlib.type import LangDef
-from ilcdlib.utils import create_openepd_attachments, none_throws
+from ilcdlib.utils import create_openepd_attachments, none_throws, provider_domain_name_from_url
 from ilcdlib.xml_parser import T_ET
 
 
 class IlcdContactReader(OpenEpdContactSupportReader, IlcdXmlReader):
     """Reader for ILCD contact data sets."""
 
     def __init__(self, element: T_ET.Element, data_provider: BaseIlcdMediumSpecificReader):
@@ -104,21 +104,25 @@
 
     def get_address(self) -> str | None:
         """Get the address of the contact described by this data set."""
         return self._get_text(
             self._entity, ("contact:contactInformation", "contact:dataSetInformation", "contact:contactAddress")
         )
 
-    def to_openepd_org(self, lang: LangDef, base_url: str | None = None) -> Org:
+    def to_openepd_org(self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None) -> Org:
         """Convert this data set to an OpenEPD org object."""
         open_epd_contact = Contact.construct(
             email=self.get_email(),
             phone=cleanup_phone(self.get_phone()),
             website=self.get_website(),
             address=self.get_address(),
         )
-        return Org.construct(
+        org = Org.construct(
             name=self.get_name(lang),
             web_domain=domain_from_url(self.get_website()),
             contacts=open_epd_contact if open_epd_contact.has_values() else None,
-            attachments=create_openepd_attachments(self.get_own_reference(), base_url),
+            attachments=create_openepd_attachments(self.get_own_reference(), base_url) if base_url else None,
         )
+        if provider_domain is None:
+            provider_domain = provider_domain_name_from_url(base_url)
+        org.set_alt_id(provider_domain, self.get_uuid())
+        return org
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/flow.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,54 +15,56 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 from typing import Type
 
+from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Measurement
-from openepd.model.lcia import ImpactSet, ScopeSet
+from openepd.model.lcia import EolScenario, ScopeSet
 
-from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdImpactSetSupportReader
+from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, XmlPath
 from ilcdlib.entity.unit import IlcdUnitGroupReader
 from ilcdlib.mapping.common import SimpleDataMapper
-from ilcdlib.mapping.impacts import default_impacts_uuid_mapper
-from ilcdlib.type import LangDef
 from ilcdlib.xml_parser import T_ET
 
 
-class IlcdLciaResultsReader(OpenEpdImpactSetSupportReader, IlcdXmlReader):
-    """Read an ILCD PCR XML file."""
+class BaseIlcdScopeSetsReader(IlcdXmlReader):
+    """Read scope sets from XML file."""
 
     def __init__(
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
         unit_group_reader_cls: Type[IlcdUnitGroupReader] = IlcdUnitGroupReader,
-        impact_mapper: SimpleDataMapper[str] = default_impacts_uuid_mapper,
     ):
         super().__init__(data_provider)
         self._entity = element
-        self.impact_mapper = impact_mapper
         self.unit_group_reader_cls = unit_group_reader_cls
 
-    def _get_scope_set_for_el(self, el: T_ET.Element) -> tuple[ScopeSet, str] | None:
+    def _get_scope_set_for_el(
+        self,
+        el: T_ET.Element,
+        reference_data_set: XmlPath,
+        mapper: SimpleDataMapper[str],
+        scenario_names: dict[str, str],
+    ) -> tuple[ScopeSet, str] | None:
+        """Extract all scope set information from element."""
         # Impact name
-        type_el = self._get_el(el, ("process:referenceToLCIAMethodDataSet"))
+        type_el = self._get_el(el, reference_data_set)
         if type_el is None:
             return None
         type_uuid = type_el.attrib.get("refObjectId") if type_el is not None else None
         if type_uuid is None:
             return None
-        impact_name: str | None = self.impact_mapper.map(type_uuid, type_uuid)
+        impact_name: str | None = mapper.map(type_uuid, type_uuid)
         if impact_name == type_uuid:
-            impact_name = self._get_localized_text(
-                el, ("process:referenceToLCIAMethodDataSet", "common:shortDescription"), ("en", None)
-            )
+            impact_name = self._get_localized_text(type_el, ("common:shortDescription",), ("en", None))
         if impact_name is None:
             return None
         # UoM
         unit_el = self._get_external_tree(
             el,
             (
                 "common:other",
@@ -78,60 +80,85 @@
         else:
             unit_name = self._get_text(
                 el, ("common:other", "epd2013:referenceToUnitGroupDataSet", "common:shortDescription")
             )
         if unit_name is None:
             return None
         # Stages
-        scopes = self.__extract_scopes(el, unit_name)
+        scopes = self.__extract_scopes(el, unit_name, scenario_names)
         return ScopeSet.construct(**scopes), impact_name  # type: ignore
 
-    def __extract_scopes(self, el: T_ET.Element, unit_name: str) -> dict[str, Measurement | dict]:
+    def __extract_scopes(
+        self, el: T_ET.Element, unit_name: str, scenario_names: dict[str, str]
+    ) -> dict[str, Measurement | dict | list]:
+        """Extract all scopes from scope set element."""
         ext: dict[str, Measurement] = {}
-        scopes: dict[str, Measurement | dict] = {"ext": ext}
+        scopes: dict[str, Measurement | dict | list] = {"ext": ext}
         for al in self._get_all_els(el, ("common:other", "epd2013:amount")):
-            module_name = al.attrib.get("{http://www.iai.kit.edu/EPD/2013}module") if al.attrib else None
-            module_name = self.__map_module_name(module_name)
-            scenario_name = al.attrib.get("{http://www.iai.kit.edu/EPD/2013}scenario") if al.attrib else None
-            if scenario_name is not None:
-                continue  # TODO: Add support for scenarios
-            if module_name is None or al.text is None:
-                continue
-            try:
-                value = float(al.text)
-            except ValueError:
-                continue
-            measurement = Measurement(mean=value, unit=unit_name)
-            if ScopeSet.is_allowed_field_name(module_name):  # type: ignore
-                scopes[module_name] = measurement
-            else:
-                ext[module_name] = measurement
+            self.__extract_scope(al, ext, scopes, unit_name, scenario_names)
         if len(ext) == 0:
             del scopes["ext"]
         return scopes
 
-    def get_impacts(self) -> ImpactSet:
-        """Get the impacts from the ILCD EPD file."""
-        ext: dict[str, ScopeSet] = {}
-        lcia_resilts = self._get_all_els(self._entity, ("process:LCIAResult",))
-        impacts: dict[str, ScopeSet | dict] = {"ext": ext}
-        for lr in lcia_resilts:
-            scope_set_and_impact_name = self._get_scope_set_for_el(lr)
-            if scope_set_and_impact_name is None:
-                continue
-            scope_set, impact_name = scope_set_and_impact_name
-            if ImpactSet.is_allowed_field_name(impact_name):
-                impacts[impact_name] = scope_set
+    def __extract_scope(
+        self,
+        el: T_ET.Element,
+        ext: dict[str, Measurement],
+        scopes: dict[str, Measurement | dict | list],
+        unit_name: str,
+        scenario_names: dict[str, str],
+    ) -> None:
+        """Extract single scope from given element."""
+        module_name = el.attrib.get("{http://www.iai.kit.edu/EPD/2013}module") if el.attrib else None
+        module_name = self.__map_module_name(module_name)
+        scenario_name = el.attrib.get("{http://www.iai.kit.edu/EPD/2013}scenario") if el.attrib else None
+
+        if module_name is None or el.text is None:
+            return None
+        try:
+            value = float(el.text)
+        except ValueError:
+            return None
+        measurement = Measurement(mean=value, unit=unit_name)
+
+        if scenario_name is None:
+            if ScopeSet.is_allowed_field_name(module_name):  # type: ignore
+                scopes[module_name] = measurement
             else:
-                ext[impact_name] = scope_set
-        if len(ext) == 0:
-            del impacts["ext"]
-        return ImpactSet.construct(**impacts)  # type: ignore
+                ext[module_name] = measurement
+        else:
+            if not EolScenario.is_allowed_field_name(module_name) or scenario_name not in scenario_names:
+                return None
 
-    def to_openepd_impact_set(self, lang: LangDef, base_url: str | None = None) -> ImpactSet:
-        """Read as openEPD ImpactSet object."""
-        return self.get_impacts()
+            scenarios = scopes.get("C_scenarios") or list()
+            scenario: dict[str, Measurement | str] = dict(
+                name=scenario_names[scenario_name],
+            )
+            scenario[module_name] = measurement
+            scenarios.append(EolScenario.construct(**scenario))  # type: ignore
+            scopes["C_scenarios"] = scenarios
 
-    def __map_module_name(self, module_name: str | None) -> str | None:
+    @staticmethod
+    def __map_module_name(module_name: str | None) -> str | None:
         if module_name == "A1-A3":
             return "A1A2A3"
         return module_name
+
+    def _extract_and_set_scope_set(
+        self,
+        el: T_ET.Element,
+        reference_path: XmlPath,
+        scope_set_type: Type[BaseOpenEpdSchema],
+        scope_set_dict: dict[str, ScopeSet | dict],
+        ext: dict[str, ScopeSet],
+        mapper: SimpleDataMapper[str],
+        scenario_names: dict[str, str],
+    ) -> None:
+        """Extract scope set from element and set to its dictionary."""
+        scope_set_and_impact_name = self._get_scope_set_for_el(el, reference_path, mapper, scenario_names)
+        if scope_set_and_impact_name is None:
+            return None
+        scope_set, impact_name = scope_set_and_impact_name
+        if scope_set_type.is_allowed_field_name(impact_name):
+            scope_set_dict[impact_name] = scope_set
+        else:
+            ext[impact_name] = scope_set
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/material.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/source.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,77 +13,73 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Type
+from typing import IO
 
-from openepd.model.pcr import Pcr
-
-from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdPcrSupportReader
+from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader
 from ilcdlib.dto import IlcdReference
-from ilcdlib.entity.contact import IlcdContactReader
 from ilcdlib.type import LangDef
-from ilcdlib.utils import create_openepd_attachments, none_throws
+from ilcdlib.utils import none_throws
 from ilcdlib.xml_parser import T_ET
 
 
-class IlcdPcrReader(OpenEpdPcrSupportReader, IlcdXmlReader):
-    """Read an ILCD PCR XML file."""
+class IlcdSourceReader(IlcdXmlReader):
+    """Reader that can parse an ILCD Standard specification from an XML file."""
 
     def __init__(
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
-        *,
-        contact_reader_cls: Type[IlcdContactReader] = IlcdContactReader,
     ):
         super().__init__(data_provider)
-        self.contact_reader_cls = contact_reader_cls
         self._entity = element
 
-    def get_own_reference(self) -> IlcdReference | None:
-        """Get the reference to this data set."""
-        return IlcdReference(entity_type="sources", entity_id=self.get_uuid(), entity_version=self.get_version())
-
     def get_uuid(self) -> str:
         """Get the UUID of the entity described by this data set."""
         return none_throws(
             self._get_text(self._entity, ("source:sourceInformation", "source:dataSetInformation", "common:UUID"))
         )
 
     def get_version(self) -> str | None:
         """Get the version of the entity described by this data set."""
         return self._get_text(
             self._entity,
             ("source:administrativeInformation", "source:publicationAndOwnership", "common:dataSetVersion"),
         )
 
-    def get_name(self, lang: LangDef) -> str | None:
-        """Get the name of the entity described by this data set."""
-        return self._get_localized_text(
+    def get_own_reference(self) -> IlcdReference | None:
+        """Get the reference to this data set."""
+        return IlcdReference(entity_type="sources", entity_id=self.get_uuid(), entity_version=self.get_version())
+
+    def get_short_name(self, lang: LangDef) -> str | None:
+        """Get the short name of the entity described by this data set."""
+        short_name = self._get_localized_text(
             self._entity, ("source:sourceInformation", "source:dataSetInformation", "common:shortName"), lang
         )
+        return short_name
 
-    def get_reference_to_contact_reader(self) -> IlcdContactReader | None:
-        """Return the reader for the reference contact."""
-        element = self._get_external_tree(
+    def get_name(self, lang: LangDef) -> str | None:
+        """Get the full name of the entity described by this data set."""
+        return self._get_localized_text(
             self._entity,
-            (
-                "source:sourceInformation",
-                "source:dataSetInformation",
-                "source:referenceToContact",
-            ),
+            ("source:sourceInformation", "source:dataSetInformation", "source:sourceDescriptionOrComment"),
+            lang,
         )
-        return self.contact_reader_cls(element, self.data_provider) if element is not None else None
 
-    def to_openepd_pcr(self, lang: LangDef, base_url: str | None = None) -> Pcr:
-        """Read as OpenEPD Pcr object."""
-        issuer_reader = self.get_reference_to_contact_reader()
-        issuer = issuer_reader.to_openepd_org(lang) if issuer_reader is not None else None
-        return Pcr.construct(
-            name=self.get_name(lang),
-            issuer=issuer,
-            attachments=create_openepd_attachments(self.get_own_reference(), base_url),
+    def get_ref_to_digital_file(self) -> str | None:
+        """Get the link to the digital file."""
+        el = self._get_el(
+            self._entity,
+            ("source:sourceInformation", "source:dataSetInformation", "source:referenceToDigitalFile"),
         )
+        return el.attrib.get("uri") if el is not None and el.attrib is not None else None
+
+    def get_digital_file_stream(self) -> IO[bytes] | None:
+        """Get the stream to the digital file."""
+        ref = self.get_ref_to_digital_file()
+        if ref:
+            return self.data_provider.get_binary_stream_by_name(ref)
+        return None
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/entity/unit.py` & `ilcdlib-0.6.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/cli.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -83,23 +83,40 @@
             dest="save",
             action="store_true",
             help="Preserve the source document downloaded from remote location as well as the output.",
             required=False,
             default=False,
         )
         parser.add_argument(
+            "--target-dir",
+            "-t",
+            dest="target_dir",
+            type=str,
+            help="Target directory to save the output document. If not specified the current directory will be used.",
+            required=False,
+            default=None,
+        )
+        parser.add_argument(
             "--extract-pdf",
             "-e",
             dest="extract_pdf",
             action="store_true",
             help="If possible extract PDF file from the input document and save it as a separate file.",
             required=False,
             default=False,
         )
         parser.add_argument(
+            "--provider-domain",
+            dest="provider_domain",
+            type=str,
+            help="Domain name of the provider to be used in alt_ids as a key.",
+            required=False,
+            default=None,
+        )
+        parser.add_argument(
             "doc",
             metavar="doc",
             type=str,
             nargs="+",
             help="Reference to the input document. Can be a file path or URL "
             "depending on supported converter capabilities.",
         )
@@ -108,48 +125,56 @@
         in_format: str = args.in_format
         out_format: str = args.out_format
         doc_refs: list[str] = args.doc
         lang: str | None = args.lang
         dialect: str | None = args.dialect
         save: bool = args.save
         extract_pdf: bool = args.extract_pdf
+        target_dir: Path = Path(args.target_dir) if args.target_dir is not None else Path.cwd()
+        provider_domain: str | None = args.provider_domain
         if in_format.lower() != "ilcd+epd":
             CLI.fail(f"Input format {in_format} is not supported.", 1)
         if out_format.lower() != "openepd":
             CLI.fail(f"Output format {out_format} is not supported.", 1)
         if in_format.lower() == out_format.lower():
             CLI.fail(f"Input format {in_format} and output format {out_format} are the same.", 1)
         if extract_pdf and not save:
             CLI.fail("Extracting PDF requires saving the input document. Consider adding -s flag", 1)
+        if target_dir.is_file():
+            CLI.fail(f"Target directory {target_dir} is a file. It must be either dir or nor existing path.", 1)
         epd_reader_factory = EpdReaderFactory()
         if dialect is not None and not epd_reader_factory.is_dialect_supported(dialect):
             CLI.fail(f"Dialect {dialect} is not supported.", 3)
         for doc in doc_refs:
             self.process_single_doc(
                 doc,
                 epd_reader_factory,
                 dialect=dialect,
                 extract_pdf=extract_pdf,
                 in_format=in_format,
                 lang=lang,
                 out_format=out_format,
                 save=save,
+                target_dir=target_dir,
+                provider_domain=provider_domain,
             )
 
     def process_single_doc(
         self,
         doc_ref: str,
         epd_reader_factory: EpdReaderFactory,
         *,
         dialect: str | None,
         in_format: str,
         out_format: str,
         lang: str | None = None,
         extract_pdf: bool = False,
         save: bool = False,
+        target_dir: Path | None = None,
+        provider_domain: str | None = None,
     ) -> None:
         CLI.print_info(f"Converting document {doc_ref} from {in_format} to {out_format}.")
         reader_cls, dialect = (
             (epd_reader_factory.get_reader_class(dialect), dialect)
             if dialect
             else epd_reader_factory.autodiscover_by_url(doc_ref)
         )
@@ -170,33 +195,48 @@
                 4,
             )
         lang_list = [lang, None]
         if prioritize_english:
             lang_list.insert(0, "en")
         CLI.print_info("Language priority: " + ",".join([x if x is not None else "any other" for x in lang_list]))
         base_url = self.__extract_base_url(doc_ref)
-        open_epd = epd_reader.to_openepd_epd(lang_list, base_url=base_url)
-        if isinstance(medium, Soda4LcaZipReader):
-            open_epd.set_ext_field("ilcd_pdf_url", medium.get_pdf_url())
+        open_epd = epd_reader.to_openepd_epd(lang_list, base_url=base_url, provider_domain=provider_domain)
         CLI.print_data(open_epd.json(indent=2, exclude_none=True, exclude_unset=True))
         if save:
-            self.save_results(epd_reader, open_epd, extract_pdf=extract_pdf)
+            self.save_results(epd_reader, open_epd, extract_pdf=extract_pdf, base_dir=target_dir)
 
-    def save_results(self, epd_reader: IlcdEpdReader, result: Epd, *, extract_pdf: bool = False):
-        output_dir = Path(epd_reader.get_uuid())
+    def save_results(
+        self, epd_reader: IlcdEpdReader, result: Epd, *, extract_pdf: bool = False, base_dir: Path | None = None
+    ):
+        if base_dir is None:
+            base_dir = Path.cwd()
+        output_dir = base_dir / Path(epd_reader.get_uuid())
         ensure_dir(output_dir)
         with open(output_dir / "openEPD.json", "w") as f:
             f.write(result.json(indent=2, exclude_none=True, exclude_unset=True))
         if isinstance(epd_reader.data_provider, ZipIlcdReader):
             epd_reader.data_provider.save_to(output_dir / "ilcd_epd.zip")
         if extract_pdf:
+            # EPD Pdf
             pdf_stream = epd_reader.get_epd_document_stream()
+            if pdf_stream is None and isinstance(epd_reader.data_provider, Soda4LcaZipReader):
+                try:
+                    pdf_stream = epd_reader.data_provider.download_pdf()
+                except ValueError:
+                    pdf_stream = None
             if pdf_stream is not None:
-                with open(output_dir / "original.pdf", "wb") as f:
+                with open(output_dir / "original.pdf", "wb") as f, pdf_stream:
                     f.write(pdf_stream.read())
+            # PCR PDF
+            pcr_reader = epd_reader.get_pcr_reader()
+            if pcr_reader:
+                pdf_stream = pcr_reader.get_digital_file_stream()
+                if pdf_stream:
+                    with open(output_dir / "pcr.pdf", "wb") as f, pdf_stream:
+                        f.write(pdf_stream.read())
         CLI.print_info("Output saved to " + str(output_dir.absolute()))
 
     def __extract_base_url(self, doc_ref: str) -> str | None:
         if doc_ref.startswith("http"):
             if "/datasetdetail/" in doc_ref:
                 return doc_ref.split("/datasetdetail/", 1)[0]
             elif "/resource/" in doc_ref:
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-0.6.0/src/ilcdlib/sanitizing/phone.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,17 +13,24 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from ilcdlib.epd.reader import IlcdEpdReader
+import re
 
+PHONE_REGEX = re.compile(r"[+\d\s\-()]+", re.IGNORECASE)
 
-class OekobauDatIlcdXmlEpdReader(IlcdEpdReader):
-    """Reader for EPDs in the Oekobau.DAT specific ILCD XML format."""
 
-    @classmethod
-    def is_known_url(cls, url: str) -> bool:
-        """Return whether the URL recognized as a known Environdec URL."""
-        return "oekobaudat" in url.lower()
+def cleanup_phone(phone: str | None) -> str | None:
+    """
+    Try to perform cleanup of the given phone number.
+
+    E.g. if the input is `Tel: +49 (0) 123 456 789 blah`, the output will be ``+49 (0) 123 456 789``.
+    """
+    if phone is None:
+        return None
+    for m in sorted(PHONE_REGEX.findall(phone), key=lambda x: len(x), reverse=True):
+        if len(m.strip()) > 0:
+            return m.strip()
+    return phone
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/factory.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/epd/reader.py` & `ilcdlib-0.6.0/src/ilcdlib/epd/reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,28 +18,40 @@
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
 from typing import IO, Sequence, Type
 
 from openepd.model.common import Amount, Measurement
 from openepd.model.epd import Epd
-from openepd.model.lcia import ImpactSet
+from openepd.model.lcia import Impacts, ImpactSet, OutputFlowSet, ResourceUseSet
+from openepd.model.org import Org
 from openepd.model.specs import Specs
+from openepd.model.standard import Standard
 
 from ilcdlib import const
 from ilcdlib.common import BaseIlcdMediumSpecificReader, IlcdXmlReader, OpenEpdEdpSupportReader
 from ilcdlib.const import IlcdDatasetType
-from ilcdlib.dto import IlcdReference, ProductClassDef
+from ilcdlib.dto import ComplianceDto, IlcdReference, ProductClassDef
+from ilcdlib.entity.compliance import IlcdComplianceListReader
 from ilcdlib.entity.contact import IlcdContactReader
+from ilcdlib.entity.exchage import IlcdExchangesReader
 from ilcdlib.entity.flow import IlcdExchangeDto, IlcdFlowReader
 from ilcdlib.entity.lcia import IlcdLciaResultsReader
 from ilcdlib.entity.material import MatMlMaterial
 from ilcdlib.entity.pcr import IlcdPcrReader
+from ilcdlib.extension import Ec3EpdExtension, IlcdEpdExtension
+from ilcdlib.mapping.compliance import StandardNameToLCIAMethodMapper, default_standard_names_to_lcia_mapper
 from ilcdlib.type import LangDef
-from ilcdlib.utils import create_ext, create_openepd_attachments, none_throws
+from ilcdlib.utils import (
+    MarkdownSectionBuilder,
+    create_ext,
+    create_openepd_attachments,
+    none_throws,
+    provider_domain_name_from_url,
+)
 
 
 class IlcdEpdReader(OpenEpdEdpSupportReader, IlcdXmlReader):
     """Reader for ILCD+EPD datasets."""
 
     def __init__(
         self,
@@ -47,20 +59,26 @@
         epd_version: str | None,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
         contact_reader_cls: Type[IlcdContactReader] = IlcdContactReader,
         pcr_reader_cls: Type[IlcdPcrReader] = IlcdPcrReader,
         flow_reader_cls: Type[IlcdFlowReader] = IlcdFlowReader,
         lcia_results_reader_cls: Type[IlcdLciaResultsReader] = IlcdLciaResultsReader,
+        exchanges_reader_cls: Type[IlcdExchangesReader] = IlcdExchangesReader,
+        compliance_reader_cls: Type[IlcdComplianceListReader] = IlcdComplianceListReader,
+        standard_names_to_lcia_mapper: StandardNameToLCIAMethodMapper = default_standard_names_to_lcia_mapper,
     ):
         super().__init__(data_provider)
         self.contact_reader_cls = contact_reader_cls
         self.pcr_reader_cls = pcr_reader_cls
         self.flow_reader_cls = flow_reader_cls
         self.lcia_results_reader_cls = lcia_results_reader_cls
+        self.compliance_reader_cls = compliance_reader_cls
+        self.exchanges_reader_cls = exchanges_reader_cls
+        self.standard_names_to_lcia_mapper = standard_names_to_lcia_mapper
         if epd_process_id is None:
             entities = data_provider.list_entities(IlcdDatasetType.Processes)
             self.__epd_entity_ref = entities[0]
         else:
             self.__epd_entity_ref = IlcdReference(IlcdDatasetType.Processes, epd_process_id, epd_version)
         self.epd_el_tree = self.get_xml_tree(*self.__epd_entity_ref, allow_static_datasets=False)
         self.post_init()
@@ -110,23 +128,24 @@
             self._get_text(
                 self.epd_el_tree,
                 ("process:modellingAndValidation", "process:LCIMethodAndAllocation", "process:typeOfDataSet"),
             )
             == "EPD"
         )
 
+    def get_dataset_type(self) -> str | None:
+        """Return the ILCD dataset type. e.g. 'average dataset', 'industry dataset', 'generic dataset', etc."""
+        return self._get_text(
+            self.epd_el_tree,
+            ("process:modellingAndValidation", "process:LCIMethodAndAllocation", "common:other", "epd2013:subType"),
+        )
+
     def is_industry_epd(self):
         """Return True if the dataset represents an industry EPD."""
-        return (
-            self._get_text(
-                self.epd_el_tree,
-                ("process:modellingAndValidation", "process:LCIMethodAndAllocation", "common:other", "epd2013:subType"),
-            )
-            == "average dataset"
-        )
+        return self.get_dataset_type() == "average dataset"
 
     def get_epd_document_stream(self) -> IO[bytes] | None:
         """Extract the EPD document."""
         return self._get_external_binary(
             self.epd_el_tree,
             (
                 "process:modellingAndValidation",
@@ -153,22 +172,26 @@
                 "process:dataSetInformation",
                 "process:name",
                 "process:functionalUnitFlowProperties",
             ),
             lang,
         )
 
-    def get_product_description(self, lang: LangDef) -> str | None:
-        """Return the product description in the given language."""
+    def get_general_comment(self, lang: LangDef) -> str | None:
+        """Return the general comment in the given language."""
         return self._get_localized_text(
             self.epd_el_tree,
             ("process:processInformation", "process:dataSetInformation", "common:generalComment"),
             lang,
         )
 
+    def get_product_description(self, lang: LangDef) -> str | None:
+        """Return the product description in the given language."""
+        return self.get_general_comment(lang)
+
     def get_date_published(self) -> datetime.date | None:
         """Return the date the EPD was published."""
         pub_date = self._get_date(
             self.epd_el_tree,
             ("process:processInformation", "process:time", "common:other", "epd2019:publicationDateOfEPD"),
         )
         if pub_date is None:
@@ -201,14 +224,89 @@
         )
         if pub_date is not None and valid_until_year is not None:
             return pub_date.replace(year=valid_until_year)
         elif valid_until_year is not None:
             return datetime.date(year=valid_until_year, month=1, day=1)
         return None
 
+    def get_technology_description(self, lang: LangDef) -> str | None:
+        """
+        Return the technology description in the given language.
+
+        Description of the technological characteristics including operating conditions
+        of the process or product system.
+        """
+        return self._get_localized_text(
+            self.epd_el_tree,
+            ("process:processInformation", "process:technology", "process:technologyDescriptionAndIncludedProcesses"),
+            lang,
+        )
+
+    def get_technological_applicability(self, lang: LangDef) -> str | None:
+        """
+        Return the technological applicability in the given language.
+
+        Description of the technological applicability of the process or product system.
+        """
+        return self._get_localized_text(
+            self.epd_el_tree,
+            ("process:processInformation", "process:technology", "process:technologicalApplicability"),
+            lang,
+        )
+
+    def get_dataset_use_advice(self, lang: LangDef) -> str | None:
+        """
+        Return the dataset use advice in the given language.
+
+        Specific methodological advice for use of the data set as application options (e.g. data set shall be used
+        for LCA of buildings) or restrictions (e.g. data set shall not be used for products produced in 'wet process').
+        """
+        return self._get_localized_text(
+            self.epd_el_tree,
+            (
+                "process:modellingAndValidation",
+                "process:dataSourcesTreatmentAndRepresentativeness",
+                "process:useAdviceForDataSet",
+            ),
+            lang,
+        )
+
+    def get_lca_discussion(self, lang: LangDef) -> str | None:
+        """Return the product lca discussion in the given language. See openEPD/lca_discussion field docs."""
+        mb = MarkdownSectionBuilder()
+        mb.add_section("Use Advice", self.get_dataset_use_advice(lang))
+        mb.add_section("Technology Description And Included Processes", self.get_technology_description(lang))
+        mb.add_section("Location description of restrictions", self.get_location_description_of_restrictions(lang))
+        return mb.build()
+
+    def get_location_description_of_restrictions(self, lang: LangDef) -> str | None:
+        """Return the location description of restrictions in the given language."""
+        return self._get_localized_text(
+            self.epd_el_tree,
+            (
+                "process:processInformation",
+                "process:geography",
+                "process:locationOfOperationSupplyOrProduction",
+                "process:descriptionOfRestrictions",
+            ),
+            lang,
+        )
+
+    def get_production_location(self) -> str | None:
+        """Return production regions in the given language."""
+        el = self._get_el(
+            self.epd_el_tree,
+            ("process:processInformation", "process:geography", "process:locationOfOperationSupplyOrProduction"),
+        )
+
+        if el is None:
+            return None
+
+        return el.attrib.get("location") if el.attrib else None
+
     def get_external_verifier_reader(self) -> IlcdContactReader | None:
         """Return the reader for the reviewer."""
         element = self._get_external_tree(
             self.epd_el_tree,
             (
                 "process:modellingAndValidation",
                 "process:validation",
@@ -226,14 +324,87 @@
                 "process:administrativeInformation",
                 "process:publicationAndOwnership",
                 "common:referenceToOwnershipOfDataSet",
             ),
         )
         return self.contact_reader_cls(element, self.data_provider) if element is not None else None
 
+    def get_publisher_reader(self) -> IlcdContactReader | None:
+        """Return the reader for the publisher."""
+        element = self._get_external_tree(
+            self.epd_el_tree,
+            (
+                "process:administrativeInformation",
+                "process:publicationAndOwnership",
+                "common:other",
+                "epd2019:referenceToPublisher",
+            ),
+        )
+
+        if element is None:
+            element = self._get_external_tree(
+                self.epd_el_tree,
+                (
+                    "process:administrativeInformation",
+                    "common:commissionerAndGoal",
+                    "common:referenceToCommissioner",
+                ),
+            )
+
+        return self.contact_reader_cls(element, self.data_provider) if element is not None else None
+
+    def get_data_entry_by_reader(self) -> IlcdContactReader | None:
+        """Return the reader for the data entry by."""
+        element = self._get_external_tree(
+            self.epd_el_tree,
+            (
+                "process:administrativeInformation",
+                "process:dataEntryBy",
+                "common:referenceToPersonOrEntityEnteringTheData",
+            ),
+        )
+        return self.contact_reader_cls(element, self.data_provider) if element is not None else None
+
+    def get_data_entry_by(self, lang: LangDef, base_url: str | None = None) -> Org | None:
+        """Return the data entry by org."""
+        data_entry_by_reader = self.get_data_entry_by_reader()
+        return data_entry_by_reader.to_openepd_org(lang, base_url) if data_entry_by_reader else None
+
+    def get_compliance_reader(self) -> IlcdComplianceListReader | None:
+        """Return the reader for the standard included in compliance declarations."""
+        element = self._get_el(
+            self.epd_el_tree,
+            (
+                "process:modellingAndValidation",
+                "process:complianceDeclarations",
+            ),
+        )
+        return self.compliance_reader_cls(element, self.data_provider) if element is not None else None
+
+    def get_compliance_declarations(self, lang: LangDef, base_url: str | None = None) -> list[ComplianceDto]:
+        """Return list of compliance data."""
+        reader = self.get_compliance_reader()
+        if reader is None:
+            return []
+        return reader.get_compliances(lang, base_url)
+
+    def get_openepd_compliance(self, lang: LangDef, base_url: str | None = None) -> list[Standard]:
+        """Return list of OpenEPD Standards."""
+        result = []
+        for compliance in self.get_compliance_declarations(lang, base_url):
+            result.append(
+                Standard.construct(
+                    short_name=compliance.short_name,
+                    name=compliance.name,
+                    link=compliance.link,  # FIXME: incompatible type "Optional[str]"; expected "Optional[AnyUrl]"
+                    issuer=compliance.issuer,
+                )
+            )
+        return result
+
     def get_pcr_reader(self) -> IlcdPcrReader | None:
         """Return the reader for the PCR."""
         element = self._get_external_tree(
             self.epd_el_tree,
             (
                 "process:modellingAndValidation",
                 "process:LCIMethodAndAllocation",
@@ -337,14 +508,41 @@
             return None
         exchange_dto = IlcdExchangeDto(
             mean_value=self._get_float(exchange_element, ("process:meanAmount",)),
             flow_dataset_reader=self.flow_reader_cls(flow_dataset_el, self.data_provider),
         )
         return exchange_dto
 
+    def get_scenario_names(self, lang: LangDef) -> dict[str, str]:
+        """Return dictionary with mapping short scenario names to full names in given language."""
+        scenarios = self._get_all_els(
+            self.epd_el_tree,
+            (
+                "process:processInformation",
+                "process:dataSetInformation",
+                "common:other",
+                "epd2013:scenarios",
+                "epd2013:scenario",
+            ),
+        )
+
+        result: dict[str, str] = dict()
+
+        for scenario in scenarios:
+            if not scenario.attrib:
+                continue
+
+            short_name = scenario.attrib.get("{http://www.iai.kit.edu/EPD/2013}name")
+            name = self._get_localized_text(scenario, ("epd2013:description",), lang)
+
+            if name and short_name:
+                result[short_name] = name
+
+        return result
+
     def get_declared_unit(self) -> Amount | None:
         """Return the reader for the flow."""
         exchange_dto = self.get_product_flow()
         if exchange_dto is None:
             return None
         reference_flow_property = none_throws(exchange_dto.flow_dataset_reader).get_reference_flow_property()
         if reference_flow_property is None:
@@ -367,46 +565,83 @@
         """Return the LCIA results reader."""
         element = self._get_el(
             self.epd_el_tree,
             ("process:LCIAResults",),
         )
         return self.lcia_results_reader_cls(element, self.data_provider) if element is not None else None
 
-    def get_lcia_results(self) -> ImpactSet | None:
+    def get_exchanges_reader(self) -> IlcdExchangesReader | None:
+        """Return the LCIA results reader."""
+        element = self._get_el(
+            self.epd_el_tree,
+            ("process:exchanges",),
+        )
+        return self.exchanges_reader_cls(element, self.data_provider) if element is not None else None
+
+    def get_lcia_results(self, scenario_names: dict[str, str]) -> ImpactSet | None:
+        """Return the LCIA results."""
+        reader = self.get_lcia_results_reader()
+        if reader is None:
+            return None
+        return reader.get_impact_set(scenario_names)
+
+    def get_impacts(self, scenario_names: dict[str, str], lca_method: str | None = None) -> Impacts | None:
         """Return the LCIA results."""
         reader = self.get_lcia_results_reader()
         if reader is None:
             return None
-        return reader.get_impacts()
+        return reader.to_openepd_impacts(scenario_names, lcia_method=lca_method)
+
+    def get_resource_uses(self, scenario_names: dict[str, str]) -> ResourceUseSet | None:
+        """Return resource uses."""
+        reader = self.get_exchanges_reader()
+        if reader is None:
+            return None
+        return reader.get_resource_uses(scenario_names)
+
+    def get_output_flows(self, scenario_names: dict[str, str]) -> OutputFlowSet | None:
+        """Return output flows."""
+        reader = self.get_exchanges_reader()
+        if reader is None:
+            return None
+        return reader.get_output_flows(scenario_names)
 
     def _product_classes_to_openepd(self, classes: dict[str, list[ProductClassDef]]) -> dict[str, str]:
         result: dict[str, str] = {}
         for classification_name, class_defs in classes.items():
-            if classification_name.lower() == "oekobau.dat":
-                result["oekobau.dat"] = none_throws(class_defs[-1].id)
-            elif classification_name.lower() == "ibucategories":
-                result["IBU"] = " >> ".join([none_throws(x.name) for x in class_defs])
             if len(class_defs) > 0:
-                result[const.ILCD_IDENTIFICATION[0]] = (
+                result[classification_name] = (
                     (class_defs[-1].id or "") + " " + " / ".join([none_throws(x.name) for x in class_defs])
                 ).strip()
         return result
 
-    def to_openepd_epd(self, lang: LangDef, base_url: str | None = None) -> Epd:  # NOSONAR
+    def to_openepd_epd(
+        self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
+    ) -> Epd:  # NOSONAR
         """Return the EPD as OpenEPD object."""
+        if provider_domain is None:
+            provider_domain = provider_domain_name_from_url(base_url)
         lang_code = lang if isinstance(lang, str) else None
         if isinstance(lang, Sequence):
             lang_code = lang[0] if len(lang) > 0 else None
         manufacturer_reader = self.get_manufacturer_reader()
-        manufacturer = manufacturer_reader.to_openepd_org(lang, base_url) if manufacturer_reader else None
+        manufacturer = (
+            manufacturer_reader.to_openepd_org(lang, base_url, provider_domain) if manufacturer_reader else None
+        )
+        publisher_reader = self.get_publisher_reader()
+        publisher = publisher_reader.to_openepd_org(lang, base_url, provider_domain) if publisher_reader else None
         program_operator_reader = self.get_program_operator_reader()
-        program_operator = program_operator_reader.to_openepd_org(lang, base_url) if program_operator_reader else None
+        program_operator = (
+            program_operator_reader.to_openepd_org(lang, base_url, provider_domain) if program_operator_reader else None
+        )
         external_verifier_reader = self.get_external_verifier_reader()
         external_verifier = (
-            external_verifier_reader.to_openepd_org(lang, base_url) if external_verifier_reader else None
+            external_verifier_reader.to_openepd_org(lang, base_url, provider_domain)
+            if external_verifier_reader
+            else None
         )
         pcr_reader = self.get_pcr_reader()
         pcr = pcr_reader.to_openepd_pcr(lang, base_url) if pcr_reader else None
         declared_unit = self.get_declared_unit()
         quantitative_props = self.get_quantitative_product_props_str(lang)
         own_ref = self.get_own_reference()
         product_name = self.get_product_name(lang)
@@ -421,33 +656,68 @@
             product_properties.update(
                 {n: (str(v.mean) + " " + v.unit if v.unit else "").strip() for n, v in other_product_props.items()}
             )
         if product_properties:
             specs = Specs(ext=create_ext(product_properties))
         else:
             specs = Specs()
-        return Epd.construct(
+        scenario_names = self.get_scenario_names(lang)
+
+        compliance = self.get_openepd_compliance(lang, base_url)
+        lcia_method: str | None = None
+        for c in compliance:
+            mapped = self.standard_names_to_lcia_mapper.map(c.short_name, None)
+            if mapped:
+                lcia_method = mapped
+                break
+
+        epd = Epd.construct(
             doctype="openEPD",
             language=lang_code,
-            attachments=create_openepd_attachments(own_ref, base_url),
+            attachments=create_openepd_attachments(own_ref, base_url) if base_url else None,
             declaration_url=own_ref.to_url(base_url) if own_ref and base_url else None,
-            name=product_name,
-            description=self.get_product_description(lang),
+            product_name=product_name,
+            product_description=self.get_product_description(lang),
             date_published=self.get_date_published(),
             valid_until=self.get_validity_ends_date(),
             program_operator_doc_id=self.get_program_operator_id(),
             manufacturer=manufacturer,
             program_operator=program_operator,
-            product_class=self._product_classes_to_openepd(self.get_product_classes()),
+            product_classes=self._product_classes_to_openepd(self.get_product_classes()),
+            manufacturing_description=self.get_technology_description(lang),
+            product_usage_description=self.get_technological_applicability(lang),
+            lca_discussion=self.get_lca_discussion(lang),
             third_party_verifier=external_verifier,
             pcr=pcr,
             declared_unit=declared_unit,
-            impacts=self.get_lcia_results(),
+            impacts=self.get_impacts(scenario_names, lca_method=lcia_method),
+            resource_uses=self.get_resource_uses(scenario_names),
+            output_flows=self.get_output_flows(scenario_names),
             specs=specs,
+            compliance=compliance,
         )
+        if own_ref:
+            epd.set_alt_id(provider_domain, own_ref.entity_id)
+
+        pdf_url = self.data_provider.get_pdf_url()
+        epd.set_attachment_if_any(const.PDF_ATTACHMENT, pdf_url)
+
+        ilcd_ext = IlcdEpdExtension(
+            dataset_type=self.get_dataset_type(),
+            dataset_version=self.get_version(),
+            dataset_uuid=self.get_uuid(),
+            production_location=self.get_production_location(),
+        )
+        ec3_ext = Ec3EpdExtension.construct(
+            epd_developer=self.get_data_entry_by(lang, base_url),
+            epd_publisher=publisher,
+        )
+        epd.set_ext(ilcd_ext)
+        epd.set_ext(ec3_ext)
+        return epd
 
     @classmethod
     def is_known_url(cls, url: str) -> bool:
         """
         Return whether the URL recognized by this particular reader.
 
         This method should be overriden by the dialect and return true if the input URL is know url for this dialect.
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/http_common.py` & `ilcdlib-0.6.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/mapping/common.py` & `ilcdlib-0.6.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-0.6.0/src/ilcdlib/mapping/impacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
         "06dcd26f-025f-401a-a7c1-5e457eb54637": "odp",
         "1e84a202-dae6-42aa-9e9d-71ea48b8be00": "pocp",
         "b5c611c6-def3-11e6-bf01-fe55135034f3": "ap",
         "b4274add-93b7-4905-a5e4-2e878c4e4216": "ap",
         "b53ec18f-7377-4ad3-86eb-cc3f4f276b2b": "ep-fresh",
         "f58827d0-b407-4ec6-be75-8b69efb98a0f": "ep-fresh",
         "b5c619fa-def3-11e6-bf01-fe55135034f3": "ep-marine",
-        "b5c614d2-def3-11e6-bf01-fe55135034f3": "ep-terrestrial",
+        "b5c614d2-def3-11e6-bf01-fe55135034f3": "ep-terr",
         "b2ad66ce-c78d-11e6-9d9d-cec0c932ce01": "WDP",
     }
 
 
 default_impacts_uuid_mapper = ImpactsUUIDToOpenIdMapper()
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-0.6.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/mapping/units.py` & `ilcdlib-0.6.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/medium/archive.py` & `ilcdlib-0.6.0/src/ilcdlib/medium/archive.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         IlcdDatasetType.Processes: "processes",
         IlcdDatasetType.FlowProperty: "flowproperties",
     }
 
     def __init__(self, zip_file: PathLike | IO[bytes]):
         try:
             self._zip_file = ZipFile(zip_file, "r")
-            self._zip_file
         except Exception:
             raise ValueError("Could not open zip file. Please check if this is a valid zip file.")
         self.__ilcd_dir = ZipPath(self._zip_file) / "ILCD"
         if not self.__ilcd_dir.is_dir():
             raise ValueError("Could not find ILCD directory in the archive root. Is it really an ILCD archive?")
 
     @overload
@@ -80,14 +79,26 @@
         :raise: ValueError if the entity does not exist.
         """
         full_path = self.__resolve_entity_path(entity_type, entity_id, entity_version)
         if full_path is None or not full_path.exists():
             raise ValueError(f"Could not find entity {entity_type} {entity_id} (version {entity_version}).")
         return full_path.open("rb" if binary else "r")  # type: ignore
 
+    def get_binary_stream_by_name(self, name: str, entity_type: str | None = None) -> IO[bytes] | None:
+        """
+        Get binary stream for the given file name.
+
+        :param name: The name of the file.
+        :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
+        """
+        full_path = self.__ilcd_dir / "external_docs" / name
+        if not full_path.exists():
+            return None
+        return full_path.open("rb")
+
     def entity_exists(self, entity_type: str, entity_id: str, entity_version: str | None = None) -> bool:
         """
         Check if the given entity exists.
 
         If you want to refer file by name only, you can use the entity_id and skip version parameter.
 
         :param entity_type: The type of the entity. e.g. "process", "contact", "flow", etc.
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-0.6.0/src/ilcdlib/medium/soda4lca.py`

 * *Files 18% similar despite different names*

```diff
@@ -69,41 +69,49 @@
         try:
             parsed_url = parse_url(endpoint)
             parsed_qs = parse_qs(parsed_url.query)
         except ValueError as e:
             raise ValueError(f"Invalid endpoint {endpoint}") from e
         host: str = none_throws(parsed_url.scheme) + "://" + none_throws(parsed_url.host)
         base_url = host
-        url_path = "/resource"
         uuid: str | None = None
+        datastock: str | None = None
         resource_type_name: str | None = None
         original_path = parsed_url.path or ""
+        url_path = "/resource"
+        if url_path in original_path:
+            base_path_prefix = original_path.split("/resource", 1)[0]
+            url_path = base_path_prefix + url_path if len(base_path_prefix) > 0 else url_path
         if original_path.endswith(".xhtml"):
             resource_type_name = original_path.rsplit("/", 1)[-1].replace(".xhtml", "").lower()
             resource_type_name = cls.__map_type_name(resource_type_name)
             uuid = parsed_qs.pop("uuid", [None])[0]  # type: ignore
             if "/datasetdetail" in original_path:
                 url_path = original_path.split("/datasetdetail", 1)[0] + url_path
         else:
             path_components = original_path.split("/")
             for i, x in enumerate(path_components):
                 if x == "resource":
                     if i + 2 > len(path_components):
                         raise ValueError(f"Invalid endpoint {endpoint}")
                     resource_type_name = path_components[i + 1]
                     uuid = path_components[i + 2]
+                    if resource_type_name == "datastocks":
+                        datastock = uuid
+                        resource_type_name = path_components[i + 3]
+                        uuid = path_components[i + 4]
                     break
         if uuid is None or resource_type_name is None:
             raise ValueError(f"Invalid endpoint {endpoint}")
         version: str | None = parsed_qs.pop("version", [None])[0]  # type: ignore
-        stock: str | None = parsed_qs.pop("datastock", [None])[0]  # type: ignore
+        datastock = parsed_qs.pop("datastock", [None])[0] if datastock is None else datastock  # type: ignore
         base_url += url_path
         return IlcdRemotePointer(
             base_url=base_url,
-            stock=stock,
+            stock=datastock,
             ref=IlcdReference(entity_type=resource_type_name, entity_version=version, entity_id=uuid),
         )
 
     def dowload_zip_archive(self, url: str) -> IO[bytes]:
         """Download a zip archive from a URL."""
         # TODO: Move this to dedicated class
         response = http.request("GET", url)
@@ -111,14 +119,35 @@
             return io.BytesIO(response.data)
         raise ValueError(f"Could not download zip archive from {url}. Status code: {response.status}")
 
     def get_pdf_url(self) -> str | None:
         """Get the URL to the PDF document if any."""
         return self._soda4lca_client.get_download_epd_document_link(self._ref.entity_id, self._ref.entity_version)
 
+    def download_pdf(self) -> IO[bytes] | None:
+        """Download the associated PDF document if any."""
+        url = self.get_pdf_url()
+        if url is None:
+            return None
+        response = http.request("GET", url)
+        if response.status == 200:
+            return io.BytesIO(response.data)
+        raise ValueError(f"Could not download PDF from {url}. Status code: {response.status}")
+
+    def resolve_entity_url(self, ref: IlcdReference, digital_file: str | None) -> str | None:
+        """
+        Resolve the url of the given entity.
+
+        If `digital_file` parameter is set, the link to the associated digital file is returned.
+
+        :param ref: reference to the entity
+        :param digital_file: optional name of the file, if link to the file is needed.
+        """
+        return self._soda4lca_client.get_entity_url(ref, digital_file=digital_file, verify=False)
+
     @staticmethod
     def __map_type_name(in_: str) -> str:
         match in_:
             case "process" | "showprocess":
                 return "processes"
             case _:
                 return in_
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/reference_data.py` & `ilcdlib-0.6.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-0.6.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-0.6.0/src/ilcdlib/type.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,24 +13,21 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-import re
+from typing import Sequence
 
-PHONE_REGEX = re.compile(r"[+\d\s\-()]+", re.IGNORECASE)
+LangDef = str | Sequence[str | None] | None
 
 
-def cleanup_phone(phone: str | None) -> str | None:
-    """
-    Try to perform cleanup of the given phone number.
+class LocalizedStr(str):
+    """A string with language code attached."""
 
-    E.g. if the input is `Tel: +49 (0) 123 456 789 blah`, the output will be ``+49 (0) 123 456 789``.
-    """
-    if phone is None:
-        return None
-    for m in sorted(PHONE_REGEX.findall(phone), key=lambda x: len(x), reverse=True):
-        if len(m.strip()) > 0:
-            return m.strip()
-    return phone
+    def __new__(cls, *args, **kwargs):  # noqa: D102
+        return super().__new__(cls, args[0])
+
+    def __init__(self, s: str, lang: str | None = None):
+        super().__init__()
+        self.lang: str | None = lang
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-0.6.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-0.6.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,18 +90,34 @@
 
         :param str process_uuid: UUID of the process
         :param str version: version of the process (optional)
         """
         params = dict()
         if version is not None:
             params["version"] = version
-        url = f"{self.base_url}/processes/{self._urlencode(process_uuid)}/epd" + "?" + urlencode(params)
+        url = f"{self.base_url}/processes/{self._urlencode(process_uuid)}/epd"
+        if params:
+            url += "?" + urlencode(params)
         response = self._do_request("head", url, raise_for_status=False)
         return url if response.ok else None
 
+    def get_entity_url(self, ref: IlcdReference, digital_file: str | None, verify: bool = False) -> str | None:
+        """Get URL to download an ILCD entity or a digital file attached to it."""
+        params = dict()
+        if ref.entity_version is not None:
+            params["version"] = ref.entity_version
+        url = f"{self.base_url}/{ref.entity_type}/{self._urlencode(ref.entity_id)}"
+        if digital_file is not None:
+            url += f"/{self._urlencode(digital_file)}"
+        url += "?" + urlencode(params)
+        if verify:
+            response = self._do_request("head", url, raise_for_status=False)
+            return url if response.ok else None
+        return url
+
     def download_epd_document(self, process_uuid: str, version: str | None = None) -> IO[bytes]:
         """
         Download an EPD document (typically in PDF format).
 
         :param str process_uuid: UUID of the process
         :param str version: version of the process (optional)
         :raise NotFoundError: if the process file does not exist
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/type.py` & `ilcdlib-0.6.0/src/ilcdlib/mapping/compliance.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import Sequence
+from ilcdlib.mapping.common import SimpleDataMapper
 
-LangDef = str | Sequence[str | None] | None
 
+class StandardNameToLCIAMethodMapper(SimpleDataMapper[str | None]):
+    """Map standard name to LCIA method."""
 
-class LocalizedStr(str):
-    """A string with language code attached."""
+    DATABASE = {
+        "EN 15804+A2": "EF 3.0",
+        "EN 15804+A1": "EF 3.0",
+    }
 
-    def __new__(cls, *args, **kwargs):  # noqa: D102
-        return super().__new__(cls, args[0])
 
-    def __init__(self, s: str, lang: str | None = None):
-        super().__init__()
-        self.lang: str | None = lang
+default_standard_names_to_lcia_mapper = StandardNameToLCIAMethodMapper()
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/utils.py` & `ilcdlib-0.6.0/src/ilcdlib/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-from typing import TYPE_CHECKING, Any, Optional, TypeVar
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Optional, Self, TypeVar
 
 from ilcdlib import const
+from ilcdlib.sanitizing.domain import domain_from_url
 
 T = TypeVar("T")
 
 if TYPE_CHECKING:
     from ilcdlib.dto import IlcdReference
 
 
@@ -46,12 +48,49 @@
 ) -> dict[str, str] | None:
     """Create a dictionary of OpenEPD attachments."""
     if reference is None:
         return None
     return {x: reference.to_url(base_url) for x in const.ILCD_IDENTIFICATION}
 
 
+def provider_domain_name_from_url(url: str | None) -> str:
+    """Return provider identifier from the given URL. If the URL is `None`, return the default value."""
+    if url:
+        return none_throws(domain_from_url(url))
+    return const.ILCD_IDENTIFICATION[0]
+
+
 def create_ext(data: Any) -> dict[str, Any] | None:
     """Create a dictionary of OpenEPD ext field."""
     if data is None:
         return None
     return {x: data for x in const.ILCD_IDENTIFICATION}
+
+
+class MarkdownSectionBuilder:
+    """
+    A builder for Markdown sections.
+
+    Allows to build a Markdown string from a list of sections (title + content).
+    """
+
+    @dataclass(kw_only=True)
+    class _MdSection:
+        title: str
+        level: int = 1
+        content: str | None = None
+
+    def __init__(self) -> None:
+        self._sections: list[MarkdownSectionBuilder._MdSection] = []
+
+    def add_section(self, title: str, content: str | None = None, level: int = 1) -> Self:
+        """Add a new section to the builder."""
+        self._sections.append(MarkdownSectionBuilder._MdSection(title=title, content=content, level=level))
+        return self
+
+    @staticmethod
+    def _build_section(section: _MdSection) -> str:
+        return f"{'#' * section.level} {section.title}\n\n{section.content or ''}"
+
+    def build(self) -> str:
+        """Build the Markdown string."""
+        return "\n\n".join([self._build_section(x) for x in self._sections if x.content is not None])
```

### Comparing `ilcdlib-0.5.0/src/ilcdlib/xml_parser.py` & `ilcdlib-0.6.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-0.5.0/PKG-INFO` & `ilcdlib-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 0.5.0
+Version: 0.6.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: lxml
 Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml"
-Requires-Dist: openepd (>=0.5.0,<1.0.0)
+Requires-Dist: openepd (>=0.10.0,<1.0.0)
 Requires-Dist: requests (>=2.1.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
 Description-Content-Type: text/markdown
 
 # ILCD Lib
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 0.5.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 0.6.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: support@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Provides-Extra: cli
 Provides-Extra: lxml Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml" Requires-Dist: openepd
-(>=0.5.0,<1.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
+(>=0.10.0,<1.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
 urllib3 (>=1.26.16,<2.0.0) Project-URL: Repository, https://github.com/
 cchangelabs/ilcdlib Description-Content-Type: text/markdown # ILCD Lib
      [https://img.shields.io/pypi/l/ilcdlib?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/ilcdlib?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/ilcdlib?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/ilcdlib?style=for-the-badge]
```

