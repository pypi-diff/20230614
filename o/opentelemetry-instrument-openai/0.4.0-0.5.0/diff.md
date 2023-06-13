# Comparing `tmp/opentelemetry_instrument_openai-0.4.0.tar.gz` & `tmp/opentelemetry_instrument_openai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrument_openai-0.4.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrument_openai-0.5.0.tar", max compression
```

## Comparing `opentelemetry_instrument_openai-0.4.0.tar` & `opentelemetry_instrument_openai-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-06-09 23:19:37.566099 opentelemetry_instrument_openai-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     1175 2023-06-13 16:52:14.687909 opentelemetry_instrument_openai-0.4.0/README.md
--rw-r--r--   0        0        0      875 2023-06-13 16:52:29.117415 opentelemetry_instrument_openai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    16588 2023-06-13 04:33:56.454201 opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0      611 2023-06-13 04:35:41.149396 opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/package.py
--rw-r--r--   0        0        0      596 2023-06-13 16:52:35.655382 opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-13 22:46:01.950351 opentelemetry_instrument_openai-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     1360 2023-06-13 22:46:01.950351 opentelemetry_instrument_openai-0.5.0/README.md
+-rw-r--r--   0        0        0      875 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    24295 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/package.py
+-rw-r--r--   0        0        0      596 2023-06-13 22:46:01.954351 opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     2310 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.5.0/PKG-INFO
```

### Comparing `opentelemetry_instrument_openai-0.4.0/LICENSE.md` & `opentelemetry_instrument_openai-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.4.0/pyproject.toml` & `opentelemetry_instrument_openai-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentelemetry-instrument-openai"
-version = "0.4.0"
+version = "0.5.0"
 description = "OpenTelemetry openai instrumentation"
 license = "Apache-2.0"
 authors = ["cartermp <pcarter@fastmail.com>"]
 maintainers = ["cartermp <pcarter@fastmail.com>"]
 readme = "README.md"
 packages = [{include = "opentelemetry", from = "src" }]
```

### Comparing `opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/__init__.py` & `opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -386,28 +386,219 @@
             )
 
         return response
 
     wrapt.wrap_function_wrapper(openai.Moderation, "create", _instrumented_create)
 
 
+def _instrument_image_generate(tracer: Tracer):
+    def _instrumented_create(wrapped, instance, args, kwargs):
+        if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
+            return
+
+        name = "openai.image.generate"
+        with tracer.start_as_current_span(name, kind=SpanKind.CLIENT) as span:
+            span.set_attribute(f"{name}.prompt", kwargs["prompt"])
+            span.set_attribute(f"{name}.n", kwargs["n"] if "n" in kwargs else 1)
+            span.set_attribute(
+                f"{name}.size", kwargs["size"] if "size" in kwargs else "1024x1024"
+            )
+            span.set_attribute(
+                f"{name}.response_format",
+                kwargs["response_format"] if "response_format" in kwargs else "url",
+            )
+            span.set_attribute(
+                f"{name}.user", kwargs["user"] if "user" in kwargs else ""
+            )
+
+            response = wrapped(*args, **kwargs)
+
+            span.set_attribute(f"{name}.response.created", response["created"])
+            for index, choice in enumerate(response["data"]):
+                if (
+                    "response_format" not in kwargs
+                    or kwargs["response_format"] == "url"
+                ):
+                    span.set_attribute(
+                        f"{name}.response.data.{index}.url", choice["url"]
+                    )
+                # Not going to instrument the b64_json response because it's huge
+
+        return response
+
+    wrapt.wrap_function_wrapper(openai.Image, "create", _instrumented_create)
+
+
+def _instrument_image_edit(tracer: Tracer):
+    def _instrumented_create(wrapped, instance, args, kwargs):
+        if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
+            return
+
+        name = "openai.image.edit"
+        with tracer.start_as_current_span(name, kind=SpanKind.CLIENT) as span:
+            span.set_attribute(f"{name}.prompt", kwargs["prompt"])
+            span.set_attribute(f"{name}.image", kwargs["image"])
+            span.set_attribute(
+                f"{name}.mask", kwargs["mask"] if "mask" in kwargs else ""
+            )
+            span.set_attribute(f"{name}.n", kwargs["n"] if "n" in kwargs else 1)
+            span.set_attribute(
+                f"{name}.size", kwargs["size"] if "size" in kwargs else "1024x1024"
+            )
+            span.set_attribute(
+                f"{name}.response_format",
+                kwargs["response_format"] if "response_format" in kwargs else "url",
+            )
+            span.set_attribute(
+                f"{name}.user", kwargs["user"] if "user" in kwargs else ""
+            )
+
+            response = wrapped(*args, **kwargs)
+
+            span.set_attribute(f"{name}.response.created", response["created"])
+            for index, choice in enumerate(response["data"]):
+                if (
+                    "response_format" not in kwargs
+                    or kwargs["response_format"] == "url"
+                ):
+                    span.set_attribute(
+                        f"{name}.response.data.{index}.url", choice["url"]
+                    )
+                # Not going to instrument the b64_json response because it's huge
+
+        return response
+
+    wrapt.wrap_function_wrapper(openai.Image, "create_edit", _instrumented_create)
+
+
+def _instrument_image_variation(tracer: Tracer):
+    def _instrumented_create(wrapped, instance, args, kwargs):
+        if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
+            return
+
+        name = "openai.image.variation"
+        with tracer.start_as_current_span(name, kind=SpanKind.CLIENT) as span:
+            span.set_attribute(f"{name}.image", kwargs["image"])
+            span.set_attribute(f"{name}.n", kwargs["n"] if "n" in kwargs else 1)
+            span.set_attribute(
+                f"{name}.size", kwargs["size"] if "size" in kwargs else "1024x1024"
+            )
+            span.set_attribute(
+                f"{name}.response_format",
+                kwargs["response_format"] if "response_format" in kwargs else "url",
+            )
+            span.set_attribute(
+                f"{name}.user", kwargs["user"] if "user" in kwargs else ""
+            )
+
+            response = wrapped(*args, **kwargs)
+
+            span.set_attribute(f"{name}.response.created", response["created"])
+            for index, choice in enumerate(response["data"]):
+                if (
+                    "response_format" not in kwargs
+                    or kwargs["response_format"] == "url"
+                ):
+                    span.set_attribute(
+                        f"{name}.response.data.{index}.url", choice["url"]
+                    )
+                # Not going to instrument the b64_json response because it's huge
+
+        return response
+
+    wrapt.wrap_function_wrapper(openai.Image, "create_variation", _instrumented_create)
+
+
+def _instrument_audio_transcription(tracer: Tracer):
+    def _instrumented_create(wrapped, instance, args, kwargs):
+        if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
+            return
+
+        name = "openai.audio.transcribe"
+        with tracer.start_as_current_span(name, kind=SpanKind.CLIENT) as span:
+            span.set_attribute(f"{name}.file", kwargs["file"])
+            span.set_attribute(f"{name}.model", kwargs["model"])
+            span.set_attribute(
+                f"{name}.prompt", kwargs["prompt"] if "prompt" in kwargs else ""
+            )
+            span.set_attribute(
+                f"{name}.response_format",
+                kwargs["response_format"] if "response_format" in kwargs else "json",
+            )
+            span.set_attribute(
+                f"{name}.temperature",
+                kwargs["temperature"] if "temperature" in kwargs else 0.0,
+            )
+            span.set_attribute(
+                f"{name}.language", kwargs["language"] if "language" in kwargs else ""
+            )
+
+            response = wrapped(*args, **kwargs)
+
+            span.set_attribute(f"{name}.response.text", response["text"])
+
+        return response
+
+    wrapt.wrap_function_wrapper(openai.Audio, "transcribe", _instrumented_create)
+
+
+def _instrument_audio_translate(tracer: Tracer):
+    def _instrumented_create(wrapped, instance, args, kwargs):
+        if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
+            return
+
+        name = "openai.audio.translate"
+        with tracer.start_as_current_span(name, kind=SpanKind.CLIENT) as span:
+            span.set_attribute(f"{name}.file", kwargs["file"])
+            span.set_attribute(f"{name}.model", kwargs["model"])
+            span.set_attribute(
+                f"{name}.prompt", kwargs["prompt"] if "prompt" in kwargs else ""
+            )
+            span.set_attribute(
+                f"{name}.response_format",
+                kwargs["response_format"] if "response_format" in kwargs else "json",
+            )
+            span.set_attribute(
+                f"{name}.temperature",
+                kwargs["temperature"] if "temperature" in kwargs else 0.0,
+            )
+
+            response = wrapped(*args, **kwargs)
+
+            span.set_attribute(f"{name}.response.text", response["text"])
+
+        return response
+
+    wrapt.wrap_function_wrapper(openai.Audio, "translate", _instrumented_create)
+
+
 class OpenAIInstrumentor(BaseInstrumentor):
     """An instrumenter for OpenAI's client library."""
 
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs):
         tracer_provider = kwargs.get("tracer_provider")
         tracer = get_tracer(__name__, __version__, tracer_provider)
         _instrument_chat(tracer)
         _instrument_embedding(tracer)
         _instrument_completions(tracer)
         _instrument_edit(tracer)
         _instrument_moderation(tracer)
+        _instrument_image_generate(tracer)
+        _instrument_image_edit(tracer)
+        _instrument_image_variation(tracer)
+        _instrument_audio_transcription(tracer)
+        _instrument_audio_translate(tracer)
 
     def _uninstrument(self, **kwargs):
         unwrap(openai.ChatCompletion, "create")
         unwrap(openai.Embedding, "create")
         unwrap(openai.Completion, "create")
         unwrap(openai.Edit, "create")
         unwrap(openai.Moderation, "create")
+        unwrap(openai.Image, "create")
+        unwrap(openai.Image, "create_edit")
+        unwrap(openai.Image, "create_variation")
+        unwrap(openai.Audio, "transcribe")
+        unwrap(openai.Audio, "translate")
```

### Comparing `opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/package.py` & `opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/version.py` & `opentelemetry_instrument_openai-0.5.0/src/opentelemetry/instrumentation/openai/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
```

### Comparing `opentelemetry_instrument_openai-0.4.0/PKG-INFO` & `opentelemetry_instrument_openai-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrument-openai
-Version: 0.4.0
+Version: 0.5.0
 Summary: OpenTelemetry openai instrumentation
 License: Apache-2.0
 Author: cartermp
 Author-email: pcarter@fastmail.com
 Maintainer: cartermp
 Maintainer-email: pcarter@fastmail.com
 Requires-Python: >=3.7.1,<4.0
@@ -24,14 +24,24 @@
 
 # opentelemetry-instrument-openai
 
 It's OpenTelemetry instrumentation (python) for OpenAI's library.
 
 Project site: https://github.com/cartermp/opentelemetry-instrument-openai-py
 
+Supported APIs:
+
+- [x] Chat
+- [x] Embeddings
+- [x] Moderation
+- [x] Image (generation, edit, variation)
+- [x] Audio (transcribe, translate)
+- [x] Completion (GPT-3)
+- [x] Edit (GPT-3)
+
 ## How to use it
 
 Simple! First, install this package.
 
 ### Usage
 
 With autoinstrumentation agent:
```

