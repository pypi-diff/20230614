# Comparing `tmp/vcr_langchain-0.0.8.tar.gz` & `tmp/vcr_langchain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcr_langchain-0.0.8.tar", max compression
+gzip compressed data, was "vcr_langchain-0.0.9.tar", max compression
```

## Comparing `vcr_langchain-0.0.8.tar` & `vcr_langchain-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-01-22 02:22:05.908380 vcr_langchain-0.0.8/LICENSE
--rw-r--r--   0        0        0     2017 2023-02-01 04:12:27.618885 vcr_langchain-0.0.8/README.md
--rw-r--r--   0        0        0      659 2023-02-01 04:15:46.285988 vcr_langchain-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      133 2023-01-22 02:59:58.597927 vcr_langchain-0.0.8/vcr_langchain/__init__.py
--rw-r--r--   0        0        0     1118 2023-01-28 01:46:39.077191 vcr_langchain-0.0.8/vcr_langchain/cache.py
--rw-r--r--   0        0        0     2381 2023-01-28 01:55:14.355809 vcr_langchain-0.0.8/vcr_langchain/cassette.py
--rw-r--r--   0        0        0     1258 2023-01-28 01:55:14.355809 vcr_langchain-0.0.8/vcr_langchain/config.py
--rw-r--r--   0        0        0      575 2023-01-28 01:47:29.021132 vcr_langchain-0.0.8/vcr_langchain/matchers.py
--rw-r--r--   0        0        0     4905 2023-02-01 04:06:16.863869 vcr_langchain-0.0.8/vcr_langchain/patch.py
--rw-r--r--   0        0        0        0 2023-01-22 03:07:34.692815 vcr_langchain-0.0.8/vcr_langchain/py.typed
--rw-r--r--   0        0        0       82 2023-01-22 02:59:58.587927 vcr_langchain-0.0.8/vcr_langchain/record_mode.py
--rw-r--r--   0        0        0     1109 2023-01-28 01:55:48.366984 vcr_langchain-0.0.8/vcr_langchain/request.py
--rw-r--r--   0        0        0      154 2023-01-28 01:55:14.355809 vcr_langchain-0.0.8/vcr_langchain/stubs.py
--rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 vcr_langchain-0.0.8/setup.py
--rw-r--r--   0        0        0     2577 1970-01-01 00:00:00.000000 vcr_langchain-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-22 02:22:05.908380 vcr_langchain-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1774 2023-02-03 07:18:44.109509 vcr_langchain-0.0.9/README.md
+-rw-r--r--   0        0        0      798 2023-02-03 07:29:11.041016 vcr_langchain-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      806 2023-02-03 07:16:44.594129 vcr_langchain-0.0.9/vcr_langchain/__init__.py
+-rw-r--r--   0        0        0     5248 2023-02-03 07:16:44.594129 vcr_langchain-0.0.9/vcr_langchain/patch.py
+-rw-r--r--   0        0        0        0 2023-01-22 03:07:34.692815 vcr_langchain-0.0.9/vcr_langchain/py.typed
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 vcr_langchain-0.0.9/setup.py
+-rw-r--r--   0        0        0     2334 1970-01-01 00:00:00.000000 vcr_langchain-0.0.9/PKG-INFO
```

### Comparing `vcr_langchain-0.0.8/LICENSE` & `vcr_langchain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vcr_langchain-0.0.8/README.md` & `vcr_langchain-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # VCR LangChain
 
-Adapts [VCR.py](https://github.com/kevin1024/vcrpy) for use with [LangChain](https://github.com/hwchase17/langchain). Refactor with confidence as you record and replay all your LLM logic in a contained environment, free from any and all side effects.
+Patches [VCR.py](https://github.com/kevin1024/vcrpy) to include non-network tooling for use with [LangChain](https://github.com/hwchase17/langchain). Refactor with confidence as you record and replay all your LLM logic in a contained environment, free from any and all side effects.
 
 ## Quickstart
 
 ```bash
 pip install vcr-langchain
 ```
 
@@ -25,19 +25,14 @@
 - the output is now deterministic
 - it executes a lot faster by replaying from cache
 - no command executions or other side effects actually happen
 - you no longer need to have real API keys defined for test execution in CI environments
 
 For more examples, see [the usages test file](tests/test_usage.py).
 
-### Why not just use VCR.py directly?
-
-- This offers higher-level, more human-readable recordings for inspection
-- This supports recordings of langchain tool interactions as well, which includes non-network requests such as command executions inside Bash or the Python REPL
-
 ### Pitfalls
 
 Note that tools, if initialized outside of the `vcr_langchain` decorator, will not have recording capabilities patched in. This is true even if an agent using those tools is initialized within the decorator.
 
 ## Documentation
 
 For more information on how VCR works and what other options there are, please see the [VCR docs](https://vcrpy.readthedocs.io/en/latest/index.html).
```

### Comparing `vcr_langchain-0.0.8/pyproject.toml` & `vcr_langchain-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 [tool.poetry]
 name = "vcr-langchain"
-version = "0.0.8"
+version = "0.0.9"
 description = "Record and replay LLM interactions for langchain"
 authors = ["Amos Jun-yeung Ng <me@amos.ng>"]
 readme = "README.md"
 packages = [{include = "vcr_langchain"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 vcrpy = "^4.2.1"
-langchain = "^0.0.75"
+langchain = "^0.0.76"
 gorilla = "^0.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 mypy = "^0.991"
 black = "^22.12.0"
 isort = "^5.11.4"
 flake8 = "^6.0.0"
 google-search-results = "^2.4.1"
+openai = "^0.26.4"
+faiss-cpu = "^1.7.3"
 
 [tool.mypy]
 ignore_missing_imports = "True"
 disallow_untyped_defs = "True"
 
+[tool.pytest.ini_options]
+markers = [
+    "network: marks tests as requiring network services",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vcr_langchain-0.0.8/vcr_langchain/patch.py` & `vcr_langchain-0.0.9/vcr_langchain/patch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,46 @@
+import itertools
+import json
 import logging
-from typing import Any, Callable, List, Tuple, Type, Union
+from typing import Any, Callable, Iterable, List, Optional, Type, Union
 
 import gorilla
-import langchain
 from langchain.python import PythonREPL
-from langchain.serpapi import SerpAPIWrapper
 from langchain.utilities.bash import BashProcess
-from vcr.patch import CassettePatcherBuilder as OgCassettePatcherBuilder
-
-from .cache import VcrCache
-from .request import Request
-from .stubs import Cassette
+from vcr.cassette import Cassette
+from vcr.errors import CannotOverwriteExistingCassetteException
+from vcr.patch import CassettePatcherBuilder
+from vcr.request import Request
 
 log = logging.getLogger(__name__)
 
 
 LANGCHAIN_VISUALIZER_PATCH_ID = "lc-viz"
 VCR_LANGCHAIN_PATCH_ID = "lc-vcr"
 # override prefix to use if langchain-visualizer is there as well
 VCR_VIZ_INTEROP_PREFIX = "_vcr_"
 
 
-class CachePatch:
-    def __init__(self, cassette: Cassette):
-        self.cassette = cassette
+log = logging.getLogger(__name__)
 
-    def __enter__(self) -> None:
-        langchain.llm_cache = VcrCache(self.cassette)
 
-    def __exit__(self, *_: List[Any]) -> None:
-        langchain.llm_cache = None
+def lookup(cassette: Cassette, request: Request) -> Optional[Any]:
+    """
+    Code modified from OG vcrpy:
+    https://github.com/kevin1024/vcrpy/blob/v4.2.1/vcr/stubs/__init__.py#L225
+    """
+    if cassette.can_play_response_for(request):
+        log.info("Playing response for {} from cassette".format(request))
+        return cassette.play_response(request)
+    else:
+        if cassette.write_protected and cassette.filter_request(request):
+            raise CannotOverwriteExistingCassetteException(
+                cassette=cassette, failed_request=request
+            )
+        return None
 
 
 class GenericPatch:
     """
     Generic class for patching into tool overrides
 
     Inherit from this, and ideally create a copy of the function you're patching in
@@ -70,16 +77,23 @@
             obj=self.same_signature_override,
             settings=gorilla.Settings(store_hit=True, allow_hit=not viz_was_here),
         )
 
     def get_generic_override_fn(self) -> Callable:
         def fn_override(og_self: Any, **kwargs: str) -> Any:
             """Actual override functionality"""
-            request = Request(tool=self.cls.__name__, **kwargs)
-            cached_response = self.cassette.lookup(request)
+            tool_name = self.cls.__name__
+            fake_uri = f"tool://{tool_name}"
+            request = Request(
+                method="POST",
+                uri=fake_uri,
+                body=json.dumps(kwargs, sort_keys=True),
+                headers={},
+            )
+            cached_response = lookup(self.cassette, request)
             if cached_response:
                 return cached_response
 
             new_response = self.og_fn(og_self, **kwargs)
             self.cassette.append(request, new_response)
             return new_response
 
@@ -92,26 +106,14 @@
     def __enter__(self) -> None:
         gorilla.apply(self.patch, id=VCR_LANGCHAIN_PATCH_ID)
 
     def __exit__(self, *_: List[Any]) -> None:
         gorilla.revert(self.patch)
 
 
-class SerpPatch(GenericPatch):
-    def __init__(self, cassette: Cassette):
-        super().__init__(cassette, SerpAPIWrapper, "run")
-
-    def get_same_signature_override(self) -> Callable:
-        def run(og_self: SerpPatch, query: str) -> str:
-            """Same signature override patched into SerpAPIWrapper"""
-            return self.generic_override(og_self, query=query)
-
-        return run
-
-
 class PythonREPLPatch(GenericPatch):
     def __init__(self, cassette: Cassette):
         super().__init__(cassette, PythonREPL, "run")
 
     def get_same_signature_override(self) -> Callable:
         def run(og_self: PythonREPL, command: str) -> str:
             """Same signature override patched into PythonREPL"""
@@ -128,15 +130,22 @@
         def run(og_self: BashProcess, commands: Union[str, List[str]]) -> str:
             """Same signature override patched into BashProcess"""
             return self.generic_override(og_self, commands=commands)
 
         return run
 
 
-class CassettePatcherBuilder(OgCassettePatcherBuilder):
-    def build(self) -> Tuple[Any, ...]:
-        return (
-            CachePatch(self._cassette),
-            SerpPatch(self._cassette),
-            PythonREPLPatch(self._cassette),
-            BashProcessPatch(self._cassette),
+def get_overridden_build(og_build: Callable) -> Callable:
+    def build(og_self: CassettePatcherBuilder) -> Iterable[Any]:
+        tool_patches = [
+            PythonREPLPatch(og_self._cassette),
+            BashProcessPatch(og_self._cassette),
+        ]
+        return itertools.chain(
+            og_build(og_self),
+            tool_patches,
         )
+
+    return build
+
+
+CassettePatcherBuilder.build = get_overridden_build(CassettePatcherBuilder.build)
```

### Comparing `vcr_langchain-0.0.8/setup.py` & `vcr_langchain-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['vcr_langchain']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['gorilla>=0.4.0,<0.5.0', 'langchain>=0.0.75,<0.0.76', 'vcrpy>=4.2.1,<5.0.0']
+['gorilla>=0.4.0,<0.5.0', 'langchain>=0.0.76,<0.0.77', 'vcrpy>=4.2.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'vcr-langchain',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Record and replay LLM interactions for langchain',
-    'long_description': '# VCR LangChain\n\nAdapts [VCR.py](https://github.com/kevin1024/vcrpy) for use with [LangChain](https://github.com/hwchase17/langchain). Refactor with confidence as you record and replay all your LLM logic in a contained environment, free from any and all side effects.\n\n## Quickstart\n\n```bash\npip install vcr-langchain\n```\n\nUse it with pytest:\n\n```python\nimport vcr_langchain as vcr\nfrom langchain.llms import OpenAI\n\n@vcr.use_cassette()\ndef test_use_as_test_decorator():\n    llm = OpenAI(model_name="text-ada-001")\n    assert llm("Tell me a surreal joke") == "<put the output here>"\n```\n\nThe next time you run it:\n\n- the output is now deterministic\n- it executes a lot faster by replaying from cache\n- no command executions or other side effects actually happen\n- you no longer need to have real API keys defined for test execution in CI environments\n\nFor more examples, see [the usages test file](tests/test_usage.py).\n\n### Why not just use VCR.py directly?\n\n- This offers higher-level, more human-readable recordings for inspection\n- This supports recordings of langchain tool interactions as well, which includes non-network requests such as command executions inside Bash or the Python REPL\n\n### Pitfalls\n\nNote that tools, if initialized outside of the `vcr_langchain` decorator, will not have recording capabilities patched in. This is true even if an agent using those tools is initialized within the decorator.\n\n## Documentation\n\nFor more information on how VCR works and what other options there are, please see the [VCR docs](https://vcrpy.readthedocs.io/en/latest/index.html).\n\nFor more information on how to use langchain, please see the [langchain docs](https://langchain.readthedocs.io/en/latest/).\n\n**Please note that there is a lot of langchain functionality that I haven\'t gotten around to hijacking for recording.** If there\'s anything you need to record in a cassette, please open a PR or issue.\n\n## Projects that use this\n\n- [LangChain Visualizer](https://github.com/amosjyng/langchain-visualizer)\n',
+    'long_description': '# VCR LangChain\n\nPatches [VCR.py](https://github.com/kevin1024/vcrpy) to include non-network tooling for use with [LangChain](https://github.com/hwchase17/langchain). Refactor with confidence as you record and replay all your LLM logic in a contained environment, free from any and all side effects.\n\n## Quickstart\n\n```bash\npip install vcr-langchain\n```\n\nUse it with pytest:\n\n```python\nimport vcr_langchain as vcr\nfrom langchain.llms import OpenAI\n\n@vcr.use_cassette()\ndef test_use_as_test_decorator():\n    llm = OpenAI(model_name="text-ada-001")\n    assert llm("Tell me a surreal joke") == "<put the output here>"\n```\n\nThe next time you run it:\n\n- the output is now deterministic\n- it executes a lot faster by replaying from cache\n- no command executions or other side effects actually happen\n- you no longer need to have real API keys defined for test execution in CI environments\n\nFor more examples, see [the usages test file](tests/test_usage.py).\n\n### Pitfalls\n\nNote that tools, if initialized outside of the `vcr_langchain` decorator, will not have recording capabilities patched in. This is true even if an agent using those tools is initialized within the decorator.\n\n## Documentation\n\nFor more information on how VCR works and what other options there are, please see the [VCR docs](https://vcrpy.readthedocs.io/en/latest/index.html).\n\nFor more information on how to use langchain, please see the [langchain docs](https://langchain.readthedocs.io/en/latest/).\n\n**Please note that there is a lot of langchain functionality that I haven\'t gotten around to hijacking for recording.** If there\'s anything you need to record in a cassette, please open a PR or issue.\n\n## Projects that use this\n\n- [LangChain Visualizer](https://github.com/amosjyng/langchain-visualizer)\n',
     'author': 'Amos Jun-yeung Ng',
     'author_email': 'me@amos.ng',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `vcr_langchain-0.0.8/PKG-INFO` & `vcr_langchain-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vcr-langchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Record and replay LLM interactions for langchain
 Author: Amos Jun-yeung Ng
 Author-email: me@amos.ng
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gorilla (>=0.4.0,<0.5.0)
-Requires-Dist: langchain (>=0.0.75,<0.0.76)
+Requires-Dist: langchain (>=0.0.76,<0.0.77)
 Requires-Dist: vcrpy (>=4.2.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # VCR LangChain
 
-Adapts [VCR.py](https://github.com/kevin1024/vcrpy) for use with [LangChain](https://github.com/hwchase17/langchain). Refactor with confidence as you record and replay all your LLM logic in a contained environment, free from any and all side effects.
+Patches [VCR.py](https://github.com/kevin1024/vcrpy) to include non-network tooling for use with [LangChain](https://github.com/hwchase17/langchain). Refactor with confidence as you record and replay all your LLM logic in a contained environment, free from any and all side effects.
 
 ## Quickstart
 
 ```bash
 pip install vcr-langchain
 ```
 
@@ -41,19 +41,14 @@
 - the output is now deterministic
 - it executes a lot faster by replaying from cache
 - no command executions or other side effects actually happen
 - you no longer need to have real API keys defined for test execution in CI environments
 
 For more examples, see [the usages test file](tests/test_usage.py).
 
-### Why not just use VCR.py directly?
-
-- This offers higher-level, more human-readable recordings for inspection
-- This supports recordings of langchain tool interactions as well, which includes non-network requests such as command executions inside Bash or the Python REPL
-
 ### Pitfalls
 
 Note that tools, if initialized outside of the `vcr_langchain` decorator, will not have recording capabilities patched in. This is true even if an agent using those tools is initialized within the decorator.
 
 ## Documentation
 
 For more information on how VCR works and what other options there are, please see the [VCR docs](https://vcrpy.readthedocs.io/en/latest/index.html).
```

