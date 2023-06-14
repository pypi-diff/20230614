# Comparing `tmp/strawberry_django_plus-2.6.2.tar.gz` & `tmp/strawberry_django_plus-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.6.2.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.6.3.tar", max compression
```

## Comparing `strawberry_django_plus-2.6.2.tar` & `strawberry_django_plus-2.6.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1094 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/LICENSE
--rw-r--r--   0        0        0     3299 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/README.md
--rw-r--r--   0        0        0     4309 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0      896 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26108 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47691 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2357 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18673 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10297 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13223 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/LICENSE
+-rw-r--r--   0        0        0     3299 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/README.md
+-rw-r--r--   0        0        0     4309 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3054 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.117674 strawberry_django_plus-2.6.3/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0      896 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26108 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1357 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47691 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18649 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10297 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13223 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-14 18:50:30.121674 strawberry_django_plus-2.6.3/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.3/PKG-INFO
```

### Comparing `strawberry_django_plus-2.6.2/LICENSE` & `strawberry_django_plus-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/README.md` & `strawberry_django_plus-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/pyproject.toml` & `strawberry_django_plus-2.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.6.2"
+version = "2.6.3"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "2.6.2"  # x-release-please-version
+__version__ = "2.6.3"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/field.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from enum import Enum
 from typing import Any, Callable, Optional, Sequence, Type, TypeVar, cast
 
 from django.db.models.base import Model
 from django.db.models.sql.query import get_field_names_from_opts  # type: ignore
 from strawberry import UNSET
 from strawberry.field import StrawberryField
-from strawberry.utils.typing import __dataclass_transform__
 from strawberry_django import filters as _filters
 from strawberry_django import utils
 from strawberry_django.fields.field import field as _field
+from typing_extensions import dataclass_transform
 
 from . import field
 from .relay import GlobalID, connection, node
 from .type import input
 
 _T = TypeVar("_T")
 
@@ -65,17 +65,17 @@
     return filter_kwargs, filter_methods
 
 
 # Replace build_filter_kwargs by our implementation that can handle GlobalID
 _filters.build_filter_kwargs = _build_filter_kwargs
 
 
-@__dataclass_transform__(
+@dataclass_transform(
     order_default=True,
-    field_descriptors=(
+    field_specifiers=(
         StrawberryField,
         _field,
         node,
         connection,
         field.field,
         field.node,
         field.connection,
```

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/ordering.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Callable, Optional, Sequence, Type, TypeVar, cast
 
 import strawberry
 from django.db.models.base import Model
 from strawberry import UNSET
 from strawberry.field import StrawberryField
-from strawberry.utils.typing import __dataclass_transform__
 from strawberry_django.fields.field import field as _field
 from strawberry_django.ordering import Ordering
+from typing_extensions import dataclass_transform
 
 from strawberry_django_plus.utils.typing import is_auto
 
 from . import field
 from .relay import connection, node
 
 _T = TypeVar("_T")
 
 
-@__dataclass_transform__(
+@dataclass_transform(
     order_default=True,
-    field_descriptors=(
+    field_specifiers=(
         StrawberryField,
         _field,
         node,
         connection,
         field.field,
         field.node,
         field.connection,
```

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.6.3/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/test/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,18 @@
     ):
         kwargs: Dict[str, object] = {"data": body, "headers": headers}
         if files:
             kwargs["format"] = "multipart"
         else:
             kwargs["content_type"] = "application/json"
 
-        return self.client.post(self.path, **kwargs)
+        return self.client.post(
+            self.path,
+            **kwargs,  # type: ignore
+        )
 
     @contextlib.contextmanager
     def login(self, user: AbstractUser):
         self.client.force_login(user)
         yield
         self.client.logout()
```

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/type.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.exceptions import MissingFieldAnnotationError, PrivateStrawberryFieldError
 from strawberry.field import UNRESOLVED, StrawberryField
 from strawberry.private import is_private
 from strawberry.types import Info
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.unset import UnsetType
-from strawberry.utils.typing import __dataclass_transform__, eval_type
+from strawberry.utils.typing import eval_type
 from strawberry_django.fields.field import field as _field
 from strawberry_django.fields.types import get_model_field, resolve_model_field_name
 from strawberry_django.type import StrawberryDjangoType as _StraberryDjangoType
 from strawberry_django.utils import get_annotations, is_similar_django_type
-from typing_extensions import Annotated
+from typing_extensions import Annotated, dataclass_transform
 
 from strawberry_django_plus.optimizer import OptimizerStore, PrefetchType
 from strawberry_django_plus.utils.typing import TypeOrSequence, is_auto
 
 from . import field
 from .descriptors import ModelProperty
 from .field import StrawberryDjangoField, connection, node
@@ -358,17 +358,17 @@
     order: Optional[Union[type, UnsetType]]
     filters: Optional[Union[type, UnsetType]]
     pagination: Optional[Union[bool, UnsetType]]
     disable_optimization: bool
     store: OptimizerStore
 
 
-@__dataclass_transform__(
+@dataclass_transform(
     order_default=True,
-    field_descriptors=(
+    field_specifiers=(
         StrawberryField,
         _field,
         node,
         connection,
         field.field,
         field.node,
         field.connection,
@@ -425,17 +425,17 @@
             prefetch_related=prefetch_related,
             disable_optimization=disable_optimization,
         )
 
     return wrapper
 
 
-@__dataclass_transform__(
+@dataclass_transform(
     order_default=True,
-    field_descriptors=(
+    field_specifiers=(
         StrawberryField,
         _field,
         node,
         connection,
         field.field,
         field.node,
         field.connection,
@@ -471,17 +471,17 @@
             description=description,
             directives=directives,
         )
 
     return wrapper
 
 
-@__dataclass_transform__(
+@dataclass_transform(
     order_default=True,
-    field_descriptors=(
+    field_specifiers=(
         StrawberryField,
         _field,
         node,
         connection,
         field.field,
         field.node,
         field.connection,
@@ -521,17 +521,17 @@
             directives=directives,
             partial=partial,
         )
 
     return wrapper
 
 
-@__dataclass_transform__(
+@dataclass_transform(
     order_default=True,
-    field_descriptors=(
+    field_specifiers=(
         StrawberryField,
         _field,
         node,
         connection,
         field.field,
         field.node,
         field.connection,
```

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/types.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.6.3/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.2/PKG-INFO` & `strawberry_django_plus-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.6.2
+Version: 2.6.3
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

