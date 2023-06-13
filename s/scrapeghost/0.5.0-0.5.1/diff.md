# Comparing `tmp/scrapeghost-0.5.0.tar.gz` & `tmp/scrapeghost-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapeghost-0.5.0.tar", max compression
+gzip compressed data, was "scrapeghost-0.5.1.tar", max compression
```

## Comparing `scrapeghost-0.5.0.tar` & `scrapeghost-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    18032 2023-03-20 02:41:03.735166 scrapeghost-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     2397 2023-03-24 23:43:59.976785 scrapeghost-0.5.0/README.md
--rw-r--r--   0        0        0      779 2023-06-06 22:39:24.524883 scrapeghost-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      157 2023-06-06 08:14:17.157308 scrapeghost-0.5.0/src/scrapeghost/__init__.py
--rw-r--r--   0        0        0     7430 2023-03-26 17:59:21.157961 scrapeghost-0.5.0/src/scrapeghost/apicall.py
--rw-r--r--   0        0        0     1464 2023-06-06 08:14:17.157856 scrapeghost-0.5.0/src/scrapeghost/cli.py
--rw-r--r--   0        0        0      348 2023-03-22 20:30:45.431201 scrapeghost-0.5.0/src/scrapeghost/errors.py
--rw-r--r--   0        0        0     4603 2023-06-06 08:19:17.686537 scrapeghost-0.5.0/src/scrapeghost/postprocessors.py
--rw-r--r--   0        0        0     1355 2023-03-24 23:01:32.548716 scrapeghost-0.5.0/src/scrapeghost/preprocessors.py
--rw-r--r--   0        0        0        0 2023-03-22 07:13:24.569881 scrapeghost-0.5.0/src/scrapeghost/py.typed
--rw-r--r--   0        0        0      460 2023-03-23 06:09:37.973075 scrapeghost-0.5.0/src/scrapeghost/responses.py
--rw-r--r--   0        0        0     9934 2023-06-06 22:37:38.898310 scrapeghost-0.5.0/src/scrapeghost/scrapers.py
--rw-r--r--   0        0        0     1133 2023-03-23 05:45:31.985498 scrapeghost-0.5.0/src/scrapeghost/utils.py
--rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 scrapeghost-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    18032 2023-03-20 02:41:03.735166 scrapeghost-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     2397 2023-03-24 23:43:59.976785 scrapeghost-0.5.1/README.md
+-rw-r--r--   0        0        0      779 2023-06-13 22:50:45.686789 scrapeghost-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-06-06 08:14:17.157308 scrapeghost-0.5.1/src/scrapeghost/__init__.py
+-rw-r--r--   0        0        0     7884 2023-06-13 21:46:33.038712 scrapeghost-0.5.1/src/scrapeghost/apicall.py
+-rw-r--r--   0        0        0     1464 2023-06-06 08:14:17.157856 scrapeghost-0.5.1/src/scrapeghost/cli.py
+-rw-r--r--   0        0        0      348 2023-03-22 20:30:45.431201 scrapeghost-0.5.1/src/scrapeghost/errors.py
+-rw-r--r--   0        0        0      767 2023-06-13 21:03:17.994214 scrapeghost-0.5.1/src/scrapeghost/models.py
+-rw-r--r--   0        0        0     4723 2023-06-07 00:48:54.516883 scrapeghost-0.5.1/src/scrapeghost/postprocessors.py
+-rw-r--r--   0        0        0     1355 2023-03-24 23:01:32.548716 scrapeghost-0.5.1/src/scrapeghost/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-03-22 07:13:24.569881 scrapeghost-0.5.1/src/scrapeghost/py.typed
+-rw-r--r--   0        0        0      460 2023-03-23 06:09:37.973075 scrapeghost-0.5.1/src/scrapeghost/responses.py
+-rw-r--r--   0        0        0    10494 2023-06-07 00:48:54.518047 scrapeghost-0.5.1/src/scrapeghost/scrapers.py
+-rw-r--r--   0        0        0      818 2023-06-13 21:03:17.994513 scrapeghost-0.5.1/src/scrapeghost/utils.py
+-rw-r--r--   0        0        0     3216 1970-01-01 00:00:00.000000 scrapeghost-0.5.1/PKG-INFO
```

### Comparing `scrapeghost-0.5.0/LICENSE.md` & `scrapeghost-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.5.0/README.md` & `scrapeghost-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.5.0/pyproject.toml` & `scrapeghost-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapeghost"
-version = "0.5.0"
+version = "0.5.1"
 description = "An experimental library for scraping websites using GPT."
 authors = ["James Turk <dev@jamesturk.net>"]
 license = "Hippocratic License HL3-EXTR-FFD-LAW-MIL-SV"
 readme = "README.md"
 
 [tool.poetry.scripts]
 scrapeghost = 'scrapeghost.cli:main'
```

### Comparing `scrapeghost-0.5.0/src/scrapeghost/apicall.py` & `scrapeghost-0.5.1/src/scrapeghost/apicall.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,17 @@
     TooManyTokens,
     MaxCostExceeded,
     BadStop,
 )
 from .responses import Response
 from .utils import (
     logger,
-    _cost,
-    _max_tokens,
     _tokens,
 )
+from .models import _model_dict
 
 Postprocessor = Callable[[Response, "OpenAiCall"], Response]
 
 
 RETRY_ERRORS = (
     openai.error.RateLimitError,
     openai.error.Timeout,
@@ -97,15 +96,15 @@
             model=model,
             messages=messages,
             **self.model_params,
         )
         elapsed = time.time() - start_t
         p_tokens = completion.usage.prompt_tokens
         c_tokens = completion.usage.completion_tokens
-        cost = _cost(model, c_tokens, p_tokens)
+        cost = _model_dict[model].cost(c_tokens, p_tokens)
         logger.info(
             "API response",
             duration=elapsed,
             prompt_tokens=p_tokens,
             completion_tokens=c_tokens,
             finish_reason=completion.choices[0].finish_reason,
             cost=cost,
@@ -136,28 +135,36 @@
         Make an OpenAPI request, with retries and model upgrades.
 
         * html - the HTML to send to the API
         * response - the Response object to augment
         """
         attempts = 0
         model_index = 0
-        model = self.models[model_index]
 
         response = Response()
 
         if not html:
             raise ValueError("html parameter cannot be empty")
-        tokens = _tokens(model, html)
-        if tokens > _max_tokens(model):
-            raise TooManyTokens(
-                f"HTML is {tokens} tokens, max for {model} is {_max_tokens(model)}"
-            )
 
         while True:
             try:
+                # check this within retries, but before API call
+                # so that we don't waste an API call but can still
+                # upgrade models
+                model = self.models[model_index]
+                model_data = _model_dict[model]
+                # this call is redundant for now since all models have the same
+                # tokenizer, but it's here for future-proofing
+                tokens = _tokens(model, html)
+                if tokens > model_data.max_tokens:
+                    raise TooManyTokens(
+                        f"HTML is {tokens} tokens, max for {model} is "
+                        f"{model_data.max_tokens}"
+                    )
+
                 attempts += 1
                 logger.info(
                     "API request",
                     model=model,
                     html_tokens=tokens,
                 )
                 self._raw_api_request(
```

### Comparing `scrapeghost-0.5.0/src/scrapeghost/cli.py` & `scrapeghost-0.5.1/src/scrapeghost/cli.py`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.5.0/src/scrapeghost/postprocessors.py` & `scrapeghost-0.5.1/src/scrapeghost/postprocessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
                     # if still invalid, raise error
                     raise InvalidJSON(response.data)
             else:
                 raise InvalidJSON(response.data)
         return response
 
     def nudge_json(self, scraper: SchemaScraper, response: Response) -> Response:
+        if not isinstance(response.data, str):
+            raise PostprocessingError(f"Response data is not a string: {response.data}")
         return scraper._raw_api_request(
             scraper.models[0],
             [
                 {
                     "role": "system",
                     "content": (
                         "When you receive invalid JSON, "
@@ -55,15 +57,15 @@
                         f"{scraper.json_schema}"
                     ),
                 },
                 {"role": "system", "content": ("Only reply with JSON, nothing else. ")},
                 {"role": "user", "content": "{'bad': 'json', }"},
                 {"role": "assistant", "content": '{"bad": "json"}'},
                 # response.data is always a string here
-                {"role": "user", "content": response.data},  # type: ignore
+                {"role": "user", "content": response.data},
             ],
             response,
         )
 
 
 class PydanticPostprocessor:
     def __init__(self, model: type):
```

### Comparing `scrapeghost-0.5.0/src/scrapeghost/preprocessors.py` & `scrapeghost-0.5.1/src/scrapeghost/preprocessors.py`

 * *Files identical despite different names*

### Comparing `scrapeghost-0.5.0/src/scrapeghost/scrapers.py` & `scrapeghost-0.5.1/src/scrapeghost/scrapers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 import re
 import json
 import typing
 import requests
 import lxml.html
 
-from typing import Any, Sequence
+from typing import Any, Sequence, Type
+from pydantic import BaseModel
 from .errors import PreprocessorError
 from .responses import Response, ScrapeResponse
-from .apicall import OpenAiCall, Postprocessor
+from .apicall import OpenAiCall, Postprocessor, RetryRule
 from .utils import logger, _tokens, _tostr
 from .preprocessors import Preprocessor, CleanHTML
 from .postprocessors import (
     JSONPostprocessor,
     PydanticPostprocessor,
 )
 
 
 class SchemaScraper(OpenAiCall):
     _default_preprocessors: list[Preprocessor] = [
         CleanHTML(),
     ]
 
-    def __init__(  # type: ignore
+    def __init__(
         self,
         schema: dict | str | list,
         extra_preprocessors: list | None = None,
         *,
         auto_split_length: int = 0,
+        # inherited from OpenAiCall
+        models: list[str] = ["gpt-3.5-turbo", "gpt-4"],
+        model_params: dict | None = None,
+        max_cost: float = 1,
+        retry: RetryRule = RetryRule(1, 30),
         extra_instructions: list[str] | None = None,
-        postprocessors: list[Postprocessor] | None = None,
-        **kwargs,
+        postprocessors: list | None = None,
     ):
-        super().__init__(**kwargs)
+        # extra_instructions & postprocessors handled
+        # differently in SchemaScraper so not passed to super()
+        super().__init__(
+            models=models, model_params=model_params, max_cost=max_cost, retry=retry
+        )
         use_pydantic = False
         if isinstance(schema, (list, dict)):
             self.json_schema = json.dumps(schema)
         elif isinstance(schema, str):
             self.json_schema = schema
         elif hasattr(schema, "schema"):
             self.json_schema = _pydantic_to_simple_schema(schema)
@@ -73,15 +82,18 @@
 
         if extra_preprocessors is None:
             self.preprocessors = self._default_preprocessors
         else:
             self.preprocessors = self._default_preprocessors + extra_preprocessors
 
         if use_pydantic:
-            self.postprocessors.append(PydanticPostprocessor(schema))  # type: ignore
+            # check if schema is a pydantic model
+            if not isinstance(schema, type):
+                raise ValueError("Schema must be a Pydantic model.")
+            self.postprocessors.append(PydanticPostprocessor(schema))
 
         self.auto_split_length = auto_split_length
 
     def _apply_preprocessors(
         self, doc: lxml.html.Element, extra_preprocessors: list
     ) -> list:
         nodes = [doc]
@@ -214,25 +226,25 @@
         "chunked tags",
         num=len(chunks),
         sizes=chunk_sizes,
     )
     return chunks
 
 
-def _pydantic_to_simple_schema(pydantic_model: type) -> dict:
+def _pydantic_to_simple_schema(pydantic_model: Type[BaseModel]) -> dict:
     """
     Given a Pydantic model, return a simple schema that can be used
     by SchemaScraper.
 
     We don't use Pydantic's schema() method because the
     additional complexity of JSON Schema adds a lot of extra tokens
     and in testing did not work as well as the simplified versions.
     """
-    schema = {}
-    for field in pydantic_model.__fields__.values():  # type: ignore
+    schema: dict = {}
+    for field in pydantic_model.__fields__.values():
         # __fields__ is present on Pydantic models, so can process recursively
         if hasattr(field.outer_type_, "__fields__"):
             schema[field.name] = _pydantic_to_simple_schema(field.outer_type_)
         else:
             type_name = field.outer_type_.__name__
             if type_name == "list":
                 (inner,) = typing.get_args(field.outer_type_)
```

### Comparing `scrapeghost-0.5.0/PKG-INFO` & `scrapeghost-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapeghost
-Version: 0.5.0
+Version: 0.5.1
 Summary: An experimental library for scraping websites using GPT.
 License: Hippocratic License HL3-EXTR-FFD-LAW-MIL-SV
 Author: James Turk
 Author-email: dev@jamesturk.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

