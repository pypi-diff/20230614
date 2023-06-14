# Comparing `tmp/robotcode_language_server-0.41.0.tar.gz` & `tmp/robotcode_language_server-0.43.0.tar.gz`

## Comparing `robotcode_language_server-0.41.0.tar` & `robotcode_language_server-0.43.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38199 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    56373 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    66000 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83635 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    85398 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19441 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23534 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24255 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42551 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    11515 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    18981 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38247 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    56507 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    66971 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83614 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    85311 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42861 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15709 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.43.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,17 @@
         from robot.parsing.lexer.tokens import Token as RobotToken
         from robot.parsing.model.statements import Variable
         from robot.variables import search_variable
 
         variable = cast(Variable, node)
 
         name_token = variable.get_token(RobotToken.VARIABLE)
+        if name_token is None:
+            return
+
         name = name_token.value
 
         if name is not None:
             match = search_variable(name, ignore_errors=True)
             if not match.is_assign(allow_assign_mark=True):
                 return
 
@@ -431,15 +434,15 @@
                     self.append_diagnostics(
                         range=kw_range,
                         message=f"'{result.name}' is a reserved keyword.",
                         severity=DiagnosticSeverity.ERROR,
                         code="ReservedKeyword",
                     )
 
-                if get_robot_version() >= (6, 0, 0) and result.is_resource_keyword and result.is_private():
+                if get_robot_version() >= (6, 0) and result.is_resource_keyword and result.is_private():
                     if self.namespace.source != result.source:
                         self.append_diagnostics(
                             range=kw_range,
                             message=f"Keyword '{result.longname}' is private and should only be called by"
                             f" keywords in the same file.",
                             severity=DiagnosticSeverity.WARNING,
                             code="PrivateKeyword",
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,19 @@
 
 if TYPE_CHECKING:
     from robotcode.language_server.robotframework.protocol import RobotLanguageServerProtocol
 
     from .namespace import Namespace
 
 
-RESOURCE_EXTENSIONS = (".resource", ".robot", ".txt", ".tsv", ".rst", ".rest")
+RESOURCE_EXTENSIONS = (
+    {".resource", ".robot", ".txt", ".tsv", ".rst", ".rest", ".json", ".rsrc"}
+    if get_robot_version() >= (6, 1)
+    else {".resource", ".robot", ".txt", ".tsv", ".rst", ".rest"}
+)
 REST_EXTENSIONS = (".rst", ".rest")
 
 
 LOAD_LIBRARY_TIME_OUT = 30
 FIND_FILE_TIME_OUT = 10
 COMPLETE_LIBRARY_IMPORT_TIME_OUT = COMPLETE_RESOURCE_IMPORT_TIME_OUT = COMPLETE_VARIABLES_IMPORT_TIME_OUT = 10
 
@@ -1218,15 +1222,15 @@
             source_type=libdoc.type,
             keywords=[
                 KeywordDoc(
                     name=kw[0].name,
                     args=[KeywordArgumentDoc.from_robot(a) for a in kw[0].args],
                     doc=kw[0].doc,
                     tags=list(kw[0].tags),
-                    source=kw[0].source,
+                    source=str(kw[0].source),
                     name_token=get_keyword_name_token_from_line(kw[0].lineno),
                     line_no=kw[0].lineno if kw[0].lineno is not None else -1,
                     col_offset=-1,
                     end_col_offset=-1,
                     end_line_no=-1,
                     libname=libdoc.name,
                     libtype=libdoc.type,
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,26 @@
 DEFAULT_LIBRARIES = (BUILTIN_LIBRARY_NAME, RESERVED_LIBRARY_NAME, "Easter")
 ROBOT_LIBRARY_PACKAGE = "robot.libraries"
 
 ALLOWED_LIBRARY_FILE_EXTENSIONS = [".py"]
 
 ROBOT_FILE_EXTENSION = ".robot"
 RESOURCE_FILE_EXTENSION = ".resource"
+REST_EXTENSIONS = {".rst", ".rest"}
+JSON_EXTENSIONS = {".json", ".rsrc"}
 
-ALLOWED_RESOURCE_FILE_EXTENSIONS = [ROBOT_FILE_EXTENSION, RESOURCE_FILE_EXTENSION]
-ALLOWED_VARIABLES_FILE_EXTENSIONS = [".py", ".yml", ".yaml"]
+ALLOWED_RESOURCE_FILE_EXTENSIONS = (
+    {ROBOT_FILE_EXTENSION, RESOURCE_FILE_EXTENSION, *REST_EXTENSIONS, *JSON_EXTENSIONS}
+    if get_robot_version() >= (6, 1)
+    else {ROBOT_FILE_EXTENSION, RESOURCE_FILE_EXTENSION, *REST_EXTENSIONS}
+)
+
+ALLOWED_VARIABLES_FILE_EXTENSIONS = (
+    {".py", ".yml", ".yaml", ".json"} if get_robot_version() >= (6, 1) else {".py", ".yml", ".yaml"}
+)
 ROBOT_DOC_FORMAT = "ROBOT"
 REST_DOC_FORMAT = "REST"
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 
 
 def convert_from_rest(text: str) -> str:
@@ -383,15 +392,15 @@
 
     @single_call
     def normalized_tags(self) -> List[str]:
         return [normalize(tag) for tag in self.tags]
 
     @single_call
     def is_private(self) -> bool:
-        if get_robot_version() < (6, 0, 0):
+        if get_robot_version() < (6, 0):
             return False
 
         return "robot:private" in self.normalized_tags()
 
     @property
     def range(self) -> Range:
         if self.name_token is not None:
@@ -815,14 +824,16 @@
 
 
 def is_library_by_path(path: str) -> bool:
     return path.lower().endswith((".py", "/", os.sep))
 
 
 def is_variables_by_path(path: str) -> bool:
+    if get_robot_version() >= (6, 1):
+        return path.lower().endswith((".py", ".yml", ".yaml", ".json", "/", os.sep))
     return path.lower().endswith((".py", ".yml", ".yaml", "/", os.sep))
 
 
 def _update_env(working_dir: str = ".") -> None:
     os.chdir(Path(working_dir))
 
 
@@ -884,19 +895,19 @@
             raise
         except BaseException:
             return []
 
     @property
     def source(self) -> Any:
         try:
-            return self.kw.source
+            return str(self.kw.source) if self.kw.source is not None else self.source
         except (SystemExit, KeyboardInterrupt):
             raise
         except BaseException:
-            return self.lib_source
+            return str(self.lib_source) if self.lib_source is not None else self.lib_source
 
     @property
     def lineno(self) -> Any:
         try:
             return self.kw.lineno
         except (SystemExit, KeyboardInterrupt):
             raise
@@ -1081,14 +1092,16 @@
     variables: Optional[Dict[str, Optional[Any]]] = None,
 ) -> Any:
     from robot.variables.finders import VariableFinder
 
     _update_env(working_dir)
 
     robot_variables = resolve_robot_variables(working_dir, base_dir, command_line_variables, variables)
+    if get_robot_version() >= (6, 1):
+        return VariableFinder(robot_variables).find(name.replace("\\", "\\\\"))
 
     return VariableFinder(robot_variables.store).find(name.replace("\\", "\\\\"))
 
 
 @contextmanager
 def _std_capture() -> Iterator[io.StringIO]:
     old__stdout__ = sys.__stdout__
@@ -1514,26 +1527,31 @@
 ) -> VariablesDoc:
     from robot.libdocpkg.robotbuilder import KeywordDocBuilder
     from robot.output import LOGGER
     from robot.running.handlers import _PythonHandler
     from robot.utils.importer import Importer
     from robot.variables.filesetter import PythonImporter, YamlImporter
 
+    if get_robot_version() >= (6, 1):
+        from robot.variables.filesetter import JsonImporter
+
     import_name: str = name
     stem = Path(name).stem
     module_spec: Optional[ModuleSpec] = None
     source: Optional[str] = None
     try:
         with _std_capture() as std_capturer:
             import_name = find_variables(name, working_dir, base_dir, command_line_variables, variables)
             get_variables = None
 
             if import_name.lower().endswith((".yaml", ".yml")):
                 source = import_name
                 importer = YamlImporter()
+            if get_robot_version() >= (6, 1) and import_name.lower().endswith(".json"):
+                importer = JsonImporter()
             else:
                 if not is_variables_by_path(import_name):
                     module_spec = get_module_spec(import_name)
 
                 # skip antigravity easter egg
                 # see https://python-history.blogspot.com/2010/06/import-antigravity.html
                 if import_name.lower() in ["antigravity"] or import_name.lower().endswith("antigravity.py"):
@@ -1886,14 +1904,15 @@
                         if f.is_dir():
                             yield CompleteResult(f.name, CompleteResultKind.MODULE)
 
                         if f.is_file():
                             if allow_modules and f.suffix.lower() not in [
                                 ".yaml",
                                 ".yml",
+                                *[".json" if get_robot_version() >= (6, 1) else []],
                             ]:
                                 yield CompleteResult(f.stem, CompleteResultKind.VARIABLES_MODULE)
                             if allow_files:
                                 yield CompleteResult(f.name, CompleteResultKind.VARIABLES)
     else:
         if path is None:
             paths = sys.path
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1765,15 +1765,15 @@
 
         if not result and self.handle_bdd_style:
             return self._get_bdd_style_keyword(name)
 
         return result
 
     def _get_keyword_from_self(self, name: str) -> Optional[KeywordDoc]:
-        if get_robot_version() >= (6, 0, 0):
+        if get_robot_version() >= (6, 0):
             found: List[Tuple[Optional[LibraryEntry], KeywordDoc]] = [
                 (None, v) for v in self.self_library_doc.keywords.get_all(name)
             ]
             if len(found) > 1:
                 found = self._select_best_matches(found)
                 if len(found) > 1:
                     self.diagnostics.append(
@@ -1809,15 +1809,15 @@
             yield ".".join(tokens[:i]), ".".join(tokens[i:])
 
     def _get_explicit_keyword(self, name: str) -> Optional[KeywordDoc]:
         found: List[Tuple[Optional[LibraryEntry], KeywordDoc]] = []
         for owner_name, kw_name in self._yield_owner_and_kw_names(name):
             found.extend(self.find_keywords(owner_name, kw_name))
 
-        if get_robot_version() >= (6, 0, 0) and len(found) > 1:
+        if get_robot_version() >= (6, 0) and len(found) > 1:
             found = self._select_best_matches(found)
 
         if len(found) > 1:
             self.diagnostics.append(
                 DiagnosticsEntry(
                     self._create_multiple_keywords_found_message(name, found, implicit=False),
                     DiagnosticSeverity.ERROR,
@@ -1828,15 +1828,15 @@
 
         return found[0][1] if found else None
 
     def find_keywords(self, owner_name: str, name: str) -> List[Tuple[LibraryEntry, KeywordDoc]]:
         if self._all_keywords is None:
             self._all_keywords = list(chain(self.namespace._libraries.values(), self.namespace._resources.values()))
 
-        if get_robot_version() >= (6, 0, 0):
+        if get_robot_version() >= (6, 0):
             result: List[Tuple[LibraryEntry, KeywordDoc]] = []
             for v in self._all_keywords:
                 if eq(v.alias or v.name, owner_name):
                     result.extend((v, kw) for kw in v.library_doc.keywords.get_all(name))
             return result
 
         result = []
@@ -1910,15 +1910,15 @@
             and candidate[1].matcher.embedded_arguments.match(other[1].name) is None
         )
 
     def _get_keyword_from_resource_files(self, name: str) -> Optional[KeywordDoc]:
         if self._resource_keywords is None:
             self._resource_keywords = list(chain(self.namespace._resources.values()))
 
-        if get_robot_version() >= (6, 0, 0):
+        if get_robot_version() >= (6, 0):
             found: List[Tuple[Optional[LibraryEntry], KeywordDoc]] = []
             for v in self._resource_keywords:
                 r = v.library_doc.keywords.get_all(name)
                 if r:
                     found.extend([(v, k) for k in r])
         else:
             found = []
@@ -1926,15 +1926,15 @@
                 s = k.library_doc.keywords.get(name, None)
                 if s is not None:
                     found.append((k, s))
 
         if not found:
             return None
 
-        if get_robot_version() >= (6, 0, 0):
+        if get_robot_version() >= (6, 0):
             if len(found) > 1:
                 found = self._prioritize_same_file_or_public(found)
 
                 if len(found) > 1:
                     found = self._select_best_matches(found)
 
                     if len(found) > 1:
@@ -1966,15 +1966,15 @@
 
         return entries
 
     def _get_keyword_from_libraries(self, name: str) -> Optional[KeywordDoc]:
         if self._library_keywords is None:
             self._library_keywords = list(chain(self.namespace._libraries.values()))
 
-        if get_robot_version() >= (6, 0, 0):
+        if get_robot_version() >= (6, 0):
             found: List[Tuple[Optional[LibraryEntry], KeywordDoc]] = []
             for v in self._library_keywords:
                 r = v.library_doc.keywords.get_all(name)
                 if r:
                     found.extend([(v, k) for k in r])
         else:
             found = []
@@ -1983,15 +1983,15 @@
                 s = k.library_doc.keywords.get(name, None)
                 if s is not None:
                     found.append((k, s))
 
         if not found:
             return None
 
-        if get_robot_version() >= (6, 0, 0):
+        if get_robot_version() >= (6, 0):
             if len(found) > 1:
                 found = self._select_best_matches(found)
                 if len(found) > 1:
                     found = self._get_keyword_based_on_search_order(found)
         else:
             if len(found) > 1:
                 found = self._get_keyword_based_on_search_order(found)
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,15 +916,15 @@
         position: Position,
         context: Optional[CompletionContext],
     ) -> Optional[List[CompletionItem]]:
         from robot.parsing.lexer.tokens import Token as RobotToken
         from robot.parsing.model.statements import Arguments, Statement
 
         if len(nodes_at_position) > 1 and isinstance(nodes_at_position[0], Statement):
-            statement_node = cast(Statement, nodes_at_position[0])
+            statement_node = nodes_at_position[0]
             if len(statement_node.tokens) > 0:
                 token = cast(Token, statement_node.tokens[0])
                 r = range_from_token(token)
                 value = token.value.strip()
                 only_stars = value is not None and "*" in value and all(v == "*" for v in value)
                 if (
                     r.start.character == 0
@@ -1156,30 +1156,30 @@
             ]
 
         def check_in_template() -> bool:
             testcase_node = cast(TestCase, node)
             if any(
                 template
                 for template in testcase_node.body
-                if isinstance(template, Template) and cast(Template, template).value is not None
+                if isinstance(template, Template) and template.value is not None
             ):
                 return True
 
             if any(
                 file
                 for file in nodes_at_position
                 if isinstance(file, File)
                 and any(
                     section
-                    for section in cast(File, file).sections
+                    for section in file.sections
                     if isinstance(section, SettingSection)
                     and any(
                         template
-                        for template in cast(SettingSection, section).body
-                        if isinstance(template, TestTemplate) and cast(TestTemplate, template).value is not None
+                        for template in section.body
+                        if isinstance(template, TestTemplate) and template.value is not None
                     )
                 )
             ):
                 return True
 
             return False
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,14 @@
             return await self.get_general_model(document, data_only)
         if document_type == DocumentType.RESOURCE:
             return await self.get_resource_model(document, data_only)
 
         raise UnknownFileTypeError(f"Unknown file type '{document.uri}'.")
 
     def __get_model(self, document: TextDocument, tokens: Iterable[Any], document_type: DocumentType) -> ast.AST:
-        from robot.parsing.lexer import Token
         from robot.parsing.parser.parser import _get_model
 
         def get_tokens(source: str, data_only: bool = False, lang: Any = None) -> Iterator[Token]:
             for t in tokens:
                 check_canceled_sync()
 
                 yield t
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
                                 str(document.uri.to_path().parent),
                                 await namespace.get_resolvable_variables(nodes, position),
                             )
                         )
                     except (asyncio.CancelledError, SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException:
+                        self._logger.exception("Error resolving variable: {e}")
                         value = ""
                 else:
                     value = ""
 
                 return Hover(
                     contents=MarkupContent(
                         kind=MarkupKind.MARKDOWN,
@@ -394,15 +395,15 @@
         self, node: ast.AST, nodes: List[ast.AST], document: TextDocument, position: Position
     ) -> Optional[Hover]:
         from robot.parsing.lexer.tokens import Token as RobotToken
         from robot.parsing.model.statements import LibraryImport
 
         library_node = cast(LibraryImport, node)
         if library_node.name:
-            name_token = cast(RobotToken, library_node.get_token(RobotToken.NAME))
+            name_token = library_node.get_token(RobotToken.NAME)
             if name_token is None:
                 return None
 
             token_range = range_from_token(name_token)
             if position.is_in_range(token_range):
                 namespace = await self.parent.documents_cache.get_namespace(document)
 
@@ -543,30 +544,34 @@
 
         return None
 
     async def hover_TestCase(  # noqa: N802
         self, node: ast.AST, nodes: List[ast.AST], document: TextDocument, position: Position
     ) -> Optional[Hover]:
         from robot.parsing.lexer.tokens import Token as RobotToken
-        from robot.parsing.model.blocks import TestCase
+        from robot.parsing.model.blocks import TestCase, TestCaseSection
         from robot.parsing.model.statements import Documentation, Tags
 
         test_case = cast(TestCase, node)
 
         if not position.is_in_range(range_from_node(test_case.header)):
             return None
 
         name_token = cast(RobotToken, test_case.header.get_token(RobotToken.TESTCASE_NAME))
         if name_token is None:
             return None
 
         doc = next((e for e in test_case.body if isinstance(e, Documentation)), None)
         tags = next((e for e in test_case.body if isinstance(e, Tags)), None)
 
-        txt = f"= Test Case *{test_case.name}* =\n"
+        section = next((e for e in nodes if isinstance(e, TestCaseSection)), None)
+        if section is not None and section.tasks:
+            txt = f"= Task *{test_case.name}* =\n"
+        else:
+            txt = f"= Test Case *{test_case.name}* =\n"
 
         if doc is not None:
             txt += "\n== Documentation ==\n"
             txt += f"\n{doc.value}\n"
 
         if tags is not None:
             txt += "\n*Tags*: "
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
                                 sub_token.lineno,
                                 sub_token.end_col_offset,
                                 namespace.source,
                                 tokval,
                                 sub_token,
                             )
                     variable_started = False
-                if toknum == python_token.ERRORTOKEN and tokval == "$":
+                if tokval == "$":
                     variable_started = True
         except TokenError:
             pass
 
     @staticmethod
     def remove_index_from_variable_token(token: Token) -> Tuple[Token, Optional[Token]]:
         from robot.parsing.lexer import Token as RobotToken
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
                     return found_issues
 
             analyser = MyRobocop(from_cli=False, config=config)
             analyser.reload_config()
 
             # TODO find a way to cancel the run_check
-            issues = await analyser.run_check(  # type: ignore
+            issues = await analyser.run_check(
                 await self.parent.documents_cache.get_model(document, False),
                 str(document.uri.to_path()),
                 document.text(),
             )
 
             for issue in issues:
                 await check_canceled()
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     SECTION = "section"
     SETTING_IMPORT = "settingImport"
     SETTING = "setting"
     HEADER = "header"
     HEADER_SETTINGS = "headerSettings"
     HEADER_VARIABLE = "headerVariable"
     HEADER_TESTCASE = "headerTestcase"
+    HEADER_TASK = "headerTask"
     HEADER_COMMENT = "headerComment"
     HEADER_KEYWORD = "headerKeyword"
     TESTCASE_NAME = "testcaseName"
     KEYWORD_NAME = "keywordName"
     CONTROL_FLOW = "controlFlow"
     ARGUMENT = "argument"
     EMBEDDED_ARGUMENT = "embeddedArgument"
@@ -227,14 +228,23 @@
                     frozenset(
                         {
                             RobotToken.CONFIG,
                         }
                     ): (RobotSemTokenTypes.CONFIG, None),
                 }
             )
+            definition.update(
+                {
+                    frozenset(
+                        {
+                            RobotToken.TASK_HEADER,
+                        }
+                    ): (RobotSemTokenTypes.HEADER_TASK, None),
+                }
+            )
 
         result: Dict[str, Tuple[Enum, Optional[Set[Enum]]]] = {}
         for k, v in definition.items():
             for e in k:
                 result[e] = v
 
         return result
```

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.43.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/.gitignore` & `robotcode_language_server-0.43.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/LICENSE.txt` & `robotcode_language_server-0.43.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/README.md` & `robotcode_language_server-0.43.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.41.0/pyproject.toml` & `robotcode_language_server-0.43.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.41.0",
-  "robotcode==0.41.0",
+  "robotcode-jsonrpc2==0.43.0",
+  "robotcode==0.43.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.41.0/PKG-INFO` & `robotcode_language_server-0.43.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.41.0
+Version: 0.43.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.41.0
-Requires-Dist: robotcode==0.41.0
+Requires-Dist: robotcode-jsonrpc2==0.43.0
+Requires-Dist: robotcode==0.43.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

