# Comparing `tmp/pydantic_xmlmodel-0.3.tar.gz` & `tmp/pydantic_xmlmodel-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.3.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.3.1.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.3.tar` & `pydantic_xmlmodel-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3/LICENSE
--rw-r--r--   0        0        0     2174 2023-06-14 18:50:15.256988 pydantic_xmlmodel-0.3/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3/pydantic_xmlmodel/py.typed
--rw-r--r--   0        0        0    14373 2023-06-14 18:47:40.251015 pydantic_xmlmodel-0.3/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      611 2023-06-14 18:53:55.354788 pydantic_xmlmodel-0.3/pyproject.toml
--rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2174 2023-06-14 18:50:15.256988 pydantic_xmlmodel-0.3.1/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0    14379 2023-06-14 19:01:31.733595 pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      613 2023-06-14 19:02:45.363532 pydantic_xmlmodel-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3.1/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.3/LICENSE` & `pydantic_xmlmodel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.3/README.md` & `pydantic_xmlmodel-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.3/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/xmlmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A module that contains the XMLModel class."""
 
-from typing import Any, Callable, Optional, Type, TypeVar, no_type_check
+from typing import Any, Callable, Dict, Optional, Type, TypeVar, no_type_check
 from xml.dom.minidom import parseString
 from xml.etree.ElementTree import Element, SubElement, fromstring, tostring
 
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
 T = TypeVar("T", bound="XMLModel")
@@ -233,15 +233,15 @@
             ... </cat>
             ... ''')
             >>> cat
             Cat(animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True), name='Kitty')
         """
 
         def from_element(element: Element, model: Type[BaseModel]) -> Any:
-            data: dict[str, Any] = {}
+            data: Dict[str, Any] = {}
             for field in model.__fields__:
                 if field == "xml_content":
                     continue
                 field_type = model.__annotations__[field]
                 is_list_like = model.__fields__[field].sub_fields is not None
                 if is_list_like:
                     sub_fields = model.__fields__[field].sub_fields
```

### Comparing `pydantic_xmlmodel-0.3/pyproject.toml` & `pydantic_xmlmodel-0.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.3"
+version = "0.3.1"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

### Comparing `pydantic_xmlmodel-0.3/PKG-INFO` & `pydantic_xmlmodel-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xmlmodel
-Version: 0.3
+Version: 0.3.1
 Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
 Home-page: https://github.com/cofob/pydanticxml
 License: MIT
 Author: cofob
 Author-email: cofob@riseup.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

