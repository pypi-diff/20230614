# Comparing `tmp/yamlfix-1.8.1.tar.gz` & `tmp/yamlfix-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlfix-1.8.1.tar", last modified: Mon Feb 13 10:41:15 2023, max compression
+gzip compressed data, was "yamlfix-1.9.0.tar", last modified: Fri Feb 17 10:22:33 2023, max compression
```

## Comparing `yamlfix-1.8.1.tar` & `yamlfix-1.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2020-11-24 19:23:51.578489 yamlfix-1.8.1/LICENSE
--rw-r--r--   0        0        0     1710 2022-12-27 11:41:38.720879 yamlfix-1.8.1/README.md
--rw-r--r--   0        0        0     6874 2023-02-13 10:41:07.055537 yamlfix-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      347 2022-03-10 20:21:31.805967 yamlfix-1.8.1/src/yamlfix/__init__.py
--rw-r--r--   0        0        0    28236 2023-02-13 10:41:05.475522 yamlfix-1.8.1/src/yamlfix/adapters.py
--rw-r--r--   0        0        0     1315 2022-12-20 12:46:21.235177 yamlfix-1.8.1/src/yamlfix/config.py
--rw-r--r--   0        0        0     1732 2023-02-06 10:21:13.682304 yamlfix-1.8.1/src/yamlfix/entrypoints/__init__.py
--rw-r--r--   0        0        0     3271 2023-02-06 10:21:13.682304 yamlfix-1.8.1/src/yamlfix/entrypoints/cli.py
--rw-r--r--   0        0        0     1028 2023-01-26 11:13:11.012465 yamlfix-1.8.1/src/yamlfix/model.py
--rw-r--r--   0        0        0        0 2023-01-09 21:44:23.473582 yamlfix-1.8.1/src/yamlfix/py.typed
--rw-r--r--   0        0        0     4674 2023-02-06 10:21:13.682304 yamlfix-1.8.1/src/yamlfix/services.py
--rw-r--r--   0        0        0      638 2023-02-13 10:41:06.967536 yamlfix-1.8.1/src/yamlfix/version.py
--rw-r--r--   0        0        0        0 2020-11-24 19:23:51.606489 yamlfix-1.8.1/tests/__init__.py
--rw-r--r--   0        0        0       64 2022-12-27 10:28:31.853652 yamlfix-1.8.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-11-24 19:23:51.606489 yamlfix-1.8.1/tests/e2e/__init__.py
--rw-r--r--   0        0        0    10775 2023-02-06 10:21:13.682304 yamlfix-1.8.1/tests/e2e/test_cli.py
--rw-r--r--   0        0        0        0 2020-12-17 16:30:38.148472 yamlfix-1.8.1/tests/integration/__init__.py
--rw-r--r--   0        0        0        0 2020-11-24 19:23:51.606489 yamlfix-1.8.1/tests/unit/__init__.py
--rw-r--r--   0        0        0    19120 2023-02-13 10:41:05.475522 yamlfix-1.8.1/tests/unit/test_adapter_yaml.py
--rw-r--r--   0        0        0    27157 2023-01-25 17:21:49.135901 yamlfix-1.8.1/tests/unit/test_services.py
--rw-r--r--   0        0        0      413 2022-06-13 08:44:02.030770 yamlfix-1.8.1/tests/unit/test_version.py
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 yamlfix-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-11-24 19:23:51.578489 yamlfix-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1710 2022-12-27 11:41:38.720879 yamlfix-1.9.0/README.md
+-rw-r--r--   0        0        0     6874 2023-02-17 10:22:17.462570 yamlfix-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      347 2022-03-10 20:21:31.805967 yamlfix-1.9.0/src/yamlfix/__init__.py
+-rw-r--r--   0        0        0    28311 2023-02-17 10:21:47.386286 yamlfix-1.9.0/src/yamlfix/adapters.py
+-rw-r--r--   0        0        0     1315 2022-12-20 12:46:21.235177 yamlfix-1.9.0/src/yamlfix/config.py
+-rw-r--r--   0        0        0     1732 2023-02-06 10:21:13.682304 yamlfix-1.9.0/src/yamlfix/entrypoints/__init__.py
+-rw-r--r--   0        0        0     3271 2023-02-06 10:21:13.682304 yamlfix-1.9.0/src/yamlfix/entrypoints/cli.py
+-rw-r--r--   0        0        0     1062 2023-02-17 10:21:47.386286 yamlfix-1.9.0/src/yamlfix/model.py
+-rw-r--r--   0        0        0        0 2023-01-09 21:44:23.473582 yamlfix-1.9.0/src/yamlfix/py.typed
+-rw-r--r--   0        0        0     4674 2023-02-06 10:21:13.682304 yamlfix-1.9.0/src/yamlfix/services.py
+-rw-r--r--   0        0        0      638 2023-02-17 10:22:17.382569 yamlfix-1.9.0/src/yamlfix/version.py
+-rw-r--r--   0        0        0        0 2020-11-24 19:23:51.606489 yamlfix-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       64 2022-12-27 10:28:31.853652 yamlfix-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-11-24 19:23:51.606489 yamlfix-1.9.0/tests/e2e/__init__.py
+-rw-r--r--   0        0        0    10775 2023-02-06 10:21:13.682304 yamlfix-1.9.0/tests/e2e/test_cli.py
+-rw-r--r--   0        0        0        0 2020-12-17 16:30:38.148472 yamlfix-1.9.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-24 19:23:51.606489 yamlfix-1.9.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    23311 2023-02-17 10:21:47.386286 yamlfix-1.9.0/tests/unit/test_adapter_yaml.py
+-rw-r--r--   0        0        0    27157 2023-02-16 10:22:13.116318 yamlfix-1.9.0/tests/unit/test_services.py
+-rw-r--r--   0        0        0      413 2022-06-13 08:44:02.030770 yamlfix-1.9.0/tests/unit/test_version.py
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 yamlfix-1.9.0/PKG-INFO
```

### Comparing `yamlfix-1.8.1/LICENSE` & `yamlfix-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/README.md` & `yamlfix-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/pyproject.toml` & `yamlfix-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.8.1"
+version = "1.9.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "src/yamlfix/version.py",
 ]
 
 [tool.autoimport.common_statements]
@@ -330,15 +330,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Utilities",
     "Natural Language :: English",
 ]
-version = "1.8.1"
+version = "1.9.0"
 
 [project.license]
 text = "GPL-3.0-only"
 
 [project.urls]
 Issues = "https://github.com/lyz-code/yamlfix/issues"
 homepage = "https://github.com/lyz-code/yamlfix"
```

### Comparing `yamlfix-1.8.1/src/yamlfix/adapters.py` & `yamlfix-1.9.0/src/yamlfix/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         )
         self.yaml.allow_duplicate_keys = config.allow_duplicate_keys
 
         # Start the document with ---
         # ignore: variable has type None, what can we do, it doesn't have type hints...
         self.yaml.explicit_start = config.explicit_start  # type: ignore
         self.yaml.width = config.line_length  # type: ignore
+        self.yaml.preserve_quotes = config.preserve_quotes  # type: ignore
 
 
 class YamlfixRepresenter(RoundTripRepresenter):
     """Yamlfix's custom implementation of the ruyaml.RoundTripRepresenter\
         that can be configured with YamlfixConfig."""
 
     def __init__(
```

### Comparing `yamlfix-1.8.1/src/yamlfix/config.py` & `yamlfix-1.9.0/src/yamlfix/config.py`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/src/yamlfix/entrypoints/__init__.py` & `yamlfix-1.9.0/src/yamlfix/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/src/yamlfix/entrypoints/cli.py` & `yamlfix-1.9.0/src/yamlfix/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/src/yamlfix/model.py` & `yamlfix-1.9.0/src/yamlfix/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,9 +26,10 @@
     indent_mapping: int = 2
     indent_offset: int = 2
     indent_sequence: int = 4
     line_length: int = 80
     none_representation: str = ""
     quote_basic_values: bool = False
     quote_keys_and_basic_values: bool = False
+    preserve_quotes: bool = False
     quote_representation: str = "'"
     sequence_style: YamlNodeStyle = YamlNodeStyle.FLOW_STYLE
```

### Comparing `yamlfix-1.8.1/src/yamlfix/services.py` & `yamlfix-1.9.0/src/yamlfix/services.py`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/src/yamlfix/version.py` & `yamlfix-1.9.0/src/yamlfix/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities to retrieve the information of the program version."""
 
 import platform
 import sys
 from textwrap import dedent
 
 # Do not edit this line manually, let `make bump` do it.
-__version__ = "1.8.1"
+__version__ = "1.9.0"
 
 
 def version_info() -> str:
     """Display the version of the program, python and the platform."""
     return dedent(
         f"""\
         ------------------------------------------------------------------
```

### Comparing `yamlfix-1.8.1/tests/e2e/test_cli.py` & `yamlfix-1.9.0/tests/e2e/test_cli.py`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/tests/unit/test_adapter_yaml.py` & `yamlfix-1.9.0/tests/unit/test_adapter_yaml.py`

 * *Files 24% similar despite different names*

```diff
@@ -207,14 +207,31 @@
         config = YamlfixConfig()
         config.none_representation = none_representation
 
         result = fix_code(source, config)
 
         assert result == fixed_source
 
+    def test_preserve_quotes_config(self) -> None:
+        """Make it configurable. That quotes are preserved"""
+        source = dedent(
+            """\
+            ---
+            str_key1: "value"
+            str_key2: 'value'
+            str_key3: value
+            """
+        )
+        config = YamlfixConfig()
+        config.preserve_quotes = True
+
+        result = fix_code(source, config)
+
+        assert result == source
+
     @pytest.mark.parametrize("quote_representation", quote_representations)
     def test_quote_all_keys_and_values_config(self, quote_representation: str) -> None:
         """Quote all keys and values with configurable quote representation."""
         source = dedent(
             """\
             none_key: null
             bool_key: true
@@ -317,14 +334,132 @@
         config.quote_representation = quote_representation
         config.quote_basic_values = True
 
         result = fix_code(source, config)
 
         assert result == fixed_source
 
+    @pytest.mark.parametrize("quote_representation", quote_representations)
+    def test_quote_all_keys_and_values_config_and_preserve_quotes(
+        self, quote_representation: str
+    ) -> None:
+        """Quote all keys and values with configurable quote representation. \
+           `quote_keys_and_basic_values` in combination with `preserve_quotes`"""
+        source = dedent(
+            """\
+            none_key: null
+            bool_key: true
+            int_key: 1
+            str_key1: "value"
+            str_key2: 'value'
+            str_key3: value
+            str_multiline: |
+              value
+              value
+            complex_key:
+              complex_key2: value
+              list:
+                - item1
+                - item2
+              complex_list:
+                - item1
+                - complex_item:
+                    key: value
+            """
+        )
+        quote = quote_representation
+        fixed_source = dedent(
+            f"""\
+            ---
+            {quote}none_key{quote}:
+            {quote}bool_key{quote}: true
+            {quote}int_key{quote}: 1
+            {quote}str_key1{quote}: "value"
+            {quote}str_key2{quote}: 'value'
+            {quote}str_key3{quote}: {quote}value{quote}
+            {quote}str_multiline{quote}: |
+              value
+              value
+            {quote}complex_key{quote}:
+              {quote}complex_key2{quote}: {quote}value{quote}
+              {quote}list{quote}: [{quote}item1{quote}, {quote}item2{quote}]
+              {quote}complex_list{quote}:
+                - {quote}item1{quote}
+                - {quote}complex_item{quote}:
+                    {quote}key{quote}: {quote}value{quote}
+            """
+        )
+        config = YamlfixConfig()
+        config.quote_representation = quote_representation
+        config.quote_keys_and_basic_values = True
+        config.preserve_quotes = True
+
+        result = fix_code(source, config)
+
+        assert result == fixed_source
+
+    @pytest.mark.parametrize("quote_representation", quote_representations)
+    def test_quote_values_config_and_preserve_quotes(
+        self, quote_representation: str
+    ) -> None:
+        """Quote only scalar values with configurable quote representation. \
+           `quote_basic_values` in combination with `preserve_quotes`"""
+        source = dedent(
+            """\
+            none_key: null
+            bool_key: true
+            int_key: 1
+            str_key1: "value"
+            str_key2: 'value'
+            str_key3: value
+            str_multiline: |
+              value
+              value
+            complex_key:
+              complex_key2: value
+              list:
+                - item1
+                - item2
+              complex_list:
+                - item1
+                - complex_item:
+                    key: 'value?'
+            """
+        )
+        quote = quote_representation
+        fixed_source = dedent(
+            f"""\
+            ---
+            none_key:
+            bool_key: true
+            int_key: 1
+            str_key1: "value"
+            str_key2: 'value'
+            str_key3: {quote}value{quote}
+            str_multiline: |
+              value
+              value
+            complex_key:
+              complex_key2: {quote}value{quote}
+              list: [{quote}item1{quote}, {quote}item2{quote}]
+              complex_list:
+                - item1
+                - complex_item:
+                    key: 'value?'
+            """
+        )
+        config = YamlfixConfig()
+        config.quote_representation = quote_representation
+        config.quote_basic_values = True
+        config.preserve_quotes = True
+
+        result = fix_code(source, config)
+
+        assert result == fixed_source
+
     def test_sequence_flow_style_config(self) -> None:
         """Make inline list style 'flow-style' configurable."""
         source = dedent(
             """\
             list:
               - item
               - item
@@ -602,15 +737,15 @@
     def test_section_whitelines(self) -> None:
         """Check if section whitelines are preserved."""
         source = dedent(
             # pylint: disable=C0303
             """\
             ---
 
-            begin_section: 
+            begin_section:
               key: value
             key1: value
 
             key2: value
 
             happy_path_section:
               key1: value
@@ -673,15 +808,15 @@
 
     def test_section_whitelines_begin_no_explicit_start(self) -> None:
         """Check that no whitelines are added at start of file when explicit start \
             is not applied."""
         source = dedent(
             # pylint: disable=C0303
             """\
-            begin_section: 
+            begin_section:
               key: value
             """  # noqa: W291
         )
         fixed_source = dedent(
             """\
             begin_section:
               key: value
```

### Comparing `yamlfix-1.8.1/tests/unit/test_services.py` & `yamlfix-1.9.0/tests/unit/test_services.py`

 * *Files identical despite different names*

### Comparing `yamlfix-1.8.1/PKG-INFO` & `yamlfix-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlfix
-Version: 1.8.1
+Version: 1.9.0
 Summary: A simple opionated yaml formatter that keeps your comments!
 License: GPL-3.0-only
 Author-email: Lyz <lyz-code-security-advisories@riseup.net>
 Requires-Python: >=3.7.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yamlfix Version: 1.8.1 Summary: A simple opionated
+Metadata-Version: 2.1 Name: yamlfix Version: 1.9.0 Summary: A simple opionated
 yaml formatter that keeps your comments! License: GPL-3.0-only Author-email:
 Lyz
 riseup.net> Requires-Python: >=3.7.2 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Natural Language :: English Classifier: Operating System :: POSIX Classifier:
 Operating System :: Unix Classifier: Programming Language :: Python Classifier:
```

