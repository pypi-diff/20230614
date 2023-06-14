# Comparing `tmp/async_eval-0.1.9.tar.gz` & `tmp/async_eval-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_eval-0.1.9.tar", max compression
+gzip compressed data, was "async_eval-0.2.0.tar", max compression
```

## Comparing `async_eval-0.1.9.tar` & `async_eval-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2022-08-09 07:18:07.203012 async_eval-0.1.9/LICENSE
--rw-r--r--   0        0        0      125 2022-08-09 07:18:07.203012 async_eval-0.1.9/README.md
--rw-r--r--   0        0        0      175 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/__init__.py
--rw-r--r--   0        0        0     5333 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/async_eval.py
--rw-r--r--   0        0        0     3213 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/asyncio_patch.py
--rw-r--r--   0        0        0        0 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/ext/__init__.py
--rw-r--r--   0        0        0       82 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/ext/pydevd/__init__.py
--rw-r--r--   0        0        0     3153 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/ext/pydevd/code.py
--rw-r--r--   0        0        0      361 2022-08-09 07:18:07.203012 async_eval-0.1.9/async_eval/ext/pydevd/integration.py
--rw-r--r--   0        0        0     1092 2022-08-09 07:18:07.207012 async_eval-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1062 2022-08-09 07:18:21.094079 async_eval-0.1.9/setup.py
--rw-r--r--   0        0        0     1055 2022-08-09 07:18:21.094487 async_eval-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-14 07:47:35.670800 async_eval-0.2.0/LICENSE
+-rw-r--r--   0        0        0      125 2023-06-14 07:47:35.670800 async_eval-0.2.0/README.md
+-rw-r--r--   0        0        0      126 2023-06-14 07:47:35.670800 async_eval-0.2.0/async_eval/__init__.py
+-rw-r--r--   0        0        0     6214 2023-06-14 07:47:35.674800 async_eval-0.2.0/async_eval/async_eval.py
+-rw-r--r--   0        0        0     1349 2023-06-14 07:47:35.674800 async_eval-0.2.0/async_eval/asyncio_patch.py
+-rw-r--r--   0        0        0        0 2023-06-14 07:47:35.674800 async_eval-0.2.0/async_eval/ext/__init__.py
+-rw-r--r--   0        0        0       82 2023-06-14 07:47:35.674800 async_eval-0.2.0/async_eval/ext/pydevd/__init__.py
+-rw-r--r--   0        0        0     3169 2023-06-14 07:47:35.674800 async_eval-0.2.0/async_eval/ext/pydevd/code.py
+-rw-r--r--   0        0        0      314 2023-06-14 07:47:35.674800 async_eval-0.2.0/async_eval/ext/pydevd/integration.py
+-rw-r--r--   0        0        0     2520 2023-06-14 07:47:35.674800 async_eval-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 async_eval-0.2.0/PKG-INFO
```

### Comparing `async_eval-0.1.9/LICENSE` & `async_eval-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `async_eval-0.1.9/async_eval/async_eval.py` & `async_eval-0.2.0/async_eval/async_eval.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,84 @@
 import ast
 import inspect
 import sys
 import textwrap
 import types
-from typing import Any, Optional, Union, cast
+from asyncio.tasks import _enter_task, _leave_task, current_task
+from contextvars import Context
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+    no_type_check,
+)
 
 try:
     from _pydevd_bundle.pydevd_save_locals import save_locals
 except ImportError:  # pragma: no cover
-
     import ctypes
 
     def save_locals(frame: types.FrameType) -> None:
         ctypes.pythonapi.PyFrame_LocalsToFast(ctypes.py_object(frame), ctypes.c_int(1))
 
 
 def _noop(*_: Any, **__: Any) -> Any:  # pragma: no cover
     return None
 
 
+_: Any
+
 try:
-    _ = verify_async_debug_available  # noqa
+    _ = verify_async_debug_available  # type: ignore # noqa
 except NameError:  # pragma: no cover
     try:
         from async_eval.asyncio_patch import verify_async_debug_available
     except ImportError:
         verify_async_debug_available = _noop
 
 try:
-    _ = apply  # noqa
+    _ = get_current_loop  # type: ignore # noqa
 except NameError:  # pragma: no cover
     try:
-        from nest_asyncio import apply
+        from async_eval.asyncio_patch import get_current_loop
     except ImportError:
-        apply = _noop
+        get_current_loop = _noop
 
 
 _ASYNC_EVAL_CODE_TEMPLATE = textwrap.dedent(
     """\
-__locals__ = locals()
-
-async def __async_exec_func__():
-    global __locals__
-    locals().update(__locals__)
-    try:
-        pass
-    finally:
-        __locals__.update(locals())
-
-__ctx__ = None
-
-try:
-    async def __async_exec_func__(
-        __async_exec_func__=__async_exec_func__,
-        contextvars=__import__('contextvars'),
-    ):
+async def __async_func__(_locals):
+    async def __func_wrapper__(_locals):
+        locals().update(_locals)
         try:
-            return await __async_exec_func__()
+            pass
         finally:
-            global __ctx__
-            __ctx__ = contextvars.copy_context()
+            _locals.update(locals())
+            _locals.pop("_locals", None)
 
-except ImportError:
-    pass
+    from contextvars import copy_context
 
-try:
-    __async_exec_func_result__ = __import__('asyncio').run(__async_exec_func__())
-finally:
-    if __ctx__ is not None:
-        for var in __ctx__:
-            var.set(__ctx__[var])
-
-        try:
-            del var
-        except NameError:
-            pass
+    try:
+       r = await __func_wrapper__(_locals)
+       is_exc = False
+    except Exception as e:
+        r, is_exc = e, True
 
-    del __ctx__
-    del __locals__
-    del __async_exec_func__
-"""
+    return is_exc, r, copy_context()
+""",
 )
 
 
 def _compile_ast(node: ast.AST, filename: str = "<eval>", mode: str = "exec") -> types.CodeType:
-    return cast(types.CodeType, compile(node, filename, mode))
+    return cast(types.CodeType, compile(node, filename, mode))  # type: ignore
 
 
 ASTWithBody = Union[ast.Module, ast.With, ast.AsyncWith]
 
 
 def _make_stmt_as_return(parent: ASTWithBody, root: ast.AST, filename: str) -> types.CodeType:
     node = parent.body[-1]
@@ -103,26 +93,39 @@
         return _compile_ast(root, filename)
 
 
 def _transform_to_async(code: str, filename: str) -> types.CodeType:
     base = ast.parse(_ASYNC_EVAL_CODE_TEMPLATE)
     module = ast.parse(code)
 
-    func: ast.AsyncFunctionDef = cast(ast.AsyncFunctionDef, base.body[1])
+    func: ast.AsyncFunctionDef = cast(ast.AsyncFunctionDef, cast(ast.AsyncFunctionDef, base.body[0]).body[0])
     try_stmt: ast.Try = cast(ast.Try, func.body[-1])
 
     try_stmt.body = module.body
 
     parent: ASTWithBody = module
     while isinstance(parent.body[-1], (ast.AsyncWith, ast.With)):
         parent = cast(ASTWithBody, parent.body[-1])
 
     return _make_stmt_as_return(parent, base, filename)
 
 
+def _compile_async_func(
+    code: types.CodeType,
+    _locals: dict,
+    _globals: dict,
+) -> Callable[[dict], Awaitable[Tuple[bool, Any, Context]]]:
+    exec(code, _globals, _locals)
+
+    return cast(
+        Callable[[dict], Awaitable[Tuple[bool, Any, Context]]],
+        _locals.pop("__async_func__"),
+    )
+
+
 class _AsyncNodeFound(Exception):
     pass
 
 
 class _AsyncCodeVisitor(ast.NodeVisitor):
     @classmethod
     def check(cls, code: str) -> bool:
@@ -172,38 +175,76 @@
     visit_DictComp = _visit_gen
 
 
 def is_async_code(code: str) -> bool:
     return _AsyncCodeVisitor.check(code)
 
 
+T = TypeVar("T")
+
+
+@no_type_check
+def _run_coro(coro: Awaitable[T]) -> T:
+    loop = get_current_loop()
+
+    if not loop.is_running():
+        return loop.run_until_complete(coro)
+
+    current = current_task(loop)
+
+    t = loop.create_task(coro)
+
+    try:
+        if current is not None:
+            _leave_task(loop, current)
+
+        while not t.done():
+            loop._run_once()
+
+        return t.result()
+    finally:
+        if current is not None:
+            _enter_task(loop, current)
+
+
+def _reflect_context(ctx: Context) -> None:
+    for v in ctx:
+        v.set(ctx[v])
+
+
 # async equivalent of builtin eval function
 def async_eval(
     code: str,
     _globals: Optional[dict] = None,
     _locals: Optional[dict] = None,
     *,
     filename: str = "<eval>",
 ) -> Any:
     verify_async_debug_available()
-    apply()  # double check that loop is patched
 
     caller: types.FrameType = inspect.currentframe().f_back  # type: ignore
 
     if _locals is None:
         _locals = caller.f_locals
 
     if _globals is None:
         _globals = caller.f_globals
 
     code_obj = _transform_to_async(code, filename)
+    func = _compile_async_func(code_obj, _locals, _globals)
 
     try:
-        exec(code_obj, _globals, _locals)
-        return _locals.pop("__async_exec_func_result__")
+        is_exc, result, ctx = _run_coro(func(_locals))
+
+        _reflect_context(ctx)
+
+        if is_exc:
+            raise result
+
+        return result
     finally:
         save_locals(caller)
 
 
 sys.__async_eval__ = async_eval  # type: ignore
 
 __all__ = ["async_eval", "is_async_code"]
```

### Comparing `async_eval-0.1.9/async_eval/ext/pydevd/code.py` & `async_eval-0.2.0/async_eval/ext/pydevd/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def _noop(*_: Any, **__: Any) -> Any:  # pragma: no cover
     return False
 
 
 try:  # pragma: no cover
     # only for testing purposes
-    _ = is_async_code  # noqa
+    _ = is_async_code  # type: ignore  # noqa
     _ = verify_async_debug_available  # type: ignore  # noqa
 except NameError:  # pragma: no cover
     try:
         from async_eval.async_eval import is_async_code
         from async_eval.asyncio_patch import verify_async_debug_available
     except ImportError:
         is_async_code = _noop
```

### Comparing `async_eval-0.1.9/PKG-INFO` & `async_eval-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: async-eval
-Version: 0.1.9
+Version: 0.2.0
 Summary: eval async code from sync
 Home-page: https://github.com/uriyyo/async-eval
 License: MIT
 Author: Yurii Karabas
 Author-email: 1998uriyyo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: pydevd-pycharm
 Provides-Extra: trio
-Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
-Requires-Dist: pydevd-pycharm (>=222.3739.30,<223.0.0); extra == "pydevd-pycharm" or extra == "all"
-Requires-Dist: trio (>=0.21.0,<0.22.0); extra == "trio" or extra == "all"
+Requires-Dist: pydevd-pycharm (<232.7295.9) ; extra == "pydevd-pycharm" or extra == "all"
+Requires-Dist: trio (>=0.21,<0.23) ; extra == "trio" or extra == "all"
 Project-URL: Repository, https://github.com/uriyyo/async-eval
 Description-Content-Type: text/markdown
 
 # async-eval
 
 ```python
 from async_eval import eval
```

