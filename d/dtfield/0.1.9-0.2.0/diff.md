# Comparing `tmp/dtfield-0.1.9.tar.gz` & `tmp/dtfield-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.9.tar", max compression
+gzip compressed data, was "dtfield-0.2.0.tar", max compression
```

## Comparing `dtfield-0.1.9.tar` & `dtfield-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.9/dtfield/__init__.py
--rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.1.9/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.9/dtfield/base_enum.py
--rw-r--r--   0        0        0    21791 2023-06-13 02:35:07.521474 dtfield-0.1.9/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.9/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.9/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.9/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.9/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.9/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.9/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.9/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.9/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.9/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.1.9/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.9/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.9/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.9/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.9/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.9/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.9/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.9/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-13 02:35:07.524633 dtfield-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-13 02:35:11.747697 dtfield-0.1.9/setup.py
--rw-r--r--   0        0        0      503 2023-06-13 02:35:11.747905 dtfield-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.0/dtfield/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.0/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.0/dtfield/base_enum.py
+-rw-r--r--   0        0        0    22624 2023-06-14 00:41:24.943418 dtfield-0.2.0/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.0/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.0/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.0/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.0/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.0/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.0/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.0/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.0/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.0/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.0/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.0/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.0/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.0/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.0/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.0/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.0/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.0/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-14 00:41:24.955878 dtfield-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-14 00:41:32.063553 dtfield-0.2.0/setup.py
+-rw-r--r--   0        0        0      503 2023-06-14 00:41:32.063788 dtfield-0.2.0/PKG-INFO
```

### Comparing `dtfield-0.1.9/dtfield/_imports.py` & `dtfield-0.2.0/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/base_enum.py` & `dtfield-0.2.0/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/engine.py` & `dtfield-0.2.0/dtfield/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,28 +23,41 @@
         'lesser_than',
         'orderby',
         'ordered',
         'reversed_dict',
         'db_descriptors',
         'query_from_string',
         'exist_query',
-        'descriptors'
+        'descriptors',
+        'display_items',
+        'display_repr',
+        'eq_function',
+        'get_attr_or_item',
+        'filter_dict',
+        'make_dict',
+        'dict_items',
+        'normalize_lower_if_string',
+        'exclude_keys_from_dict'
 ]
 
 
 from deta.base import FetchResponse
 from dtfield._imports import *
 from dtbase import *
 from .parse import *
 from .functions import *
 
 
 context = copy_context()
 
 
+def exclude_keys_from_dict(data: Mapping, exclude: list[str]):
+    return {k: v for k, v in data.items() if not k in exclude}
+
+
 def get_attr_or_item(obj: Any, name: str = 'key'):
     if isinstance(obj, Mapping):
         return obj.get(name)
     elif hasattr(obj, name):
         return getattr(obj, 'key')
     raise AttributeError(f'O objeto "{obj}" não possuir uma chave ou attributo "{name}".')
 
@@ -182,16 +195,16 @@
     def descriptors(cls):
         return tuple(descriptors(cls))
     
     @classmethod
     def descriptorskeys(cls):
         return tuple([i.public_name for i in cls.descriptors()])
     
-    def asjson(self):
-        return json_parse(asdict(self))
+    def asjson(self, exclude: list[str] = None):
+        return json_parse(exclude_keys_from_dict(asdict(self), exclude or list()))
     
     def asjson_to_db(self):
         return json_parse(filter_dict(asdict(self), condition=lambda x: x[0] in db_descriptors(self).keys()))
 
 
         
 @dataclass
@@ -216,29 +229,37 @@
     def exist_params(cls):
         return cls.EXIST_PARAMS
     
     async def exist_response(self):
         return await DetaBase(self.table()).fetch(exist_query(self))
     
     async def save(self):
-        new = await DetaBase(self.table()).put(self.asjson_to_db())
+        new = await DetaBase(self.table()).insert(self.asjson_to_db())
         if new:
             await self.update_context()
             return self.safe_create(**new)
         return None
     
     async def save_new(self):
         exist = await self.exist_response()
         if exist.count == 0:
             return await self.save()
         elif exist.count == 1:
             return self.safe_create(**exist.items[0])
         else:
             return None
-    
+        
+    async def update_instance(self, **kwargs):
+        current = self.asjson()
+        current.update(exclude_keys_from_dict(kwargs, exclude=['key']))
+        key = current.pop('key')
+        updated = await DetaBase(self.table()).put(data=current, key=key)
+        await self.update_context()
+        return self.from_context(key)
+        
     
     @classmethod
     def singular(cls):
         return cls.SINGULAR or cls.clsname()
     
     @classmethod
     def plural(cls):
@@ -261,29 +282,30 @@
         return {d.public_name: d for d in cls.descriptorsmap().values() if d.has_dependants is True}
     
     @classmethod
     def model_dependants(cls, collection: list = None):
         return model_dependants(cls, collection or list())
 
     @classmethod
-    def from_context(cls, key: str) -> Self:
+    def from_context(cls, key: str = None) -> Self:
+        if key is None:
+            return None
         data = cls.get_context().get(key, None)
         if data:
             return cls.safe_create(**data)
         return None
     
     @classmethod
     async def set_context(cls):
         context.run(cls.CTXVAR.set, make_dict(await cls.fetch_all()))
         
     @classmethod
     def get_context(cls):
         return context.get(cls.CTXVAR)
 
-    
     @classmethod
     async def fetch_all(cls, query: DetaQuery = None) -> list[dict[str, Jsonable]]:
         return await DetaBase(cls.table()).fetch_all(query or cls.DETA_QUERY)
     
     @classmethod
     async def fetch(cls, query: DetaQuery = None, last: Optional[str] = None, limit: int = 1000) -> FetchResponse:
         return await DetaBase(cls.table()).fetch(query or cls.DETA_QUERY, last, limit)
```

### Comparing `dtfield-0.1.9/dtfield/functions.py` & `dtfield-0.2.0/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.2.0/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.2.0/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.2.0/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.2.0/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.2.0/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.2.0/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/dates.py` & `dtfield-0.2.0/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/json_encoder.py` & `dtfield-0.2.0/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/number.py` & `dtfield-0.2.0/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/string.py` & `dtfield-0.2.0/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/dtfield/parse/type_hint.py` & `dtfield-0.2.0/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.9/setup.py` & `dtfield-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

