# Comparing `tmp/ecmind_blue_client_objdef-0.0.8.tar.gz` & `tmp/ecmind_blue_client_objdef-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecmind_blue_client_objdef-0.0.8.tar", last modified: Fri Feb 10 10:26:27 2023, max compression
+gzip compressed data, was "ecmind_blue_client_objdef-0.0.9.tar", last modified: Wed Jun 14 08:44:42 2023, max compression
```

## Comparing `ecmind_blue_client_objdef-0.0.8.tar` & `ecmind_blue_client_objdef-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-02-10 10:26:27.598449 ecmind_blue_client_objdef-0.0.8/
--rw-r--r--   0 rk        (1000) rk        (1000)     1069 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/LICENSE
--rw-r--r--   0 rk        (1000) rk        (1000)     1363 2023-02-10 10:26:27.598449 ecmind_blue_client_objdef-0.0.8/PKG-INFO
--rw-r--r--   0 rk        (1000) rk        (1000)      845 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/README.md
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-02-10 10:26:27.598449 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/
--rw-r--r--   0 rk        (1000) rk        (1000)      292 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/__init__.py
--rw-r--r--   0 rk        (1000) rk        (1000)      421 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/cabinet.py
--rw-r--r--   0 rk        (1000) rk        (1000)      838 2023-02-10 10:23:40.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/field.py
--rw-r--r--   0 rk        (1000) rk        (1000)      262 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/field_types.py
--rw-r--r--   0 rk        (1000) rk        (1000)      482 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/object.py
--rw-r--r--   0 rk        (1000) rk        (1000)     7790 2023-02-10 10:16:41.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/object_definition.py
--rw-r--r--   0 rk        (1000) rk        (1000)      653 2023-02-10 07:10:24.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/table_column.py
--rw-r--r--   0 rk        (1000) rk        (1000)      644 2023-02-10 10:16:15.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/table_field.py
-drwxr-xr-x   0 rk        (1000) rk        (1000)        0 2023-02-10 10:26:27.598449 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/
--rw-r--r--   0 rk        (1000) rk        (1000)     1363 2023-02-10 10:26:27.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/PKG-INFO
--rw-r--r--   0 rk        (1000) rk        (1000)      587 2023-02-10 10:26:27.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/SOURCES.txt
--rw-r--r--   0 rk        (1000) rk        (1000)        1 2023-02-10 10:26:27.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/dependency_links.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       44 2023-02-10 10:26:27.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/requires.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       26 2023-02-10 10:26:27.000000 ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/top_level.txt
--rw-r--r--   0 rk        (1000) rk        (1000)       38 2023-02-10 10:26:27.598449 ecmind_blue_client_objdef-0.0.8/setup.cfg
--rw-r--r--   0 rk        (1000) rk        (1000)      853 2023-02-10 10:26:16.000000 ecmind_blue_client_objdef-0.0.8/setup.py
+drwxr-xr-x   0 uw        (1000) uw        (1000)        0 2023-06-14 08:44:42.868436 ecmind_blue_client_objdef-0.0.9/
+-rw-r--r--   0 uw        (1000) uw        (1000)     1069 2023-06-08 13:42:08.000000 ecmind_blue_client_objdef-0.0.9/LICENSE
+-rw-r--r--   0 uw        (1000) uw        (1000)     1496 2023-06-14 08:44:42.868436 ecmind_blue_client_objdef-0.0.9/PKG-INFO
+-rw-r--r--   0 uw        (1000) uw        (1000)      977 2023-06-14 08:43:07.000000 ecmind_blue_client_objdef-0.0.9/README.md
+drwxr-xr-x   0 uw        (1000) uw        (1000)        0 2023-06-14 08:44:42.868436 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/
+-rw-r--r--   0 uw        (1000) uw        (1000)      292 2023-06-13 08:48:17.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/__init__.py
+-rw-r--r--   0 uw        (1000) uw        (1000)     2278 2023-06-14 08:37:25.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/addons.py
+-rw-r--r--   0 uw        (1000) uw        (1000)      421 2023-06-08 13:42:08.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/cabinet.py
+-rw-r--r--   0 uw        (1000) uw        (1000)      864 2023-06-13 07:08:52.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/field.py
+-rw-r--r--   0 uw        (1000) uw        (1000)      326 2023-06-13 08:19:32.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/field_types.py
+-rw-r--r--   0 uw        (1000) uw        (1000)      482 2023-06-08 13:42:08.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/object.py
+-rw-r--r--   0 uw        (1000) uw        (1000)     9247 2023-06-14 07:32:37.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/object_definition.py
+-rw-r--r--   0 uw        (1000) uw        (1000)      653 2023-06-08 13:42:08.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/table_column.py
+-rw-r--r--   0 uw        (1000) uw        (1000)      607 2023-06-08 13:42:08.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/table_field.py
+drwxr-xr-x   0 uw        (1000) uw        (1000)        0 2023-06-14 08:44:42.868436 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/
+-rw-r--r--   0 uw        (1000) uw        (1000)     1496 2023-06-14 08:44:42.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/PKG-INFO
+-rw-r--r--   0 uw        (1000) uw        (1000)      623 2023-06-14 08:44:42.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/SOURCES.txt
+-rw-r--r--   0 uw        (1000) uw        (1000)        1 2023-06-14 08:44:42.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/dependency_links.txt
+-rw-r--r--   0 uw        (1000) uw        (1000)       44 2023-06-14 08:44:42.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/requires.txt
+-rw-r--r--   0 uw        (1000) uw        (1000)       26 2023-06-14 08:44:42.000000 ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/top_level.txt
+-rw-r--r--   0 uw        (1000) uw        (1000)       38 2023-06-14 08:44:42.868436 ecmind_blue_client_objdef-0.0.9/setup.cfg
+-rw-r--r--   0 uw        (1000) uw        (1000)      853 2023-06-14 08:43:21.000000 ecmind_blue_client_objdef-0.0.9/setup.py
```

### Comparing `ecmind_blue_client_objdef-0.0.8/LICENSE` & `ecmind_blue_client_objdef-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client_objdef-0.0.8/PKG-INFO` & `ecmind_blue_client_objdef-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmind_blue_client_objdef
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper modules for the `ecmind_blue_client` to ease the work with object definition APIs.
 Home-page: https://gitlab.ecmind.ch/open/ecmind_blue_client_objdef
 Author: Roland Koller
 Author-email: info@ecmind.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,18 +20,18 @@
 
 `pip install ecmind_blue_client_objdef`
 
 ## Usage
 
 ```python
 from ecmind_blue_client.tcp_client import TcpClient as Client
-from ecmind_blue_client_objdef import objdef
+from ecmind_blue_client_objdef import object_definition
 
 client = Client(hostname='localhost', port=4000, appname='test', username='root', password='optimal')
-asobjdef = objdef.load_object_definition(client)
+asobjdef = object_definition.load_object_definition(client)
 for cabinet in asobjdef.cabinets:
     print(cabinet)
 ```
 
 ## Changes
 
 ### Version `0.0.3`
@@ -41,7 +41,12 @@
 ### Version `0.0.4`
 
 - Workaround and warn message for tables without columns.
 
 ### Version `0.0.5`
 
 - Workaround and warn message for tab pages without controls.
+
+### Version `0.0.9`
+
+- Add list addon support
+- Add missing field types YES_NO, LETTERS_ONLY and ALPHA_DIGITS
```

### Comparing `ecmind_blue_client_objdef-0.0.8/README.md` & `ecmind_blue_client_objdef-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 `pip install ecmind_blue_client_objdef`
 
 ## Usage
 
 ```python
 from ecmind_blue_client.tcp_client import TcpClient as Client
-from ecmind_blue_client_objdef import objdef
+from ecmind_blue_client_objdef import object_definition
 
 client = Client(hostname='localhost', port=4000, appname='test', username='root', password='optimal')
-asobjdef = objdef.load_object_definition(client)
+asobjdef = object_definition.load_object_definition(client)
 for cabinet in asobjdef.cabinets:
     print(cabinet)
 ```
 
 ## Changes
 
 ### Version `0.0.3`
@@ -27,7 +27,12 @@
 ### Version `0.0.4`
 
 - Workaround and warn message for tables without columns.
 
 ### Version `0.0.5`
 
 - Workaround and warn message for tab pages without controls.
+
+### Version `0.0.9`
+
+- Add list addon support
+- Add missing field types YES_NO, LETTERS_ONLY and ALPHA_DIGITS
```

### Comparing `ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/field.py` & `ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from ecmind_blue_client_objdef import FieldTypes
 from typing import Dict
 
+from ecmind_blue_client_objdef import FieldTypes
+from .addons import Addons
+
 class Field():
     def __init__(
         self, 
         internal_name:str, 
         name:str,
-        table_name:str,
         names:Dict[str, str],
         db_field:int, 
         type:FieldTypes,
         length:int,
         guid:str,
         tab_order:int,
         page_control:str=None,
-        page:str=None
+        page:str=None,
+        addons: Addons=None
     ):
         self.internal_name = internal_name
         self.name = name
-        self.table_name = table_name
         self.names = names
         self.db_field = db_field
         self.type = type
         self.length = length
         self.guid = guid
         self.tab_order = tab_order
-        self.page_control = page_control
+        self.page_control = page_control,
         self.page = page
+        self.addons = addons
 
     def __repr__(self) -> str:
         return f'{self.internal_name} ({self.db_field}) "{self.name}"'
```

### Comparing `ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/object_definition.py` & `ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/object_definition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from datetime import datetime
-from typing import Dict, List
+from typing import Dict
 from warnings import warn
 
 from ecmind_blue_client import Client, Job
 from ecmind_blue_client.const import MainTypeId
 from XmlElement import XmlElement
 
-from ecmind_blue_client_objdef import FieldTypes, Field, TableColumn, TableField, Object, Cabinet
+from ecmind_blue_client_objdef import (Cabinet, Field, FieldTypes, Object,
+                                       TableColumn, TableField)
+
+from .addons import Addons, ListAddon, ListAddonRow
 
 
 class ObjectDefinition():
     def __init__(self, obj_def_xml:str):
         xml_elem = XmlElement.from_string(obj_def_xml)
         xml_elem.find('languages').find('language').flag_as_list = True
         for cab in xml_elem.findall('cabinet'):
@@ -24,43 +27,75 @@
         language_by_id = { l['@lang_id']: l['@name'] for l in self.raw['languages']['language'] }
 
         self.cabinets:Dict[str, Cabinet] = {}
         self.registers:Dict[str, Object] = {}
         self.documents:Dict[str, Object] = {}
 
         for raw_cabinet in self.raw['cabinet']:
-            raw_objects = raw_cabinet['object']
+            if isinstance(raw_cabinet['object'], list):
+                raw_objects = raw_cabinet['object']
+            else:
+                raw_objects = [ raw_cabinet['object'] ]
             
-            def __parse_fields__(raw_object:dict, raw_list:dict, page_control:Field=None, page:str=None) -> dict:
+            def __parse_fields__(raw_list:dict, page_control:Field=None, page:str=None) -> dict:
                 fields = {}
                 if not isinstance(raw_list, list):
                     raw_list = [ raw_list ]
 
                 for raw_field in raw_list:
                     raw_names = raw_field['names']['name']
                     if not isinstance(raw_names, list):
                         raw_names = [ raw_names ]
 
 
                     internal_name = raw_field['@internal']
                     name = raw_field['@name']
                     names = { language_by_id[n['@lang_id']]: n['#'] for n in raw_names }
-                    db_field = raw_field['@fieldname']
+                    db_field = ['@fieldname']
                     guid = raw_field['@os_guid']
                     tab_order = raw_field['@taborder']
                     length = raw_field['flags']['@input_length'] if '@input_length' in raw_field['flags'] else 0
 
                     try:
-                        type=FieldTypes(str(raw_field['flags']['@dt']))
-                    except:
-                        type=None
+                        field_type = FieldTypes(str(raw_field['flags']['@dt']))
+                    except Exception as _:
+                        field_type = None
                         warn(f'Datatype "{str(raw_field["flags"]["@dt"])}" for field {raw_field["@internal"]} is unknown.')
 
+                    addons = Addons()
+
+                    # List or Addons
+                    if "list" in raw_field: 
+                        addon_data = raw_field['list']
+
+                        # List / Tree Addon
+                        if 'ADDON32' not in raw_field['list']:
+                            multiselection = addon_data['@multiselection'] == 1
+                            order = addon_data['@order']
+                            keyselcol =  addon_data['@keyselcol'] if '@keyselcol' in addon_data else 0
+                            sortcol = addon_data['@sortcol'] if '@sortcol' in addon_data else 0
+                            rawdata = addon_data['rawdata']
+                            
+                            # List
+                            if 'row' in addon_data:
+                                icon_index = 0
+                                icons = []
+                                while f'ICON{icon_index}' in addon_data:
+                                    icons.append(addon_data[f'ICON{icon_index}'])
+                                    icon_index += 1
+
+                                rows = []
+                                row_index = 0
+                                for row in addon_data['row']:
+                                    rows.append(ListAddonRow(row, icons, row_index))
+
+                                addons.list = ListAddon(rows, multiselection, order, keyselcol, sortcol, rawdata)
 
-                    if type == FieldTypes.TABLE:
+
+                    if field_type == FieldTypes.TABLE:
                         columns:Dict[str, TableColumn] = {}
                         if 'listctrl' in raw_field:
                             for raw_column in raw_field['listctrl'] if isinstance(raw_field['listctrl'], list) else [ raw_field['listctrl'] ]:
                                 raw_col_names = raw_column['names']['name'] if isinstance(raw_column['names']['name'], list) else [ raw_column['names']['name'] ]
                                 columns[raw_column['@internal']] = TableColumn(
                                     internal_name=raw_column['@internal'],
                                     name=raw_column['@name'],
@@ -69,19 +104,18 @@
                                     id=raw_column['@id'],
                                     type=FieldTypes(str(raw_column['@type'])),
                                     length=raw_column['@length'],
                                     guid=raw_column['@os_guid']
                                 )
                         else:
                             warn(f'Table "{str(internal_name)}" (GUID {guid}) has no columns.')
-                        table_name = f"{raw_object['@tablename']}{db_field}"
-                        field = TableField(internal_name, name, table_name, names, db_field, type, length, guid, tab_order, page_control, page, columns)
+
+                        field = TableField(internal_name, name, names, db_field, field_type, length, guid, tab_order, page_control, page, columns)
                     else:
-                        table_name = f"{raw_object['@tablename']}"
-                        field = Field(internal_name, name, table_name, names, db_field, type, length, guid, tab_order, page_control, page)
+                        field = Field(internal_name, name, names, db_field, field_type, length, guid, tab_order, page_control, page, addons)
 
                     
                     fields[raw_field['@internal']] = field
 
                     if 'page' in raw_field:
                         if isinstance(raw_field['page'], list):
                             raw_pages = raw_field['page']
@@ -92,15 +126,14 @@
                                 page = raw_page['@internal']
                             else:
                                 page = raw_page['@page_id']
                                 warn(f'Page "{raw_page["@page_id"]}" has no internal name.')
                             if raw_page['fields'] != None:                                    
                                 fields.update(
                                     __parse_fields__(
-                                        raw_object,
                                         raw_page['fields']['field'],
                                         page_control=field, 
                                         page=page
                                     )
                                 )
                             else:
                                 warn(f'Page "{page}" of page control "{internal_name}" has no elements.')
@@ -108,22 +141,22 @@
                 return(fields)
 
             cabinet_registers:Dict[str, Object] = {}
             cabinet_document:Dict[str, Object] = {}
             for raw_child in raw_objects:
                 
                 if raw_child['@maintype'] == MainTypeId.FOLDER.value:
-                    cabinet_fields = __parse_fields__(raw_child, raw_child['fields']['field'])  
+                    cabinet_fields = __parse_fields__(raw_child['fields']['field'])  
                 else:
                     child = Object(
                         type_id= raw_child['@maintype']* 2**16 + raw_child['@cotype'],
                         internal_name=raw_child['@internal'],
                         name=raw_child['@name'],
                         table_name=raw_child['@tablename'],
-                        fields = __parse_fields__(raw_child, raw_child['fields']['field'])  
+                        fields = __parse_fields__(raw_child['fields']['field'])  
                     )
 
                     if raw_child['@maintype'] == MainTypeId.REGISTER.value:
                         self.registers[raw_child['@internal']] = child
                         cabinet_registers[raw_child['@internal']] = child
                     else:
                         self.documents[raw_child['@internal']] = child
```

### Comparing `ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef/table_column.py` & `ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef/table_column.py`

 * *Files identical despite different names*

### Comparing `ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/PKG-INFO` & `ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmind-blue-client-objdef
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper modules for the `ecmind_blue_client` to ease the work with object definition APIs.
 Home-page: https://gitlab.ecmind.ch/open/ecmind_blue_client_objdef
 Author: Roland Koller
 Author-email: info@ecmind.ch
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,18 +20,18 @@
 
 `pip install ecmind_blue_client_objdef`
 
 ## Usage
 
 ```python
 from ecmind_blue_client.tcp_client import TcpClient as Client
-from ecmind_blue_client_objdef import objdef
+from ecmind_blue_client_objdef import object_definition
 
 client = Client(hostname='localhost', port=4000, appname='test', username='root', password='optimal')
-asobjdef = objdef.load_object_definition(client)
+asobjdef = object_definition.load_object_definition(client)
 for cabinet in asobjdef.cabinets:
     print(cabinet)
 ```
 
 ## Changes
 
 ### Version `0.0.3`
@@ -41,7 +41,12 @@
 ### Version `0.0.4`
 
 - Workaround and warn message for tables without columns.
 
 ### Version `0.0.5`
 
 - Workaround and warn message for tab pages without controls.
+
+### Version `0.0.9`
+
+- Add list addon support
+- Add missing field types YES_NO, LETTERS_ONLY and ALPHA_DIGITS
```

### Comparing `ecmind_blue_client_objdef-0.0.8/ecmind_blue_client_objdef.egg-info/SOURCES.txt` & `ecmind_blue_client_objdef-0.0.9/ecmind_blue_client_objdef.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 ecmind_blue_client_objdef/__init__.py
+ecmind_blue_client_objdef/addons.py
 ecmind_blue_client_objdef/cabinet.py
 ecmind_blue_client_objdef/field.py
 ecmind_blue_client_objdef/field_types.py
 ecmind_blue_client_objdef/object.py
 ecmind_blue_client_objdef/object_definition.py
 ecmind_blue_client_objdef/table_column.py
 ecmind_blue_client_objdef/table_field.py
```

### Comparing `ecmind_blue_client_objdef-0.0.8/setup.py` & `ecmind_blue_client_objdef-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ecmind_blue_client_objdef',
-    version='0.0.8',
+    version='0.0.9',
     author='Roland Koller',
     author_email='info@ecmind.ch',
     description='Helper modules for the `ecmind_blue_client` to ease the work with object definition APIs.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.ecmind.ch/open/ecmind_blue_client_objdef',
     packages=setuptools.find_packages(),
```

