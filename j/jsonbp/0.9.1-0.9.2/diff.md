# Comparing `tmp/jsonbp-0.9.1.tar.gz` & `tmp/jsonbp-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonbp-0.9.1.tar", last modified: Sun Jul  3 19:04:40 2022, max compression
+gzip compressed data, was "jsonbp-0.9.2.tar", last modified: Fri Aug 26 22:37:12 2022, max compression
```

## Comparing `jsonbp-0.9.1.tar` & `jsonbp-0.9.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.834118 jsonbp-0.9.1/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)       39 2022-07-03 19:04:37.000000 jsonbp-0.9.1/MANIFEST.in
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      751 2022-07-03 19:04:40.834118 jsonbp-0.9.1/PKG-INFO
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      174 2022-07-03 16:23:04.000000 jsonbp-0.9.1/README.rst
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      107 2022-07-03 19:04:40.834118 jsonbp-0.9.1/setup.cfg
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      822 2022-07-03 19:04:17.000000 jsonbp-0.9.1/setup.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.830118 jsonbp-0.9.1/src/
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.830118 jsonbp-0.9.1/src/jsonbp/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      602 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/__init__.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.834118 jsonbp-0.9.1/src/jsonbp/jbp/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/__init__.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     1017 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/array.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11525 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/blueprint.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      319 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/declaration.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)     2867 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/error.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      392 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/field.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      669 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/types.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)       40 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/jbp/violation.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.834118 jsonbp-0.9.1/src/jsonbp/localization/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      862 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/localization/messages.en_US.ini
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      964 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/localization/messages.pt_BR.ini
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11188 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/parser.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.834118 jsonbp-0.9.1/src/jsonbp/ply/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      116 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/ply/__init__.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    35241 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/ply/lex.py
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)    98438 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp/ply/yacc.py
-drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-07-03 19:04:40.830118 jsonbp-0.9.1/src/jsonbp.egg-info/
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      751 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp.egg-info/PKG-INFO
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)      588 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp.egg-info/SOURCES.txt
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)        1 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp.egg-info/dependency_links.txt
--rw-r--r--   0 gustavo   (1000) gustavo   (1000)        7 2022-07-03 19:04:40.000000 jsonbp-0.9.1/src/jsonbp.egg-info/top_level.txt
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.061141 jsonbp-0.9.2/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)       39 2022-07-03 19:04:37.000000 jsonbp-0.9.2/MANIFEST.in
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      751 2022-08-26 22:37:12.061141 jsonbp-0.9.2/PKG-INFO
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      174 2022-07-03 16:23:04.000000 jsonbp-0.9.2/README.rst
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      107 2022-08-26 22:37:12.061141 jsonbp-0.9.2/setup.cfg
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      822 2022-08-26 22:37:01.000000 jsonbp-0.9.2/setup.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.057141 jsonbp-0.9.2/src/
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.057141 jsonbp-0.9.2/src/jsonbp/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      602 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/__init__.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.061141 jsonbp-0.9.2/src/jsonbp/jbp/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/__init__.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     1017 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/array.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11513 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/blueprint.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      319 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/declaration.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)     2867 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/error.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      392 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/field.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      669 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/types.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)       40 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/jbp/violation.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.061141 jsonbp-0.9.2/src/jsonbp/localization/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      862 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/localization/messages.en_US.ini
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      964 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/localization/messages.pt_BR.ini
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    11188 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/parser.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.061141 jsonbp-0.9.2/src/jsonbp/ply/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      116 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/ply/__init__.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    35241 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/ply/lex.py
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)    98438 2022-08-26 22:37:11.000000 jsonbp-0.9.2/src/jsonbp/ply/yacc.py
+drwxr-xr-x   0 gustavo   (1000) gustavo   (1000)        0 2022-08-26 22:37:12.057141 jsonbp-0.9.2/src/jsonbp.egg-info/
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      751 2022-08-26 22:37:12.000000 jsonbp-0.9.2/src/jsonbp.egg-info/PKG-INFO
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)      588 2022-08-26 22:37:12.000000 jsonbp-0.9.2/src/jsonbp.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)        1 2022-08-26 22:37:12.000000 jsonbp-0.9.2/src/jsonbp.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavo   (1000) gustavo   (1000)        7 2022-08-26 22:37:12.000000 jsonbp-0.9.2/src/jsonbp.egg-info/top_level.txt
```

### Comparing `jsonbp-0.9.1/PKG-INFO` & `jsonbp-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonbp
-Version: 0.9.1
+Version: 0.9.2
 Summary: JSON Python Deserializer
 Home-page: https://github.com/vottini/jsonbp
 Author: Gustavo Venturini
 Author-email: gustavo.c.venturini@gmail.com
 License: MIT
 Keywords: json,deserialization
 Platform: any
```

### Comparing `jsonbp-0.9.1/setup.py` & `jsonbp-0.9.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.rst", "r") as fd:
 	long_description = fd.read()
 
 setup(
 	name='jsonbp',
 	description='JSON Python Deserializer',
-	version='0.9.1',
+	version='0.9.2',
 	license='MIT',
 	python_requires='>=3.6',
 	platforms='any',
 	author="Gustavo Venturini",
 	author_email='gustavo.c.venturini@gmail.com',
 	packages=find_packages('src'),
 	package_dir={'': 'src'},
```

### Comparing `jsonbp-0.9.1/src/jsonbp/__init__.py` & `jsonbp-0.9.2/src/jsonbp/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/jbp/array.py` & `jsonbp-0.9.2/src/jsonbp/jbp/array.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/jbp/blueprint.py` & `jsonbp-0.9.2/src/jsonbp/jbp/blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 			specs = self.find_element_declaration(fieldType)
 			baseType = specs['__baseType__']
 
 		deserialize_method = globals()['d_' + baseType]
 		return deserialize_method(fieldName, value, specs)
 
 
-	def validate_enum(self, fieldName, value, enumType):
+	def validate_enum(self, fieldName, enumType, value):
 		if None == value:
 			return False, jbpError.createForField(fieldName,
 				jbpError.NULL_VALUE)
 
 		if not isinstance(value, str):
 			return False, jbpError.createForField(fieldName,
 				jbpError.INVALID_ENUM, value=value)
@@ -240,15 +240,15 @@
 
 				contents[idx] = processed
 
 			return True, contents
 
 		if arrayKind == jbpField.ENUM:
 			for idx, value in enumerate(contents):
-				success, processed = self.validate_enum(fieldName, value, arrayType)
+				success, processed = self.validate_enum(fieldName, arrayType, value)
 
 				if not success:
 					processed.setAsArrayElement(idx)
 					return False, processed
 
 				contents[idx] = processed
 
@@ -276,29 +276,29 @@
 				if fieldData.optional: continue
 				return False, jbpError.createForNode(nodeName,
 					jbpError.MISSING_FIELD, field=fieldName)
 
 			retrieved = contents[fieldName]
 			if jbpArray.isArray(fieldData):
 				success, processed = self.validate_array(fieldName, fieldData, retrieved)
-				if not success: return success, processed
-				continue
+				if success: continue
+				return success, processed
 
 			fieldKind = fieldData.fieldKind
 			fieldType = fieldData.fieldType
 
 			if fieldKind == jbpField.NODE:
 				nodeSpecs = self.find_node_declaration(fieldType)
 				success, processed = self.validate_node(fieldName, nodeSpecs, retrieved)
 				if not success: return success, processed
 				contents[fieldName] = processed
 				continue
 
 			if fieldKind == jbpField.ENUM:
-				success, processed = self.validate_enum(fieldName, retrieved, fieldType)
+				success, processed = self.validate_enum(fieldName, fieldType, retrieved)
 				if not success: return success, processed
 				contents[fieldName] = processed
 				continue
 
 			success, processed = self.deserialize_field(fieldName, fieldType, retrieved)
 			if not success: return False, processed
 			contents[fieldName] = processed
@@ -315,19 +315,18 @@
 
 		if rootKind == jbpField.NODE:
 			rootNode = self.find_node_declaration(rootType)
 			return self.validate_node(None, rootNode, rootContents)
 
 		if rootKind == jbpField.ENUM:
 			rootEnum = self.find_enum_declaration(rootType)
-			return self.validate_enum(None, rootNode, rootContents)
+			return self.validate_enum(None, rootType, rootContents)
 
 		if rootKind == jbpField.SIMPLE:
 			return self.deserialize_field(None, rootType, rootContents)
-			pass
 
 
 	def deserialize(self, contents):
 		tag_number = lambda x : taggedNumber(x)
 		ident = lambda x : x
 
 		try:
```

### Comparing `jsonbp-0.9.1/src/jsonbp/jbp/error.py` & `jsonbp-0.9.2/src/jsonbp/jbp/error.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/jbp/types.py` & `jsonbp-0.9.2/src/jsonbp/jbp/types.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/localization/messages.en_US.ini` & `jsonbp-0.9.2/src/jsonbp/localization/messages.en_US.ini`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/localization/messages.pt_BR.ini` & `jsonbp-0.9.2/src/jsonbp/localization/messages.pt_BR.ini`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/parser.py` & `jsonbp-0.9.2/src/jsonbp/parser.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/ply/lex.py` & `jsonbp-0.9.2/src/jsonbp/ply/lex.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp/ply/yacc.py` & `jsonbp-0.9.2/src/jsonbp/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `jsonbp-0.9.1/src/jsonbp.egg-info/PKG-INFO` & `jsonbp-0.9.2/src/jsonbp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonbp
-Version: 0.9.1
+Version: 0.9.2
 Summary: JSON Python Deserializer
 Home-page: https://github.com/vottini/jsonbp
 Author: Gustavo Venturini
 Author-email: gustavo.c.venturini@gmail.com
 License: MIT
 Keywords: json,deserialization
 Platform: any
```

### Comparing `jsonbp-0.9.1/src/jsonbp.egg-info/SOURCES.txt` & `jsonbp-0.9.2/src/jsonbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

