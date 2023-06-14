# Comparing `tmp/robotcode-0.9.5.tar.gz` & `tmp/robotcode-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotcode-0.9.5.tar", max compression
+gzip compressed data, was "robotcode-0.9.6.tar", max compression
```

## Comparing `robotcode-0.9.5.tar` & `robotcode-0.9.6.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    13821 2022-03-19 09:53:48.432442 robotcode-0.9.5/CHANGELOG.md
--rw-r--r--   0        0        0    10947 2022-03-19 09:53:48.432442 robotcode-0.9.5/LICENSE
--rw-r--r--   0        0        0     9547 2022-03-19 09:54:19.206441 robotcode-0.9.5/README.md
--rw-r--r--   0        0        0     3736 2022-03-19 09:54:11.085925 robotcode-0.9.5/pyproject.toml
--rw-r--r--   0        0        0       34 2022-03-19 09:53:48.476445 robotcode-0.9.5/robotcode/__init__.py
--rw-r--r--   0        0        0       22 2022-03-19 09:54:11.089925 robotcode-0.9.5/robotcode/_version.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0    13363 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0     2971 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/client.py
--rw-r--r--   0        0        0    24128 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    43291 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     5832 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/launcher/__main__.py
--rw-r--r--   0        0        0    10471 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     7368 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0       63 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/modifiers/__init__.py
--rw-r--r--   0        0        0     1527 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/modifiers/longname_modifiers.py
--rw-r--r--   0        0        0    12426 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0    11271 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/jsonrpc2/__init__.py
--rw-r--r--   0        0        0    25070 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/jsonrpc2/protocol.py
--rw-r--r--   0        0        0     7858 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/jsonrpc2/server.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0     7837 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     1592 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      276 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    48895 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/lsp_types.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     3366 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     5119 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     3565 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     3557 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0     8212 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2300 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     4925 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    10661 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2083 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4080 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2203 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     3648 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0      387 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2313 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     6286 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3471 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     1646 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    16660 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0     9209 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      844 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     7149 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     2125 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    20769 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     4190 2022-03-19 09:53:48.480445 robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    40086 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    58589 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    67110 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0     2916 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    69499 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     7704 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0     9212 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0    14422 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/discovering.py
--rw-r--r--   0        0        0    13573 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0    11043 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    13645 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4878 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     6173 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26448 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23087 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0    17336 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      407 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    33648 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0     5547 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     1269 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0    33331 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11535 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0     4813 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      286 2022-03-19 09:53:48.484445 robotcode-0.9.5/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1710 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7708 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/ast.py
--rw-r--r--   0        0        0     2895 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11589 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0     1579 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/process_pool.py
--rw-r--r--   0        0        0     1929 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1339 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0     1456 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0       65 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/py.typed
--rw-r--r--   0        0        0        0 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/__init__.py
--rw-r--r--   0        0        0     2677 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/async_itertools.py
--rw-r--r--   0        0        0    24417 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/async_tools.py
--rw-r--r--   0        0        0     7764 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/dataclasses.py
--rw-r--r--   0        0        0     1202 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/debugpy.py
--rw-r--r--   0        0        0     3680 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/event.py
--rw-r--r--   0        0        0     3546 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/glob_path.py
--rw-r--r--   0        0        0     1431 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/inspect.py
--rw-r--r--   0        0        0    15793 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/logging.py
--rw-r--r--   0        0        0      899 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/net.py
--rw-r--r--   0        0        0      350 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/path.py
--rw-r--r--   0        0        0     4702 2022-03-19 09:53:48.488446 robotcode-0.9.5/robotcode/utils/uri.py
--rw-r--r--   0        0        0    10939 2022-03-19 09:54:46.067539 robotcode-0.9.5/setup.py
--rw-r--r--   0        0        0    11069 2022-03-19 09:54:46.068587 robotcode-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    14454 2022-03-23 07:52:08.574645 robotcode-0.9.6/CHANGELOG.md
+-rw-r--r--   0        0        0    10947 2022-03-23 07:52:08.574645 robotcode-0.9.6/LICENSE
+-rw-r--r--   0        0        0     9547 2022-03-23 07:52:43.254351 robotcode-0.9.6/README.md
+-rw-r--r--   0        0        0     3736 2022-03-23 07:52:32.506408 robotcode-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0       34 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/__init__.py
+-rw-r--r--   0        0        0       22 2022-03-23 07:52:32.510408 robotcode-0.9.6/robotcode/_version.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0    13363 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0     2971 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/client.py
+-rw-r--r--   0        0        0    24128 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    43291 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     5832 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/launcher/__main__.py
+-rw-r--r--   0        0        0    10471 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     7368 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0       63 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/modifiers/__init__.py
+-rw-r--r--   0        0        0     1527 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/modifiers/longname_modifiers.py
+-rw-r--r--   0        0        0    12394 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0    11271 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/jsonrpc2/__init__.py
+-rw-r--r--   0        0        0    25054 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/jsonrpc2/protocol.py
+-rw-r--r--   0        0        0     7882 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/jsonrpc2/server.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0     7837 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     1592 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      276 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    48895 2022-03-23 07:52:08.618646 robotcode-0.9.6/robotcode/language_server/common/lsp_types.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     3366 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     5119 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     3565 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     3557 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0     8212 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2300 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     4925 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    10661 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2083 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4080 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2203 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     3648 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0      387 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2313 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     6286 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3471 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     1646 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    16660 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0     9209 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      844 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     7149 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     2185 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    25061 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     6071 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    40848 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    57242 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    68204 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0     2916 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    70139 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     7704 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0     9212 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0    14422 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/discovering.py
+-rw-r--r--   0        0        0    13573 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0    11043 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    13645 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4878 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     6173 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26448 2022-03-23 07:52:08.622646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23087 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0    19975 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      407 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    33999 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0     5547 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     1269 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0    33331 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11535 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0     4813 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      286 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1710 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7708 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/ast.py
+-rw-r--r--   0        0        0     2895 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11589 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0     1579 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/process_pool.py
+-rw-r--r--   0        0        0     1929 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1339 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0     1456 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0       65 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/py.typed
+-rw-r--r--   0        0        0        0 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/__init__.py
+-rw-r--r--   0        0        0     2677 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/async_itertools.py
+-rw-r--r--   0        0        0    24417 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/async_tools.py
+-rw-r--r--   0        0        0     7764 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/dataclasses.py
+-rw-r--r--   0        0        0     1202 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/debugpy.py
+-rw-r--r--   0        0        0     3680 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/event.py
+-rw-r--r--   0        0        0     3546 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/glob_path.py
+-rw-r--r--   0        0        0     1431 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/inspect.py
+-rw-r--r--   0        0        0    15793 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/logging.py
+-rw-r--r--   0        0        0      899 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/net.py
+-rw-r--r--   0        0        0      350 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/path.py
+-rw-r--r--   0        0        0     4702 2022-03-23 07:52:08.626646 robotcode-0.9.6/robotcode/utils/uri.py
+-rw-r--r--   0        0        0    10939 2022-03-23 07:53:05.769857 robotcode-0.9.6/setup.py
+-rw-r--r--   0        0        0    11069 2022-03-23 07:53:05.770711 robotcode-0.9.6/PKG-INFO
```

### Comparing `robotcode-0.9.5/CHANGELOG.md` & `robotcode-0.9.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # Change Log
 
 All notable changes to the "robotcode" extension will be documented in this file.
 
 ## [Unreleased]
 - none so far
+##  0.9.6
+
+- Variable analysis, finds undefined variables
+  - in variables, also inner variables like ${a+${b}}
+  - in inline python expression like ${{$a+$b}}
+  - in expression arguments of IF/WHILE statements like $a<$b
+  - in BuiltIn keywords which contains an expression or condition argument, like `Evaluate`, `Should Be True`, `Skip If`, ...
+- Improve handling of completion for argument definitions
+- Support for variable files
+  - there is a new setting `robotcode.robot.variableFiles` and corresponding `variableFiles` launch configuration setting
+  - this corresponds to the `--variablefile` option from robot
+
 ##  0.9.5
 
 ### added
 
 - Correct handling of argument definitions wich contains a default value from an allready defined argument
 
 ##  0.9.4
```

### Comparing `robotcode-0.9.5/LICENSE` & `robotcode-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/README.md` & `robotcode-0.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 Autocompletion for:
 - Libraries with parameters
 - Resources,
 - Variables
 - Keywords with parameters
 - Namespaces
 
-![Autocomplete Libraries and Keywords](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/autocomplete1.gif)
+![Autocomplete Libraries and Keywords](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/autocomplete1.gif)
 
 Autocompletion supports all supported variables types
   - local variables
   - variables from resource files
   - variables from variables file (.py and .yaml)
     - static and dynamic
   - command line variables
   - builtin variables
 
-![Autocomplete Variables](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/autocomplete2.gif)
+![Autocomplete Variables](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/autocomplete2.gif)
 
 ### Code Navigation
 
 - Symbols
 - Goto definitions and implementations
   - Keywords
   - Variables
@@ -86,15 +86,15 @@
 
 RobotCode can format your code with the internal RobotFramework robot.tidy tool (deprecated), but also with [Robotidy](https://robotidy.readthedocs.io/). Just install it.
 
 ### Running and Debugging
 
 RobotCode supports running and debugging of RobotFramework testcases and tasks out of the box, directly from the definition of the test or suite.
 
-![Running Tests](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/running_tests.gif)
+![Running Tests](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/running_tests.gif)
 
 In the debug console you can see all log messages of the current run and navigate to the keyword the message was written by.
 
 ### Multi-root Workspace folders
 
 RobotCodes support for [Multi-root Workspaces](https://code.visualstudio.com/docs/editor/multi-root-workspaces), enables loading and editing different Robotframework projects/folders with different RobotFramework/Python environments and settings at the same time or you can share the same RobotFramework/Python environment and settings for all folders in the workspace.
 
@@ -139,32 +139,32 @@
 
 ### Using Pre-Release Version
 
 Starting from VSCode version 1.63 it is possible to use pre-release versions of an extension. RobotCode uses recommend way for a version scheme, the major.EVEN_NUMBER.patch for release versions and major.ODD_NUMBER.patch for pre-release versions. RobotCode pre-release version will provide smaller changes or bugfixes maybe just one or two, and then all changes where collected to create a normal minor release with an even minor number.
 
 You can select install pre-release version at installion via extensions view:
 
-![Extensions View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/install_prelease_extension_list.gif)
+![Extensions View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/install_prelease_extension_list.gif)
 
 Or you can switch between release and pre-release version in the RobotCode Extension Information view:
 
-![Extension Information View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/switch_release_prerelease.gif)
+![Extension Information View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/switch_release_prerelease.gif)
 
 
 ## Customization
 
 ### Editor Style
 
 You can change some stylings for RobotFramework files in VSCode editor, independently of the current theme. (see [Customizing a Color Theme](https://code.visualstudio.com/docs/getstarted/themes#_customizing-a-color-theme))
 
 See the difference:
 
 | Before                                                           | After                                                      |
 | ---------------------------------------------------------------- | ---------------------------------------------------------- |
-| ![Without customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/without_customization.gif) | ![With customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/with_customization.gif) |
+| ![Without customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/without_customization.gif) | ![With customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/with_customization.gif) |
 
 
 As a template you can put the following code to your user settings of VSCode.
 
 Open the user `settings.json` like this:
 
 <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> or <kbd>F1</kbd> or <kbd>CMD</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>
```

### Comparing `robotcode-0.9.5/pyproject.toml` & `robotcode-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "robotcode"
-version = "0.9.5"
+version = "0.9.6"
 description = "Language server, debugger and tools for Robot Framework"
 authors = ["Daniel Biehl <daniel.biehl@imbus.de>"]
 homepage = 'https://github.com/d-biehl/robotcode'
 repository = 'https://github.com/d-biehl/robotcode'
 readme = "README.md"
 license = "Apache-2.0"
 include = ["robotcode/py.typed", "README.md", "CHANGELOG.md"]
```

### Comparing `robotcode-0.9.5/robotcode/debugger/__main__.py` & `robotcode-0.9.6/robotcode/debugger/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/client.py` & `robotcode-0.9.6/robotcode/debugger/client.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/dap_types.py` & `robotcode-0.9.6/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/debugger.py` & `robotcode-0.9.6/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/launcher/__main__.py` & `robotcode-0.9.6/robotcode/debugger/launcher/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/launcher/server.py` & `robotcode-0.9.6/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/listeners.py` & `robotcode-0.9.6/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/modifiers/longname_modifiers.py` & `robotcode-0.9.6/robotcode/debugger/modifiers/longname_modifiers.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/debugger/protocol.py` & `robotcode-0.9.6/robotcode/debugger/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,18 +117,18 @@
         )
 
     @staticmethod
     def _generate_json_rpc_messages_from_dict(
         data: Union[Dict[Any, Any], List[Dict[Any, Any]]]
     ) -> Iterator[ProtocolMessage]:
         def inner(d: Dict[Any, Any]) -> ProtocolMessage:
-            result = from_dict(d, (Request, Response, Event))  # type: ignore
+            result = from_dict(d, (Request, Response, Event))
             if isinstance(result, Response) and not result.success:
                 result = from_dict(d, ErrorResponse)
-            return result  # type: ignore
+            return result
 
         if isinstance(data, list):
             for e in data:
                 yield inner(e)
         else:
             yield inner(data)
```

### Comparing `robotcode-0.9.5/robotcode/debugger/server.py` & `robotcode-0.9.6/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/jsonrpc2/protocol.py` & `robotcode-0.9.6/robotcode/jsonrpc2/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
             if "jsonrpc" in d:
                 if d["jsonrpc"] != PROTOCOL_VERSION:
                     raise InvalidProtocolVersionError("Invalid JSON-RPC2 protocol version.")
                 d.pop("jsonrpc")
 
                 return from_dict(
                     d,
-                    (  # type: ignore
+                    (
                         JsonRPCRequest,
                         JsonRPCResponse,
                         JsonRPCNotification,
                         JsonRPCError,
                     ),
                 )
```

### Comparing `robotcode-0.9.5/robotcode/jsonrpc2/server.py` & `robotcode-0.9.6/robotcode/jsonrpc2/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,27 +206,27 @@
         self._serve_func = self._server.serve_forever
         self._run_func = self.loop.run_forever
 
     @_logger.call
     def start_pipe(self, pipe_name: Optional[str]) -> None:
         from typing import TYPE_CHECKING
 
-        if TYPE_CHECKING:
-            from asyncio.streams import StreamReaderProtocol
-            from asyncio.windows_events import ProactorEventLoop
-
         if pipe_name is None:
             raise ValueError("pipe name missing.")
 
         self.mode = JsonRpcServerMode.PIPE
 
         try:
             #  check if we are on windows and using the ProactorEventLoop, to use the undocumented
             #  create_pipe_connection method
             if sys.platform == "win32" and hasattr(self.loop, "create_pipe_connection"):
+                if TYPE_CHECKING:
+                    from asyncio.streams import StreamReaderProtocol
+                    from asyncio.windows_events import ProactorEventLoop
+
                 self.loop.run_until_complete(
                     cast("ProactorEventLoop", self.loop).create_pipe_connection(
                         lambda: cast("StreamReaderProtocol", self.create_protocol()), pipe_name
                     ),
                 )
             else:
                 self.loop.run_until_complete(self.loop.create_unix_connection(self.create_protocol, pipe_name))
```

### Comparing `robotcode-0.9.5/robotcode/language_server/__main__.py` & `robotcode-0.9.6/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/decorators.py` & `robotcode-0.9.6/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/lsp_types.py` & `robotcode-0.9.6/robotcode/language_server/common/lsp_types.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/code_lens.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/completion.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/declaration.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/definition.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/diagnostics.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/document_highlight.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/document_symbols.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/documents.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/folding_range.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/formatting.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/hover.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/implementation.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/references.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/signature_help.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/window.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/parts/workspace.py` & `robotcode-0.9.6/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/protocol.py` & `robotcode-0.9.6/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/server.py` & `robotcode-0.9.6/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/common/text_document.py` & `robotcode-0.9.6/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/configuration.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @config_section("robotcode.robot")
 @dataclass
 class RobotConfig(ConfigBase):
     args: Tuple[str, ...] = field(default_factory=tuple)
     python_path: List[str] = field(default_factory=list)
     env: Dict[str, str] = field(default_factory=dict)
     variables: Dict[str, Any] = field(default_factory=dict)
+    variable_files: List[str] = field(default_factory=list)
     paths: List[str] = field(default_factory=list)
     output_dir: Optional[str] = None
     output_file: Optional[str] = None
     log_file: Optional[str] = None
     debug_file: Optional[str] = None
     log_level: Optional[str] = None
     mode: Optional[str] = None
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,46 +15,132 @@
     Location,
     Position,
     Range,
 )
 from ...common.text_document import TextDocument
 from ..parts.model_helper import ModelHelperMixin
 from ..utils.ast import (
+    HasTokens,
+    Statement,
     Token,
     is_not_variable_token,
     range_from_node_or_token,
     range_from_token,
 )
 from ..utils.async_ast import AsyncVisitor
+from .entities import VariableNotFoundDefinition
 from .library_doc import KeywordDoc, is_embedded_keyword
 from .namespace import DIAGNOSTICS_SOURCE_NAME, KeywordFinder, Namespace
 
 EXTRACT_COMMENT_PATTERN = re.compile(r".*(?:^ *|\t+| {2,})#(?P<comment>.*)$")
 ROBOTCODE_PATTERN = re.compile(r"(?P<marker>\brobotcode\b)\s*:\s*(?P<rule>\b\w+\b)")
 
 
 class Analyzer(AsyncVisitor, ModelHelperMixin):
     def __init__(self, model: ast.AST, namespace: Namespace) -> None:
         from robot.parsing.model.statements import Template, TestTemplate
 
         self.model = model
-        self._namespace = namespace
+        self.namespace = namespace
         self.current_testcase_or_keyword_name: Optional[str] = None
-        self.finder = KeywordFinder(self._namespace)
+        self.finder = KeywordFinder(self.namespace)
         self.test_template: Optional[TestTemplate] = None
         self.template: Optional[Template] = None
+        self.node_stack: List[ast.AST] = []
 
     async def run(self) -> List[Diagnostic]:
         self._results: List[Diagnostic] = []
 
         await self.visit(self.model)
         return self._results
 
     async def visit(self, node: ast.AST) -> None:
-        await super().visit(node)
+        from robot.parsing.lexer.tokens import Token as RobotToken
+        from robot.parsing.model.statements import KeywordCall
+        from robot.variables.search import contains_variable
+
+        self.node_stack.append(node)
+        try:
+            if isinstance(node, HasTokens):
+                for token in (
+                    t
+                    for t in node.tokens
+                    if t.type != RobotToken.VARIABLE and t.error is None and contains_variable(t.value, "$@&%")
+                ):
+                    async for var_token, var in self.iter_variables_from_token(
+                        token,
+                        self.namespace,
+                        self.node_stack,
+                        range_from_token(token).start,
+                        skip_commandline_variables=False,
+                        return_not_found=True,
+                    ):
+                        if isinstance(var, VariableNotFoundDefinition):
+                            await self.append_diagnostics(
+                                range=range_from_token(var_token),
+                                message=f"Variable '{var.name}' not found",
+                                severity=DiagnosticSeverity.ERROR,
+                                source=DIAGNOSTICS_SOURCE_NAME,
+                            )
+            if (
+                isinstance(node, Statement)
+                and isinstance(node, self.get_expression_statement_types())
+                and (token := node.get_token(RobotToken.ARGUMENT)) is not None
+            ):
+                async for var_token, var in self.iter_expression_variables_from_token(
+                    token,
+                    self.namespace,
+                    self.node_stack,
+                    range_from_token(token).start,
+                    skip_commandline_variables=False,
+                    return_not_found=True,
+                ):
+                    if isinstance(var, VariableNotFoundDefinition):
+                        await self.append_diagnostics(
+                            range=range_from_token(var_token),
+                            message=f"Variable '{var.name}' not found",
+                            severity=DiagnosticSeverity.ERROR,
+                            source=DIAGNOSTICS_SOURCE_NAME,
+                        )
+            elif isinstance(node, Statement) and isinstance(node, KeywordCall) and node.keyword:
+                kw_doc = await self.namespace.find_keyword(node.keyword)
+                if kw_doc is not None and kw_doc.longname in [
+                    "BuiltIn.Evaluate",
+                    "BuiltIn.Should Be True",
+                    "BuiltIn.Should Not Be True",
+                    "BuiltIn.Skip If",
+                    "BuiltIn.Continue For Loop If",
+                    "BuiltIn.Exit For Loop If",
+                    "BuiltIn.Return From Keyword If",
+                    "BuiltIn.Run Keyword And Return If",
+                    "BuiltIn.Pass Execution If",
+                    "BuiltIn.Run Keyword If",
+                    "BuiltIn.Run Keyword Unless",
+                ]:
+                    tokens = node.get_tokens(RobotToken.ARGUMENT)
+                    if tokens and (token := tokens[0]):
+                        async for var_token, var in self.iter_expression_variables_from_token(
+                            token,
+                            self.namespace,
+                            self.node_stack,
+                            range_from_token(token).start,
+                            skip_commandline_variables=False,
+                            return_not_found=True,
+                        ):
+                            if isinstance(var, VariableNotFoundDefinition):
+                                await self.append_diagnostics(
+                                    range=range_from_token(var_token),
+                                    message=f"Variable '{var.name}' not found",
+                                    severity=DiagnosticSeverity.ERROR,
+                                    source=DIAGNOSTICS_SOURCE_NAME,
+                                )
+
+            await super().visit(node)
+        finally:
+            self.node_stack = self.node_stack[:-1]
 
     @staticmethod
     async def should_ignore(document: Optional[TextDocument], range: Range) -> bool:
         import builtins
 
         if document is not None:
             lines = await document.get_lines()
@@ -79,15 +165,15 @@
         code_description: Optional[CodeDescription] = None,
         source: Optional[str] = None,
         tags: Optional[List[DiagnosticTag]] = None,
         related_information: Optional[List[DiagnosticRelatedInformation]] = None,
         data: Optional[Any] = None,
     ) -> None:
 
-        if await self.should_ignore(self._namespace.document, range):
+        if await self.should_ignore(self.namespace.document, range):
             return
 
         self._results.append(
             Diagnostic(range, message, severity, code, code_description, source, tags, related_information, data)
         )
 
     async def _analyze_keyword_call(
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,23 +503,38 @@
             absolute_path = str(Path(p).absolute())
             if absolute_path not in self._python_path:
                 self._python_path.insert(0, absolute_path)
 
         return self._python_path or []
 
     @_logger.call
-    def get_command_line_variables(self) -> List[VariableDefinition]:
+    async def get_command_line_variables(self) -> List[VariableDefinition]:
+        from robot.utils.text import split_args_from_name_or_path
+
         if self._command_line_variables is None:
             if self.config is None:
                 self._command_line_variables = []
             else:
                 self._command_line_variables = [
                     CommandLineVariableDefinition(0, 0, 0, 0, "", f"${{{k}}}", None, has_value=True, value=(v,))
                     for k, v in self.config.variables.items()
                 ]
+                for variable_file in self.config.variable_files:
+                    name, args = split_args_from_name_or_path(variable_file)
+                    try:
+                        lib_doc = await self.get_libdoc_for_variables_import(
+                            name, tuple(args), str(self.folder.to_path()), self
+                        )
+                        if lib_doc is not None:
+                            self._command_line_variables += lib_doc.variables
+
+                    except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
+                        raise
+                    except BaseException as e:
+                        self._logger.exception(e)
 
         return self._command_line_variables
 
     @async_tasking_event
     async def libraries_changed(sender, libraries: List[LibraryDoc]) -> None:  # NOSONAR
         ...
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,60 +161,14 @@
 RUN_KEYWORD_IF_MATCHER = KeywordMatcher(RUN_KEYWORD_IF_NAME)
 
 RUN_KEYWORDS_MATCHER = KeywordMatcher(RUN_KEYWORDS_NAME)
 
 ALL_RUN_KEYWORDS_MATCHERS = [KeywordMatcher(e) for e in ALL_RUN_KEYWORDS]
 
 
-class InvalidVariableError(Exception):
-    pass
-
-
-class VariableMatcher:
-    def __init__(self, name: str) -> None:
-        from robot.utils.normalizing import normalize
-        from robot.variables.search import VariableSearcher
-
-        self.name = name
-
-        searcher = VariableSearcher("$@&%", ignore_errors=True)
-        match = searcher.search(name)
-
-        if match.base is None:
-            raise InvalidVariableError(f"Invalid variable '{name}'")
-
-        self.base = match.base
-
-        self.normalized_name = str(normalize(self.base, "_"))
-
-    def __eq__(self, o: object) -> bool:
-        from robot.utils.normalizing import normalize
-        from robot.variables.search import VariableSearcher
-
-        if isinstance(o, VariableMatcher):
-            return o.normalized_name == self.normalized_name
-        elif isinstance(o, str):
-            searcher = VariableSearcher("$@&%", ignore_errors=True)
-            match = searcher.search(o)
-            base = match.base
-            normalized = str(normalize(base, "_"))
-            return self.normalized_name == normalized
-        else:
-            return False
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-    def __str__(self) -> str:
-        return self.name
-
-    def __repr__(self) -> str:
-        return f"{type(self).__name__}(name={repr(self.name)})"
-
-
 @dataclass
 class Error:
     message: str
     type_name: str
     source: Optional[str] = None
     line_no: Optional[int] = None
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,31 +48,32 @@
     tokenize_variables,
 )
 from ..utils.async_ast import AsyncVisitor
 from ..utils.variables import BUILTIN_VARIABLES
 from .entities import (
     ArgumentDefinition,
     BuiltInVariableDefinition,
+    CommandLineVariableDefinition,
     EnvironmentVariableDefinition,
     Import,
     LibraryImport,
     LocalVariableDefinition,
     ResourceImport,
     VariableDefinition,
+    VariableMatcher,
     VariablesImport,
 )
 from .imports_manager import ImportsManager
 from .library_doc import (
     BUILTIN_LIBRARY_NAME,
     DEFAULT_LIBRARIES,
     KeywordDoc,
     KeywordError,
     KeywordMatcher,
     LibraryDoc,
-    VariableMatcher,
 )
 
 DIAGNOSTICS_SOURCE_NAME = "robotcode.namespace"
 
 
 class DiagnosticsError(Exception):
     pass
@@ -208,38 +209,41 @@
         )
 
     async def visit_Arguments(self, node: ast.AST) -> None:  # noqa: N802
         from robot.errors import VariableError
         from robot.parsing.lexer.tokens import Token as RobotToken
         from robot.parsing.model.statements import Arguments
 
+        args: List[str] = []
         n = cast(Arguments, node)
         arguments = n.get_tokens(RobotToken.ARGUMENT)
         for argument_token in (cast(RobotToken, e) for e in arguments):
             try:
                 argument = self.get_variable_token(argument_token)
 
                 if argument is not None:
                     if (
                         self.in_args
                         and self.position is not None
                         and self.position in range_from_token(argument_token)
                         and self.position > range_from_token(argument).end
                     ):
-                        continue
+                        break
 
-                    self._results[argument.value] = ArgumentDefinition(
-                        name=argument.value,
-                        name_token=strip_variable_token(argument),
-                        line_no=argument.lineno,
-                        col_offset=argument.col_offset,
-                        end_line_no=argument.lineno,
-                        end_col_offset=argument.end_col_offset,
-                        source=self.source,
-                    )
+                    if argument.value not in args:
+                        args.append(argument.value)
+                        self._results[argument.value] = ArgumentDefinition(
+                            name=argument.value,
+                            name_token=strip_variable_token(argument),
+                            line_no=argument.lineno,
+                            col_offset=argument.col_offset,
+                            end_line_no=argument.lineno,
+                            end_col_offset=argument.end_col_offset,
+                            source=self.source,
+                        )
 
             except VariableError:
                 pass
 
     async def visit_ExceptHeader(self, node: ast.AST) -> None:  # noqa: N802
         from robot.errors import VariableError
         from robot.parsing.lexer.tokens import Token as RobotToken
@@ -538,14 +542,16 @@
         self._analyze_lock = Lock()
         self._library_doc: Optional[LibraryDoc] = None
         self._library_doc_lock = Lock()
         self._imports: Optional[List[Import]] = None
         self._import_entries: OrderedDict[Import, LibraryEntry] = OrderedDict()
         self._own_variables: Optional[List[VariableDefinition]] = None
         self._own_variables_lock = Lock()
+        self._global_variables: Optional[List[VariableDefinition]] = None
+        self._global_variables_lock = Lock()
         self._diagnostics: List[Diagnostic] = []
         self._keywords: Optional[List[KeywordDoc]] = None
         self._keywords_lock = Lock()
 
         # TODO: how to get the search order from model
         self.search_order: Tuple[str, ...] = ()
 
@@ -597,14 +603,16 @@
             self._own_variables = None
             self._keywords = None
             self._library_doc = None
             self._analyzed = False
             self._diagnostics = []
             self._finder = None
 
+            await self._reset_global_variables()
+
         self.invalidated_callback(self)
 
     @_logger.call
     async def get_diagnostisc(self) -> List[Diagnostic]:
         await self.ensure_initialized()
 
         await self._analyze()
@@ -715,14 +723,16 @@
                                     self._resources.copy(),
                                     self._variables.copy(),
                                     self._diagnostics.copy(),
                                     self._import_entries.copy(),
                                 ),
                             )
 
+                    await self._reset_global_variables()
+
                     self._initialized = True
 
         return self._initialized
 
     @property
     def initialized(self) -> bool:
         return self._initialized
@@ -749,69 +759,85 @@
     def get_builtin_variables(cls) -> List[BuiltInVariableDefinition]:
         if cls._builtin_variables is None:
             cls._builtin_variables = [BuiltInVariableDefinition(0, 0, 0, 0, "", n, None) for n in BUILTIN_VARIABLES]
 
         return cls._builtin_variables
 
     @_logger.call
-    def get_command_line_variables(self) -> List[VariableDefinition]:
-        return self.imports_manager.get_command_line_variables()
+    async def get_command_line_variables(self) -> List[VariableDefinition]:
+        return await self.imports_manager.get_command_line_variables()
+
+    async def _reset_global_variables(self) -> None:
+        async with self._global_variables_lock:
+            self._global_variables = None
+
+    async def get_global_variables(self) -> List[VariableDefinition]:
+        if self._global_variables is None:
+            async with self._global_variables_lock:
+                if self._global_variables is None:
+                    self._global_variables = list(
+                        itertools.chain(
+                            await self.get_command_line_variables(),
+                            await self.get_own_variables(),
+                            *(e.variables for e in self._resources.values()),
+                            *(e.variables for e in self._variables.values()),
+                            self.get_builtin_variables(),
+                        )
+                    )
+
+        return self._global_variables
 
     @_logger.call
     async def yield_variables(
         self,
         nodes: Optional[List[ast.AST]] = None,
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
     ) -> AsyncGenerator[Tuple[VariableMatcher, VariableDefinition], None]:
         from robot.parsing.model.blocks import Keyword, TestCase
         from robot.parsing.model.statements import Arguments
 
-        # await self.ensure_initialized()
-
         yielded: Dict[VariableMatcher, VariableDefinition] = {}
 
+        test_or_keyword_nodes = list(
+            itertools.dropwhile(lambda v: not isinstance(v, (TestCase, Keyword)), nodes if nodes else [])
+        )
+        test_or_keyword = test_or_keyword_nodes[0] if test_or_keyword_nodes else None
+
         async for var in async_chain(
             *[
-                await BlockVariableVisitor(
-                    self.source, position, isinstance(nodes[-1], Arguments) if nodes else False
-                ).get(n)
-                for n in nodes or []
-                if isinstance(n, (Keyword, TestCase))
+                (
+                    await BlockVariableVisitor(
+                        self.source, position, isinstance(test_or_keyword_nodes[-1], Arguments) if nodes else False
+                    ).get(test_or_keyword)
+                )
+                if test_or_keyword is not None
+                else []
             ],
-            [] if skip_commandline_variables else (e for e in self.get_command_line_variables()),
-            (e for e in await self.get_own_variables()),
-            *(e.variables for e in self._resources.values()),
-            *(e.variables for e in self._variables.values()),
-            (e for e in self.get_builtin_variables()),
+            await self.get_global_variables(),
         ):
-            if var.name is not None:
-                matcher = VariableMatcher(var.name)
-                if matcher not in yielded.keys():
-                    yielded[matcher] = var
-                    yield matcher, var
+
+            if var.matcher not in yielded.keys():
+                yielded[var.matcher] = var
+
+                if skip_commandline_variables and isinstance(var, CommandLineVariableDefinition):
+                    continue
+
+                yield var.matcher, var
 
     async def get_resolvable_variables(
         self, nodes: Optional[List[ast.AST]] = None, position: Optional[Position] = None
     ) -> Dict[str, Any]:
         return {
             v.name: v.value
             async for k, v in self.yield_variables(nodes, position, skip_commandline_variables=True)
             if v.has_value
         }
 
     @_logger.call
-    async def get_variable_definitions(
-        self, nodes: Optional[List[ast.AST]] = None, position: Optional[Position] = None
-    ) -> Dict[str, VariableDefinition]:
-        await self.ensure_initialized()
-
-        return {m.name: v async for m, v in self.yield_variables(nodes, position)}
-
-    @_logger.call
     async def get_variable_matchers(
         self, nodes: Optional[List[ast.AST]] = None, position: Optional[Position] = None
     ) -> Dict[VariableMatcher, VariableDefinition]:
         await self.ensure_initialized()
 
         return {m: v async for m, v in self.yield_variables(nodes, position)}
 
@@ -1002,14 +1028,16 @@
                     await self.append_diagnostics(
                         range=value.range(),
                         message=str(e),
                         severity=DiagnosticSeverity.ERROR,
                         source=DIAGNOSTICS_SOURCE_NAME,
                         code=type(e).__qualname__,
                     )
+            finally:
+                await self._reset_global_variables()
 
             return result, variables
 
         current_time = time.time()
         self._logger.debug(lambda: f"start imports for {self.document if top_level else source}")
         try:
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/completion.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from ..diagnostics.namespace import Namespace
 from ..utils.ast import (
     HasTokens,
     Token,
     get_nodes_at_position,
     get_tokens_at_position,
     range_from_token,
+    tokenize_variables,
     whitespace_at_begin_of_token,
     whitespace_from_begin_of_token,
 )
 from ..utils.version import get_robot_version
 from .model_helper import ModelHelperMixin
 
 if TYPE_CHECKING:
@@ -406,15 +407,15 @@
                 insert_text_format=InsertTextFormat.PLAINTEXT,
                 text_edit=TextEdit(
                     range=range,
                     new_text=s.name[2:-1],
                 ),
                 filter_text=s.name[2:-1] if range is not None else None,
             )
-            for s in (await self.namespace.get_variable_matchers(nodes, position)).values()
+            for s in (await self.namespace.get_variable_matchers(list(reversed(nodes)), position)).values()
             if s.name is not None and (s.name_token is None or not position.is_in_range(range_from_token(s.name_token)))
         ]
 
     async def create_settings_completion_items(self, range: Optional[Range]) -> List[CompletionItem]:
         return [
             CompletionItem(
                 label=setting,
@@ -645,14 +646,29 @@
                         insert_text_format=InsertTextFormat.PLAINTEXT,
                         text_edit=TextEdit(range=r, new_text=k) if r is not None else None,
                     )
                 )
 
         return result
 
+    def get_variable_token(self, token: Token) -> Optional[Token]:
+        from robot.parsing.lexer.tokens import Token as RobotToken
+
+        return next(
+            (
+                v
+                for v in itertools.dropwhile(
+                    lambda t: t.type in RobotToken.NON_DATA_TOKENS,
+                    tokenize_variables(token, ignore_errors=True),
+                )
+                if v.type == RobotToken.VARIABLE
+            ),
+            None,
+        )
+
     async def complete_default(
         self,
         nodes_at_position: List[ast.AST],
         position: Position,
         context: Optional[CompletionContext],
     ) -> Optional[List[CompletionItem]]:
         from robot.parsing.lexer.tokens import Token as RobotToken
@@ -679,23 +695,24 @@
                         if position.is_in_range(r1) or position == r1.end:
                             r.end = r1.end
                             return await self.create_section_completion_items(r)
 
         elif position.character == 0:
             return await self.create_section_completion_items(None)
 
-        if (
-            len(nodes_at_position) > 1
-            and isinstance(nodes_at_position[0], Statement)
-            and not isinstance(nodes_at_position[0], Arguments)
-        ):
+        if len(nodes_at_position) > 1 and isinstance(nodes_at_position[0], HasTokens):
             node = nodes_at_position[0]
             tokens_at_position = get_tokens_at_position(node, position)
             token_at_position = tokens_at_position[-1]
 
+            if isinstance(node, Arguments):
+                arg = self.get_variable_token(token_at_position)
+                if arg is not None and position <= range_from_token(arg).end:
+                    return None
+
             token_at_position_index = tokens_at_position.index(token_at_position)
             while token_at_position.type in [RobotToken.EOL]:
                 token_at_position_index -= 1
                 if token_at_position_index < 0:
                     break
                 token_at_position = tokens_at_position[token_at_position_index]
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/discovering.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/discovering.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/goto.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/hover.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Set,
     Tuple,
     Type,
     Union,
 )
 
 from ...common.lsp_types import Position
-from ..diagnostics.entities import VariableDefinition
+from ..diagnostics.entities import VariableDefinition, VariableNotFoundDefinition
 from ..diagnostics.library_doc import KeywordDoc, KeywordError
 from ..diagnostics.namespace import LibraryEntry, Namespace
 from ..utils.ast import (
     Token,
     is_not_variable_token,
     iter_over_keyword_names_and_owners,
     range_from_token,
@@ -235,33 +235,45 @@
     @staticmethod
     async def iter_expression_variables_from_token(
         expression: Token,
         namespace: Namespace,
         nodes: Optional[List[ast.AST]],
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
+        return_not_found: bool = False,
     ) -> AsyncGenerator[Tuple[Token, VariableDefinition], Any]:
         from robot.api.parsing import Token as RobotToken
 
         variable_started = False
 
         for toknum, tokval, (_, tokcol), _, _ in generate_tokens(StringIO(expression.value).readline):
             if variable_started:
                 if toknum == python_token.NAME:
                     var = await namespace.find_variable(
                         f"${{{tokval}}}", nodes, position, skip_commandline_variables=skip_commandline_variables
                     )
+                    sub_token = RobotToken(
+                        expression.type,
+                        tokval,
+                        expression.lineno,
+                        expression.col_offset + tokcol,
+                        expression.error,
+                    )
                     if var is not None:
-                        yield RobotToken(
-                            expression.type,
+                        yield sub_token, var
+                    elif return_not_found:
+                        yield sub_token, VariableNotFoundDefinition(
+                            sub_token.lineno,
+                            sub_token.col_offset,
+                            sub_token.lineno,
+                            sub_token.end_col_offset,
+                            namespace.source,
                             tokval,
-                            expression.lineno,
-                            expression.col_offset + tokcol,
-                            expression.error,
-                        ), var
+                            sub_token,
+                        )
                 variable_started = False
             if toknum == python_token.ERRORTOKEN and tokval == "$":
                 variable_started = True
 
     @staticmethod
     def remove_index_from_variable_token(token: Token) -> Tuple[Token, Optional[Token]]:
         from robot.parsing.lexer import Token as RobotToken
@@ -327,18 +339,27 @@
     async def iter_variables_from_token(
         cls,
         token: Token,
         namespace: Namespace,
         nodes: Optional[List[ast.AST]],
         position: Optional[Position] = None,
         skip_commandline_variables: bool = False,
+        return_not_found: bool = False,
     ) -> AsyncGenerator[Tuple[Token, VariableDefinition], Any]:
         from robot.api.parsing import Token as RobotToken
         from robot.variables.search import contains_variable, search_variable
 
+        def is_number(name: str) -> bool:
+            from robot.variables.finders import NOT_FOUND, NumberFinder
+
+            if name.startswith("$"):
+                finder = NumberFinder()
+                return bool(finder.find(name) != NOT_FOUND)
+            return False
+
         async def iter_token(
             to: Token, ignore_errors: bool = False
         ) -> AsyncGenerator[Union[Token, Tuple[Token, VariableDefinition]], Any]:
             for sub_token in cls._tokenize_variables(to, ignore_errors=ignore_errors):
                 if sub_token.type == RobotToken.VARIABLE:
                     base = sub_token.value[2:-1]
                     if base and not (base[0] == "{" and base[-1] == "}"):
@@ -348,16 +369,28 @@
                             RobotToken(
                                 sub_token.type, base[1:-1], sub_token.lineno, sub_token.col_offset + 3, sub_token.error
                             ),
                             namespace,
                             nodes,
                             position,
                             skip_commandline_variables=skip_commandline_variables,
+                            return_not_found=return_not_found,
                         ):
                             yield v
+                    elif base == "" and return_not_found:
+                        yield sub_token, VariableNotFoundDefinition(
+                            sub_token.lineno,
+                            sub_token.col_offset,
+                            sub_token.lineno,
+                            sub_token.end_col_offset,
+                            namespace.source,
+                            sub_token.value,
+                            sub_token,
+                        )
+                        return
 
                     if contains_variable(base, "$@&%"):
                         async for sub_token_or_var in iter_token(
                             RobotToken(to.type, base, sub_token.lineno, sub_token.col_offset + 2),
                             ignore_errors=ignore_errors,
                         ):
                             if isinstance(sub_token_or_var, Token):
@@ -380,31 +413,57 @@
                 var = await namespace.find_variable(
                     name, nodes, position, skip_commandline_variables=skip_commandline_variables
                 )
                 if var is not None:
                     yield strip_variable_token(sub_token), var
                     continue
 
+                if is_number(sub_token.value):
+                    continue
+
                 if (
                     sub_token.type == RobotToken.VARIABLE
                     and sub_token.value[:1] in "$@&%"
                     and sub_token.value[1:2] == "{"
                     and sub_token.value[-1:] == "}"
                 ):
                     match = cls.__match_extended.match(name[2:-1])
                     if match is not None:
                         base_name, _ = match.groups()
                         name = f"{name[0]}{{{base_name.strip()}}}"
                         var = await namespace.find_variable(
                             name, nodes, position, skip_commandline_variables=skip_commandline_variables
                         )
+                        sub_sub_token = RobotToken(sub_token.type, name, sub_token.lineno, sub_token.col_offset)
                         if var is not None:
-                            yield strip_variable_token(
-                                RobotToken(sub_token.type, name, sub_token.lineno, sub_token.col_offset)
-                            ), var
+                            yield strip_variable_token(sub_sub_token), var
+                            continue
+                        if is_number(name):
+                            continue
+                        elif return_not_found:
+                            yield strip_variable_token(sub_sub_token), VariableNotFoundDefinition(
+                                sub_sub_token.lineno,
+                                sub_sub_token.col_offset,
+                                sub_sub_token.lineno,
+                                sub_sub_token.end_col_offset,
+                                namespace.source,
+                                name,
+                                sub_sub_token,
+                            )
+                            continue
+                if return_not_found:
+                    yield strip_variable_token(sub_token), VariableNotFoundDefinition(
+                        sub_token.lineno,
+                        sub_token.col_offset,
+                        sub_token.lineno,
+                        sub_token.end_col_offset,
+                        namespace.source,
+                        sub_token.value,
+                        sub_token,
+                    )
             else:
                 yield token_or_var
 
     __expression_statement_types: Optional[Tuple[Type[Any]]] = None
 
     @classmethod
     def get_expression_statement_types(cls) -> Tuple[Type[Any]]:
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/references.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 from ..utils.ast import (
     HasTokens,
     Statement,
     Token,
     get_nodes_at_position,
     get_tokens_at_position,
     is_not_variable_token,
-    iter_nodes_at_position,
     iter_over_keyword_names_and_owners,
     range_from_token,
     tokenize_variables,
 )
 from ..utils.async_ast import iter_nodes
 
 if TYPE_CHECKING:
@@ -262,14 +261,15 @@
     @_logger.call
     async def find_variable_references_in_file(
         self,
         doc: TextDocument,
         variable: VariableDefinition,
     ) -> List[Location]:
         from robot.parsing.lexer.tokens import Token as RobotToken
+        from robot.parsing.model.blocks import Block, Keyword, Section, TestCase
 
         namespace = await self.parent.documents_cache.get_namespace(doc)
         model = await self.parent.documents_cache.get_model(doc)
 
         if (
             variable.source
             and variable.source != str(doc.uri.to_path())
@@ -277,31 +277,37 @@
                 e for e in (await namespace.get_resources()).values() if e.library_doc.source == variable.source
             )
             and not any(
                 e
                 for e in (await namespace.get_imported_variables()).values()
                 if e.library_doc.source == variable.source
             )
+            and not any(e for e in await namespace.get_command_line_variables() if e.source == variable.source)
         ):
 
             return []
 
         expression_statements = self.get_expression_statement_types()
 
         result: List[Location] = []
+        current_block: Optional[Block] = None
 
         async for node in iter_nodes(model):
+            if isinstance(node, Section):
+                current_block = None
+            elif isinstance(node, (TestCase, Keyword)):
+                current_block = node
 
             if isinstance(node, HasTokens):
                 for token1 in node.tokens:
                     async for token in self.yield_argument_name_and_rest(node, token1):
                         async for token_and_var in self.iter_variables_from_token(
                             token,
                             namespace,
-                            [n async for n in iter_nodes_at_position(model, range_from_token(token).start)],
+                            [*([current_block] if current_block is not None else []), node],
                             range_from_token(token).start,
                         ):
                             sub_token, found_variable = token_and_var
 
                             if found_variable == variable:
                                 result.append(Location(str(doc.uri), range_from_token(sub_token)))
 
@@ -309,15 +315,15 @@
                 isinstance(node, Statement)
                 and isinstance(node, expression_statements)
                 and (token := node.get_token(RobotToken.ARGUMENT)) is not None
             ):
                 async for token_and_var in self.iter_expression_variables_from_token(
                     token,
                     namespace,
-                    [n async for n in iter_nodes_at_position(model, range_from_token(token).start)],
+                    [*([current_block] if current_block is not None else []), node],
                     range_from_token(token).start,
                 ):
                     sub_token, found_variable = token_and_var
 
                     if found_variable == variable:
                         result.append(Location(str(doc.uri), range_from_token(sub_token)))
```

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/protocol.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/ast.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/ast.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/process_pool.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/process_pool.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/variables.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/language_server/robotframework/utils/version.py` & `robotcode-0.9.6/robotcode/language_server/robotframework/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/async_itertools.py` & `robotcode-0.9.6/robotcode/utils/async_itertools.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/async_tools.py` & `robotcode-0.9.6/robotcode/utils/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/dataclasses.py` & `robotcode-0.9.6/robotcode/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/debugpy.py` & `robotcode-0.9.6/robotcode/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/event.py` & `robotcode-0.9.6/robotcode/utils/event.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/glob_path.py` & `robotcode-0.9.6/robotcode/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/inspect.py` & `robotcode-0.9.6/robotcode/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/logging.py` & `robotcode-0.9.6/robotcode/utils/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/net.py` & `robotcode-0.9.6/robotcode/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/robotcode/utils/uri.py` & `robotcode-0.9.6/robotcode/utils/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode-0.9.5/setup.py` & `robotcode-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 {'': ['*']}
 
 install_requires = \
 ['robotframework>=4.0.0']
 
 setup_kwargs = {
     'name': 'robotcode',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'Language server, debugger and tools for Robot Framework',
-    'long_description': '# RobotCode\n\nAn [extension](https://marketplace.visualstudio.com/VSCode) which brings support for [RobotFramework](https://robotframework.org/) to [Visual Studio Code](https://code.visualstudio.com/), including features like IntelliSense, linting, debugging, code navigation, code formatting, test explorer, find references for keywords and variables, and more!\n\n## Requirements\n\n* Python 3.8 or above\n* Robotframework 4.0 and above\n* VSCode version 1.61 and above\n\n## Installed extensions\n\nRobotCode will automatically install [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python).\n\nExtensions installed through the marketplace are subject to the [Marketplace Terms of Use](https://cdn.vsassets.io/v/M146_20190123.39/_content/Microsoft-Visual-Studio-Marketplace-Terms-of-Use.pdf).\n\n## Features\n\nWith RobotCode you can edit your code with auto-completion, code navigation, syntax checking and many more.\nHere is a list of Features:\n\n- [Autocomplete and IntelliSense](#Autocomplete-and-IntelliSense)\n- [Code Navigation](#code-navigation)\n- [Diagnostics]()\n- [Diagnostics and Linting](#diagnostics-and-linting)\n- [Code Formatting](#code-formatting)\n- [Running and Debugging](#running-and-debugging)\n- [Multi-root Workspace folders](#multi-root-workspace-folders)\n- Test Explorer\n- and many more\n\n### Autocomplete and IntelliSense\n\nAutocompletion for:\n- Libraries with parameters\n- Resources,\n- Variables\n- Keywords with parameters\n- Namespaces\n\n![Autocomplete Libraries and Keywords](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/autocomplete1.gif)\n\nAutocompletion supports all supported variables types\n  - local variables\n  - variables from resource files\n  - variables from variables file (.py and .yaml)\n    - static and dynamic\n  - command line variables\n  - builtin variables\n\n![Autocomplete Variables](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/autocomplete2.gif)\n\n### Code Navigation\n\n- Symbols\n- Goto definitions and implementations\n  - Keywords\n  - Variables\n  - Libraries\n  - Resources\n- Find references\n  - Keywords\n  - Variables\n  - Imports\n    - Libraries\n    - Resources\n    - Variables\n- Errors and Warnings\n\n### Diagnostics and Linting\n\nRobotCode analyse your code and show diagnostics for:\n- Syntax Errors\n- Unknown keywords\n- Duplicate keywords\n- Missing libraries, resource and variable imports\n- Duplicate libraries, resource and variable imports\n- ... and many more\n\nFor most things RobotCode uses the installed RobotFramework version to parse and analyse the code, so you get the same errors as when you run it.\n\n\nGet additional code analysis with [Robocop](https://robocop.readthedocs.io/). Just install it in your python environment.\n\n### Code Formatting\n\nRobotCode can format your code with the internal RobotFramework robot.tidy tool (deprecated), but also with [Robotidy](https://robotidy.readthedocs.io/). Just install it.\n\n### Running and Debugging\n\nRobotCode supports running and debugging of RobotFramework testcases and tasks out of the box, directly from the definition of the test or suite.\n\n![Running Tests](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/running_tests.gif)\n\nIn the debug console you can see all log messages of the current run and navigate to the keyword the message was written by.\n\n### Multi-root Workspace folders\n\nRobotCodes support for [Multi-root Workspaces](https://code.visualstudio.com/docs/editor/multi-root-workspaces), enables loading and editing different Robotframework projects/folders with different RobotFramework/Python environments and settings at the same time or you can share the same RobotFramework/Python environment and settings for all folders in the workspace.\n\n\n## Quick start\n\n1. [Install a supported version of Python on your system](https://code.visualstudio.com/docs/python/python-tutorial#_prerequisites)\n(note: only Python 3.8 and above are supported)\n\n2. [Install a supported version of RobotFramwork on your system](https://github.com/robotframework/robotframework/blob/master/INSTALL.rst) (note: only RobotFramework 4.0 and above are supported)\n\n3. [Install the RobotCode extension for Visual Studio Code](https://code.visualstudio.com/docs/editor/extension-gallery).\n4. Open or create a robot file and start coding! 😉\n\n\n## Setting up your environment\n\nYou can alway use your local python environment, just select the correct python interpreter in Visual Studio Code.\n\n### With pipenv\n\nThis is the simpliest way to create an running environment.\n\n- As a prerequisite you need to install [pipenv](https://pipenv.pypa.io/) like this:\n\n    ```bash\n    python -m pip install pipenv\n    ```\n\n\n- Create your project directory (robottest is just an example)\n    ```bash\n    mkdir robottest\n    cd robottest\n    ```\n- Install robotframework\n    ```bash\n    python -m pipenv install robotframework\n    ```\n- Open project in VSCode\n- Set the python interpreter to the created virtual environment\n\n### Using Pre-Release Version\n\nStarting from VSCode version 1.63 it is possible to use pre-release versions of an extension. RobotCode uses recommend way for a version scheme, the major.EVEN_NUMBER.patch for release versions and major.ODD_NUMBER.patch for pre-release versions. RobotCode pre-release version will provide smaller changes or bugfixes maybe just one or two, and then all changes where collected to create a normal minor release with an even minor number.\n\nYou can select install pre-release version at installion via extensions view:\n\n![Extensions View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/install_prelease_extension_list.gif)\n\nOr you can switch between release and pre-release version in the RobotCode Extension Information view:\n\n![Extension Information View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/switch_release_prerelease.gif)\n\n\n## Customization\n\n### Editor Style\n\nYou can change some stylings for RobotFramework files in VSCode editor, independently of the current theme. (see [Customizing a Color Theme](https://code.visualstudio.com/docs/getstarted/themes#_customizing-a-color-theme))\n\nSee the difference:\n\n| Before                                                           | After                                                      |\n| ---------------------------------------------------------------- | ---------------------------------------------------------- |\n| ![Without customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/without_customization.gif) | ![With customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/with_customization.gif) |\n\n\nAs a template you can put the following code to your user settings of VSCode.\n\nOpen the user `settings.json` like this:\n\n<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> or <kbd>F1</kbd> or <kbd>CMD</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>\n\nand then type:\n\n`Preferences: Open Settings (JSON)`\n\nput this to the `settings.json`\n\n```jsonc\n"editor.tokenColorCustomizations": {\n    "textMateRules": [\n        {\n            "scope": "variable.function.keyword-call.inner.robotframework",\n            "settings": {\n                "fontStyle": "italic"\n            }\n        },\n        {\n            "scope": "variable.function.keyword-call.robotframework",\n            "settings": {\n                //"fontStyle": "bold"\n            }\n        },\n        {\n            "scope": "entity.name.function.testcase.name.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "entity.name.function.keyword.name.robotframework",\n            "settings": {\n                "fontStyle": "bold italic"\n            }\n        },\n        {\n            "scope": "variable.other.readwrite.robotframework",\n            "settings": {\n                //"fontStyle": "italic",\n            }\n        },\n        {\n            "scope": "keyword.control.import.robotframework",\n            "settings": {\n                "fontStyle": "italic"\n            }\n        },\n        {\n            "scope": "keyword.other.header.setting.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.variable.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.testcase.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.keyword.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.setting.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.comment.robotframework",\n            "settings": {\n                "fontStyle": "bold italic underline"\n            }\n        },\n        {\n            "scope": "constant.character.escape.robotframework",\n            "settings": {\n                //"foreground": "#FF0000",\n            }\n        }\n    ]\n}\n\n"editor.semanticTokenColorCustomizations": {\n    "rules": {\n        "*.documentation:robotframework": {\n            "fontStyle": "italic",\n            //"foreground": "#aaaaaa"\n        }\n    }\n}\n\n```',
+    'long_description': '# RobotCode\n\nAn [extension](https://marketplace.visualstudio.com/VSCode) which brings support for [RobotFramework](https://robotframework.org/) to [Visual Studio Code](https://code.visualstudio.com/), including features like IntelliSense, linting, debugging, code navigation, code formatting, test explorer, find references for keywords and variables, and more!\n\n## Requirements\n\n* Python 3.8 or above\n* Robotframework 4.0 and above\n* VSCode version 1.61 and above\n\n## Installed extensions\n\nRobotCode will automatically install [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python).\n\nExtensions installed through the marketplace are subject to the [Marketplace Terms of Use](https://cdn.vsassets.io/v/M146_20190123.39/_content/Microsoft-Visual-Studio-Marketplace-Terms-of-Use.pdf).\n\n## Features\n\nWith RobotCode you can edit your code with auto-completion, code navigation, syntax checking and many more.\nHere is a list of Features:\n\n- [Autocomplete and IntelliSense](#Autocomplete-and-IntelliSense)\n- [Code Navigation](#code-navigation)\n- [Diagnostics]()\n- [Diagnostics and Linting](#diagnostics-and-linting)\n- [Code Formatting](#code-formatting)\n- [Running and Debugging](#running-and-debugging)\n- [Multi-root Workspace folders](#multi-root-workspace-folders)\n- Test Explorer\n- and many more\n\n### Autocomplete and IntelliSense\n\nAutocompletion for:\n- Libraries with parameters\n- Resources,\n- Variables\n- Keywords with parameters\n- Namespaces\n\n![Autocomplete Libraries and Keywords](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/autocomplete1.gif)\n\nAutocompletion supports all supported variables types\n  - local variables\n  - variables from resource files\n  - variables from variables file (.py and .yaml)\n    - static and dynamic\n  - command line variables\n  - builtin variables\n\n![Autocomplete Variables](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/autocomplete2.gif)\n\n### Code Navigation\n\n- Symbols\n- Goto definitions and implementations\n  - Keywords\n  - Variables\n  - Libraries\n  - Resources\n- Find references\n  - Keywords\n  - Variables\n  - Imports\n    - Libraries\n    - Resources\n    - Variables\n- Errors and Warnings\n\n### Diagnostics and Linting\n\nRobotCode analyse your code and show diagnostics for:\n- Syntax Errors\n- Unknown keywords\n- Duplicate keywords\n- Missing libraries, resource and variable imports\n- Duplicate libraries, resource and variable imports\n- ... and many more\n\nFor most things RobotCode uses the installed RobotFramework version to parse and analyse the code, so you get the same errors as when you run it.\n\n\nGet additional code analysis with [Robocop](https://robocop.readthedocs.io/). Just install it in your python environment.\n\n### Code Formatting\n\nRobotCode can format your code with the internal RobotFramework robot.tidy tool (deprecated), but also with [Robotidy](https://robotidy.readthedocs.io/). Just install it.\n\n### Running and Debugging\n\nRobotCode supports running and debugging of RobotFramework testcases and tasks out of the box, directly from the definition of the test or suite.\n\n![Running Tests](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/running_tests.gif)\n\nIn the debug console you can see all log messages of the current run and navigate to the keyword the message was written by.\n\n### Multi-root Workspace folders\n\nRobotCodes support for [Multi-root Workspaces](https://code.visualstudio.com/docs/editor/multi-root-workspaces), enables loading and editing different Robotframework projects/folders with different RobotFramework/Python environments and settings at the same time or you can share the same RobotFramework/Python environment and settings for all folders in the workspace.\n\n\n## Quick start\n\n1. [Install a supported version of Python on your system](https://code.visualstudio.com/docs/python/python-tutorial#_prerequisites)\n(note: only Python 3.8 and above are supported)\n\n2. [Install a supported version of RobotFramwork on your system](https://github.com/robotframework/robotframework/blob/master/INSTALL.rst) (note: only RobotFramework 4.0 and above are supported)\n\n3. [Install the RobotCode extension for Visual Studio Code](https://code.visualstudio.com/docs/editor/extension-gallery).\n4. Open or create a robot file and start coding! 😉\n\n\n## Setting up your environment\n\nYou can alway use your local python environment, just select the correct python interpreter in Visual Studio Code.\n\n### With pipenv\n\nThis is the simpliest way to create an running environment.\n\n- As a prerequisite you need to install [pipenv](https://pipenv.pypa.io/) like this:\n\n    ```bash\n    python -m pip install pipenv\n    ```\n\n\n- Create your project directory (robottest is just an example)\n    ```bash\n    mkdir robottest\n    cd robottest\n    ```\n- Install robotframework\n    ```bash\n    python -m pipenv install robotframework\n    ```\n- Open project in VSCode\n- Set the python interpreter to the created virtual environment\n\n### Using Pre-Release Version\n\nStarting from VSCode version 1.63 it is possible to use pre-release versions of an extension. RobotCode uses recommend way for a version scheme, the major.EVEN_NUMBER.patch for release versions and major.ODD_NUMBER.patch for pre-release versions. RobotCode pre-release version will provide smaller changes or bugfixes maybe just one or two, and then all changes where collected to create a normal minor release with an even minor number.\n\nYou can select install pre-release version at installion via extensions view:\n\n![Extensions View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/install_prelease_extension_list.gif)\n\nOr you can switch between release and pre-release version in the RobotCode Extension Information view:\n\n![Extension Information View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/switch_release_prerelease.gif)\n\n\n## Customization\n\n### Editor Style\n\nYou can change some stylings for RobotFramework files in VSCode editor, independently of the current theme. (see [Customizing a Color Theme](https://code.visualstudio.com/docs/getstarted/themes#_customizing-a-color-theme))\n\nSee the difference:\n\n| Before                                                           | After                                                      |\n| ---------------------------------------------------------------- | ---------------------------------------------------------- |\n| ![Without customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/without_customization.gif) | ![With customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/with_customization.gif) |\n\n\nAs a template you can put the following code to your user settings of VSCode.\n\nOpen the user `settings.json` like this:\n\n<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> or <kbd>F1</kbd> or <kbd>CMD</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>\n\nand then type:\n\n`Preferences: Open Settings (JSON)`\n\nput this to the `settings.json`\n\n```jsonc\n"editor.tokenColorCustomizations": {\n    "textMateRules": [\n        {\n            "scope": "variable.function.keyword-call.inner.robotframework",\n            "settings": {\n                "fontStyle": "italic"\n            }\n        },\n        {\n            "scope": "variable.function.keyword-call.robotframework",\n            "settings": {\n                //"fontStyle": "bold"\n            }\n        },\n        {\n            "scope": "entity.name.function.testcase.name.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "entity.name.function.keyword.name.robotframework",\n            "settings": {\n                "fontStyle": "bold italic"\n            }\n        },\n        {\n            "scope": "variable.other.readwrite.robotframework",\n            "settings": {\n                //"fontStyle": "italic",\n            }\n        },\n        {\n            "scope": "keyword.control.import.robotframework",\n            "settings": {\n                "fontStyle": "italic"\n            }\n        },\n        {\n            "scope": "keyword.other.header.setting.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.variable.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.testcase.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.keyword.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.setting.robotframework",\n            "settings": {\n                "fontStyle": "bold underline"\n            }\n        },\n        {\n            "scope": "keyword.other.header.comment.robotframework",\n            "settings": {\n                "fontStyle": "bold italic underline"\n            }\n        },\n        {\n            "scope": "constant.character.escape.robotframework",\n            "settings": {\n                //"foreground": "#FF0000",\n            }\n        }\n    ]\n}\n\n"editor.semanticTokenColorCustomizations": {\n    "rules": {\n        "*.documentation:robotframework": {\n            "fontStyle": "italic",\n            //"foreground": "#aaaaaa"\n        }\n    }\n}\n\n```',
     'author': 'Daniel Biehl',
     'author_email': 'daniel.biehl@imbus.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/d-biehl/robotcode',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `robotcode-0.9.5/PKG-INFO` & `robotcode-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode
-Version: 0.9.5
+Version: 0.9.6
 Summary: Language server, debugger and tools for Robot Framework
 Home-page: https://github.com/d-biehl/robotcode
 License: Apache-2.0
 Keywords: Test,Testing,RobotFramework,Keyword Driven,Data Driven,Acceptance Testing,Acceptance Test Driven Development,BDD,Behavior Driven Testing,BDT,Robotic Process Automation,RPA,Language Server Protocol,Debug Adapter Protocol,Visual Studio Code
 Author: Daniel Biehl
 Author-email: daniel.biehl@imbus.de
 Requires-Python: >=3.8,<4.0
@@ -64,25 +64,25 @@
 Autocompletion for:
 - Libraries with parameters
 - Resources,
 - Variables
 - Keywords with parameters
 - Namespaces
 
-![Autocomplete Libraries and Keywords](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/autocomplete1.gif)
+![Autocomplete Libraries and Keywords](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/autocomplete1.gif)
 
 Autocompletion supports all supported variables types
   - local variables
   - variables from resource files
   - variables from variables file (.py and .yaml)
     - static and dynamic
   - command line variables
   - builtin variables
 
-![Autocomplete Variables](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/autocomplete2.gif)
+![Autocomplete Variables](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/autocomplete2.gif)
 
 ### Code Navigation
 
 - Symbols
 - Goto definitions and implementations
   - Keywords
   - Variables
@@ -116,15 +116,15 @@
 
 RobotCode can format your code with the internal RobotFramework robot.tidy tool (deprecated), but also with [Robotidy](https://robotidy.readthedocs.io/). Just install it.
 
 ### Running and Debugging
 
 RobotCode supports running and debugging of RobotFramework testcases and tasks out of the box, directly from the definition of the test or suite.
 
-![Running Tests](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/running_tests.gif)
+![Running Tests](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/running_tests.gif)
 
 In the debug console you can see all log messages of the current run and navigate to the keyword the message was written by.
 
 ### Multi-root Workspace folders
 
 RobotCodes support for [Multi-root Workspaces](https://code.visualstudio.com/docs/editor/multi-root-workspaces), enables loading and editing different Robotframework projects/folders with different RobotFramework/Python environments and settings at the same time or you can share the same RobotFramework/Python environment and settings for all folders in the workspace.
 
@@ -169,32 +169,32 @@
 
 ### Using Pre-Release Version
 
 Starting from VSCode version 1.63 it is possible to use pre-release versions of an extension. RobotCode uses recommend way for a version scheme, the major.EVEN_NUMBER.patch for release versions and major.ODD_NUMBER.patch for pre-release versions. RobotCode pre-release version will provide smaller changes or bugfixes maybe just one or two, and then all changes where collected to create a normal minor release with an even minor number.
 
 You can select install pre-release version at installion via extensions view:
 
-![Extensions View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/install_prelease_extension_list.gif)
+![Extensions View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/install_prelease_extension_list.gif)
 
 Or you can switch between release and pre-release version in the RobotCode Extension Information view:
 
-![Extension Information View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/switch_release_prerelease.gif)
+![Extension Information View](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/switch_release_prerelease.gif)
 
 
 ## Customization
 
 ### Editor Style
 
 You can change some stylings for RobotFramework files in VSCode editor, independently of the current theme. (see [Customizing a Color Theme](https://code.visualstudio.com/docs/getstarted/themes#_customizing-a-color-theme))
 
 See the difference:
 
 | Before                                                           | After                                                      |
 | ---------------------------------------------------------------- | ---------------------------------------------------------- |
-| ![Without customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/without_customization.gif) | ![With customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.5/doc/images/with_customization.gif) |
+| ![Without customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/without_customization.gif) | ![With customization](https://raw.githubusercontent.com/d-biehl/robotcode/v0.9.6/doc/images/with_customization.gif) |
 
 
 As a template you can put the following code to your user settings of VSCode.
 
 Open the user `settings.json` like this:
 
 <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd> or <kbd>F1</kbd> or <kbd>CMD</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>
```

