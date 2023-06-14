# Comparing `tmp/pydantic_xmlmodel-0.2.tar.gz` & `tmp/pydantic_xmlmodel-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.2.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.2.1.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.2.tar` & `pydantic_xmlmodel-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.2/LICENSE
--rw-r--r--   0        0        0     2323 2023-06-07 13:50:14.138462 pydantic_xmlmodel-0.2/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.2/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.2/pydantic_xmlmodel/py.typed
--rw-r--r--   0        0        0     9806 2023-06-13 10:18:19.983642 pydantic_xmlmodel-0.2/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      611 2023-06-13 10:19:00.609226 pydantic_xmlmodel-0.2/pyproject.toml
--rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1800 2023-06-14 13:48:51.929705 pydantic_xmlmodel-0.2.1/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0     9678 2023-06-14 14:08:24.265636 pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      613 2023-06-14 14:14:16.007116 pydantic_xmlmodel-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.2.1/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.2/LICENSE` & `pydantic_xmlmodel-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.2/README.md` & `pydantic_xmlmodel-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pydantic-xmlmodel
+Version: 0.2.1
+Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
+Home-page: https://github.com/cofob/pydanticxml
+License: MIT
+Author: cofob
+Author-email: cofob@riseup.net
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1,<2)
+Project-URL: Repository, https://github.com/cofob/pydanticxml
+Description-Content-Type: text/markdown
+
 # PydanticXML
 
 PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa. It is built on top of the Pydantic library and extends it with XML-specific functionality.
 
 ## Installation
 
 You can install PydanticXML with pip:
@@ -14,18 +33,14 @@
 
 To use PydanticXML, you need to import the `XMLModel` class from the `pydanticxml` module:
 
 ```python
 from pydantic_xmlmodel import XMLModel
 ```
 
-Here is the class diagram of the library:
-
-![Graph](https://mermaid.ink/img/pako:eNp9UstqwzAQ_BWhUxqcHzAh0NetpodeCnERG2ntiugRpHXTkObfu3ZCGpNQgSxpZnYGr7SXOhqUpdQOcn6y0CbwdRA8BkS8Vy8VK1yFBGJ_ZPoxn3tGBs1i8QcLpQJulZpolwsRwGMhVpCRD0CUeJlO11tIbb4rxX3YHSsPtxLHaQ9sMsCXaTOlvr1TfYxSpXjdkI0B3DJT-ritarqge9FI_gjOwcrhcigsRP-9rtcxEAb6J0ioFumcNeE_ZP6CNlYTReYnNhi2ujCygTjYBu06g4PFF6bMXClWMborqyZF3xvxHCgWnDs06uno_uY_s9kZkYX0mDxYw9c_9LqW9Ikea1ny1kAS61rW4cBC6Ci-7YKWJaUOC9ltDBCenssYfDaWYpJlAy4ziMOxOj2yGBrbysMv1qTMwg?type=png)
-
 ## Examples
 
 ### Defining a Model
 
 You can define a model by subclassing `XMLModel` and defining attributes with type annotations:
 
 ```python
@@ -70,11 +85,12 @@
 cat = Cat.from_xml(xml)
 print(cat)
 ```
 
 This will output:
 
 ```python
-animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True, __xml_content__=None) name='Kitty' __xml_content__='\n    '
+animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True, xml_content=None) name='Kitty' xml_content='\n    '
 ```
 
-*(Note that the `__xml_content__` attribute is not part of the model. It is used to store the XML content, like this `<element> xml_content <other_element /></element>`)*
+*(Note that the `xml_content` attribute is not part of the model. It is used to store the XML content, like this `<element> xml_content <other_element /></element>`)*
+
```

### Comparing `pydantic_xmlmodel-0.2/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.2.1/pydantic_xmlmodel/xmlmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     It's a subclass of `pydantic.BaseModel` and can be used as a regular model (and can be nested in other models).
 
     It's currently missing support for lists and dictionaries (it will be added as json attribute to the XML element).
 
     It adds the following class attributes to XMLModel:
         - `__xml_name__`: The name of the XML element. If not specified, the name of the class is used.
         - `__xml_name_function__`: A function that used if `__xml_name__` is not specified.
-        - `__xml_content__`: The content of the XML element inside `<element>{{__xml_content__}}</element>`. If not specified, the element will not have any content.
+        - `xml_content`: The content of the XML element inside `<element>{{xml_content}}</element>`. If not specified, the element will not have any content.
     """
 
     __xml_name__: Optional[str] = None
     """The name of the XML element. If not specified, the name of the class is used."""
 
     __xml_name_function__: Optional[Callable[[str], str]] = lambda x: x.lower()
     """A function that used if `__xml_name__` is not specified.
@@ -65,23 +65,16 @@
         >>> class ExampleSchema(NewXMLModel):
         ...     pass
         ...
         >>> ExampleSchema._get_xml_name()
         'EXAMPLESCHEMA'
     """
 
-    __xml_content__: Optional[str] = None
-    """The content of the XML element inside `<element>{{__xml_content__}}</element>`. If not specified, the element will not have any content."""
-
-    def __init__(self, **data: Any) -> None:
-        """Initialize the model."""
-        xml_content = data.pop("__xml_content__", None)
-        super().__init__(**data)
-        if xml_content is not None:
-            object.__setattr__(self, "__xml_content__", xml_content)
+    xml_content: Optional[Any] = None
+    """The content of the XML element inside `<element>{{xml_content}}</element>`. If not specified, the element will not have any content."""
 
     @classmethod
     def _get_xml_name(cls) -> str:
         """Return the name of the XML element."""
         if cls.__xml_name__ is not None:
             return cls.__xml_name__
         else:
@@ -116,52 +109,55 @@
             ... ).to_xml(indent=4)
             <?xml version="1.0" ?>
             <cat name="Kitty">
                 <animal_characteristics color="black" is_friendly="true" weight="10"/>
             </cat>
         """
 
-        def to_xml(e: Element, obj: Any) -> None:
+        def to_xml_innner(e: Element, obj: Any) -> None:
             """Convert the model to XML recursively."""
             # Iterate over the fields of the model and convert them to XML
             for field, _ in obj.dict().items():
-                # We skip the __xml_content__ field because we handle it separately
-                if field == "__xml_content__":
+                # We skip the xml_content field because we handle it separately
+                if field == "xml_content":
                     continue
                 # We get the value of the field using getattr() because the we need subclass of BaseModel, not just dict
                 value = getattr(obj, field)
                 # If the value is a BaseModel, we convert it to XML recursively
                 if isinstance(value, BaseModel):
                     # Get the name of the XML element
                     name = value.__class__.__name__
                     if isinstance(value, XMLModel):
                         name = value._get_xml_name()
                     # Create the XML element and add it to the parent element
                     sub = SubElement(e, name)
                     # Convert the BaseModel to XML recursively
-                    to_xml(sub, value)
+                    to_xml_innner(sub, value)
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
-            if obj.__xml_content__ is not None:
-                e.text = obj.__xml_content__
+            if isinstance(obj, XMLModel) and obj.xml_content is not None:
+                e.text = str(obj.xml_content)
 
         # Create the root XML element
         root = Element(self._get_xml_name())
         # Convert the model to XML recursively
-        to_xml(root, self)
+        to_xml_innner(root, self)
         # Convert the XML element to string
+        #
+        # I know it's not the best way to do it, but it's the only way I found to convert
+        # the Element to Document
         xml = parseString(tostring(root, encoding="unicode"))
 
         if not include_xml_version:
             # See https://stackoverflow.com/a/65516230
             xml = xml.childNodes[0]
 
         xml_str: str
@@ -201,47 +197,45 @@
             >>> cat
             Cat(animal_characteristics=AnimalCharacteristics(color='black', weight=10, is_friendly=True), name='Kitty')
         """
 
         def from_element(element: Element, model: Type[BaseModel]) -> Any:
             data = {}
             for field in model.__fields__:
-                # We skip the __xml_content__ field because we handle it separately
-                if field == "__xml_content__":
+                if field == "xml_content":
                     continue
-
                 field_type = model.__annotations__[field]
                 if issubclass(field_type, XMLModel):
                     xml_name = field_type._get_xml_name()
                 else:
                     xml_name = (
                         model.__fields__[field].field_info.extra.get("__xml_name__")
-                        or field
+                        or model.__fields__[field].alias
                     )
 
                 # Get the value of the field
-                if xml_name in element.attrib:
-                    data[field] = element.attrib[xml_name]
+                if xml_name in element.attrib and not issubclass(field_type, BaseModel):
+                    data[xml_name] = element.attrib[xml_name]
                 # If the field is a subelement, we convert it to XML recursively
                 else:
                     child = element.find(xml_name)
                     if child is not None:
                         if issubclass(field_type, BaseModel):
                             data[field] = from_element(child, field_type)
                         else:
                             data[field] = child.text or ""
 
+            # Handle the xml_content field
+            # Set the content of the XML element
+            xml_content_meta = model.__fields__.get("xml_content")
+            if xml_content_meta is not None:
+                data[xml_content_meta.alias] = element.text or ""
+            else:
+                data["xml_content"] = element.text or ""
+
             # Convert the data to the model
             out = model(**data)
 
-            # Set the content of the XML element
-            if isinstance(out, XMLModel):
-                object.__setattr__(out, "__xml_content__", element.text)
-
             return out
 
         root = fromstring(xml)
         return from_element(root, cls)  # type: ignore
-
-    def set_xml_content(self, value: Optional[str]) -> None:
-        """Set the content of the XML element."""
-        object.__setattr__(self, "__xml_content__", value)
```

### Comparing `pydantic_xmlmodel-0.2/pyproject.toml` & `pydantic_xmlmodel-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.2"
+version = "0.2.1"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

