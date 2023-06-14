# Comparing `tmp/pydantic_xmlmodel-0.2.1.tar.gz` & `tmp/pydantic_xmlmodel-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.3.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.2.1.tar` & `pydantic_xmlmodel-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.2.1/LICENSE
--rw-r--r--   0        0        0     1800 2023-06-14 13:48:51.929705 pydantic_xmlmodel-0.2.1/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/py.typed
--rw-r--r--   0        0        0     9678 2023-06-14 14:08:24.265636 pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      613 2023-06-14 14:14:16.007116 pydantic_xmlmodel-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3/LICENSE
+-rw-r--r--   0        0        0     2174 2023-06-14 18:50:15.256988 pydantic_xmlmodel-0.3/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0    14373 2023-06-14 18:47:40.251015 pydantic_xmlmodel-0.3/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      611 2023-06-14 18:53:55.354788 pydantic_xmlmodel-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.2.1/LICENSE` & `pydantic_xmlmodel-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.3/pydantic_xmlmodel/xmlmodel.py`

 * *Files 26% similar despite different names*

```diff
@@ -128,36 +128,74 @@
                     name = value.__class__.__name__
                     if isinstance(value, XMLModel):
                         name = value._get_xml_name()
                     # Create the XML element and add it to the parent element
                     sub = SubElement(e, name)
                     # Convert the BaseModel to XML recursively
                     to_xml_innner(sub, value)
+                elif obj.__fields__[field].sub_fields is not None:
+                    # If the field is a list-like field but not a list of BaseModel, we raise an error
+                    if not issubclass(
+                        obj.__fields__[field].sub_fields[0].type_, BaseModel
+                    ):
+                        raise ValueError(
+                            f"Field {field} is a list-like field but not a list of BaseModel"
+                        )
+                    # Iterate over the list and convert each item to XML recursively
+                    for item in value:
+                        # Get the name of the XML element
+                        name = item.__class__.__name__
+                        if isinstance(item, XMLModel):
+                            name = item._get_xml_name()
+                        # Create the XML element and add it to the parent element
+                        sub = SubElement(e, name)
+                        # Convert the BaseModel to XML recursively
+                        to_xml_innner(sub, item)
                 # Else, we add the value as an attribute
                 else:
                     # Get the name of the XML attribute
                     pydantic_field = obj.__fields__[field]
                     # If the field has an alias, we use it as the name of the XML attribute
                     name = pydantic_field.name
                     if pydantic_field.alias is not None:
                         name = pydantic_field.alias
                     # Add the attribute to the XML element
                     e.set(name, str(value))
             # If the model has content, we add it to the XML element
             if isinstance(obj, XMLModel) and obj.xml_content is not None:
-                e.text = str(obj.xml_content)
+                xml_content_field = obj.__fields__["xml_content"]
+                # if field is a list-like field but not a list of BaseModel, we raise an error
+                if xml_content_field.sub_fields is not None and not issubclass(
+                    xml_content_field.sub_fields[0].type_, BaseModel
+                ):
+                    raise ValueError(
+                        f"xml_content field of {obj.__class__.__name__} must be a List[BaseModel] "
+                        f"but got {xml_content_field.sub_fields[0].type_.__name__}"
+                    )
+                # if field is a list-like field, we add each item as a separate XML element
+                if xml_content_field.sub_fields is not None:
+                    type_ = xml_content_field.sub_fields[0].type_
+                    name = type_.__name__
+                    if issubclass(type_, XMLModel):
+                        name = type_._get_xml_name()
+                    for item in obj.xml_content:
+                        sub = SubElement(e, name)
+                        to_xml_innner(sub, item)
+                # else, we add the content as a text
+                else:
+                    e.text = str(obj.xml_content)
 
         # Create the root XML element
         root = Element(self._get_xml_name())
         # Convert the model to XML recursively
         to_xml_innner(root, self)
         # Convert the XML element to string
         #
         # I know it's not the best way to do it, but it's the only way I found to convert
-        # the Element to Document
+        # the Element to Document. If you know a better way, please let me know.
         xml = parseString(tostring(root, encoding="unicode"))
 
         if not include_xml_version:
             # See https://stackoverflow.com/a/65516230
             xml = xml.childNodes[0]
 
         xml_str: str
@@ -195,46 +233,89 @@
             ... </cat>
             ... ''')
             >>> cat
             Cat(animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True), name='Kitty')
         """
 
         def from_element(element: Element, model: Type[BaseModel]) -> Any:
-            data = {}
+            data: dict[str, Any] = {}
             for field in model.__fields__:
                 if field == "xml_content":
                     continue
                 field_type = model.__annotations__[field]
-                if issubclass(field_type, XMLModel):
+                is_list_like = model.__fields__[field].sub_fields is not None
+                if is_list_like:
+                    sub_fields = model.__fields__[field].sub_fields
+                    if not sub_fields:
+                        raise ValueError(
+                            f"Field {field} is a list-like field but it's empty"
+                        )
+                    type_ = sub_fields[0].type_
+                    field_info = sub_fields[0].field_info
+                    if not issubclass(type_, BaseModel):
+                        raise ValueError(
+                            f"Field {field} is a list-like field but not a list of BaseModel"
+                        )
+                    if issubclass(type_, XMLModel):
+                        xml_name = type_._get_xml_name()
+                    else:
+                        xml_name = field_info.extra.get("__xml_name__")
+                elif issubclass(field_type, XMLModel):
                     xml_name = field_type._get_xml_name()
                 else:
                     xml_name = (
                         model.__fields__[field].field_info.extra.get("__xml_name__")
                         or model.__fields__[field].alias
                     )
 
                 # Get the value of the field
                 if xml_name in element.attrib and not issubclass(field_type, BaseModel):
                     data[xml_name] = element.attrib[xml_name]
+                # If the field is a list-like field, we convert each XML element to a BaseModel
+                elif is_list_like:
+                    data[field] = []
+                    for child in element.findall(xml_name):
+                        data[field].append(from_element(child, type_))
                 # If the field is a subelement, we convert it to XML recursively
                 else:
-                    child = element.find(xml_name)
-                    if child is not None:
+                    child_find = element.find(xml_name)
+                    if child_find is not None:
                         if issubclass(field_type, BaseModel):
-                            data[field] = from_element(child, field_type)
+                            data[field] = from_element(child_find, field_type)
                         else:
-                            data[field] = child.text or ""
+                            data[field] = child_find.text or ""
 
             # Handle the xml_content field
             # Set the content of the XML element
             xml_content_meta = model.__fields__.get("xml_content")
+            xml_content_data: Any
+            # if the field is a list-like field, we add each item as a separate XML element
+            if xml_content_meta is not None and xml_content_meta.sub_fields is not None:
+                if not issubclass(xml_content_meta.sub_fields[0].type_, BaseModel):
+                    raise ValueError(
+                        f"xml_content field of {model.__name__} must be a List[BaseModel] "
+                        f"but got {xml_content_meta.sub_fields[0].type_.__name__}"
+                    )
+                xml_content_data = []
+                name = xml_content_meta.sub_fields[0].type_.__name__
+                if issubclass(xml_content_meta.sub_fields[0].type_, XMLModel):
+                    name = xml_content_meta.sub_fields[0].type_._get_xml_name()
+                for child in element:
+                    if child.tag != name:
+                        continue
+                    xml_content_data.append(
+                        from_element(child, xml_content_meta.sub_fields[0].type_)
+                    )
+            # else, we add the content as a text
+            else:
+                xml_content_data = element.text or ""
             if xml_content_meta is not None:
-                data[xml_content_meta.alias] = element.text or ""
+                data[xml_content_meta.alias] = xml_content_data
             else:
-                data["xml_content"] = element.text or ""
+                data["xml_content"] = xml_content_data
 
             # Convert the data to the model
             out = model(**data)
 
             return out
 
         root = fromstring(xml)
```

### Comparing `pydantic_xmlmodel-0.2.1/pyproject.toml` & `pydantic_xmlmodel-0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.2.1"
+version = "0.3"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

### Comparing `pydantic_xmlmodel-0.2.1/PKG-INFO` & `pydantic_xmlmodel-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xmlmodel
-Version: 0.2.1
+Version: 0.3
 Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
 Home-page: https://github.com/cofob/pydanticxml
 License: MIT
 Author: cofob
 Author-email: cofob@riseup.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,24 @@
 Project-URL: Repository, https://github.com/cofob/pydanticxml
 Description-Content-Type: text/markdown
 
 # PydanticXML
 
 PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa. It is built on top of the Pydantic library and extends it with XML-specific functionality.
 
+## Features
+
+- Convert Pydantic models to XML and vice versa
+- Support for XML attributes, elements, content, **lists**.
+- Compatible with most Pydantic features (e.g. default values, validators, `Field` etc.)
+- Very easy to use. Extends Pydantic's API with only a few methods.
+- Has no dependencies other than Pydantic
+- Have a good docs in the source code
+- Fully tested
+
 ## Installation
 
 You can install PydanticXML with pip:
 
 ```bash
 pip install pydantic-xmlmodel
 ```
```

