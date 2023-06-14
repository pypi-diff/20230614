# Comparing `tmp/ftmq-0.1.0.tar.gz` & `tmp/ftmq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.1.0.tar", max compression
+gzip compressed data, was "ftmq-0.1.2.tar", max compression
```

## Comparing `ftmq-0.1.0.tar` & `ftmq-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.0/LICENSE
--rw-r--r--   0        0        0     4039 2023-06-14 16:58:41.577739 ftmq-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-02-13 11:00:34.058881 ftmq-0.1.0/ftmq/__init__.py
--rw-r--r--   0        0        0     1058 2023-06-14 15:35:29.068036 ftmq-0.1.0/ftmq/cli.py
--rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.0/ftmq/exceptions.py
--rw-r--r--   0        0        0     5131 2023-06-14 16:58:42.021732 ftmq-0.1.0/ftmq/filters.py
--rw-r--r--   0        0        0     1581 2023-06-14 16:14:34.537028 ftmq-0.1.0/ftmq/io.py
--rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.0/ftmq/query.py
--rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.0/ftmq/types.py
--rw-r--r--   0        0        0      229 2023-06-14 15:37:13.378112 ftmq-0.1.0/ftmq/util.py
--rw-r--r--   0        0        0     1251 2023-06-14 17:04:16.198352 ftmq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 ftmq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4039 2023-06-14 16:58:41.577739 ftmq-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-14 18:57:52.786294 ftmq-0.1.2/ftmq/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-14 18:32:14.390982 ftmq-0.1.2/ftmq/cli.py
+-rw-r--r--   0        0        0       43 2023-02-17 15:30:40.666516 ftmq-0.1.2/ftmq/exceptions.py
+-rw-r--r--   0        0        0     5115 2023-06-14 18:50:42.961409 ftmq-0.1.2/ftmq/filters.py
+-rw-r--r--   0        0        0     1593 2023-06-14 18:17:13.454654 ftmq-0.1.2/ftmq/io.py
+-rw-r--r--   0        0        0     1784 2023-06-14 17:04:10.502390 ftmq-0.1.2/ftmq/query.py
+-rw-r--r--   0        0        0      383 2023-06-14 15:32:48.293679 ftmq-0.1.2/ftmq/types.py
+-rw-r--r--   0        0        0      523 2023-06-14 17:55:59.782847 ftmq-0.1.2/ftmq/util.py
+-rw-r--r--   0        0        0     1285 2023-06-14 18:57:52.786294 ftmq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5161 1970-01-01 00:00:00.000000 ftmq-0.1.2/PKG-INFO
```

### Comparing `ftmq-0.1.0/LICENSE` & `ftmq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.0/README.md` & `ftmq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.0/ftmq/cli.py` & `ftmq-0.1.2/ftmq/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from typing import Optional
 
 import typer
+from typing_extensions import Annotated
+
+from ftmq.io import smart_read_proxies, smart_write_proxies
 
 from .query import Query
-from .util import smart_read_proxies, smart_write_proxies
 
 cli = typer.Typer()
 
 
 @cli.command()
 def ftmq(
-    input_uri: str = typer.Option("-", "-i", help="input file or uri"),
-    output_uri: str = typer.Option("-", "-o", help="output file or uri"),
-    dataset: Optional[list[str]] = typer.Option(
-        None, "-d", "--dataset", help="Dataset(s)"
-    ),
-    schema: Optional[list[str]] = typer.Option(
-        None, "-s", "--schema", help="Schema(tas)"
-    ),
+    input_uri: Annotated[
+        Optional[str], typer.Option("-i", help="input file or uri")
+    ] = "-",
+    output_uri: Annotated[
+        Optional[str], typer.Option("-o", help="output file or uri")
+    ] = "-",
+    dataset: Annotated[
+        Optional[list[str]], typer.Option("-d", "--dataset", help="Dataset(s)")
+    ] = None,
+    schema: Annotated[
+        Optional[list[str]], typer.Option("-s", "--schema", help="Schema(tas)")
+    ] = None,
     schema_include_descendants: bool = False,
     schema_include_matchable: bool = False,
 ):
     """
     Apply ftmq to a json stream of ftm entities.
     """
     q = Query()
@@ -31,8 +37,8 @@
         q = q.where(
             schema=value,
             include_descendants=schema_include_descendants,
             include_matchable=schema_include_matchable,
         )
 
     proxies = q.apply_iter(smart_read_proxies(input_uri))
-    smart_write_proxies(proxies)
+    smart_write_proxies(output_uri, proxies, serialize=True)
```

### Comparing `ftmq-0.1.0/ftmq/filters.py` & `ftmq-0.1.2/ftmq/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from enum import StrEnum
 from typing import TypeVar
 
 from banal import as_bool, ensure_list
 from followthemoney import model
 from followthemoney.property import Property
 from followthemoney.schema import Schema
 from nomenklatura.dataset import Dataset
 from nomenklatura.entity import CE
 
 from .exceptions import ValidationError
 from .types import Value
-from .util import make_dataset
+from .util import StrEnum, make_dataset
 
 
 class BaseFilter:
     instance: Dataset | Schema | Property | None = None
     options: StrEnum = None
 
     def __init__(self, value: str | Dataset | Schema | Property | None):
```

### Comparing `ftmq-0.1.0/ftmq/io.py` & `ftmq-0.1.2/ftmq/io.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,13 +49,15 @@
 
 def smart_write_proxies(
     uri: PathLike,
     proxies: Iterable[CE | SDict],
     mode: str | None = "wb",
     serialize: bool | None = False,
 ) -> int:
+    ix = 0
     with smart_open(uri, sys.stdout.buffer, mode=mode) as fh:
-        for ix, proxy in enumerate(proxies):
+        for proxy in proxies:
+            ix += 1
             if serialize:
                 proxy = proxy.to_dict()
             fh.write(orjson.dumps(proxy, option=orjson.OPT_APPEND_NEWLINE))
-    return ix + 1
+    return ix
```

### Comparing `ftmq-0.1.0/ftmq/query.py` & `ftmq-0.1.2/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.1.0/pyproject.toml` & `ftmq-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.1.0"
+version = "0.1.2"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -14,15 +14,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 packages = [{include = "ftmq"}]
 
 [tool.poetry.scripts]
-investigraph = "ftmq.cli:cli"
+ftmq = "ftmq.cli:cli"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/investigativedata/ftmq/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -39,12 +39,14 @@
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pre-commit = "^3.3.3"
 flake8 = "^6.0.0"
 moto = "^4.1.11"
+ipdb = "^0.13.13"
+bump2version = "^1.0.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ftmq-0.1.0/PKG-INFO` & `ftmq-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.1.0
+Version: 0.1.2
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
```

