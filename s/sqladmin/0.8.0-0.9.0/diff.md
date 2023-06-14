# Comparing `tmp/sqladmin-0.8.0.tar.gz` & `tmp/sqladmin-0.9.0.tar.gz`

## Comparing `sqladmin-0.8.0.tar` & `sqladmin-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/__init__.py
--rw-r--r--   0        0        0     7991 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/_queries.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/_types.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/_validators.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/ajax.py
--rw-r--r--   0        0        0    19962 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/application.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/authentication.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/exceptions.py
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/fields.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/formatters.py
--rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/forms.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/helpers.py
--rw-r--r--   0        0        0    35151 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/models.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/py.typed
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/widgets.py
--rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/css/flatpickr.min.css
--rw-r--r--   0        0        0    68945 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/css/fontawesome.min.css
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/css/main.css
--rw-r--r--   0        0        0    14966 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/css/select2.min.css
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/css/solid.min.css
--rw-r--r--   0        0        0   279740 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/css/tabler.min.css
--rw-r--r--   0        0        0    62399 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/bootstrap.min.js
--rw-r--r--   0        0        0    58060 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/flatpickr.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/jquery.min.js
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/main.js
--rw-r--r--   0        0        0    19167 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/popper.min.js
--rw-r--r--   0        0        0    79212 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/select2.full.min.js
--rw-r--r--   0        0        0   137925 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/js/tabler.min.js
--rw-r--r--   0        0        0   303480 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   126828 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/statics/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/base.html
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/create.html
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/details.html
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/edit.html
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/error.html
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/index.html
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/layout.html
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/list.html
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/login.html
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sqladmin-0.8.0/sqladmin/templates/modals/delete.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sqladmin-0.8.0/.gitignore
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 sqladmin-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 sqladmin-0.8.0/README.md
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 sqladmin-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 sqladmin-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/__init__.py
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/_queries.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/_types.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/_validators.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/ajax.py
+-rw-r--r--   0        0        0    19994 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/application.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/authentication.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/exceptions.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/fields.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/formatters.py
+-rw-r--r--   0        0        0    19569 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/forms.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/helpers.py
+-rw-r--r--   0        0        0    35612 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/models.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/py.typed
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/widgets.py
+-rw-r--r--   0        0        0    16166 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/css/flatpickr.min.css
+-rw-r--r--   0        0        0    68945 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/css/fontawesome.min.css
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/css/main.css
+-rw-r--r--   0        0        0    14966 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/css/select2.min.css
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/css/solid.min.css
+-rw-r--r--   0        0        0   279740 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/css/tabler.min.css
+-rw-r--r--   0        0        0    62399 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/bootstrap.min.js
+-rw-r--r--   0        0        0    58060 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/flatpickr.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/jquery.min.js
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/main.js
+-rw-r--r--   0        0        0    19167 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/popper.min.js
+-rw-r--r--   0        0        0    79212 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/select2.full.min.js
+-rw-r--r--   0        0        0   137925 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/js/tabler.min.js
+-rw-r--r--   0        0        0   303480 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   126828 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/statics/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/base.html
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/create.html
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/details.html
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/edit.html
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/error.html
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/index.html
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/layout.html
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/list.html
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/login.html
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 sqladmin-0.9.0/sqladmin/templates/modals/delete.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 sqladmin-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 sqladmin-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 sqladmin-0.9.0/README.md
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 sqladmin-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 sqladmin-0.9.0/PKG-INFO
```

### Comparing `sqladmin-0.8.0/sqladmin/_queries.py` & `sqladmin-0.9.0/sqladmin/_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-from re import L
 from typing import TYPE_CHECKING, Any, Dict, List
 
 import anyio
 from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Session, joinedload
 from sqlalchemy.sql.expression import Select
 
-from sqladmin._types import MODEL_ATTR_TYPE
+from sqladmin._types import MODEL_PROPERTY
 from sqladmin.helpers import get_column_python_type, get_direction, get_primary_key
 
 if TYPE_CHECKING:
     from sqladmin.models import ModelView
 
 
 class Query:
     def __init__(self, model_view: "ModelView") -> None:
         self.model_view = model_view
 
-    def _get_to_many_stmt(self, relation: MODEL_ATTR_TYPE, values: List[Any]) -> Select:
+    def _get_to_many_stmt(self, relation: MODEL_PROPERTY, values: List[Any]) -> Select:
         target = relation.mapper.class_
         target_pk = get_primary_key(target)
         target_pk_type = get_column_python_type(target_pk)
         pk_values = [target_pk_type(value) for value in values]
         related_stmt = select(target).where(target_pk.in_(pk_values))
         return related_stmt
 
-    def _get_to_one_stmt(self, relation: MODEL_ATTR_TYPE, value: Any) -> Select:
+    def _get_to_one_stmt(self, relation: MODEL_PROPERTY, value: Any) -> Select:
         target = relation.mapper.class_
         target_pk = get_primary_key(target)
         target_pk_type = get_column_python_type(target_pk)
         related_stmt = select(target).where(target_pk == target_pk_type(value))
         return related_stmt
 
-    def _set_many_to_one(self, obj: Any, relation: MODEL_ATTR_TYPE, value: Any) -> Any:
+    def _set_many_to_one(self, obj: Any, relation: MODEL_PROPERTY, value: Any) -> Any:
         fk = relation.local_remote_pairs[0][0]
         fk_type = get_column_python_type(fk)
         setattr(obj, fk.name, fk_type(value))
         return obj
 
     def _set_attributes_sync(self, session: Session, obj: Any, data: dict) -> Any:
         for key, value in data.items():
@@ -115,16 +114,16 @@
             anyio.from_thread.run(self.model_view.after_model_change, data, obj, False)
             return obj
 
     async def _update_async(self, pk: Any, data: Dict[str, Any]) -> Any:
         pk = get_column_python_type(self.model_view.pk_column)(pk)
         stmt = select(self.model_view.model).where(self.model_view.pk_column == pk)
 
-        for relation in self.model_view._relations:
-            stmt = stmt.options(joinedload(relation.key))
+        for relation in self.model_view._relation_attrs:
+            stmt = stmt.options(joinedload(relation))
 
         async with self.model_view.sessionmaker(expire_on_commit=False) as session:
             result = await session.execute(stmt)
             obj = result.scalars().first()
             await self.model_view.on_model_change(data, obj, False)
             obj = await self._set_attributes_async(session, obj, data)
             await session.commit()
```

### Comparing `sqladmin-0.8.0/sqladmin/_validators.py` & `sqladmin-0.9.0/sqladmin/_validators.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,38 @@
 
         try:
             Currency(field.data)
         except (TypeError, ValueError):
             raise ValidationError("Not a valid ISO currency code (e.g. USD, EUR, CNY).")
 
 
+class PhoneNumberValidator:
+    """Form validator for sqlalchemy_utils PhoneNumberType."""
+
+    def __call__(self, form: Form, field: Field) -> None:
+        from sqlalchemy_utils import PhoneNumber, PhoneNumberParseException
+
+        try:
+            PhoneNumber(field.data)
+        except PhoneNumberParseException:
+            raise ValidationError("Not a valid phone number.")
+
+
+class ColorValidator:
+    """General Color validator using `colour` package."""
+
+    def __call__(self, form: Form, field: Field) -> None:
+        from colour import Color
+
+        try:
+            Color(field.data)
+        except ValueError:
+            raise ValidationError('Not a valid color (e.g. "red", "#f00", "#ff0000").')
+
+
 class TimezoneValidator:
     """Form validator for sqlalchemy_utils TimezoneType."""
 
     def __init__(self, coerce_function: Callable[[Any], Any]) -> None:
         self.coerce_function = coerce_function
 
     def __call__(self, form: Form, field: Field) -> None:
```

### Comparing `sqladmin-0.8.0/sqladmin/ajax.py` & `sqladmin-0.9.0/sqladmin/ajax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TYPE_CHECKING, Any, Dict, List
 
-from sqlalchemy import String, cast, inspect, or_, select, text
+from sqlalchemy import String, cast, inspect, or_, select
 
 from sqladmin.helpers import get_primary_key
 
 if TYPE_CHECKING:
     from sqladmin.models import ModelView
```

### Comparing `sqladmin-0.8.0/sqladmin/application.py` & `sqladmin-0.9.0/sqladmin/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,18 @@
 
         data = [loader.format(m) for m in await loader.get_list(term)]
         return JSONResponse({"results": data})
 
     def get_save_redirect_url(
         self, request: Request, form: FormData, model_view: ModelView, obj: Any
     ) -> str:
-        """Get the redirect URL after a save action is triggered from create/edit page."""
+        """
+        Get the redirect URL after a save action
+        which is triggered from create/edit page.
+        """
 
         identity = request.path_params["identity"]
         pk = getattr(obj, model_view.pk_column.name)
 
         if form.get("save") == "Save":
             return request.url_for("admin:list", identity=identity)
         elif form.get("save") == "Save and continue editing" or (
```

### Comparing `sqladmin-0.8.0/sqladmin/authentication.py` & `sqladmin-0.9.0/sqladmin/authentication.py`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/fields.py` & `sqladmin-0.9.0/sqladmin/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import operator
 from typing import Any, Callable, Generator, List, Optional, Set, Tuple, Union
 
 from sqlalchemy import inspect
-from wtforms import Form, SelectFieldBase, ValidationError, fields, widgets
+from wtforms import Form, ValidationError, fields, widgets
 
 from sqladmin import widgets as sqladmin_widgets
 from sqladmin.ajax import QueryAjaxModelLoader
 
 __all__ = [
     "AjaxSelectField",
     "AjaxSelectMultipleField",
@@ -162,15 +162,19 @@
         self._formdata = None
 
     def iter_choices(self) -> Generator[Tuple[str, str, bool], None, None]:
         if self.allow_blank:
             yield ("__None", self.blank_text, self.data is None)
 
         if self.data:
-            primary_key = str(inspect(self.data).identity[0])
+            primary_key = (
+                self.data
+                if isinstance(self.data, str)
+                else str(inspect(self.data).identity[0])
+            )
         else:
             primary_key = None
 
         for pk, label in self._select_data:
             yield (pk, self.get_label(label), str(pk) == primary_key)
 
     def process_formdata(self, valuelist: List[str]) -> None:
@@ -247,15 +251,19 @@
     @data.setter
     def data(self, data: tuple) -> None:
         self._data = data
         self._formdata = None
 
     def iter_choices(self) -> Generator[Tuple[str, Any, bool], None, None]:
         if self.data is not None:
-            primary_keys = [str(inspect(m).identity[0]) for m in self.data]
+            primary_keys = (
+                self.data
+                if all(isinstance(d, str) for d in self.data)
+                else [str(inspect(m).identity[0]) for m in self.data]
+            )
             for pk, label in self._select_data:
                 yield (pk, self.get_label(label), pk in primary_keys)
 
     def process_formdata(self, valuelist: List[str]) -> None:
         self._formdata = list(set(valuelist))
 
     def pre_validate(self, form: Form) -> None:
@@ -264,15 +272,15 @@
         elif self.data:
             pk_list = [x[0] for x in self._select_data]
             for v in self.data:
                 if v not in pk_list:  # pragma: no cover
                     raise ValidationError(self.gettext("Not a valid choice"))
 
 
-class AjaxSelectField(SelectFieldBase):
+class AjaxSelectField(fields.SelectFieldBase):
     widget = sqladmin_widgets.AjaxSelect2Widget()
     separator = ","
 
     def __init__(
         self,
         loader: QueryAjaxModelLoader,
         label: Optional[str] = None,
@@ -306,15 +314,15 @@
                 self._formdata = valuelist[0]
 
     def pre_validate(self, form: Form) -> None:
         if not self.allow_blank and self.data is None:
             raise ValidationError("Not a valid choice")
 
 
-class AjaxSelectMultipleField(SelectFieldBase):
+class AjaxSelectMultipleField(fields.SelectFieldBase):
     widget = sqladmin_widgets.AjaxSelect2Widget(multiple=True)
     separator = ","
 
     def __init__(
         self,
         loader: QueryAjaxModelLoader,
         label: Optional[str] = None,
@@ -345,7 +353,20 @@
 
     def process_formdata(self, valuelist: list) -> None:
         self._formdata = set()
 
         for field in valuelist:
             for n in field.split(self.separator):
                 self._formdata.add(n)
+
+
+class Select2TagsField(fields.SelectField):
+    widget = sqladmin_widgets.Select2TagsWidget()
+
+    def pre_validate(self, form: Form) -> None:
+        ...
+
+    def process_formdata(self, valuelist: list) -> None:
+        self.data = valuelist
+
+    def process_data(self, value: Optional[list]) -> None:
+        self.data = value or []
```

### Comparing `sqladmin-0.8.0/sqladmin/forms.py` & `sqladmin-0.9.0/sqladmin/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,32 @@
     IntegerField,
     StringField,
     TextAreaField,
     validators,
 )
 from wtforms.fields.core import UnboundField
 
-from sqladmin._types import ENGINE_TYPE, MODEL_ATTR_TYPE
-from sqladmin._validators import CurrencyValidator, TimezoneValidator
+from sqladmin._types import ENGINE_TYPE, MODEL_PROPERTY
+from sqladmin._validators import (
+    ColorValidator,
+    CurrencyValidator,
+    PhoneNumberValidator,
+    TimezoneValidator,
+)
 from sqladmin.ajax import QueryAjaxModelLoader
 from sqladmin.exceptions import NoConverterFound
 from sqladmin.fields import (
     AjaxSelectField,
     AjaxSelectMultipleField,
     DateField,
     DateTimeField,
     JSONField,
     QuerySelectField,
     QuerySelectMultipleField,
+    Select2TagsField,
     SelectField,
     TimeField,
 )
 from sqladmin.helpers import get_direction, get_primary_key, is_relationship
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
@@ -64,15 +70,15 @@
         ...  # pragma: no cover
 
 
 class ConverterCallable(Protocol):
     def __call__(
         self,
         model: type,
-        prop: MODEL_ATTR_TYPE,
+        prop: MODEL_PROPERTY,
         kwargs: Dict[str, Any],
     ) -> UnboundField:
         ...  # pragma: no cover
 
 
 T_CC = TypeVar("T_CC", bound=ConverterCallable)
 
@@ -102,22 +108,25 @@
                 for classname in obj._converter_for:
                     converters[classname] = obj
 
         self._converters = converters
 
     async def _prepare_kwargs(
         self,
-        prop: MODEL_ATTR_TYPE,
+        prop: MODEL_PROPERTY,
         engine: ENGINE_TYPE,
         field_args: Dict[str, Any],
         field_widget_args: Dict[str, Any],
         form_include_pk: bool,
         label: Optional[str] = None,
         loader: Optional[QueryAjaxModelLoader] = None,
     ) -> Optional[Dict[str, Any]]:
+        if not isinstance(prop, (RelationshipProperty, ColumnProperty)):
+            return None
+
         kwargs: Union[dict, None]
         kwargs = field_args.copy()
         widget_args = field_widget_args.copy()
         widget_args.setdefault("class", "form-control")
 
         kwargs.setdefault("label", label)
         kwargs.setdefault("validators", [])
@@ -218,15 +227,15 @@
                 return [
                     (self._get_pk_value(obj, pk), str(obj))
                     for obj in objects.scalars().all()
                 ]
 
         return []  # pragma: nocover
 
-    def get_converter(self, prop: MODEL_ATTR_TYPE) -> ConverterCallable:
+    def get_converter(self, prop: MODEL_PROPERTY) -> ConverterCallable:
         if isinstance(prop, RelationshipProperty):
             direction = get_direction(prop)
             return self._converters[direction]
 
         column = prop.columns[0]
         types = inspect.getmro(type(column.type))
 
@@ -255,15 +264,15 @@
         raise NoConverterFound(  # pragma: nocover
             f"Could not find field converter for column {column.name} ({types[0]!r})."
         )
 
     async def convert(
         self,
         model: type,
-        prop: MODEL_ATTR_TYPE,
+        prop: MODEL_PROPERTY,
         engine: ENGINE_TYPE,
         field_args: Dict[str, Any],
         field_widget_args: Dict[str, Any],
         form_include_pk: bool,
         label: Optional[str] = None,
         override: Optional[Type[Field]] = None,
         form_ajax_refs: Dict[str, QueryAjaxModelLoader] = {},
@@ -408,45 +417,58 @@
     # @converts("dialects.mysql.types.YEAR", "dialects.mysql.base.YEAR")
     # def conv_MSYear(self, field_args: Dict, **kwargs: Any) -> Field:
     #     field_args["validators"].append(validators.NumberRange(min=1901, max=2155))
     #     return StringField(**field_args)
 
     @converts(
         "sqlalchemy.dialects.postgresql.base.INET",
+        "sqlalchemy.dialects.postgresql.types.INET",
         "sqlalchemy_utils.types.ip_address.IPAddressType",
     )
     def conv_ip_address(
         self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
     ) -> UnboundField:
         kwargs.setdefault("label", "IP Address")
         kwargs.setdefault("validators", [])
         kwargs["validators"].append(validators.IPAddress(ipv4=True, ipv6=True))
         return StringField(**kwargs)
 
-    @converts("sqlalchemy.dialects.postgresql.base.MACADDR")
+    @converts(
+        "sqlalchemy.dialects.postgresql.base.MACADDR",
+        "sqlalchemy.dialects.postgresql.types.MACADDR",
+    )
     def conv_mac_address(
         self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
     ) -> UnboundField:
         kwargs.setdefault("label", "MAC Address")
         kwargs.setdefault("validators", [])
         kwargs["validators"].append(validators.MacAddress())
         return StringField(**kwargs)
 
     @converts(
         "sqlalchemy.dialects.postgresql.base.UUID",
+        "sqlalchemy.sql.sqltypes.UUID",
         "sqlalchemy_utils.types.uuid.UUIDType",
     )
     def conv_uuid(
         self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
     ) -> UnboundField:
         kwargs.setdefault("label", "UUID")
         kwargs.setdefault("validators", [])
         kwargs["validators"].append(validators.UUID())
         return StringField(**kwargs)
 
+    @converts(
+        "sqlalchemy.dialects.postgresql.base.ARRAY", "sqlalchemy.sql.sqltypes.ARRAY"
+    )
+    def conv_ARRAY(
+        self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
+    ) -> UnboundField:
+        return Select2TagsField(**kwargs)
+
     @converts("sqlalchemy_utils.types.email.EmailType")
     def conv_email(
         self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
     ) -> UnboundField:
         kwargs.setdefault("label", "Email")
         kwargs.setdefault("validators", [])
         kwargs["validators"].append(validators.Email())
@@ -474,14 +496,30 @@
     ) -> UnboundField:
         kwargs.setdefault("validators", [])
         kwargs["validators"].append(
             TimezoneValidator(coerce_function=prop.columns[0].type._coerce)
         )
         return StringField(**kwargs)
 
+    @converts("sqlalchemy_utils.types.phone_number.PhoneNumberType")
+    def conv_phone_number(
+        self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
+    ) -> UnboundField:
+        kwargs.setdefault("validators", [])
+        kwargs["validators"].append(PhoneNumberValidator())
+        return StringField(**kwargs)
+
+    @converts("sqlalchemy_utils.types.color.ColorType")
+    def conv_color(
+        self, model: type, prop: ColumnProperty, kwargs: Dict[str, Any]
+    ) -> UnboundField:
+        kwargs.setdefault("validators", [])
+        kwargs["validators"].append(ColorValidator())
+        return StringField(**kwargs)
+
     @converts("ONETOONE")
     def conv_one_to_one(
         self, model: type, prop: RelationshipProperty, kwargs: Dict[str, Any]
     ) -> UnboundField:
         kwargs["allow_blank"] = True
         return QuerySelectField(**kwargs)
 
@@ -506,17 +544,18 @@
     column_labels: Optional[Dict[str, str]] = None,
     form_args: Optional[Dict[str, Dict[str, Any]]] = None,
     form_widget_args: Optional[Dict[str, Dict[str, Any]]] = None,
     form_class: Type[Form] = Form,
     form_overrides: Optional[Dict[str, Type[Field]]] = None,
     form_ajax_refs: Optional[Dict[str, QueryAjaxModelLoader]] = None,
     form_include_pk: bool = False,
+    form_converter: Type[ModelConverterBase] = ModelConverter,
 ) -> Type[Form]:
     type_name = model.__name__ + "Form"
-    converter = ModelConverter()
+    converter = form_converter()
     mapper = sqlalchemy_inspect(model)
     form_args = form_args or {}
     form_widget_args = form_widget_args or {}
     column_labels = column_labels or {}
     form_overrides = form_overrides or {}
     form_ajax_refs = form_ajax_refs or {}
```

### Comparing `sqladmin-0.8.0/sqladmin/helpers.py` & `sqladmin-0.9.0/sqladmin/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import csv
 import os
 import re
 import unicodedata
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Generator, List, TypeVar, Union
+from typing import Callable, Generator, List, TypeVar
 
 from sqlalchemy import Column, inspect
 from sqlalchemy.orm import RelationshipProperty
 
-from sqladmin._types import MODEL_ATTR_TYPE
+from sqladmin._types import MODEL_PROPERTY
 
 T = TypeVar("T")
 
 
 _filename_ascii_strip_re = re.compile(r"[^A-Za-z0-9_.-]")
 _windows_device_files = (
     "CON",
@@ -115,32 +115,26 @@
 
 def get_primary_key(model: type) -> Column:
     pks = inspect(model).mapper.primary_key
     assert len(pks) == 1, "Multiple Primary Keys not supported."
     return pks[0]
 
 
-def get_relationships(model: Any) -> List[MODEL_ATTR_TYPE]:
-    return list(inspect(model).relationships)
-
-
-def get_attributes(model: Any) -> List[MODEL_ATTR_TYPE]:
-    return list(inspect(model).attrs)
-
-
-def get_direction(attr: MODEL_ATTR_TYPE) -> str:
-    assert isinstance(attr, RelationshipProperty)
-    name = attr.direction.name
-    if name == "ONETOMANY" and not attr.uselist:
+def get_direction(prop: MODEL_PROPERTY) -> str:
+    assert isinstance(prop, RelationshipProperty)
+    name = prop.direction.name
+    if name == "ONETOMANY" and not prop.uselist:
         return "ONETOONE"
     return name
 
 
 def get_column_python_type(column: Column) -> type:
     try:
+        if hasattr(column.type, "impl"):
+            return column.type.impl.python_type
         return column.type.python_type
     except NotImplementedError:
         return str
 
 
-def is_relationship(attr: MODEL_ATTR_TYPE) -> bool:
-    return isinstance(attr, RelationshipProperty)
+def is_relationship(prop: MODEL_PROPERTY) -> bool:
+    return isinstance(prop, RelationshipProperty)
```

### Comparing `sqladmin-0.8.0/sqladmin/models.py` & `sqladmin-0.9.0/sqladmin/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,23 @@
 from sqlalchemy.sql.expression import Select, select
 from starlette.requests import Request
 from starlette.responses import StreamingResponse
 from starlette.templating import Jinja2Templates
 from wtforms import Field, Form
 
 from sqladmin._queries import Query
-from sqladmin._types import ENGINE_TYPE, MODEL_ATTR_TYPE
+from sqladmin._types import ENGINE_TYPE, MODEL_PROPERTY
 from sqladmin.ajax import create_ajax_loader
 from sqladmin.exceptions import InvalidColumnError, InvalidModelError
 from sqladmin.formatters import BASE_FORMATTERS
-from sqladmin.forms import get_model_form
+from sqladmin.forms import ModelConverter, ModelConverterBase, get_model_form
 from sqladmin.helpers import (
     Writer,
-    get_attributes,
     get_column_python_type,
     get_primary_key,
-    get_relationships,
     prettify_class_name,
     secure_filename,
     slugify_class_name,
     stream_to_csv,
 )
 from sqladmin.pagination import Pagination
 
@@ -395,23 +393,28 @@
             pass
         ```
     """
 
     save_as: ClassVar[bool] = False
     """Set `save_as` to enable a “save as new” feature on admin change forms.
 
-    Normally, objects have three save options: “Save”, “Save and continue editing”, and “Save and add another”.
-    If save_as is True, “Save and add another” will be replaced by a “Save as new” button 
-    that creates a new object (with a new ID) rather than updating the existing object.
+    Normally, objects have three save options:
+    ``Save`, `Save and continue editing` and `Save and add another`.
+
+    If save_as is True, `Save and add another` will be replaced 
+    by a `Save as new` button 
+    that creates a new object (with a new ID) 
+    rather than updating the existing object.
 
     By default, `save_as` is set to `False`.
     """
 
     save_as_continue: ClassVar[bool] = True
-    """When `save_as=True`, the default redirect after saving the new object is to the edit view for that object.
+    """When `save_as=True`, the default redirect after saving the new object 
+    is to the edit view for that object.
     If you set `save_as_continue=False`, the redirect will be to the list view.
 
     By default, `save_as_continue` is set to `True`.
     """
 
     # Templates
     list_template: ClassVar[str] = "list.html"
@@ -579,14 +582,28 @@
                     'fields': ('street', 'zip_code'),
                     'order_by': ('id',),
                 }
             }
         ```
     """
 
+    form_converter: ClassVar[Type[ModelConverterBase]] = ModelConverter
+    """Custom form converter class.
+    Useful if you want to add custom form conversion in addition to the defaults.
+
+    ???+ example
+        ```python
+        class PhoneNumberConverter(ModelConverter):
+            pass
+
+        class UserAdmin(ModelAdmin, model=User):
+            form_converter = PhoneNumberConverter
+        ```
+    """
+
     # General options
     column_labels: ClassVar[Dict[Union[str, InstrumentedAttribute], str]] = {}
     """A mapping of column labels, used to map column names to new names.
     Dictionary keys can be string names or SQLAlchemy columns with string values.
 
     ???+ example
         ```python
@@ -639,60 +656,66 @@
         class UserAdmin(ModelView, model=User):
             count_query = select(func.count(User.id))
         ```
     """
 
     def __init__(self) -> None:
         self._mapper = inspect(self.model)
-        self._relations = get_relationships(self.model)
-        self._attrs = get_attributes(self.model)
+        self._relation_props = list(self._mapper.relationships)
+        self._relation_attrs = [
+            getattr(self.model, prop.key) for prop in self._relation_props
+        ]
+        self._column_props = list(self._mapper.columns)
+        self._props = self._mapper.attrs
 
         self._column_labels = self.get_column_labels()
         self._column_labels_value_by_key = {
             v: k for k, v in self._column_labels.items()
         }
 
-        self._list_attrs = self.get_list_columns()
+        self._list_props = self.get_list_columns()
         self._list_columns = [
-            (name, attr)
-            for (name, attr) in self._list_attrs
-            if isinstance(attr, ColumnProperty)
+            (name, prop)
+            for (name, prop) in self._list_props
+            if isinstance(prop, ColumnProperty)
         ]
-
-        self._details_attrs = self.get_details_columns()
-        self._details_columns = [
-            (name, attr)
-            for (name, attr) in self._details_attrs
-            if isinstance(attr, ColumnProperty)
+        self._list_relations = [
+            prop
+            for (_, prop) in self._list_props
+            if isinstance(prop, RelationshipProperty)
         ]
+        self._list_relation_attrs = [
+            getattr(self.model, prop.key) for prop in self._list_relations
+        ]
+
+        self._details_props = self.get_details_columns()
 
         column_formatters = getattr(self, "column_formatters", {})
         self._list_formatters = {
-            self.get_model_attr(attr): formatter
+            self._attr_to_prop(attr): formatter
             for (attr, formatter) in column_formatters.items()
         }
 
         column_formatters_detail = getattr(self, "column_formatters_detail", {})
         self._detail_formatters = {
-            self.get_model_attr(attr): formatter
+            self._attr_to_prop(attr): formatter
             for (attr, formatter) in column_formatters_detail.items()
         }
 
-        self._form_attrs = self.get_form_columns()
+        self._form_props = self.get_form_columns()
 
-        self._export_attrs = self.get_export_columns()
+        self._export_props = self.get_export_columns()
 
         self._search_fields = [
-            getattr(self.model, self.get_model_attr(attr).key)
+            getattr(self.model, attr) if isinstance(attr, str) else attr
             for attr in self.column_searchable_list
         ]
 
         self._sort_fields = [
-            getattr(self.model, self.get_model_attr(attr).key)
-            for attr in self.column_sortable_list
+            self._attr_to_prop(attr).key for attr in self.column_sortable_list
         ]
 
         self._form_ajax_refs = {}
         for name, options in self.form_ajax_refs.items():
             self._form_ajax_refs[name] = create_ajax_loader(
                 model_admin=self, name=name, options=options
             )
@@ -707,45 +730,45 @@
             async with self.sessionmaker(expire_on_commit=False) as session:
                 result = await session.execute(stmt)
                 return result.scalars().unique().all()
         else:
             return await anyio.to_thread.run_sync(self._run_query_sync, stmt)
 
     def _url_for_details(self, request: Request, obj: Any) -> str:
-        pk = getattr(obj, get_primary_key(obj).name)
+        pk = getattr(obj, self.pk_column.name)
         return request.url_for(
             "admin:details",
             identity=slugify_class_name(obj.__class__.__name__),
             pk=pk,
         )
 
     def _url_for_edit(self, request: Request, obj: Any) -> str:
-        pk = getattr(obj, get_primary_key(obj).name)
+        pk = getattr(obj, self.pk_column.name)
         return request.url_for(
             "admin:edit",
             identity=slugify_class_name(obj.__class__.__name__),
             pk=pk,
         )
 
     def _url_for_delete(self, request: Request, obj: Any) -> str:
-        pk = getattr(obj, get_primary_key(obj).name)
+        pk = getattr(obj, self.pk_column.name)
         query_params = urlencode({"pks": pk})
         url = request.url_for(
             "admin:delete", identity=slugify_class_name(obj.__class__.__name__)
         )
         return url + "?" + query_params
 
-    def _url_for_details_with_attr(
-        self, request: Request, obj: Any, attr: RelationshipProperty
+    def _url_for_details_with_prop(
+        self, request: Request, obj: Any, prop: RelationshipProperty
     ) -> str:
-        target = getattr(obj, attr.key)
+        target = getattr(obj, prop.key)
         if target is None:
             return ""
 
-        pk = getattr(target, attr.mapper.primary_key[0].name)
+        pk = getattr(target, prop.mapper.primary_key[0].name)
         return request.url_for(
             "admin:details",
             identity=slugify_class_name(target.__class__.__name__),
             pk=pk,
         )
 
     def _get_default_sort(self) -> List[Tuple[str, bool]]:
@@ -779,16 +802,16 @@
         sort: str = "asc",
     ) -> Pagination:
         page_size = min(page_size or self.page_size, max(self.page_size_options))
 
         count = await self.count()
         stmt = self.list_query.limit(page_size).offset((page - 1) * page_size)
 
-        for relation in self._relations:
-            stmt = stmt.options(joinedload(relation.key))
+        for relation in self._list_relation_attrs:
+            stmt = stmt.options(joinedload(relation))
 
         if sort_by:
             sort_fields = [(sort_by, sort == "desc")]
         else:
             sort_fields = self._get_default_sort()
 
         for sort_field, is_desc in sort_fields:
@@ -811,176 +834,168 @@
         return pagination
 
     async def get_model_objects(self, limit: Union[int, None] = 0) -> List[Any]:
         # For unlimited rows this should pass None
         limit = None if limit == 0 else limit
         stmt = self.list_query.limit(limit=limit)
 
-        for relation in self._relations:
-            stmt = stmt.options(joinedload(relation.key))
+        for relation in self._list_relation_attrs:
+            stmt = stmt.options(joinedload(relation))
 
         rows = await self._run_query(stmt)
         return rows
 
     async def get_model_by_pk(self, value: Any) -> Any:
         pk_value = get_column_python_type(self.pk_column)(value)
         stmt = select(self.model).where(self.pk_column == pk_value)
 
-        for relation in self._relations:
-            stmt = stmt.options(joinedload(relation.key))
+        for relation in self._relation_attrs:
+            stmt = stmt.options(joinedload(relation))
 
         rows = await self._run_query(stmt)
         if rows:
             return rows[0]
         return None
 
-    def get_attr_value(
-        self, obj: type, attr: Union[Column, ColumnProperty, RelationshipProperty]
+    def get_prop_value(
+        self, obj: type, prop: Union[Column, ColumnProperty, RelationshipProperty]
     ) -> Any:
         result = None
 
-        if isinstance(attr, Column):
-            result = getattr(obj, attr.name)
-
-        if isinstance(attr, (ColumnProperty, RelationshipProperty)):
-            result = getattr(obj, attr.key)
+        if isinstance(prop, Column):
+            result = getattr(obj, prop.name)
+        else:
+            result = getattr(obj, prop.key)
             result = result.value if isinstance(result, Enum) else result
 
         return result
 
-    def get_list_value(self, obj: type, attr: MODEL_ATTR_TYPE) -> Tuple[Any, Any]:
+    def get_list_value(self, obj: type, prop: MODEL_PROPERTY) -> Tuple[Any, Any]:
         """Get tuple of (value, formatted_value) for the list view."""
-        value = self.get_attr_value(obj, attr)
+        value = self.get_prop_value(obj, prop)
         formatted_value = self._default_formatter(value)
 
-        formatter = self._list_formatters.get(attr)
+        formatter = self._list_formatters.get(prop)
         if formatter:
-            formatted_value = formatter(obj, attr)
+            formatted_value = formatter(obj, prop)
         return value, formatted_value
 
-    def get_detail_value(self, obj: type, attr: MODEL_ATTR_TYPE) -> Tuple[Any, Any]:
+    def get_detail_value(self, obj: type, prop: MODEL_PROPERTY) -> Tuple[Any, Any]:
         """Get tuple of (value, formatted_value) for the detail view."""
-        value = self.get_attr_value(obj, attr)
+        value = self.get_prop_value(obj, prop)
         formatted_value = self._default_formatter(value)
 
-        formatter = self._detail_formatters.get(attr)
+        formatter = self._detail_formatters.get(prop)
         if formatter:
-            formatted_value = formatter(obj, attr)
+            formatted_value = formatter(obj, prop)
         return value, formatted_value
 
-    def get_model_attr(
-        self, attr: Union[str, InstrumentedAttribute]
-    ) -> MODEL_ATTR_TYPE:
-        assert isinstance(attr, (str, InstrumentedAttribute))
-        attrs = inspect(self.model).attrs
-
+    def _attr_to_prop(self, attr: Union[str, InstrumentedAttribute]) -> MODEL_PROPERTY:
         if isinstance(attr, str):
             key = attr
         else:
             key = attr.prop.key
 
-        if key in attrs:
-            return attrs[key]
+        if key in self._props:
+            return self._props[key]
 
         raise InvalidColumnError(
             f"Model '{self.model.__name__}' has no attribute '{key}'."
         )
 
     def _build_column_list(
         self,
-        default: List[MODEL_ATTR_TYPE],
+        defaults: List[MODEL_PROPERTY],
         include: Optional[Sequence[Union[str, InstrumentedAttribute]]] = None,
         exclude: Optional[Sequence[Union[str, InstrumentedAttribute]]] = None,
-    ) -> List[Tuple[str, MODEL_ATTR_TYPE]]:
+    ) -> List[Tuple[str, MODEL_PROPERTY]]:
         """This function generalizes constructing a list of columns
         for any sequence of inclusions or exclusions.
         """
         if include:
-            attrs = [self.get_model_attr(attr) for attr in include]
+            props = [self._attr_to_prop(prop) for prop in include]
         elif exclude:
-            exclude_columns = [self.get_model_attr(attr) for attr in exclude]
-            attrs = list(set(self._attrs) - set(exclude_columns))
+            exclude_props = {self._attr_to_prop(prop) for prop in exclude}
+            props = [prop for prop in self._props if prop not in exclude_props]
         else:
-            attrs = default
+            props = defaults
 
-        return [(self._column_labels.get(attr, attr.key), attr) for attr in attrs]
+        return [(self._column_labels.get(prop, prop.key), prop) for prop in props]
 
-    def get_list_columns(self) -> List[Tuple[str, MODEL_ATTR_TYPE]]:
-        """Get list of columns to display in List page."""
+    def get_list_columns(self) -> List[Tuple[str, MODEL_PROPERTY]]:
+        """Get list of properties to display in List page."""
 
         column_list = getattr(self, "column_list", None)
         column_exclude_list = getattr(self, "column_exclude_list", None)
 
         return self._build_column_list(
             include=column_list,
             exclude=column_exclude_list,
-            default=[getattr(self.model, self.pk_column.name).prop],
+            defaults=[self._props[self.pk_column.key]],
         )
 
-    def get_details_columns(self) -> List[Tuple[str, MODEL_ATTR_TYPE]]:
-        """Get list of columns to display in Detail page."""
+    def get_details_columns(self) -> List[Tuple[str, MODEL_PROPERTY]]:
+        """Get list of properties to display in Detail page."""
 
         column_details_list = getattr(self, "column_details_list", None)
         column_details_exclude_list = getattr(self, "column_details_exclude_list", None)
 
         return self._build_column_list(
             include=column_details_list,
             exclude=column_details_exclude_list,
-            default=self._attrs,
+            defaults=self._props,
         )
 
-    def get_form_columns(self) -> List[Tuple[str, MODEL_ATTR_TYPE]]:
-        """Get list of columns to display in the form."""
+    def get_form_columns(self) -> List[Tuple[str, MODEL_PROPERTY]]:
+        """Get list of properties to display in the form."""
 
         form_columns = getattr(self, "form_columns", None)
         form_excluded_columns = getattr(self, "form_excluded_columns", None)
 
-        columns = list(self._mapper.columns)
         default = []
-        for attr in self._attrs:
-            if attr in self._relations:
-                default.append(attr)
-            if attr in columns:
-                default.append(attr)
+        for prop in self._props:
+            if prop in self._relation_props or prop in self._column_props:
+                default.append(prop)
 
         return self._build_column_list(
             include=form_columns,
             exclude=form_excluded_columns,
-            default=self._attrs,
+            defaults=self._props,
         )
 
-    def get_export_columns(self) -> List[Tuple[str, MODEL_ATTR_TYPE]]:
-        """Get list of columns to export."""
+    def get_export_columns(self) -> List[Tuple[str, MODEL_PROPERTY]]:
+        """Get list of properties to export."""
 
         columns = getattr(self, "column_export_list", None)
         excluded_columns = getattr(self, "column_export_exclude_list", None)
 
         return self._build_column_list(
             include=columns,
             exclude=excluded_columns,
-            default=[item[1] for item in self._list_attrs],
+            defaults=[item[1] for item in self._list_props],
         )
 
     async def on_model_change(self, data: dict, model: Any, is_created: bool) -> None:
         """Perform some actions before a model is created or updated.
         By default does nothing.
         """
 
     async def after_model_change(
         self, data: dict, model: Any, is_created: bool
     ) -> None:
-        """Perform some actions after a model was created or updated and committed to the database.
+        """Perform some actions after a model was created
+        or updated and committed to the database.
         By default does nothing.
         """
 
     def get_column_labels(
         self,
-    ) -> Dict[MODEL_ATTR_TYPE, str]:
+    ) -> Dict[MODEL_PROPERTY, str]:
         return {
-            self.get_model_attr(column_label): value
+            self._attr_to_prop(column_label): value
             for column_label, value in self.column_labels.items()
         }
 
     async def delete_model(self, obj: Any) -> None:
         await Query(self).delete(obj)
 
     async def insert_model(self, data: dict) -> Any:
@@ -1001,22 +1016,23 @@
 
     async def scaffold_form(self) -> Type[Form]:
         if self.form is not None:
             return self.form
         return await get_model_form(
             model=self.model,
             engine=self.engine,
-            only=[i[1].key or i[1].name for i in self._form_attrs],
+            only=[i[1].key or i[1].name for i in self._form_props],
             column_labels={k.key: v for k, v in self._column_labels.items()},
             form_args=self.form_args,
             form_widget_args=self.form_widget_args,
             form_class=self.form_base_class,
             form_overrides=self.form_overrides,
             form_ajax_refs=self._form_ajax_refs,
             form_include_pk=self.form_include_pk,
+            form_converter=self.form_converter,
         )
 
     def search_placeholder(self) -> str:
         """Return search placeholder text.
 
         ???+ example
             ```python
@@ -1025,38 +1041,39 @@
                 column_searchable_list = [User.name, User.email]
 
             # placeholder is: "Name, Email"
             ```
         """
 
         search_fields = [
-            self.get_model_attr(attr) for attr in self.column_searchable_list
+            self._attr_to_prop(attr) for attr in self.column_searchable_list
         ]
         field_names = [
             self._column_labels.get(field, field.key) for field in search_fields
         ]
         return ", ".join(field_names)
 
     def search_query(self, stmt: Select, term: str) -> Select:
-        """Specify the search query given the SQLAlchemy statement and term to search for.
+        """Specify the search query given the SQLAlchemy statement
+        and term to search for.
         It can be used for doing more complex queries like JSON objects. For example:
 
         ```py
         return stmt.filter(MyModel.name == term)
         ```
         """
         expressions = [
-            cast(attr, String).ilike(f"%{term}%") for attr in self._search_fields
+            cast(prop, String).ilike(f"%{term}%") for prop in self._search_fields
         ]
         return stmt.filter(or_(*expressions))
 
     def get_export_name(self, export_type: str) -> str:
         """The file name when exporting."""
-        filename = f"{self.name}_{time.strftime('%Y-%m-%d_%H-%M-%S')}.{export_type}"
-        return filename
+
+        return f"{self.name}_{time.strftime('%Y-%m-%d_%H-%M-%S')}.{export_type}"
 
     def export_data(
         self,
         data: List[Any],
         export_type: str = "csv",
     ) -> StreamingResponse:
         if export_type == "csv":
@@ -1066,19 +1083,19 @@
 
     def _export_csv(
         self,
         data: List[Any],
     ) -> StreamingResponse:
         def generate(writer: Writer) -> Generator[Any, None, None]:
             # Append the column titles at the beginning
-            titles = [c[0] for c in self._export_attrs]
+            titles = [c[0] for c in self._export_props]
             yield writer.writerow(titles)
 
             for row in data:
-                vals = [str(self.get_attr_value(row, c[1])) for c in self._export_attrs]
+                vals = [str(self.get_prop_value(row, c[1])) for c in self._export_props]
                 yield writer.writerow(vals)
 
         # `get_export_name` can be subclassed.
         # So we want to keep the filename secure outside that method.
         filename = secure_filename(self.get_export_name(export_type="csv"))
 
         return StreamingResponse(
```

### Comparing `sqladmin-0.8.0/sqladmin/pagination.py` & `sqladmin-0.9.0/sqladmin/pagination.py`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/widgets.py` & `sqladmin-0.9.0/sqladmin/widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
-from typing import Any, Dict
+from typing import Any
 
 from markupsafe import Markup
 from wtforms import Field, widgets
 from wtforms.widgets import html_params
 
 __all__ = [
+    "AjaxSelect2Widget",
     "DatePickerWidget",
     "DateTimePickerWidget",
+    "Select2TagsWidget",
     "TimePickerWidget",
 ]
 
 
 class DatePickerWidget(widgets.TextInput):
     """
     Date picker widget.
@@ -64,7 +66,14 @@
             kwargs["multiple"] = "1"
         else:
             data = field.loader.format(field.data)
             if data:
                 kwargs["data-json"] = json.dumps([data])
 
         return Markup(f"<select {html_params(name=field.name, **kwargs)}></select>")
+
+
+class Select2TagsWidget(widgets.Select):
+    def __call__(self, field: Field, **kwargs: Any) -> str:
+        kwargs.setdefault("data-role", "select2-tags")
+        kwargs.setdefault("data-json", json.dumps(field.data))
+        return super().__call__(field, **kwargs)
```

### Comparing `sqladmin-0.8.0/sqladmin/statics/css/flatpickr.min.css` & `sqladmin-0.9.0/sqladmin/statics/css/flatpickr.min.css`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/css/fontawesome.min.css` & `sqladmin-0.9.0/sqladmin/statics/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/css/select2.min.css` & `sqladmin-0.9.0/sqladmin/statics/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/css/solid.min.css` & `sqladmin-0.9.0/sqladmin/statics/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/css/tabler.min.css` & `sqladmin-0.9.0/sqladmin/statics/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/bootstrap.min.js` & `sqladmin-0.9.0/sqladmin/statics/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/flatpickr.min.js` & `sqladmin-0.9.0/sqladmin/statics/js/flatpickr.min.js`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/jquery.min.js` & `sqladmin-0.9.0/sqladmin/statics/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/main.js` & `sqladmin-0.9.0/sqladmin/statics/js/main.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -128,8 +128,22 @@
         success: function(result) {
             window.location.href = result;
         },
         error: function(request, status, error) {
             alert(request.responseText);
         }
     });
+});
+
+// Select2 Tags
+$(':input[data-role="select2-tags"]').each(function() {
+    $(this).select2({
+        tags: true,
+        multiple: true,
+    });
+
+    existing_data = $(this).data("json") || [];
+    for (var i = 0; i < existing_data.length; i++) {
+        var option = new Option(existing_data[i], existing_data[i], true, true);
+        $(this).append(option).trigger('change');
+    }
 });
```

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/popper.min.js` & `sqladmin-0.9.0/sqladmin/statics/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/select2.full.min.js` & `sqladmin-0.9.0/sqladmin/statics/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/js/tabler.min.js` & `sqladmin-0.9.0/sqladmin/statics/js/tabler.min.js`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/webfonts/fa-solid-900.ttf` & `sqladmin-0.9.0/sqladmin/statics/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/statics/webfonts/fa-solid-900.woff2` & `sqladmin-0.9.0/sqladmin/statics/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/templates/base.html` & `sqladmin-0.9.0/sqladmin/templates/base.html`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/templates/create.html` & `sqladmin-0.9.0/sqladmin/templates/create.html`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/templates/details.html` & `sqladmin-0.9.0/sqladmin/templates/details.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 {% extends "layout.html" %}
 {% block content %}
 <div class="col-12">
   <div class="card">
     <div class="card-header">
-      <h3 class="card-title">{{ model_view.pk_column.name }}: {{ model_view.get_attr_value(model, model_view.pk_column) }}</h3>
+      <h3 class="card-title">{{ model_view.pk_column.name }}: {{ model_view.get_prop_value(model, model_view.pk_column) }}</h3>
     </div>
     <div class="card-body border-bottom py-3">
       <div class="table-responsive">
         <table class="table card-table table-vcenter text-nowrap table-hover table-bordered">
           <thead>
             <tr>
               <th class="w-1">Column</th>
               <th class="w-1">Value</th>
             </tr>
           </thead>
           <tbody>
-            {% for name, attr in model_view._details_attrs %}
+            {% for name, prop in model_view._details_props %}
             <tr>
               <td>{{ name }}</td>
-              {% set value, formatted_value = model_view.get_detail_value(model, attr) %}
-              {% if attr in model_view._relations %}
+              {% set value, formatted_value = model_view.get_detail_value(model, prop) %}
+              {% if prop in model_view._relation_props %}
               {% if is_list( value ) %}
               <td>
               {% for elem, formatted_elem in zip(value, formatted_value) %}
               <a href="{{ model_view._url_for_details(request, elem) }}">({{ formatted_elem }})</a>
               {% endfor %}
               </td>
               {% else %}
-              <td><a href="{{ model_view._url_for_details_with_attr(request, model, attr) }}">{{ formatted_value }}</a></td>
+              <td><a href="{{ model_view._url_for_details_with_prop(request, model, prop) }}">{{ formatted_value }}</a></td>
               {% endif %}
               {% else %}
               <td>{{ formatted_value }}</td>
               {% endif %}
             </tr>
             {% endfor %}
           </tbody>
@@ -42,15 +42,15 @@
           <div class="col-md-1">
             <a href="{{ url_for('admin:list', identity=model_view.identity) }}" class="btn">
               Go Back
             </a>
           </div>
           {% if model_view.can_delete %}
           <div class="col-md-1">
-            <a href="#" data-name="{{ model_view.name }}" data-pk="{{ model_view.get_attr_value(model, model_view.pk_column) }}" data-url="{{ model_view._url_for_delete(request, model) }}" data-bs-toggle="modal" data-bs-target="#modal-delete" class="btn btn-danger">
+            <a href="#" data-name="{{ model_view.name }}" data-pk="{{ model_view.get_prop_value(model, model_view.pk_column) }}" data-url="{{ model_view._url_for_delete(request, model) }}" data-bs-toggle="modal" data-bs-target="#modal-delete" class="btn btn-danger">
               Delete
             </a>
           </div>
           {% endif %}
           {% if model_view.can_edit %}
           <div class="col-md-1">
             <a href="{{ model_view._url_for_edit(request, model) }}" class="btn btn-primary">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% extends "layout.html" %} {% block content %}
-**** {{ model_view.pk_column.name }}: {{ model_view.get_attr_value(model,
+**** {{ model_view.pk_column.name }}: {{ model_view.get_prop_value(model,
 model_view.pk_column) }} ****
 Column     Value
            {% for elem,
            formatted_elem in zip
 {{ name }} (value, formatted_value) {{_formatted_value_}} {{ formatted_value }}
            %} ({{_formatted_elem
            }}) {% endfor %}
```

### Comparing `sqladmin-0.8.0/sqladmin/templates/edit.html` & `sqladmin-0.9.0/sqladmin/templates/edit.html`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/templates/layout.html` & `sqladmin-0.9.0/sqladmin/templates/layout.html`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/templates/list.html` & `sqladmin-0.9.0/sqladmin/templates/list.html`

 * *Files 5% similar despite different names*

```diff
@@ -59,66 +59,66 @@
     </div>
     <div class="table-responsive">
       <table class="table card-table table-vcenter text-nowrap">
         <thead>
           <tr>
             <th class="w-1"><input class="form-check-input m-0 align-middle" type="checkbox" aria-label="Select all" id="select-all"></th>
             <th class="w-1"></th>
-            {% for name, attr in model_view._list_attrs %}
+            {% for name, prop in model_view._list_props %}
             <th>
-              {% if attr in model_view._sort_fields %}
-              {% if request.query_params.get("sortBy") == attr.key and request.query_params.get("sort") == "asc" %}
+              {% if prop.key in model_view._sort_fields %}
+              {% if request.query_params.get("sortBy") == prop.key and request.query_params.get("sort") == "asc" %}
               <a href="{{ request.url.include_query_params(sort='desc') }}"><i class="fa-solid fa-arrow-down"></i> {{ name }}</a>
-              {% elif request.query_params.get("sortBy") == attr.key and request.query_params.get("sort") == "desc" %}
+              {% elif request.query_params.get("sortBy") == prop.key and request.query_params.get("sort") == "desc" %}
               <a href="{{ request.url.include_query_params(sort='asc') }}"><i class="fa-solid fa-arrow-up"></i> {{ name }}</a>
               {% else %}
-              <a href="{{ request.url.include_query_params(sortBy=attr.key, sort='asc') }}">{{ name }}</a>
+              <a href="{{ request.url.include_query_params(sortBy=prop.key, sort='asc') }}">{{ name }}</a>
               {% endif %}
               {% else %}
               {{ name }}
               {% endif %}
             </th>
             {% endfor %}
           </tr>
         </thead>
         <tbody>
           {% for row in pagination.rows %}
           <tr>
             <td>
-              <input type="hidden" value="{{ model_view.get_attr_value(row, model_view.pk_column) }}">
+              <input type="hidden" value="{{ model_view.get_prop_value(row, model_view.pk_column) }}">
               <input class="form-check-input m-0 align-middle select-box" type="checkbox" aria-label="Select item">
             </td>
             <td class="text-end">
               {% if model_view.can_view_details %}
               <a href="{{ model_view._url_for_details(request, row) }}" data-bs-toggle="tooltip" data-bs-placement="top" title="View">
                 <span class="me-1"><i class="fa-solid fa-eye"></i></span>
               </a>
               {% endif %}
               {% if model_view.can_edit %}
               <a href="{{ model_view._url_for_edit(request, row) }}" data-bs-toggle="tooltip" data-bs-placement="top" title="Edit">
                 <span class="me-1"><i class="fa-solid fa-pen-to-square"></i></span>
               </a>
               {% endif %}
               {% if model_view.can_delete %}
-              <a href="#" data-name="{{ model_view.name }}" data-pk="{{ model_view.get_attr_value(row, model_view.pk_column) }}" data-url="{{ model_view._url_for_delete(request, row) }}" data-bs-toggle="modal" data-bs-target="#modal-delete" title="Delete">
+              <a href="#" data-name="{{ model_view.name }}" data-pk="{{ model_view.get_prop_value(row, model_view.pk_column) }}" data-url="{{ model_view._url_for_delete(request, row) }}" data-bs-toggle="modal" data-bs-target="#modal-delete" title="Delete">
                 <span class="me-1"><i class="fa-solid fa-trash"></i></span>
               </a>
               {% endif %}
             </td>
-            {% for name, column in model_view._list_attrs %}
+            {% for name, column in model_view._list_props %}
             {% set value, formatted_value = model_view.get_list_value(row, column) %}
-            {% if column in model_view._relations %}
+            {% if column in model_view._relation_props %}
             {% if is_list( value ) %}
             <td>
             {% for elem, formatted_elem in zip(value, formatted_value) %}
             <a href="{{ model_view._url_for_details(request, elem) }}">({{ formatted_elem }})</a>
             {% endfor %}
             </td>
             {% else %}
-            <td><a href="{{ model_view._url_for_details_with_attr(request, row, column) }}">{{ formatted_value }}</a></td>
+            <td><a href="{{ model_view._url_for_details_with_prop(request, row, column) }}">{{ formatted_value }}</a></td>
             {% endif %}
             {% else %}
             <td>{{ formatted_value }}</td>
             {% endif %}
             {% endfor %}
           </tr>
           {% endfor %}
```

#### html2text {}

```diff
@@ -16,26 +16,26 @@
 model_view.can_delete %}
 Delete_selected_items
 {% endif %}
 {% if model_view.column_searchable_list %}
 [{{ request.query_params.get('search', '') }}] Search
 % if not request.query_params.get('search') %}disabled{% endif %}>
 {% endif %}
-                               {% if attr in
+                               {% if prop.key in
                                model_view._sort_fields
                                %} {% if
                                request.query_params.get
-                               ("sortBy") == attr.key
+                               ("sortBy") == prop.key
                                and
                                request.query_params.get
                                ("sort") == "asc" %}
                                 {{_name_}}
 ⁰                             {% elif
                                request.query_params.get
-                               ("sortBy") == attr.key
+                               ("sortBy") == prop.key
                                and
                                request.query_params.get
                                ("sort") == "desc" %}
                                 {{_name_}}
                                 {% else %} {{_name_}}
                                {% endif %} {% else %} {
                                { name }} {% endif %}
```

### Comparing `sqladmin-0.8.0/sqladmin/templates/login.html` & `sqladmin-0.9.0/sqladmin/templates/login.html`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/sqladmin/templates/modals/delete.html` & `sqladmin-0.9.0/sqladmin/templates/modals/delete.html`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/LICENSE.md` & `sqladmin-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqladmin-0.8.0/README.md` & `sqladmin-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,19 @@
 
 ```shell
 $ pip install sqladmin
 ```
 
 ---
 
+## Screenshots
+
+<img width="1492" alt="sqladmin-1" src="https://user-images.githubusercontent.com/19784933/208232730-0114a155-2740-4e89-9d73-64a4e51a5cf5.png">
+<img width="1492" alt="sqladmin-2" src="https://user-images.githubusercontent.com/19784933/208232731-6d783dde-b93e-41c0-911b-3d1c3c73f1d5.png">
+
 ## Quickstart
 
 Let's define an example SQLAlchemy model:
 
 ```python
 from sqlalchemy import Column, Integer, String, create_engine
 from sqlalchemy.ext.declarative import declarative_base
```

### Comparing `sqladmin-0.8.0/pyproject.toml` & `sqladmin-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requires-python = ">=3.7"
 license = "BSD-3-Clause"
 keywords = ["sqlalchemy", "fastapi", "starlette", "admin"]
 authors = [
   { name = "Amin Alaee", email = "mohammadamin.alaee@gmail.com" },
 ]
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Environment :: Web Environment",
@@ -25,15 +25,15 @@
   "License :: OSI Approved :: BSD License",
   "Topic :: Internet :: WWW/HTTP",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "starlette[full]",
   "typing_extensions>=4.0;python_version < '3.8'",
-  "sqlalchemy >=1.4, <1.5",
+  "sqlalchemy >=1.4",
   "wtforms >=3, <4",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://aminalaee.dev/sqladmin"
 Issues = "https://github.com/aminalaee/sqladmin/issues"
@@ -49,46 +49,84 @@
 ]
 
 [tool.hatch.build]
 exclude = [
   "tests/*",
 ]
 
-[tool.hatch.envs.default]
+[tool.hatch.envs.test]
 dependencies = [
   "aiosqlite==0.17.0",
+  "arrow==1.2.3",
   "asyncpg==0.27.0",
-  "autoflake==1.7.7",
   "babel==2.10.3",
-  "black==22.10.0",
   "build==0.9.0",
+  "colour==0.1.5",
   "coverage==6.5.0",
   "email-validator==1.3.0",
   "greenlet==2.0.0",
   "httpx==0.23.0",
-  "isort==5.10.1",
   "itsdangerous==2.1.2",
+  "phonenumbers==8.13.5",
+  "psycopg2-binary==2.9.5",
+  "pytest==7.2.0",
+  "python-dateutil==2.8.2",
+  "sqlalchemy_utils==0.38.3", 
+]
+
+[tool.hatch.envs.lint]
+dependencies = [
+  "black==22.10.0",
+  "isort==5.10.1",
+  "mypy==0.982",
+  "ruff==0.0.237",
+  "sqlalchemy~=1.4", # MyPy issues with SQLAlchemy V2
+]
+
+[tool.hatch.envs.docs]
+dependencies = [
   "mkdocs-material==8.5.7",
   "mkdocs==1.4.1",
   "mkdocstrings==0.18.1",
-  "mypy==0.982",
-  "psycopg2==2.9.5",
-  "pytest==7.2.0",
-  "sqlalchemy_utils==0.38.3",
-  "sqlmodel==0.0.8",
 ]
-[tool.hatch.envs.default.scripts]
-check = "isort --check --project=sqladmin . && black --check . && mypy sqladmin"
-clean = "rm -r dist site"
-cov = "coverage report --show-missing --skip-covered --fail-under=99 && coverage xml"
-docs = "mkdocs serve"
-docs_build = "mkdocs build"
-docs_deploy = "mkdocs gh-deploy --force"
-lint = "autoflake --in-place --recursive .s && isort --project=sqladmin . && black ."
-test = "python -m coverage run --concurrency=thread,greenlet -m pytest"
+
+[tool.hatch.envs.test.scripts]
+cov = [
+  "coverage report --show-missing --skip-covered --fail-under=99",
+  "coverage xml",
+]
+test = "coverage run -a --concurrency=thread,greenlet -m pytest"
+
+[tool.hatch.envs.lint.scripts]
+check = [
+  "ruff .",
+  "isort --check --project=sqladmin .",
+  "black --check .",
+  "mypy sqladmin",
+]
+format = [
+  "isort --project=sqladmin .",
+  "black .",
+  "ruff --fix .",
+]
+
+[tool.hatch.envs.docs.scripts]
+build = "mkdocs build"
+serve = "mkdocs serve --dev-addr localhost:8080"
+deploy = "mkdocs gh-deploy --force"
+
+[[tool.hatch.envs.test.matrix]]
+sqlalchemy = ["1.4", "2.0"]
+
+[tool.hatch.envs.test.overrides]
+matrix.sqlalchemy.dependencies = [
+  { value = "sqlalchemy~=1.4", if = ["1.4"] },
+  { value = "sqlmodel==0.0.8", if = ["1.4"] },
+  { value = "sqlalchemy~=2.0", if = ["2.0"] },
+]
 
 [tool.mypy]
 disallow_untyped_defs = true
 ignore_missing_imports = true
 show_error_codes = true
 no_implicit_optional = true
```

### Comparing `sqladmin-0.8.0/PKG-INFO` & `sqladmin-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: sqladmin
-Version: 0.8.0
+Version: 0.9.0
 Summary: SQLAlchemy admin for FastAPI and Starlette
 Project-URL: Documentation, https://aminalaee.dev/sqladmin
 Project-URL: Issues, https://github.com/aminalaee/sqladmin/issues
 Project-URL: Source, https://github.com/aminalaee/sqladmin
 Author-email: Amin Alaee <mohammadamin.alaee@gmail.com>
+License-Expression: BSD-3-Clause
 License-File: LICENSE.md
 Keywords: admin,fastapi,sqlalchemy,starlette
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
-Requires-Dist: sqlalchemy<1.5,>=1.4
+Requires-Dist: sqlalchemy>=1.4
 Requires-Dist: starlette[full]
 Requires-Dist: typing-extensions>=4.0; python_version < '3.8'
 Requires-Dist: wtforms<4,>=3
 Description-Content-Type: text/markdown
 
 <p align="center">
 <a href="https://github.com/aminalaee/sqladmin">
@@ -79,14 +80,19 @@
 
 ```shell
 $ pip install sqladmin
 ```
 
 ---
 
+## Screenshots
+
+<img width="1492" alt="sqladmin-1" src="https://user-images.githubusercontent.com/19784933/208232730-0114a155-2740-4e89-9d73-64a4e51a5cf5.png">
+<img width="1492" alt="sqladmin-2" src="https://user-images.githubusercontent.com/19784933/208232731-6d783dde-b93e-41c0-911b-3d1c3c73f1d5.png">
+
 ## Quickstart
 
 Let's define an example SQLAlchemy model:
 
 ```python
 from sqlalchemy import Column, Integer, String, create_engine
 from sqlalchemy.ext.declarative import declarative_base
```

