# Comparing `tmp/django_ninja_crud-0.1.0.tar.gz` & `tmp/django_ninja_crud-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_crud-0.1.0.tar", max compression
+gzip compressed data, was "django_ninja_crud-0.1.1.tar", max compression
```

## Comparing `django_ninja_crud-0.1.0.tar` & `django_ninja_crud-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-06-10 11:57:11.729156 django_ninja_crud-0.1.0/LICENSE
--rw-r--r--   0        0        0      451 2023-06-11 15:42:17.942247 django_ninja_crud-0.1.0/README.md
--rw-r--r--   0        0        0      293 2023-06-10 13:47:48.223201 django_ninja_crud-0.1.0/ninja_crud/__init__.py
--rw-r--r--   0        0        0      151 2023-06-11 15:53:53.567181 django_ninja_crud-0.1.0/ninja_crud/apps.py
--rw-r--r--   0        0        0      574 2023-06-10 21:56:23.750270 django_ninja_crud-0.1.0/ninja_crud/tests/__init__.py
--rw-r--r--   0        0        0     5225 2023-06-11 15:51:50.222750 django_ninja_crud-0.1.0/ninja_crud/tests/test_abstract.py
--rw-r--r--   0        0        0     4637 2023-06-11 15:51:50.216703 django_ninja_crud-0.1.0/ninja_crud/tests/test_create.py
--rw-r--r--   0        0        0     2593 2023-06-11 15:51:50.236472 django_ninja_crud-0.1.0/ninja_crud/tests/test_delete.py
--rw-r--r--   0        0        0     3300 2023-06-11 15:51:50.207121 django_ninja_crud-0.1.0/ninja_crud/tests/test_list.py
--rw-r--r--   0        0        0     3064 2023-06-11 15:51:50.241315 django_ninja_crud-0.1.0/ninja_crud/tests/test_retrieve.py
--rw-r--r--   0        0        0     4515 2023-06-11 15:51:50.231286 django_ninja_crud-0.1.0/ninja_crud/tests/test_update.py
--rw-r--r--   0        0        0      346 2023-06-11 15:24:40.144029 django_ninja_crud-0.1.0/ninja_crud/tests/utils.py
--rw-r--r--   0        0        0      397 2023-06-11 13:09:53.064995 django_ninja_crud-0.1.0/ninja_crud/utils.py
--rw-r--r--   0        0        0      409 2023-06-10 15:53:09.464020 django_ninja_crud-0.1.0/ninja_crud/views/__init__.py
--rw-r--r--   0        0        0      796 2023-06-04 15:07:06.501956 django_ninja_crud-0.1.0/ninja_crud/views/abstract.py
--rw-r--r--   0        0        0     3876 2023-06-11 15:51:50.219466 django_ninja_crud-0.1.0/ninja_crud/views/create.py
--rw-r--r--   0        0        0     1550 2023-06-11 15:51:50.228343 django_ninja_crud-0.1.0/ninja_crud/views/delete.py
--rw-r--r--   0        0        0     3975 2023-06-11 15:51:50.225594 django_ninja_crud-0.1.0/ninja_crud/views/list.py
--rw-r--r--   0        0        0     1547 2023-06-11 15:51:50.233876 django_ninja_crud-0.1.0/ninja_crud/views/retrieve.py
--rw-r--r--   0        0        0     1958 2023-06-11 15:51:50.210361 django_ninja_crud-0.1.0/ninja_crud/views/update.py
--rw-r--r--   0        0        0     1611 2023-06-11 16:10:10.036264 django_ninja_crud-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4083 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/ninja_crud/__init__.py
+-rw-r--r--   0        0        0      151 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/ninja_crud/apps.py
+-rw-r--r--   0        0        0      574 2023-06-14 11:56:18.628616 django_ninja_crud-0.1.1/ninja_crud/tests/__init__.py
+-rw-r--r--   0        0        0     5225 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_abstract.py
+-rw-r--r--   0        0        0     4637 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_create.py
+-rw-r--r--   0        0        0     2593 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_delete.py
+-rw-r--r--   0        0        0     3300 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_list.py
+-rw-r--r--   0        0        0     3064 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_retrieve.py
+-rw-r--r--   0        0        0     4515 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/test_update.py
+-rw-r--r--   0        0        0      303 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/tests/utils.py
+-rw-r--r--   0        0        0      397 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/utils.py
+-rw-r--r--   0        0        0      409 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/abstract.py
+-rw-r--r--   0        0        0     3876 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/create.py
+-rw-r--r--   0        0        0     1551 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/delete.py
+-rw-r--r--   0        0        0     3975 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/list.py
+-rw-r--r--   0        0        0     1548 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/retrieve.py
+-rw-r--r--   0        0        0     1959 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/ninja_crud/views/update.py
+-rw-r--r--   0        0        0     1611 2023-06-14 11:56:18.632616 django_ninja_crud-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 django_ninja_crud-0.1.1/PKG-INFO
```

### Comparing `django_ninja_crud-0.1.0/LICENSE` & `django_ninja_crud-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/__init__.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/test_abstract.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/test_abstract.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from typing import Callable, List, NamedTuple, Optional, Tuple, Type
 
 from django.db.models import Model, QuerySet
 from django.http import HttpResponse
 from django.test import Client, TestCase
 from ninja import Schema
 
+from ninja_crud.tests.utils import default_serializer
 from ninja_crud.views import (
     AbstractModelView,
     CreateModelView,
     ListModelView,
     ModelViewSet,
 )
-from ninja_crud.tests.utils import default_serializer
 
 
 class Credentials(NamedTuple):
     ok: dict
     forbidden: Optional[dict] = None
     unauthorized: Optional[dict] = None
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/test_create.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/test_create.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
 from ninja_crud import utils
-from ninja_crud.views.create import CreateModelView
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials, Payloads
+from ninja_crud.views.create import CreateModelView
 
 
 class CreateModelViewTest(AbstractModelViewTest):
     model_view = CreateModelView
 
     def __init__(
         self,
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/test_delete.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/test_delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
-from ninja_crud.views.delete import DeleteModelView
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
+from ninja_crud.views.delete import DeleteModelView
 
 
 class DeleteModelViewTest(AbstractModelViewTest):
     model_view = DeleteModelView
 
     def delete_model(self, id: UUID, credentials: Optional[dict]) -> HttpResponse:
         if credentials is None:
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/test_list.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/test_list.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
-from ninja_crud.views.list import ListModelView
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
+from ninja_crud.views.list import ListModelView
 
 
 class ListModelViewTest(AbstractModelViewTest):
     model_view = ListModelView
 
     def list_model(self, id: UUID, credentials: Optional[dict]) -> HttpResponse:
         if credentials is None:
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/test_retrieve.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/test_retrieve.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.urls import reverse
 
 from ninja_crud import utils
-from ninja_crud.views.retrieve import RetrieveModelView
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials
+from ninja_crud.views.retrieve import RetrieveModelView
 
 
 class RetrieveModelViewTest(AbstractModelViewTest):
     model_view = RetrieveModelView
 
     def retrieve_model(self, id: UUID, credentials: Optional[dict]) -> HttpResponse:
         if credentials is None:
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/tests/test_update.py` & `django_ninja_crud-0.1.1/ninja_crud/tests/test_update.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from django.db.models import Model
 from django.http import HttpResponse
 from django.test import TestCase
 from django.urls import reverse
 
 from ninja_crud import utils
-from ninja_crud.views.update import UpdateModelView
 from ninja_crud.tests.test_abstract import AbstractModelViewTest, Credentials, Payloads
+from ninja_crud.views.update import UpdateModelView
 
 
 class UpdateModelViewTest(AbstractModelViewTest):
     model_view = UpdateModelView
 
     def __init__(
         self,
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/views/abstract.py` & `django_ninja_crud-0.1.1/ninja_crud/views/abstract.py`

 * *Files identical despite different names*

### Comparing `django_ninja_crud-0.1.0/ninja_crud/views/create.py` & `django_ninja_crud-0.1.1/ninja_crud/views/create.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router, Schema
 
 from ninja_crud import utils
-from ninja_crud.views.abstract import AbstractModelView
 from ninja_crud.utils import merge_decorators
+from ninja_crud.views.abstract import AbstractModelView
 
 
 class CreateModelView(AbstractModelView):
     def __init__(
         self,
         input_schema: Type[Schema],
         output_schema: Type[Schema],
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/views/delete.py` & `django_ninja_crud-0.1.1/ninja_crud/views/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from http import HTTPStatus
 from typing import Callable, List, Type
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router
+
 from ninja_crud import utils
-from ninja_crud.views.abstract import AbstractModelView
 from ninja_crud.utils import merge_decorators
+from ninja_crud.views.abstract import AbstractModelView
 
 
 class DeleteModelView(AbstractModelView):
     def __init__(
         self,
         decorators: List[Callable] = None,
         pre_delete: Callable[[HttpRequest, Model], None] = None,
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/views/list.py` & `django_ninja_crud-0.1.1/ninja_crud/views/list.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from django.db.models import Model, QuerySet
 from django.http import HttpRequest
 from ninja import FilterSchema, Query, Router, Schema
 from ninja.pagination import LimitOffsetPagination, paginate
 
 from ninja_crud import utils
-from ninja_crud.views.abstract import AbstractModelView
 from ninja_crud.utils import merge_decorators
+from ninja_crud.views.abstract import AbstractModelView
 
 
 class ListModelView(AbstractModelView):
     def __init__(
         self,
         output_schema: Type[Schema],
         filter_schema: Type[FilterSchema] = None,
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/views/retrieve.py` & `django_ninja_crud-0.1.1/ninja_crud/views/retrieve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from http import HTTPStatus
 from typing import Callable, List, Type
 from uuid import UUID
 
 from django.db.models import Model, QuerySet
 from django.http import HttpRequest
 from ninja import Router, Schema
+
 from ninja_crud import utils
-from ninja_crud.views.abstract import AbstractModelView
 from ninja_crud.utils import merge_decorators
+from ninja_crud.views.abstract import AbstractModelView
 
 
 class RetrieveModelView(AbstractModelView):
     def __init__(
         self,
         output_schema: Type[Schema],
         queryset_getter: Callable[[UUID], QuerySet[Model]] = None,
```

### Comparing `django_ninja_crud-0.1.0/ninja_crud/views/update.py` & `django_ninja_crud-0.1.1/ninja_crud/views/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from http import HTTPStatus
 from typing import Callable, List, Type
 from uuid import UUID
 
 from django.db.models import Model
 from django.http import HttpRequest
 from ninja import Router, Schema
+
 from ninja_crud import utils
-from ninja_crud.views.abstract import AbstractModelView
 from ninja_crud.utils import merge_decorators
+from ninja_crud.views.abstract import AbstractModelView
 
 
 class UpdateModelView(AbstractModelView):
     def __init__(
         self,
         input_schema: Type[Schema],
         output_schema: Type[Schema],
```

### Comparing `django_ninja_crud-0.1.0/pyproject.toml` & `django_ninja_crud-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["ninja_crud", "tests", "examples"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "django-ninja-crud"
-version = "0.1.0"
+version = "0.1.1"
 description = "Django Ninja CRUD is a library that allows you to create CRUD APIs in a few lines of code."
 authors = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 maintainers = ["Hicham Bakri <hicham.bakri76@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/hbakri/django-ninja-crud"
 license = "MIT"
 classifiers = [
```

