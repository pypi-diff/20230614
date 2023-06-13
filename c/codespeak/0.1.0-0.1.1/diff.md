# Comparing `tmp/codespeak-0.1.0.tar.gz` & `tmp/codespeak-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codespeak-0.1.0.tar", max compression
+gzip compressed data, was "codespeak-0.1.1.tar", max compression
```

## Comparing `codespeak-0.1.0.tar` & `codespeak-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,50 @@
--rw-r--r--   0        0        0        0 2023-06-10 22:32:57.535348 codespeak-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-10 22:32:57.535316 codespeak-0.1.0/codespeak/__init__.py
--rw-r--r--   0        0        0      274 2023-06-10 22:33:34.308966 codespeak-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 codespeak-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4797 2023-06-13 18:29:30.683863 codespeak-0.1.1/README.md
+-rw-r--r--   0        0        0     6148 2023-06-13 18:29:30.684245 codespeak-0.1.1/codespeak/.DS_Store
+-rw-r--r--   0        0        0      226 2023-06-13 22:08:40.406442 codespeak-0.1.1/codespeak/__init__.py
+-rw-r--r--   0        0        0     1375 2023-06-13 18:29:30.685025 codespeak-0.1.1/codespeak/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:29:30.685083 codespeak-0.1.1/codespeak/core/__init__.py
+-rw-r--r--   0        0        0     7137 2023-06-13 22:08:40.406870 codespeak-0.1.1/codespeak/core/code_generator.py
+-rw-r--r--   0        0        0     5738 2023-06-13 18:29:30.685471 codespeak-0.1.1/codespeak/core/codespeak_service.py
+-rw-r--r--   0        0        0     1430 2023-06-13 18:29:30.685635 codespeak-0.1.1/codespeak/core/diff.py
+-rw-r--r--   0        0        0     1395 2023-06-13 22:08:40.407101 codespeak-0.1.1/codespeak/core/executor.py
+-rw-r--r--   0        0        0     3048 2023-06-13 18:29:30.685940 codespeak-0.1.1/codespeak/core/openai_service.py
+-rw-r--r--   0        0        0     2723 2023-06-13 18:29:30.686115 codespeak-0.1.1/codespeak/core/prompt.py
+-rw-r--r--   0        0        0     4042 2023-06-13 18:41:04.484074 codespeak-0.1.1/codespeak/core/results_collector.py
+-rw-r--r--   0        0        0     2553 2023-06-13 18:29:30.686456 codespeak-0.1.1/codespeak/declaration/body_imports.py
+-rw-r--r--   0        0        0     5129 2023-06-13 22:08:40.407367 codespeak-0.1.1/codespeak/declaration/codespeak_declaration.py
+-rw-r--r--   0        0        0     6029 2023-06-13 22:08:40.407580 codespeak-0.1.1/codespeak/declaration/declaration_file_service.py
+-rw-r--r--   0        0        0     1714 2023-06-13 18:29:30.687033 codespeak-0.1.1/codespeak/declaration/declaration_helpers.py
+-rw-r--r--   0        0        0     2275 2023-06-13 22:08:40.407768 codespeak-0.1.1/codespeak/decorate.py
+-rw-r--r--   0        0        0       91 2023-06-13 18:29:30.687444 codespeak-0.1.1/codespeak/definitions/__init__.py
+-rw-r--r--   0        0        0     5649 2023-06-13 18:29:30.687657 codespeak-0.1.1/codespeak/definitions/classify.py
+-rw-r--r--   0        0        0      919 2023-06-13 18:29:30.687955 codespeak-0.1.1/codespeak/definitions/definition.py
+-rw-r--r--   0        0        0     1046 2023-06-13 18:29:30.688156 codespeak-0.1.1/codespeak/definitions/free_modules.py
+-rw-r--r--   0        0        0      491 2023-06-13 18:29:30.688390 codespeak-0.1.1/codespeak/definitions/types/builtin.py
+-rw-r--r--   0        0        0      671 2023-06-13 18:29:30.688578 codespeak-0.1.1/codespeak/definitions/types/custom_type_reference.py
+-rw-r--r--   0        0        0      497 2023-06-13 18:29:30.688778 codespeak-0.1.1/codespeak/definitions/types/generic.py
+-rw-r--r--   0        0        0      648 2023-06-13 18:29:30.688984 codespeak-0.1.1/codespeak/definitions/types/installed_class.py
+-rw-r--r--   0        0        0     2982 2023-06-13 18:29:30.689217 codespeak-0.1.1/codespeak/definitions/types/local_class.py
+-rw-r--r--   0        0        0     1195 2023-06-13 18:29:30.689426 codespeak-0.1.1/codespeak/definitions/types/local_class_as_self.py
+-rw-r--r--   0        0        0      476 2023-06-13 18:29:30.689642 codespeak-0.1.1/codespeak/definitions/types/none.py
+-rw-r--r--   0        0        0     1951 2023-06-13 18:29:30.689879 codespeak-0.1.1/codespeak/definitions/types/typing_type.py
+-rw-r--r--   0        0        0      634 2023-06-13 18:29:30.690067 codespeak-0.1.1/codespeak/definitions/types/union_type.py
+-rw-r--r--   0        0        0      560 2023-06-13 18:29:30.690265 codespeak-0.1.1/codespeak/definitions/utils/dedupe.py
+-rw-r--r--   0        0        0      557 2023-06-13 18:29:30.690455 codespeak-0.1.1/codespeak/definitions/utils/flat_uniques.py
+-rw-r--r--   0        0        0      276 2023-06-13 18:29:30.690644 codespeak-0.1.1/codespeak/definitions/utils/flatten.py
+-rw-r--r--   0        0        0      399 2023-06-13 18:29:30.690802 codespeak-0.1.1/codespeak/definitions/utils/group.py
+-rw-r--r--   0        0        0     1131 2023-06-13 18:29:30.690966 codespeak-0.1.1/codespeak/definitions/utils/swap_custom_types.py
+-rw-r--r--   0        0        0     1261 2023-06-13 18:29:30.691278 codespeak-0.1.1/codespeak/generate.py
+-rw-r--r--   0        0        0      632 2023-06-13 18:29:30.691432 codespeak-0.1.1/codespeak/generated_exception.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:29:30.691476 codespeak-0.1.1/codespeak/helpers/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-13 18:29:30.691686 codespeak-0.1.1/codespeak/helpers/gather_arguments.py
+-rw-r--r--   0        0        0      363 2023-06-13 18:29:30.691856 codespeak-0.1.1/codespeak/helpers/get_attr_from_qualname.py
+-rw-r--r--   0        0        0      529 2023-06-13 18:29:30.692022 codespeak-0.1.1/codespeak/helpers/self_type.py
+-rw-r--r--   0        0        0      388 2023-06-13 18:29:30.692180 codespeak-0.1.1/codespeak/helpers/set_attr_for_qualname.py
+-rw-r--r--   0        0        0      309 2023-06-13 18:29:30.692351 codespeak-0.1.1/codespeak/metadata/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-13 18:29:30.692500 codespeak-0.1.1/codespeak/metadata/digest.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:29:30.692545 codespeak-0.1.1/codespeak/static_cushion/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-13 18:29:30.692743 codespeak-0.1.1/codespeak/static_cushion/example_return.py
+-rw-r--r--   0        0        0       50 2023-06-13 18:29:30.692883 codespeak-0.1.1/codespeak/static_cushion/preserve_imports.py
+-rw-r--r--   0        0        0      500 2023-06-13 22:08:40.407903 codespeak-0.1.1/codespeak/unsafe_execute.py
+-rw-r--r--   0        0        0      396 2023-06-13 22:09:59.627989 codespeak-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 codespeak-0.1.1/PKG-INFO
```

